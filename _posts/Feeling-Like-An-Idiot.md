---
layout: post
title: Feeling Like An Idiot
---

Christmas Eve marked the 6 month anniversary of my first "real-world" job since I graduated last May. Those first six months have been more information dense than the four year that lead me to the job.

I was under no disillusions that a degree was going teach me everything I had to know about entering the industry but I never expected to spend many days feeling like a fucking idiot.

# Feeling like an idiot

## The process

The first thing I struggled with was understanding the process around software development. I had a course on agile software development, and felt like I understood that but now there were many more people doing different things that was out of scope of our course. I've worked in plenty of teams while I was a student but everybody gets involved in everything. People who are dedicated and talented at one thing that I may have only briefly gave a thought to in the past like testing, user experience, and product management 

Absolutely every project I'd undertaken at this point as been a greenfield project. I've never had to dive into an existing code and understand what or why a previous engineer has done what they have done. All university assignments are short lived, so those responsible were always within distance. This problem was only compounded by working with a language I was mostly unfamiliar with. 

We use C# for the vast majority of our backend systems, a language I had only _very_ briefly used in a university assignment a long time ago. Additionally, we have an unorthodox frontend setup as we are still migrating to a new version of Angular, but some AngularJS codebases still lurk around making development more complex and challenging than it has to be.

I found the process of code reviewing terrifying for the first few times, the first couple of times silly obvious mistakes would surface. Things like that I haven't covered some things with unit tests, leaving in temp variable names, or my all time favourite - committing `_logger.Information('blah blah');`. These were just careless mistakes but they had a notable impact because I knew I was better than that. 

## The bigger mistakes

I had picked up a boomerang bug in that occurred in our user permissions service. The bug in question wasn't all that thrilling, roughly was that some things weren't being populated as expected under a set of particular circumstances.

I was also up against a rather large function with a high cyclomatic complexity due to the nature the possible permissions. Code can be hard to read at the best of times but I found this case extremely challenging. A piece of advice my lead dev gave me was to just set a couple of breakpoints and trace it locally. This was actually working pretty well, and I was learning how things work quite happily. This was until something came in on slack.

![An anonymous slack message which reads "at channel, did someone change the super admin? Because it's totally broken now."](/images/Feeling-Like-An-Idiot/ohno.png)

Yup, it was me.

This felt especially bad because I've now impacted other people trying to do their job while I was tip toeing around. I had authenticated using the incorrect account and accidentally changed some permissions. Fortunetly I was now familiar with our possible permissions that I was able to quickly revert the changes and created my own test account for this bug. However I still felt pretty deflated because I wasn't thinking how this may impact others as I should have been doing.

## Talking myself down

It was a rough feeling.

I had always enjoyed porgamming and computer science and I was always heading for the degree classification I wanted so I was mostly pretty relaxed about it all, that's not say to it wasn't without it's challenges.

I've never felt that grades were a good reflection of ability but I had other ways to make me feel like I was competent at what I was saying and doing. I went across the country and Europe to hackathons, competing five times and [organising one at Dundee University](https://conorhaining.com/posts/Dundees-Hackathon/), a legacy that's went into my career as a corporate sponsor for student hackathons across Scotland. In my final year of study, I was a lab tutor to a total seven different modules and would have supported well over a hundred students in some form or another. I also ran a [Codeclub](https://codeclub.org/en/) at a local primary school for around 2 and half years, which I felt did wonders for my communication skills and requires a lot of patience.

# Tackling the imposter syndrome

## Being DRY

Don't Repeat Yourself (DRY) is a software principle meaning that if you keeping writing the same bit of code over and over, then you should abstact it away somehow. I also try to apply it outside of software I write. When I have a code review comment about missing tests, I'll check my coverage before pushing. If some work has a bug in it, I more carefully think about test cases. Over time I noticed the improvement and that helped my confidence.

This reduced the silly mistakes that I would see in my code reviews and reduce the back and forth between me and the review. This was also pretty good for my productivity and left me feeling more satisfied instead of feeling bogged down with one particular work item. I also try avoid the number of times work is returned from QA with bugs or a need for further information. This was a big win against feeling like an imposter because nothing scream imposter more than buggy code.

## Supporting myself

I have access to [Pluralsight](https://www.pluralsight.com/) through my work account, this allows me to study larger and broader topics which relevant to the day job but can't be as easily understood as part of day job development. The most sucessful use of this for me has been trying to map it to technologies or libraries I am confident and familar with. For me these were questions like what is Entity Framework? and how does it differ from what I'd used in the part; or what's the difference between .NET Core and .NET Standard? How does C# do package management differently than other languages and a whole other bunch of questions.

From time to time we also host [Test Driven Development Katas](http://www.peterprovost.org/blog/2012/05/02/kata-the-only-way-to-learn-tdd/) - an intense session where a group work on their unit testing skills. These are particularly nerve wracking the first few times, because it involves writing code infront of other (more experienced) engineers, it's easy to feel like a fool. However what I noticed once I overcome those neves was that this was a safe place to be a fool and that having a safe space to learn like this was vital, despite the very high barrier to feeling comfortable.

## Parting Wisdom

Similar to being DRY, I think it's also helpful to pass on your knowledge from the mistakes I've made. Two graduates joined my team a few months after I did, so I felt like I could heavily relate to their experiences starting out. Part of what helped me overcome the imposter syndrome was to explain the processes and systems I had struggled with. This really helped cement my own knowledge but also helped these people grow within the team in a different way than I had done.

Pairing with them and going through our architecture was also a valuable experience because it allowed me to reassess what I had been taught about our setup. When I couldn't answer a question, I knew who was the most appropriate person to asnswer rather than flood my buddy with questions. The bonus being that there is a learning experience for more than one person.

## Getting ahead on the features

When I first joined, I had an idea of the work that was going on and why we had to do it. More recently I've found that taking some time to understand the bigger picture of the work. I've found that having an outlook of what is coming up ahead allows me to mentally prepare for what I need to understand before we get there. This includes learning how our current things work by reading code, documentation, or asking those around me; or by looking at the libraries, frameworks, or techniquies to do it properly.

# Wrap it up

It's understood and accepted that imposter syndrome can strike any person in any way. I was hesitating to write and publish this piece at times because I wasn't sure I properly understood imposter syndrome which says it all. The first thing I find helpful is to remind yourself that there is a perfectly valid reason you're in the position you're in and to work out the system you need to manage the imposter feeling. For me it's reducing my own mistakes and helping others avoid the same but everyone's milage will vary.

I hope that going over my experience and feelings that I may help others realise that this is a very common feeling and that the vast majority of engineers go through it, particularly at the beginnings of their career. Some of the strategies I outlined may work for you but I know that isn't true of everybody so if you do find yourself struggling with imposter syndrome I would love to know how you delt with it, so feel free to reach out.