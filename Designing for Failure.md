After watching this video, you will be able to recognize the importance of
embracing failure, explain the importance of quick recovery from failure,
describe how retry patterns, circuit breaker patterns, and bulkhead patterns
help make applications resistant to failure, and describe chaos engineering.
Once you design your application as a collection of stateless microservices,
there are a lot of moving parts, which means that there is a lot that can go
wrong. Services will occasionally be slow to respond or even have outages so you
can’t always rely on them being available when you need them. Hopefully, these
incidents are very short-lived, but you don’t want your application failing just
because a dependent service is running slow or there is a lot of network latency
on a particular day. This is why you need to design for failure at the
application level. Since failure is inevitable, you must build your software to
be resistant to failure and scale horizontally. We must design for failure. We
must embrace failure. Failure is the only constant. We must change our thinking,
from moving from how to avoid failure to how to identify failure when it
happens, and what to do to recover from it. This is one of the reasons why we
moved DevOps measurements from “mean time to failure” to “mean time to
recovery.” It’s not about trying not to fail. It’s about making sure that when
failure happens, and it will, you can recover quickly. Application failure is no
longer purely an operational concern. It is a development concern as well. For
the application to be resistant or resilient, developers need to build that
resilience right in from the start. And because microservices are always making
external calls to services that you don’t control, these services become
especially prone to problems. Plan to be throttled. You're going to pay for a
certain level of quality of service from your backing services in the cloud, and
they will hold you to that agreement. Let’s say you pick a plan that allows 20
database reads per second. When you exceed that limit, the service is going to
throttle you. You are going to get a 429_TOO_MANY_REQUESTS error instead of
200_OK and you need to handle that. In the case, you would retry, right, in this
case. This logic needs to be in your application code. When you retry, you want
to back off exponentially when it fails. The idea is to degrade gracefully. If
you can, cache where appropriate so that you don’t always have to make these
remote calls to these services if the answer isn’t going to change. There are a
number of patterns that are important strategies to help you make applications
resilient. I just want to go over a few of the popular ones. The first one is
the retry pattern. This enables an application to handle transient failures when
it tries to connect to a service or a network resource, by transparently
retrying and failing the operation. I've heard developers say that you must
deploy the database before you start my service because it expects the database
to be there when it starts. That is a fragile design, which isn't appropriate
for cloud native applications. If the database is not there, your application
should wait patiently and then retry again. You must be able to connect, and
reconnect, and fail to connect and connect again. That is how you design robust
cloud native microservices. The key here is the retry pattern, to back off
exponentially, and delay longer in between each try. Instead of retying 10 times
in a row and overwhelming the service, you retry, it fails. You wait one second
and you retry again. Then you wait 2 seconds, then you wait 4 seconds, then you
wait 8 seconds. Each time you retry, you increase the wait time by some factor
until all of the retries have been exhausted and then you return an error
condition. This gives the backend service time to recover from whatever is
causing the failure. It could be just temporary network latency. The circuit
breaker pattern is similar to the electrical circuit breakers in your home. You
have probably experienced a circuit breaker tripping in your house. You may have
done something that exceeds the power limit of the circuit and it causes the
lights to go out. That’s when you go down to the basement with a flashlight and
you reset the circuit breaker to turn the lights back on. This circuit breaker
pattern works in the same way. It is used to identify a problem and then do
something about it to avoid cascading failures. A cascading failure is when one
service is not available, and it causes a cascade of other services to fail.
With the circuit breaker pattern, you can avoid this by tripping the breaker and
having an alternate path return something useful until the original service
recovers and the breaker closes again. The way it works is that everything flows
normally as long as the circuit breaker is closed. The circuit breaker is
monitoring for failure up to a certain limit. Once it reaches that limit
threshold, right, that certain threshold, the circuit breaker trips open, and
all further calls to the circuit breaker return with an error, without even
calling the protected service. Then after a timeout, it enters this half-open
state where it tries to communicate with the service again. If it fails, it goes
right back to closed. If it succeeds, it becomes fully open again. The bulkhead
pattern can be used to isolate failing services to limit the scope of a failure.
This is a pattern where using separate thread pools can help to recover from a
failed database connection by directing traffic to an alternate thread pool
that’s still active. Its name comes from the bulkhead design on a ship.
Compartments that are below the waterline have walls called “bulkheads” between
them. If the hull is breached, only one compartment will fill with water. The
bulkhead stops the water from affecting the other compartments and sinking the
ship. Using the bulkhead pattern isolates consumers from the services as
cascading failures by allowing them to preserve some functionality in the event
of a service failure. Other services and features of the application continue to
work. Finally, there is chaos engineering, otherwise known as monkey testing.
While not a software design pattern, it is a good practice to prove that all of
your design patterns work as expected under failure. In chaos engineering, you
deliberately kill services to see how other services are affected. Netflix has a
suite of failure-inducing tools called The Simian Army. Chaos Monkey solely
handles termination of random instances. Netflix randomly kills things to see if
they come up and whether the system will recover gracefully. You cannot know how
something will respond in a failure in production until it actually fails in
production. So, Netflix does this on purpose. All of these patterns can help you
build more robust software and respond gracefully to intermittent failures. In
this video, you learned that failure is inevitable, so we design for failure
rather than trying to avoid failure. Developers need to build in resilience to
be able to recover quickly. Retry patterns work by retrying failed operations.
Circuit breaker patterns are designed to avoid cascading failures. Bulkhead
patterns can be used to isolate failing services. Chaos engineering is
deliberately causing services to fail to see how other services are affected.