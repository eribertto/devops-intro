After watching this video, you will be able to explain working in small batches
and recognize how single piece flow yields faster feedback Working in small
batches is a concept from Lean Manufacturing. It is important in situations
where fast feedback is required because it enables you to learn quickly from
your decisions.  You may be testing a hypothesis and you don't want to get too
far before you know if it's going to work. Working in small batches allows you
to experiment more, in order to quickly gain insights. In contrast, working in
large batches that take months to complete means that you don't get feedback for
months.  Working in small batches also minimizes waste. Because you gain
feedback faster and you don't waste time developing things your customer doesn't
like. Using large batches, you may spend months developing something that isn't
what the customer wanted.  In keeping with DevOps practices of cross-functional
teams and lightweight approaches, the best way to rapidly progress from
development through test and operations into production in a matter of minutes
is working in small batches. Let's take a look at an example of working in large
batches versus small batches. Let's say I need to mail out one thousand
brochures. The steps are to fold the brochures, insert the brochures into
envelopes, seal the envelopes, and then stamp the envelopes with postage. We
will use this brochure example to compare large batch and small batch execution.
Let's say that I'm going to process the first thousand brochures in batches of
50. These are large batches, with 50 brochures in each batch. Assume that each
step takes about six seconds to complete. So, I can do about 10 steps per
minute.  I start with the first step, which is folding. And at 10 per minute, it
takes me about five minutes to fold 50 of them. Then I move on to the next step.
The next step is inserting them all. I can do about 10 of them per minute, so it
takes me five more minutes, plus the five minutes from before. Now I'm 10
minutes into it.  Once I have them all folded and I insert it, I move on to the
next step, which is sealing them all.  If I’m sealing 10 per minute, I can do
another 50 in another five minutes.  So, I'm up to 15 minutes at this point in
wall clock time.  Finally, I get to step four, stamping, and it took me 16
minutes to get my first finished product.  This is the first time I have things
that I can actually inspect to check the quality.  What if the envelopes had no
glue? It would be 11 minutes before I figured out that something went wrong.
What if there's a typo on the brochure?  I have to go all the way back to the
beginning. So, this is very wasteful working in these large batches. Now let's
look at the same example with small batches using single piece flow. Again,
assume each step takes about six seconds to complete. With single piece flow, I
fold one, and put it into the envelope and seal it and put a stamp on it and the
first finished product is in about 24 seconds. Now I can inspect it, see if it
works, see if it's what I thought it was, and then let the rest of the flow
continue if it was acceptable. I received fast feedback in only 24 seconds
instead of 11 minutes with the large batch. What if the envelopes had no glue?
I would find out after 18 seconds. And if there was a typo in the brochure,
after 24 seconds. It’s very important that we don't work in large batches. We
need fast feedback, so that we can quickly pivot if we need to do something
different.  Working in small batches helps you implement other DevOps practices
like Continuous Integration and Continuous Delivery. So how do you know if your
batches are small enough? I would start with the size of your stories in your
backlog. Are your application features decomposed in such a way as to support
frequent releases? You have to ask yourself, how often are releases possible?
Are there delays in the release because the features are too large? Can features
be completed in a sprint?  If you have features that take several sprints, then
your batches are too large.  Optimally a feature should be small enough to be
completed in a week or less.  The features you build are one step toward a goal.
Many people feel that only a completed goal is worth shipping. Instead of
thinking of useful subsets that can be delivered in increments to gain feedback
toward the ultimate goal. In this video, you learned that working in small
batches means delivering something useful quickly. Using single piece flow leads
to faster feedback loops.