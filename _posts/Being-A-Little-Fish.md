---
layout: post
title: Being a little fish
---

Christmas Eve marked the 6 month anniversary of my first "real-world" job since I graduated in May. The 6 months has been much more information and learning dense than the 4 year course, but that's perhaps a story for another time.

Retrospectively I can honestly say I've nothing bad to report. It isn't hellish, and the usual grind is to be expected. But I can only say that _now_ because the couple of months I spent a lot of time feeling like a fucking idiot. 

# Feeling like a fucking idiot

The first thing I struggled with was understanding the process around software development. I had a course on Agile software development, and felt like I understood that but now there were many more people involved in the process than I was use to. I've worked in plenty of teams while I was a student but everybody gets involved in everything. Dedicated people who specialise in areas I may have only briefly gave a thought to in the past like quality assurance, user experience, and product management.

Absolutely every project this point as been a greenfield project. I've never had to dive into an existing code and understand what a previous developer has written. All university assignments are short lived, so if I had to understand why somebody did something it was always easy enough to ask. I think it's generally accepted that reading and understanding other people's code is difficult, certainly a sentiment I can get on board with, and something I've noticed myself which has improved over time. This problem was compounded by working with a language I was mostly unfamiliar with. 

We use C# for the vast majority of our backend systems, a language I had only _very_ briefly used in a university assignment a long time ago. And even then it was more a look at multi-threading than it was the features of C#. Additionally, we had a peculiar frontend setup as we migrate to a shiny new version of Angular, but some AngularJS codebases still lurk around making development more complex and challenging than it has to be if you're unfamiliar with the way to set it up properly.

The first couple of times I put out code for review, silly mistakes would get pointed out to me. Things like that I haven't covered some things with unit tests, leaving in temp variable names, or my all time favourite - committing `_logger.Information('blah blah');`. These were just careless mistakes but they had a notable impact because I knew I was better than that. However the worst was yet to come.

## Bigger mistakes

I had picked up a boomerang bug in that occurred in our user permissions service. The bug in question wasn't all that thrilling, roughly was that some cells weren't being populated as expected under a set of particular circumstances.

I was also up against a rather large function with a high cyclomatic complexity due to the nature the possible permissions. Code can be hard to read at the best of times but I found this case extremely challenging. A piece of advice my lead dev gave me was to just set a couple of breakpoints and trace it locally. This was actually working pretty well, and I was learning how things work quite happily. This was until something came in on slack.

![An anonymous slack message which reads "at channel, did someone change the super admin? Because it's totally broken now."](/images/ohno.png)

Guess who changed the super admin. It was me 👋.

This felt particularly bad because I've now impacted other people trying to do their job while I was tip toeing the codebase and our user permissions. Since I couldn't be sure of the damage I had caused, I felt panicked. Now fortunately I was able to trace back the changes I had made to the super admin and quickly to switch to use a different account and kept my head down. It was silly of me to be using the super admin anyway.

None of this felt very good, and a lot of the time I was left feeling deflated and feeling lost and unsure if I was cut out for this.

# Rationale

It was a rough feeling.

I had always enjoyed software development and computing at large and I was always heading for the degree classification I wanted so I was mostly pretty relaxed about it all, that's not say to it wasn't without it's challenges.

I've never felt that grades were a good reflection of ability but I had other ways to make me feel like I was competent at what I was saying and doing. I went across the country and Europe to hackathons, competing five times and [organising one at Dundee University](https://conorhaining.com/posts/Dundees-Hackathon/), a legacy that's went into my career as a corporate sponsor for student hackathons across Scotland. In my final year of study, I was a lab tutor to a total seven different modules and would have supported well over a hundred students in some form or another. I also ran a [Codeclub](https://codeclub.org/en/) at a local primary school for around 2 and half years, which I felt did wonders for my communication skills and requires a lot of patience. I was also an intern in the same organisation and offered a full time position, so they were clearly keen to keep me around.

# Understanding why and taking action

I was keen to shake this crappy feeling. I knew about impostor syndrome but during this time it had consciously escaped me. I tried to take some action on discovering the root cause of this problem. I have kept a list of the mistakes I've make since starting this job with a commitment to only do them once, understand why and never again. Out of this list, I noticed a handful of common themes that I was never taught or even hinted at during education so I've tried to tackle those gaps first.

Trying to understand the business process was also something else that took some time. Knowing that software development isn't just a case of beep boop and ship it, but understanding what our processes are is a challenge, and especially because these processes exist to minimise errors and disruptions. University assignments lets me put on many different hats. Particularly my honours project, I was all the hats; I was the product manager, I was the UX designer, the developer, the tester, I was devops, I was it all. It was a great opportunity for me to learn a little about a lot, but not really master anything. Now I was surrounded by people who were much better at wearing those hats than I was now learning how all the hats work with each other.

# Being the help you wanted
---
#################################################
After four years in the School of Computing at the University of Dundee, I graduated in May earlier this year. 

 # Feeling like a serious fucking idiot

To have such a juxtaposition of feelings was a real source of anxiety for me, anyone who has known me for a long time knows I'm computer daft and I always have been. I really wanted to understand why I felt like this, because I really hoped it wasn't the case.

I have since 

As I was getting use to all these processes and people around me, I found myself making small non-consequential mistakes such as forgetting unit tests, forgetting company naming conventions, or leaving silly things in PRs that I had not cleaned up.

## Having Support

The impostor syndrome was knocking on my front door, trying to drag me out. Nothing was making rational sense, yet I was feeling overwhelemed by everything I had was trying to take on. It wasn't like I was thrown in at the deep-end either, I had a team where I could ask questions, engineers who were able to mentor me through my gaps in knowledge, access to [Pluralsight](https://www.pluralsight.com/) where I could overdose on video content.

I was able to, and still do, bake some learning into my day-to-day when I can. We sometimes pair program on our backlogs and bugs, there are [Test Driven Development Katas](http://www.peterprovost.org/blog/2012/05/02/kata-the-only-way-to-learn-tdd/) - an intense session where a group work on their unit testing.

# Surviving your first mistake

Pffft.

## Tracking the wins

Despite the nightmare story above, I got some value from that experience implicitly. I mentioned earlier how I have kept a list of mistake I've made, I also track the little successes I've found after learning about a [brag document](http://citation-needed.com).

I was able to pick up a lot about unit testing in C#, it's best practices and our standards. How to properly mock and stub method calls and properly isolate the function under test. I've since come to really enjoy unit testing in C#, _a statement that absolutely will not come back to bite me._ I was able to cover my test case and a couple of others I had found that were tricky to understand but weren't covered.

Finally, this once the fix had went under sufficent QA it was pushed out to production, exactly a month after I first joined.

# This isn't Code'n'Go

It took sometime to understand that it isn't just me now. Sure I've worked in plenty of teams while at university and while at hackathons but in those situations, everybody gets involved in everything. Dedicated people who specialise in areas I may have only breifly gave a thought to in the past like quality assurance, user experience, and product management. Frankly, I've never had a product to manage in the past.

Understanding who all the people are around to support me and _how_ they support me

There's also more peripheral things they don't teach you at school, like CS32032 setting up all your software to work, CS52011 Understanding the company's values, or most importantly CS12032 Why you need a pension at 22.