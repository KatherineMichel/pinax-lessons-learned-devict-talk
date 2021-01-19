# Pinax Lessons Learned- DevICT

# Table of Contents

- [About](#about)
- [Slides and Script Table of Contents](#slides-and-script-table-of-contents)
- [Slides and Script](#slides-and-script)   
- [Attribution](#attribution)
- [Contact Kati](#contact-kati)
- [Copyright](#copyright)

<hr>

## About

Slides and script for a talk Katherine "Kati" Michel ([Twitter](https://twitter.com/KatiMichel), [GitHub](https://github.com/KatherineMichel)) gave at DevICT [Lunch Talks](https://www.meetup.com/devict/events/275303517/) Wednesday, January 13, 2021 at 12:00 noon CST via Google Meetup.
 
Slide Deck
* [Original slide deck](https://docs.google.com/presentation/d/1oAGBBRBcbaBLUU57OjaCeXLRtiEe1Lf9XQBnKZfCiyg/edit?usp=sharing)

:top: <sub>[**back to top**](#table-of-contents)</sub>

<hr>

## Slides and Script Table of Contents

- [Pinax Lessons Learned](#pinax-lessons-learned)
- [About Me](#about-me)
- [In Summary](#in-summary)
- [Time Machine](#time-machine)
- [Time Machine: 2008](#time-machine-2008)
- [How It Began](#how-it-began)
- [Fast Forward: 2017](#fast-forward-2017)
- [How It Was Going, 80 Project and Apps](#how-it-was-going-80-project-and-apps)
- [How It Was Going, GitHub Organization, Global Docs, and Slack](#how-it-was-going-gitHub-organization-global-docs-and-slack)
- [How It Was Going, Sustainability Lacking](#how-it-was-going-sustainability-lacking)
- [Tribal Knowledge](#tribal-knowledge)
- [Pinax Documentation](#pinax-documentation)
- [Documentation](#documentation)
- [One Source of Docs](#one-source-of-docs)
- [Variations in Configurations](#variations-in-configurations)
- [One Configuration Approach](#one-configuration-approach)
- [Reduce the Backlog](#reduce-the-backlog)
- [Engagement with Individuals](#engagement-with-individuals)
- [Communicate Better](#communicate-better)
- [Engagement with Community](#engagement-with-community)
- [Automation](#automation)
- [Biggest Lesson Learned](#biggest-lesson-learned)
- [Thank You](#thank-you)

:top: <sub>[**back to top**](#table-of-contents)</sub>

<hr>

## Slides and Script

The script is a general outline and varies somewhat from what was said during the talk.

<table>

<tr><td width="30%">

![Slide 1](https://speakerd.s3.amazonaws.com/presentations/a1b7d9619ede4b67a0e5c531e47adc81/slide_0.jpg)

</td><td>

### Pinax Lessons Learned

* Hi everyone
* It’s great to be here with you
* My name is Katherine Michel. I also go by Kati
* My talk is about “Pinax Lessons Learned”
* It’s actually taken from a much longer talk that will air February 7 in the FOSDEM Python Devroom
* So check it out if you want to know more

</td></tr>


<table>

<tr><td width="30%">

![Slide 2](https://speakerd.s3.amazonaws.com/presentations/a1b7d9619ede4b67a0e5c531e47adc81/slide_1.jpg)

</td><td>

### About Me 

* A little bit about me
* I’m currently a Consultant to the Wharton School at the UPenn
* I’m working on a project called Simpl… it’s an open-source Python/Django/React game simulation framework 
* Pinax Maintainer/Web Developer

</td></tr>


<table>

<tr><td width="30%">

![Slide 3](https://speakerd.s3.amazonaws.com/presentations/a1b7d9619ede4b67a0e5c531e47adc81/slide_2.jpg)

</td><td>

### In Summary 

* My talk is about Pinax
* Pinax is an open-source library of reusable Django starter projects, apps, and themes for building websites. When developers began building Pinax in 2007, they had fun adding to it, but eventually Pinax had grown to be around 80 projects and apps. 
* There was not a strategy in place to make Pinax as easy as possible to maintain. So the maintainers began to suffer burnout. 
* I was hired to work on Pinax in the fall of 2017. In my talk, I'll outline the critical problems I discovered and the solutions I've implemented to make Pinax healthier and easier to maintain.

</td></tr>


<table>

<tr><td width="30%">

![Slide 4](https://speakerd.s3.amazonaws.com/presentations/a1b7d9619ede4b67a0e5c531e47adc81/slide_3.jpg)

</td><td>

### Time Machine

* To better understand this story, we need to go back in time to 2008

</td></tr>


<table>

<tr><td width="30%">

![Slide 5](https://speakerd.s3.amazonaws.com/presentations/a1b7d9619ede4b67a0e5c531e47adc81/slide_4.jpg)

</td><td>

### Time Machine: 2008

* Some Django enthusiasts had formed a group. 
* They had found themselves reusing some of the same code patterns while building websites with Django
* At the first ever DjangoCon US, James Tauber, one of the original Pinax authors, gave a talk about this new community called Pinax

</td></tr>


<table>

<tr><td width="30%">

![Slide 6](https://speakerd.s3.amazonaws.com/presentations/a1b7d9619ede4b67a0e5c531e47adc81/slide_5.jpg)

</td><td>

### How It Began

* James talked about his own site Quisition
* Even though it was a flashcard site, much of its functionality had nothing to do with flashcards
* So they began to abstract these patterns into reusable starter projects, apps, and themes
* The idea was that they could use this reusable library to go from website idea to realization more quickly

</td></tr>


<table>

<tr><td width="30%">

![Slide 7](https://speakerd.s3.amazonaws.com/presentations/a1b7d9619ede4b67a0e5c531e47adc81/slide_6.jpg)

</td><td>

### Fast Forward: 2017

* Let’s fast forward to 2017
* It had been around 10 years since the Pinax idea had been born
* I was hired to work on Pinax

</td></tr>


<table>

<tr><td width="30%">

![Slide 8](https://speakerd.s3.amazonaws.com/presentations/a1b7d9619ede4b67a0e5c531e47adc81/slide_7.jpg)

</td><td>

### How It Was Going, 80 Project and Apps

* By 2017, Pinax had grown to be a large group of professionally-quality, interdependent Django projects and apps
* This included starter projects with Pinax apps pre-installed and a command line interface to install them
* This also includes sophisticated testing, packaging, and continuous integration configurations
* The Pinax GitHub organization alone has around 80 repos in it

</td></tr>


<table>

<tr><td width="30%">

![Slide 9](https://speakerd.s3.amazonaws.com/presentations/a1b7d9619ede4b67a0e5c531e47adc81/slide_8.jpg)

</td><td>

### How It Was Going, GitHub Organization, Global Docs, and Slack

* In addition to the GitHub organization
* Pinax now had a global docs site and a Pinax Slack channel for community and support

</td></tr>


<table>

<tr><td width="30%">

![Slide 10](https://speakerd.s3.amazonaws.com/presentations/a1b7d9619ede4b67a0e5c531e47adc81/slide_9.jpg)

</td><td>

### How It Was Going, Sustainability Lacking

* Without a strategy in place to make Pinax as easy as possible to maintain, the maintainers began to suffer burnout. 
* By now, many of the original authors had moved on
* Sustainability was lacking

</td></tr>


<table>

<tr><td width="30%">

![Slide 11](https://speakerd.s3.amazonaws.com/presentations/a1b7d9619ede4b67a0e5c531e47adc81/slide_10.jpg)

</td><td>

### Tribal Knowledge

* Problem: Tribal knowledge
* Solution: Document the tribal knowledge
* The Pinax authors knew how to do things quickly, but the knowledge remained in their heads
* But… the barrier of entry knowledge-wise was fairly high and the docs were sparse and not beginner friendly

</td></tr>


<table>

<tr><td width="30%">

![Slide 12](https://speakerd.s3.amazonaws.com/presentations/a1b7d9619ede4b67a0e5c531e47adc81/slide_11.jpg)

</td><td>

### Pinax Documentation

* I started by creating a release plan that explained the “Pinax way of doing things”
* Then moved on to creating a global community health file repo filled with default files
* This included a Code of Conduct
* A community plan
* Contributing and support information
* Information for Maintainers
* And issue and PR templates

</td></tr>


<table>

<tr><td width="30%">

![Slide 13](https://speakerd.s3.amazonaws.com/presentations/a1b7d9619ede4b67a0e5c531e47adc81/slide_12.jpg)

</td><td>

### Documentation

* Problem: Existing docs difficult to find, duplicated, and inconsistent
* Solution: One source of documentation, easy to find, and use
* There were bits of documentation here and there, some forgotten, some private

</td></tr>


<table>

<tr><td width="30%">

![Slide 14](https://speakerd.s3.amazonaws.com/presentations/a1b7d9619ede4b67a0e5c531e47adc81/slide_13.jpg)

</td><td>

### One Source of Docs

* Pinax has a wiki
* I organized these historical docs, links, and new release plans in a Pinax wiki
* Then a blurb was added to the repo READMEs to make all of the docs more discoverable
* Including the global docs, app specific docs, tagged and published releases, support, contributing, and release docs

</td></tr>


<table>

<tr><td width="30%">

![Slide 15](https://speakerd.s3.amazonaws.com/presentations/a1b7d9619ede4b67a0e5c531e47adc81/slide_14.jpg)

</td><td>

### Variations in Configurations

* Problem: Variation in configurations
* Solution: Choose one configuration approach and implement across projects
* A number of people had created and worked on different Pinax projects at different times
* Because of this, there was a lot of variation in terms of how things had been done
* I can tell you from personal experience that as a newcomer, this made the code collectively harder to understand and more difficult to maintain

</td></tr>


<table>

<tr><td width="30%">

![Slide 16](https://speakerd.s3.amazonaws.com/presentations/a1b7d9619ede4b67a0e5c531e47adc81/slide_15.jpg)

</td><td>

### One Configuration Approach

* After some research, I chose one configuration approach and implemented it across repos 
* I also detailed it in the release plan
* The more consistent the GitHub organization is, the better

</td></tr>


<table>

<tr><td width="30%">

![Slide 17](https://speakerd.s3.amazonaws.com/presentations/a1b7d9619ede4b67a0e5c531e47adc81/slide_16.jpg)

</td><td>

### Reduce the Backlog

* Problem: Lack of engagement with individuals
* Solution: Reduce backlog of issues and PRs and catch up with engagement

</td></tr>


<table>

<tr><td width="30%">

![Slide 18](https://speakerd.s3.amazonaws.com/presentations/a1b7d9619ede4b67a0e5c531e47adc81/slide_17.jpg)

</td><td>

### Engagement with Individuals

* Between releases
* Over 160 issues closed
* Over 100 PRs merged
* Over 30 PRs closed
* Countless questions answered in issues and Slack
* I began with resolving the lowest hanging fruit issues and PRs knowledge-wise and working my way up
* The idea was to reduce the number until the new and existing issues and PRs would be more manageable

</td></tr>


<table>

<tr><td width="30%">

![Slide 19](https://speakerd.s3.amazonaws.com/presentations/a1b7d9619ede4b67a0e5c531e47adc81/slide_18.jpg)

</td><td>

### Communicate Better

* Lack of engagement with the community
* Write more blog posts about plans and progress, and publicize well

</td></tr>


<table>

<tr><td width="30%">

![Slide 20](https://speakerd.s3.amazonaws.com/presentations/a1b7d9619ede4b67a0e5c531e47adc81/slide_19.jpg)

</td><td>

### Engagement with Community

* I began to write blog posts and tweet about them
* The posts might be about Pinax, or some other Django-related activity and I would mention Pinax
* People began to become interested in Pinax, telling me that they had heard about Pinax through my writing
* It can have a huge benefit to stop and take time to write about the accomplishments and progress of the project and sharing it with the community 
* Even if a handful, or even one person, becomes interested and contributes, it can make a major impact
* It makes people aware of the project and gives them social proof that it’s actively being maintained

</td></tr>


<table>

<tr><td width="30%">

![Slide 21](https://speakerd.s3.amazonaws.com/presentations/a1b7d9619ede4b67a0e5c531e47adc81/slide_20.jpg)

</td><td>

### Automation

* Problem: Tasks being done manually
* Solution: Automate tasks
* Automating tasks lowers the risk of burnout

</td></tr>


<table>

<tr><td width="30%">

![Slide 22](https://speakerd.s3.amazonaws.com/presentations/a1b7d9619ede4b67a0e5c531e47adc81/slide_21.jpg)

</td><td>

### Biggest Lesson Learned

* In July 2020, based on what I had learned,I oversaw the completion of an important Pinax release. 
Around 28 apps were included and we notably dropped support for Python 2.7
* It was a huge milestone for me, personally and professionally. Not only did I initiate the release, but I managed the end-to-end process. I created the release plan, oversaw the work of others, updated 10 apps myself, merged all of the PRs, and tagged and published the packages. 
* The biggest lesson I’ve learned while working on Pinax is that the latest release succeeded because of my communication and teaching skills
* I learned this by accident
* My blog posts attracted contributors
* The release could not have been completed without the help of these contributors… it would have been too much work and required specialized skill
* The release documentation I had written enabled the contributors to help, to mutual benefit
* I was thrilled that they were able to use this documentation to complete a large portion of the work, with occasional support from me

</td></tr>


<table>

<tr><td width="30%">

![Slide 23](https://speakerd.s3.amazonaws.com/presentations/a1b7d9619ede4b67a0e5c531e47adc81/slide_22.jpg)

</td><td>

### Thank You

* Twitter: KatiMichel
* GitHub: KatherineMichel
* Email: kthrnmichel@gmail.com

</td></tr>


</table>

:top: <sub>[**back to top**](#table-of-contents)</sub>

<hr>

## Attribution

The style of this transcript is heavily inspired by:

* Ana Balica's ([Twitter](https://twitter.com/anabalica), [GitHub](https://github.com/ana-balica)) transcript of her [Humanizing among coders](https://ana-balica.github.io/2017/05/28/humanizing-among-coders/) keynote for [PyCon CZ 2016](https://cz.pycon.org/2016). 
* Honza Javorek's ([Twitter](https://twitter.com/honzajavorek), [GitHub](https://github.com/honzajavorek)) transcript of Anna Ossowski's ([Twitter](https://twitter.com/OssAnna16), [GitHub](https://github.com/OssAnna16)) keynote [Be(Come) A Mentor! Help Others Succeed!](https://github.com/honzajavorek/become-mentor) for [PyCon CZ 2017](https://cz.pycon.org/2017/). 

Thank you!

:top: <sub>[**back to top**](#table-of-contents)</sub>

<hr>

## Contact Kati

* Email: kthrnmichel@gmail.com
* GitHub: https://github.com/KatherineMichel
* Twitter: https://twitter.com/KatiMichel

:top: <sub>[**back to top**](#table-of-contents)</sub>

<hr>

## Copyright

© 2021 to Present Katherine Michel. All Rights Reserved.

