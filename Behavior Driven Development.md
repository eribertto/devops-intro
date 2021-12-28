After watching this video, you will be able to define behavior driven
development (BDD), explain how BDD can drive customer expectations, and describe
the key benefits of BDD. Behavior driven development (BDD), as its name implies,
focuses on the behavior of the system as observed from the outside in. This is
different from test driven development, which focuses on the minutia of how the
system works inside. BDD is great for integration testing to see if all of the
components are behaving together. It forces you to think "from the outside in.”
In other words, you implement only those behaviors that contribute most directly
to business outcomes. One of the advantages of BDD is that it describes
behaviors in a single notation, which is directly accessible to domain experts,
testers, developers, and customers. This improves communications across the
team. If we compare BDD to TDD we see that they are coming from opposite
directions. BDD describes the behavior of the system from the outside in. It is
looking at the system as a consumer of it would. While TDD tests the functions
of the system from the inside out. It is making sure that each component is
working correctly while BDD is making sure that they all work together at a
higher level. Put another way, BDD is ensuring that you are building the right
thing. Do you have the right set of capabilities and these behaviors? TDD is
ensuring that you are building the thing right. Does each feature perform the
task that it was intended to? The workflow starts with the developers, testers,
and customers exploring the problem's domain and collaborating to produce
concrete examples that describe the behavior they want. They document these
behaviors using a language known as Gherkin. It is a natural language
representation that I will talk about in a moment. Next, the team uses a BDD
tool like Behave for Python, or jBehave for Java, or Cucumber for Ruby, to run
these examples as automated acceptance tests. As the team works on the solution,
the BDD tool tells them which examples are implemented and working and warns
them about the ones that aren’t. Before you know it, you have one document that
is both the specification and the tests for your software. Gherkin is an
easy-to-read natural language syntax that uses a familiar Given... When...
Then... syntax. Gherkin is easily understandable by both technical and
non-technical people. If you're wondering where the name Gherkin came from, the
original tool that used this syntax was called Cucumber, and Gherkin is a pickle
and pickles are made from cucumbers. Tools have a way of producing funny names
like that. Here is how the Gherkin syntax is used. Given some context. This is
setting up the context or the precondition that sets the stage for the test. The
purpose is to put the system in a known state before the user (or external
system) starts interacting with it. When some event happens. This is the
principal action or actions that describe what is being performed. This is what
takes you from the initial state to the new observed state. Then some testable
outcome or behavior is validated. Then is used to observe the outcomes. The
observations should be related to the business value or the benefit of the
feature. And is used for continuations. Given this And that… Then this And that…
and so on. It gives you a natural way of adding more context, events, or
outcomes. Let's look at an example from a retail store. These are called feature
files or feature documents and you will have one feature per document and many
scenarios describing this feature. There is only one scenario in this example,
but there could be certainly more to cover all of the permutations. This feature
is called “Returns go to stock.” This feature is described by the behavior of
the system when a customer returns an item that they have purchased. Notice that
it uses the "As a," "I need," "So that" syntax; we use this in writing our user
stories. You can think of this as a user story with acceptance criteria, where
the acceptance criteria are the scenarios. This first scenario is called
“Refunded items should be returned to stock.” It reads as follows: Given that a
customer previously bought a black sweater from me, And I have 3 black sweaters
in stock, when they return the black sweater for a refund, Then I should have 4
black sweaters in stock. It's fairly straightforward. Your stakeholders should
be able to look at this and say, "Yes, this is how returning items to stock
works." Or maybe, "Here is another way it could happen." Then you would document
a new scenario for the "Returns go to stock" feature. The point is, your
stakeholders are actually helping you define the behavior of the system in a
formal syntax that you can now execute test cases against. Let me say that
again: You can actually execute test cases against this document. BDD tools like
Behave and Cucumber can consume this document with no further editing or
manipulation and execute test cases to prove that the system does indeed exhibit
the behavior. That will put a smile on your developer’s face. This is why I add
acceptance criteria to every user story. I use the Gherkin syntax to define that
acceptance criteria in the user stories that we write. There is no arguing over
the definition of "done" at the end of a sprint. It’s indisputable. The code
either does or does not exhibit this behavior. BDD improves communication among
the team members like developers, testers, product owners, and other
stakeholders. It leads to more precise guidance on how the system should behave.
It does this by providing a common syntax that is close to everyday language and
has a shallower learning curve compared to TDD tools. Tools targeting the BDD
approach generally afford the automatic generation of technical and end user
documentation from the BDD feature specification. Having clear behavior
visibility results in higher-quality code, which reduces the cost of maintenance
and eliminates the risk. Finally, with BDD acceptance criteria you are already
converted to user stories and test scenarios before the actual development.
Thus, automating test cases can start creating test processes even before the
product is tested. In this video, you learned that BDD focuses on the behavior
of the system from the outside in. It looks at the system as a consumer of it.
BDD uses an approachable syntax that everyone can understand. Key benefits of
BDD include improvement in communications, a common syntax, and acceptance
criteria for user stories.