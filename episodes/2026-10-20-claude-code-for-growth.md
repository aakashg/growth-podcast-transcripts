---
title: "Claude Code for Growth: Complete Masterclass with James McAulay"
subtitle: "I got him to give away a free Operating System for Growth in Claude Code!"
date: "2026-10-20"
host: "Aakash Gupta"
guests: ["James McAulay"]
speaker_names: "substack"
substack_url: "https://www.news.aakashg.com/p/claude-code-for-growth"
youtube_url: "https://www.youtube.com/watch?v=FTbkpiKWLKw"
duration: "01:07:29"
word_count: 12251
source: "Substack episode transcript (aired audio)"
sponsors:
  - name: "Ariso"
    url: "https://ariso.ai/aakash"
  - name: "Customer.io"
    url: "http://customer.io/productgrowth"
---

**Sponsors:** This episode is brought to you by [Ariso](https://ariso.ai/aakash) and [Customer.io](http://customer.io/productgrowth).

# Claude Code for Growth: Complete Masterclass with James McAulay

*I got him to give away a free Operating System for Growth in Claude Code!*

**James McAulay** (00:00:00)

AI has just completely unlocked what growth people can do. We no longer need to wait for engineers to build growth experiments. You can simply ship to production with permission from your engineers yourself. We're seeing these full-stack growth hires achieve incredible amounts. I think this operating system will help you get better growth results. [music] It's my sort of take on how to work with Claude as a growth person.

**Aakash Gupta** (00:00:33)

Meet James McCauley, who helped Eleven Labs double from 100 million to 200 million ARR in nine months and helped AI startups like Jack and Jill and Wonder Studios with their growth.

**James McAulay** (00:00:43)

When I was at Eleven Labs in 2025, we were definitely ahead of the curve with AI, but actually our launch processes were mostly custom GPTs, and that's because skills hadn't been formalized across the AI ecosystem. How the hell did you scale up this

**Aakash Gupta** (00:00:55)

business to 100k revenue in just four months?

**James McAulay** (00:00:58)

So my first startup was a marketplace. It actually took us six years to reach £100,000 of monthly revenue. My current business hit that goal in 95 days. I haven't hired a single full-time employee.

**Aakash Gupta** (00:01:10)

So you've taught over 400 people now. What do most people get wrong as they're

**James McAulay** (00:01:14)

learning this stuff?

<!-- sponsor -->
**Aakash Gupta** (00:01:18)

Before we get into today's show, please take a second to check that you're subscribed on YouTube and following on Apple and Spotify podcasts. If you want access to all of my favorite AI tools, I've gotten them to give you an entire year of their paid plans. Check out bundle.akashg.com for an entire year of Bolt.new, Airtable, Speechify, Descript, Magic Patterns, Linear, Dovetail, Arise, and Mobbin. And now, into today's show. We've been talking a lot about how you use Claude Code for product work,

**James McAulay** (00:01:54)

but what about all the important growth work,

**Aakash Gupta** (00:01:57)

SEO, ads, product marketing? These are really important skills. And if you are on a growth team, you might've been wondering, how do I apply everything in this channel? If you're a PM at a startup who has to handle growth work, you might've been wondering, How do I apply this to my growth work? Today I've brought in an expert, somebody who's not only grown his own business to $100,000 monthly revenue, but he has helped grow other companies. James, welcome to the show.

**James McAulay** (00:02:24)

Thanks for having me. Really excited to

**Aakash Gupta** (00:02:26)

be here. How do people know what they're going to see right now actually works?

**James McAulay** (00:02:31)

Yeah, in a nutshell, I ran my own company as CEO for 10 years and I was responsible for growth there as the CEO is. And then after we were acquired, joined the Living Labs and spent a year at Living Labs. And for me, that was a masterclass in growth. One of the fastest growing AI companies in history. And I learned a hell of a lot while I was there. After I left, I sort of spent a month going deep on Cloud Code. I did some growth consulting for a few other AI companies. And now I'm running my own business teaching people how to use AI agents to grow faster. So I think my track record checks out and I think I've... I've seen enough companies and I've seen a company like 11 Labs from the inside to hopefully know what I'm talking about.

**Aakash Gupta** (00:03:15)

So what are we going to learn today?

**James McAulay** (00:03:16)

So I'm going to show you the system I use to run my business. 12 months ago, I was still using Cloud Chat like a lot of people, but today I I run everything inside the terminal and I'm going to walk you through the system that I'm using. I'm going to show you some skills. I'm going to show you some tools that I use, some growth experiment discipline for anyone to kind of approach growth in a rigorous way. And also this system I use for making sure that I'm like actually working towards what really matters. I think with AI, it's possible to get distracted. It's possible to go down rabbit holes. Build anything. But I've sort of deliberately engineered this whole harness so that I'm constantly kept on track. And Claude or any agent that drops in here is sort of laser focused on the growth goals.

**James McAulay** (00:04:03)

So I've been using Claude code for this. And if you go into the link at the bottom of this video, there's going to be like a way to download this. It'll be a GitHub repo. And you can just install this in like a couple of commands. This works in Claude code, Codex, Hermes. OpenClaw, if anyone's still using OpenClaw. But I guess, yeah, 12 months ago, I was, you know, like a lot of people, in Claw Chat, I had a project, and I started putting, like, context into this project. And I realized that with the right context, as we all know by now, an AI agent can be incredibly helpful. And so... I'd heard about Claude Code. It was pretty new at the time, but pretty much this time last year, after I left to live in labs, I actually flew to Mallorca for a week, went cycling.

**James McAulay** (00:04:50)

And then when I wasn't on the bike, I was just in the terminal every waking hour for two weeks, just becoming obsessed with this stuff. And so I'll show you... The system that I've spent basically a year tweaking that I run my business through with goals and also with skills and with tools. And hopefully by the end of this video, You'll know how to put it to work and why I think it's worth implementing either my system or something very similar to this. Aakash, where would you like to start?

**Aakash Gupta** (00:05:21)

I guess, how do we set it up? What's the scaffolding here that makes it all work?

**James McAulay** (00:05:25)

Okay, so I've packaged this up as a GitHub repo. It's called Growth Agents, and there's a couple of instructions down here that will get it running. Essentially, what this is is... I've packaged up some of the tools that I think are incredibly helpful for working agentically. I only work with tools that have good APIs or good CLIs. Everything feeds back into whichever agent

**Aakash Gupta** (00:05:53)

you're using.

**James McAulay** (00:05:54)

I've also packaged up a bunch of skills. We can go through some of these. These are skills genuinely that I use, you know, every day. Morning stand-up skill, monthly retro, but also like a good PRD skill, an SEO audit, etc. We can get into that. It's a collection of skills. It's a recommended set of tools. I've got some weekly routines or like cron jobs, depending on how you want to set it up, that basically improves the harness every week. So it looks at the way you're working and it suggests new skills or it goes looking for new CLIs. So I guess you could call this like, yeah, an agentic growth operating system. You could use this if you were like, you know, a full stack growth person, first growth hire. If you're quite specialized product marketer, SEO lead, you can basically onboard. And it will ask you about your goals and then sort of customize all of it to you.

**James McAulay** (00:06:46)

Maybe we start with this because I actually think that this is quite interesting unless you want to go somewhere else, Aakash.

**Aakash Gupta** (00:06:51)

Let's do it.

**James McAulay** (00:06:52)

Okay. So this time last year, I sort of wrote down my Q4 goal and I edited the project instructions in Claude and said, Everything we talk about has to move me towards that goal. And it was really helpful. Like Claude told me when I was getting distracted, helped me prioritize, really helped me with career decisions, actually. I was tempted to go back into full-time work, but I had told Claude that I wanted this freedom to run my own company again.

**Aakash Gupta** (00:07:18)

I've been using Ari from Oriso for a while now, and the thing that hooked me isn't one feature, it's the memory. Most AI tools forget you the second chat ends. Ari doesn't. It connects to my email, calendar, Slack, and it remembers everything. Every commitment I make, every thread I'm on, every person I That's the individual side. The bigger side is what Oriso does inside companies. It coaches managers, keeps teams aligned with the actual And turns all that scattered activity, the meetings, messages, and docs into a clear picture of how execution is really going. Leaders see drift before it costs them a quarter. One brain for you, shared clarity for the whole org. Try Ari at ariso.ai slash akash. That's A-R-I-S-O dot A-I

**James McAulay** (00:08:07)

slash A-A-K-A-S-H.

**Aakash Gupta** (00:08:09)

Every growth team has a funnel they should be watching more closely. Usually it's checkout. Amplitude custom agents will watch that funnel for you on the schedule you set. Let me show you. You start by describing the job. Watch my checkout drop off. The agent builder will ask a few questions to shape it and then the agent connectors plug it into your stack. That part matters. The agent reads the PRD, the tickets, the team conversations, so its analysis actually carries the full context of what's happened. From there, it monitors the funnel on a schedule, and when it spots a problem, it acts. Right here, It files the linear ticket itself. The loop between knowing and doing closes on its own. That's the shift. Set up the agent once and it runs the work. Custom agents are free for all Amplitude customers in open beta right now. There's a library of pre-built agents too, including the exact checkout drop-off investigator.

**Aakash Gupta** (00:09:05)

Start at amplitude.com slash ai-agents. The agent library is linked right there.

**James McAulay** (00:09:11)

And Claude helped me hold the line. And so this year, I've got a big punchy goal for my company. And this goes into a mission file. I then run quarterly OKRs. Don't need to explain those. I'm sure everyone working in product knows what OKRs are. And again, these are documented in the system. They tie back into the mission. I then run a monthly retro. And so at the end of every month, Claude pulls data from all the tools that matter. For me, it's Stripe, PostHog, Xero, Atio. And basically sort of ladders this up and says, like, did you hit the OKRs? And like, are we on track for the mission this year? And helps me sort of like plan the following month. But then week to week, I'm also doing like a Friday retro. And I'm not joking. I spend about... An hour on these weekly retros, usually just with Whisperflow, just kind of like speaking into Claude about what went well this week and what didn't.

**James McAulay** (00:10:05)

And you'll notice here I've said that it takes my personal reflections on like how I feel the week went. And then it takes quantitative measurements from all the tools that are connected to it. So instead of me saying, oh, I feel like, you know, sales are maybe a bit slow this week. It just goes to ATEO and says, we're on track or we're not on track. If I say, I'm not sure if the main landing page is converting, Claude just gets the hard, cold numbers. So I do that every week. And then I have a skill called daily stand-up. If you're in a company, I think daily stand-ups, if they're done well, if they last about five minutes, and if you're actually standing up, they're just really helpful. But when you're working by yourself, You don't have anyone to stand up with. So instead, I do my daily stand up with Claude, and it sort of checks that I'm working towards the biggest goal this week, which ties into the month, which ties into the OKRs.

**James McAulay** (00:10:56)

So this kind of cadence I find really helpful. Growth is all about prioritization. We do not want to get distracted. We don't want to waste time running the wrong experiments. And so I think this system is basically what's kind of like keeping me or you, if you install this, on track. And I've set up a session hook so that when you start Claude, every time it's basically reminding you of your goals.

**Aakash Gupta** (00:11:21)

So these are everything I'm going to show you is sort of fictitious numbers,

**James McAulay** (00:11:24)

just as an example. When you start Claude, instead of getting distracted and going off and Using Astra to build some 3D game that doesn't matter. It's going to remind you that, look, here's the mission. And this is what you said we would work on this quarter. It's going to push back. Basically, when you install this, your Claude.md will get sort of customized. And so if Claude sees you getting distracted, it's going to sort of pull you back on track. So yeah, I guess you could think about this as having your own growth lead who is just repeatedly saying, is this a 10x bet? Is this going to move the needle? Why did you get distracted this week? Is there anything you want to get into on any of that?

**Aakash Gupta** (00:12:05)

Well, I have to admit, I have tried this, the weekly review, the daily stand-up. I haven't tried the quarterly, monthly part of it, but what I found was that AI would miss certain context about And so unlike a human where I felt like the standup and the retros were useful for alignment, I have kind of stopped using these skills just sticking to execution. You're not the only guest who has emphasized how important these are. So can you convince me, like, why should I be using AI as a thought partner for all these retros and stand-ups?

**James McAulay** (00:12:46)

I have iterated on these skills. You know, the one I use most often is weekly retros. Like, I sometimes forget to do a stand-up. I'm going to be honest, like, the stand-up is maybe like the sort of least valuable one, and I often forget to do it. But the weekly retro, I am religious. I think I've done like 10, 15 of them over the last 10, 15 weeks. So... For me, it basically notices patterns. And I'll give you an example. Technical or engineering-minded people, I sometimes overbuild. I'm sometimes keen to just go and add more features, and that's not what is actually going to move the needle. And so Claude noticed after two or three retros, because it can see my to-do list, I've got it connected up to Todoist, could basically see that there were certain outreach or certain marketing tasks that were just stale every week.

**James McAulay** (00:13:35)

And then it would look at GitHub and it would say... Hang on, you've shipped so much that we did not need to ship. You've refactored part of your platform for no reason other than it was fun to refactor. So I guess for me, I think it's helpful just in spotting blind spots and basically being held to account on what you say matters. Because I do think this is one of the biggest risks with AI now is that we can build anything, right? It's not an exaggeration to say that if you or I sat down You know, tomorrow morning we could have a working sort of MVP or like a feature by the end of the day. But if nobody wants that feature, if nobody wants that product, we've wasted our time. So I think it's I think staying on track and I think like spotting your own patterns of maybe avoidance or procrastination or doing fun stuff instead of doing the stuff that's really going to move the needle.

**James McAulay** (00:14:30)

Personally, I found Claude very good at holding me to account

**Aakash Gupta** (00:14:34)

on that. Okay. Well, maybe I'll have to give it a try with these updated skills. Maybe my skills just weren't very good. And maybe you can show us later what the output looks like. Yeah, of course. All right. So how do we spin up our first agent? Okay.

**James McAulay** (00:14:48)

So let's try a live demo. I've basically set up a sort of folder of context for a fictitious product marketer. Let's get into Claude.

**Aakash Gupta** (00:14:56)

And you're in iTerm2. Why iTerm2?

**James McAulay** (00:14:59)

I just quite like some of the themes in iTerm. It feels like quite a fast and snappy terminal, but I mean, it's basically the same. It's basically the same as Terminal. I'm going to get people in the comments saying it's not the same as Terminal. But I think I installed it like 15 years ago when I was doing computer science at uni. And every computer I've had since, I've just installed iTerm and then moved on to iTerm.

**Aakash Gupta** (00:15:22)

Have you tried like a VS Code or something? Like how should people be thinking about where you run

**James McAulay** (00:15:27)

Cloud Code? When I was learning Cloud Code last year, I was doing it inside Cursor. And so I had my files in the middle, agent on the right. And maybe I'm going to get hate for this from engineers as well. But I realized very quickly that I wasn't reading the files. Like I was setting up tests. I was inspecting all the front end. I was basically managing the coding agent, but trusting that with the right testing harness, it couldn't ship something that would break. And eventually I thought, well, I have this full screen, right? I've got my full desktop screen, but I'm only using this column on the right. I'm ignoring all this. Why don't I just run terminal as my preferred way of running cloud code? I also think that the cursor pricing... I was running Claude code through Cursor, and I remember very quickly, you know, they were trying to move me up the pricing levels.

**James McAulay** (00:16:23)

And I think just running Claude code, $200 a month plan inside the terminal was the fastest way to do it. And so I'm going to show you a demo here, right, where I've got like one screen. I've got this nice plugin called Claude Heads Up Display, just keeps an eye on my context, reminds me which branch, which work tree I'm in. But when I'm at home, I have like Super wide screen, and I will often have two windows like this, or maybe five. It's definitely not the most aesthetically pleasing way to work with agents, but I find it just snappiest, fastest. I don't like the Cloud Code desktop app.

**Aakash Gupta** (00:16:59)

I find it just a little bit clunky compared to this. Cool. So let's get this agent spun out.

**James McAulay** (00:17:04)

Okay, so hopefully this is going to work. I've set up a demo folder. It's got a bunch of context on what this person's trying to achieve. I've designed this in a way that it will interview you about your goals. It will ask you where your goals are. Are they written down somewhere in Asana? Are they in Google Docs? Are they in your head? And it will try to crystallize all of this for you. And then basically, we'll sort of Pressure test your goals and set up like a folder for growth experiments. If I come back to here while this is just working, I've set up a bunch of rules around like how to run growth experiments. I don't know if you've tried this, I've actually found that Claude is a very good sort of analyst of data. And we want to make sure that our A-B tests are not only statistically significant, but set up correctly.

**James McAulay** (00:17:55)

We want to make sure that we don't prematurely read the result of an experiment. So I've sort of packaged all of this up into a set of rules. And then I've also set up this loop that basically makes sure all your experiments get closed. So I don't know if this happened to you, It's very easy to start a growth experiment and then get distracted by shiny object syndrome and basically forget to close it. And so like you try something and you never close the loop. Or, you know, you get to the end of the year, you have run like a bunch of growth experiments, but they're not documented. So, you know, you've got a bunch of post hoc experiments, but you haven't actually documented the learnings. So this system is constantly asking you and looking at the data, you know, Can we conclude this? What did we learn?

**James McAulay** (00:18:42)

Let's document it. Let's use that to inform the next growth experiment. So it's trying to hold you to account, basically. If you start something, make sure you finish it and make sure that whatever you learn is documented so that the next experiment is better.

**Aakash Gupta** (00:18:58)

How often do we forget that, right? It's so easy. And that's actually where that alpha is, is figuring out, okay, this one failed, but here's why. And like you said, I think Claude is pretty good at having like a rigor around these experiments. Like once I ran an experiment, it was like, oh, wait, but here's this confound. So we have to actually look at this media mix model in order to look at it. So it's actually pretty smart at that point.

**James McAulay** (00:19:22)

Yeah, it's really good. I've seen this play out, you know, in my first company, We'd run a bunch of experiments, and we wouldn't document them very well. And then we'd hire someone new, and they would say, oh, I want to experiment here, this part in the funnel. And we'd say, oh, sorry, I already tried that. And they'd say, cool, where can I see the results? Well, we can tell you that it didn't work, but we don't actually have it documented.

**Aakash Gupta** (00:19:47)

I think with AI now there's kind of no excuse for not documenting stuff.

**James McAulay** (00:19:51)

Okay, so we've run this setup and basically the agent has sort of looked through the folder that it's been like started in. So I imagine most people watching your show have got their own, maybe it's a second brain, maybe it's like one folder on their computer that's got all the context they need. But I'm not trying to like get anyone to create a new folder. This is basically going to like run inside your existing folder. And it's read through and it's saying, okay, here I can see that you've got some OKRs already. This is good. You know, you want 6 million net new ARR. You've got some OKRs on Q2, but I don't see anything for Q3. I don't see anything about like what your focus is this month. You've written some notes about this week and maybe some Q4 planning. A couple of tests I can see that you ran, some information on the business and I've done an audit and I have some sense of what you're trying to achieve.

**James McAulay** (00:20:51)

Now it's asking me, do you want to do a rapid setup where I ask you quick questions or do you want to do a full setup where I interview you about everything to do with your role and I get full context? For the purposes of this demo, we should probably do Rapid, but when I teach people how to use co-work or code properly, the first exercise I do is getting them to do an interview with Claude that takes up to two hours. It feels like a slog. It feels, you know, like you're just answering loads of questions. But in doing that and having Claude basically sort of structure your context in a second brain, every answer, every question from there on out is better. I was just doing the full onboarding and just like switch on Whisperflow, just talk out loud. But for the sake of the interview...

**James McAulay** (00:21:46)

Let's do some rapid onboarding. Fingerprint is exactly that.

**Aakash Gupta** (00:22:02)

Accuracy is the number one reason customers choose Fingerprint, because their device intelligence goes deeper than identification alone, resolving visitors with precision that holds up through spoofing and evasion attempts for months at a time. Fingerprint collects more than 100 signals across devices, network, and behavior to build a single identifier. Then provide signals like bot, agency, proxy, and VPN detection to give technical teams a complete picture of risk. They ship hundreds of product updates a year, so they adapt first as browsers update, privacy requirements change, and fraud tactics change. With one API call, teams can get this running in minutes. Over 6,000 companies rely on fingerprint every day. Join them now at fingerprint.com. I used to think I had a retention problem. Turns out I had a messaging problem. I was sending the same onboarding emails to every new user, whether they activated on day one or never logged in again.

**Aakash Gupta** (00:22:53)

I had no idea who was slipping or why. Customer.io changed that. Every message I send is now based on what users actually do in the product. Someone hits a key activation They also have an MCP server, which means AI tools like Claude can see directly what's happening in your customer.io workspace. Your segments, your customer data, your attribution, all of it. So instead of explaining your business context every time you need help, Claude already knows it. Notion used Customer.io to personalize their onboarding and hit nearly 50% open rate. [music] The idea is simple. Customer.io helps you deliver more impact from every message you send. If you're a PM or founder and your onboarding is still one size fits all, try Customer.io at Customer.io. Imagine learning AI product management, AI product strategy, AI product leadership, advanced PM with cloud code, all from frontier leaders at OpenAI, Anthropic, and Google for less than $10 a day.

**Aakash Gupta** (00:24:14)

Actually, you don't have to imagine it. That's exactly what Product Faculty's AI Builder Fellowship gets you. One yearly membership, six live cohorts. Not recorded videos or another content library you never finish. Real live sessions with frontier AI leaders, hands-on AI build labs, executive Insight sessions, capstone projects, unlimited retakes, and continuous access to new programs as the AI landscape evolves. You'll also get every new certification they add while you're a fellow at no extra cost. The goal is simple, help you master frontier AI skills to become an AI native product builder and operator, not just someone who talks about AI. Purchased separately, these programs are worth more than $19,245. The lowest price certification alone starts at $2,700. But founding members can join the entire fellowship for less than $3,600 per year. That's less than $10 a day. Soon, the price increases to $5,000 a year. So if you're serious about becoming the person your company turns to for AI, this is one of the highest ROI decisions you can make this year.

**Aakash Gupta** (00:25:25)

Join the AI Builder Fellowship at ProductFaculty.com.

**James McAulay** (00:25:30)

Okay, so it's saying, yeah, you're a growth lead. I don't really know, like, sort of what your core objectives are. And it's saying here, do these exist already? Like, are these in Notion? Are they in Asana, Linear? And then it's also noticed, you know, you exported some data from Analytics, like, Is there a tool I can connect to? So I'm just gonna say quick demo to make sure that it doesn't go too deep into this, but no Q3 objectives actually written down, and data from post hoc. So yeah, it's gonna piece together all of this stuff, and then you're gonna have, let me just come back to here. It's going to say, okay, cool. We got these skills. Do you want to do a daily stand-up? Probably not. And the skills I've sort of put together, we've got these content skills that I use all the time, like a tone of voice skill that sort of interviews you, asks you for examples of your tone of voice.

**Aakash Gupta** (00:26:33)

I'm sure people have talked about that on your show before.

**James McAulay** (00:26:36)

I do a lot of YouTube, as you do, for growth. So I've got a skill that basically does the package, the title, description, the keywords, the research. I've got a skill that looks at competitors. There's some stuff in there for anyone doing YouTube. You mentioned SEO at the start of the call. I've basically remixed a really good skill by a guy called Corey Haynes. Do you know Corey Haynes? So he has done, he's done this amazing set of skills called Marketing Skills. I definitely think you should get him on the show. And his most popular one is SEO Audit. So I took this, I've sort of like put my own spin on it. I noticed, for example, that like if you ask Claude to scrape a website, it often hits like Cloudflare blocks or like doesn't read the website accurately. So one of the tools that I've suggested installing for anyone doing SEO is Firecrawl, just like turn any website into an MD file.

**James McAulay** (00:27:33)

And then also data for SEO, which is this like Dirt Cheap SEO API. I can't believe how cheap it is. You give Claude Code the API key and it can just research like any term for like a few cents. So I've like kind of wired those into the SEO audit.

**Aakash Gupta** (00:27:50)

So you don't recommend like whatever $100 age refs subscription or something when you can just do it in cents for whatever you need from data for SEO?

**James McAulay** (00:28:00)

No. I've been, you know, my company used SEMrush and then I live in labs. I think we used SEMrush. But I noticed, you know, I've done years of SEO work. They were basically like the same tasks. I just wanted to see like my performance over, you know, certain keywords. I wanted to know our keyword gaps. I was often wanting to like put together a keyword universe. I found it so clunky in those tools to actually kind of like put together a keyword universe. Whereas with Claude, I said, you know, analyze my website, analyze competitors, use data for SEO to create a keyword universe, and then we will like attack the keywords that matter. So yeah, do you have a website? Like, do you have a personal website? What is it?

**Aakash Gupta** (00:28:45)

Www.news.akashg.com.

**James McAulay** (00:28:53)

Okay. So yeah, I think this skill is amazing. And not only is it going to analyze your backlink profile, not only is it going to look for basic stuff like, are your H1s correct? Are your links correct? It's also going to do a page speed analysis. So I don't know how much you know about SEO, but there's a Google tool called Lighthouse, measures like how quick your website loads. You used to have to like go to page speed, their website to kind of like get a test, export the test, save it, give it to the agent, and then ask the agent to kind of like make the change. But this uses the Lighthouse CLI. So it basically just like Tests it for you, pulls all the data, looks at, you know, if it's inside your repo, so I'm doing a sort of like outsider test on your website, but if I run this inside my own code base, it immediately finds ways that we can like speed up Our website, which actually matters quite a lot for SEO and helps with conversion.

**James McAulay** (00:29:52)

I think there was a study that said, you know, every second of load time that you can like reduce has this kind of like proven gain in conversion. So anyway, I think this is like a really good skill. You can see here it's just kind of like crunching through. Maybe we can come back or I can send you that afterwards. But this is one I, this is genuinely one I use all the time. I used it on my own website a few months ago. I used it this morning. I literally deployed a new page and just ran SEO audit to check that again, it was like done correctly. So yeah, one of my favorite skills, if you pair it up with data for SEO.

**Aakash Gupta** (00:30:30)

Can we go back to the agent that we spun up and that was pulling your context and just close the loop on how to build sort of like an autonomous growth agent?

**James McAulay** (00:30:39)

Yeah, of course. So I guess I want to manage expectations here that these are not fully autonomous growth agents. You can set up these skills to run on a schedule. You can You can take any of these skills and you could create an agent using something like Vercel's eFramework, OpenClaw, Hermes. My system is not really like this agent is 24-7 sitting on my Mac Mini doing work for me. It's like I am in the driving seat and at any time I'm sort of like sending this agent off to do a piece of work that might take an hour. And then I'm like sending this one off that might take, you know, another hour. I've, you know, for example, the SEO audit, I have a cloud code routine. So if I've shipped something that had a negative impact, then it sends me an email and it says there's been a regression and that was an agent that sort of woke up Sunday, ran the test and then like sort of shut down.

**James McAulay** (00:31:44)

But yeah, basically what I've, this is more of like an operating system. Like if you're going to be doing work inside of Claude, I think this operating system will like help you get better growth results. And it's my sort of take on like how to work with Claude as a growth person.

**Aakash Gupta** (00:32:00)

So are autonomous agents overhyped or are they just not there at quality or why do we just have kind of like this schedule on skills?

**James McAulay** (00:32:08)

That's a really good question. Overhyped in that I reckon like a lot of the people telling you on LinkedIn and X that they have, you know, autonomous agents doing stuff for them. They're either like burning tokens on sort of like kind of useless stuff or, you know, these agents are maybe like going out to scan a competitor and sending a briefing back. But in my experience, like people are using these kind of autonomous agents to basically like summarize information once a day or like once a week. You know, I think we've both seen instinct go kind of viral on X over the last few weeks. I wouldn't call instinct autonomous in that I don't think it just decides to go and do a piece of work for you. These agents are at your beck and call. You give them a command and they can go and spend two or three hours, 24 hours on a project.

**James McAulay** (00:33:00)

I'd say that's, you know, like relatively autonomous. But the idea that we have these agents that we sort of create and then they just go off and like print money for us without us sort of doing anything, I think is a little bit of a fantasy and maybe some kind of overhyping on Twitter. What about you? Like, do you have any agents that are sort of doing stuff without you really sort of steering them? Or is it like this kind of direct the agent, have them work for a few hours, come back?

**Aakash Gupta** (00:33:28)

I am painfully bad at focusing on growth stuff. All I focus on is content, content, content. So the only thing I have is like a couple of schedules. Like I look at something religiously called like my LinkedIn post lab, which basically I have a schedule which pulls from a hundred creators who I follow on LinkedIn every morning. So I don't actually browse LinkedIn really. I just browse my LinkedIn post lab and I actually host it on my website. And so that's just a schedule. And then I have a couple loops running. The idea with these loops is that they're gonna go look at the feedback that I give them to become self-improving. So they're not autonomous in the sense that they're not doing anything without my review. But I do have, for example, a loop that's focused on helping me figure out what I'm going to post on LinkedIn.

**Aakash Gupta** (00:34:22)

And so it'll go look at my post performance yesterday and it'll automatically update itself and say, okay, You tried this. Like, for instance, realistically, yesterday I tried, hey, what if I post two posts instead of one post per day? One link post and one image. What's going to happen? And so this morning it came back to me and said, hey, your net impressions were actually lower than one post a day. So maybe that experiment didn't work. And so here's what I'm proposing you write about today. You just published this deep dive. You should write about that.

**James McAulay** (00:34:52)

I mean, you said you're not doing much growth, but that sounds very scientific.

**Aakash Gupta** (00:34:57)

It sounds like you're doing You're doing content-led growth, right?

**James McAulay** (00:35:00)

And you're trying to iterate, you're trying to run experiments. I think you're underselling what you've built slightly. And that sounds cool. I think we could call that sort of proactive agent. You could say it's autonomous if you were sort of using the term liberally. But as we both know, it's probably a skill that runs on a schedule. Does the same thing sort of every day. And that can be powerful. But yeah, I'm not claiming that if anyone installs this, they can sort of like retire and just have agents like run their business for them. I think this is like, I mean, I feel like I had

**Aakash Gupta** (00:35:38)

an analogy for this recently, but.

**James McAulay** (00:35:40)

Yeah, my day-to-day is like five or six tabs, sending off different pieces of work to Claude Code. Sometimes I use like GLM or Kimmy if like Claude is down. But the whole harness around this is basically what is like, you know, sort of nudging me towards the goals and sort of making sure that we like document and learn from what we do. And in these skills, you know, you can spin these up as sub-agents, you know, but you could set them up as a schedule, but I'm not sort of, I'm not claiming that this is like an agentic team that runs itself. Not yet, anyway.

**Aakash Gupta** (00:36:15)

So maybe can we circle back to the SEO audit? I think there we'll find that I don't focus on SEO quite enough.

**James McAulay** (00:36:23)

Okay, so yeah, one thing I forgot to do here is I forgot to ask for this as like an HTML report. But we got some issues. So, well, it thinks that the issue is a lot of your posts are paywalled, which is probably intentional. Apparently, a lot of posts don't have SEO descriptions. And there's a bunch of stuff about, like, crawlability. Some of your titles are quite long. There's, like, some duplication going on. There's quite a lot of good stuff here. And I remember 10 years ago, paying SEO agencies quite a lot of money to come back. It was a report like this, like two or three weeks after we'd engaged them. And then I remember giving a report like this to my developers and waiting two or three weeks to have it all prioritized, backlogged, built. Whereas now, if I sent you this report, you gave it to whichever agent is inside your repo and said slash goal, test and refine until all of these are solved, it would do it.

**James McAulay** (00:37:22)

And so in about a couple of hours, we've just tidied up your SEO presence

**Aakash Gupta** (00:37:26)

quite a lot. Does this match what you were expecting? Well, I'm actually literally in the process of looking at what happened to my SEO because in May I was getting like 25K visits from SEO and it's down to like 10K. So these are all great next steps for me and I'm literally...

**James McAulay** (00:37:44)

Yeah, definitely. I don't have your email to hand, but I will like, I'll send this to you straight afterwards.

**Aakash Gupta** (00:37:50)

I mean, a couple of things that I think are interesting.

**James McAulay** (00:37:53)

So we could talk about my PRD skill. I mean, effectively, everyone in your audience knows what a PRD is. I don't think we need to go into this in too much detail. But again, like I said earlier, Mine just really grills you on like why you want to build something. So, you know, there's the famous five whys test. I think it was like Toyota that came up with this where they were actually using it to like get to the root of a problem. So something happened and they'll ask like, well, why did that happen? Okay, well, why did that happen? And eventually you get a kind of root cause analysis. I've taken that and I've basically like pointed it back at the user and said like, why do you want to build this? So for example, I want to, you know, let's say I want to like build a new page on my marketing site.

**James McAulay** (00:38:37)

And Claude will say, okay, cool. Like this seems like it might be a good idea. Tell me why, like what metric is it going to move? And I'll say, well, I think, you know, it might rank for this term on SEO. And then it will sort of look at the data and say, the volume isn't actually that high. Are you sure you want to build it? And so sometimes it's trying to talk you out of building something, but then basically you Once it's got the PRD, it's set up in a way that it's got all these checkboxes and the PRD and it just basically sort of ticks off its work as it goes. And so if you hit a context limit or you need to like kill the session and you continue after that, the agent just looks at the PRD and it sees, you know, I'm halfway through and then just keeps going.

**James McAulay** (00:39:14)

So I think this is like... A good PRD skill, but we don't need to sort of dwell on it too much. This is something that I use all the time, multi-agent refine. I don't know if this visual is like the best visual, but basically when I've written a PRD, when I've created anything, when I've built something that I think is like quite critical, like payments infrastructure, I'll run this skill that basically spawns sub-agents. It could be three or four, sometimes up to 10. And they all just take a slightly different lens. And so one of them is maybe looking for technical correctness. One of them is asking if we missed anything. One of them is looking for simplicity. So if I'm building something, then it's these sub-agents in an engineering sense. But if I'm planning a piece of growth work, then this multi-agent refine Basically takes a few different approaches on growth strategy and then comes back and says, okay, your plan is strong in this area, but the critics, the panel of critics found these weaknesses.

**James McAulay** (00:40:20)

And as soon as I created this skill and started using it, I don't think I've stopped using it on a daily basis because even Fable, even Astra... You can miss quite big things. I think the sub-agent that I find particularly helpful, I don't know, yeah, here, this one missing.

**Aakash Gupta** (00:40:40)

Often we will sort of have an idea, we'll go to an agent and we'll say,

**James McAulay** (00:40:44)

let's build this, maybe interview me before we build it, write the PRD. But it's kind of like we don't know what we don't know. And so if you ask an agent what's missing from this plan, It very often surfaces things that you hadn't thought of and that your primary agent hadn't thought of. So yeah, I love this skill. The one thing I would say about this is make sure that you're using Sonnet subagents. I accidentally spun up like 20 Fable subagents yesterday and just immediately hit my limits.

**Aakash Gupta** (00:41:18)

So yeah, make sure you're using Sonnet or Opus subagents for this one. Can you show us that in action?

**James McAulay** (00:41:23)

Yeah, let's see what we've got here.

**Aakash Gupta** (00:41:26)

Okay.

**James McAulay** (00:41:31)

So we got this. I don't know if this is going to open at the moment. But we've got their Q2 Growth OKRs, right? And so I'm going to say Multi-Agent Refine OKRs. And so I use this quite a lot for strategy planning documents. And so it's going to spin up maybe like four. Actually, let me do this. Let me just switch this on it so that all our demos happen faster. OK. Okay, so it's going to spin up, I think, five sub-agents to critique our OKRs. Now, as I've mentioned in the GitHub repo, there's some stock sub-agents that I use all the time, like what's missing, is this feasible? You can also, if you want, I've seen people set up their panel of advisors, like Paul Graham, Hormozy, like whoever you look up to, you can basically train an agent on their writing. And then when you run multi-agent refine, it will sort of like approach it as they would.

**James McAulay** (00:42:35)

So what it's going to say is it's going to say, do you want autonomous improvements? So like it's going to run a first pass. The master agent is going to like review the results and then just go and fix it for you. Or do you want to be involved? Like, do you want to kind of like see the critics results and then like decide what you want to change? I use both. But for this one, let's say like we'll sort of check in. It's, you know, notice that we are critiquing Q2 goals in Q3, but this is this is just a demo. So, yeah, it's looking for like, are these OKRs measurable and rigorous? Are they feasible and do we have capacity to do them? Are they aligned with the mission? Have we missed anything from these? And then, yeah, those are the four. So they're running here.

**James McAulay** (00:43:21)

You can see these are sub-agents. This one, you're a skeptical critic reviewing this company's growth OKRs. You are only, oh, okay, it's back. Sonnet is fast. So it's found a lot of problems here, right? This document is stale. I mean, that's an obvious problem. There's a note in the retro that undermines these numbers. Bunch of technical things about qualitative judgment instead of quantitative judgment. I've seen all of this happen before, right? When teams write OKRs, it's not set up to be measured correctly, or they've hedged some of the numbers because the wording of the OKR was wrong. So yeah, these agents have just finished, actually. I forgot how fast Sonnet 5 was. And so now our main agent is like synthesizing what they all found. And it's going to come back to me and say, okay, like P1s or even P0s, like you need to fix these things in this document.

**James McAulay** (00:44:13)

P1, P2, and then like P3, you can certainly leave that out. And again, just like adversarial review, this is called adversarial review, always, in my experience, surfaces like far more than just getting one agent to kind of like review its own work. So it's come back here and said, you know, numbers are still again. It's not actually linked up to company OKRs. We don't actually know if this person's OKRs are helping the company OKRs and et cetera. So you can run this and then it will say, which of these do you want to change? And you can sort of go through. I think you have to try this skill out to kind of like experience the magic,

**Aakash Gupta** (00:44:49)

but trust me, this is a very good skill. So should you be running like multi-agent review on the SEO audit or when should you be running that?

**James McAulay** (00:44:58)

Let's go to this example. Yeah. So it's basically, it's found these issues. If this was my repo, I would then... Turn this into a PRD. And the agent would go and research the code base. It would research the audit. It would put together a phased PRD. And then I would multi-agent refine the PRD. So... Audit, PRD, five sub-agents attack the PRD. And usually, yeah, they'll kind of find improvements and maybe things that the first agent missed. So I'm often using multi-agent refine in this planning phase just before I then hand the plan over to the build agent or client.

**Aakash Gupta** (00:45:38)

And then once you have multi-agent review, how do you get it to do the kind of the disciplined experiment process?

**James McAulay** (00:45:44)

Yeah. So this is all sort of built in. If I just come in here. So we've got this like template here, you know, our hypothesis, if it's tied to a key result, like the baseline, the primaries, you know, any confounders. What might make us stop this experiment? Like this alone, I wish I'd had this, you know, like many years ago when I was sort of running growth in a small startup. Just this alone will force you to be rigorous in your experiments, right? And then we've also got like a playbook on A-B testing, maybe with like specific stuff on your site. So if I was in this demo, let's just like close this off. Help me set up an experiment for top of funnel. Landing page conversion, want to test, exit popup. So with all these rules, with all of these kind of templates, it's just going to make sure that your experiment is documented correctly.

**James McAulay** (00:46:45)

And then all the skills I showed you Weekly, Retro, even Daily Stand-Up, they look at the list of running experiments and kind of ask you to, you know, they'll say this one's finished. Like, shall we do a review of it? Or this one's gone stale. It was supposed to finish two weeks ago and you haven't documented it.

**Aakash Gupta** (00:47:01)

So the whole system is kind of like looking to make sure that these experiments get wrapped up.

**James McAulay** (00:47:06)

So in this example, you know, it's asking me for baseline conversion rate. Traffic, et cetera. Nobody should be answering these questions manually, right? This is all data that should come from PostHog, Mixpanel, Amplitude. So in this demo folder, I haven't got PostHog set up, but I've referred in this like set of tools. PostHog is like the first tool that I recommend everyone set up. Have you used PostHog yourself? Have you used it in product work? I use it. Yeah, it's so good.

**Aakash Gupta** (00:47:33)

And in particular, I feel like there's so much on the free plan, which is so nice.

**James McAulay** (00:47:37)

You're literally the second person to say this to me in 24 hours. Like, they're very generous with their free plan. And in fact, I think I only upgraded last week because I wanted, you know, retention past 12 months. But they have built just like a stunning MCP, API, CLI. They've got like a sort of PostHog wizard now that you just like one line into code code and PostHog will sort of, you know, run all your experiments for you. I mean, just to show you mine, I... Created this post hoc account at the same time as I was like discovering Claude Code. And so I haven't created like any of these dashboards. Claude Code has done all of this through the API. Similarly, you know, with my experiments, I haven't created these in the UI. Basically Claude's API key has permission to do this. It's set up the measurement.

**James McAulay** (00:48:26)

We're waiting for our test. So far, our test isn't quite working as we wanted it to, but it's still got loads of time left. So yeah, like PostHog plus Cloud Code is to me just like a growth person's dream. I also think, you know, if you're a growth person, try to get, try, try, try to get at least read-only access to your company. Like, Git repo. Like, your team might not let you ship stuff, but if your agent can see all the event definitions in post-hog, then, you know, it can basically sort of help you measure absolutely anything. But if your kind of post-hog system is a bit of a black box, you know, if you're a growth person that only has the UI and cannot see the code, you're often going to be, like, pinging engineers on Slack saying, like, When do we fire this event?

**James McAulay** (00:49:13)

And when was this event last updated? And why have we got two of this event? Whereas if your team just give you a read-only key for Git, you can just answer all those questions yourself.

**Aakash Gupta** (00:49:23)

What are some tips and tricks to get the most out Okay,

**James McAulay** (00:49:28)

so definitely what I just mentioned about having access to your code base, if you can, even if you're not going to be writing code or shipping PRs, just get access to Git so that you can understand how events are firing. If you're shipping PRs, whether you're a sort of product person, growth engineer, I have set up a bunch of tests in my CI, so like continuous integration. When I push a PR and all the tests run, one of the tests is that everything has to have a post hoc event. So I cannot merge code into production unless it has all of the post hoc tracking set up because I know that I'm going to forget this. Like I'm going to be excited about a feature. I'm going to create a new landing page and I'm just going to forget about PostHog. Whereas like right in, you know, day one of setting up this repo, I thought, okay, what is the system that means I never forget PostHog events ever again?

**James McAulay** (00:50:21)

And the system was, you know, a test when we submit a PR. So I'd highly recommend doing that. So you don't need to think about, you know, adding new events. And then something else I did, I'm trying to remember where it is in the UI. And again, I don't use the UI that often.

**Aakash Gupta** (00:50:35)

It's mainly like, Through Cloud Code, right? That's how I use it.

**James McAulay** (00:50:40)

Oh, yeah. Yeah, yeah, yeah. This is me showing the UI because we're on screen and it's slightly more interesting. One thing I did last week that was really helpful is I basically wrote very good definitions for every event. So I was good at creating the events and, you know, every event existed. I hired an agency who We were doing some A-B tests across my funnel. And they were in post-hoc chat. And I noticed that one or two things were getting misinterpreted. And it was because we had event names, but we didn't have event definitions. And so I basically... Wrote a PRD where I said, okay, like we're going to define every single event. I want you to like scan all of them, make the plan. Then I multi-agent refined the PRD just to check that we were like taking the right approach. And now I can see every event says, you know, when this is fired, where it's fired, use this for, you know, measuring these types of things.

**James McAulay** (00:51:35)

And every single event in my entire sort of list of 350 is documented. Now, pre-AI... You'd only have this if you were working with like a God tier product manager, right? Like I just, I don't think anyone's data would be sort of this well annotated, but this was a task I did in about two hours last week across like five different things I was doing. So yeah, highly recommend just making sure your data, it's a bit boring, but make sure your data is like well labeled, well annotated.

**Aakash Gupta** (00:52:05)

What's like the right prompt here to Cloud Code? Like Audit all of my telemetry and event definitions, figure out gaps where we should create new events, figure out places where our definitions are wrong and help update something like that. That was perfect. Yeah. Basically,

**James McAulay** (00:52:22)

I mean, if you like, I can go back into Cloud Code and find the exact prompt and we could show it on screen. But what you've just described would absolutely work. And just when you do that, just make sure, you know, I'm not going to go into my API key settings right now, but just make sure that that key has the ability to, like, read and write to your, like, event definitions.

**Aakash Gupta** (00:52:43)

So you've set up this agentic growth OS. A lot of people... They might just be getting access to the tools to set it up. You've made the mistakes along the way. What are the big mistakes and learnings that people can just speed up their process by learning from your mistakes?

**James McAulay** (00:52:59)

So when I started working with CodeCode, I think like everyone, I felt like a caveman that had discovered fire. And I kind of like fell under the spell of Claude Code and thought that it could do anything and I could solve any problem. And I realized that, you know, we've all experienced this, but like Claude will confidently give you information that's just wrong. And it will introduce bugs even when you're supposed to have tests. So I guess one thing on, you know, if you're doing this in any sort of technical capacity... I now use Cubic as like AI code reviewer, which just like makes sure I'm not shipping bugs because I had one or two bugs that were like, they didn't cost me money, but they were like quite annoying. So definitely, yeah, Cubic. And I also use Sentry for error reporting. So I highly recommend if you're going to be writing code, you know, don't trust Claude on its own.

**Aakash Gupta** (00:53:53)

I've said here, you know, you

**James McAulay** (00:53:54)

can use any agent here. I'm primarily in Cloud Code, but like this is all set up in a kind of agent agnostic way. So like I do also open Codex sometimes and just kind of like keep working in this folder. I think my biggest piece of advice is like get everything connected as fast as possible. So like this is another diagram, right, of like my setup. And I've got, you know, Century, Cubic that I just mentioned here. Playwright is great for kind of like testing stuff. But I think a lot of your audience aren't even writing code. So, you know, I've also got all my like content tools, right? Like 11 Labs, Epidemic, Mistral. On Analytics, I've got like VidIQ, Data for SEO. Like I would recommend just trying to plug everything together. Into cloud code, like giving it full context across every ecosystem you work in is what kind of like helps it move at an incredible speed.

**James McAulay** (00:54:46)

You know, yesterday, I don't know if I've got it here. Yeah, I use Kit for my mailing list. And I was thinking, oh, wouldn't it be cool to get like an alert in Slack every day that shows me people who engaged with an email, right? So I've like sent an email to like a thousand people. Show me the people who've engaged. And then I thought, well, actually, I don't want just everyone. I want people who haven't bought from me before. And also, I want them to be enriched. So I want to use something like Apollo to see their LinkedIn, to see their profile. And I want to use Atio, my CRM, to kind of check who's paid and who hasn't. Now, if I hadn't connected all those tools, that would require an engineer and That would just be a painful exercise. But that was a prompt.

**James McAulay** (00:55:29)

Yesterday, I sent that prompt saying, I want a daily Slack alert that sends me non-booked leads enriched with Apollo with a link to Atio. I'm not going to show you. I could show you on Slack, but it's got... It's got emails, so I'm not going to do that. And that flow is so helpful for me and for someone who's helping me with sales at the moment. And it's only possible because everything is plugged in to Cloud Code, whether it's an official MCP, an official CLI, or just an API key. If you give Cloud Code an API key, it will usually... Work wonders

**Aakash Gupta** (00:56:05)

for you. Wow. So we talked a little bit about this at the beginning, but I want to circle back this. How has this stuff evolved since you were at Eleven Labs?

**James McAulay** (00:56:16)

Yeah, I was at Eleven Labs in 2025, and we were definitely ahead of the curve on AI. And in 2025, being ahead of the curve meant using custom GPTs. You know, skills, if I'm correct, you can fact check me on this, but I'm pretty sure that like skills as a concept were really formalized in like autumn last year. So for the majority of last year, you know, people weren't using agent skills. We had a few different custom GPTs. We had one for... Just making sure that like copy was on brand, for example, like a living labs has a sort of like fairly well defined like tone of voice. And so it was a custom GPT, you could run anything through it and it would just sound on brand. And so then we started to extend that, you know, we had a big spreadsheet, like a launch checklist.

**James McAulay** (00:57:08)

And every launch, you would like duplicate this sheet, you would like adjust it, whether it was like a tier one product launch, tier two product launch. And then you just work through the sheet. And we started to build out like custom GPTs that would like take on parts of that process. I am 100% sure now, you know, I left 11 Labs last year, but I'm 100% sure there is like a launch skill now. So I think it's come on a long way. I would also bet that the majority of people in the growth team at 11 Labs will be working in the way that I just showed, like inside Cloud Code plugged into all the tools. 12 months ago, even the developers were just discovering Cloud Code. I don't think growth people and product people were inside Cloud Code this time last year. So yeah, as a growth industry, as a product industry, I think we've We've been given these superpowers in the last 12 months that, you know, really do unlock so many abilities for like non-technical people.

**Aakash Gupta** (00:58:05)

It's actually wild. What do you see as like the next frontier? You mentioned instinct. Is that part of it? What's like What's coming up in the next couple months that everybody in growth is going to be adopting?

**James McAulay** (00:58:18)

Well, I think I've heard people talk about this idea of the autonomous company, like the company of agents that kind of grows itself. And I've seen like a few people on X kind of claim to have built something like this. And I have had attempts at building growth. Something like this, you know, where I want to kind of like close my laptop at 6pm and just have agents, as we talked about earlier, like autonomously pick the right task, work on it, check their own work. And then in the morning, I sort of wake up, review it. Maybe I don't even review it. So... Yeah, to me, I think it's like this notion of like a self-improving 24-7 company of agents. And right now, you know, my system works really well, but it still kind of waits for my prompt. I've got some scheduled tasks like you have.

**James McAulay** (00:59:16)

But I would love to reach a point where an agent came back to me and said, like, I've wrapped up this experiment. It was a success. I've kicked off the next one. You didn't do anything. And I think just this idea of like an agent running 24-7 is just not quite ironed out yet. Like Vercel have built a great framework called Eve, highly recommend trying that out. People bought Mac Minis and just sort of like set up OpenClaw on them. Instinct is kind of the latest personal agent and like Meta's Muse assistant this week as well. Just this idea that like there's an agent not bound to your computer, like running in the cloud somewhere, kind of getting stuff done for you. Maybe even preempting what you want or need. Whoever figures that out for companies, I think is going to make a lot of money.

**James McAulay** (01:00:05)

And then I think growth people will be tasked with pointing these agents at the right experiments. You've got to understand your customers to run good experiments. There's no point in running A-B tests on a page that no one cares about. So yeah, that would be my sort of prediction. I want to talk about you for a second.

**Aakash Gupta** (01:00:23)

How the hell did you scale up this business to 100K revenue in just four months?

**James McAulay** (01:00:27)

Okay, so I was doing consulting. I was doing growth consulting and I got asked to do like a workshop teaching execs on AI. And actually like 12 years ago, I was teaching execs coding through coding bootcamps. So I did this one day workshop and I got really good feedback and people were like, oh, you're a good presenter. I feel like I transformed technology. How I use Claude in two days. And so I thought, okay, maybe I'm onto something. And I'd been like plugging all my MCPs into Claude. I had this pretty good system that was using like Apollo, Granola, Todoist. And I ran a workshop online and I said, hey, I'm going to show you like how I'm running this business. It's still consulting. Like at this point, I'm still just doing growth consulting. And I got something like 150 people attend that just mostly from my own network.

**James McAulay** (01:01:18)

And so again, I thought, okay, there's appetite. Like I've got product market fit here. People want to know how to actually use AI to grow faster. And so I was doing consulting like four or five days a week and I thought, okay, I'm going to pull that back to three days a week and I'm going to give myself two days a week to run some sort of cohort. Like, can I teach, you know, like a bunch of companies, maybe like 20 people. Can I teach them over four weeks how to like get all this stuff set up? And I got 60 people signed up. And so that was like the busiest month of my life was like three days a week of consulting and then sort of. And yeah, I think like, you know, I put my heart and soul into it. I really made sure that everyone got good results.

**James McAulay** (01:01:59)

And the word of mouth has just been kind of crazy. I incentivized them with a referral program. I said, you know, if you've enjoyed this and you know someone that you want to kind of like get trained, here's your link. And, you know, it gets them a discount. It gets you some money. Again, Claude Code set it up for me. I used something called Rewardful with an API that was like very easy to use. And then I got people referring, you know, like companies that wanted to train 20 people at once. And with my pricing model, like, you know, 20 people at once is pretty good. So... I've basically been sort of like building my own learning platform, running cohorts like this every couple months and doing like private workshops as well. So I've like just got back from Vegas, went to Greece in the summer to do these like intensive either hackathons or sort of like exec training sessions.

**James McAulay** (01:02:48)

And yeah, I think I've found a format that people want. And I've used Claude fully as much as I can. I've maxed out that Claude $200 a month subscription. And I just feel like I've applied everything that I learned Like running a company, being out of living labs, doing growth consulting. So yeah, I think just good timing and sort of like the right stage of my life to apply all the lessons I've learned.

**Aakash Gupta** (01:03:14)

You've basically like taken everything you've done in the past and you've put it into like a business built around that skill set, which is genius. So you've taught over 400 people now. What do most people get wrong as they're learning this stuff?

**James McAulay** (01:03:27)

I think people don't realize that you can ask an agent to improve itself. Like so much of what I do, and actually I've seen, maybe, yeah, one of the things I learned was like, I was at this company, Jack and Jill, and they're an agent company. I don't know if you've heard of them. Jack kind of speaks to candidates and Jill speaks to recruiters. And together they try to like match people. And it's like a AI native, you know, like agentic first company. And I would hear these like, I'd hear conversations in the office where someone would say like, I asked Jack, How he would improve his own system prompt. And he came back with this 10-step list and I did it and now he's better. I was like, what? I'm not talking about recursive self-improvement in this sort of AGI sense. More just that you can point An LLM at its own system prompt or at its own skill and run evals or just say, like, how can we improve this?

**James McAulay** (01:04:24)

And I think that's a skill that, like, a lot of people haven't even realized is possible. You know, quite often someone comes to me with a question. They're like, how can I improve my Cloud.md? Now, I can give them... My take on it, I can say, okay, here's some best practices. But what I usually say to them is like, well, have you asked Claude? Like, have you said to Claude, based on all of our recent interactions, everything you know about me, and by the way, go and read the Anthropic docs, how could we improve my Claude.nd? So yeah, I think people just haven't yet sort of figured out that these agents can improve themselves. I think as well that the reason for that Is Claude Chat isn't very good at like editing itself, right? Like it's in the cloud. It can't really like set up second brain.

**James McAulay** (01:05:15)

It can't edit its own system instructions. But once you get into Claude code and code work, you know, they are able to like reflect on their own work and basically edit any file on your computer. And I think when people make that jump from like cloud based chat to kind of like file based agent, they start to realize, oh, like Claude can fix anything about itself. So yeah, maybe that's like the biggest breakthrough for a lot of people.

**Aakash Gupta** (01:05:40)

So I've got your LinkedIn here. People got the GitHub link below. You're on YouTube. You have a website. You obviously have the Agent Accelerator. Is there anything else people should know if they want to work with James or learn more from you?

**James McAulay** (01:05:53)

I think you've covered it. I mean... I post daily tips on LinkedIn. I am posting a good video every week on YouTube. If you want to book a call with me, there's a link on the Agent Accelerator website to find out if we would be a good fit. But yeah, I think you are more prepared than I was there with all the links. So I think that covers it.

<!-- sponsor -->
**Aakash Gupta** (01:06:15)

All right, guys, we'll put those in the description or the email where you found this and see you in the next episode. I hope you learned as much from today's episode as I did. If you can do one thing that's totally free that would help the show, it would be to check that you're following on Apple and Spotify podcasts. Check that you've left ratings and reviews on those platforms. Check that you're subscribed on YouTube. Leave a like and a comment on this video, and then share it with your friends. We're trying to make better and better podcasts. After two years, we think we've gotten something pretty good going. So let us know what we can do to make it even better, who else we should interview, and we We'll put on the best shows we possibly can. Finally, don't forget my offer for the bundle. You get an entire year of my paid newsletter, plus my favorite AI tools, Boltut New, Airtable, Speechify, Descript, Magic Patterns, Linear, Dovetail, Arise, and Mobbin.

<!-- sponsor -->
**Aakash Gupta** (01:07:09)

That's $27,000 worth of value for just $150. So check that out at bundle.akashgu.com if it interests you, and I can't wait to share our next episodes.
