---
title: "Inside the AI Stack of an $8.3B AI Company’s Product Team | Together AI"
subtitle: "I got a truly AI-pilled product team to demo the 4 key tools in their stack"
date: "2026-09-14"
host: "Aakash Gupta"
guests: ["Charles Zedlewski", "Necoline Hubner", "Pavneet Singh Ahluwalia"]
speaker_names: "substack"
substack_url: "https://www.news.aakashg.com/p/together-ai-product-team"
youtube_url: "https://www.youtube.com/watch?v=8TgxUPSuvNQ"
duration: "00:59:27"
word_count: 10195
source: "Substack episode transcript (aired audio)"
---

# Inside the AI Stack of an $8.3B AI Company’s Product Team | Together AI

*I got a truly AI-pilled product team to demo the 4 key tools in their stack*

**Charles Zedlewski** (00:00:00)

It felt like after a while that the new party foul was flooding your co-workers' context. We all just start launching slop at one another.

**Necoline Hubner** (00:00:08)

What if we could put all these linings into one place? And so that became this Together product repository.

**Pavneet Singh Ahluwalia** (00:00:15)

Together AI just raised an $800 million funding round, valuing them at $8.3 billion. I got their product team to show you their exact repo they use to automate their work. [music]

**Aakash Gupta** (00:00:42)

We've all discovered ChatGPT in 2023 and were horrified at the output and started handwriting. What is a good PRD in the AI era?

**Pavneet Singh Ahluwalia** (00:00:51)

I come from Amazon. I used to work at Amazon, so we are used to writing like 20-pager PRDs. What replaces the bulk of that is actually a prototype.

**Charles Zedlewski** (00:00:57)

We're all going to live in a multi-model, multi-harness world. That's essentially the new bar for UX for the kind of products we build. A lot of these things don't get magically better with AI.

**Aakash Gupta** (00:01:08)

Where does the line of product manager end and developer begin? Before we get into today's show, please take a second to check that you're subscribed on YouTube and following on Apple and Spotify podcasts. If you want access to all of my favorite AI tools, I've gotten them to give you an entire year of their paid plan. Check out bundle.akashg.com for an entire year of Bolt.new, Airtable, Speechify, Descript, Magic Patterns, Linear, Dovetail, Arise, and Mobbin. And now, into today's show. Charles, so I'm fascinated by how you guys work and how you guys have been using AI. What have been some of the big unlocks for your team in productivity?

**Charles Zedlewski** (00:01:51)

Together AI is a platform for powering AI applications and agents. And so we saw going back to the rise back when Cursor was starting to hit its growth spurt, what an amazing superpower an AI agent could be for any kind of knowledge worker in addition to and including product people. But it made me think a bit about what would a world be like full of product people and engineers that could all generate as much code and content as they liked. And it wasn't clear to me that the sum of all that was actually necessarily forward progress for us as a startup. And I imagine it's probably the same for a lot of other organizations. What we set out to do as a team is ask ourselves, what would it mean to use AI, but not to use AI to just make ourselves individually productive, where we all just start launching slop at one another, but rather AI to make us collectively more productive, that the code and the content and the research that we did actually advanced the company as a whole.

**Charles Zedlewski** (00:03:15)

That led us to a bunch of decisions about what we wanted to do centrally and what we wanted to leave people to be free to do individually. That's largely what brought us to where we are today.

**Aakash Gupta** (00:03:26)

How do you coordinate and centralize all this information?

**Necoline Hubner** (00:03:28)

Hi, I'm Nicolina. I'm a product manager at Together. A few months back, we've been talking about the way that we use AI in the hallway, but we never really sat down and discussed how We actually do our day-to-day work. And when we did, we found that a lot of people had unique workflows that made a lot of sense the area that they were working in, checking to see the reason behind a node failure, working with customer support, drafting reports. But then the rest of us were doing, on the day-to-day basis, we were doing things that were largely the same, researching customer needs, creating PRDs or one-pagers. And so we thought, you know, if we're really being thoughtful about how we're constructing these skills and how we're thinking about agents versus skills and now like, you know, loop engineering, what if we could put all these learnings into one place?

**Necoline Hubner** (00:04:25)

And so that became this together product repository. It's composed mostly of Markdown files, some YAML files as well. And what we put in here are both contexts that is useful for us across the board. So we have this context document or Markdown file. Sorry, this context directory and it has a number of groups of the products, the product grouping that we have. So customer intelligence, sandboxes, but we also have the result of strategy meetings that we have on a regular basis where we divide up product by mission, our strategy, what we want to accomplish, milestone over milestone, quarter over quarter. So that when we're thinking through our research and we're composing these documents with our agents, we can pull this context as it's relevant. And it's also useful to be able to look at the context from other people's sections. So if you're building something that is touching, we're going to create a joint workflow.

**Necoline Hubner** (00:05:29)

So if I'm creating sandboxes that reinforcement learning users are going to make, I can of course sit down with the product manager from the model shaping team Or I can look at the documents that she's already thoughtfully composed about their entry points and how they use SDKs and how an ideal integration might look and kind of work out a really decent proposal before I then put it before her and try to do that legwork. I'm taking advantage of the work she has done. On the skills front, it's a mix of things that are useful for anyone outside of a code repository. So everything that's relevant to specific code really shouldn't live here. But if you want to do something like figure out if we are serving all of the generative media models that all of the users are interested in, Artificial analysis, I can have that skill here.

**Necoline Hubner** (00:06:23)

So I could run that as somebody who supports generative media, but someone else could as well. And they can see the output of that in the terminal or things that we do on a regular basis. So this top line status one is one that I really love at the end of every sprint. We go through all the projects that we work on and we create an update of what's been shipped, what's ongoing, what's coming up next. And on the skill, you can just decide who, um, What areas you're going to pull from. For sandboxes, there's a lot of linear projects, but for the SDK and API, that pulls from a lot of projects. You can pull directly from a repository, see what features got pushed, and then it'll form an update based off of the sources that it was fed. Then you edit it, add additional updates that it missed or context that would be useful for leadership.

