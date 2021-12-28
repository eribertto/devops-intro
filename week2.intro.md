After watching this video, you will be able to: Describe social coding
principles and recognize how pair programming creates better code and better
programmers. What is social coding? I like to call it "Open Source for Inner
Source." Social coding is something that the open-source community has been
doing for years. What’s new is bringing these concepts into the enterprise and
coding as a community on internal projects. In the past, developers worked in
private repositories (repos) and you had to be a member of the team to
contribute. Everything was controlled by access control lists and a strict "need
to know" basis. The problem with that is no one knows that you're working on it,
so there is no possibility of reusing code because no one even knows it exists.
So, enterprises continually re-invent the wheel because no one knows the wheel
has already been built. With social coding, repositories are public, and
everyone is encouraged to fork the code and contribute. This is a hugely
different way of thinking. Development teams love to think "this is my code and
no one else can touch it" but they need to get over that for the good of the
company. You would think that anarchy would ensue, but actually, it works quite
well because it’s controlled by the repository owner. The person who owns the
repository is still in complete control of the contributions. What problem is
social coding solving? Let's say, you see a component, it’s 80% of what you
need, but there are some missing features. How do you add those missing
features? You now have a decision to make: Do you make a feature request to the
repo owner for a new feature and risk that your request will be at the bottom of
their priority list? Or worse, their funding gets cut, and your request will be
cut out first. Or do you rebuild 100% of the code just to get the 20% that you
need so as not to have a dependency on another team? It’s sad to report, but
many teams select the latter and re-invent the entire wheel just to get the
functionality they need. This is a huge waste of resources for any company, but
it happens all the time. How does adopting social coding principles solve this?
You discuss the new feature with the repo owner, and you agree to develop it for
them. This allows you to leverage everything that they've done and add the
feature that you need. You open up a GitHub Issue and you assign it to yourself
so that everyone knows you’re working on it. Then you fork the repo, create a
branch, and make your changes. When you’re all done and have something to
contribute back, then you issue a pull request signaling that you are ready for
a review and the repo owner can decide whether to merge your code back into the
main project. The repo owners are in full control. They can ask for changes
because they do the merge. They can ask that you write more test cases if you
don't have adequate test coverage. They treat you and your contribution like any
other member of the team. This is a win-win situation. You get to leverage
another team’s code and all the functionality that you need, and the other team
gets a feature added for free. The company saves money because code is being
reused instead of rewritten and everyone is happy. This is how open-source works
and this is how companies should treat their inner source. Pair programming is
an aspect of social coding that is taken from Extreme Programming. It consists
of two programmers sharing a single workstation (one screen, one keyboard, and
mouse between the pair). The programmer at the keyboard is usually called the
“driver.” The other programmer, also actively involved in the programming task,
but focused more on the overall direction, is called the “navigator.” While the
driver is typing, the navigator is checking their work, or perhaps looking
something up, or thinking about what's coming next. Then, after about 20 minutes
they swap roles. This way they both get to play each role. I pair program
whenever I can at work. I like this aspect of social coding. One of my personal
weaknesses is that I will agonize over what to call a new variable or function.
I want to get it perfect, to make the code as readable as possible. Having
someone else to bounce ideas off of helps me make those decisions faster. You
might think that pair programming is using twice the resources to get the same
amount of work, but it’s not like that. There are many benefits of pair
programming. The first benefit is higher code quality. There is something about
"programming out loud" that leads to a clearer understanding of the code. In the
past, when I wrote code, and I wrote it alone, and then when I explained it to
someone, I would pick up on a bug as I was talking out loud. I didn’t see the
bug when I was looking over the code in my head, but I saw it as I talked out
loud. Having to explain code to someone forces clarity. This means that defects
are found earlier. That's a good thing because it lowers the maintenance costs
right down the line. The later a defect is found in the process, the more it
costs to fix. Pair programming also forces skills transfer, creating better
programmers. I like to pair junior programmer developers with senior developers.
I do this all the time so that each one learns from the other’s approach to a
problem. They pick up tips and tricks that the other one uses. It creates better
programmers. You also get two sets of eyes on every line of code. You don't want
code that only one person understands. Then, that person goes on vacation, and
no one knows how to fix their code. Pair programming leads to a better
understanding of the code. More people understand the code well enough to fix
and enhance it. In this video, you learned that: Social coding is done
communally with public repositories and all team members are encouraged to
contribute. Pair programming results in higher quality code because defects are
found earlier, costs are lowered, and there is a broader understanding of the
codebase.