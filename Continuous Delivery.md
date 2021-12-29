After watching this video, you will be able to describe a CI/CD pipeline, define
continuous delivery, list the five key principles of continuous delivery, define
continuous deployment, and describe how DevOps manages risk.  Martin Fowler
defines Continuous Delivery as a software development discipline where you build
software in such a way that the software can be released to production at any
time. That’s easier said than done. Let’s start with what Fowler means by “In
order to be able to release to production at any time.” It means that the master
branch should always be deployable. In order to do that you need to build and
test every change. Building and testing every change which is the definition of
continuous integration, so continuous delivery requires continuous integration.
This may be why people simply say CI/CD like it is one word, because you need
continuous integration in place before you can implement continuous delivery.
You need a way to know if something will "break the build.” One way to
accomplish this is by delivering every change to a production-like environment.
It doesn’t have to be the actual production environment, but it should be enough
like it so that the same procedure can be used to deploy to production. Along
the way, there are automated gates that create a pipeline of checks such as unit
testing, integration testing, quality checks, vulnerability scans, and security
tests. These tests ensure the quality of the code. When this is all set up we
refer to it as a CI/CD pipeline. Like a pipeline, it is a set of tools where the
output of one feeds the input of another. Let’s talk about what is needed to set
up a CI/CD pipeline. To start off with, you need a code repository to host and
manage all your source code. That’s the starting point that initially feeds the
pipeline. Then you need a build server to build the application from source
code. Most cloud-based CI tools like Travis CI and GitHub Actions provide this
for you. Then you’ll need an integration server/orchestrator to automate the
build and run the quality and other tests. Most Cloud based CI/CD pipelines like
IBM Cloud Continuous Delivery will provide an orchestration capability for you.
You will also need an artifact repository to store binaries, the artifacts of
the application. This is where your Java jar and war files, Python wheels, Ruby
gems, Docker images, or whatever compiled artifacts have been tested and proven
to work. Finally, you will need a tool for the automatic configuration of your
deployment environment. Again, most cloud-based CI/CD pipeline tools will
provide a way to automate your deployment. When we overlay Continuous
Integration and Continuous Delivery on top of the software development
lifecycle, we can see that plan, code, build, and test are part of continuous
integration. And, release, deploy, and operate are part of continuous delivery.
These are the two cycles, CI and CD, that feed each other. There are five key
principles that are at the heart of Continuous Delivery. The first is built in
quality. The CI/CD pipeline comes into play here, because it allows every code
change to go through a set of rigorous checks to ensure high code quality. The
second principle is working in small batches. Working in small batches is
important because smaller changes are easier to test and represent less risk of
something getting broken. The third, it is important to acknowledge that
computers are good at performing repetitive tasks, but people-- not so much.
People are good at solving problems. It is best to automate the repetitive tasks
using computers and then leave the problem solving to the people. The fourth key
principle is to relentlessly pursue continuous improvement. We should always be
looking for ways to improve. That means that we need to measure, using
actionable measurements, and then take action when the measurement shows what we
can improve. Finally, the fifth key principle is that everyone is responsible.
When a build is broken, it is everyone’s responsibility to help fix the build.
Broken builds hold back everyone from moving forward. I wanted you to be aware
of the term “continuous deployment.” I wish they had called it “continuous
release” to distinguish the initials from continuous delivery. Continuous
deployment is reserved for deploying to production. You can see by this graphic
how continuous integration covers pushing code to version control and automating
the build and testing once it is integrated. Then continuous delivery takes
over, using the artifacts from the build, and automatically deploys them to some
environment. When we use automation to deploy to production, then it is referred
to as continuous deployment. Right about now you might be thinking to yourself,
“All of this automation sounds risky.” How do you manage that risk? DevOps
manages risk by increasing the rate of change rather than avoiding change. It
sounds counter intuitive, but here is how it works. In DevOps, deployment is
king, deployment should be painless. You want to deploy early and often. The
idea is to build up muscle memory. You deploy your code several times before it
goes to production. You deploy it to a development environment. You deploy it to
a test environment. You deploy it to a staging environment. You might deploy it
to a pre-production environment. Since these deployments are automated, by the
time you deploy it to production, you know that it works. It would be unusual
for it not to work because computers are really good at repetitive tasks. This
is why you don’t want humans involved doing manual steps. Once you automate
deployment, the code is going to go to production the same way every time. The
second notion is that deployment is decoupled from activation. This may sound
strange, but you can deploy code with something called a feature flag. Feature
flags turn your code on and off without having to redeploy. You can deploy a
feature, turn it on, and see how it works. If it is not working, turn it off. Or
if it is not ready, turn it off until it is ready, and then turn it on in
production. Feature flags have become very popular for decoupling deployment
from activation. You can also do waves of activation using blue-green deploys
and canary testing. This is where you deploy a new feature but only send 10% of
your traffic to it and monitor if it is working properly. Then you can then
gradually send a higher and higher traffic percentages to the new version until
you are happy that it is working and then send 100% of the traffic. Or if it is
not working properly, then roll it back. This is also known as “zero down-time”
deployment because at no time do you have the system take an outage. Right? You
don’t have to bring it down to deploy new code. Finally, deployment is not a
“one size fits all.” You need to see what works for the product you are building
and for what your customer expects. There are many techniques that can be
adopted to fit continuous delivery into your business scenario. In this video,
you learned that CI/CD pipeline tools provide a way to automate deployment.
Release, deploy, and operate are part of continuous delivery. The five key
principles of continuous delivery have to do with quality, working in small
batches, automation, continuous improvement, and shared responsibility.
Continuous deployment is when automation is used to deploy to production. DevOps
manages risk by increasing the rate of change rather than avoiding it.