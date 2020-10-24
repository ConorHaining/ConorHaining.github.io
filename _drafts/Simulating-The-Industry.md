---
layout: post
title: Attempting to simulate the software industry for student
header-image: /images/video-calls.jpg
header-alt: An irrelevant stock image showing a load of video calls
category: Tech
---

I was very recently acting as a client to around 100 University of Dundee students, who work intensly for three weeks at the begining of their final year of undergraduate study in order to refine and extend their knowledge on the software development process. Having previously taken this class as a student, I was very keen to pass on the knowledge and skills I have discovered since I graduated onto the students I'd be working with.

This was not without its challenges and my own concerns. I believe it's exceptionally hard to offer a truly authentic experience: it's hard to simulate a company's culture, mission, or bureaucracy without inserting bias into peoples perceptions of the industry. This kind of thing also varies widly between organisations. My mental approach here is to pretend they're working at Conor Inc, where I get to decide these things. I had a personal goal inject some of the knowledge I wish I had when I started working full-time.

To keep marking for the lecturers managable, students were placed in ten teams of ten, but I was worried that [ten people is far too many to have working together](https://en.wikipedia.org/wiki/Brooks's_law) on the same project and the same codebase. I had suggested at the begining of the project that the teams should divide themselves into smaller teams to allow them to work more effectivly. This was also a nice segway into my second suggestion; software products are bigger than the software itself. Software grows legs and arms into various specialisations like infrastructure, quality assurance, user experience, data, and others. 

As a fresh graduate, I struggled with the loss of absolute creative freedom since I was now working with many more people very skilled in their disiplines. As part of their sub-teams, many students took up these specialisations, from devops to product management, documentation to user experience. This was particularly encouraging to see, as for as much as I like writing software, plenty of my friends didn't and it was not until they did internships that they learned about the other possibilities.

# Refining the software skills

I have vivid trauma while in my second year of uni, where a project had totally fallen to bits right before the deadline. We had been using source control and branching the code, but no body checked when code was merged back in to the master branch. I didn't make it mandatory for students in this project but heavily encouraged them to do this. Additionally, reading software that you're not familiar with is really difficult and I had spend so long in university writing software that I just wasn't able to read other peoples code as effectivley. This hit me like a brick wall as a graduate.

I had also hoped to see some teams take up some forms of automated testing, something I had never given much thought to as a student but is a whole fractal of opportunities in software. I also personally believe that software engineers should have the knowledge to deploy their applications to the world, and was glad to see many teams deploy their applications into some type of cloud service.

Having also been the client for the same module last year, I also wanted to reduce some of the friction I'd seen from teams last year. A huge majority of teams had spend the first week "getting the basic functionality" together in one form or another. What I discovered was this meant was the team was often writing an application from scratch; their own routing, database queries, interface styles and so on. These are interesting exercises to do of course, but for the scope of a prototyping project I felt that utilising frameworks would have allowed them to make more progress much faster. Was very pleased to see that this year students took that advice on, and also interesting to see the range of frameworks chosen. [React](https://reactjs.org/) & [Node](https://nodejs.org/en/) being the most popular choices and combination, but some [Flask](https://flask.palletsprojects.com/en/1.1.x/), [.NET](https://dotnet.microsoft.com/angu), [Angular](https://angular.io/), and a little [Vue](https://vuejs.org/).

# The project brief

Last year's student were given a project to create a price comparison webiste based on average charges for certain procedures in US hospitals, based on Medicare payments - a dataset we created from open data from the [CMS](https://www.cms.gov/Research-Statistics-Data-and-Systems/Statistics-Trends-and-Reports/Medicare-Provider-Charge-Data/). We noticed that this brief generated a lot of confusion and misunderstanding, particularly around the data we supplied to the students and in turn this generated a lot of questions which we had to clarify. It's also no surprise that medical billing isn't exactly a thrilling subject, and difficult to wrap your head around in three weeks.

Firstly, the project had to be interesting, but simultaneously not too out there so it's attainable by all teams. Secondly, I had to reduce the friction for the teams to allow them to spend more time on their projects and less time clarifying questions and requirements with me. Not providing any data to the teams also means less responsibility on my side should there be problems with that. I also wanted to leave the brief open ended in some way to allow some creative freedom that may disapear from them in the industry. I also had to had a couple of stretch features incase were able to rattle through the work very quickly.

I was inspired by the rise of the [online pub quiz](https://www.theguardian.com/culture/2020/may/09/phones-away-please-the-rise-and-rise-of-the-online-pub-quiz) in April and May, as well as the sudden growth of many online communities as more people found themselves with a lot more time to spend on the internet, so I asked the teams to create a virual quizing application that could be played with friends without the need of sourcing questions for yourself or managing scores. You can see the full brief below.

<details>
    <summary>Press for the full project brief</summary>
    <ul>
        <li>Create a quizzing application</li>
        <ul>
            <li>For myself</li>
            <li>For others in person</li>
            <li>For friends virtually</li>
            <li>For strangers?</li>
        </ul>
        <li>No accounts/logins</li>
        <li>Need a large and diverse set of questions so it’s not boring</li>
        <li>Powerups, hints, or lifelines when users are stuck</li>
        <li>Scoring, leaderboards, trophies, achievements</li>
        <li>Available on Web, Android, iOS and Windows</li>
        <li>You may want to theme it on a franchise like The Chase, Jeopardy, Pointless or keep it plain</li>
    </ul>
</details>

# Making progress

I really enjoying seeing how each group interprets the same brief, it speaks to the way that software development is more of a creative process than the mathematical nature of computers would have you believe. Teams generally went in one of two directions: The first half were focused more on project planning before commiting to any specific features or design. These teams typically had spend time carfully creating a high fedelity mockup of their application. I think that served as a good base for the whole team to understand what is to be achieved but simultaneously having a "thing" to show and discuss with their client. Other teams had dived straight in to development and had working application to show, and in many cases it had just to be connected to connect everything all up, but they had an interactable prototype to show.

By the second week of the project, all teams had made significant progress to the achieving the minimal viability of the inital brief. It was very endearing to see that - as far as I could tell - the teams had no major or inhibiting hiccups in while they were developing the project. A number of teams were able to insert their own innovations into the project, one of which was asynchronous play which was inspired by the fact the team were working across multiple timezones so realtime play wasn't always available. Another team had an original mechanism for selecting the answers to questions and blended quiz & game. While many teams were mindful of having a strong visual design which was accessible to a wide varity of users.

# The final presentations

I absolutely love this part of this module. Getting to see all the final products and sucessful teams really does make me happy. Each team, and every student, had blown me away with what they were able to do in such a short space of time, and given the circumstances. The entire class was run remotely this year, and students were working across mutliple time zones. Some students became unavilable as some students contracted coronavirus and their teams re-adjusted. It was pretty admirable having to deal with all that plus attempt to contend in the upcoming job market as many [companies cut intern and entry level position](https://www.theguardian.com/money/2020/aug/30/no-internships-no-entry-level-work-under-25s-fear-a-jobs-squeeze) and I do hope that the work they've done in this module, and the acquired skills will give them the edge.