**Necoline Hubner** (00:07:14)

That's something that used to take me I don't know, anywhere from like 10 minutes to 30 minutes, depending on what I'm sleuthing through with the engineers, that now takes me a handful of minutes just to type in the prompts and then put the answers into the right location there. And as you can see, this is all Claude. Originally, I think we, for the most part, we adopted Claude code, but a lot of the harnesses that support open source models are We are used to looking at Claude Markdown files and being able to run them just as well. We've started to move more over to using our own models. One, because they're fantastic and it's really nice to use our own models. Two, it's more affordable because Claude is, I think, like many teams are learning across the globe that Anthropic and all these other models are starting to become quite pricey.

**Necoline Hubner** (00:08:11)

This is an example of using OpenCode. It's the same repository. This is one of the skills. It's just a news report that I run in the morning. It looks at our competitors, other model labs, just to collect information from what happened over the last 24 hours, and I will read it over my morning coffee. It takes a minute so I ran this earlier but you can see it's going to read the skill and kind of look through all of the listed sources that I wanted to find news articles for and then it will create a nice report that I can then click into and build out or read through any information that I want to learn more about that day.

**Aakash Gupta** (00:08:57)

So if we return to the context, like who owns and maintains this? Because the worst thing is if you're going to have like out of date context. So is that one, is that like, let's say Charles sets the overall product strategy. Is it his deliverable to maintain the strategy document that is in a good format for any AI harness or how do you guys manage these types of behaviors and responsibilities?

**Necoline Hubner** (00:09:23)

I think for the areas that, you know, the sandboxes or the customer intelligence that I own, it would be my responsibility. And then on the general, it has been kind of updated based off of larger events. So if we have a strategy or planning session, then someone would sit down and decide like who's going to sit down and translate that into what material. So there's typically a lot of Documents that have been written in the lead-up, and so it would be a matter of just translating that into a markdown file. But the CEO will write letters or write documents of direction, and that's a very clean moment. You know when direction is being set, and I think that speaks a lot to how well our leadership communicates direction. But you know that this is a pivot. They make it very clear. Lay it out for you.

**Necoline Hubner** (00:10:15)

And so that's kind of your signal. And I think as a product team, it's just a matter of us. I tend to update this, I think, quite a bit, but I think if anyone else makes a PR, it's like any other PR. It's like if somebody takes the initiative to create a PR, make the update to the markdown file, then that's that. But as soon as you want to pull from it and you realize it's missing, then you go ahead and make that change.

**Aakash Gupta** (00:10:41)

And going into the skills. So how do you maintain, how do you maintain like what's going to be a team skill and an individual? Maybe somebody has like a different way of writing a PRD. What is the sort of prescription or guidance? You should be using our team PRD. You should be customizing them. What's the line?

**Necoline Hubner** (00:10:59)

Yeah, I think when it comes to updating skills, there's a rule set on where each skill should live. You want to keep it closest to the work you're trying to do. So if it's a skill that is referencing code or is housed within, if it's housed within a set of work that a team is working on that's always in that one repository, then keeping everything whole located makes a lot of sense. And then all the rest of the skills Need to go somewhere. So you're either going to have a personal repository or you're going to have a shared repository and potentially you create a branch where you test out a skill and you say, okay, first I think this is relevant. I think this is repeatable. I'll see if I use this a few times. And if you do, then you can push it up to main.

**Necoline Hubner** (00:11:48)

And that's been my approach so far. And if it's something that I think is super niche, then it might just stay in a branch that never gets pushed.

**Aakash Gupta** (00:11:57)

Makes sense. And so everybody can connect into this harness using whatever model they want, but the harness primarily is these context and skill files. Is there any other components that people need to know about?

**Necoline Hubner** (00:12:08)

So there's the repository and then there's the harness. And the harness, there's many open source harnesses. Open code is one of the primary ones that we've been watching as it's evolved over time. And supported a lot of the models that we support as well. But HairMaze is also recently published one that I've enjoyed playing around with. And as you figure out which harness you prefer in your day-to-day work, or if you're looking for models that suit a specific I think a lot of product managers are starting to become a bit more familiar with what models are suited to different tasks. But as more open source models are coming out, I think it's really interesting to see how is GLM for coding? How is it for creating these product prototypes? Or Kimi for doing analysis. And I really enjoyed that experimentation because as these models evolve, you feel like you've got a lot more control over pairing the right model for the capability that you're after at the time.

**Aakash Gupta** (00:13:16)

I've been building a lot of AI products lately. My job search OS has 16 different agents. My newsletter has a recommendation engine. And I kept running into the same problem. I'd ship something, it would work in my testing, and then I'd get messages from users saying it's hallucinating That's where Arise comes in. Let me show you. Now Cloud Code already knows how to instrument my agent. I tell it set up tracing to arise and it automatically analyzes my My codebase figures out where the LLM and toolcalls are and adds instrumentation automatically. Now I can see everything. Every trace. Every span. Every decision. And more importantly, I can evaluate it. That's the shift. Trace what's happening. Evaluate where it fails, then fix it. This trace right here, my resume feedback agent was supposed to pull the company's tech stack from the job posting, but instead it hallucinated that they use React when the posting said Python.

**Aakash Gupta** (00:14:28)

I never would have caught that without seeing the trace. And here's the part that blew my mind. I asked Cloud Code to look at these traces and tell me what I should be evaluating. It came back with four eval criteria I hadn't written. Things like picking the right tool and staying grounded in the input. I wrote the evals, ran them, and found that my agent was making the same kind of mistakes That whole loop took about 20 minutes and now it runs automatically. If you're building AI products Amazing. So Pavneeth, can you show us what this is like in action? How does someone day-to-day use this for customer interviews, writing PRDs, and getting things into a state that they'll hand it over for engineers?

