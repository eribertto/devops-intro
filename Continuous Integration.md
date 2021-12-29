After watching this video, you will be able to describe Continuous Integration
and Continuous Delivery, explain the reason for using small batches in
Continuous Integration, and describe the benefits of Continuous Integration.
People use the acronym CI/CD as if it is one thing, but Continuous Integration
and Continuous Delivery are two separate and distinct practices.  Continuous
Integration (CI) is the process of continuously building, testing, and
integrating every developer change into the master branch after a set of tests
have passed.  The result is potentially deployable code. Continuous Delivery
(CD) is a series of practices designed to ensure that code can be rapidly and
safely deployed to production by delivering every change to a production-like
environment. Notice that I said “production-like.” It doesn’t have to be
deployed into production and, in fact, many people reserve the term “Continuous
Deployment” for when you are deploying continuously to production.  You just
have to deploy it somewhere like a development, test, or staging environment
that mimics the production environment. For example, if the production
environment is containers running on Kubernetes, you should deploy to a
development environment in containers on Kubernetes. Let’s start by looking at
how traditional development is done. Developers work in long-lived development
branches. Typically, they do it this way because older version control systems
made a complete copy of the code whenever you made a branch, so making branches
was very expensive. The cost causes people to resist making branches and when
they do, they don’t delete very them often. With modern version control systems,
like Git, this is no longer the case. But some development teams have kept the
traditional practice. These development branches are kept separate from the
release branches and, periodically, merged into a release branch, but not
without lots of breakage. This is because the amount of changes made over a long
period of time, make the branch more vulnerable to merge conflicts. Builds are
run periodically, sometimes nightly, on the release candidate branch.
Developers continue to add to the development branch, which drifts further and
further from the master release branch. In this scenario, it may take days to
merge the code to get it back working. In contrast, Continuous Integration is a
development practice that requires developers to frequently integrate code into
a shared repository, and by frequently, I mean daily, if possible.  This is
accomplished by having developers work in short-lived feature branches that are
merged into the master once the feature is complete. This means you integrate
each feature as it is completed. You don’t wait until a long list of features
are complete before you integrate them. Each check-in is then verified by
automated testing and an automated build, allowing teams to detect problems
early and often. Once merged, the branch is then deleted, and a new branch is
created for the new feature. Working in small batches helps accomplish
Continuous Integration. By committing regularly, every developer can reduce the
number of conflicting changes because less time has passed between merges.  The
more time that passes, the greater the risk of merge conflicts.  Working for a
week on the code and then checking it all in at once increases the risk of that
the new features will conflict with other features. These conflicts can be
difficult and time-consuming to resolve. Using pull requests allows team members
to communicate about the change they are making. Every pull request is an
opportunity for a code review, so that other developers review the code. This
ensures that all of the code is being looked at by more than one person and
lowers the risk of something going wrong.  Committing all changes at least once
a day, or once per feature build, is generally considered part of a definition
of Continuous Integration. Speaking of pull requests, every pull request should
be built and tested. This should happen automatically.  The system should build
changes of the current working version to verify that the integration works
correctly. A common practice is to use automation, in which a CI tool monitors
the revision control system and then automates and runs the build automatically.
Most CI tools like Travis CI, Circle CI, Jenkins, and GitHub Actions have the
capability to monitor your version control system for changes as well as
automate the build process. Once the code is built, all tests should be run to
confirm that the code behaves the way the developers expect it to.  In other
words, make the build self-testing. The test results should feed back to the
pull request, and you should never merge a pull request that has failing tests.
One of the benefits of practicing Continuous Integration is that you can get
faster reaction time to changes and you can move faster. You can move faster
because your tests are automated. Since the tests are automated you know that
everything you have done up to that point has been tested and known to work.  If
you have these tests run automatically, you’re not wasting time testing; you’re
spending your time building features. CI reduces the risk of integrating code
because you are integrating smaller changes. When things change less, there is
less risk of breakage due to changes. Submitting pull requests puts more eyes on
the code and therefore results in higher code quality. Everyone has input on the
quality of the code.  Finally, you know that the code that is in version control
works.  Remember, the master branch should always be deployable.  I’ve had
students ask me, “Can I write the test case after I build the user interface?”
And I tell them, that by that time it is too late. You have committed the user
interface to the master branch and if we need to deploy the master branch, we
have no idea if the user interface works. You should assume that code that has
not been tested does not work. You should never merge untested code into the
master branch. The master branch should always be deployable. In this video, you
learned that Continuous Integration is building, testing, and integrating every
change into the master branch after tests have passed. Continuous Delivery
ensures that code can be rapidly and safely deployed to production by delivering
every change to a production-like environment. Working in small batches aids
continuous integration by reducing the number of conflicting changes.  The
benefits of Continuous Integration include faster reaction time, moving faster,
and reducing the risk of integrating code.