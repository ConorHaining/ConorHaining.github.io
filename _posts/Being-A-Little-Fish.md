---
layout: post
title: Being a little fish
---
After four years in the School of Computing at the University of Dundee, I graduated in May earlier this year. I had always enjoyed software development and computing at large so it was very rare for me to be genuinely stressed about the grades I was receiving. I wasn't always hitting it out of the park, but that was fine, I was always heading for the classification I wanted which was the main thing really. I was mostly pretty relaxed about it all, that's not say to it wasn't without it's challenges.

I've never felt that grades were a good reflection of ability, and that I was lucky to be good at getting tested. But I had other ways to make me feel like I was competent at what I was saying and doing. I went across the country and Europe to hackathons, competing five times and [organising one at Dundee University](https://conorhaining.com/posts/Dundees-Hackathon/), a legacy that's went into my career as a corporate sponsor for student hackathons across Scotland. In my final year of study, I was a lab tutor to a total seven different modules and would have supported well over a hundred students in some form or another. I also ran a [Codeclub](https://codeclub.org/en/) at a local primary school for around 2 and half years, which I felt did wonders for my communication skills and requires a lot of patience. 

 I knew I enjoyed what I did a lot, I've always gotten a lot of satisfaction out of it - I think that's a relatable sentiment for many programmers. So why was it that when I first entered the industry for realsies that I hit with feeling like a serious fucking idiot a lot of the time?

 # Feeling like a serious fucking idiot

To have such a juxtaposition of feelings was a real source of anxiety for me, anyone who has known me for a long time knows I'm computer daft and I always have been. I really wanted to understand why I felt like this, because I really hoped it wasn't the case.

I have since tried something pretty bold, I kept a list of the mistakes I've make since starting this job with a commitment to only do them once, understand why and never again. This isn't something I'd want to share in it's entirety but we'll get to the highlight reel a little later on. Out of this list, I noticed a handful of common themes that I was never taught or even hinted at during education. Retrospectively they're obvious now but a heads up would have been nice.

Firstly, absolutely every single thing I've ever done up until this point as been a greenfield project. I've never had to dive into an existing code and understand what a previous developer has written. All assignments are short lived, no more than 3 weeks in an extreme case, so if I had to understand why somebody did something it was always easy enough to ask. I had a bit of a gap since I wasn't really use to reading and deeply understanding some code. This problem was compounded by working with a language I was mostly unfamiliar with. I think it's generally accepted that reading and understanding other people's code is difficult, certainly a sentiment I can get on board with, and it seems to be only something that gets better with time.

We use C# for the vast majority of our backend systems, a language I had only _very_ briefly used in a university assignment a long time ago. And even then it was more a look at multi-threading than it was the features of C#.

Trying to understand the business process was also something else that took some time. Knowing that software development isn't just a case of beep boop and ship it, but understanding what our processes are is a challenge, and especially because these processes exist to minimise errors and disruptions. University assignments lets me put on many different hats. Particularly my honours project, I was all the hats; I was the product manager, I was the UX designer, the developer, the tester, I was devops, I was it all. It was a great opportunity for me to learn a little about a lot, but not really master anything. Now I was surrounded by people who were much better at wearing those hats than I was now learning how all the hats work with each other.

As I was getting use to all these processes and people around me, I found myself making small non-consequential mistakes such as forgetting unit tests, forgetting company naming conventions, or leaving silly things in PRs that I had not cleaned up.

## Having Support

The impostor syndrome was knocking on my front door, trying to drag me out. Nothing was making rational sense, yet I was feeling overwhelemed by everything I had was trying to take on. It wasn't like I was thrown in at the deep-end either, I had a team where I could ask questions, engineers who were able to mentor me through my gaps in knowledge, access to [Pluralsight](https://www.pluralsight.com/) where I could overdose on video content.

I was able to, and still do, bake some learning into my day-to-day when I can. We sometimes pair program on our backlogs and bugs, there are [Test Driven Development Katas](http://www.peterprovost.org/blog/2012/05/02/kata-the-only-way-to-learn-tdd/) - an intense session where a group work on their unit testing.

# Surviving your first mistake

Pffft.

I had picked up a boomerang bug in that occurred in our user permissions service. The bug in question wasn't all that thrilling, roughly was that some cells weren't being populated as expected under a set of particular circumstances. This was my first time really being left alone with a C# codebase, ontop of attempting to understand wthe complex user permissions we have for our users.

Additionally I was also up against a rather large function with a high cyclomatic complexity due to the nature the possible permissions. Code can be hard to read at the best of times but I found this case extremely challenging. A piece of advice my lead dev gave me was to just set a couple of breakpoints and trace it locally. This was actually working pretty well, and I was sucessfully updating permissions for test users quite happily. This was until something came in on slack.

![A somewhat angry slack message which reads "at channel, did someone change the super admin? Because it's totally broken now."](/images/ohno.png)

Guess who changed the super admin. It was me 👋.

This felt particularlly bad because I've now impacted other people trying to do their job while I was tip toeing around around attempting to solve this bug. Since I couldn't be sure of the damage I had caused, I felt panicked. Now fortunetly I was able to back track the changes I had made to the super admin and decided to switch to use a different account. Worth also pointing out it was silly to play with the super admin account.

Onboarding to any codebase is going to be a challenge for anybody, understanding how it impacts the processes, teams, and systems around you is an additional challenge.

## Tracking the wins

Despite the nightmare story above, I got some value from that experience implicitly. I mentioned earlier how I have kept a list of mistake I've made, I also track the little successes I've found after learning about a [brag document](http://citation-needed.com).

I was able to pick up a lot about unit testing in C#, it's best practices and our standards. How to properly mock and stub method calls and properly isolate the function under test. I've since come to really enjoy unit testing in C#, _a statement that absolutely will not come back to bite me._ I was able to cover my test case and a couple of others I had found that were tricky to understand but weren't covered.

Finally, this once the fix had went under sufficent QA it was pushed out to production, exactly a month after I first joined.

# This isn't Code'n'Go

It took sometime to understand that it isn't just me now. Sure I've worked in plenty of teams while at university and while at hackathons but in those situations, everybody gets involved in everything. Dedicated people who specialise in areas I may have only breifly gave a thought to in the past like quality assurance, user experience, and product management. Frankly, I've never had a product to manage in the past.

Understanding who all the people are around to support me and _how_ they support me

There's also more peripheral things they don't teach you at school, like CS32032 setting up all your software to work, CS52011 Understanding the company's values, or most importantly CS12032 Why you need a pension at 22.