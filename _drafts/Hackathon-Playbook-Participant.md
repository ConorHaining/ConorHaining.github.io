---
layout: post
title: Being a Hackathon Particpant
header-image: /images/HackathonParticpant/HackathonPlaybookParticipantTitle.jpg
header-alt: Flying the University of Dundee flag while at GUTS 2018
category: Hackathon Playbook
summary: 
---

I've been very fortunate to be heavily involved in hackathon culture while I was a student and into my fulltime job. I've been able to be on all sides of the coin as an organiser , a participant and as a corporate sponsor. In this three part series I'm documenting the processes and ideas I follow to successfully contribute to this community. In part one, I'm discussing how I've been a participant and how I've taken on challenges across Scotland and Europe.

# Finding a hackathon

In my experience, hackathons tend to broadly fall into one of three categories. University organised events are typically put together by that university's computer science or tech society with the committee members organising it alongside their studies. Then there is I call "Major Hackathons" are hackathons which are open to students and those early in their career but are more polished events that have the backing of dedicated organisers. Finally there are corporate organised events which have dedicated organisers and typically one sponsor who foots the bill for the entire event. Most often hackathons run over a weekend and vary in length between 24 and 48 hours long.

Knowing what kind of hackathon you're attending sets your own expectations for the types of challenges and organisations that are going to be a key part of the event. I don't have any personal experience with corporate sponsored events but I would assume that for the most part, what I'm going to lay out here is applicable to all three types of events.

If you're looking for places to pick up your first hackathon, here's some places to start. Firstly, your local university's tech or compsci societies are likely to host one every year so that's a solid place to start. Following that, neighbouring universities are also solid places to checkout. They usually have Facebook pages and sometimes websites.

## Major League Hacking

Major League Hacking (MLH) are an organisation which support student hackathons across the world by creating leagues in each region which run concurrently in North America, Europe, and Asia Pacific. I'll come back to MLH more in the organiser section, but while they are a great and well intentioned organisation, they are very focused on North America and have a tendency to overlook smaller events in Europe.

# What you should be looking for

First and foremost, decide what you want to get out of the event. There is plenty of things to gain from hackathon and here's a couple of things I often looked to get out of it.

## Employment

There is one reason alone that a company is sponsoring events, it is part of their recruitment efforts. This is a great chance to meet enthusiastic engineers who may have only recently entered the field. Even if you don't want to join the company they're at I've found most people are happy to talk shop. It's worth quickly pointing out that at some hackathons, particularly the larger ones, there are sometimes companies who are looking to acquire IP and create startups or spinouts but I've never had any experience with that.

## Something new

There's few opportunities for you to dedicate some time to picking up something new with little recourse. Hackathon projects can be a throwaway adventure but still a great learning experience. I've had a chance to play with Unity and it's VR capabilities when creating a balloon popping game, my first ever project. The first time I used NodeJS was at a hackathon, as well as dipping into machine learning with Jupiter notebooks.

# Preparing yourself

For most hackathons that you want to get to, it's a case of hopping on a train or bus to wherever. Some are a bit further, I've been very luck to visit Edinhoven and Helsinki for hackathons. Some, and again it's more often the larger hackers, offer travel reimbursement for some amount which depends on the distance you're travelling. If an event doesn't offer reimbursement and you don't think you could make it otherwise, it's worth contacting them to find out if they can support you.

One thing I can't stress enough, if you've travelled internationally for an event, you cannot get by on the sleeping arrangements at the event. You will need to get yourself a proper bed to sleep in at some point.

If you're packing a bag to go, make sure you've got a change of clothes and some toiletries to see you through the weekend. Nothing is worse than not getting the chance to freshen up. You may be fortunate enough to either be close to home where you can nip home and shower or you're at a venue with those facilities, if either are true then it's strongly advised you do so. No matter how much you want to press on with your hack, taking some time away from it gives your mind a rest.

There's nothing worse than being at an event with poor connectivity, and this can have dramatic consequences for your hack. It's safer to assume this is the case, so make sure you've got all the big bandwidth items such as code editors, SDKs, and other bits of software you might think you'll need to enable your hack.

# Hacking Begins

