---
title: "How Srini Raghavan helped $3.4B SaaS Giant Freshworks Embrace the AI PDLC"
subtitle: "+ Why he uses Grok models, and the future of the “Product Builder” role"
date: "2026-08-24"
host: "Aakash Gupta"
guests: ["Guest"]
speaker_names: "inferred"
substack_url: "https://www.news.aakashg.com/p/srini-raghavan-podcast"
youtube_url: "https://www.youtube.com/watch?v=0qNZVlW8IR4"
duration: "01:05:19"
word_count: 11690
source: "Substack episode transcript (aired audio)"
sponsors:
  - name: "Customer.io"
    url: "https://www.try.customer.io/paid/trial?utm_medium=ads&utm_source=sponsored&utm_campaign=q22026_productgrowthpod&utm_term=demand%20gen"
  - name: "Ariso"
    url: "https://ariso.ai/aakash"
---

**Sponsors:** This episode is brought to you by [Customer.io](https://www.try.customer.io/paid/trial?utm_medium=ads&utm_source=sponsored&utm_campaign=q22026_productgrowthpod&utm_term=demand%20gen) and [Ariso](https://ariso.ai/aakash).

# How Srini Raghavan helped $3.4B SaaS Giant Freshworks Embrace the AI PDLC

*+ Why he uses Grok models, and the future of the “Product Builder” role*

**Guest** (00:00:00)

You told me that you think these titles will all go away in a couple of years. I think these three different roles are going to be replaced by what I call a product builder.

**Aakash Gupta** (00:00:10)

Meet Srini Raghavan, CPO of the $2.8 billion employee experience giant Freshworks. He manages a team of over 200 people and they have completely

**Guest** (00:00:20)

adopted AI. The traditional linear handoff where product manager writes product requirements document and then it hands it over to user experience designer who then takes the product requirement documents, builds the prototyping Figma and then creates a wireframe from it and then hands it off to an engineer. This is a very linear process

**Aakash Gupta** (00:00:39)

and this is completely dead.

**Guest** (00:00:42)

Here's my employment registration error. I wish I could be making this money. I don't, but that's not my real life.

<!-- sponsor -->
**Aakash Gupta** (00:00:46)

I thought you just doxxed your salary. For your fellow CPOs out there who are running product teams that aren't where you're at now, what is the roadmap to transform your team into this new way of work? Before we get into today's show, please take a second to check that you're subscribed on YouTube and following on Apple and Spotify podcasts. If you want access to all of my favorite AI tools, I've gotten them to give you an entire year of their paid plans. Check out bundle.akashg.com for an entire year of Bolt.new, Airtable, Speechify, Descript, Magic Patterns, Linear, Dovetail, Arise, and Mobbin. And now into today's show. Look, we've had a lot of startup CPOs on the podcast, AI native CPOs on the podcast who are showing you how their teams build with AI. The difference with today's episode is you have the CPO of a public company.

<!-- sponsor -->
**Aakash Gupta** (00:01:47)

Freshworks went public in 2021. They're valued at $3.8 billion. They're known for their employee experience and customer service platform. They have over 70,000 customers. They are a giant of SaaS. How do you move a giant, which is serving enterprises, into the new way of building AI? Freshworks was known for a six-month release cycle. How do you go from a six-month release cycle to a two-week release cycle? Srini drops all of the knowledge today. And one of the coolest things about today's episode is he doesn't just talk about it. He actually shows you. So I hope you enjoy this episode as much as I did.

**Guest** (00:02:27)

Srini, welcome to the podcast. Thank you, Aakash. Great to be here.

**Aakash Gupta** (00:02:31)

You manage a team of over 200 people with titles like user experience researcher, designer, product manager. But you told me that you think these titles will all go away in a couple of years. Tell me more.

**Guest** (00:02:43)

Look, I think it's a matter of time before these titles existed in the past because of a reason. And the reason that these titles existed was because it was a linear handoff that was happening from a product manager to a user experience designer to an engineer building things. But now, by leveraging AI, each one can do all three things. Which is why I think these three different roles are going to be replaced by what I call as a product builder role. Where a single person can research the customer, spend more time talking to users, understand their pain points, and then build things and ship things. And that I think is what is going to happen. Probably it's already happening in some companies, in startups, but I think it will be much more widely prevalent in the very near future.

**Aakash Gupta** (00:03:37)

I love the bold take. So today, guys, we are going to walk you through this masterclass of how this product builder rule happens in three steps. We'll walk through the AI PDLC, the ex-AI agent that they created, and how it interacts with MCPs in Cloud Code. Srini, can you get us started with the AI PDLC?

**Guest** (00:03:55)

Yes. Let me show you something instead of talking about it. I'm going to show you how we are building software today. So I'm going to spend maybe about two minutes to sort of talk about the AI first versus the data first approach to building software. So there's a lot of noise out there that everybody is building software by leveraging AI. What you see on the left is the foundation for building the software is having an appropriate design system, an appropriate coding system, and a repository that can be leveraged across. So I call this the data-first approach versus the AI-first approach. And what the difference is mainly building the, what you see on the right is building the foundations that makes the AI first approach go faster. Not start with the AI first approach, but building the foundations. And I'm gonna show you how we built it.

**Guest** (00:04:54)

And then building on top of it, which makes things go a lot more faster. So here's the product development lifecycle ecosystem that we have at Freshworks today. This is pretty common across a lot of the software companies. There's discovery, there's design, planning, development, We have an AI agent that's helping in every step of this process. And that's what we call as the AI PDLC, AI Product Development Lifecycle. And we have a governed framework. We have an eval framework for it. And we have built something called what you see here on your bottom left is the prism. This is, we have our knowledge hub, which has the product knowledge and dependencies. And we have the context hub, which has the feature context that's passed across the different phases. And we have a central skills repository. We call it the AI builder artifacts, which is skills, rules, commands.

**Guest** (00:05:51)

Agents, all these are very specific to Freshworks because we are a billion dollar revenue company and 75,000 customers use our products and it touches almost 300 million end users. So that's a lot of stuff. Users that are using our software. So we need to make sure that whatever we build reaches those people and it's governed. So this is our life cycle of how we build software. Now today, I'm going to go deep on the first two things, which is the discovery aspect and the design aspect of it. I'll show you the other things briefly, but I'm going to focus mainly on the discovery and the design aspect of it. Where we have a product discovery agent and a design agent, and I'll show you how those things work. It all sort of starts and ends in cursor. So I was an engineer for 10 years before I went to the non-engineering parts of the job.

**Guest** (00:06:40)

I did multiple jobs. I was in professional services, I was an investment banker, I was in corporate strategy, and then I became a product leader. And during that course, I used to use an IDE to build software, but now After almost 14 years of not touching code, now I'm again spending a lot of time in cursors. So now I'm spending time building software. So we have built something called a PRD GD, which is used by the PMs to draft Product Requirements document and they also use it for spinning up the prototype and it lives inside Cursor. And you can also do the pull request from inside Cursor to actually build the thing that you have wrote the requirements for and done the design for. When you do this, then the research burden is there on the PMs. They spend a lot of times gathering evidence for functionality, comparative analysis, customer feedbacks, there's metrics and metrics come in different forms.

**Guest** (00:07:32)

How many people are using it? What are the feature requests that are submitted by our community? And then there's a dependency analysis. This is a lot of burden on the PMs. It's not just writing the PRD, but they have to get all this information and get it into the product requirements document. And this leaves very less time for strategic thinking. So the PM spend a lot more time on, call it operational work, rather than thinking strategically about what they need to build and what customers need. And that's exactly the problem that the PRD Genie has solved. It drafts 80% of the PRD almost instantly, and I'm going to show you this in action, and it's grounded in real data. It drafts real specs, and then it hunts for evidence. It gets evidence on how much are users asking for, what bugs does it solve, what are the functionality that we can do, and pickle the So what you see here is our data lake where we have all the usage metrics from 75,000 customers.

**Guest** (00:08:33)

And then it looks at the competitive benchmarks to see what problems are, how are the competitors doing it and how we can do it better than others. And then I call this the CPO check, It's an AI agent that reviews the document for strategic alignment, clarity, and what are the edge cases. These are the things I look for when I'm reviewing a PRD, but the AI agent does it automatically now. And finally, it sinks into action. It seamlessly plugs the rest of the AI PDLC process across all the teams. So these are the 12 steps. I call it the 12-phase specialized intelligence, from idea briefing to requirements to knowledge, competitive analysis, et cetera, et cetera. And I'm going to show you how we built an entire system To get this into action. These are some of the things, competitor analysis, customer feedback analysis, quantitative metrics. So it's not just the quality, customer analysis and competitive analysis is qualitative and this is quantitative metrics of showing what the usage data shows and what we should be doing.

**Guest** (00:09:30)

And finally, internal dependency analysis. You can imagine when it's a large company, there are dependencies on platform, there are dependencies on System, all the other things. So it also does the dependency mapping and analysis. And finally it does the automated visual prototyping. And so it goes from having a spec to getting a final screen. And finally it does the quality assurance. Now let me actually show you How this looks. And I'm going to show you this in Cursor. And why Cursor? Ah, very good question. The Cursor is an integrated development environment, which to me, I like Cursor for three reasons. Number one is I can get started and it's a no-code IDE, completely non-technical person can use it. So as opposed to the other IDEs that are out there in the market, which mostly are geared towards an engineer, This, a completely non-technical person can use it and they can get good at it.

**Guest** (00:10:24)

That's number one. Number two is, unless you pick and choose the models, like not everything needs a latest LLM model. You can pick and choose the models that you want and it'll perform based off of what needs to be done. Number three, it has connections to Figma and other third-party sources. Like I use, my favorite thing is to use the Figma MCP plugin, whereby it can read the Figma mockups that we create and it can create code from it. So these are the three reasons why I primarily like cursor as the development environment.

**Aakash Gupta** (00:10:56)

Nice.

**Guest** (00:10:57)

Here's a quick word from our sponsors.

**Aakash Gupta** (00:10:59)

I used to think I had a retention problem. Turns out I had a messaging problem. I was sending the same onboarding emails to every new user, whether they activated on day one or never logged in again. I had no idea who was slipping or why. Customer.io changed that. Every message I send is now based on what users actually do in the product. Someone hits a key activation They also have an MCP server, which means AI tools like Claude can see directly what's happening in your customer.io workspace. Your segments, your customer data, your attribution, all of it. So instead of explaining your business context every time you need help, Claude already knows it. Notion used Customer.io to personalize their onboarding and hit nearly 50% open rate, improved conversion by 6-7% with localized campaigns, and pushed open rates up another 20% through A-B testing. The idea is simple.

**Aakash Gupta** (00:12:04)

Customer.io helps you deliver more impact from every message you send. If you're a PM or founder and your onboarding is still one size fits all, try Customer.io at Customer.io. If you've worked at any company bigger than 30 people, you know this one. The CEO sets strategy. Every time it reaches the people actually doing the work, it goes through three or four layers of translation. Half of it gets lost and nobody finds out until the quarter is over. That's the problem Mariso is built for. It's an AI operating partner for every manager and team. It connects to where work actually happens. The meetings, the messages, the docs, and it turns all

**Guest** (00:12:36)

that fragmented activity into a clear picture of execution.

**Aakash Gupta** (00:12:40)

Managers get real coaching grounded in their team's actual work, not generic advice. Teams stay aligned with strategy as it changes, not as it was last quarter. And leaders see where execution is drifting in weeks. Not in the postmortem. One shared memory for the whole org. Everyone finally working from the same picture. If you lead a team, check out ariso.ai slash akash. That's A-R-I-S-O dot A-I slash

**Guest** (00:13:02)

A-A-K-A-S-A. So this is the cursor environment. And what you see here is a Freshworks AI PDLC demo. So which means we have created a project here. We have the artifacts. I'm going to initiate this. So now I have a problem. Let me describe the problem I'm trying to solve. What I'm trying to solve is we launched a AI agent studio for our customer experience product called Freshdesk back in November of 2025. And we recently launched our EX AI Agent Studio, which is seen as CX, but for employee experience. And we did that within like four months. And when we launched the product, one of the functionality that was missing is the performance analysis. So think about it as, you know, a lot of people, I guess when I'm working in different companies, imagine AI agent is answering questions about, hey, my Zoom is not working. What do I do?

**Guest** (00:13:54)

Or I need to get access to cursor. Or I need to request my time off. Like all these things, an AI agent is answering questions. But as it's answering questions, most of it will answer. Some of it won't answer. Imagine you are the IT admin and you want to see how the AI agent is performing. That's what it's called as performance analysis of how the AI agent is performing. That functionality we need to build. So we built it for CX. We are going to have a fast follow for EX. And now I need to build it. So that's the project that I'm going to show you. So I'm going to start with initializing this project. Okay. So I initiated it and it's 12 step process. Remember what I just told you earlier, it's a 12 step process in terms of building things and what it's asking for to initialize the AI PDLC.

**Guest** (00:14:41)

It's asking for the business unit, Epic ID, feature, team, All this other information that it needs. And I'm going to give the information that it's asking for. So the business unit here is EX, which is employee experience. I'm giving it the Epic ID and the team, et cetera. So once I give this information, it's going to run. It's going to plan its next moves. And it's now setting up an artifact demo so that it can So this is going to take some time. In the interest of time, I'm going to just show you how this looks like. So instead of doing all 12 steps, which will probably take another 30 minutes, I'm going to shortcut it. And I'm going to say that I did this earlier. So I'm going to say that I'm staging what I was able to do in cursor earlier. So if one and two, it can ask me questions and this stuff.

**Guest** (00:15:41)

Otherwise, it'll just keep asking questions. So I'm just going to say that, look, don't keep asking me questions. Just proceed to the next step. Okay. Now it's going to ask Okay, let's give it, this should not take too long. It's probably take like 30 seconds. What it's doing now, it's like a normal developer, right? Think of it like a developer. It's creating the directories and it's creating the files that it needs. It's initiating everything. It's creating the scaffolding that's needed to build it. And now it's completed it. So that didn't take like, it took like 15 seconds. Now I'm actually going to describe the problem statement that I said earlier. So it's a long one, but essentially what it is, as you can see, the problem here is EXAI Agent Studio, they don't have any unified view of how their AI agent performs across the employee channels.

**Guest** (00:16:34)

We already have that for EXAI Agent Studio, and that's what we want to build. Users are IT and HR admins, IT manager, or HR business partners. Think of a CIO or a CHRO or a Service Desk Lead. Why now? It's because we just launched the EXAI agents and customers are starting to use it and they want this functionality. And I said, look, you don't have to reinvent the wheel. There's always something like this that exists for CX. So you can pretty much take what it is and customize it. In employee experience, people experience it through Microsoft Teams, Slack, etc. For customer experience, it's not data. So there are some nuances that have been added here. So I've given it this how it needs to ideate. Now it's going to go ahead and start looking at the problem and come back with some questions that it has.

**Guest** (00:17:25)

Think about it as a product manager. When somebody tells you, hey, go build a performance dashboard for an agent studio, As a PM, you would want to ask some clarifying questions on what exactly is needed, which is essentially what the AI agent is thinking and saying, okay, what are the things that I need to understand in order for me to create a very comprehensive product requirements document and a design mock-up that can be used? So it's now planning for those things. And all these... So these commands have been given as part of the init process that I told you earlier. So these commands have been done and now it has come back with the questions. Look at some of these questions. It's asking what a logical question would be. How deep should the analytics drill down go? And where do ticket level details live? What is the primary persona score workflow?

**Guest** (00:18:18)

What does success metrics look like in six months? Et cetera, et cetera, right? And these are all domain specific questions, which ITSM process framing, service catalog, all these are things that an IT admin would understand. So it's asking all the relevant questions. So it understands the domain, which is what I said earlier when I started, which is having the appropriate data is the basis for building faster using it. Now I'm going to give it answers. Here are the answers. So I said, these are the things that you need. Analytics deal-down should be at this level, agent, topic, subtopic level, and the owner is IT or HR admin, and the landing view should be performance overview. It should create Sankey charts for better visualization. So I'm going to give it the instructions. And it comes back with sort of asking questions, et cetera. What do you think, Aakash, so far?

**Aakash Gupta** (00:19:08)

This is the first time anybody has used the Grok family of models. And I think since Grok 4.5, you get really good performance really fast. Is that why you chose it? That's right.

**Guest** (00:19:19)

I'm increasingly, I used to use Cloud Opus 4.6. And I'll still use it. And they've come out 4.0, 4.8 right now. But Grok seems to be working really well. It's really, really fast. I mean, nothing took more than like 10, 15 seconds, as you could see.

**Aakash Gupta** (00:19:34)

Yeah, I mainly do Fable and a little bit of GPT 5.6. So watching this go like 10 times faster is blowing my mind.

**Guest** (00:19:44)

Let me actually show you while this is running, this is going to take a few seconds. Let me show you something that I already have created. So these are the 12 steps. As I told you, the steps are, let me just walk you through the steps that happened here. What happened here is, it's a lot of stuff. It's first, when I answered, it started gathering the knowledge. It started gathering knowledge of epics, of how the analytics should be, and it gathered the Analytics, how the analytics screens are laid out right now. Then it sort of cross-checked with the competitor analysis. How are competitors doing? Like GSM is Atlassian. So it's now, what are they doing? Just looking at how they are doing things. And it sort of flagged some things for review just to confirm. And then it sort of did the market and competitor research.

**Guest** (00:20:32)

That's stage four. Stage five, we saw a voice of the customer. What are the customers saying? What is the feedback we heard from customers? Then metrics. These metrics, as you can see, these metrics are coming from Baikal. Baikal is our Databricks data lake, which has all the usage data. So let me just show you how it looks. As you can see, here's the hypothesis. What it did, it literally wrote SQL queries to query the Baikal data lake. And you can see, Here, it wrote a bunch of these SQL queries and it defined what metrics are needed and it extracted the metrics. And finally, it gave the data. What are the data gaps? It identified what are the data gaps that are needed and it came up with what data we need.

**Aakash Gupta** (00:21:15)

So you can see a lot of stages

**Guest** (00:21:17)

that have been passed. So when I said everything is grounded in data, what I meant by that is different companies have different ways of writing software, like PRD, what are the steps in the PRD? And what is the amount of qualitative data versus quantitative data that you use? And every company is different and every project is different. This particular one, we have this 12 step process. As you can see on the right side, these are your markdown files. You see the idea brief, requirements, knowledge gathering, all this stuff are the different stages that the AI agent just went through to create. And this is the final checklist. They call it the CPO review. They really like me in the product management team, which is why I think they called it CPU review. So the agent studio performance dashboard, they sort of run through the CPU review, step one, checker, self-administered, final approval.

**Guest** (00:22:12)

So these are all the things that a normal Product Manager would go through. They would have to write all this. Imagine it would take days and days to do this. The agent just did this in a matter of seconds, not even minutes. So you can see here, going back to this, it's completed all the steps. So you're just three to 12, it's already completed. And that's what I just showed you. Now that it has completed these steps, The next thing is to go look at how the PRD looks like. Ultimately, that's the outcome. So you can see here, it's created a PRD. This is the markdown file. This is the PRD markdown file. Let me make this bigger. So, let's look at what this PRD looks like. This is the PRD for Agent Studio Performance Dashboard. And it has, there is a major blind spot. It's sort of figuring out that EX, Employee Experience, has something called Service Catalog, which is different from what the CX product had.

**Guest** (00:23:13)

So it has considered that and it has accounted for it. It gives you the problem statement, what are the goals, what scope, in scope, out of scope. And then it shows you who are the users. Service desk lead, IT manager, etc. And then this sort of lays out what the solution is. Then it sort of lays out the market and customer evidence. What did our customers want when they were using the product? And how does the landscape look like? And it sort of... It's sort of the important part, quantitative evidence. It sort of shows, this is what I said by code, which is our data lake built on Databricks. It shows you how many catalog requests we have, how many ITSM accounts we have, like, and by region, it sort of said, okay, what are the things that quantitatively are needed in order for us to build the capability?

**Guest** (00:23:57)

And then it sort of built the user stories. You know, user stories which are positive scenarios and negative scenarios. It built a bunch of user stories. You can see a ton of user stories that it's built. Almost 10 user, eight user stories. And then it sort of built the requirements. Here are the functional requirements that it built, non-functional requirements. And these are things that we've been doing for the last seven or eight years when we were building software. But it was done in a very manual way. Now everything is automated. It also has the recommendations on pricing and packaging, what's the rollout plan. It came out with all these things. Now this is the PRD that we can take. So now the PRD is done. Now what do you do? Now what do you do is to build the actual mockup, right?

**Aakash Gupta** (00:24:42)

The worry I always have with like these AI generated PRDs is, you know, for metrics, just as an example, we're looking at the quantitative information. There's a million definitions of a metric. Did it really pull the right definition? Did it look at the right thing? We looked at how it was detangling experience you had in one product versus the other. Does it really have the latest version of what's live on the internet or does it have what's the latest based on Jira? So this is where the initialization process is very handy. So when we started this, when you use

**Guest** (00:25:22)

AI for building completely new things. Like think of Lovable or Replit or any of your favorite tools. It's very easy to use AI or even Figma Make for that matter. It's very easy to build new things from scratch because there's no precedence. There's no 75,000 customers that are using the product. With this, that's why it's important to have the appropriate references to what it needs to use. That's what the initialization process does. When it created these markdown files, you will see that in the markdown files, it specifically tells you which version that it referenced and why did it reference that. So there are specific instructions that are given as part of the AI PDLC process. So it's not completely automated. The way I would describe it is, AI is not running completely on autopilot. It's actually a copilot. There is still value for the product manager.

**Guest** (00:26:15)

If the product manager is doing it for the product manager to do it, if the engineer is doing it, the engineer should be doing it. So the value sort of shifts from doing operational work to judgment. Which version should I give? And how should I prompt the AI to do things faster? So going faster doesn't mean you sacrifice quality. And the way to do this of not sacrificing quality is to ground it on things that it needs to reference so that it doesn't help. You can't afford AI to hallucinate in building software. It's just not acceptable. Because then 75,000 customers are going to get affected. Of course, there are quality checks in place. There are checks and balances that we put in place. But the important thing is to ground AI on the things that it needs to know.

**Aakash Gupta** (00:26:56)

Got it. Now let's see that prototype. How do we go from document to visual?

**Guest** (00:27:01)

Yes. Let me show you the prototype. So let me start with... The Figma make. Well, let me start with the same as how we started with Figma, where we had a Freshworks init process. You see here that we have the fresh service starter and we have due Due is our design system. And Fresh Service is the, think of it like a scaffolding. We have two main products, Fresh Service and Fresh Desk. Fresh Service is the scaffolding in which all the functionality that the users see is inside the scaffolding. So I'm going to start with this scaffolding of Fresh Service because the functionality that we are trying to build right now, the performance dashboard, is inside the Fresh Service scaffolding. So I'm preloading the fresh service scaffolding so that when I create the prototype using the PRD that I created earlier, that the scaffold, we don't start with a blank canvas.

**Guest** (00:28:01)

We start with the canvas that's already used by 75,000 customers. And this is the scaffolding. When I say scaffolding, what I mean is this is literally the screen that, you know, half a million of our user base sees when they log in. Now, this is the ticket screen and this is the setting screen. These are all the buttons and it has the onboarding screen. This is the template that all of our users see today. And what I'm going to do with this is I'm going to say that using this Fresh Service Starter Kit, Build the analyze section from the PRD. So I'm going to go back to cursor, take the PRD that I had and paste it into Figma make here. Okay. It's pasted it as a link. As you can see, I'm going to tell it to plan. Ah, let me actually go here where I've already started.

**Guest** (00:29:00)

So, because it's going to take some time. So what I did here is I gave it the PRD and I said, using this fresh Service starter as the shell, build the analyze section. And it started reasoning it, and it has started building it. How much of the analyze section should I build? And now it's asking questions. All eight modules, P0 modules, overview, I'm going to say all eight. So now it's going to start. You will see that it's actually starting to build all the eight modules, the different modules. Remember the eight use cases that I just showed you in cursor? So those are the same use cases. It's calling each of those as modules and it's going to start building all the eight modules in the screen, which is what you're going to see.

**Aakash Gupta** (00:29:43)

So is Figma Make your preferred prototyping tool because it has access to your design system and you can easily bring it into Figma files? Or is there any other reason?

**Guest** (00:29:51)

So two reasons. One is what you just said. It has our design system, which is our dual system. But we have built our design system into Cloud as well. As many of your listeners might know, Cloud has Cloud Design where you can also feed in your design system.

<!-- sponsor -->
**Aakash Gupta** (00:30:07)

Quick thought experiment for you. Is there anything in this video you should be trying on your own? If there is, try it, take a screenshot, post it on LinkedIn or X, and tag me. I'd love to see what you're learning. Now a quick word from our sponsors before we get into the back half of the pod.

**Guest** (00:30:22)

Are you looking to up your AI product management chops?

**Aakash Gupta** (00:30:26)

I highly recommend the AI product management certification by product faculty. It has a 4.7 with 1,249 reviews on Maven for a reason. I myself took the course back in 2014 And it was awesome. Since then, they have upgraded it. So now you get to learn from product leaders at OpenAI and Anthropic. On top of that, Pavel Hearn, author of the Product Compass, leads the Build Labs. So you will go from theoretical knowledge about It's going to help you identify AI leverage opportunities. It's going to help you design trustworthy AI experiences. It's going to help you systematically optimize outputs for accuracy and relevance, build rigorous evaluations, So do check it out with my link in the description. They have been one of my longest sponsors for a reason. I trust this product and I think you should consider the cohort. I want to take a second to talk to you about the fourth cohort of LAN PM Job.

**Aakash Gupta** (00:31:33)

I trained 30 students in cohort one, 50 students in cohort two, and 75 students in cohort three. And I am bringing back the program for cohort four. It starts in August and it lasts You're going to have intense sessions, a Monday morning session where I go over your resume, behavioral interviews, LinkedIn. On top of that, Bart Jaworski is going to be teaching you the PM fundamentals in 2026, how to write AI PRDs, how to AI prototype with clients. So it is a full package. It is three courses in one for one low fee. So join at landpmjob.com. Every growth team has a funnel they should be watching more closely. Usually it's checkout. Amplitude custom agents will watch that funnel for you on the schedule you set. Let me show you. You start by describing the job. Watch my checkout drop off. The agent builder will ask a few questions to shape it and then the agent connectors plug it into your stack.

**Aakash Gupta** (00:32:49)

That part matters. The agent reads the PRD, the tickets, the team conversations, so its analysis actually carries the full context of what's happened. From there, it monitors the funnel on a schedule, and when it spots a problem, Right here, it files the linear ticket itself. The loop between knowing and doing closes on its own. That's the shift. Set up the agent once and it runs the work. Custom agents are free for all Amplitude customers in open beta right now. There's a library of pre-built agents too, including the exact checkout drop-off investigator. Start at Amplitude.com slash AI dash agents. The agent library is linked right there.

**Guest** (00:33:30)

So number two reason is a lot of our user experience designers, a lot of our product managers are very familiar with Figma. And Figma also lets you connect with other external data sources like cursor and other places. And so it makes it easier. From an adoption standpoint, when you are changing The ethos of how software is built, you don't want to change too much of the tools that they are using. And the tools usage can evolve over time. Now I see a lot of our PMs and user experience people actually using Cloud Design and Figma, and this evolves. You know, we'll be sitting here 12 months from now and maybe everybody will be inside Clark. Just the current best. Got it. So in this one, this is going to take some time. I'm going to show you how this actually looks like. So this is a fully built out design.

**Guest** (00:34:19)

It's going to take at least four or five minutes. So I already did this. So I'm going to show it for you. And I'm going to show you that there is actually a bunch of back and forth that I did. So it's not straightforward that you just give it the design. So here it said, do design components. Then it asked me some questions. I responded and it actually didn't get it right the first time. It didn't use, it had a couple of places where it was not using the due system. So I had to tell, I had to, so the judgment is still important. So you can't just take what AI does and say that this is what it is. So I had to say that there are some specific components that it has to use and I had to give it references to it. Then it changed everything.

**Guest** (00:35:00)

Finally, it came back. And then I realized that this design does not work in narrow monitors. So I said, you know, people use real users. Some of them have wide monitors like the one I'm using now, and some have narrow monitors, some have small screens. So, coding and business knowledge and experience of writing product requirements was important in the past, but now judgment is very important. A really experienced designer would know that, hey, it needs to work in different screens. And that's why understanding the end users. So that's why I said, okay, it has to work in narrow monitors. Then it responded to that. The Sankey chart, Sankey chart is this cool thing that you see here. For those of you that don't know, This thing that you see here is called a Sankey Chart. Sankey Chart shows you what percentage of topics are based on feature requests, what is software application errors, like that.

**Guest** (00:35:58)

So this is the Sankey Chart, and the Sankey Chart was not showing up, so I had to fix that. So these are all the things that I did, and finally it came up with... So this is actually the working product. You can see that this is a prototype of what the Analyze and Performance Task Force should look like. And this is now a completely built out mock-up that Figma, Figma Make, essentially the agent running within Figma Make, has built it for us.

**Aakash Gupta** (00:36:25)

And the PM applies their judgment really in finalizing the PRD, if there's any mysterious that it's wrong, in iterating here on the design, and then I'm keen to see what happens on the spinal step.

**Guest** (00:36:36)

That's right, that's exactly right. What I just showed you was how we built the functionality into, how we use the AI PDLC to build the core functionality of performance dashboard in Agent Studio. Okay, now I'm going to show you how the actual Agent Studio itself looks like. And this is the Agent Studio that we released maybe two months back. And think of this Agent Studio as clock. Claw is used by millions of people around the globe to get a lot of things done. People summarize things, people brainstorm on things. But what the agent studio is meant for is meant for two specific things. The specific things are to get when an employee joins a company and they need help with their IT issues or HR related issues, or they want to provision new software, et cetera, how a company can build very domain specific agents in IT and HR to serve their internal employees in a very seamless way.

**Guest** (00:37:40)

And most employees are either in Slack or Teams or they are in support portal to access their needs. And that's what the Agent Studio does. Now let me show you the actual Agent Studio itself. So this is our Agent Studio. You can see what we have here is AI agents. So this is what we call as Agent Studio. This is what I have logged into right now is fresh service, which is used by millions of users. And here is the Agent Studio, which is inbuilt into the interface that they are already used to. And we have AI agents here. And what the AI agents do It helps, you can see here, IT agents, HR agents, and some companies actually prefer to have IT and HR together. And these are the pre-built AI agents. And you'll see the libraries here. When I go to AI agents, these are the pre-built IT and HR agents.

**Guest** (00:38:29)

Now I'll show you the workflows. Think of workflows as things that are building blocks. So for example, there is a workflow for creating an incident inside PagerDuty. Imagine your service goes down and you want to create an incident inside PagerDuty. That's the incident one. And here there is a password reset. If you want to reset your password, most companies have either Okta or Azure. Here's the password reset in Okta. Here's the password reset in Azure AD. These are pre-built workflows that come out of the box. The way we have come up with this is we looked at 80% of our customers. What are the most often used workflows? And we built their workflows. Despite that, a lot of our customers actually built their own workflows. Look at locked computer. If some computer is locked, Jamf is used for unlocking. And there's a bunch of other workflows that a lot of our customers have built.

**Guest** (00:39:21)

Then the next one that I want to show you is the knowledge. Here's the knowledge. If I go to one of the existing AI agents, let me look at this IT and HR agent. So think of knowledge as what feeds the AI agent. So these AI agents cannot hallucinate, which means they need to have guardrails and they need to be governed. And one of the ways in which we make sure that the agents don't hallucinate and they're governed inside the enterprise data is by giving it Data to train. So for example, in this case, and that's what we call as knowledge. And knowledge can come in terms of URLs. So in this case, we have fed the Microsoft 365 help, support help, and it ingested all the things related to Microsoft Office 365 so that people don't have to waste time searching for things. They can just get answers.

**Guest** (00:40:10)

And second one is policy. For example, how to... How to do the withholding form for W-4. So employees, when they join, they want the W-4 form and they want to say my single or married or how my tax withholding should be. We have actually documented that in what we call a standard operating procedure and that's the document that exists here. There's a bunch of solution articles that people create. And in different categories, whether related to IT, Hardware, HR. And then finally, the apps. So not all the knowledge has to live within the agent studio. There is knowledge that exists most often in third party apps. Enterprises tend to store their data in Google. So we have a connector to Google or SharePoint. We have a search connector or Confluence. A lot of the knowledge can decide there. So you can connect your apps in your companies to fetch the knowledge from third-party sources outside of fresh service.

**Guest** (00:41:03)

So Google, SharePoint, Confluence, etc. So that's knowledge. Then I'm going to show you something very specific, which is a service catalog. Think of a service catalog as a list of things that you can have to get information. For example, here is an example of a fresh service inside our company. And if I want to request a service, Think of a service as, hey, I need access to Slack or I need access to information verification. It's in here. And there are some collaboration tools if I want to have access to Zoom or Box. So IT, this is somewhat of an IT jargon where the IT department that the CIO's department maintains a list of all the services that are offered Inside, like for example, HR applications. They have a bunch of HR applications here and software installer. So they have Adobe. Think of it as the approved software, things that an employee can get.

**Guest** (00:41:56)

So they cannot randomly ask for things. They have to ask within the service catalog. That's what this is. And similarly, there are some instructions that you can give to the AI agent. You know, what is the business context? What do we do? Like Freshworks as a company, we use this. We have 5,000 people and we all use this. So we can give them what is Freshworks? What is his business? What do we do? And we can give some custom instructions as well. If we want to, you know, some of the financial services companies, they probably don't want PII data to be shared. Like those kinds of instructions that you can give. And then there's configurations, you know, there's multilingual support. You know, people are spread over in different countries and sometimes the AI agent is asked questions in English or Spanish or German, etc. So you can support multiple different languages here and how it needs to act.

**Guest** (00:42:41)

That's conversation behavior. So bottom line, you can customize the AI agent to behave and act in the way that you prefer. And finally, you can test the agent here once you build the agent. So primarily, all these screens are used by an IT admin to build an AI agent because they know their users really well. And before they launch it, they can test it. And here's some tests that they can do. And finally, they can deploy it. They can deploy it within a support portal or Mostly what we find is our customers deployed within Slack or Microsoft team because that's where most of the users are. And what I'm going to show you how the Slack, so we use Slack. So I'm going to show you a demo of Slack and how once an agent is configured, how does it, Respond to questions in Slack. All right.

**Guest** (00:43:28)

So now let me go to Slack and show you how the agent is actually doing. So what we call this is what we have done now is created an IT and HR agent. We call it hire to retire, which means from the time somebody comes in to retire, these are the things that they can do. So this is how AI agent can help them in the different phases where they need help. So imagine this is Srini. Slack. Well, I don't even have access to Slack. So I assume that I have requested access to Slack and Slack is here and it has already installed Slack. It uses Jamf. Now I have Slack. Then what I'm going to do is I have some questions regarding my health insurance policy. And previously what used to happen was I had to email the HR and somebody in HR will say, hey, contact this person or that person.

**Guest** (00:44:28)

And now I don't have to do that. Here is a, I call this the concierge, the live IT HR. This is my private channel. And I can use this to ask questions privately. So I can say here, what are the mental health benefits offered as part of my insurance policy? If I'm the kind of person that wants a private answer, then I can ask this here. Or in some instances, HR might actually say, hey, this question might help others. So I can ask it in a public channel. So this is HR help. HR help is something where people can go to ask questions about HR related things. So here it's saying insurance policy includes several mental health benefits and it gave me a bunch of benefits that I have. And it's also showing the source. The source is actually a document. So if you remember, I showed you earlier how the HR team can actually put a solutions article.

**Guest** (00:45:21)

So it's coming from one of the solution articles. Same thing happened in my private conversation as well. It gave me the same response. So it really depends. It's all the customer preferences. Some customers want a central channel or some customers want a private. So you can achieve both the things from here. Then I can say, Well, what about forms? Used to be that when I needed a form, I had to, like W4 form, I had to either go to some archaic website, which nobody remembers, or again, even an HR. So here, I'm just asking a question to my AI agent saying, hey, can I get a blank W4 tax form? And it comes back and boom, there's the W4 tax form. You can see here it shows, here's the thing and I can access the form directly from Slack, right? So that's the tax form. So I'll give you a couple more examples to show you the power of this.

**Guest** (00:46:17)

I want to generate, let's say I need a employment verification letter. I just join, you know, my W4 form is taken care of and I want to apply for a loan. So I'm buying a house. I'm applying for a mortgage. So I'm going to ask it for an employment verification letter. So remember how it used to be when you needed an employment verification letter, you had to either email your HR or you had to jump through hoops to get this. Now I'm just going to ask the question here. I need an official employment verification letter generated for my bank. Let's see what it does. Now remember, this is very personal to me. And it needs to know exactly. So it's asking for details. It's asking for why do I need this? What's the address? What's the purpose of the letter? Right? These are all very valid questions.

**Guest** (00:47:13)

And I'm going to give it answers. This is the organization name, Acme Company. Here's the address. And the purpose of the letter is that I'm applying for home mortgage. So I'm giving you the information. So remember this used to take multiple emails or potentially even a phone call conversation or going to an HR department and sitting down with someone and spending 30 minutes explaining to them why it is. Now it's verifying the information. I'm saying, yes, all this looks good. Now we'll go to work and it has to generate a employment verification letter. There you go. One moment. Okay. There's my employment verification letter. See this in Slack. Here's my employment registration error. I wish I could be making this money. I don't, but that's where I could do this.

**Aakash Gupta** (00:47:58)

That's not very alive. I thought you just doxxed your salary. I joined way before 2025. So there you go.

**Guest** (00:48:08)

But you see how it is, right? The AI agent is helping. It's not about the power of AI agent, but imagine as an employee, look, all of you must have joined companies where it took hoops. You need to know someone that knows someone to get work done. You know how it is. Now you don't. You can just literally go to this AI agent and AI agent is going to help you with day-to-day tasks. So what we have heard from 20,000 odd customers that we have for our fresh service is it significantly improves something We call experience. So people used to have SLAs, which is service level experience. Now there is experience level agreements, which is how satisfied am I as an employee? Customer satisfaction matters. People talk about customer satisfaction, but the employee satisfaction is also very, very important. I would actually argue that it's way more important because if you have happy employees, which will ultimately result in happy customers.

**Guest** (00:49:02)

So that's the power of AI Agent Studio for you. Look, this took five minutes. I was able to show you how to set up an agent and how easy it is to set up an agent in our Agent Studio and how easy it is to use from inside Slack.

**Aakash Gupta** (00:49:16)

Amazing. How do MCPs and using this with cloud come

**Guest** (00:49:20)

into the picture? Okay, that's the last bit. Let me show you how the cloud, a lot of our customers actually use cloud to connect to a fresh service. So first of all, we launch fresh service. We launched a cloud connector. So let me actually show you, let me log into cloud right now. Let me share cloud. All right. So I'm going to open a new chat. And this is already connected. This is my Cloud. I have connected it to Fresh Service MCP. So think of this as a company that uses Cloud to query data from Fresh Service and get information and resolve things on the fly from Cloud. So I'm going to ask it some questions. I'm going to say, hey, fetch all the tickets with Windows 11 rate ratios reported in the last 60 days. And generate a visual report with root cause analysis. If people were to do this today, they actually jump through three steps and there's like three people involved because somebody has to fetch the data, somebody has to create a report, and then somebody has to look at the report and say, okay, what caused it?

**Guest** (00:50:21)

Root cause analysis and all of that. Now it's just a single prompt. I'm going to give it a single prompt. It's going to figure out, it's going to take a couple of minutes. So it says, this is a FreshBooks instance. By the way, by talking of governance and security, it is governed, which means none of this data leaves outside our environment. So now what it's doing is it's looking at the data. I already have a pre-baked thing here. You see, it's the same thing. I gave it the same command and it created a beautiful report. You see here, this is the report. What you see on the right is a Windows 11 update regression. What it said is there were 12 tickets across 60 days. There are two separate rollouts that happened. So Windows 11 patch happened and that resulted in the tickets getting created. And you can see that the shape of the incident July 10th and 13th, more so 13th is when a lot of the issues happened.

**Guest** (00:51:11)

Six incidents happened on 13th. So clearly some Windows 11 patch was applied and it shows you the root cause analysis. The two big things are Current driver regression, so some driver was applied, which sort of made it blue screens to appear. And there's a patch that was applied, and the install hangs meet progress, et cetera. And it also gives you the reference of all the tickets. Here's the ticket, here's the cluster it belongs to, when it was created, what's the status of the ticket, has anybody responded to it or not, and what are the actions to take. So it actually gave me more than what I asked for. I just asked for what is the root cause analysis. What it showed me is actually the recommended actions. Reply to tickets at the pilot ring before the fleet-wide rollout. Like this is Claude being way more proactive in doing things than just being a passive health test person that has to wait to take response.

**Guest** (00:52:06)

Now, what I'm going to do is, and I think the live demo that I had should have come back now. Here's what it is. Well, it's still working. But I already did this. So what I asked next is, help me answer these tickets with relevant response by searching the Knowledge Base articles available. So it went back into, used the MCP, Fresh Service MCP, went back into Fresh Service, got the KB articles, and that's how it said, what do I do when the system freeze happens? And this is like ticket number 158, and it says, random freezing after Windows 7 update is usually caused by background re-indexing and driver optimization. As is the case with most problems with Windows, it said restart the system. How many times have you heard that? And it gave solutions for each one of these things, system freezing, windows lagging, et cetera, et cetera.

**Guest** (00:52:59)

Then I said, okay, there's a bunch of these 12 tickets. There's no way that I want to do it one at a time. It actually suggested, do you want me to send the And I said, okay, great. Go ahead and send these replies to the tickets. And it actually sent the replies to all these tickets. I'll show you how the ticket responses were sent. And it's actually logged in for service as well that these tickets have been now answered. See, this is the power of MCP where an IT agent now Remember how I started it. If I'm an IT agent, I'm spending all my day just responding to tickets. Now I don't really have to do that. What I can do is I can come in and just ask for, okay, what happened in the last 10 days or 60 days? Then I get all the information.

**Guest** (00:53:46)

Then in one shot, I say, okay, help me answer these tickets because I may be a new agent. I just joined. So I don't know much about any of these things. Usually the IT agents are either Windows experts or server experts. Now you can be an expert in overall IT environment. It's not only answering questions, it's getting the answers and it's phrasing the answers and it says, and it can even send the responses right from here. So this usually used to take, imagine each ticket is usually takes about one or two hours to resolve. Now 12 tickets, think of it like 12 hours, 12 to 24 hours. We just did this in like five minutes. And that's where a combination of the Fresh Service MCP plus Cloud is helping the users, in this case, the users are IT agents, to be way more effective in catering to their end employees.

**Guest** (00:54:40)

So remember what I told you earlier by using the AI agents, it was making the users way more happier, the employees way more happier, the employee satisfaction increase. In this case, it's making the IT agents way more happier. So the IT agents are very happy because they don't have to spend as much time in Digging through information, chasing things. They're making them way more productive and as a result, they're way more happier. And as a result, even the end users who are submitting these tickets, they get immediate responses instead of having to wait. So that's the power of MCP.

**Aakash Gupta** (00:55:09)

Wow. So we just walked through AI PDLC. How do you, what this looks like an example product where you're having your user build agents and then how they can connect that with MCP into your agents. What do PMs need to know who haven't built AI agents and MCP features in order to build this next generation of product features?

**Guest** (00:55:31)

I think be curious. The world is evolving so fast that everything, the entire employee experience landscape and the customer experience landscape has literally turned on its head in the last 12 months. And it'll continue to evolve and it'll drastically change. I would say think about every single workflow. A bunch of the people are working in SaaS companies. You'll have to unlearn a lot of things that you've done and relearn things. Like everything, entire software was built for humans. What we just saw with MCP, that was not a system that was built for humans. It was built for an AI agent that was built for Cloud to be more effective. And you have to think about CLI, everything that we did in cursor. Was from a command line interface. I was literally chatting away with Cursor. Everything that I was doing in Slack, I was just chatting with an AI agent.

**Guest** (00:56:25)

So there is no concept of I have to build a thing for a person. You have to build a thing for a human being and for AI agents. So you need to learn completely unlearn how you are building things and relearn how you build things for not just for human beings, but also for AI agents.

**Aakash Gupta** (00:56:41)

One of the craziest things you shared with me is that Freshworks is changing its ratio of PMs to engineers from when you began to now. Can you walk through that evolution and what's driving it?

**Guest** (00:56:52)

Yeah. So when I started, which was like 18 months back and not too long, we had almost 1 is to 20 in terms of PM to engineer ratio. And in some teams, in some teams, one is 20, in some teams, one is to 10. So somewhere between 10 to 20. So in the last three to six months, what I've seen teams that are adopting it is the PM to engineer ratio. And we used to have one PM for it, one UX person for every two PMs and then 20 engineers for every PM. To that, what's happened is we have evolved into one PM to maybe one engineer. And sometimes there's not even a user experience designer. And it's gone to the drastic level where teams are operating so fast and there's not a lot of layers as well. You don't need to have the sprint planning session, six months planning session.

**Guest** (00:57:49)

You plan in two weeks. You release things in two weeks. Now we are seeing that with our agent studio that we just launched. We're able to see that although the number of the ratios have changed, the velocity of how we release things and deliver things to our end customers has significantly improved. So imagine coming down from six months to two weeks. And that's the pace at which it has changed. And I won't be surprised if in the next six months we go down from two weeks to maybe releasing things every two days, every week. Like that, it's almost unheard of. And in SaaS, there's also now room to do alpha beta testing. You can release things for a control group. You can even personalize software for every persona. It used to be really hard and you had to go through a bunch of bells and whistles to customize the SaaS software for different personas and for different industry verticals.

**Guest** (00:58:43)

And that is going to significantly change in the future where you will have personalized, customized software, personalized software for personas, customized software for industries.

**Aakash Gupta** (00:58:52)

For your fellow CPOs out there who are running product teams that aren't where you're at now, what is the roadmap to transform your team into this new way of working?

**Guest** (00:59:01)

The number one thing to do is not just have an edict across the organization, but actually do it. Like I was an engineer, but I was an engineer at like 15 years back. So you have to set an example. So show it, not just saying it because a bunch of PowerPoint slides and a ton of documents. People read these things and they're like, okay, whatever, this guy's sitting in ivory tower and preaching. But you don't have to preach. You have to actually show. So I picked up, again, software development in the last six months and I'm really enjoying it. And I've probably written more code than... Maybe when I was an engineer. And that's saying a lot because I'm an engineer for like 10 years. And what I just showed you, the demonstration that I showed you is an example of things that I'm doing. And so you'll have to, like at every level, people have to show it.

**Guest** (00:59:51)

And once they see it, and PMs will be like, well, if my CPU is doing it, why can't I do it? And I'm not saying that I'm doing it. There are pockets of people. So set an example. For the other CPO, set an example. So show it. Rather than saying it, show it. And there are pockets of people in every organization that are... Leading edge, that are bleeding edge and they really want to change the trajectory. Identify those people, identify those champions. So we do a monthly product team meeting where literally it's like showcasing, it's demos. It's people showing demos of things that they're doing. The PRD genie that I showed you earlier was something that one of my team members came up with and he said, hey, I built this PRD genie, I want to show it to everybody. We showed it to everybody, then we standardized it.

**Guest** (01:00:39)

The whole cursor thing that I just showed you One of the guys in our design team said, hey, I've completely reimagined the product development lifecycle. Can I show you? Those are the people that you need to identify and champion them.

**Aakash Gupta** (01:00:51)

So the worry with embracing this new way of working is that you are shipping more, you're shipping more frequently, but your metrics aren't going up. Kind of the age-old product problem, like 90% of what you ship doesn't actually move the metrics in a positive direction. How do you not only ship more, but ship at a higher quality?

**Guest** (01:01:11)

I think it's not about Shipping more, but even when you ship more, you learn faster and you can fail fast. These feedback loop that we have right now, so I almost think of the product's job as a third of it is launching the product. The other third is actually making sure the user adopted. The last third is monetizing it. Because once you ship things, you need to make sure that people are using it and then you need to make sure if people are loving what you ship, then they should be prepared to pay for it. So I would say what this does is you fail and fail fast or you succeed and then you succeed way more effectively than what you did before.

**Aakash Gupta** (01:01:50)

So circling back to where we started, these titles might dissolve. PMs might have to become PM plus engineer, this new product builder role. How are you personally hiring people, hiring AI PMs at Freshworks? How are you assessing whether they have this level of capability?

**Guest** (01:02:08)

Look, this is fairly new for everybody. I think we look for curiosity. Are you the kind of person that is open to change? And it's not just people that we hire from outside. Even for people that are there, we're making sure that we have We have a systematic training program to train people. And we have POCs that we do. And we do these innovations in pockets to make sure that it works. And when we hire people, we look for, because not a lot of people might have done this before, but you should be open, you should be curious. And I really want to see, when I interview a PM, I want to see their Git repository. How much of the things that they have done on their own. Because you can't teach passion to people. You can teach skills. You can teach technical things to people, but teaching passion is not something that is teachable.

**Guest** (01:02:57)

So people should inherently have it. So what I look for is have people done things on their own? What have they built? So the interviews are not more of, hey, tell me about this, tell me about that, but why don't you open a cursor and just show me what you did?

**Aakash Gupta** (01:03:09)

Wow. And do you guys do structured case interviews or is it mainly like show us what you've done in the past?

**Guest** (01:03:14)

So we do a combination of both depending on the level of the role and what we are hiring for. We do case interviews and we also do, okay, show me what you've done.

**Aakash Gupta** (01:03:22)

Okay. There you guys go. And Freshworks is hiring. I keep seeing PM AI PM roles.

**Guest** (01:03:27)

If people want to get in touch with you or hear more, where can they do that? Please contact me on LinkedIn. My LinkedIn is linkedin.com slash four slash srinivasan28 and Aakash, I'm sure you will publish it. So please reach out to me on LinkedIn. Yes, we are hiring. So please reach out.

**Aakash Gupta** (01:03:41)

All right, guys, for my money, seems like a very exciting product job. Find the link to his LinkedIn below in the description. Thank you for tuning in and Srini, thanks for dropping so much knowledge.

**Guest** (01:03:53)

Thank you, Aakash.

**Aakash Gupta** (01:03:53)

It was a pleasure. All right, guys. So I hope you enjoyed that deep dive into how they have used PRD Genie and AI prototyping and Figma Make to vastly accelerate how they build AI agent and MCP products.

**Guest** (01:04:06)

If you want more episodes like this, comment below.

<!-- sponsor -->
**Aakash Gupta** (01:04:08)

I hope you learned as much from today's episode as I did. If you can do one thing that's totally free that would help the show, it would be to check that you're following on Apple and Spotify podcasts. Check that you've left ratings and reviews on those platforms. Check that you're subscribed on YouTube, leave a like and a comment on this video, and then share it with your friends. We're trying to make better and better podcasts. After two years, we think we've gotten something pretty good going. So let us know what we can do to make it even better, who else we should interview, and we will put on the best shows we possibly can. Finally, don't forget my offer for the bundle. You get an entire year of my paid newsletter, plus my favorite AI tool. Bolt Up New, Airtable, Speechify, Descript, Magic Patterns, Linear, Dovetail, Arise, and Mobbin.

<!-- sponsor -->
**Aakash Gupta** (01:04:59)

That's $27,000 worth of value for just $150. So check that out at bundle.akashgu.com if it interests you. And I can't wait to share our next episode soon.