**Pavneet Singh Ahluwalia** (00:15:32)

Hey, Aakash. I'm Pavneet Allawalia. I'm the Product Manager for Infrastructure at Together AI. So how it really comes into action is basically based on two processes. One is the initial discovery and aligning process. And the second part is the build and ship, which is more automated. And really what this ensures is that as a PM, when I'm shipping a PR or I'm writing some code, it's not noise to engineering. It's actually grounded in our best practices in architecture. So let me show you this in action. So I have my cloud code here. I'm going to first start with like, see a feature that I want to work on, right? So let's say I want to do some research on a potential feature that I heard some customer complaining about. So one that I'm looking into right now is how many customers are complaining about shared storage resizing.

**Pavneet Singh Ahluwalia** (00:16:24)

And what this feature is going to do is it's basically linked to Pylon, which is where our support tickets lived, to Linear, which is where all our project and engineering execution is tracked, and to Notion, where some of our internal product documents live. And it's basically pulling all the information from there to show me how big is this as a customer problem, how many customers are complaining about it, give me some verbatims and some tickets that I can go and deep dive into.

**Aakash Gupta** (00:16:50)

So you had mentioned that Certain parts of the product process are more automated than the others. Which do you feel like are more automated?

**Pavneet Singh Ahluwalia** (00:16:57)

Yeah. So the way we see it is the part which is where the decisions are being made, right, which is defining the feature, defining the API surface area, the abstraction layer, those are very human in the loop, right, where I'm hands on with Claude. And the code writing part, the execution part, is actually the part which is automated. And how we would typically do that is like, I would basically trigger a goal, right? And say, give me production ready PRs for a feature to resize. So exactly the feature that we are going to work on, right? Resize, shared volumes. For a running cluster without destroying data, right? Just hypothetically. Now, typically as part of this goal, I will also give it a few other tasks. For example, give me a design doc that I can review with engineering. And first let's verify on a POC cluster.

**Pavneet Singh Ahluwalia** (00:18:02)

So we would typically deploy it on a cluster just as a POC to validate everything that's working as intended. And this is where, because goals are amazing, this will spin off multiple sub-agents and actually start tracking all the pieces. And it's going to prompt me for information along the way, for example, like a POC cluster or more information about the feature. And that's where we'll feed it the PRD or maybe a UX prototype that I built along the way.

**Aakash Gupta** (00:18:29)

So very, very powerful engineer skills. It sounds like you have a lot of confidence and the engineering org has built skills that you can just give a goal command, like get a production PR ready and it will go pull the relevant skills. It will be able to read your code base and get something actually production ready.

**Pavneet Singh Ahluwalia** (00:18:49)

Absolutely. We actually have a full engineering repo where it's just our architecture details, right? It's a bunch of skills which tells it for things that we've done in the past, how to redo it, like runbooks, engineering architecture, design documents, which Claude has access to through our shared repo. And that's why it's able to build high fidelity PRs in like a first attempt, really.

**Aakash Gupta** (00:19:14)

Wow. I didn't realize just how good these had gotten at AI Native companies. So that really then, like you were saying, in the human and the loop parts gives you a lot more time to focus on those in depth.

**Pavneet Singh Ahluwalia** (00:19:27)

Yeah. So if you see right now, it's actually spun off a subagent to look at how is the data plane working, and then another subagent to check how is the control plane working. And now a new one to look at docs, right? Is there existing internal or external documentation on how we might do this?

**Aakash Gupta** (00:19:45)

And do you have a point of view like you're using looks like cloud code in the terminal? How do you what's the easiest way to use a shared team repo harness?

**Pavneet Singh Ahluwalia** (00:19:54)

Yeah. So actually, if you look at this, it's currently running in my OS directory, which is actually pulled a lot of the shared repo artifacts. So, for example, Nico shared a few artifacts around research. So it's actually this skill. The feature research skill, which is actually a shared skill that everybody uses in the team. Then there's another one, which is my personal favorite, which is PRD Writer. This is actually pretty cool. Let me just actually trigger it off, right? So resize shared volumes for existing running clusters. So what this actually does is it does a turn-by-turn interview It'll interview me basically on what are the decisions I want to make in this feature. And if I show you the skill, so this is the actual skill. It ingests, it can take a prototype. So if I already have a UX prototype, it'll ingest that. If I have a running POC, it can take that or nothing, just like a simple prompt, right?

**Pavneet Singh Ahluwalia** (00:20:58)

And then it has access to all the information, the shared context that Neko shared about. Right. It's pulling all of that in. And then it's going to ask me questions turn by turn. And it's specifically instructed to not, you know, to push me, to challenge me on my assumptions and basically the decisions I'm making. And then it goes into drafting a PRD. And we've given it a question bank, basically, to kind of ground it in what type of questions typically we need to make. For example, like, what are the trade-offs? Is there any one-way door decision we are making along the way?

**Aakash Gupta** (00:21:31)

Amazing. So we've spinned off, I think we have currently three agents working for us, right? Research, PR, and PRD.

**Pavneet Singh Ahluwalia** (00:21:38)

Yeah, so this one is actually done. So the research agent came back. It's saying all these customers have asked for this feature in the last six months. There are 19 tickets that were filed in the last two months alone. So this is a pretty heavily requested ask. I have the source, so I can actually go into these tickets if I want to dig deep exactly what happened and why did customers ask this. And what was Pylon again? Pylon is where our support tickets live. It's the support platform. And then actually it figured out that we had started working on this feature because it has access to linear as well. And it was partially implemented, but it's broken in some way. So we stopped working on it. So now I'm not duplicating. I'm not like replicating work. I can actually build off somebody else's work or actually talk to that engineer and figure out, Hey, what happened?

**Pavneet Singh Ahluwalia** (00:22:29)

What issues we ran into.

**Aakash Gupta** (00:22:30)

