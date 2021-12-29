After watching this video, you will be able to define infrastructure as code,
describe ephemeral infrastructure, and describe immutable delivery via
containers. Infrastructure as code is the practice of describing infrastructure
in textual format. I’m not talking about documentation here. I’m talking about a
textual format that is executable, otherwise known as code. You want to be able
to configure your infrastructure using a textual description that you can give
to a tool to execute. The tools that make this possible are called configuration
management systems. These are tools like Ansible, Puppet, and Chef that allow
you to describe your infrastructure as code, and then they create that
infrastructure and keep it in that state. You never want to perform system
changes on software configurations manually. This is not reproducible and is
extremely error prone. You want to use templates and scripts that describe how
to install and automatically configure elements such as systems, devices,
software, and users. Then you can take that textual code and store it in your
version control system so that you have a history of all of the changes. This
way everyone knows which version is the latest version and how the
infrastructure should look. Technology like Docker, Vagrant, Terraform, and even
Kubernetes, also allow you to describe your infrastructure as code, and this
code should be checked into version control. The reason this is so important is
because server drift is a major source of failure. Over time, servers get
updated for various reasons, and not always by the same people. This causes them
to drift from their original configuration. Sometimes the accumulation of these
changes cause failures in unpredictable ways. Even worse is having servers that
are supposed to be the same, but one of them keeps failing due to a
misconfiguration somewhere. The saying, “Servers are cattle, not pets,” refers
to how you treat servers. Suppose you have a thousand head of cattle. You don’t
take the time to give each one a name. When one gets sick you put them out of
their misery and replace them with another. Pets on the other hand? They're
lovingly cared for and nursed back to health when they are sick. The message is
to not lovingly hand-craft servers or spend too much time debugging when they
don’t work. You want to be able to replace them with an identical server that is
working properly. That means that you must think about your infrastructure as
something ephemeral or transient. It only exists for the time that you need it
and then you remove it when it’s not being used. For example, in the past,
building test environments took weeks. So, you would keep them around for months
because it took weeks to build them. But when you have infrastructure as code,
it takes minutes to deploy a new set of test servers. You can bring up a test
environment, use it for a period of time and then destroy it. If you need it
again another day, create a new one. You don’t keep it running forever. You just
bring it up when you need it and bring it down when you no longer need it. It's
transient. This also allows us to release through parallel infrastructure. For
example, I can build up a server that looks just like the one that is in
production. I can deploy a new version of an application or monitor it to see if
it’s working correctly. If it looks like it is behaving correctly, I shut down
the one in production, I make the new one the production server. With parallel
infrastructure I can keep things running constantly. Infrastructure as code
allows me to create identical infrastructure every time. Ephemeral
infrastructure can be used and then discarded because servers are built on
demand, via automation, using infrastructure as code techniques. Tools, such as
Docker, help us create immutable delivery. Docker is a packaging technology that
allows us to bring things up and bring them down in a consistent fashion, in an
isolated environment called a container. Docker supports infrastructure as code
by allowing you to specify how to build the image from code called a Dockerfile.
These Dockerfiles build the same image in the same way every time. Docker then
creates a container from that image in the same way every time it’s deployed.
This means that the same container that is running in production can be run on
the developer’s laptop. It is the ultimate development-production parity. This
is because all of the dependencies to run the application are packaged together
inside the container. This limits any variance or possible side effects. There
is nothing else needed except for the container runtime like Docker to run it
on. Tools like Docker also allow you to do rolling updates with immediate
roll-back. You are not installing the application to see if it works and then
uninstalling it if it doesn’t. You simply bring up a Docker container with the
new version. If it starts misbehaving, you stop it, bring it down, and bring up
the previous version which is already installed in its own container. It
literally takes seconds. You would treat containers that start misbehaving the
same way. You delete the container, and you create another one to take its
place. The new container is going to be exactly like the old one on the first
day it came up. If there was some kind of corruption, it is going to be clear
that corruption will bring the whole thing back to its original state. This is a
very different way of working. You never make changes to running containers like
you would a running server. Remember: “cattle, not pets.” You don’t patch
containers for vulnerabilities or modify them in any way. To make any change,
you make a change to the image that the container was created from. Then you
redeploy the new container to take the place of the old one. The reason is
simple: if you patch a container and it dies, the new one is brought up to take
its place, the new container won’t have the patches. That’s why it’s imperative
that you modify the image. They are the template for creating the containers and
they are the things that must be kept up to date, not the running containers. In
this video, you learned that infrastructure as code describes infrastructure in
an executable textual format. Ephemeral infrastructure can be used and then
discarded. Servers are built on demand, via automation. Rather than patching a
running container, immutable delivery is making changes to the container image,
then redeploying a new container.