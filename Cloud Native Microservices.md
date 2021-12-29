After watching this video, you will be able to recognize the impact of cloud
native microservices on application design, describe stateless microservices,
and compare monolithic and microservices architectures. To fully leverage
DevOps, you need to think differently about application design. You need to be
thinking about cloud native microservices. This image shows an application that
is designed as a collection of small microservices. Each one of these services
is independent of the others. Each service a particular domain of the
application. You may have gathered from the names of the services that this
example is a ride-sharing service. There are drivers, payments, trip management,
and notifications. These are all small services that are single-purpose based
around a business domain. Notice the lines going from one service to the other.
These are pointing to the REST APIs (representational state transfer
architectural style Application Programming Interface). No service is accessing
another service’s database. In fact, databases aren't even included in the
picture. This is a cloud native design using microservices. It is a collection
of stateless services. Cloud native means, "born on the cloud," taking advantage
of the horizontal scalability that the cloud has to offer. These services are
following the guidelines set forth in "The Twelve-Factor App," which describes
how cloud native applications should behave. This was first created in 2011 by
the Heroku team. Heroku was one of the first platform-as-a-service
implementations that paved the way for the cloud native platforms that we have
today. Applications are designed as a collection of stateless microservices.
Stateless doesn't mean that the application doesn't have a state. It means that
the services don't maintain the state, any hidden state. The state is persisted
in a database and each service maintains its own state in a separate database or
persistent object-store. Separation of state is important. If services were to
share state you wouldn't have microservices. You would just have a distributed
monolith. Resilience and horizontal scaling are achieved through deploying
multiple instances. Once you break your application down into multiple
independent services you can scale them independently as needed. For example, I
can scale up the notification service without scaling up the other services.
This takes advantage of the seamless, endless horizontal scaling of the cloud
platform. Instead of debugging and patching, failing instances are killed and
respawned. We often use the expression that instances are "cattle not pets."
Don't get too attached to your instances. We scale them out as needed and we
scale them back when not needed. Once you break up that application into lots of
little microservices, you need to leverage DevOps pipelines to help manage
continuous delivery of these services. The term microservice was coined by
Martin Fowler and James Lewis. They said, "…the microservice architectural style
is an approach to developing a single application as a suite of small services,
each running in its own process..." These are not just threads. These are full
processes running independently, "...and communicating with lightweight
mechanisms, often an HTTP resource." We now use REST APIs as these lightweight
mechanisms. Fowler and Lewis want on to say, "These services are built around
business capabilities and independently deployable by fully automated deployment
machinery." You saw that each service in the ride share application was built
around a business capability, such as driver service, passenger service, and
notification service. These services are independently deployable. For example,
I can upgrade the notification service without redeploying everything else. It
is particularly important that microservices enable everything to be
independently deployed. How does this work with a monolith compared to working
with microservices? Suppose you have a monolith that has calculations, copy
capabilities, and to-dos. When you deploy this application, you have to deploy
all the components together. We can split those out into multiple instances of
independent microservices. If I need to increase my capacity to perform
calculations, I can scale out those three instances and maybe make ten. I would
not have to scale out the to-dos or the copy capabilities. It's very important
to be able to scale them independently to make the best use of cloud resources.
Each microservice would have its own database where it is keeping track of its
own state. I could deploy them independently and change the database
independently. I would only need to change and coordinate with my team to
accomplish this because other services are using REST APIs to communicate. They
are not selecting over each other’s tables in the database. Suppose I am working
on an e-commerce website, which is a monolith, and I want to change the customer
table. I would probably need to coordinate with people on the order team and the
shipping team to change the customer table because they depend on it for orders
and shipping. With a microservice, there is no need to coordinate with other
teams because you are simply calling my REST API. You do not care what my table
looks like. You come in through the API. I could change from using a SQL
database to a NoSQL database and you would never know. You ask for customer data
and I give you customer data. That is the one difference between a monolith and
microservice architecture. With microservices, each service is loosely coupled
and communicates through a REST API. In this video, you learned Cloud native
architecture is a collection of independently deployable microservices.
Stateless microservices each maintain their own state in a separate database or
persistent object-store. Microservices are loosely coupled services, designed
for scalability and communicate with APIs.