And is this hooked up to the live code base? So it could go check, like in case there's some discrepancy between linear and the code base. Yes.

**Pavneet Singh Ahluwalia** (00:22:38)

Because it's in my personal OS directory, it has a skill which gives it access to all the internal GitHub repos and it knows what can map that.

**Charles Zedlewski** (00:22:49)

By the way, Akash, later on I can show you a God's eye view of what this looks like across all products for repos as well as across all customer feedback.

**Aakash Gupta** (00:22:58)

Okay. I'm excited for that. So beneath here, we've got the research report. What's your take on this research report? Is this a, like, how long would this have taken you? What do you give this out of one out of 10?

**Pavneet Singh Ahluwalia** (00:23:09)

Yeah. So if I had to do this manually, this would have easily occupied half of my day, if not more. And this is actually pretty good. It gives me the brief snapshot that I wanted to know, which tells me the feature passes the smell test. There are enough customers asking for it. I know most customers actually want to increase their storage volume, right? So I actually know what's my like MVP use case. And then I have a source so I can actually dig dive into some of them to actually get a better sense of the customer pain. And it gives me verbatims as well, which kind of helps. So I know, for example, here, it calls out a customer called Moonlake. And we have a separate tool called Customer Insights, where all customer calls live. So let me go into that. So this is the Customer Insights tool, where every customer call that our sales team is getting into, all our support tickets are getting summarized and cataloged.

**Pavneet Singh Ahluwalia** (00:24:02)

So I can actually go into this and actually see what exactly happened with Moon Valley. So they wanted a 50 terabyte, but there's a lock icon in the UX, which is preventing the action. And they are basically, they reached out to sales team and they basically want to sell some workflow, right? So I kind of get a pretty good sense of what the customer problem is within like five minutes instead of maybe a full day.

**Aakash Gupta** (00:24:25)

And this customer insights tool. So you guys have built an MCP server sitting on top of Gong and this has been visualized by V0. That's what we're looking at right now.

**Charles Zedlewski** (00:24:34)

It covers both Gong, Slack, Pylon. Yeah, at least those. So it's actually more than just Gong.

**Aakash Gupta** (00:24:42)

And who maintains this? Sales Ops?

**Charles Zedlewski** (00:24:44)

Hassan, you want to speak to that? It's largely automated.

**Aakash Gupta** (00:24:47)

Yes. Me and my team maintain it. So my name is Hassan. I run the developer experience team here at Together. And me and my team have built a bunch of this kind of stuff. We maintain it. We continue to have new features, but it's largely kind of working by itself. At this point, we have a daily cron job that runs every day that grabs all of the calls, all of the pylon tickets, all of the Slack channels, everything that happened in the last 24 hours, and it adds it to the database that this is running on. And yeah, what put me to showing is the daily screen that like where we show like five to 10 kind of insights from customers every single day based on all these calls. We also have an MCP server. We have a chat where you can ask it anything. There's a lot of kind of facets to this tool as well.

**Aakash Gupta** (00:25:32)

But yeah, my team continues to maintain it and kind of add new features here and there. Okay. So developer experience maintains like various MCPs. What other MCPs are you maintaining? Good question. We have this one. I mean, some of them, a lot of these tools are exposed differently. This one has an MCP server. For example, another tool is called Orchestrator. Charles is going to show it off and talk about it momentarily. That one has kind of Just a UI and as a wrapper on top of all our GitHub repos. And really my team just experiments with a lot of this stuff. We build things that we think may or may be useful for the product team and the rest of the company. And some of the internal tools kind of flop and we're Like, well, you know, this is not used very much and probably our two or some of our most used ones have been this like Customer Insights, MCP and App and Orchestrator and Agent Evals, which I'll also show off.

**Aakash Gupta** (00:26:27)

So those are like the top three that have been, that people have been using. Sweet. So we get to see all three. Awesome. And Bhavneet, how's our PRD and our PR agents looking?

**Pavneet Singh Ahluwalia** (00:26:40)

Yeah, so it's now asking for evidence. So this is where typically I would run this in a single chat because this is sort of somewhat sequential work. But typically then I would take the output of this research, which is pretty detailed for like a starter starting point. And I would actually give it to the PRD agent to run with. So now it has a sense of the customer problem. So it can ask me more educated questions on, hey, what are the trade-offs? Should we build as an abstraction? Should it be self-serve? When do we pull in support? Those kind of questions.

**Aakash Gupta** (00:27:14)

So almost like managing different agents that feed each other.

**Pavneet Singh Ahluwalia** (00:27:18)

Okay. So now it's asking me, hey, do you want to give me a Figma or a running POC or some screenshots? Or I can just say, no, run with it. Let's do it turn by turn by discussing it.

**Aakash Gupta** (00:27:32)

We've all gone through phases of using AI for PRDs. We've all discovered ChatGPT in 2023 and were horrified at the output and started handwriting. Then we discovered Claude and said, okay, maybe it can write well. And then it almost feels like people were overloading our colleagues' context windows with long documents. What is a good PRD in the AI era?

**Pavneet Singh Ahluwalia** (00:27:56)

Yeah. So that's actually a question we thought a lot about. So where we really use PRD, like historically, like companies started using PRDs as like a gating document where everybody, all stakeholders need to come together, align on it. And only then we'll start building the feature. A little bit differently where it's a tool to trigger ideation and problem solving. That's it. And it's short. It's usually one to two pages. It defines the customer problem well so that everybody has a shared understanding of the customer problem we are trying to solve. It lays out some solution options, right? Doesn't have to be fully thought through necessarily, but at least like what are the different ways we could go solve this problem, right? And then a sample user journey, like based on the option we want to go with, It will define either an API-based journey or a UX-based journey to show, hey, these are the three, four steps that a user would go through in the solved world once this feature is shipped.

**Pavneet Singh Ahluwalia** (00:28:50)

