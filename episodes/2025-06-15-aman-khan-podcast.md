---
title: "AI PM Crash Course 2026: Prototyping → Observability → Evals"
subtitle: "These are all the skills you need to become an AI PM like Aman Khan — who has been an AI PM at Arize (Evals Leader), Spotify, and Cruise (Autonomous Driving)."
date: "2025-06-15"
host: "Aakash Gupta"
guests: ["Aman Khan", "Guest"]
speaker_names: "substack"
substack_url: "https://www.news.aakashg.com/p/aman-khan-podcast"
youtube_url: "https://www.youtube.com/watch?v=Ej4pBDaHspk"
duration: "02:04:36"
word_count: 22052
source: "Substack episode transcript (aired audio)"
sponsors:
  - name: "Miro"
    url: "https://miro.com"
  - name: "Jira Product Discovery"
    url: "https://www.atlassian.com/software/jira/product-discovery"
  - name: "Amplitude"
    url: "https://bit.ly/4hl25RG"
---

**Sponsors:** This episode is brought to you by [Miro](https://miro.com), [Jira Product Discovery](https://www.atlassian.com/software/jira/product-discovery) and [Amplitude](https://bit.ly/4hl25RG).

# AI PM Crash Course 2026: Prototyping → Observability → Evals

*These are all the skills you need to become an AI PM like Aman Khan — who has been an AI PM at Arize (Evals Leader), Spotify, and Cruise (Autonomous Driving).*

**Aman Khan** (00:00:00)

Companies are laying off entire teams, entire orgs, and PMs are sort of grouped up into that. I almost never see it where an AI PM team is going to be laid off to some degree.

**Aakash Gupta** (00:00:10)

Can anyone become an AI PM?

**Aman Khan** (00:00:11)

I think we're all kind of feeling it, right? Like as product managers, the expectations on us, we kind of know our role is changing.

**Aakash Gupta** (00:00:19)

what is the right way to teach this material? What is the right sectioning of this material? And we've come up with five steps for you guys. So we're gonna go through AI prototyping, which is kind of the heart and soul of it all. We'll go into observability on top of our prototype, evals on our prototype, the difference between rag, fine tuning, and prompt engineering. And then we'll end with working with AI engineers, working with researchers.

**Aman Khan** (00:00:41)

So let's hop into AI prototyping.

**Aakash Gupta** (00:00:44)

So for AIPMs, you'd really recommend they learn cursor over the other tools?

**Aman Khan** (00:00:49)

I would recommend getting familiar with it, definitely.

**Aakash Gupta** (00:00:51)

Yeah. When it comes to people creating AIPM content, Aman Khan is amongst the most insightful and informed. And that's because he's been an AIPM since 2019. He worked at Cruise on self-driving cars. He's worked with Spotify on their AI systems. And now he works at Arise, one of the leading observability and evals companies. So if we go back then and we compare those three terms that fine-tuning, prompt engineering, RAG, how do those all compare?

**Aman Khan** (00:01:17)

I think it's helpful to have just like a really quick diagram here of like what is each thing. It kind of depends on what your goal is. So if your goal is to adjust the tone or the instructions, I think prompt engineering is really helpful for that. With RAG, you can provide context over a lot of data. Fine-tuning is, think of this as adjusting the model layer a little bit. So it's actually taking the LLM and making it more specialized.

**Aakash Gupta** (00:01:41)

Working with AI engineers and researchers, working on these longer development timelines, how can AI PMs master that? Yeah, so I think this is where... Really quickly, I think a crazy stat is that more than 50% of you listening are not subscribed. If you can subscribe on YouTube, follow on Apple or Spotify podcasts, my commitment to you is that we'll continue to make this content better and better. And now on to today's episode. Welcome to the podcast, Aman.

**Aman Khan** (00:02:13)

Thanks so much for having me, Akash. It's great to be here. I've been waiting for this one for a long time. I'm so excited to speak to you. So...

**Aakash Gupta** (00:02:20)

Yeah, I think that there's no better person to really give us a crash course in all of the key AIPM skills as they stand here in June 2025. But before we even get there, I need to know, can anyone become an AIPM?

**Aman Khan** (00:02:36)

Yeah, I mean, I think the whole narrative here of like, you know, I think we're all kind of feeling it, right? Like as product managers, the expectations on us, we kind of know our role is changing. Our stakeholders are expecting more from us. Our customers are expecting more from us. And I think we're already feeling that role of AI in our day-to-day life more and more. I mean, that's the reason why that narrative is really sticking. It's that, you know, can any PM become an AI PM? And I really think to just define what an AI PM is, it's really some flavor of either adopting AI in your day-to-day workflow, think of this as like an AI-powered PM, or building AI into your product, which is, you can think of that as like an AI product PM. And I really don't think that, you know, being an AI PM is not an either or.

**Aman Khan** (00:03:30)

I really view it more as an X, meaning like you can think of yourself as a FinTech X AI PM or a healthcare X AI PM. And the reason I say that is because AI is really powering your workflows as a product manager rather than taking the job you have away. You really want to be able to take that core insight and knowledge and specific industry sort of knowledge that you have and apply that towards the field using AI, you know, sort of to power those workflows. So that's really how I view it. I think every PM will become some flavor of AI PM either using those tools or building around them if you aren't already. And I wouldn't view it as mutually exclusive with the type of product management you might already be doing. So that's kind of how I view it. Think of it as like more of an accelerator on top of the workflows you already have.

**Aakash Gupta** (00:04:22)

agreed and i think that people often come up with the edge cases like hey i'm an internal tools pm or i work in this really regulated industry but in the last few weeks and months i've been talking to exactly those types of pms implementing ai i talked to an experimentation pm who is dealing with the problem that everybody else has a slight variation on their prd template by getting an LLM to convert that into a clear output of what the hypothesis is, what the North Star metric is, what the world real metrics is. So genius use case to standardize input into his experimentation system. I've been talking to people over in the financial industries. They're working on new credit models based on AI. So it seems like whatever exception you draw up, there's going to be a counterpoint to that exception. And just about every PM needs to learn how to build AI features.

**Aman Khan** (00:05:07)

I think that's, that's totally true. Like, and I think there's definitely a feeling where there's maybe some, some amount of like hesitation or, you know, unsure of like wanting to brand or label yourself as like, oh, I'm an AIP. I'm like kind of worried you might be jumping on some sort of like hype train, but I really urge folks to think about what the market for product management looks like and what what the roles and skill sets will require in the future. And that's really why I think that, you know, the sooner that you kind of think of yourself as an AI PM building in fintech, building in healthcare, the faster you'll kind of adopt those tools, the faster you'll become a leader in your own space and using AI as well.

**Aakash Gupta** (00:05:52)

So enough talking, let's get into the five skills. You and I have been going back and forth on what is the right way to teach this material? What is the right sectioning of this material? And we've come up with five steps for you guys. So we're gonna go through AI prototyping, which is kind of the heart and soul of it all. We'll go into observability on top of our prototype, evals on our prototype. the difference between rag, fine tuning, and prompt engineering. And then we'll end with working with AI engineers, working with researchers. All right, so now we're going to get into these skills, starting with AI prototyping. So maybe even consider opening up your browser alongside Aman as we walk you through these key skills.

**Aman Khan** (00:06:31)

Okay, so let's hop into AI prototyping. So what we've got here, if you haven't seen this tool before, this is Cursor. Cursor is basically a fork of VS Code, which is a really common tool used by developers for actually, you know, has been used for many years to kind of write and iterate on code in an IDE, which is an interactive developer environment. We're gonna hop into using Cursor as our prototyping tool, just because the amount of improvements that have been made to it in sort of the recent weeks and months have made it really my go-to tool for prototyping, even relative to some of the others right now. And just to maybe linger on that point for a moment, there's a lot of tools out there like Lovable, Bolt, Replit, Vercel, V0. And I think they all have their place when it comes to prototyping.

**Aman Khan** (00:07:24)

For instance, Vercel is really strong at front end. Lovable and Bolt is really easy to deploy and get started with. Replit is really powerful for Python-based applications and having an agent built in. But the reason I really like Cursor is just because of the amount of control and flexibility it gives me to be able to iterate on specific components. I completely admit, there's a little bit of a learning curve to get started with using Cursor, But I promise you, if you spend a little bit of time on being able to just be able to kind of feel comfortable with the interface, you're going to get a lot more out of the tool just because of the sort of the features and components it has built into it from a usability perspective.

**Aakash Gupta** (00:08:09)

So for AI PMs, you'd really recommend they learn cursor over the other tools?

**Aman Khan** (00:08:14)

I would recommend getting familiar with it, definitely. Yeah, I think that the other tools are going to keep improving and they're really helpful for building a really quick and dirty mock, you know, to build like just a quick UI. But if you really want to get a little bit deeper than that and understand how do I implement, let's say, an agent next, or can I have more control over the system, you're going to need a tool like Cursor, definitely.

**Aakash Gupta** (00:08:41)

Okay, cool. Yeah, maybe we can prototype like a agentic system since that's what's hot.

**Aman Khan** (00:08:47)

Yeah, absolutely. I think that's a great idea. So let me go ahead and actually start here from scratch. So when you first load up cursor, you're going to get the screen where you can either set up a repo or set up a directory. It doesn't really matter what you get started with here. I have a starting point of a workspace, but the two commands that you want to kind of hit right off the bat On your laptop are command T, which pulls up your terminal. And don't worry, you can actually just type in natural language instructions here to get started with terminal commands as well. So that's actually running the code on your computer. And then command K, which is really how you spin up the agent, which you're going to be using for... Oh, it looks like that commands. Oh, sorry, not command K. What you're going to want to do is actually hit command L to pull up the agent.

**Aman Khan** (00:09:41)

And the agent is this new kind of somewhat new feature in cursor that allows you to go ahead and actually it will write the code for you and actually run the code for you too. What I've been using recently is Claude4 Sonnet. Claude4 is just, I think, a massive improvement on top of previous models here when it comes to understanding commands and writing code. So really, I just go ahead and start typing in what I want this agent to do, and it's able to kind of get started from there. Let's take an example. So when we were talking about agent based systems, I kind of pulled this up. This is in our repo in Arise. It's a fully open source repo. It's a workflow for actually using crew AI, which is a very kind of popular framework these days for setting up agent-based systems. You can either use Crew AI, there's a ton of others out there.

**Aman Khan** (00:10:39)

It doesn't really matter. But all I wanted to do is pull up some example contexts that I can use and plug in so that I kind of know what the output looks like. So this is a notebook that just creates a crew AI agent, really just starts spinning up a workflow for research and deciding, you know, being able to do some market research. It doesn't matter, but it's more so just for grounding the agent in the first place. And what I'm gonna do is actually rebuild and re-architect the system entirely on the fly, just using this code example. So the instructions I'm gonna give are build me a trip planner agents using instead of crew AI, use lane graph, which is just another framework, really just to show like, it doesn't matter which agent framework you use, you can be really flexible here. The trip planner should have a front end I can use as an application.

**Aman Khan** (00:11:41)

So what I'm doing here is basically defining I want this agent to have a UI that I can actually click and interact with further. So we've got kind of two components in here, which is build me a trip planner agent. Here's the framework to use. And then if you need to, what you used to be able to do in the sort of before was actually use at web. and um and at web allows the agent to go and sort of search the internet as well and take action actually search look at documents and take that information and apply it in the code so let's go ahead and hit enter here and see the agent sort of go off on its own and see what it generates

**Aakash Gupta** (00:12:22)

And it's not a very complex prompt, really.

**Aman Khan** (00:12:24)

No, and that's sort of the beauty of it. I know that there's a ton of upfront work you can do to make that initial shot sort of what we kind of call in prompting is like the first shot or zero shot better. But just know that the workflow I really promote in terms of people getting comfortable with these tools is just being able to iterate. And so knowing how to ask the right questions from the agent to give it what you want. So let's take a look here. So it says, I'll help you build a trip planner agent using lane graph instead of crew AI with a front end application. And so it'll actually go in and read the tutorial and understand what the components are. Great. And says, okay, I'm going to go ahead and take a look at this implementation and create the lane graph trip planner.

**Aman Khan** (00:13:16)

So it's going to go ahead and create a new directory for me. So it didn't even matter what my starting point was because the agent can actually create folders on your machine. It can create directories. It can pull in the right data and even import packages. So it's actually going off and doing this live. It's creating the requirements for the agent in the first place.

<!-- sponsor -->
**Aakash Gupta** (00:13:35)

Today's episode is brought to you by Miro. Let me ask you something. How many tools are you juggling just to get a single project across the finish line? One for brainstorming, another for planning, something else for tracking tickets. That's where Miro comes in. It becomes an all-in-one collaboration workspace. Whether you're consolidating user research from several interviews, developing and synthesizing product briefs or a wireframe, or project managing development. Miro brings everyone into the same space. It's fast, intuitive, and fully loaded with features like project templates, two-way Jira Sync, and integration with software like Draw.io and PlantUML. Miro's AI features can be used to synthesize elements in a board to develop a ready-to-review product requirements document in seconds. If you're tired of tab overload and scattered workflows, try Miro. We'll be right back. That's A-T-L-A-S-S-I-A-N dot com slash product dash discovery. Jira Product Discovery. Build the right thing.

<!-- sponsor -->
**Aakash Gupta** (00:15:27)

That chain of thought reasoning is really useful too. It seems like that's one of the important steps for people is to actually understand a little bit of what's going on and not just ignore that, but start learning. And as you do that 10, 20 times, then you really get used to it.

**Aman Khan** (00:15:40)

Absolutely. And being able to, you know, what's really cool about this is you can actually go in and see what are the files that it referenced, be able to see, okay, here's what it's referencing. So if you need to, you can always pause it, pause the agent and say, hey, I actually want you to go take a look at this part of the code or this resource. what's really cool and we can kind of will kind of show this as you can even paste in images and using those images the agent can actually you know kind of infer oh this is what I want the UI to look like or not so it's a really really powerful multimodal based agent that can write code so now it's actually writing the code of the file itself

**Aakash Gupta** (00:16:23)

and here is What is going on behind the scenes? It's using those websites and the Phoenix thing that we started off with, or it's writing a lot of scratch code. What's going on?

**Aman Khan** (00:16:34)

Yeah. So, so actually, you know, the repo I kind of gave was just a starting point and it can really just be any directory. What's going on underneath the hood is the agent has kicked off a search. Well, first it took the prompt and the context I gave the agent and it said, let me build a plan. And that's actually the first step in all of this is actually to generate a plan, which it doesn't show here, but there is basically a chain of thought for the plan here. So if you hit this thought for four seconds, you'll see what the agent is thinking it should do. and it says i should first look at the crew ai tutorial design a lane graph based trip planner then build a front-end application and then integrate it all together and so that's just like you would give this to an engineer if you were hopefully you're giving better requirements an engineer but you don't have to give really good requirements to your agent because the agent will just like make sense of whatever you've given it and try its best to figure it out so it's very robust to that So once you've got that plan, then the agent executes code on your machine to actually implement that plan.

**Aman Khan** (00:17:45)

The first thing it did was create a directory that it's writing code into. So it's actually created a new folder in my workspace where it's actually writing code on my machine. And the code is really just text files. In this case, it's Python. You can define different frameworks if you want to. I could have said use Python or use React, but in this case, I've just let the agent go off and do its thing. I wasn't super prescriptive. So great. So it actually built the back end here, which you can see. And now it's going to build the React front end. So it's going and actually building the UI components. And just to zoom out for a moment, to be able to do this even a year ago would have been really, really challenging. Because you're just not going to get robust UI components and sort of an agent that understands what goes into building a React application with a degree of confidence and understanding when there's errors, how to fix those errors.

**Aman Khan** (00:18:47)

So let me show you an example here. The agent actually built a file and What it found was that there was an error in the file and on the fly, it went back and it's rewriting parts of the file because the agent can actually see and read errors as they come up and is able to go back and iterate on those same files all within the chat window as well.

**Guest** (00:19:11)

Okay.

**Aman Khan** (00:19:12)

In this case, there's times when you as a human might need to intervene. particularly when there's files being deleted. So it might prompt you to either accept to do something or not. I generally just let, you know, I'll take a look at what the agent is asking me to review, and then I'll either accept or reject based on that. And it can actually tweak its path based on whether or not you accept or reject the suggestion. Okay, great. So now it's going ahead and creating a directory and installing all of the components for the UI right now.

**Aakash Gupta** (00:19:47)

So it seems like from zero to one, it might be a teeny bit slower than a lovable Bolt or V0, but after zero to one, the power to edit more, implement more cursors, allowing more potential.

**Aman Khan** (00:20:01)

Absolutely. I think that one way to think of it is like the application that we've given it is, and I'm using a pretty capable model as well. I'm using Cloud4. which is a reasoning model, so it's a little bit slower than some of the faster models out there. But the reason that you, you know, one reason to actually start here is you just have complete control over the files. You can go in and if you wanted to, one thing I do is actually I'll take a look at the file and I'll ask the agent, you can reference a specific file here in the context window, and you can actually say what is going on in this file and you can just have a conversation with the code uh you know with the agent on top of your code so even if you you know want to know do i really need this file um can you make this better i noticed this one thing my engineer pointed something out you're just going to have a lot more control over that system using cursor so it's it's worthwhile to invest a little bit more time to get this thing set up on your machine

**Aakash Gupta** (00:20:59)

okay And is it possible to do those types of things in parallel, or while it's working, while it's generating, you can't chat until this generation is done?

**Aman Khan** (00:21:06)

Yeah, I think, you know, we could try, actually. So I've started a new chat. Let's see. Okay. Yeah, so with cursor, you actually, yeah, you can't have multiple... I don't believe you can

**Aakash Gupta** (00:21:29)

have

**Aman Khan** (00:21:29)

multiple chat windows going at the same time. I think you can only do one chat, but maybe someone can prove me wrong there.

**Aakash Gupta** (00:21:39)

So now that it's done, you could chat with it, though.

**Aman Khan** (00:21:41)

Yeah, let's see. So this one, I think we may have broken it, actually. Continue building. Which is part of exploration. Did it actually finish or not? Let's see. Okay, so what's funny is the system is super robust. We just broke it because I went to another tab and I came back and I'm like, hey, you know what? I'm sorry for interrupting your work. Just keep doing what you were doing. And

**Aakash Gupta** (00:22:10)

it's just

**Aman Khan** (00:22:10)

like, oh, okay, here's what I was doing before. Let me just recap it for myself. I'm just gonna keep going on my way. It's sort of like tapping an engineer on the shoulder. I'm not worried about breaking my code anymore or like changing one line because I know and I have so much confidence that the system is going to be able to recover from some of those mistakes when it comes from starting from scratch for sure. I will say if you try to go to your like production code base and you're like hey can we start using cursor all over the place like this you're gonna get a lot of pushback because I will say like with these types of agents, they're really good for going from zero to one and maybe even building something that gets you to production. But when you already have a system that's using multiple dependencies, it gets a little bit harder to know.

**Aman Khan** (00:22:59)

You really do want to make sure the changes that you're making are correct in the first place. So I do recommend that, at least when you're just getting started, use this on zero to one projects that you own entirely and not so much necessarily your production code base that you might be building on top of.

**Aakash Gupta** (00:23:16)

Yeah, I was worried that it was going to break when we were clicking around, but it just started right back up.

**Aman Khan** (00:23:22)

Yeah, I think that's part of where, look, I mean, I think I'll just say like from the perspective of a product manager today, being comfortable with the fact that this thing is writing code, it's just going to go off and start doing things. You should really just feel comfortable knowing how to interact with it. And that's, I think part of that is just, it's just a comfort level that comes with working with these tools.

**Aakash Gupta** (00:23:46)

For sure. Looks like, can I edit some files, but it'll just go out and continue on its own. And this readme, can we read that, me readme, and see what's going on behind that?

**Aman Khan** (00:23:54)

Yeah, absolutely. So it's actually, when it's writing a file, so you used to be able to just see it, like, writing code in real time. I think with the agent mode, you have to wait until the file is written. But let's give it a sec to write that file, and we can read what the readme is.

**Aakash Gupta** (00:24:12)

Because I think it's often like a PRD style doc.

**Aman Khan** (00:24:14)

Exactly. And you could, you know, I think that there's some really great examples. If we were being more sophisticated, I could have given it a better prompt as well. But you're right. It's basically, here's what's going on underneath the system.

**Aakash Gupta** (00:24:28)

And it

**Aman Khan** (00:24:28)

says, this is what I did. Here are the features that it has. architecture, back-end, front-end.

**Aakash Gupta** (00:24:37)

Written with full emojis.

**Aman Khan** (00:24:40)

Yeah, I don't know why LLMs really like to use emojis these days.

**Aakash Gupta** (00:24:46)

That's how you know somebody's LinkedIn post had some ChatGPT editing. Oh

**Aman Khan** (00:24:49)

my gosh. I mean, for sure, yeah, ChatGPT, Claude, we're definitely trained on LinkedIn as well. So it kind of goes both ways, right? It's like self-reinforcing with these models.

**Aakash Gupta** (00:25:00)

Yeah.

**Aman Khan** (00:25:02)

Okay. So it's actually, so try to run the code. It hit an example, it hit a problem here. And now it's actually creating the Docker file. We don't necessarily need Docker, but it's helpful if you want it to actually deploy this thing. Docker

**Guest** (00:25:14)

is

**Aman Khan** (00:25:14)

a way for you to just wrap everything up and think of it as like a folder that you can deploy and put on the internet.

**Guest** (00:25:20)

Yep.

**Aman Khan** (00:25:22)

Okay, so it's writing all of this. And what we can actually do is it's given me enough information here where I can actually try to run this live. So I don't need to have it finished a Docker file. And it's sort of just running tests. So it actually knows to actually test the agent itself, make

**Aakash Gupta** (00:25:39)

sure that

**Aman Khan** (00:25:39)

the backend is working. And as long as it's working, then it'll actually move on to the next step. Um, let's go ahead and so it's got local hosts. We've got it here. I have a feeling that this might break, uh, but we will try it because it didn't ask me for an open AI key. So let's see what happens. Okay. Let's first actually go to here. We'll go to the back end. And so all I've done now is I'm looking at the readme and it actually lays out the quick start steps for how to spin up the system. So all you have to do is copy paste these lines of code. So I can go to lane graph. And a little bit of like the terminal commands is helpful to know like cd dot dot to navigate your directory structure. But we're going to go ahead and

**Aakash Gupta** (00:26:31)

and dot dot like moves you up a level right

**Aman Khan** (00:26:33)

exactly dot dot moves you up a level

**Aakash Gupta** (00:26:36)

and then ls lists the files in there

**Aman Khan** (00:26:39)

yeah um so we're gonna try to go to cd agent

**Aakash Gupta** (00:26:46)

cd is just change directory

**Aman Khan** (00:26:48)

change directory exactly pip uh is your python so um let's make sure we're in we're gonna create a new python So let's call this.

**Aakash Gupta** (00:27:15)

So we created a workspace, we set up a project, we have an environment.

**Aman Khan** (00:27:20)

Yeah, so one thing you definitely want to be careful of when you're running Python on your machine, every developer will have faced this at some point, it's sort of a rite of passage, is you don't want to be writing, you know, updating packages and installing packages to your Python locally. You want to be using virtual environments because your system Python is sort of, you want to kind of keep that protected because that can really break things. So what we've done is just created a virtual environment using a tool called Conda. And if you get stuck on that or you're like, what is going on here? Don't worry, the agent will actually, you can also specify, use a virtual environment or, you know, how should I do this on my machine? And it will help you out. It'll guide you through those steps as well.

**Aakash Gupta** (00:28:07)

Okay. Yeah.

**Aman Khan** (00:28:10)

Okay, so now we've kind of done that. Now we're going to install our requirements. So we just, we're in the right directory, and now we're just gonna hit pip install requirements. And if this works, it will actually install those requirements into my Python virtual environment.

**Aakash Gupta** (00:28:24)

Okay.

**Aman Khan** (00:28:28)

Great. Setup environment variables. Okay, so let me go here and open up that file. So we actually want to name this dot env. So actually, let's see what environment variables it needs. I'm not even sure. So we're just going to run the Python main and see what pops up. So we'll go back and do the env variables after. Exactly, yeah. Because I'm kind of curious. I could go in and read it. Okay, module not found. So it looks like it hit a problem here. This is great because what that means is I can go in and just copy that error and say, hey, you hit this error. Let's see how it fixes that. Hit skip, stop. And all I mostly do is my workflow is copy the terminal, paste it in and say, literally just give it back to it and say, hey, there's this bug here.

**Aman Khan** (00:29:23)

And it will read the terminal lines and understand what's going on and try and infer that. Nice. So this is what I mean where I say, don't be scared about things breaking. They're going to break. What matters is how you can work with the agent to fix your problems.

<!-- sponsor -->
**Aakash Gupta** (00:29:45)

Yep. Today's episode is brought to you by Maven. If you're enjoying this episode with Aman, you'll love his course on Maven, today's podcast sponsor. The problem with most courses online like Udemy is there's no live component and the instructors aren't experts in their fields, they're professors. At Maven, you get direct live access to experts and operators from the world's best tech companies. You can't get that access anywhere else, in any university, and you usually can't find them on YouTube either. I featured so many of Maven's experts in the newsletter and podcast for that reason. To help you out, I've put together a collection of courses I recommend at maven.com slash x slash Akash. This includes courses like AI prototyping for PMs, product sense for PMs, and getting an AI PM certification. Visit it now at maven.com slash x slash A-A-K-A-S-H. Today's episode is brought to you by Amplitude.

<!-- sponsor -->
**Aakash Gupta** (00:30:42)

Replays of mobile user engagement are critical to building better products and experiences, but many session replay tools don't capture the full picture. Some tools take screenshots every second, leading to choppy replays and high storage costs from enormous capture sizes. Others use wireframes, but key moments go missing, creating gaps in your understandings. And also setting aside enough time to just persevere. Definitely, yeah.

**Aman Khan** (00:31:31)

Okay, now it's gonna actually try to run these commands. Let's see if that works. Okay, so I have to enter in OpenAI key. That's what I was kind of expecting. So it actually built this .env file, and great. Let me go ahead and insert an OpenAI key. Hopefully this works. I'm gonna go ahead and move this to a different window so I don't blast this on the internet. Okay, yeah, don't share your OpenAI keys or your keys, you know, widely. That's definitely something to keep in mind.

**Aakash Gupta** (00:32:15)

That'll be expensive fast.

**Aman Khan** (00:32:16)

Yeah. Okay, press enter. Okay, port is already in use. Let me go ahead.

<!-- sponsor -->
**Aakash Gupta** (00:32:27)

Today's episode is brought to you by Amplitude. Replays of mobile user engagement are critical to building better products and experiences. But many session replay tools don't capture the full picture. Some tools take screenshots every second, leading to choppy replays and high storage costs from enormous capture sites. Others use wireframes, but key moments go missing, creating gaps in your understanding. Neither approach gives you a truly mobile experience. Amplitude does things differently. Their mobile replays capture the full experience. Every tap, every scroll, and every gesture. With no lag and no performance hit. It's the most accurate way to understand mobile behavior. See the full story with Amplitude. And also setting aside enough time to just persevere.

**Aman Khan** (00:33:10)

Definitely, yeah. Okay, now it's gonna actually try to run these commands. Let's see if that works. Okay, so I have to enter in OpenAI key. That's what I was kind of expecting. So it actually built this .env file. And great, let me go ahead and insert an OpenAI key. Hopefully this works. I'm gonna go ahead and move this to a different window so I don't blast this on the internet. Okay, yeah, don't share your OpenAI keys or your keys, you know, widely. That's definitely something to keep in mind.

**Aakash Gupta** (00:34:02)

That'll be expensive fast.

**Aman Khan** (00:34:04)

Yeah. Okay, press enter. Okay, port is already in use. Let me go ahead. Not a big deal. I had something working in the background and it's going to kill that process. I added my OpenAI key. Great, and now it says it's built. Let's go ahead and navigate to that and see where it's running. I feel like I didn't see the UI. It looks like it ran the backend. Okay, and now it says in a new terminal do this. So let's go ahead and do that. So we're gonna go ahead and run this. We're gonna try this again, see if it actually fixed the problems before. Oh, it's still hitting this problem.

**Aakash Gupta** (00:35:18)

existing virtual environment with an old incompatible version. Okay.

**Aman Khan** (00:35:25)

That's okay. I mean, we'll just try that again. We're going to uninstall those old versions.

**Aakash Gupta** (00:35:32)

So some of the steps that has you do. Oh, you could have hit run, actually. Yeah, I

**Aman Khan** (00:35:36)

can hit run in the terminal environment on the right or the one on the left. For me, I just wanted to kind of take a look at it here. So I'm going to run it over here.

**Aakash Gupta** (00:35:44)

Okay. Yeah.

**Aman Khan** (00:35:47)

OK, let's try this again. So

**Aakash Gupta** (00:35:52)

we're going to install a fresh virtual environment. And when we see those errors there, what are those? Like ignored the following yanked version.

**Aman Khan** (00:36:07)

Yeah, I think, so some of these are, if some of those versions or those packages existed already, then it kind of looks a little bit scary because it's like all in red or versions are mismatching. Again, I would just say like if you hit a bug or a problem, you can always pass those back off to the agent to go and fix.

**Guest** (00:36:27)

Okay.

**Aman Khan** (00:36:28)

So in this case, it looks like it's trying to use a version that doesn't exist. So that might be part of the problem here is it's actually trying to use a version for a package that doesn't exist.

**Aakash Gupta** (00:36:41)

Okay. Yeah, I think there we go. I noticed the same thing. So it's going to work with the current package. Yeah.

**Aman Khan** (00:36:52)

So here it's saying, okay, you know what? Let me just try to create a more simple version of this agent and see if that works. So let's

**Aakash Gupta** (00:37:00)

see if

**Aman Khan** (00:37:00)

this works in the first place, just to get something off the ground. So even the agent is sort of realizing, you know what? I may have overbuilt this first version. Let me go ahead and build a simple version.

**Aakash Gupta** (00:37:13)

Probably PMs can relate with their PRDs.

**Aman Khan** (00:37:17)

Maybe you overbuilt the first, yeah. Build a simpler MVP, right?

**Aakash Gupta** (00:37:23)

Happened to me, certainly. So I'm just trying to read the code here. OK. It's generating. So

**Aman Khan** (00:37:33)

we can go ahead and read through what's going on here actually a little bit as well.

**Aakash Gupta** (00:37:38)

It feels like being able to read this code is just a key skill.

**Aman Khan** (00:37:42)

You know, the best part is the reason I like to work in Python is it is very readable and the agent does a pretty good job of commenting as well what it's trying to do in the code. So you can see, okay, so it's importing a bunch of packages, loading environment variables. All that means is it's like loading up the state that it needs to get started. And then it starts defining classes and functions to actually execute on the code. So let's

**Aakash Gupta** (00:38:07)

go

**Aman Khan** (00:38:07)

ahead and see what it's done here. So, okay, so we create a simplified version. Let's try this and see if it works. And if it doesn't, then we're back to square one. OK, so it might just need this package. So I'm just going to go ahead and paste in those errors again.

**Aakash Gupta** (00:38:33)

I remember doing all this without an agent. It was like a lot of looking up stack overflow and stuff. At least you have somebody to talk to now. Yeah, exactly.

**Aman Khan** (00:38:41)

Let's try on this window and see if this is working. Okay, so there's a version conflict. It's because I think it actually created two versions of the requirements file, and they were sort of sitting on top of each other. That's okay. Let's try this minimal version.

**Aakash Gupta** (00:39:01)

Yeah, we see requirements minimal, requirements simple, requirements.

**Aman Khan** (00:39:06)

Yeah, exactly. This is really bad practice that it implemented, and you can always go back and be like, hey, fix up the problems that you have in your code base, and it will also be able to go and simplify and remove extraneous files. So I think that's a pretty common occurrence. If you're testing with Python, it's very likely you're going to have package and version dependency problems.

**Aakash Gupta** (00:39:31)

And

**Aman Khan** (00:39:31)

so I think just accepting that that's part of working with Python. Again, you're getting one level deeper than Bolt and Lovable, right? So a little bit of that comfort of there's a little bit more code here, but knowing that you can just kind of, again, mostly what I'm doing is copy pasting the errors and letting the agent figure things out. I could go in and read the code and try to understand things better. And that's worthwhile to do when you're building something to production, but to just get something off of the ground, I kind of let the agent define, you know, here's the right environment for me to work in.

**Aakash Gupta** (00:40:04)

Yup. Let's test if the simplified version works. Okay, server.

**Aman Khan** (00:40:14)

Because it's actually testing if the server has started and seeing what's the problem with the server. Okay. Well, we have a server up now.

**Guest** (00:40:33)

Look at that.

**Aman Khan** (00:40:34)

So it actually figured out, okay, you know what? I might be on the wrong port. Let me see if I should try to run this thing differently. And here we go. So you can actually see this is a Python server that it started. And this is a backend server that actually just routes the calls that we're going to be using for our trip planner agent. So this is a backend that's up. Now, what do you want to change about the backend? The backend is basically a way to route calls to open AI or to other services. So it's actually kind of doing this in real time. Like it just built this backend for us.

**Aakash Gupta** (00:41:07)

Nice. And what is it working on now?

**Aman Khan** (00:41:11)

That's a good question. It looks like it has... Okay, let's try to hit skip here. You know what? Let's see. Okay, so it wanted to test the backend. Okay, so this is interesting. That's actually a really good example you just pointed out, Akash. Sometimes when the agent is trying to run code in the terminal, if it's a longstanding process, it can get stuck. And so you might need to hit move to background or skip just to have it move on to the next step. Okay, so let's try to actually run this. Now run the end-to-end application.

**Aakash Gupta** (00:41:57)

And remind me, what's the difference between this right side and the bottom middle?

**Aman Khan** (00:42:04)

The terminal, you mean, or the...

**Aakash Gupta** (00:42:07)

Okay,

**Aman Khan** (00:42:07)

yeah, so on the right side, this is... Think of this as like the agent environment. It can interact with your terminal, or you can have multiple terminals up. So you'll see it actually. The terminal is... These are... The IDEs consists of different windows that you can reconfigure in different ways that you want to. So I have a terminal running in here. It actually pulled up the terminal in this area. You can have a terminal down here, but it's really just wherever you're executing code on the machine.

**Aakash Gupta** (00:42:35)

Okay, so the right is the chat, and it can go in and do terminal commands, and sometimes you're doing manual terminal commands in the bottom middle. That's right,

**Aman Khan** (00:42:43)

exactly. That's definitely correct. Okay, now it's starting the front end. Let's see what it looks like. Oh, it noticed there's a package dependency. Now it's going to go back, read that file, and let's look at it in real time. It's removing the problematic dependency. But what's great is that the backend is up. The backend server is working here.

**Aakash Gupta** (00:43:10)

Okay. So we can dependencies. Yeah, if anyone's ever tried to teach themselves Python before, they'd probably face this as well. A lot of versioning type issues.

**Aman Khan** (00:43:24)

There's definitely this like upfront work when you go from a rapid prototyping tool like Bolt and Lovable to Cursor. But the amount of control it's going to give you and flexibility and that, you know, it's a worthwhile investment, I think, to be able to read the code and understand what's going on.

**Aakash Gupta** (00:43:47)

So what are these unsupported engine warnings that we're seeing here?

**Aman Khan** (00:43:53)

So let's see what's going on. Looks like it might be hitting a problem with the packages it decided to use. Let's see if it can figure it out. I might hit skip here just to have it keep moving and see what happens. Wow, I feel like we hit, like, every possible thing that can go wrong with the versions of Node in this one. And so it's a really extensive demo. But what it realizes, like, it's using a version of Node that actually has problems with some of the other packages. So it's

**Aakash Gupta** (00:44:29)

going to

**Aman Khan** (00:44:29)

go and reinstall the front-end environment. Cool. Again, you know, it's going to happen. It's just accepting that there's going to be this, you know, sort of a little bit of friction of like, is the agent doing the right thing? And it's just kind of making it move along and figure it out. I feel like we got the agent today on an off day, like it didn't have its morning coffee or something. You know, it's like making a bunch more mistakes, but that's okay.

**Aakash Gupta** (00:45:00)

And Node, for people who don't know, that's like a runtime environment. What does that do for us?

**Aman Khan** (00:45:04)

So this gives you your front end. So this is actually able to accept and take requests, make requests to the backend server, which was your Python code, and serve you a UI or a front end. So it's sort of, think of this as like when you go to any website, like what the UI that you see is.

**Aakash Gupta** (00:45:24)

Okay.

**Aman Khan** (00:45:25)

Okay. So it says both services are running. Let me check the status. So it's going to go ahead and check. It looks like things are happening. Wow. Agent is stoked today. So, all right. So we've got a front end. Let's go ahead and take a look at what that front end looks like. So it even says, here's how to use your trip planer agent. Okay. Now we're going to go back. All right. That was a deep dive. Boom. Oh, wow. So that is the application you just built. We just built it. And all it took was giving a couple of examples, persevering through the Python dependencies that we hit.

**Aakash Gupta** (00:46:04)

And we

**Aman Khan** (00:46:05)

have a real prototype here. You have a UI that can point to the backend and actually serve up requests that we wanna make. So that's a real prototype. Let's go ahead and test it now. What do you think, Akash?

**Aakash Gupta** (00:46:18)

Yeah, let's see it. And let's also just explain, like we were trying to create an agentic system. So where are the agents involved here?

**Aman Khan** (00:46:25)

Yeah, so great question. So we went ahead and it's funny, it actually, it does list them out here in the UI, but you can specify whatever agents you want. Some of these were actually determined in the example that I gave, but let's go ahead and kind of break down like, what are the agents here? So the agents that we've built in, and again, this is fully customizable. So you can give different agents for more specific tasks. The agents here are a research specialist. So that's an agent that's like an expert on doing research on a specific geography, like climate, you know, the attractions, etc. You have a planner agent that can plan day by day. So for a specific day, what should we do for this trip? You have a budget advisor and a local curator. So the budget advisor just takes a budget and actually does analysis on that based on the user's input here, which you're going to put in your budget, and then a local curator to kind of find maybe off the beaten path things.

**Aman Khan** (00:47:28)

But these agents, you can kind of think of them as... LLMs and prompts and contacts that you've packaged and wrapped together to perform a specific task. It's a lot like saying I'm an expert on a specific area and I'm just going to go ahead and focus on giving the best possible output for that specific thing. Like the budget agent is going to be really good at budgeting. The planner agent is going to be really good at making plans. So that's kind of how I would view these different systems a little bit.

**Guest** (00:47:58)

Cool.

**Aman Khan** (00:47:59)

So let's go ahead and give this a shot. So we're gonna say, we're gonna go to Spain. Let's say we're gonna do a quick Europe trip. I know you recently did a summer trip to Europe. Let's go ahead and click Spain. We can say, let's type in we're going for one week. We're going to give a budget of, let's just say like a thousand dollars and maybe some interest we can give our food. And then we can even click the travel style. So let's say we want to go a little bit more adventure. And these are, this form is fully programmatic, right? So if I wanted to, I could go back here and say, you know, change the form color, change the form fields. This is too long. Change how it looks and feels. But you've given something that kind of is, is a good starting point for, for, you know, a prototype you might wanna build for yourself.

**Aman Khan** (00:48:46)

Okay, I'm gonna click plan my trip. And what's going on in the background, and you know, this loading state's not great, and that's probably something I could ask the agent to go and improve on the loading state, but what it's actually gonna do is build an itinerary for me here. And it's gonna take the inputs I have, great, and it says, here's a seven day itinerary for Spain, food and adventure. It's actually given me a day to day sort of hour to hour level analysis of what I could be doing in different cities.

**Aakash Gupta** (00:49:23)

as well as accounting for

**Aman Khan** (00:49:24)

travel.

**Aakash Gupta** (00:49:26)

But it's pretty detailed. It's faster than a real human tip plan would have been for sure. You reading up 10 Google search results, right?

**Aman Khan** (00:49:33)

Right, or even if you pasted, like think of this interface here, right? Like what you've basically done is you've wrapped those prompts of plan me a trip to Spain for one week with a budget of $1,000, interest or food, and in this range. And you've created something that's a lot more programmatic on top of that. You've created a prototype that you could actually go and deploy. And you can build so much more on top of this, right? You can have it referenced, like maybe you want to use a specific API to help you book the flight or suggest flights. You can hook it up to that. You can give it access to search. And so it's a fully programmatic system that you can really go in and tweak on the fly in your cursor environment as well.

**Guest** (00:50:14)

Okay,

**Aman Khan** (00:50:15)

so we've gotten an output here. Now this is really helpful to just get started, but I think we wanna go one level deeper, right? Like as a product manager, just being able to look at this, like I'm not really sure what's going underneath the hood unless I go and read the code. And that's kind of takes us to what observability is. And observability is sort of a key part of being able to understand your AI application. So

**Guest** (00:50:41)

let's go

**Aman Khan** (00:50:41)

ahead and hop to that. So what we did when we actually built the system is we've added what's called tracing. And tracing is a really standard way of looking at the calls that your server is making. That's actually related to the tool that I'm kind of working on, which helps with observability and with sort of tracing applications. And so let's go ahead and look at some specific examples here. So these are some requests that I've made, which are basically to this agent-based system. And this is one we just made, which was Spain, one week. In this case, I clicked sailing and adventure.

**Aakash Gupta** (00:51:25)

This diagram is really cool. What are we seeing here on the bottom left?

**Aman Khan** (00:51:28)

Yeah, so this is actually the same agent that you just built in code represented graphically. So what you actually have is a way for you to visually see what is your agent-based system doing. And remember, you asked a great question, which was like, What agents can we build? And we have a research agent. We have a local experiences agent. We have a budget agent. And all of that goes into an itinerary. And that's what the output is. And so what's really helpful looking at this is when you are thinking about going one step further from your AI prototype to building a prototyped agent or an agent application, being able to visually see what are the paths that the agent is taking to accomplish a goal. You can see what happens here is when I give the input, it kicks off three different agents in parallel to generate an output, and all of those go into the itinerary.

**Aman Khan** (00:52:26)

Remember, I didn't even really define this. i gave this to cursor to go right and i said cursor go ahead and build an agent-based system and this is the architecture it developed and came back to me and uh and that's what what gives you the output that you get on the other end and so what i've gotten is one level deeper on cursor and that's actually a really key point which is It's kind of tough to do this with Bolt and Lovable. You're not gonna get this representation the same way. And so if you wanna see what's going on underneath the hood, you kind of need to use, you have to be a little bit more in the code to be able to define how to get those outputs.

**Aakash Gupta** (00:53:05)

And you could probably use WindSurf too, right?

**Aman Khan** (00:53:07)

That's right, yeah. So as long as you, really what matters is that you can edit the code.

**Aakash Gupta** (00:53:12)

So

**Aman Khan** (00:53:13)

whether that's WindSurf or Cursor, being able to add to the code tracing is really what matters. And I work on this tool, but there's a lot of other tools out there for tracing as well. I think what matters is what's your workflow. So don't take my word for it. Go out and try a tool and implement tracing or ask your, work with your engineer to implement tracing and you'll be able to get a visualization like this at the end of the

**Aakash Gupta** (00:53:40)

day. What was the steps involved with implementing tracing?

**Aman Khan** (00:53:42)

To that, I think it's probably easier to just show what that looks like here. This is our docs for Arise. We actually have a whole section on tracing. Tracing is, think of this as like the units of work that your code is making. And it's actually because this is, you know, we're taking software best practices and applying them to this like AI agent world. It's actually fairly straightforward these days. All you really have to do is install a tracing package and wrap your code in sort of a decorator that is a fancy word for saying take this process or this function and call that a span or a trace so that when you're actually running that code, it picks up that unit and it puts it into what you see here, which is the UI for each of the steps that the agent is taking. So it's really, the short answer Akash is like, it's a line of code that you implement on top of your functions.

**Aakash Gupta** (00:54:49)

So you could probably just point the agent to this doc and it would figure it out.

**Aman Khan** (00:54:53)

Totally. That's actually how I did it as well. Yeah. So that's where the example that I kind of gave it had tracing in it already

**Aakash Gupta** (00:55:00)

as

**Aman Khan** (00:55:01)

a starting point. But what you can do is just literally copy paste this, type it in here, and I could say implement tracing. I won't need to do that now because it already has it, but it will be able to go and infer, okay, here are the steps I need to go and implement the tracing.

**Aakash Gupta** (00:55:18)

Nice. And then you get that awesome thing that we were looking at. Can you break down the top left, what we're reading as well? It looks like there's like multiple levels there. So it's like budget. Then what are we seeing after that?

**Aman Khan** (00:55:27)

Yeah, exactly. So these are the agents that we've defined now, right? So this is a multi-agent system using lane graph. And I've got a budget here, which is you can look at the input. Let's take a look at the input really quick. So this isn't a chat based agent, right? Like I think everyone, a lot of people, it makes sense, right? You want to build something with chat, but what if you just take a form and take these inputs and actually put them into here? That's what this looks like. Spain, one week, the budget, in this case, it's sailing, and then the travel style. And those are inputs to the system. And then those get kicked out to each of these agents. Let's go ahead and take a look at what's going on. And this is really the budget agent, the local experiences agent, research agent.

**Aman Khan** (00:56:17)

That agent has its own sort of tool that it has access to here. And let's go ahead and go one level deeper at the prompt. So this is the system prompt of the agent. The system prompt says, analyze budget requirements for a one-week trip to Spain. And here's the budget. So it actually plumbed in the budget from the form. And it says, this is what you should do. Include a breakdown of all of these things. These are all things that you would think about when you're developing a budget. Like, what would I spend money on when I'm traveling? And so the agent has actually defined for itself in the system prompt, how should I take this thousand dollars and best allocate it for accommodations? And what's interesting is it's, you know, it's actually kind of gone and done a pretty wide search for different tiers of options because it's not really making a decision on what uh you know what is the um the range of the type of trip i want to take it's offloading that to another agent to make that decision all it's doing is saying i have a thousand dollars what can i do with a thousand dollars how should i think about spending that money and let the other agents decide how to best pull that together.

**Aman Khan** (00:57:30)

So then that goes into what's called this like analyzing this budget tool, which takes that destination, the week, and the budget. And that's basically, think of this as like pulling out a structured JSON that goes into the system prompt. So

**Guest** (00:57:48)

these

**Aman Khan** (00:57:48)

tools are basically ways for you to get data from from an unstructured way or from some one format and put it into another format. And it's really important to think about tools or functions as ways for you to get, you know, sort of think of them as like API calls or ways to get data from a system for your agent to use. And that's what this little icon kind of represents here is a tool. And then this is the actual LLM call. And this is the top level agent, which wraps all of that together. And- And you'll notice like this kind of looks complex if this is the first time you are seeing a system like this, right? Like what are all of these lines? There's all these boxes and colors. But I would really stress like this type of system is truly an MVP in today's world of agents.

**Aman Khan** (00:58:40)

So if your team or you're an AI PM and you're thinking about building an agent-based system, your first starting point would probably look something like this. It's not really going to look a ton simpler, to be honest, for multiple agents.

**Aakash Gupta** (00:58:55)

It's more

**Aman Khan** (00:58:55)

likely that there will be multiple calls being made to different services and taking data out of that and putting them back in to then use for LLM calls. So I just wanted to set that kind of context, which is like your starting point is to see what's going on underneath the hood and try to understand... LLMs, LLM calls, tool calls, agents, and how they all sort of ladder up into this overall system.

**Aakash Gupta** (00:59:21)

And we even get the time. So we were saying like, oh, this might be a little bit slow, but this is break down. If you wanted to observe it, which is what we're talking about here, this is how you can break down. Okay, maybe we chip off some time with the budgeting one, and then you could go in and you could work on that.

**Aman Khan** (00:59:35)

Absolutely. I mean, and think about it this way. Like, you know, if I'm using a model... How do I know if I want to change to a different model? Let's say OpenAI launches a new model tomorrow. Is that a good thing for me to implement into my system? We should probably be able to see an A-B test, just like you would A-B test an end user experience. You can now A-B test different models. You can A-B test different prompts. The fact is that you probably want to, you know, in your tool that you're actually using for observability, you should think about ways to be able to do that. So let's actually take one of those examples here. This is a good one where it took a really long time to generate this itinerary. And what we can do is actually go and, you know, from here, we can actually go into a prompt playground.

**Aman Khan** (01:00:31)

So this is what it looks like when you are iterating on your system, right? This is the same system prompt that you would be able to see in cursor in your code and that your agent built for you or that your engineering team built. But what you have here are variables. And this is really important because this agent is being able to take inputs from the form for maybe hundreds, thousands of your users and plumb them in to get a reliable system on the other end, which is taking your destination, the week, duration, the travel style, and then takes the inputs of all of the other analysis and constructs a finalized itinerary. So this is the sort of the step-by-steps of take all of the other agent inputs and construct that final itinerary that you saw. So why does this matter, right? Well, I think you actually pointed out something really useful, right?

**Aman Khan** (01:01:32)

Like, which is, this is kind of long. Like, I don't know if I'm gonna read all of this. It's really detailed, but does it really need to be this detailed? And is this really the tone that I want the agent to have? What if I wanted this agent to offer a discount to users or act extra friendly? Well, that's really where prompt engineering comes in. This is another kind of core part of the workflows we were talking about, which is, so we've done prototyping, we've done observability. Now let's see what parts of the agent stack we can change and iterate on and what the output looks like. And to that end, we have rag, prompt engineering, fine tuning, right? And so we're gonna kind of go through each of those and see what the impact is on the end output of your agent.

**Aakash Gupta** (01:02:26)

Okay.

**Aman Khan** (01:02:28)

So I've got a model here. I can change the model if I want to. Let's try a slightly different one.

**Aakash Gupta** (01:02:33)

4.0 Mini, yeah. Andre yesterday said, don't use ever, right?

**Aman Khan** (01:02:41)

Exactly, yeah. I think it's being deprecated. I'm surprised. Maybe it still works, but let's see. And that's the thing. I mean, honestly, I know we're joking, but that's a really good point. These models are going to change all the time, right? Yeah. I love the like, oh, this new model came out. Here's my prompting guide for it. Those prompting guides, a lot of them, they do end up getting out of date when there's a new model or, you know, the old, you know, how you work with these new models changes. So what you could do is say like, I'm changing to this new model. How should I prompt the system? And you can generate a new prompt based on this as well.

**Aakash Gupta** (01:03:16)

We

**Aman Khan** (01:03:16)

actually have a tool that lets you kind of generate new prompts as well in the product. But let's say I want to just make some really specific tactical changes to this. So I'm going to go ahead and say... I

**Aakash Gupta** (01:03:32)

feel like we don't need a detailed day-by-day plan. Can we just delete that part and make it more like... a day by day event summary or something like that. That's a good

**Aman Khan** (01:03:40)

point. So what I'm doing here is actually changing the prompt and you can do is actually save, you could save this prompt and say, I want to iterate on it in the system and say like,

**Aakash Gupta** (01:03:52)

this

**Aman Khan** (01:03:53)

is my travel agent prompt.

**Aakash Gupta** (01:03:56)

Yeah. That's like the detailed version.

**Aman Khan** (01:03:57)

Exactly. Yeah. And then what we can do is sort of pull in that same travel agent prompt here.

**Aakash Gupta** (01:04:04)

So

**Aman Khan** (01:04:04)

now I'm actually iterating on the same prompt, but when I save it, I'll save it as a new version. So let's go ahead and it's a good best practice. So we're going to say, instead of a day by day plan, we're going to do, I think that's what I said before. We're going to say, give me, give me a, so, so actions. Give me a day to day plan. Doesn't need to be. super detailed, right? Because I don't

**Aakash Gupta** (01:04:32)

think

**Aman Khan** (01:04:32)

we're planning out our lives like day to hour to hour. It's really helpful when you're doing generation to also say, because we're giving all of this as context, this is all rag to some degree of context that the agent is using. And we're gonna say, you know, max 1000 characters, because we don't want it to go on super long.

**Aakash Gupta** (01:04:57)

And when you say RAG, RAG is retrieval augmented generation, which means kind of like condensing a lot of knowledge, right? Is that what it's about?

**Aman Khan** (01:05:06)

Yeah, good point. So yeah, so in case you've heard this term before and you're like, what is that thing? RAG is retrieval augmented generation. I like to think of it as giving, you know, when you're thinking about like doing a test or let's say you go to a doctor, the doctor might be super specialized. You can kind of think of specialization as like fine tuning. And when the doctor is kind of answering your questions, wouldn't it be great if they just had access to like the internet or to a textbook? And that's what RAG is. RAG is basically getting access to a specific part of the data of your overall data set that is useful to answer a question on the spot. So that's like the context that helps you answer a question basically or perform a task. So it's like, think of it as like pulling out a page from a notebook or a textbook.

**Aman Khan** (01:06:01)

That's really hard to find the right page, and that's a whole other area of study, but that's really what RAG is underneath the hood. It's just like pulling out data and using it. So another few things we can do is say, you know, always answer in a super friendly tone because it kind of sounds robotic to me. I feel like this itinerary, like I don't know if I would want to use this. I kind of want like, you know, something that might feel a little bit more interactive. And maybe we wanna build a product here where we wanna use this product to collect email addresses as just a super simple first pass, right? Like if you're a PM and you're like, maybe this is really useful for me to go get feedback from these users and ask them more follow-up questions, you could say, ask the user for their email and offer a discount.

**Aman Khan** (01:06:52)

So now we've done a couple of things, right? We're gonna change this to 4.1. We're gonna see how long that takes. as well. And we're gonna run the two systems against each other and see what the output looks like. So we're actually, we hit run all, which is gonna run the original prompt we have against the new prompt and take the models and actually compare the two against each other too. Okay, so that was faster. So you can see that, you know, it still took a little bit, but it's looking like a little bit more friendly here. In this case, it's

**Aakash Gupta** (01:07:24)

a

**Aman Khan** (01:07:24)

trip to Marrakesh, but it loves to use emojis. uh we've got the day by day um so let's let this kind of generate here still generating this output this is again the inputs that we're using and all of the research from the previous agents goes into here and now i've got let me kind of zoom in and make this a little bit easier to see we've got we still have the original this is the original prompt which is, I think it's definitely taken out the hour by hour, which was, I think we changed that hour by hour step here. But this is still a little bit more high level. Day one, day two, day three, day four. And it's definitely more friendly here. And it also says, would you like me to continue the rest of the two weeks? Also shoot me your email and I can send you a nicely formatted itinerary plus a cool discount.

**Aman Khan** (01:08:13)

I mean, this is like way more helpful, right? Like this is like something I would definitely want to interact with a bit more because it's a little bit more high level and you can always tweak it to get it to sound the way you want it to. This is what prompt engineering really is, is it gives you, think of it as like sculpting a block of clay or stone into getting it into the right shape that you want. The amount of impact that you can have from prompt engineering is huge because you can, you know, make the agent actually... listen to your instructions much more easily with text. So that's really what you're doing here.

**Aakash Gupta** (01:08:47)

Cool. So basically we changed the prompt that was sent to OpenAI 4.1 mini, which we specified here, whereas the other one had 4.0 mini. They both actually used the same input from the other three agents, but it led to kind of dramatically different result and dramatically different time taken.

**Aman Khan** (01:09:08)

Right, yeah, that's a really good point, right? Like the time for 4.0 mini, the same exact input, just slightly changed prompt, is 32 seconds versus this is 8.9 seconds. And that's where you can do things like change the model. And you can even A-B test even further. You can keep the model the same and just add that character, which was basically being able to basically retain, only max out like 1,000 tokens or 1,000 characters, for instance. So

**Aakash Gupta** (01:09:39)

that's

**Aman Khan** (01:09:39)

an example of the changes that you make and what impact they have on your system. This is like, I would view this as Try to change your model, try to change your prompt, very low effort. Once you have observability in place, very high impact on the end user experience.

**Aakash Gupta** (01:09:59)

So how do you set up the right evals to start to like in an automated way, understand whether you should adopt the latest and greatest prompt instead of kind of just as a human looking at it each time?

**Aman Khan** (01:10:10)

Yeah, good question. So evals are really helpful when you're actually making changes to your system and being able to quantify. Okay, now I can kind of... This is what you kind of call vibe coding, right? So we've kind of come up to this point. I would say everything up until this point is pretty much vibe coding because you're kind of like looking at the... You're basically giving text... You know, this whole time we've been vibe coding, you've been giving texts to the agent, it's generating output, you have an agent system, you've made tweaks to the prompt and you're like, looks good, looks fine. But I think that going one step beyond that is actually being able to run evals. And evals are the way that you can more quantify your system overall. So I like to joke, it's like going from vibe coding to thrive coding.

**Aman Khan** (01:10:57)

because you're going one step deeper, right? So what we can do is take some of these examples. And I actually ran a few of these yesterday on a similar agent, same agent system. And what I can do is actually build a data set and a very, very common workflow. I mean, look, we work, you know, with some of the leading like companies in AI, like Uber, Reddit, Instacart, Duolingo, all these companies. And the reason that we're building these tools to have a data set is because you want to be able to make a change to your system and know that, you know, quantitatively what the impact that change is having with evals. So there's a long winded way of saying I basically constructed a couple of examples here and let's go ahead and delete these so that we can actually just do this from scratch. I don't wanna, these are what we're gonna jump to later, so.

**Aman Khan** (01:11:46)

Okay. Cool. Okay, so what do we have here? So this is what's called a data set of the same data that you saw earlier. And specifically, I took the itinerary step and I've constructed a set of examples I'm going to use to iterate on top of. And that's really what these are. So if I go in, you can see it was the same prompt that we were editing in the prompt playground. And what we're gonna do is actually run evals on top of this system and see if we're making the system better or worse. And that's really what, you can think of evals as basically a way for you to understand. You can think of evals as a way for you to understand are you making your system better or worse, just very simply. Okay, so what we're gonna do is, let me refresh this page.

**Aman Khan** (01:12:45)

Just kind of look here. Okay, so let's create our first experiment and we're gonna go back into that prompt playground, but now I'm actually pulling in the data that you just saw. So I've picked and hand sampled those examples that I wanna use for iteration. I can do the same thing here, which is it has the same inputs and I have those outputs. And now what I wanna do is I actually made that change to that prompt that we were talking about earlier, and I saved it to the prompt hub. And so I'm gonna pull in this latest version of the prompt, and you'll see this is the same prompt we made edits to before. And now what I can do is, let me go ahead and A-B test this, and let's kind of make this a little more authentic. We said that this was GPT-40 mini, so we're gonna do an A-B test apples to apples.

**Aman Khan** (01:13:38)

And we'll do the same thing of hitting run all, but now instead of on one example, we're generating this on a data set of like 10 or 12 examples here. So it's basically giving you an output that you can use for experimentation. So this is generating a new output on that data. Yeah. To back up for a second, you have your initial dataset of examples that you've kind of built on top of. Even if you don't have that initial dataset, it's really just, I could go in and I could go and just add, basically what I did was I just re-entered, you know, instead of going to Spain, I want to go to Tokyo. And instead of one week, I want to make it two weeks. The budget could be like $500. And a lot of times what you kind of call this when you're building an application is bootstrapping a data set.

**Aman Khan** (01:14:25)

And it's just a way for you to get started. You can synthetically generate that data too.

**Aakash Gupta** (01:14:30)

So

**Aman Khan** (01:14:30)

using an LLM if you wanted to. Okay, and then now what we've done is once we have that data set, we can pull this in, and we've regenerated the prompts, and it looks like it actually generated the experiments for this. So let's go ahead and go back here. And so those experiments are the outputs from the prompt playground that we had before. So this is new outputs on the original prompt, and I can compare this to the change prompt that I used as well. So I've got two prompts side by side next to each other now. And again, if you're using the system, it's kind of hard to read, it's kind of hard to say, is one better than the other? I don't really know. So let's go ahead and run some evals on here. So I've got these evals set up, but let's go through the process of talking through what an eval is.

**Aman Khan** (01:15:28)

So think of this as there are basically three types of evals that you have options to use right now. One of them is human labels. And it's really important to go in and label this data yourself. And you can go and actually go through the data set and label the data. We'll kind of talk through that. We'll come back to that one. And that's really an important role for an AI PM is to know when I'm looking at an output, is this what I want the LLM or the agent to actually generate? Like, is this good or bad? Because you're ultimately determining the end user experience as a PM. You're saying like good or bad. And that's what the label is. The second option is to use code. And so you can do things like checking code. basically to say, it's like a Python-based eval, which, you know, Python eval could be things like check for instances of like, is a competitor referenced in the LLM's output?

**Aman Khan** (01:16:24)

And those are really, just think of those as ways of, you know, writing code to generate evals. And then the third option that we're gonna be kind of focusing on here is actually using an LLM to check the work of the other agent. And so you think of these as like eval types of agent systems that are really used to kind of scale up your feedback.

**Aakash Gupta** (01:16:46)

So this is what almost everybody's using these days, these LLM as judge systems where they create like almost like numeric scores with various dashboards to look at things.

**Aman Khan** (01:16:55)

Exactly. Yeah. So great point. So when we say like, you know, there's there's a lot of buzz around. evals are the secret and they're the moat what people say when they're saying like evals are the secret to a great ai product experience what they're saying is that you need a reliable way to scale up the feedback on your system and the way that you can do that is using llms as a judge or a grader on the output so that's what an eval as a judge or eval system looks like with llms And I'm going to break this down a little bit further for you, which is what we can do is basically give an eval template. And the same way that we had an agent basically going in and saying, like, generate an itinerary, generate a budget. What I'm doing is actually creating an eval, which sets the role, which is saying you are examining written content.

**Aman Khan** (01:17:50)

Here's the text. And then I've given the text from that we just generated as the output. And we're stuffing that into here as context. Then I'm giving the agent a task which says, examine the text and determine whether the tone is friendly or not. Friendly tone is defined. And then I'm defining and giving an example of like, here's what I mean when I say evaluate for friendliness. Please focus heavily on the concept of friendliness. Then I'm gonna give it an action, which is based on the information, the context, give an output label of friendly or robotic based on the information that you have so again we've we've said we've given the agent a role we've given it context we've given it an example of what is good or bad and then we've given it the action to perform and those four steps are really all you need to get an eval in place um to at least get started Now, what I will kind of caveat and say as we run this, and so once I've defined that, I can actually set these up here, and I've got another one here, and we'll kind of quickly go through this one.

**Aman Khan** (01:18:59)

This is like checking if we offered a discount to the user based on the email. So this is text that says, determine whether the text contains an offer for a discount. And this might be something we wanna check for, right? Did we actually accomplish that goal of giving a discount to a user? I can go ahead and just run these on the system and say, select the experiments. Those are the two experiments we have. And I'm just gonna hit run. And while that's going off, I'll kind of go back here. And this should run pretty fast, but what I'm basically doing is getting an LLM generated label on all of those rows that you just saw. And that's really helpful for me to then go one level deeper and say, was my LLM correct or was the judge correct? And I can basically go in and fine tune that even further.

**Aman Khan** (01:19:48)

So, Okay, and we did, one small note is we like flip the order of operations here because experiment two, okay, so it looks like experiment two was like the second one that generated and then experiment one was the first one that finished, which was the better one. So we're actually thinking of this like backwards, this chart, but this was like the one that took a really long time. This was the older prompt. Think of this as the old prompt. And you can see, okay, it was actually, I guess the LLM as a judge did note that as friendly instead of robotic. But it looks like it offered a discount 0% of the time. And then if I go to the one that was faster, the new updated prompt, the LLM judge actually did mark all of the responses as friendly. And then it offered a discount 100% of the time.

**Aman Khan** (01:20:40)

So it actually went in and checked the outputs and said, did you give a discount or not?

**Aakash Gupta** (01:20:46)

yeah what if we did something like gave it like a friendliness score maybe that'll give us like more dispersion

**Aman Khan** (01:20:51)

yeah exactly so so what we when we generate uh the label when we generate the label, we actually do also get a score with it as well. So we've just assigned a one or a zero as the output. And then you could go in and say, give me a friendly score from one through five. Fun fact, Akash, for people that are listening to this, this is a best practice is actually to use text to ground the output of the LLM judge. The reason for that instead of numbers is... although this technology is amazing llms are still really bad at being able to understand numbers um fun

**Guest** (01:21:31)

fact

**Aman Khan** (01:21:31)

just from a tokens perspective so i said

**Aakash Gupta** (01:21:33)

yeah

**Aman Khan** (01:21:34)

if i say you know put a one or a two it won't really be able to give you the justification for why it picked one versus two but

**Aakash Gupta** (01:21:44)

if i

**Aman Khan** (01:21:44)

say score from uh bad good, very good, really, really, you know, if I give like more distinct text, that's a better way to generate a label from

**Aakash Gupta** (01:21:54)

a

**Aman Khan** (01:21:54)

judge. So that's just the

**Aakash Gupta** (01:21:55)

best practice. Text labels over number labels. Yeah,

**Aman Khan** (01:21:58)

exactly. Use labels. And then let's go one level deeper, right? So like... i have this eval but i i kind of maybe want an explanation for why i got a specific score well the llm as a judge actually gives you an explanation so it's giving me the justification for why it gave a specific label and this is all of the reasoning of the llm judge as well so it's actually the chain of thought of how it analyzed the text to say, you know, should this be, is this considered friendly or not friendly? So that's really helpful as well as make sure when you're generating evals that you have an explanation that you can go in and understand one level further. Now, you might disagree with the LLM judge, and that's okay, right? That means that that's a system. When you think about your system, you have your agents in your application, you have your evals, but that doesn't mean that they're perfect off the bat, right?

**Aman Khan** (01:22:58)

You might want to go in and iterate on this LLM as a judge. And to do that, that's where those human labels and human annotations kind of come in. So what you can do is actually take that same data set and go in and actually label it as friendly or not, and use the same labels that you're using for your LLM as a judge. And in here I've actually labeled, I actually think a lot of these responses are robotic. So this is an example of an AI PM basically saying, hey, I actually think the LLM as a judge needs improvement and I want

**Aakash Gupta** (01:23:33)

my

**Aman Khan** (01:23:33)

team to go and improve on that system. So what you can do is add your own label and there's a there's really is kind of a note here of as we get a little bit further like whose job is it to generate the labels i argue a pm should be in the data and labeling and basically saying what's good and bad so that you can give a metric for your team to go and improve on

**Aakash Gupta** (01:23:56)

and i've said

**Aman Khan** (01:23:57)

these are bad like these i don't i i went in and labeled those these uh as i was generating these yesterday and i was like i think these are pretty robotic Well, once you have that system in place, you can actually take the same human labels and do another LLM, either an LLM or a code-based eval that says, take that human label and match it to the eval that was generated and tell me if my human label matched the LLM as a judge or not. And that's really helpful to say, Is what I'm saying the same thing that the LLM as a judge is saying? And if not, I wanna know why, and I wanna go one level deeper.

**Aakash Gupta** (01:24:38)

So

**Aman Khan** (01:24:40)

we're gonna go ahead and run this eval on the same experiments. And this is what's called like a match eval basically to say, should I go ahead and improve on my LLM as a judge? So it's actually going one level deeper. I don't, I don't see too many people actually, when they talk about evals saying that you need to check the work of the LLM as a judge, but this is, this is what that looks like is taking human labels and comparing them to your LLM as a judge.

**Aakash Gupta** (01:25:09)

Yep.

**Aman Khan** (01:25:13)

Okay. Awesome. And so what, what I have here is this is an example of where I actually need to go in and you can see my, in this case, I was a discount check and it looks like my, it did always offer a discount. And here I also matched a hundred percent. And so this kind of tells you, okay, when I didn't match on a specific eval, I want to go in and figure out why that is, uh,

**Aakash Gupta** (01:25:38)

like

**Aman Khan** (01:25:38)

why is my judge different than my, my label?

**Aakash Gupta** (01:25:44)

So where am I seeing that it didn't match? It looks like it didn't match on the left side for friendliness, is that right?

**Aman Khan** (01:25:50)

Yeah, so I think this one was a discount one, but we should, you know what? Let's just make that a little bit more, let's just make this example a little bit more concrete. So I'm gonna go ahead and actually remove, let me go ahead and create this eval one more time and just do, this one was a discount one. Let's go ahead and do a friendliness one. I think that's actually a better one, honestly. So we're just going to generate this on the fly. Again, it's not super complicated. I'm basically saying friendly. And you can see I have my type ahead here a little bit. So we're going to use friendly. And then we're going to do the same thing over here. And so what am I doing here? I'm basically using an LLM. I mean, it could be code. This is definitely, like, you have options here of, like, do you want to do this with code or do you want to do this with LLMs?

**Aman Khan** (01:26:42)

We're going to

**Guest** (01:26:42)

do this

**Aman Khan** (01:26:43)

with an LLM just because it's a little faster for me. And I'm saying check if the eval label matches the annotation label. This is a really lazy eval. But you can, you know, if you were actually doing this in production, you would make this more specific. And then the Rails system is basically just making sure that you get a label that you can use for plotting the chart. So we're gonna do a friendly match. As you just mentioned, what am I actually checking for here? I wanna make sure that my friendly label matched or didn't. And so let's run this here. It should only take a second to run. The point of a lot of this though, while this is running is that when you think about your system as a whole, okay, actually that ran faster than I thought it would. So let's just talk about that for a second.

**Aman Khan** (01:27:36)

We'll come back to the zoom out. So you can see here, my friendly label matched 0%, which means I thought that all of those results were not friendly. I thought that they were robotic yesterday. But the LLM thought that they were friendly, right? Like the LLM as a judge was like, this is friendly enough for me. That's an example where I would go in and say, hey team, let's go iterate on our LLM as a judge text and make it catch what's friendly, not friendly better. So that's what's really helpful is like my LLM as a judge is totally misaligned from my labels, my human labels. That's what that's telling me. Got it.

**Aakash Gupta** (01:28:14)

Yeah. And then we could go in and we could, how would we iterate and improve that judge?

**Aman Khan** (01:28:19)

Yeah, so that's a great, great question. Why don't we just do that on the fly, too? So we've got a friendly here. Let's go ahead and try to rerun this.

**Aakash Gupta** (01:28:32)

Like, is there a way to give it our human touch and then get it to, like, just learn that human labeling?

**Aman Khan** (01:28:39)

Well, now, I think... I'm like very, I would love to show the workflow for that, but to be honest Akash, the truth is that that's coming out really soon on our end. So if you check, by the time you're watching this, the workflow will actually look really different because we'll have a button that says, take the human labels and optimize your prompts. So that's the part of like a little bit of like, when you think about how self-driving cars or fine tuning works, it is actually taking those labels and using that to iterate. And we call that prompt learning. And actually

**Aakash Gupta** (01:29:25)

Andre

**Aman Khan** (01:29:25)

Karpathy also tweeted about something similar, which is take your human labels and use them to iterate on your prompt. So it's a little bit of the, like, coming very soon. The workflow is, you can do the workflow today, which is take the eval and try to hand tune it a little bit based on the human label. But yeah, wouldn't it be great if you could just click a button and it updates your prompts for you? So that's the product that we're working on next.

**Aakash Gupta** (01:29:52)

So this is evals. I think where I want to go next is start to break down some of these terms. We talked a little bit about rag, but fine tuning and prompt engineering and really understand how they all fit together.

**Aman Khan** (01:30:04)

Yeah. So I think like it's helpful to zoom out and see like, what do all of these things really mean when you build a product? And to that, I'm going to go to just Excalidraw and just sort of whiteboard some of this. Um, By the way, just as a note, do you think we should start here? Should we go up to the cursor, like the bolt example? What do you feel like would be more

**Aakash Gupta** (01:30:28)

natural? Maybe we start with the bolt diagram.

**Aman Khan** (01:30:31)

OK, perfect. Awesome. So when you think about pulling all of these concepts together, I think it's really helpful to go from, you've built this initial system, but what does this look like in practice when you go from prototype to production? And I think it's helpful to look at great tools out there that we all kind of have used or tried at some point and that are really taking a lot of attention from the AI product mindset. and try to understand how they work a little bit more. Maybe we can use this as an example to just go through like how Bolt works at a really high level just to pull all of this together. So if you haven't used Bolt yet or, you know, I like to do this thing in person, like where I'll ask how many people have heard of Bolt or Lovable? Everyone raises their hand.

**Aakash Gupta** (01:31:20)

Okay, how many

**Aman Khan** (01:31:21)

people have like actually tried to use the tool and like half the hands go down? And I think that's part of the problem. But I do recommend like, you know, we jumped into the deep end with Cursor. If you haven't tried Bolt yet, please go and try it. It's really straightforward. Just ask it to do the same prompt we just gave Cursor and you'll get a good A-B test feeling of like what's different between these systems. So once we've built something in Bolt, what you'll kind of notice is it's a workflow which also generates code and gives you a UI as a prototype. It kind of feels like magic, right? Like, I feel like, you know, I had this feeling when I first tried, I was like, wow, holy cow. It just knows exactly what to do and built this UI in like one second with everything that I asked for.

**Aman Khan** (01:32:05)

but it's not magic. And let's talk about what's going on underneath the hood a little bit more. And I wanna preface and say like, this is just from reading the code and that's why it's so important to be able to read code so that you can interpret, you know, what's going on with your AI product. So what you can do is Bolt has their code hosted on GitHub, like an open source version. And if you go in, I thought, wow, this is gonna be really sophisticated, but really, at a high level bolt contains a system prompt which you we just saw what a prompt was with an agent a system prompt you're going to notice a lot of similarities here and you'll see you are bolt an expert ai assistant an exceptional senior software developer with vast knowledge across multiple programming languages so what bolt really is is it's basically a really big good prompt which is doing the same things we just talked about you're setting the role you are a developer you're setting context you're saying you are operating in an environment called a web container you're generating tools or implicit tool calling.

**Aman Khan** (01:33:09)

I call it implicit tool calling because you're referencing the tools in the context. You're not explicitly calling a service externally, but you're sort of setting, you know, here's what's available to you to be able to implement something. So it says, prefer using Vite, which is maybe just a framework here instead of implementing a custom web server. So that's like saying, don't go off and use a tool that's not Vite. and then you set priorities in the instructions so you can see literally the prompt contains important use valid markdown ultra important do not be verbose so you're really setting what the output looks like in your prompt very important you're then providing few shot examples of what good looks like once bolt contains all of this information in the prompt really all that's going on is it's taking this user input request and that's being fed into the agent system with the same context we just talked about, the system prompt, the user prompt, and then access to all of those tools in the prompt itself, which are structuring the problem, picking the right framework.

**Aman Khan** (01:34:20)

There's a concept of a terminal and then retrieving context above. And these are, think of these are just like components in your prompt here. All of that goes into an LLM, and then you get generated code. And that generated code, I thought this was gonna be way more sophisticated. With Cursor, there's like a three and a half hour interview with the Cursor founders on Lex Friedman. It's fascinating. I was like, wow, Cursor is a really sophisticated problem to solve. And then I was shocked at you can get such a good result with Bolt and Lovable, Because really all they're doing is generating code and rendering that code. So it's just going into basically an environment which takes the code that's written and is just able to run the code, executes it. And if there's a problem, it will go back and fix itself. Similar to the agent that you just saw.

**Aman Khan** (01:35:12)

But it's really, why is this important to note? Because... Bolt is even simpler to some degree in terms of the system you see here than the agent that we wrote in cursor, to some degree. Because what's really the secret sauce here is you can take generated code, break it up into files, and then render that code, and you get a UI. Now, if you try to use Bolt to make external API calls, for instance, or call other services or images, it gets a lot harder to do because of what Bolt is wired up to. It's a closed box, basically. You can't go in and plug in external things to it very easily. And maybe just to recap that, it's really just a system prompt, goes into reasoning to generate, what do I need to do? Let me make a plan. The same thing we just saw with the cursor agent.

**Aman Khan** (01:36:04)

What tools do I have? Takes that context, generates code, deploys it, and then renders that code. And then based on user feedback, it can iterate on that. And what that really means is, I like to think about this as product principles for a full stack coding agent, where you can pull together prompting, your system prompt, prompt engineering, reasoning in the form of agents. Really it's like agent-based reasoning or chain of thought reasoning. Tool calling, in this case it's implicit tool calling, and RAG, which is the context from that you've just provided the agent. All of that goes into an LLM and you get the generated code. So it's kind of constructing your, you could fine tune the model more if you wanted to, the LLM layer. You can update your rag and change what context is provided. You can change your prompts. And that's a huge component of this as well.

**Aman Khan** (01:37:00)

And then you kind of string all that together with evals. And you can basically get this really, you know, kind of slick generated code on the other end. I actually put evals in green because from what I could tell, Bolt isn't running evals on the fly and that's actually an opportunity. I think like this is an example where if you're an AI PM, take note of what are the opportunities in the system where you can go and actually improve on the system overall. For instance, there could be a version of Bolt that never makes mistakes. Like you could have it running an eval on the fly. Right now, Bolt is, when you're actually running Bolt, it can break because it's making mistakes in code. you could have an eval that's run that checks is the code correct or not and that would be an example of running evals to actually improve on the system make bolt even more reliable and so those are all i think of this as like tearing down a product out there and thinking oh what are the opportunities to make this better and

**Aakash Gupta** (01:37:57)

that's

**Aman Khan** (01:37:57)

that's really helpful to pull all of this together

**Aakash Gupta** (01:38:02)

so if we go back then and we compare those three terms that fine tuning, prompt engineering, RAG, how do those all compare and when do we use what?

**Aman Khan** (01:38:12)

Yeah, good question. So you've still got the system here where this is all kind of, you know, different components. When should you use what, right? That's sort of the note of your question. And I kind of, I think it's helpful to have just like a really quick diagram here of like, what is each thing? So let's look at prompt engineering. It kind of depends on what your goal is. So if your goal is to adjust the tone or the instructions, I think prompt engineering is really helpful for that. So that's basically changing. We kind of did that just now on the fly with our agent and with Bolt. You can see you can change the instructions and the tone. That's how Bolt literally works. With RAG, you can provide context over a lot of data. So if you need to give the agent access or the tool, your AI application access to data internally in your system, that's when you would use RAG, which is using that data to create a generation on top with the context.

**Aman Khan** (01:39:10)

So you're stuffing that into the prompt. Fine tuning is, think of this as adjusting the model layer a little bit. So it's actually taking the LLM and making it more specialized. What's really useful for fine tuning is sort of style to make sure it always responds a certain way and increases the reliability. And then I put distribution, but distribution is like giving it more data in the LLM itself that makes it more specific or specialized. It's useful to think about what's the effort of each of these. Prompt engineering relative to some of the others is really, really low effort, actually. All you have to do is have access to the prompts, change those prompts, and then get the eval result to understand are you making the system better or worse. RAG is a little bit more complicated where you have a database now, so how you retrieve information from the database can have an impact on how much work this is actually.

**Aman Khan** (01:40:09)

And then thinking about like fine tuning, if you change the model layer, you change this variable that might have a lot more impact on the rest of the system. And so I kind of view this a little bit more as like medium to high today because it requires a bit more sort of specialization to adjust the model. That being said, the impact is really important to think about too, right? Like as a PM, we're always thinking, what's the effort? What's the impact? The impact of prompt engineering is really high. And in fact, that means that, you know, a small change to the prompt can get you 10, 20, 30, even more percent gains on your eval scores. Think about it that way. Like if you're designing your AI product around your evals, like evals are your requirements now. then you really want to think about how can you have the highest impact on those.

**Aman Khan** (01:40:55)

And I think prompt engineering is huge. RAG is another really high impact way to improve on your system. A lot of times this might mean like adding RAG to your system when it doesn't have it already. So just adding more context or adding better context. And then I think fine tuning, it sort of depends on what you're trying to do. Fine-tuning is really helpful for saving cost, which might be a very serious concern as you scale up, or reducing latency in your system. So if you want the model to be faster, fine-tuning can be really useful for that. Another helpful way to think about this to some degree, and this is not perfect, so feel free to grill me in the comments that I got this wrong, but this is my mental model I use. I think of prompt engineering as giving really clear instructions to an engineer or to an employee.

**Aman Khan** (01:41:43)

Because what you're trying to do, the more specific you are, the better result you're gonna get. Like in the beginning of this video, if I had given clearer instructions to the agent, I may have gotten my tool, my product out faster, but we wanted to see what it looked like to just like try to prototype with not great instructions. And that's the output that you get. With RAG, I think about this as like a doctor having access to the medical textbook at all times. Meaning this agent can go and look things up to get more information. Like if I copy-pasted a doc into Cursor, it's gonna go to that website and read the doc to try to understand what I'm asking it to do. And that can be really helpful when you're asking it for stuff that it doesn't know in its memory already. And then sort of last but not least, fine tuning is sort of like going from college to specializing in a career.

**Aman Khan** (01:42:31)

What's kind of interesting is that these models are so good now at generalizing that you kind of trade off things when you go to specialization. Like, you know, a lot of people view hallucinations as things you want to remove, but I think hallucinations are a feature, not a bug of these models. And so just note that when you change the model architecture by fine tuning, you might be getting rid of some of the generalization that can be really helpful. for a production application. So this is my mental model for like prompt engineering, rag and fine tuning, and how they all kind of come together when you're thinking about building an AI product system.

**Aakash Gupta** (01:43:08)

Awesome. So we covered four of the five skills. The final skill, and I don't know if we'll need screen share for this, you tell me, is working with AI engineers and researchers, working on these longer development timelines, how can AI PMs master that? Yeah. So I think

**Aman Khan** (01:43:26)

this is where I'll come back to like, what are we, what are we kind of talking about when we say our, our job is changing as AI PMs. And I think about this as the, the expectation on AI PMs is changing. from our stakeholders. And our stakeholders, when we think about who are they right now, they're not necessarily just engineers that were working in their own way either. Like the way engineers are working and how they're expected to work is changing too. And if you're working on AI products specifically, you might have data scientists or AI engineers that are also ramping up to using Gen AI in their workflows as well. So they're gonna be using data to make decisions. And I think the best way I can think about here is, Your job now has become to get a little bit more in the details of what it actually takes to ship an AI product by understanding the core concepts and principles of what goes into great AI products, understanding how they work and when to use what tools.

**Aman Khan** (01:44:39)

And then sort of very importantly, last but not least, when you work with an AI engineer is to know what they're thinking, what they need from you. so let's take an example of what that means tactically when when we're thinking about evals an ai engineer might be looking at an example and saying like was this the agent good or bad in this case like you as an ai pm should be able to answer that question because you are representing what the end if you sort of experience for a customer looks like right like you are the ultimately the person that's like on the hook if the AI product is successful or unsuccessful. And so I think I really view it as you want to be in the details of what the team is working on and how it works. You want to be a little bit more in the details of the data of is the experience good or bad?

**Aman Khan** (01:45:27)

And can you give that feedback back to the team to know what to go and improve on? And then I think, last but not least, being able to interact in the same platform and work in the same tools as your AI engineers is gonna help that communication much more. When I talk to AI engineers, what they come back and tell me is, I can't believe my PM is still sending me Google Docs. of PRDs and saying like, go and implement this thing. I wish that they would just be able to look at the system as a whole of like what the agents actually look like and what they're calling and be able to tell me, is this correct or not? Or I wish that they were actually looking at customer data and telling me what's good or bad. And so I think that that's really important is to speak the same language as your engineering team now, as they're ramping up on building around AI as well.

**Aman Khan** (01:46:19)

And this is really an opportunity for AI PMs to stand out from other sort of product managers that maybe haven't ramped up in that way either. I would argue that the stronger you are at communicating with data, communicating around what are the concepts to implement in your product, the more impact and sort of influence you're gonna have as an AI product manager on your organization and on your leadership. Because to be honest, you might even be able to influence at a higher level than even what you were able to do before because you're able to communicate around these terms more powerfully.

**Aakash Gupta** (01:46:57)

So should PMs be writing AI evals?

**Aman Khan** (01:47:00)

Oh, I think absolutely. I think evals are... I would really reframe this as like... you know, we kind of mentioned evals are kind of what tells you what's good or bad about your system, but what if evals were your requirements instead of your AI product? So like you come back to the team and instead of saying, you know, when you think about a PRD product requirements doc, What if that actually looked like an evals requirements doc? And instead of a doc, it's actually just, here's the data, here's the eval score. Now you guys go and improve on this eval and show me how you're improving on that. And that is a really interesting position to be in because you can work with your engineering team on getting the right data in place. You can be hands-on with them and you'd get to determine like what's good and bad at the end of the day, which is what the end product experience actually looks and feels like.

**Aman Khan** (01:47:50)

And I guarantee you that what we just saw, a lot of the code, like AI engineers, they want to be thinking about the right model. They want to be thinking about context. They want to be thinking about prompting. But they're not necessarily always going to be thinking about the end user experience the same way that you will. Like they're thinking about implementation. So they need someone to give that feedback of end user experience. And I think evals are a really good way to represent that.

**Aakash Gupta** (01:48:18)

Awesome. Awesome. So that's our mini crash course. We've talked a little bit about how to become an AI PM and in other places you've talked in even more detail. What should you not do?

**Aman Khan** (01:48:33)

Yeah, that's a really good question. I think I kind of view this as like, what are some of the things I see people doing today that, you know, from an AI PM, like they could be doing, like what are people not doing today is one way to look at this, like where there's a set of opportunities here. I think generally, if you are thinking about what we just walked through from a project perspective, Imagine if you had side projects kind of going all the time to help you kind of use these tools. So very common mistake I see is AI PMs don't, you know, I'll talk to AI PMs and I'll say like, what are you working on the side? That's actually, by the way, like a bit of an interview hack is like, it's actually like my first interview is usually I ask like, aside from work, like what are you building on the side?

**Aman Khan** (01:49:26)

And the reason for that is you can immediately tell what someone is interested in and you see that they're curious, you see what their interests are, but you also see that they're taking initiative and they're trying to build and use these tools on the side. So you can immediately gauge like how close are they to actually building products? How much do they really care about building products? So that's a very common mistake I think I see is like, you know, if you don't have side projects, you might, kind of end up having a bad time in the interview process. And I think a classic example of someone who does this really well and posts about it is Claire, Claire Vo. Like she has chat PRD. you know two years ago out right like i actually use an early version of that system and i'm like it's not that great like what's different about this than like talking to chat gpt but then you realize that she's been using this side project to learn about the stack every single week on her weekends and so the architecture has changed the models have changed so very classic example kind of building off of that is like you don't have side projects if you wait until the models get better, you're gonna be left behind as well.

**Aman Khan** (01:50:35)

So Claire kind of took that project and kind of kept iterating on it and building on it. So now when the models get really good, the product gets better and you already have all of that scaffolding and experience that you've built up building the side projects to take advantage of the newest models. So just imagine like if you already have some product ideas or problems that you wanna solve in your day-to-day life, then you may as well start getting building on them now so that when the models do get better, you're not waiting on that. You're actually already have something in place to just kind of plug and play the model. And then I'll kind of take another sort of step back and say like on the other end of the spectrum, a very common mistake I think I see AI PMs make is trying to automate too much of their job off of the bat.

**Aman Khan** (01:51:23)

So what I mean by that is you want to use AI as like a second brain to save costs by doing things like analysis and deep research and maybe even taking some action on your behalf. But I would be really careful about automating too much right off of the bat. So kind of leverage the fact that these reasoning models are really good at being able to do analysis and push and poke your ideas a bit. So let me give you an example of that. Some of my favorite prompts when I use a reasoning model, and when I say reasoning model, I mean like O3 or now the new Cloud4 as well, which can basically run, the LLM sort of runs for longer and thinks about what response to give you. And one prompt I'll use really commonly is give me five alternative solutions to what we just talked about and rank them in order of risk or ability to accomplish a goal.

**Aman Khan** (01:52:18)

And then give me pros and cons of each. So what that does is it helps me interrogate my own thinking a bit without trying to automate too much away or just take the first solution from the LLM and try to go implement it. So my recommendation is don't try to automate too much and just take the first recommendation, like push back a little bit and learn how to work with your LLMs and agents to get more out of them. Another example of that is like help me simulate follow up questions from a customer or a vendor. in a space I might not be as experienced in and say, what are some of the questions they might ask me? What are some responses I should give? And then what are some follow up questions based on that? And so now you can actually show up to an interview much more prepared for what direction some person might take the questioning.

**Aman Khan** (01:53:06)

And that's like another recommendation of, you know, you can't really automate that because at the end of the day, you're still going to be on the other side of the screen or a conversation. And you should kind of be able to anticipate what someone is going to say. So those are a couple of examples. I'd say three examples, you know, have side projects. If you don't have side projects, that's a really common mistake. Don't wait until the models get better. Like now's a great time to just start building something and swapping your components in and out. And then don't try to automate too much right off the bat. Learn how to use AI as a second brain to scale up your analysis and research.

**Aakash Gupta** (01:53:42)

Amazing. So a lot of that sounds like it could be a lot of work, especially the side projects. But if somebody just has two hours a week and they want to become an AI PM, what are the exact steps they should follow?

**Aman Khan** (01:53:55)

Yeah, good question. And I feel this myself, right? Like we have to, you know, we have commitments, we have commitments to our jobs, to our families, to other people in our lives. And we can't, you know, trying to ramp up here, it feels like a lot, especially when the space is changing so rapidly. And It's hard to keep up, definitely. The three things I think about whenever I feel like there's something new or something I'm trying to ramp up on when it comes to AI specifically, it's really just three steps. I'd recommend to try the tools yourself firsthand. I then recommend to build AI intuition and then apply that AI intuition. And let's kind of talk about each of those in a little bit more depth. So when I say try the tools, I don't mean like go and try to like implement them into your company right off the bat.

**Aman Khan** (01:54:48)

I don't mean like go back to your CPO and say like, we need an AI agent. I mean, just try the tools for your own kind of use cases and day-to-day life. an example is you know i wanted to build an ai storybook generator um for someone in my life and i was you know like for for a young child and say let me build images specific for this person based on a theme and based on you know what uh what i might be trying to like tell for like a bedtime story or something like that right like really nice use case for for a kid and i think When I tried to use the tools, I actually found where they fell short and what was hard about them. And so when I actually started using the tools myself, I started realizing, huh, this is what is possible.

**Aman Khan** (01:55:33)

And here's what's hard about using these tools. So when you do that, you kind of you gain a sense of AI intuition a little bit of like what's possible today and what's hard. The next is, I think, trying to tear down AI products by building AI intuition like we just did with Bolt. So when you see an experience that feels magical, try to go one level deeper and understand how the system works a bit so you can see how these kind of buzzwords like, MCP, RAG, like how they come together to actually form the system you just use. And they feel a little bit less like hypey and a little bit more real, right? Like the same way we just said with Bolt, like it's not using a ton of complexity. It's actually just prompting. And we kind of learned that by tearing the system down.

**Aman Khan** (01:56:18)

You can do this by watching YouTube videos, talking to other AI PMs. You can try to look at code as you get more proficient or copy paste the code into an LLM and ask it to explain it to you. And then you can just try to recreate the product a little bit yourself and see what's hard about that. And then I think last but not least is actually try to apply these two things, apply your curiosity and what you've learned and try to build something that you can keep going on the side as a side project where you can actually try to build your own product. And that way you're always kind of motivated to try to try a new technology and see if it makes your product better or worse. So those are I think if you have two hours a week. You can at least try a tool, pick a tool, whatever it might be.

**Aman Khan** (01:57:01)

This week for me, it's gonna be Veo3 because that one just launched. And I wanna go and try and understand, okay, how good is this thing really? Can I build something around it? And then I'll kind of learn what the boundaries are, what the edges are of the technology so that I know, okay, here's the opportunities around that. Here's what I can take back as learning. And the whole goal is really just to keep learning so that you can apply that in your day job or for projects you might be building.

**Aakash Gupta** (01:57:28)

So I was really excited to have you on. I consider you, Tal, Colin, Pavel, like four of the best AIPM creators. But there's a little group that's been criticizing us, talking all about AIPM. And what they keep saying is, where are the AIPM jobs? So are there really that many AIPM jobs out there?

**Aman Khan** (01:57:50)

Yeah, I think so. I think part of it is like, I'll be honest, I don't know if the hiring managers have like rebranded LinkedIn jobs to say like AI PM just yet. What I have been noticing is like, you'll see PM jobs that say product manager, like comma AI. And that's, that in my mind is sort of an AI PM job. What I will say is that the, the space, the PM space is really catching up here. So we're a little bit ahead of the curve and that's kind of where you want to be a little bit from a technology perspective is ahead of the wave so that when the wave really comes, you're able to ride that wave, just like in surfing, right? Like you don't want to be behind the wave, you're going to miss it. So think about, here's a mental model for you or like a, you know, sort of a thought exercise is think about like, realistically, what is the overall number of PM jobs out there today?

**Aman Khan** (01:58:45)

And think, okay, maybe it's in the thousands in your local city, wherever you might be living. But then think about in three-year times, how many PM jobs like that will there be? And what's the ratio of AI PM today relative to where we'll be in three years? So when you think about that, you might notice like in the headlines, you'll see companies are laying off entire teams, entire orgs, and PMs are sort of grouped up into that. But it's really rare and very, I think like, you know, I almost never see it where an AIPM team is going to be laid off to some degree.

**Aakash Gupta** (01:59:22)

And so

**Aman Khan** (01:59:23)

what you're trying to do is future proof your career a little bit by being ahead by basically either taking an AIPM position or positioning yourself as a what could be an AIPM to fill that role internally at your company, because that's where companies are starting to invest their resources when it comes to product management headcount because of the opportunity around this technology. So coming back to an earlier point, I don't think it's an either or. Like, I don't think it's like, you know, AIPM or bust. I think it's like AI as an opportunity that intersects with the type of product management you might be doing already, like fintech healthcare growth. And it's just that AI is another way to leverage that up a bit more.

**Aakash Gupta** (02:00:07)

And to prove everybody who's getting mad at us about these AIPM jobs, while Aman was talking, I decided to search on LinkedIn, right? AI product manager. And like he said, it's that product manager comma AI, you're getting over a thousand results just in New York City. So this is a real job out there. I've examined the compensation of this in other articles. These AI PMs are getting paid 20 to 30% more than regular PMs. We have given you the full toolkit today. If people want to go deeper, Aman, where can they find you online? Tell us more about what else you're doing outside of appearing on podcasts and doing your day job as a director of product. Yeah,

**Aman Khan** (02:00:48)

for sure. Well, so you can find me on amank.ai. That's my website. I'm also on LinkedIn. If you just search for Aman Khan and Twitter, we can kind of plug all the socials. I think for me, I really am trying to be as helpful as possible to people that are trying to make this transition in their careers as well to going from product management to either building around AI in their own products or using AI in the day to day. So my goal is really to try to just give away as much for free, give away as much as I possibly can to people so that they can understand how this technology is gonna impact their day job. In the same way, I wish people were doing that for me in the past. And so my recommendation is like, Pick, you know, content curators or creators like yourself, Akash.

**Aman Khan** (02:01:34)

You do such an incredible job of bringing on like, you know, extremely talent rich people that are, you know, able to share unique perspectives. And I learned something every time I watch, you know, your videos and read your content. And I think that that's really what I'm aiming to do is just try to give my perspective of being at the edge of building AI products, what I see, so that you can go kind of build that into your own companies or your own life. Kind of taking like, think of this as like taking the bleeding edge of AI and trying to make it more approachable for people a bit more.

**Aakash Gupta** (02:02:08)

Love it. And you also, I'm just looking, you have a course on Maven. What's that all about?

**Aman Khan** (02:02:12)

Yeah. So this one is a pretty recent addition, actually, to the offering. So I kind of view this as a way for, you know, you can think of this as like you could go get a gym membership and like watch YouTube videos. And I think that that's useful. This is sort of more of like personal training. is how I view it. So like you should really only take this course, to be honest, if you are kind of, you've already, you're in the early stages of the curve and you've maybe gotten to a point where you've built a prototype and you feel a little bit comfortable in cursor and some of the workflows we showed, that's really gonna be the starting point for this course. So think going from cursor prototype to real production application using evals and some of the workflows we just showed. The goal for me here is to give you an H1 or H2 strategy doc that you can take back to your leadership team for what an AI product could look like in your organization.

**Aman Khan** (02:03:08)

And to do that, I want to help you build the foundations of trying the products out at the early stages, but really going into, you know, day to day workflows of what AI product management looks like when you're building these products. So, yeah, that's this. The course is kicking off on July 1st. It's going to be a relatively small cohort to get started with. Based on that, we're going to try and run that more repeatedly, really as being a way for you to bounce ideas off of and really in a structured way to give you the tools to build this H1, H2 AI strategy.

**Aakash Gupta** (02:03:42)

All right, guys. If you want to go deeper, you can check out my code. It's in the description to get a little bit of a discount off of Amon's course. I can personally vouch this man knows his stuff. Good luck to you on your AIPM journey. Find both of us on LinkedIn if you need more, and we'll see you next time. Thanks for having me on, Akash. This was awesome. I really hope you guys enjoyed that episode. It would mean a ton to me and the team if you could please subscribe on YouTube, follow on Apple and Spotify podcasts, and leave a rating and review. Those ratings and reviews really help grow the show and help other people discover the show. And they help fund the production so that we can do bigger and better productions. Can't wait to share the next episode with you. Until then, see you later.
