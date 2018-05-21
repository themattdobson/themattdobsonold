---
permalink: /Alexa-Vocal/
layout: page
title:  Alexa Experiments
date:   2015-01-03 21:21
---

In early 2017 I was part of a small product team that partnered with Humana’s innovation team on series of lean experiments to understand how voice technology might augment integrated care delivery and in-home care.

![](https://d2mxuefqeaa7sj.cloudfront.net/s_8A12A285956CF139A6BA188A75B22D63FC72EB68EB97C431743DB4C39574F367_1515945758398_Amazon_Echo.jpg)


**Problem(s)**
The recent wide adoption of voice-driven virtual assistants has created new opportunities to connect with members in their homes. The innovation team identified several areas where these voice assistants could make a significant impact on some of our sickest members.

**Congestive Heart Failure**
To begin understanding how to design and develop for voice we started with members being served by IVR, an existing voice-based technology.  Currently, members with Congestive Heart Failure (CHF) recieve automated outbound phone calls that ask a series of questions to identify exacerbations in a member’s condition. These calls typically have a low response rate and aren’t perceived as being very effective.

Our hypothesis is that we could use a voice assistant, particularly Alexa, to reimagine this experience and make it more effective. Our first steps toward improving the experience was to make it more conversational and dynamics, not the binary decision tree of the IVR menu.

We also wanted to give members more meaningful feedback and another line of communication with their Care Managers. In addition to the IVR contact, many members with CHF also participate in a connected scale program that provides quantitative feedback to Care Managers based on the member’s daily weigh-in. Our reimagined CHF skill used the daily routine of weighing in to prompt a conversation with the member about any symptoms they might be having. Providing vocal feedback to the member would help them understand their condition and provide the reassurance that their Care Managers are aware of any daily changes.

![](https://d2mxuefqeaa7sj.cloudfront.net/s_8A12A285956CF139A6BA188A75B22D63FC72EB68EB97C431743DB4C39574F367_1515956752171_CHF_Storyboard.jpg)


**What we built…**
To facilitate testing our hypothesis we built a working interactive skill that used mock data. We performed a series of in-lab usability testing sessions to challenge tour assumptions about we could improve and evolve the IVR experience using Alexa and a more conversational approach. This prototype skill couldn’t be fully developed or released under current privacy and HIPAA regulations but, it gave us an opportunity to explore and demonstrate how we might more meaningfully engage with our members in their homes.

**What we learned…**
The usabilty tests quickly exposed how difficult it can be to design a conversation.  We found that we had to find a way to be friendly without leaving options too open, frustrating users when the skill can’t respond intelligently.

 It also became quickly apparent that it can be very difficult to account for all of the possible utterances a user might respond with. We saw that seniors had little patience for errors  and we needed to design the skill in a way that it could get the conversation back on track if something was misunderstood. Often, having Alexa humbly acknowledge her shortcomings helped ease the tension with errors.


**Dementia**
In preparation for this engagement with the Digital Experience Center the innovation team lead a ‘friends and family’ study that introduced Alexa’s into homes of seniors. The participants in this study had accesss to the default capabilities of Alexa and whatever skills they added on their own. This small study was designed to determine the viability seniors adopting an in-home voice assistant.

A surprising outcome of the ‘friends and family’ study was the level of engagement with Alexa by participants with dementia. These participants reacted positively to interacting with Alexa and particularly with he ability to play music on demand.

To better understand the lives of our members with dementia and how they were interacting with Alexa we had a series of interviews with both the members and their caregivers. One of the many problems we identified was that caregivers are often overwhelmed with repetitive questions as their loved ones struggle with memory. We observed that many relied on an elaborate collection of notes and reminders to help navigate their homes and lives.



![](https://d2mxuefqeaa7sj.cloudfront.net/s_8A12A285956CF139A6BA188A75B22D63FC72EB68EB97C431743DB4C39574F367_1515958301748_Dementia_Story_1.jpg)
![](https://d2mxuefqeaa7sj.cloudfront.net/s_8A12A285956CF139A6BA188A75B22D63FC72EB68EB97C431743DB4C39574F367_1515958238238_Dementia_Story_2.jpg)


**What we built…**
We explored the hypothesis that by creating a skill That could easily record and replay message that we could help the dementia patient remember important messages. This skill could also lighten the caregivers burden, freeing them to use their time to help in other ways.

From the caregiver’s perspective we kept the experience simple and familiar by providing a phone number hey could call or text to leave a message. For the member with the device in their home they simply had to had to say “Alexa open Message Box” and the skill would play back recorded messages or read back transcriptions from text messages.


**What we learned…**
After some initial demos and usability tests in the lab we piloted the skill in a dozen members. The pilot included both members that were living at home and those that were in assisted living facilities. Our pilot concluded when Amazon released messaging as a core feature for Alexa, overlapping many of the features we’d developed.

There are many challenges in trying to create a voice experience to serve people with dementia. The syntax for invoking a third-party skill can be awkward and difficult to remember for anyone, especially for someone struggling with memory issues. To help improve this experince for our pilot participants we included a set of simple instructional cards with the invocations for our skill along with some of the default features like checking the weather.  

There are some additinal challenges in developing a voice experience for seniors. Many seniors have difficulty with hearing and Alexa can have trouble with accents. In our observation seniors are easily frustrated with technology, those with dementia even more so.


![](https://d2mxuefqeaa7sj.cloudfront.net/s_8A12A285956CF139A6BA188A75B22D63FC72EB68EB97C431743DB4C39574F367_1515956504116_Vocal2.gif)


**Prototyping for voice**

For each of the experiments we needed to be able to test the Alexa skills with users.  We needed to be able to create and refine these experiences we were testing as quickly as we were learning. Prototyping and usability testing is a normal part of our product design process at the DEC but, normally we are designing a visual interface. None of the tools we used for quickly prototyping screen interfaces helped in designing for voice.

At the time there were very few if any viable commercial tools available for prototyping a dynamic voice interface through an Alexa device. Our first attempt at usability testing we used a ‘man behind the curtain’ approach. To facilitate this technique our engineers developed a simple skill that had Alexa speak whatever they typed, that way, as I facilitated the session with the user the engineers could listen in and respond as if it was a fully developed skill.

This approach had some shortcomings. It was difficult to respond quickly, even when choosing from prewritten response, and when there was an inevitable delay in the response Alexa would time out and quit working due to inactivity. Mimicking a working skill also limited our ability to observe the users interaction with the skill when it presented an error or the skill misunderstand the user’s commands.

Our next solution for prototyping came from adapting an open source tool Amazon had developed for making adventure games for Alexa. We took this ‘choose your own adventure’ tool and added functionally that allowed us to quickly create working skills through a visual interface. We dubbed this tool ‘Vocal’. It was exciting to work directly with engineers as we developed and put new features into use as soon as they were built. The new features allowed to quickly design, save, and iterate on skills. The tool was nimble enough that we could update responses during a usability session to present different scenarios to the same user.

“Vocal” made it possible for us to create working prototypes of skills quickly enough to support a weekly schedule of usability testing. We used feedback from each session to refine the experience and interactions. Meanwhile, the engineers on our team developed a working version of the skill to pilot in members homes.






****
****