And that's it. That's enough to actually have a detailed discussion around, hey, how should we build this feature? What should engineering design look like? Is it even worth building or not? And that's it. That's what the PRD template that this skill uses builds off. And actually what replaces our typical historical six pager, like I come from Amazon, right? I used to work at Amazon. So we are used to rising like 20 pager PRDs. What replaces the bulk of that is actually a prototype. So we built a separate skill. Let me start a new cloud window. And there's a separate skill called UX prototype, which actually you give it that one pager that we just discussed, and it'll give you a very detailed prompt on how to build it in like a Figma make or any design by code too. Like you can use it in VO, you could use it in cloud design or even Figma, right?

**Pavneet Singh Ahluwalia** (00:29:46)

And that's where a lot more debate will happen because now everybody can visualize it, visualize the solution, see how it's going to interact with the user. And that's where we find a lot of the best critical feedback comes from engineering, marketing, or anybody else.

**Aakash Gupta** (00:30:00)

Do you find you're living outside of cloud design then a lot? You're getting this to generate the prompt and then giving it to Figma make?

**Pavneet Singh Ahluwalia** (00:30:07)

Yeah, the only reason I use Figma Make is because it's easy to share a Figma Make link and others can iterate on top of it. It's easy to click around. Cloud builds like HTML files, which it's hard to keep version tracking and stuff like that. Figma is just like more shareable. That's why we use Figma Make.

**Aakash Gupta** (00:30:23)

Makes sense. So how do our PRD and PR agents look?

**Pavneet Singh Ahluwalia** (00:30:28)

Yeah. So now it's asking me questions, right? So it's saying, hey, the evidence splits into two different directions. One is multi-tenant substrate coda bumps, and the other is dedicated conversion expansion. Which one do you want to go for? I actually want to go in a very specific direction, just looking at the feedback we got from customers. I want to say, hey, we should focus On increasing the attached storage volume sizes for tenants. Tenants here is basically a customer cluster, right? So tenants in a running cluster.

**Aakash Gupta** (00:31:10)

So here's where your domain expertise, your human judgment is coming in.

**Pavneet Singh Ahluwalia** (00:31:14)

Yeah, like it's not a substitute for me, but it really does two things. A, it speeds up the whole PRD writing, like it solves the blank page problem to a large extent, but it also catches a lot of things that I might not have thought of. Like I often find it's asking me questions that I might have missed if I'm not spending a lot of time thinking about the problem. So ignore Becca issues. I'm just giving it a sample to focus its energy and to reduce the scope so it's not trying to boil the ocean in the problem space.

**Aakash Gupta** (00:31:46)

So a 10 out of 10 that comes out of it, it's going to be kind of that very short document that accompanies a prototype. Yeah. If this all goes well.

**Pavneet Singh Ahluwalia** (00:31:55)

Yeah, so I actually did this and I have that PRD. If you want, I can show it to you what that looks like.

**Aakash Gupta** (00:32:01)

Yeah, let's take a look.

**Pavneet Singh Ahluwalia** (00:32:02)

So this is what the final output looks like, right? So first of all, it's telling, like, where's the evidence? It looked like we had 20 pilot tickets across 14 customers, right? So straight up, you know, there's evidence. And this is what it looks like. It first defines the customer and the business problem, like we talked about. The 20 confirmed customer issues, it's name dropping some customers just to give us a sense of which customers, right? Is it our top big customers? Is it like a long tail of customers? And then It gives you a sense of what is the actual pain, right? It seems like we cannot update this in the UI. And that's basically the ask. They just want to self-serve the volume resizing. And that's pretty obvious from the customer verbatims. And then you go into goals and non-goals. This is important for scope creep, which is the number one problem I feel like PMs and engineering faces.

**Pavneet Singh Ahluwalia** (00:32:52)

So it gives you some goals, like it's giving me a goal that, hey, if done well, this should basically handle over 90% of resized requests, right? It works in both directions, upwards and downwards, like scale up and scale down. Billing should adjust immediately. See, this is something I did not think of, actually. When somebody... Reduces the size or increases the size, we need to make sure that the billing matches up and they're not over or undercharged for it. And capacity block requests. What happens when we don't have enough capacity, right? If it's a fully self-serve experience, when do we actually need to get support involved? And then it defines the top goals as well. User stories so that, you know, whoever is reading this and when we are doing a discussion in engineering, everybody understands the key use cases. And then actually the proposal overview, right?

**Pavneet Singh Ahluwalia** (00:33:38)

It's giving me some API specs. It actually gives like a detailed API design as well. So we are going to add to our existing API some changes on how to basically allow for resizing. This is the user story, sort of, right? Like what are the different API specs and what is the API calls? And then UX as well. End-to-end user flow. Happy path. What are the steps that a user will follow?

**Aakash Gupta** (00:34:02)

So I feel like it always gets the headers right, but sometimes the devil is in the details. Is it nailing the details?

**Pavneet Singh Ahluwalia** (00:34:08)

So let's look at this one, right? So admin sets a new size in the console, API validates. This is some internal detail, actually. So maybe this part not necessarily needed in the user flow. This is actually internal detail. And then it shows the status. It shows that it's available and billing rate is updated. So it got the user journey right, but it bled some So it's still

**Aakash Gupta** (00:34:34)

going to need a little bit of editing. You can't just immediately take this and start sharing this with your colleagues.

**Pavneet Singh Ahluwalia** (00:34:41)

Yeah, absolutely. Actually, at the top, it says this is a draft one-pager PRD. It's not meant to go wide distribution for everyone. And that, again, kind of goes back to the process that we were talking about, where in this initial discovery and design phase, it's human in the loop. So the expectation is that the PM will go and make changes. So we've

**Aakash Gupta** (00:35:09)

got the repo, we've gotten to see it in action. We've got a little preview about an orchestrator agent. Charles, can you walk us through this? How do you get to see this bird's eye view at the top of the product ladder?

**Charles Zedlewski** (00:35:23)

