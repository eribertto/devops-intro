After watching this video, you will be able to: describe problems with the
Waterfall method and describe the typical relationship between software
development and operations prior to DevOps. It's important to understand what
brought us to DevOps in order to fully appreciate the problem that it solves.
Architects would spend months and months designing the system on paper, creating
requirements documents, creating design documents, and making high-level
designs, and low-level designs, and system level designs. Then finally we would
get to a development phase, where development worked for months on features in
an isolated development environment. As they developed the code, if the designs
were wrong it was very expensive to go back to the architects. Once we developed
all the code, we would get to a testing phase. We would test all the code at
once. Testing would open defects and send the code back to development until no
more severity 1 or 2 defects were found. At some point, development would
release the code to operations for deployment. This release for deployment would
happen several months after the code was written, maybe even a year later. Some
of these projects took up to two years. Then the operations team would take what
seemed like forever to deploy it because they had no idea what the developers
had built. And the operations team kept it running from that point on. We call
this way of working the Waterfall method. With Waterfall, everything happens in
phases. Requirements are gathered and a requirements document is generated. Then
that phase ends. The artifacts for that phase flow down into the next one. In
the next phase, we do all the design and the design is documented in high-level
designs, low-level designs, system-level designs, and then that phase ends.
Those artifacts get passed down to the next phase and the coding begins where
developers take the low-level design documents and write the code that
implements those designs. There are entrance and exit criteria to each of the
phases. So, all along, we're coding in isolation, we're not integrating my
module with the next person's module. Finally, you get to the integration phase
when all those modules come together. This is the first time we realize, we
don’t know whether all these pieces even work together. And then we move on to
the testing phase, because now we've got a system that people can test. And as
they find bugs, they must go swim back, up the waterfall, and open some bugs in
the coding phase and do some re-coding. Finally, after all the testing, we
deploy the software. It is called Waterfall because if there is a problem, it is
very hard to go back, like trying to swim up a waterfall. You have to go all the
way back to the design phase. In fact, because we treat software development
like civil engineering projects, sometimes some of those architects have moved
on to the next project, and you've got to go find them and then get them to
change the design. You get the developers to change the code and hope that it
integrates this time. This process was very error prone and there was no room
for making changes late in the process. You didn't know whether it worked until
the end, so it was very high risk. But we developed software like this for
years. What is wrong with this approach?  Well, there's no provision for change.
Every phase has entrance and exit criteria. When one phase ends, the next one
begins. There's just no provision for going back and changing the design or
changing the requirements or anything like that. Another problem is that you
don't know if it works until the end. There is no intermediate delivery. Nothing
is delivered, until that last step, when we give it to the operations team and
say, go deliver this thing into production. In addition, with each phase, there
are issues that are just passed down. And, of course, every one of these is an
opportunity to lose information, and to have a mishap. People get blocked,
because they can't accept the work from the previous phase.  Then the next phase
is delayed. Mistakes that are found later on are very, very costly, it is
especially costly to find something that's designed wrong in the testing phase
and go all the way back and redesign it. Finally, these delays create long lead
times between deliveries. Also, the overall problem with Waterfall is that teams
are working separately, and they're unaware of their impact on each other.
Designers are unaware of the impact on the code, and the coders are unaware of
their impact on testing or the impact on integration before we get all the code
together. Everybody is working in their silos for their phase. And the scariest
thought is that the people who are furthest away from the code, the poor
operations team, have to deploy it, run it, and manage it in production. They
know the least about the code, and they're the ones expected to run it. In this
video, you learned that: Traditional Waterfall development creates problems such
as delays, frustration, long lead times, expensive late changes, and operations
managing unfamiliar code. And that in the past, software developers and
operations worked in silos, rather than working together.