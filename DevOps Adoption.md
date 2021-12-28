After watching this video, you will be able to: Describe how major companies are
embracing DevOps and recognize that DevOps requires a cultural change. DevOps
takes a completely different mindset so you must first unlearn what you have
learned. To really embrace the culture of DevOps you must unlearn your current
culture. It is easier said than done. For companies that are startups who are
not steeped in enterprise culture, it is easier. New startups begin with a new
culture, but the big enterprise businesses must unlearn what they have learned
and change their ways. This is extremely difficult to do. But consider this:
What if you could fail fast and rollback quickly? You could limit your blast
radius of a change. You could put something out into production and if it goes
wrong, it doesn't bring the whole system down by limiting the blast radius of
that change. What if you could test in market instead of second-guessing and
analyzing? Companies do this all the time. They will be A/B testing and you will
say to your friend, “Hey, did you see that widget on the website? You click on
that thing in and it...” And your friend is looking at you like, “What are you
talking about?” Your friend didn’t see it, they didn’t see any widget. Your
friend doesn’t see it because the site was A/B testing. You were in the A group,
they were in the B group. They did not get to see that new widget. Companies
take a subset of their customers and show them something new and see how they
react, instead of trying it out on everyone. This is testing in market and it
can be very powerful. What if you had an application design that allowed you to
change individual components to be replaced? You wouldn’t have big bang
releases. This is how apps like Spotify are designed. Spotify is not just one
big monolithic app. It is a bunch of little microservices. They have a
recommendation engine, it's a microservice that shows up on the app. If they
want to roll out a new recommendation algorithm, that team can roll that new
recommendation out without affecting any other part of the app. It might make
totally wacky recommendations, but it’s not bringing the whole Spotify service
down. You just get some recommendations that seem a little ridiculous, but you
are listening to your music. What do you care? These are things that enable you
to move fast in market. In 2009, at the Velocity conference, it opened a lot of
people's eyes. John Allspaw and Paul Hammond gave their now famous presentation
at the Velocity 2009 conference, entitled "10+ Deploys per day – Dev and Ops
Cooperation at Flickr". Allspaw was at Flickr at the time, and he talked about
how they are doing 10 deploys per day and people's heads exploded - 10 deploys
per day! They were happy if they could just get a deploy out every six months.
But they were not deploying all of Flickr 10 times a day. People did not realize
this at first. They had a different application design. They were deploying
little pieces. This opened a lot of people's eyes to the possibility of what
could be if Dev and Ops worked together to move things out instead of Ops being
the gate for Dev. In that talk, they said that in the last week there were 67
deploys of 496 changes by 18 people at Flickr. And that was back in December of
2008. In January 2011, Etsy talked about deploying to production 517 times that
month. What they actually said was that in January 2011, a month, they had over
a billion views, their code was committed by 76 unique individuals and deployed
to production a total of 517 times. I did a little back of the napkin
calculation and estimated that they are deploying every 25 minutes. People were
looking at this and saying, “How are they doing it?” Chad Dickerson was the
Chief Technical Officer of Etsy. He said that Etsy’s deployment environment
requires a lot of trust, transparency, communication, and discipline across the
teams. He and his teams, working together for a common goal, not working against
each other in silos. You might think these are mythical companies, right? These
are the sparkly unicorns. You could never do this in a big enterprise. No way,
no how. Enterprises cannot change and move that fast. They just cannot do it. It
won’t happen. Then in 2016 at the DevOps Enterprise Summit, which had 1,300
attendees, Gene Kim from IT Revolution, and author of The Phoenix Project, began
outlining where the industry stands and what is driving DevOps adoption in the
enterprise. You had major companies, like Ticketmaster, Nordstrom, Target, USAA,
ING. Major retail companies, insurance companies, banks… standing up and singing
the praises of DevOps. This is when other enterprises started to notice this
"DevOps thing" was not just for startups. It actually works in big enterprises.
Ticketmaster talked about 98% reduction in mean time to recovery. Traditional IT
is measured in mean time to failure, but DevOps is all about mean time to
recovery. Stuff is going to fail. How quickly can you recover is the question?
Nordstrom had achieved 20 percent shorter lead times. Target’s full stack deploy
went from three months to minutes. Obviously, they did a lot of automation.
Sometimes that three months is not all work. Sometimes the three months is
having to go before a change review board, and they only meet the first Tuesday
of every month and today is the Wednesday after that Tuesday, so I have to wait
another whole month to get something reviewed. This is how big corporations
work. If you want to move faster, you have to break down those barriers and to
push changes faster. USAA releases went from 28 days to 7. That is pretty good:
from a month down to a week. And ING has 500 applications teams doing DevOps.
CSG went from 200 incidents per release down to 18. That's amazing. These are
major companies that are singing the praises of DevOps at the DevOps Enterprise
Summit back in 2016. People were starting to take notice. This is not just the
unicorns anymore. So, how are they doing this? What is their secret? Is it some
magic tool? ...and where can I buy it? No! They have embraced the DevOps
culture. It is not a tool that they bought. It is not some procedure that they
follow. They actually changed the culture of their company, something very hard
to do but necessary to gain the advantages that DevOps has to offer. Until and
unless you change the culture of your company, you will fail at attempting
DevOps because DevOps is not about tools. It's about trust, transparency,
communication, coordination, and discipline. You can't buy DevOps in a box. In
this video you learned: The impact of John Allspaw’s “10+ Deploys per Day –
DevOps at Flickr” in 2009. And that DevOps is a cultural change that requires
trust, transparency, and discipline across teams.