The basic idea is each of the individual product people are sort of married up hand in glove with their corresponding engineering team. And Pavnik kind of gave you a good example of how that works where like he wants to be able to go pretty far into the definition and implementation for some of the things he works on. And the specific engineering team he works with has given him the kind of skills connected to their code base that he can go do that. From my vantage point, what I need to do is be able to get a check on where things sit in all kinds of different things that we're building as a company. And I don't want to have to build the equivalent of So I have this nice tool here called Orchestrator and you can see that essentially all the major repositories we have as a company for all of our products are represented here.

**Charles Zedlewski** (00:36:18)

So if you see, I'll give you kind of a quick So you can see here, we have the repo that PubNeed was just living in Tcloud, but you can see that it coexists along with many other repos. So for sake of argument, One of the other products we have we call model shaping, which is basically the ability to adapt the behaviors of open-weight models. And I can decide how I want to interrogate what's going on in that code base, what's going on in that product area. I can pick my harness. I can use either OpenCode, Claude, or Cursor. I can pick my model. So in this case, I tend to be a GLM OpenCode kind of guy. And I can ask some question like, What's the most recent model we have enabled or supervised? Supervised fine-tuning. So we basically have more than 30 models that you can adapt and fine-tune, but these are changing all the time.

**Charles Zedlewski** (00:37:24)

I don't wanna have to go understand the entire world of the product lead for model shaping. I just wanna understand what's going on in this one specific, to answer this one specific question. And you can see that essentially what we'll do in this case is we'll actually create a sandbox, we'll call in the repo, all this happening in the background. In a minute, it's gonna basically interrogate that portion of the code base It's going to go research what are the most recent changes and let me know what happened most recently. You can see it cogitating right now. Like the proverbial cooking show, I have like kind of a synopsized version of like the conclusion. And in this case, it looks like the answer is the last model that we enabled for supervised fine tuning is the new NVIDIA Nematron Super 120B model. So I can do this exercise essentially across any product, any portion of the code base for that product.

**Charles Zedlewski** (00:38:29)

And it's not just limited. Here I'm just asking questions. But if I also find some part of the product that annoys me and it's something small, I can actually generate a pull request from here as well.

**Aakash Gupta** (00:38:41)

Okay. So you're mainly living in the orchestrator, not inside Cloud Code and the team repo? Yeah.

**Charles Zedlewski** (00:38:46)

I use cloud code in the team repo for if there's some requirement I'm writing myself for some part of the code base, then I would do that. But if it's me shopping across like all the different products we have and it's like some small UX chain. Or things like this, then I would sooner use the Orchestrator because this is basically not just pointed at all the different repos we have as a company, but it's inheriting all of the skills and or MCP servers That are local to each of those repos. So I don't want to have to build all that into my local open code just to make one small change. It's a lot simpler to just use orchestrator. And I know it's going to have the latest, greatest skills in MTP servers for that portion of the code base.

**Aakash Gupta** (00:39:35)

Got it. So who are the other users of Orchestrator within the company? Who is this product exactly built for?

**Charles Zedlewski** (00:39:41)

It's sort of intended for casuals, right? So it's intended for, let's say, Pavne wants to investigate something Or let's say Nekaleen wants to make a suggestion on our infrastructure as a service. They don't want to build and replicate all of the specific skills and context native to that particular portion of the code base. It's a lot simpler to just look at just to use Orchestrator where everything is going to maintain server side.

**Aakash Gupta** (00:40:14)

Hmm. Okay. So this is like for whenever you're casually working, maybe like trying to learn something about another team, this is also creating that connectivity.

**Charles Zedlewski** (00:40:24)

Yeah. One of the things that we talked about as a team was like, like, like it goes back to this point about how much is shared and how much is individual. Right. And there was a point at which I thought, well, wouldn't it be great if everybody knew what everybody else was doing? And there was sort of like, we all had the same context and everybody else at all times. And in reality. Most people don't have a whole lot of motivation to want to understand all the depth and nuance of the context of somebody else's area. They want to know just about they need to get one single question answered or to get one single problem resolved. And they're really not interested in the rest. So we sort of set aside the idea that there is one big, broad, flat set of context that we're all going to swim in.

**Charles Zedlewski** (00:41:09)

And it's much more like a context hierarchy. And some of us belong all the way down to the bottom of the depths of that hierarchy. And some just want to traverse the top.

**Aakash Gupta** (00:41:20)

Fascinating. Okay. So if a team company watching this, they wanted to replicate what's being built in Orchestrator, how are they going to spin up their own version of this?

**Charles Zedlewski** (00:41:33)

From what we see in terms of our own customers, this is becoming increasingly common. I was at an AI conference in Paris the other week and I saw a digital They basically already built their equivalent of the same thing, where they have every portion of the codebase you want to change is all in one place. Everything can be spun up as a sandbox and generate its own unique pull request or its own questions. I think this set of tools is not that out of reach for most software development organizations. And this idea of like, we're all going to live in a multi-model, multi-harness world. And the main endeavor then is how do you organize shared context? That's kind of, I think, what everybody is starting to build. To give a more specific answer, Hassan, what was the total time invested, would you say, to build Orchestrator?

**Aakash Gupta** (00:42:45)

I would say a few weeks of work, maybe a month of work to build it, of engineering time. Yeah, and a lot of it was kind of just like trying to figure stuff out fairly early, trying to figure out the right architecture, the right tools to use, a lot of that stuff. But as Charles said, I think like this has kind of been replicated by a bunch of other companies. There's like a few open source versions of this as well that exists out there. So it's kind of easier than ever once you have the architecture. But yeah, for our team, it took a few weeks. So if we're just drafting the PRD for an internal orchestrator for yourself, what are the key things? It needs to hook into all of your code bases and your different repos. It needs to inherit all the active MCPs and skills from the different team repos.

**Charles Zedlewski** (00:43:30)

