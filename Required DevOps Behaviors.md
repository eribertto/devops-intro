After watching this video, you will be able to differentiate between traditional
Ops and DevOps, describe ways Dev and Ops view each other, and list required
DevOps behaviors. DevOps presents diametrically opposed views to how traditional
enterprises think. Enterprises are built around end-to-end processes that see
"new" as complex, high risk, expensive, and time-consuming.  They approach
anything new as a one-time project to be completed in a fixed time frame for a
fixed budget and then move the people on to the next project.  DevOps seeks to
turn this on its head, breaking big projects down to deliver a continual series
of small changes that are more manageable. Smaller changes can be completed with
less risk, so DevOps reduces the risk of large projects. The catch is that small
changes cannot survive the traditional overhead that enterprises add to
everything you want to do.  Processes like change review boards don't work in
DevOps because they cannot move at the speed needed for small changes. We have a
clash of work cultures between traditional Ops and DevOps. In traditional Ops,
we make manual configuration changes to critical infrastructure. In DevOps, we
automate deployment to all environments. This is why traditional Ops needs
change review boards. Everything is done manually, and humans are fallible and
even if the change is approved, there is no guarantee that it will be
implemented correctly. In traditional Ops, application architectures are defined
by the network design. In DevOps, it is the other way around. Network design is
defined by the application architectures. We have software-defined networks that
conform to whatever the architecture needs. In traditional Ops, bespoke
infrastructure is built once and then maintained forever. In DevOps, ephemeral
infrastructure is created for new deployments. We don't maintain the
infrastructure.  We tear it down and replace it entirely. You can't do this
unless everything is automated.  The manual overhead would slow you down too
much. In traditional Ops, risk is managed through change windows. Changes are
only made at certain times, predesignated as change windows. That is, no change
can happen outside of those windows. In DevOps, risk is managed through
progressive activation. We can make a change to the system at any time.  We use
deployment techniques to activate or deactivate the change as needed.  Finally,
traditional Ops has a process biased toward “build once.” Traditional Ops builds
everything manually and maintains it forever, or at least until it's not needed
anymore, which is usually several years. Sometimes they build it once and can't
figure out how to build it again the same way because the build wasn't
documented.  In DevOps, processes are re-engineered for high volume, rapid
throughput of changes, making builds repeatable, leveraging Infrastructure as
Code to ensure that anything we do can be built again.  When cultures clash,
it's a no-win scenario. Development is measured by how much innovation
developers can produce. They keep up with the changing needs of the users by
developing and deploying new enhanced capabilities.  Operations wants stability.
They want to ensure that users can use those services and applications and that
their data and information are kept safe.  These two goals are in opposition.
You can't have both! Andrew Clay Shafer called this the "wall of confusion" that
exists between Dev and Ops.  What we need to do is break down that wall. The
first step is to change the way development and operations view each other. Ops?
Well... the Ops view of development is that development is throwing dead cats
over the wall. They manually implement changes.  They lack back-out plans and
lack testing. Their environments do not look like the production environments.
The Devs thinks Ops makes these all-or-nothing changes in the dead of night
during these change windows. They are furthest from code, so they don't
understand it. Ops is using cut and paste from runbooks, or Word documents.
Silos breed apathy.  You cannot have people working in two silos with
diametrically opposed metrics.  It is never going to work. You must bring these
people together.  You must give them one set of metrics that add value to the
customer.  If the website works, the developers get the praise.  If the website
is down, Ops gets the blame. Did I mention the no-win scenario?  This is not a
healthy working environment. Here are some required DevOps behaviors.  DevOps
turns a number of these things on their head.  You need to break down the
organizational silos and the handoffs that they cause and move to a culture of
shared ownership and high collaboration.  There is no hole on your side of the
boat. Everyone must see themselves as in this together for a common goal. You
must go from fear of change to managing risk by embracing change, managing
changes that are small.  Big changes are always scary to everyone. Make the
changes small and manage the change. Go from building something once, these
hand-crafted, snowflake servers where, each one is unique, and you can never
find another one just like it, to using ephemeral infrastructure deployed using
Infrastructure as Code techniques so that they are repeatable. Every time you
build a docker container, every time you build a virtual machine, build it
exactly the same. If you did not change the code, it will be built exactly the
same, and get the same results.  Change from manual fulfillment (ticket queues,
people manually doing things) to enabling automated self-service. I've seen
companies adopt the cloud and then put a ticket queue in front of it so that
only IT people can provision from the cloud.  That defeats the whole purpose of
having a self-service cloud.  Self-service is the way to move quickly. Finally,
you must change from alarms, callbacks, and escalations to fast feedback loops
that are data-driven.  Make sure you can get that information about what is
going wrong in production and then react to it when you need to. These are the
behaviors that must change in order for you to fully become a DevOps
organization. In this video, you learned that enterprises see change as complex
and time-consuming. DevOps breaks big projects into a series of small,
manageable changes. Traditional Ops builds once and maintains. In DevOps,
ephemeral infrastructure is created for each new deployment. Dev wants
innovation, while Ops wants stability.  Required DevOps behaviors include shared
ownership, collaboration, embracing change, and data-driven responses.