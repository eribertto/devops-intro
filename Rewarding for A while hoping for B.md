After watching this video, you will be able to explain the importance of
measuring what you want to improve, identify the value of social and DevOps
metrics, and recognize that DevOps changes your approach to problem resolution.
How do you change a culture? This is from a paper by Steven Kerr from the
Academy Management Journal back in 1975 on “The folly of rewarding for A, while
hoping for B.” “Whether dealing with monkeys, rats, or human beings, it is
hardly controversial to state that most organisms seek information concerning
what activities are rewarded, and then seek to do (or at least pretend to do)
those things, often to the virtual exclusion of activities not rewarded. The
extent to which this occurs, of course, will depend on the perceived
attractiveness of the reward offered, but neither operant nor expectancy
theorists would quarrel with the essence of this notion.” You cannot measure for
A and hope you get B. It’s not going to happen because you get what you measure.
So, measure what matters. If you measure widget production, you will get lots of
widgets. If you measure lines of code, you will get many lines of code.
Semicolons all the way down. We used to measure lines of code by the thousands
of lines of code (KLOC). Is it good code? I do not know; I do not care. I am
measured by how many lines of code I write, so I am going to write verbose code.
Remember, you get what you measure. If you measure people by ranking them
against each other, you will get antisocial behavior. A lot of companies do
this—they rank people. So, let me get this straight. You want me to help my
peer, but you are going to rank us against each other? So, I help them so that
they get a better ranking than me, then they get the pay raise or the promotion
that I want? Yeah, how does that work? Companies do this all the time, and their
management doesn’t seem to get it. You get what you measure. If you want people
to be social, then you must measure them on being social. You should measure
developers by their social interactions and sharing of code and knowledge. That
is how you get social coders. Here are two metrics that I like to use to measure
social coders. Who is leveraging the code you are building? Are you building
code that the rest of the company or open-source community find valuable enough
to reuse in their solutions? But that’s only half of the puzzle. That will get
people thinking about how they can make their code valuable to others. But you
need the second metric. Whose code are you leveraging? Are you wasting all of my
development dollars reinventing wheels or are you leveraging the existing wheels
and only building the bespoke parts that don’t exist? Both of these metrics are
needed because they incentivize both sides to share their code and reuse each
other’s code because… you get what you measure. You need a social metric to get
social behavior. DevOps is all about continuous improvement. That means that you
must know where you are coming from in order to measure if you are going in the
right direction. It starts with taking a baseline. What do you want to improve?
Maybe it currently requires six team members 10 hours to deploy a release of
your product. Maybe it costs X dollars for every release. Whatever that
measurement is, that’s the baseline. Then you need to create a goal. Metric
goals allow you to reason about these numbers and judge the success of your
progress. Perhaps you want to reduce deployment time from 10 hours to 2 hours.
That’s a very achievable goal. Your baseline determines that it takes 10 hours,
so you aim for a threshold of fivefold improvement to 2 hours. Or maybe you want
to go from needing 6 team members to one team member. Or maybe you want to
reduce the number of defects found in production. Whatever it is, choose a goal
and work on one at a time. Then you judge the success of your process. Did you
go from 10 hours to 2 hours? No? Try something different until you achieve this
measurement. Then you start working on the next goal. DevOps changes the
objective. We used to measure mean time to failure where you tried to make sure
the server never went down. That is old-school thinking. We need to go from mean
time to failure to mean time to recovery. You anticipate that the server will go
down. Just be sure you can recover quickly. If your applications are built as a
collection of microservices deployed in containers as multiple instances, you
can recover quickly by bringing up a new container. And your customer might
never even know that the service went down because there was no single point of
failure. Containers may be continuously going up and down, but if you can
recover quickly by spinning up a new container, who cares it went down? The
customer never noticed. It’s a whole new way of thinking about availability. In
this video, you learned that you should measure and reward what you want to
improve. Measuring social metrics leads to improved socialization and measuring
DevOps metrics allows you to see the progression toward goals. DevOps changes
the objective of problem resolution from failure prevention to failure recovery.