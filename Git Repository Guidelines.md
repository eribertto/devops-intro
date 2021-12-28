After watching this video, you will be able to explain how the Git Feature
Branch Workflow supports social coding. Let's talk about guidelines for your
repositories and workflow. Create a repository for every component whether it’s
a microservice or something else you’re building. Don't put multiple
microservices in one repository. Those are called mono repos and are frowned
upon.  People often create what we call a “mono repo” which is a single repo
with multiple microservices in it to make demonstrations easier, but this should
not be done for production code.  You don't want someone to have to check out a
lot of code that they don't care about just to get to the code that they do care
about. You want to have one component or microservice per repo. This is very
important.  Don't be afraid to have multiple repos. Create a new branch for
every issue that you’re working on. You don't want to have long-lived branches.
I don’t believe in having a "development" branch that all the work gets merged
into and done.  That's the old way of thinking. Branches are very lightweight in
Git.  There’s a master branch, and there are feature branches and that's all
there is.  When you're done with the feature branch you delete it.  Don't get
too attached to it, because you delete it and create a new one for the next
issue you’re working on. Use pull requests to merge your code back to master.
The only way code should get into the master branch is through a pull request. A
pull request gives an opportunity for other people to look at your code and
review it. Never merge your own pull request.  Don't do it! You always want to
have someone else on the team merge your pull request because every pull request
is an opportunity to have a code review. Have them look at the code, make sure
it makes sense to them, and then have them do the merge. This way you get two
sets of eyes on all the code that's going into the repository. We call this the
Git Feature Branch Workflow and here is how it works. Let’s begin with the
GitHub Repo.  You create a new repository for your component or, if you’re
contributing to someone else’s component, you fork an existing repository. Next,
you clone that down to your workstation and it becomes your local repository.
All of your changes will be made in this repository. Next, you create a branch
to work on your feature.  This can also be followed for bugs or other fixes. It
is called a feature branch, but the idea is that it’s the branch for the code
that is associated with the GitHub Issue that you’re working on. When you are
ready to submit your code back to the main project, or if you just want someone
to review your changes to get feedback, you push your code to a remote branch.
Finally, you create a pull request to request that your changes be reviewed. The
pull request will be reviewed and if the code is complete and meets the
standards set out by the team, it will be merged back into the master branch and
become part of the original GitHub repository.  In this video, you learned that:
In this video, you learned that creating a repository for every component,
following the Git Feature Branch workflow, then creating branches, and using
pull requests is a good practice.