I've found venues to come in all shapes and sizes. I've hacked in small breakout areas on uni campuses, [to former factory floors for Phillips](https://conorhaining.com/posts/HEX-2018/). Scoping out the venue is worthwhile, finding a good spot can be make or break for the weekend. Organisers and sponsors like wandering around to see what hackers are up to, and if you're quick enough you can use the opportunity to do some very early project discovery. Use it to clarify you're going in the right direction for your hack.

Hackathons typically either have a Slack workspace or a Discord for you to join, it's important to get on this early so you'll see announcements from the organisers for when food arrives and a chance to interact with the sponsors who usually have their own channel.

You're going to need a crack team to successfully take on any challenge. I've always arrived at an event with friends as a team but if you're not able to gather people beforehand then hackathons usually setup the chance for you to find team mates. Hackathons often kick off around lunch, but I have known events to kick off after dinner, in either case it's usually proceeding a mealtime which gives you time to mingle and try find people or existing teams. It's also another reason to join the Slack/Discord so you can broadcast your enthusiasm while looking for a team.

Now you've got your team, get a git repo setup, add people as collaborators and setup some scaffolding for what you need to do.

## Idea Planning

However long your hackathon is, you should subtract 8 hours for rest (whether you use it or not is another matter) to give you a realistic estimate of how long you have to complete your hack. There is no one-size-fits-all approach to hackathon ideas but there are some things I think can give you an edge.

Ensure that you truly understand the challenge you're taking on, some challenges require some proper research and reading before you can properly develop a solution. When at [Junction](https://hackjunction.com/) we took on a challenge to detect a [SS7 attack](https://www.theguardian.com/technology/2016/apr/19/ss7-hack-explained-mobile-phone-vulnerability-snooping-texts-calls) in a stream of pcap data, which is the format of SMS traffic over a real mobile network. The challenge came with a length document of background research which we skim read and dived into what we thought was the solution. The result of this was a failed hack. Because we didn't understand properly what we should be looking for, the AI model we created was incorrect and by the time we realised what was going wrong, it was too late to retrain the model. We declared it a failure and went to explore Helsinki instead.

> can i find a picture of the ballpit

Your hack should seek to meet the challenge in the smallest and cleverest way possible. For fun hacks that are either purposefully silly or are game based, you're seeking to impress or enthuse the judges of the challenge. I do that by trying to inject the team's personality into the hack. While at [RGUHack](https://rguhack.uk/) in 2017, we created a ball pit VR game modelled on the open space theatre that was being used for the venue. This advice can definitely extend to more serious challenges as well, when at [GUTS](https://gutechsoc.com/hackathon) in 2018 we created a help center like application for a challenge that looked to perform analysis on some audio stream but we used the [Cantina Band](https://www.youtube.com/watch?v=sHD-knhS6es) as our hold music before you get connected. Both of these things gave us an edge and I think made us more memorable.

Don't feel like you need to knock it out the park and be a superstar coder to create a good hack, when we created the VR balloon pit game, that was our team's first time using VR or Unity. It's impressive to see teams take on something absolutely new to them and still produce a product. It makes that win all the more rewarding and sweeter.

# Hacking

You need to be prepared and in a mindset to accept a vast amount of information in a condensed period of time. You will also need to open to changing power within the team, meaning that if somebody is very skilled in using a particular API then step back and let them lead and direct; if you're able to contribute skills then don't be afraid to take control and guide your team to completing something. You may find yourself in the back seat for the full ride, which is an unfortunate roll of the dice but you're guaranteed to walk away with a wealth of knowledge.

You don't have the time to set out a comprehensive system architecture, so if you're working across different parts of a system, you must be crystal clear about what your expect and return for the functionality you're working on. You'll be constantly communicating about what you're doing, and don't be upset if somebody hasn't registered what you're doing, there is a lot going on and it's easy for things to fall out of a persons mind. You'll be sharing verbally but you should always be pushing your code so everyone has access to it. Don't be afraid to get help from your team, mentors, or anybody really. Sure, a hackathon is a competition, but the learning experience is the key thing to remember. Most people will be glad to show off some skill or thing they know, as long as people are friendly and grateful then everyone becomes better of.

Keep it simple, stupid. While hacking it's very easy to start thinking of things that can enhance your project before you've completed what you're doing, in the real world this is scope creep. Write these ideas down at the very least and come back to them when you're confident with your actual solution. It's very simple of projects to spiral out of control as people start wanting to show off - which is great - but it's not possible to do this without a solid foundation. Everyone in the team needs to be cautious and concious of this, if you start dismissing other peoples feature ideas it has to be legitimately to stop scope creep.

It is vital to get some rest. It's a common joke and mantra about continuously coding throughout the night like you're some kind of all powerful machine. You are not the [Duracell Bunny](https://www.youtube.com/watch?v=4AZg11VPKow), no matter what you think, you need the time to stop, put your mind elsewhere and recharge. Even if you are capable of staying awake for the duration of the event, the hangover from that lasts for days and days and is hellish. For your own sake don't do this.

# Final Countdown

As you approach the end of the hacking period, there is a couple of administrative items you need to have ready. Many events ask you to publish your hack onto [Devpost](https://devpost.com/) which enables judging and showcasing. Often if you neglect to do this, you don't qualify for judging and the time you've spent writing code won't receive recognition.

Give your consideration to how you'll show off your work. As a general rule of thumb, you shouldn't have any slides unless there's no actual product to show. Show off what you've done, what you'd like it to do then, and where applicable, give the judges a chance to use it. If you've got a uniquely interactable component, show it off! In the hack at GUTS mentioned previously, we made our judges call our hack to see it work live in from of them. 

However be aware that live demos can suck, are very risky, but are exceptionally cool when you are able to pull them off. Remove as much risk as you can, so you may need to fake a couple of items but since you can guide people through your narrative you can often get away with this.

Document what you've learned and make sure your judges know this as well. One of the secondary judging criteria is enthusiasm and showing off your willingness to learn is endearing to see as a judge.

Taking part in a hackathon is designed to be a fun experience, and it's a safe sandbox for you to try out new tech and to expand your learning. You also meet wonderful like minded people who you can share this experience with. If you are early in your career, hackathon projects give you an edge against candidates with similar academic background. I interviewed for my current job after winning at a hackathon and was able to show off my experiences and learnings from that.

Next time I'll go through planning and organising your own hackathon for your community.