It needs a sandboxing mechanism because you're basically going to, essentially like each individual thing you're researching or each pull request you're going to propose, that all gets done in a sandbox environment. So you're basically cloning a fraction of the repo, right? The portion of the repo that's necessary. In the sandbox to generate that one pull request.

**Aakash Gupta** (00:43:50)

Got it.

**Charles Zedlewski** (00:43:51)

You also are going to need some form of a model gateway or router. So you notice I have a whole choice of models that I could use. So that's typically another piece of the puzzle. But as Hassan mentioned, every one of these components I've mentioned so far, either it's relatively quick to build, There are open source tools and libraries that let you do these things. And there's commercial shrink wrap software if you don't feel like doing either the previous two things.

**Aakash Gupta** (00:44:19)

Fascinating. So we're walking through the whole product development lifecycle. The last step, evaluating how these things are going live. Hassan, how are you guys doing agent evaluations? Great question. As you said, this is kind of the final step that we do. I'm going to share my screen. I'm going to go over this tool that our team built called Agent Evals. And just to give a little bit of context on Agent Evals, you know, I think the whole world is moving to this agent-centric way of doing things, right? You don't kind of manually write code anymore. And kind of it's moving up the stack with like, you just give your agents stuff to do. And so, you know, my team is called Developer Experience. I think Charles is This close to renaming it Agent Experience. And because it's something we're increasingly thinking more about and it's very, very top of mind, we've re-architected our docs in kind of this agent first way where it works very, very well for humans, obviously, but also for agents.

**Aakash Gupta** (00:45:17)

You actually on some pages on our docs, like when an agent is reading them, we'll inject something extra if we think it'll help the agent. We worked on it together, MCP Server. We worked on together, Skills. And so we're exploring all of these ways that we can make it as easy as possible for agents to use our product. And agent evals is kind of the tool that ties them all together or the tool where we can actually say like, okay, We're pretty confident in how this works. So I'm going to share my screen and we're going to go over this. Fantastic. Okay. So agent evals, there's a lot here, but agent evals is the tool we use kind of at the end of this product development life. We have the product, it's shipped, right? Some kind of some major feature or a product or a second version of the product.

**Aakash Gupta** (00:46:03)

And now we need to validate that it actually works well with agents. So what we do is I tend to work with a lot of the product managers in each of the And we write a series of tests of like the main, like here are the main ways that we think users will use a specific product. So let's actually take fine tuning as an example or we'll take, yeah, Let's take fine tuning as an example. So if I click on fine tuning, this is a prompt that we give for, this is one fine tuning task that we're testing. So here we're saying, hey, we gave it a data set and we said, hey, run a fine tuning job for this data set. And when it's done, spin up this new fine tune model As a dedicated endpoint and evaluate it, right? Where it's gonna send it some inference requests.

**Aakash Gupta** (00:46:47)

And then delete the endpoint when you're done, right? So we gave it, and this actually touches on a few of our different products. It touches on our fine tuning product and our inference product. And so some of these tasks are a little more simple. Some of them are a little more complex. But the point is that the most important part is to find a series of tasks and give it to this tool. And what we do, What we do actually has a very similar architecture to orchestrator, which we talked about. So what it'll do is it'll spin up a sandbox, it'll spin up right now cloud code, and it'll give it this prompt. It'll give it together API key, and then it gives it whatever it needs for the prompt, In this case, we gave it actually a dataset. And then it just watches Cloud Code do its work, right?

**Aakash Gupta** (00:47:27)

It's just, it lets us do its thing and then it evaluates it at the end. And for us, this is like the best test of like, can an agent actually do stuff in your product? We try to make sure, we try to make everything in our product We try to make it so that you can do everything in our product, for example, in our UI as a human, but also as an agent through our API or CLI or SDK. So in this case, it actually got it correct, but we go very, very deep here. A lot of different runs. Some of these runs are just using our docs as contacts. Some of them use our MCP server. Some of them use our skills. And we can click into every one of these and we can get a lot of information on the run, how it worked.

**Aakash Gupta** (00:48:08)

We can get some high-level info. We can get improvements, which this is one of the most important pieces of this. And this is something we see a lot, where we'll ship a feature, or we'll be in the validation stages of a feature, and we give it to agent evals, and then it's like, oh, well, I had trouble doing this thing, right? I wasn't able to, for example here, I said it wasn't able to discover what fine-tunable models we have, right? Obviously this is a big problem if it can't find this. And it said, hey, like it couldn't find a docs page listing currently fine-tunable models. And so we should do this. And so we make a ton of improvements to our docs based on this. In this case, actually what happened is we had a page that Listed all the fine-tunable models, but the agent actually couldn't find it.

**Aakash Gupta** (00:48:49)

We were able to go into the transcript. You can go to the transcript and you can see the full transcript of this agent and what it did, right? We gave it this initial prompt and you can see all of the different terms. We can see that the agent started exploring the repo. Started looking at the data set. It like did all of this stuff, right? Like the full transcript. And we looked at it and we saw like actually it had trouble finding that one page in the docs because it's not linked in So then we're like, okay, well, we'll just go submit a PR to our docs and add that page to our fine tuning quick start. So, um, the agent evals has been responsible for, for like dozens of like docs fixes that we've done. Um, and, and it's been really, really valuable to really understand like, uh, and get this bird's eye view from agents on like how good are agents at using this particular tool or this particular API that, that we just shipped.

**Charles Zedlewski** (00:49:41)

And Akash, like I just wanted to like add on, I mean, you think about any sizable feature or product that you'd build in the past and the idea about like, well, did you get the design right? Like, did it actually, you know, can the outside user, whether it's like someone technical, like a developer or non-technical, Be consistently successful using that feature. And think of how long you had to wait to validate that as a product person before. You have to wait till you did a bunch of user tests and then you're going to get a bunch of conflicting signal or you're going to have a bunch of developers evaluated and they're all going to say, well, I don't think this is sufficiently Pythonic or I don't like the way you did this syntactically. And so it's like, it's really hard to get Timely signal and it's really hard to get objective signal.

**Charles Zedlewski** (00:50:36)

And here essentially, at this point for a lot of our products, agents are already the majority user. And so the idea is that the nice part about that is now, did the feature work from a design point of view? This is something that we can validate immediately and continuously. So it's really powerful to sort of always know where you're at. And it's really powerful to have the confidence to know that whatever your documentation says your product is, you can be sure that it actually is that because essentially every few hours we have agents revalidating that. And across time, what we plan to do is keep expanding the range of harnesses and models that we do this for, because that's essentially the new bar for UX for the kind of products we build.

**Aakash Gupta** (00:51:27)

Okay. Very cool. So if your product isn't used by agents yet much, does this still have value? Is this able to kind of simulate what a human is like and should people still be setting this up?

**Charles Zedlewski** (00:51:42)

So in, in, For us, it is because our users are developers, and so they're going to use our SDK, and this is basically validating that there's valid, successful paths using our SDK. If we had a more GUI, web front-end intensive product, we would have to adapt this tool. To use more, you know, like a visual reasoning model that could actually do the click throughs and like interpret the screens and see whether or not that was like naturally intuitive to the model. So it could be extended to human centric examples. But for our case where agent use is already so popular, it works as is.

**Aakash Gupta** (00:52:27)

All right. So we've been able to cover front to back from customer research through to actually evaluating how agents would be using your feature. This is kind of the whole product development life cycle. I'm curious where this ends. We kind of drew the line here at create the PRs, create the prototype. Where does the line of product manager end and developer begin?

**Charles Zedlewski** (00:52:54)

I want to think how to best respond to that without just repeating what Pelni just said at the beginning of our whole thing. I think that the essence of... What the product person does versus the essence of what the engineer does, ironically, is probably not all that different than what it was before AI in the sense that the most valuable thing the product person can do is bring a unique insight about the market that's been well validated by lots of internal and external context. And that's essentially what you still saw Pavni do. And the essence of what an engineer does to add value to the company is to arrive at a design that is the most efficient way to meet a need. The essence of the engineer's job is You can thrive in a design that most efficiently satisfies a need and is also something that you can maintain and extend and contributes to the long-term architectural strength of the product.

**Charles Zedlewski** (00:54:11)

The essence of each thing I don't think is actually all that different today than it was before AI. What's different is the convenience with which the product person can reach into the engineering world and accomplish small and medium-sized tasks. And the inverse is true as well. The degree to which the engineer can reach into the product management process and answer their own questions. So just like it's possible for me to interrogate the code base and make small pull requests, it's just as possible for one of my colleagues in engineering To use that customer insights tool and do their own analysis and have their own standing query for whatever the customers have been asking for in the past month in their area. So it's sort of easier for each side to reach into each other's area to do small things. But in terms of what each person is supposed to contribute that brings their unique talents and perspectives, I think that's actually the same core as it's ever been.

**Aakash Gupta** (00:55:10)

That's amazing. So I've been preaching to people, get your PM OS, get your team OS, get your company OS. You guys just demonstrated and are actually living that reality. So you're at the very top of the AI adoption curve. And I heard a really interesting observation from Chema. He said, you know, our token costs are something like doubling every 70 days, but our actual engineering productivity is just up like 5%. When you look at it from a product lens on that, like how are your costs on AI growing? And are you seeing a tangible, like some sort of tangible productivity gain that you can point to from it?

**Charles Zedlewski** (00:55:51)

We never were in a place where we were doing story points or other kind of velocity measures, so I can't prove it on that level. But I would definitely say that our velocity has gained more than 5%. I find claims of 3x to be very suspicious. When you get a team of, let's say, a dozen engineers and a product manager, There's so much of building software, which is discovery, debate, kind of re-evaluation... Coordination. And a lot of these things don't get magically better with AI. So even if you compress the research and even if you compress the coding and the testing, I think that's worth a lot in terms of velocity. I don't know that I would say our experience has been that like 3x or some huge multiple like this is the case. And as far as expense goes, I think we went through the same surge that a lot of folks did.

**Charles Zedlewski** (00:56:56)

It was easier for us to mitigate because we can use our own open weight models and they're a lot less expensive. But the other part is, it goes back to this first point, which is, I think if you're focused on making teams collectively productive as opposed to yourself feeling individually productive by producing lots of output, I think it's unlikely that you wind up with these crazy token budgets of three times people's salaries or things like this. I don't know that we ever reached that type of peak.

**Aakash Gupta** (00:57:28)

I like how measured you guys were in selling the benefits of all of this, where none of it was overhyped, but we got to tactically see how it helped both individual ICPMs like both Neath and a product leader like yourself, Charles. All four of you guys, thank you so much for dropping so much insider knowledge about how together works.

**Charles Zedlewski** (00:57:51)

Thank you for having us.

**Aakash Gupta** (00:57:52)

I hope you guys enjoyed that episode as much as I did. They have been kind enough to literally open source the tools, the repo, the orchestrator, how they built this. So check the link in description below if you want to get your hands on how to get their I hope you learned as much from today's episode If you can do one thing that's totally free that would help the show, it would be to check that you're following on Apple and Spotify podcasts. Check that you've left ratings and reviews on those platforms. Check that you're subscribed on YouTube. Leave a like and a comment on this video. We're trying to make better and better podcasts. After two years, we think we've gotten something pretty good going. So let us know what we can do to make it even better, who else we should interview, and we will put on the best shows we possibly can.

**Aakash Gupta** (00:58:53)

Finally, don't forget my offer for the bundle. You get an entire year of my paid newsletter, plus my favorite AI tools, Bolt Up New, Airtable, Speechify, Descript, Magic Patterns, Linear, Dovetail, Arise, and Mobbin. That's $27,000 worth of value for just $150. So check that out at bundle.akashgu.com if it interests you, and I can't wait to share our next episode soon.
