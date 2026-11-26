---
title: "How PMs Ship 100K Lines of Code at OpenAI with Ryan Lopopolo, Member of Technical Staff"
subtitle: "The roadmap for how PMs operate inside a frontier AI company"
date: "2026-05-25"
host: "Aakash Gupta"
guests: ["Ryan Lopopolo"]
speaker_names: "substack"
substack_url: "https://www.news.aakashg.com/p/ryan-lapopolo-podcast"
youtube_url: "https://www.youtube.com/watch?v=8suwvrF0Lv0"
duration: "01:14:45"
word_count: 12399
source: "Substack episode transcript (aired audio)"
sponsors:
  - name: "AI PM Certification"
    url: "https://maven.com/product-faculty/ai-product-management-certification?promoCode=AAKASH550C7"
  - name: "Bolt"
    url: "https://bolt.new/solutions/product-manager?utm_source=Promoted&utm_medium=email&utm_campaign=aakash-product-growth"
  - name: "Customer.io"
    url: "http://customer.io/productgrowth"
  - name: "Ariso"
    url: "https://ariso.ai/aakash"
  - name: "Pendo"
    url: "http://www.pendo.io/aakash"
---

**Sponsors:** This episode is brought to you by [AI PM Certification](https://maven.com/product-faculty/ai-product-management-certification?promoCode=AAKASH550C7), [Bolt](https://bolt.new/solutions/product-manager?utm_source=Promoted&utm_medium=email&utm_campaign=aakash-product-growth), [Customer.io](http://customer.io/productgrowth), [Ariso](https://ariso.ai/aakash) and [Pendo](http://www.pendo.io/aakash).

# How PMs Ship 100K Lines of Code at OpenAI with Ryan Lopopolo, Member of Technical Staff

*The roadmap for how PMs operate inside a frontier AI company*

**Ryan Lopopolo** (00:00:00)

One of the craziest statements I heard from you was code is a liability. What does that mean exactly? Yeah,

**Aakash Gupta** (00:00:06)

there's a bunch of different ways that this expresses, but primarily all of our human software engineering organizations have been tooled around this idea that code is the most expensive thing to produce. You have synchronous limited throughput of your human engineer operators on the keyboards.

**Ryan Lopopolo** (00:00:22)

Ryan Lopopolo led the team building it. He works on the OpenAI Frontier team and today he is letting you inside how you can transform your code base, transform how you work to operate at the Frontier. You've said that if you're not using a billion tokens a day, you're basically negligent.

**Aakash Gupta** (00:00:38)

The more tokens that you're running through these models, the smarter they get, the more intelligence you're able to extract from them. This is sort of like the realization behind why we have reasoning models in the first place, right? If we give the model more effort to do inference, we're actually able to get greater results out of this.

**Ryan Lopopolo** (00:00:55)

The engineer owns the code, the designer owns how it looks, the PM owns the problems we're trying to solve. What do the new lines look like in a new EPD org? Before we get into today's episode, I wanted to share that you can get a free year of my favorite AI tools, including Bolt.New, Mobbin, Arise, RelayApp, Dovetail, Linear, MagicPatterns, ReforgeBuild, Descript, and If you join my bundle at bundle.akashg.com On top of that, I wanted to quickly ask you to please double check that you are subscribed on YouTube, Apple, and Spotify podcasts. It's a free thing you can do that really helps support the show. And now into today's episode. Every time I talk to people from OpenAI, I get the feeling that they are operating how the rest of us are going to be operating in two years. Whether that's PMs and designers actually having access to the code base.

**Ryan Lopopolo** (00:01:56)

How many of us still don't have access to the code base, right? Or actually building the right scaffolding so that PMs and designers can feel confident operating the code base. That is the next level. And today we have on one of the people who gave the best talks on harness engineering that I have ever seen, Ryan LaPopolo. He leads one of the teams at OpenAI on the Frontier, OpenAI Frontier. And today he's going to break down how you can go from the old way of working to the new way of working. Ryan, thanks so much for being on the podcast.

**Aakash Gupta** (00:02:34)

Thanks, Akash, for having me. And I'm super excited to talk a little bit about today around like what it means to enter this new wave of working where we can sort of empower the machine to do much of the work for us, which frees up the humans in our organizations and teams to focus on the things that the the true value that they bring to the table right scheduling the work bringing their taste and expertise and making sure that we're shipping actual delightful high quality products to the world that solve real user needs right that's the job and it's been fun to be able to experiment with how we can do that more effectively and at higher velocity

**Ryan Lopopolo** (00:03:10)

I'm so glad you said that because I think there's a sort of a definitional phase we need to help people with at the front one of the Crisiest statements I heard from you was code is a liability. What does that mean exactly? And what has been recently enabled with the latest versions of GPT-5 and 5.5 that allows you to say that?

**Aakash Gupta** (00:03:33)

Yeah, there's a bunch of different ways that this expresses, but primarily All of our human software engineering organizations have been tooled around this idea that code is the most expensive thing to produce. You have synchronous limited throughput of your human engineer operators on the keyboard. There has been a high sense of protectedness around that code. It is expensive to produce. It is expensive to validate. It is expensive to deploy. These things have been treated as Requiring the bulk of the organizational apparatus to manage. In this world we are today, where the token prediction machine, these lovely, highly advanced models that we have, Codex is fantastic at taking all the best parts of GPT-5 and putting those codes and words into the world. The code is trivial to generate. It can be generated at arbitrarily parallelism depending on how confident you are that the code is able to solve those problems, which we will get into in a little bit more detail, right?

**Aakash Gupta** (00:04:40)

But you kind of have to change the way you think about scheduling work and exploring when you no longer have what was the overriding constraint in your teams. because of this you can sort of remove humans from the loop almost entirely on that production aspect of the code and then you have a whole host of other problems on what it means to ensure quality right you have a less tight feedback loop for those human engineers right because they're not physically typing on the keyboard they can't attest to every line of code as it is produced but this is sort of the same spot that the rest of the organization has traditionally been in, right? There is an indirection from my designer putting a mock in Figma to me actually realizing that in HTML, SVG, and CSS. There's also this lossy translation between doing customer interviews going to a PRD and turning that into code and deployed artifacts so it's kind of nice that we have this equalizing force here where we can potentially end up in this world where every member of these software delivery teams kind of is on equal footing in terms of what it means to actually produce that executable artifact which we're delivering

**Ryan Lopopolo** (00:05:56)

When everybody's on equal footing, though, what even is the purpose of roles? Traditionally, we've had this triangle, product manager, designer, engineering. We've been able to cling to what we own. The engineer owns the code. The designer owns how it looks. The PM owns the problems we're trying to solve. What do the new lines look like in a new EPD org that's built to take advantage of the latest this technology is offering?

**Aakash Gupta** (00:06:23)

Yeah, this is really interesting. It's a question I've gotten a lot actually from executives and VP director-shaped folks that I'm talking to here. And everyone comes to this question with a slightly different set of priors basically asking which roles do I need to hire more of or less of sort of thing. But I think that's the wrong way to answer this question. Every one of these individuals on your team brings their unique lens of viewing the world. And these coding agents have all the best parts and all the worst parts of how to build software in them. So having a diverse team with a bunch of different perspectives This is what it means for GPT-5 series of models to be fully agentic. They're able to do the full job. It's not just fancy autocomplete, it's not pair programming, it's being able to go from Understanding of the user challenges, understanding the actual code base we have, the design system that we're building on top of.

**Aakash Gupta** (00:07:35)

typography primitives are how we actually are able to deploy these vehicles in order to get them into the hands of users what it means to observe whether or not they are effective and then feeding bug reports and user feedback back into the work this is like a fully closed loop that I would traditionally expect a team of four five six seven to have to do but if instead all of these different people with diverse perspectives are empowering the same agent that one agent can kind of like with full context do the full job

**Ryan Lopopolo** (00:08:04)

so If you were to frame what the old and the new roles are how would you do that?

<!-- sponsor -->
**Aakash Gupta** (00:08:11)

So sort of in the old way of working you've got your engineering team who is responsible for compiling the User visible artifacts that we want to see into code that is then deployed into the world and to do that because code has been very expensive to produce and loops have been long on feedback this has been something that has been bounded by throughput because the human engineers need to spend a lot of synchronous time and attention maintaining the quality bar maintaining the long-term viability of the code base as a long-lived artifact sort of thing and Because their time has been largely focused on the production of code within this system, there has been at least in my career, comparatively little effort around empowering others to do that same sort of work. This is why very often in organizations you see elbows out around not permitting folks outside of the team or outside of the engineering organization to contribute directly because the code that is produced is potentially very expensive to unwind or very expensive to lift to the quality bar versus having had your expert code authors producing it from scratch.

<!-- sponsor -->
**Aakash Gupta** (00:09:29)

and this has sort of led to each role on the team operating within their own lane with these very expensive coordination points and handoff points between folks and because you have these sort of bottlenecks between handing off work they're highly contended and low signal there's lossiness there it's very difficult for the designer to in the weeds observe how difficult it is to compile some of their mocks into code given the constraints of the design system that the engineering team is working with and because the designer doesn't feel that pain directly there can be sort of either resentment or missing feedback channels from the engineers to design which means like on the whole the system is not working together as effectively as it could be. Sort of when I think about you know collaborating with my infrastructure teams and developer productivity teams, we often want to shift left as early as possible, right?

<!-- sponsor -->
**Aakash Gupta** (00:10:29)

We want to feel the breakage in a system before it gets to customers, before it gets to a PR early in the developer loop because it's easier to correct them. Similarly, If it is the case that we are adopting product explorations that are difficult to prototype or experiment with because we don't have the right experimentation infrastructure here, right, as a hypothetical example, it may be difficult to push back on product priorities in favor of this sort of product platform work. This collection of three roles as a whole would very much benefit from being able to pull that work above the line in order to inflect their throughput going forward. and basically being able to in this new world get all three of these roles directly collaborating in the same codebase artifact feeling each other's challenges means there's much more empathy between them folks are able to help each other more often and in the happy case where everyone has contributed their expertise here we get higher throughput higher velocity more experimentation more high quality ui and more product delivered into end user hands

**Ryan Lopopolo** (00:11:43)

I hope you're enjoying today's episode. Are you interested in becoming an AI product manager, making hundreds of thousands of dollars more, joining OpenAI and Anthropic? Then you might want to do a course that I've taken myself, the AIPM Certificate, ran by OpenAI Product If you use my code and my link you get a special discount on this course. It is a course that I highly recommend. We have done a lot of collaborations together on things like AI product strategy. So check out our newsletter articles if you want to see the quality of the type of thinking you'll get. One of my frequent collaborators Pavel Hearn is the build labs leader so you're gonna live build an AI product with Pavel's feedback if you take this AIPM certificate so be sure to check that out be sure to use my code and my link in order to get a special discount here's the dirty secret about You spend two weeks building a prototype.

**Ryan Lopopolo** (00:12:33)

You validate your assumptions. Engineering loves the direction. Then what happens? You throw the whole thing away. Bolt changes this completely. When you prototype in Bolt, you're not building throwaway mock-up. You're building real front-end code that integrates with your existing design system. So when you hand it to engineering, they don't throw it away. They ship on top of what you've built. I use Bolt every single day. I host my land PM job cohort on it. And honestly, I'm up till 2 a.m. some days just vibing in the tool, having fun and building. That's when you know a product is good. When you're using it past midnight, not because you need to, but because you want to. Check out Bolt at bolt.new. Link in the show notes. that's what I want to see how what is what are the receipts what actually happens how can we quantify whether we're getting more product velocity more throughput at quality

**Aakash Gupta** (00:13:21)

so I can talk a little bit about sort of the project that I worked on here this experiment that I was running and back in June of last year These coding models had just started to become viable, right? We were working with Codex Mini and internally the early versions of GPT-5. We had just launched Codex CLI and for historical happenstance and accident, I set about to try and build an agent utilizing these capabilities that was for non-coding knowledge work. the thesis was that all agents were coding agents and we were going to prototype an internal agent that we were going to deploy at OpenAI and in order to do that we started from zero empty codebase and had Codex do the full software engineering job to produce this artifact one interesting thing here from a product development perspective is that having This process of codecs can only do the job to produce something that was not an engineering native agent was super, super useful because it force us into delivering value to actual end customers that were not the builders, which helped with prioritization and externalizing the learnings that we were due in this new product category to folks that could give feedback about the product, rather feedback about the process of developing the product.

**Aakash Gupta** (00:14:49)

but in doing so we produce a repository with about a million lines of code funny story about producing agents there's a lot of prompts embedded in agents about 250,000 lines of markdown in this repository because When you're shipping an agent, what you're really shipping is a multi-agent system. You have agents running around all over the place in what was an Electron app for us. Things that, you know, garden the individual Git repositories that are used to bootstrap all the tasks that the agents are working on. Things for summarization, things for distilling skills, things for actually executing the work that we're doing on users' behalf. Pretty, pretty cool way of building products and an interesting way for non-engineering users to collaborate. Because if many of the product surfaces are driven by agents, improving their behavior or changing their behavior is prompt engineering, is tweaking text. And everybody knows how to tweak text.

**Aakash Gupta** (00:15:49)

Everybody can tweak text and run the agent to get a vibe check to do an eval on whether or not the change was good. And that in and of itself is super, super empowering. but the important thing is not just that we produced an app with a million lines of code it's that when doing so literally zero of those lines of code were written by humans and this was like Ryan has dictator constraint that I have imposed on my team here which I thought was very interesting because it forces the engineers right into the backseat of the Uber right you can't drive the only thing you can do is like very politely give backseat driver directions and you know that sort of mental model is I think very useful because like It's not great to yell at your Uber driver. You need to have them use the tools available to them in the car in order to get you to where you're going.

**Aakash Gupta** (00:16:47)

A big part of building in this way is making sure that the car, the GPS, the test harness, the lints in the codebase, all the knowledge corpus of all the features we've built, critical user journeys, is there in the moment ready for the coding agent to drive. When Codex was given a task and for whatever reason was not able to do the thing, the job of the engineers working on the code base was to basically stop, diagnose what went wrong, Figure out creatively how to prevent the agent from making those mistakes going forward and try again. And every time you do that, you've taken feedback that normally you would have to give via synchronous steering and figured out a way for the repository itself to give that context to the agent. And this is why it was so easy for us to have non-engineers contribute to the code base.

**Aakash Gupta** (00:17:43)

Because every time the agent made a mistake, the engineers were forcing the agent to learn how to self-correct. which means we basically did not have slop in the codebase it was very slow to get to that point but you can not have slop by simply not permitting the agent to write slop in the first place and you do that with tests review agents and other mechanisms that are you know LLM as judge driven to prevent that slop from being permitted to be committed in the first place

**Ryan Lopopolo** (00:18:13)

You mentioned it took a little while to get there, and I think elsewhere you also talked about how the first month was about 10x slower than it would have been doing it solo. Can you explain, like, what did the first month and the evolution look like?

**Aakash Gupta** (00:18:29)

Yeah, so the earliest versions of the product exploration, starting from zero, was to kind of have the agent triage pages on my behalf, right? Going on call is a thing that I do. We're exploring what it means to have these agents do knowledge work. Dealing with outages is a thing that I do. It's text heavy. I thought it was pretty amenable to having agents do this work. And from zero, at the time, without all these lovely apps we have in Codex today, if you said, read my Slack and figure out inbound outages are happening. It's just not a thing the harness was able to do. So it's obviously, of course, much quicker for me to tab over to Slack and copy and paste into Codex, but that's not the goal, right? The goal is to get Codex to do full job. I had to stop and say, okay, I can copy and paste, but I don't want to.

**Aakash Gupta** (00:19:23)

What must I build first to give Codex access to Slack? Actually, the thing I have to build first is credential management in the harness so Codex is able to request credentials on my behalf. and in order to do that I need access to the keychain and in order to do that I need like secure coding practices that prevent me from making cryptography mistakes when we're dealing with this sensitive material and you can kind of recurse into a task like that sometimes like six seven eight times before you bottom out at the core primitive capability that is missing and then you kind of like pop back up the stack to accomplish the actual higher level primitive that you were trying to add to the product One neat thing about that is as you're doing this breadth-first search through the tools and quality gates that you need to give the agent, you knock those out one by one.

**Aakash Gupta** (00:20:14)

You don't have to do them going forward. You are importing leverage into the codebase for every subsequent change. It means that every bit of feedback I give, I at most have to give two or three times before we figure out a way for that misbehavior to just go away entirely.

**Ryan Lopopolo** (00:20:35)

So one part that blew my mind, and I always like this PM angle, is that your PM just wrote a PRD in markdown and they went to a shipped pull request. Can you give us a couple concrete examples of what they shipped and how that flow works?

**Aakash Gupta** (00:20:51)

Sure. Back in September of last year, we were experimenting with what were the precursor to skills in this agent. This idea that the human driver should be able to teach the model about the things they care about. We were doing some data analysis tasks, so understanding the data ontology of what it means to do uh business metrics in this particular part of the company was important uh and we want the model we want the harness to be able to pull this information out from the user right you know we have this lovely machine that is able to write a bunch of text it should be easy for it to have a conversation with the user to figure out the things they care about versus the things they don't so that all subsequent runs that are doing these business metrics questions kind of a crew that leverage context and the thing that we wanted to explore was what product shape does this look like right how can we give the user the ability to inject durable knowledge into the agent over and over again so our PM set about to explore this and the hypothesis was that a library with the ability to both interview the user and learn from all the tasks that the agent was already doing was the way we wanted to package up this capability and we kind of reviewed the PRD as a team and sort of the beginning of the week team meeting And at the end of the week on our demos without any of the engineers having, you know, talked at all to the PM, we had a demo of this feature and it rolled out to customers in the next week.

**Aakash Gupta** (00:22:31)

And this is very, very cool. It was able to be done safely because we have architected our code in a very, very modular way where individual pieces of business logic are able to connect together in safe ways without kind of spaghetti dependencies everything takes an interface the concrete implementations are hidden it means every bit of business logic that we have whether it was the skill wiki or the ability to manage connectors always exports a high fidelity fake for tests which means the tests that RPM was vibing into existence actually exercise its dependent services and the real business logic of the skill library without having to worry about monkey patching or having tests that don't reflect reality. The eval here is whether or not the agent was able to learn from these skills, whether or not they were mounted into context, whether or not the UI presented in the way that it should.

**Aakash Gupta** (00:23:36)

This is the same way I would think about evaling this slide deck we're looking at now, which was also created by Codex, right? Codex is a coding agent. It's going to write code in order to make this slide deck, but I don't care about that code. I care that it produces a final artifact that I care about. And putting all this work into the harness, into the repo, means that we can actually move to sort of PRD as code input with the app as compiled output. slow in the beginning. You can't do that in any brownfield codebase today and expect to get good results, I think. We'll talk a little bit around how we can sort of give you a cookbook for what to do next week in your codebases, but I think The idea here is to have the role of the engineering team to encode leverage around what it means to do a good job so the actual specifics around what you build and how it is realized in code are just kind of artifacts of the repository itself.

**Ryan Lopopolo** (00:24:40)

Encoding leverage is the name of the game. We've heard a success story on the PM side. In our pre-call, you had mentioned that it wasn't always successful. There were some things that, for instance, you guys built with your designer early on. It was like an open-claw style that you had to trash. So what failed? What did you learn? And how can people learn from that failure so it doesn't happen to them?

**Aakash Gupta** (00:25:06)

Yeah, so one thing we were trying to build was what you now see in the Codex app as automation, sort of this scheduled cron mechanism in order to kick off agent tasks on your behalf on a schedule, very OpenClaw-like, as you said. this was a capability that our designer put into the product but in doing so had to bite off a fairly chunky bit of app infrastructure work in order to put in a cron system which interface cleanly with our agentic core we wanted you know the cron itself to create tasks not necessarily be responsible for driving them to completion we wanted a nice loose coupling between these core infrastructure primitives The ultimate thing that our designer wanted to prove out was the UI interaction pattern, what it would mean to even surface scheduling to users in ways that they felt was intuitive. But in order to go from zero to putting that feature in front of users, felt that the backend needed to exist as well.

**Aakash Gupta** (00:26:14)

and the reason we ended up unwinding that is because we ended up with spaghetti, right? We were still halfway through realizing the true value of the harness here, right? Engineering had not yet fully specified all these non-functional requirements of what it means to write high quality code that is scalable for future maintenance. This is really all the harness is, is figuring out ways to get those non-functional requirements written down and injected into the agent just in time. This is what enables everyone to contribute to it safely. This is what empowers growth of the team to continue to accrue leverage back into the harness. But in the absence of that, we ended up with a spaghetti mess. I think the scheduler lived in the frontend JavaScript at some point. I look at this and I'm like, oh, I'm going to regret this later. So we made the decision to revert the PR, but we did want to enable the core objective here, which was to experiment with what this product surface could look like to figure out which interaction patterns were most intuitive to users.

**Aakash Gupta** (00:27:26)

And we do want our designer contributing to the code base because we need his expertise on how to use the design system effectively, how we should think about component architecture. We wanted to continue to explore good information architecture so we're not overwhelming users but also giving them the power tools that they need. So the norm we aligned on was we would kind of put a door between the UI as exposed to users and actually implemented functionality on the back end and ended up with what we're calling a painted door style where we can get the full product feature implemented with just a no-op on the back end with the addition of some creative product instrumentation actually able to get most of the way there in terms of doing that experimentation and actually get higher signal for the engineering team on whether or not we should even prioritize this work.

**Aakash Gupta** (00:28:24)

With code generation increasingly being automated, the bulk of my time is spent on feature triage and scheduling. So figuring out ways to get more information into that part of my work is an amazing outcome of this sort of norm we aligned on.

**Ryan Lopopolo** (00:28:41)

I used to think I had a retention problem. Turns out I had a messaging problem. I was sending the same onboarding emails to every new user whether they activated on day one or never logged in again. I had no idea who was slipping or why. Customer.io changed that. Every message I send is now based on What users actually do in the product? Someone hits a key activation moment, they get nudged to the next one. Someone goes quiet, they get a different path entirely. Their AI agent makes it fast. I describe the campaign I want and it builds the full journey form. Triggers, timing, copy, even and branching logic and when I want to know how something is performing I just ask the agent directly and it tells me what to do next they also have an MCP server which means AI tools like Claude can see directly what's happening in your customer.io workspace your segments your customer data your Notion used customer.io to personalize their onboarding and hit nearly 50% open rate.

**Ryan Lopopolo** (00:29:30)

Improved conversion by 6-7% with localized I'm notoriously bad at my inboxes. I guess there's a version of that where I seem cool and unavailable, but the reality is I miss sponsor emails, guest pitches, and stuff that my team actually needs me for. So I got an AI assistant, the sponsor of today's episode, a reason. Ariso connects to my email, calendar, and Slack. Then I just chat with it over Slack and it helps me with everything. It builds workflows to respond to emails, resolve customer issues, prep me for meetings. It actually comes to my meetings, updates its own knowledge, and remembers context from past conversations. So every time I talk to it, it already knows what I'm working on. I used to pay for Granola and Lindy separately. Ariso replaced both. One tool does more and it lives right in Slack where I already work. Check it out at ariso.ai slash akash.

**Ryan Lopopolo** (00:30:41)

That's A-R-I-S-O dot A-I

**Aakash Gupta** (00:30:44)

slash A-A-K-A-S-H.

**Ryan Lopopolo** (00:30:46)

Today's podcast is brought to you by Pendo, the leading software experience management platform. McKinsey found that 78% of companies are using Gen AI, but just as many have reported no bottom line improvements. So how do you know if your AI agents are actually working? Are they giving users the wrong answers, creating more work instead of less, improving retention, or hurting it? When your software data and AI data are disconnected, you can't answer these questions. But when you bring all your usage data together in one place, you can see what users do before, during, and after they use AI. Showing you when agents work, how they help you grow, and when to prioritize on your roadmap. Pendo Agent Analytics is the only solution built to do this for product teams. Start measuring your AI's performance with Agent Analytics at pendo.io slash akash. That's p-e-n-d-o dot i-o slash a-a-k-a-s-h.

**Ryan Lopopolo** (00:31:36)

Okay, so PM writes, PRD and markdown, designer paints a door, then engineering team takes over the actual back end. That's the high level, boiled down summary that I'm hearing. The thing that makes this all possible is the harness. Can you show us what's actually in it?

**Aakash Gupta** (00:31:56)

The harness lives in the repository, but really the harness is a mechanism for getting the coding agent, getting codecs, the right context it needs in order to do the job at all phases of the implementation lifecycle. I think there's kind of three phases you would think about here. One is I'm getting ready to go to work. I have a ticket, I have a PRD, and I need to figure out what must be done in order to implement the thing and get it deployed. The next phase is kind of in the messy middle of implementation. I'm writing code, I'm exercising the UI, I'm seeing the bugs, I'm seeing logs, I'm making sure that, you know, everything is pixel perfect. And then there's the back half of things where I have produced a diff that I claim implements the feature and I need to convince the rest of my team to merge it, that it is acceptable, that it meets the actual user need that we're trying to solve with this change.

**Aakash Gupta** (00:32:52)

and in each of those phases we have different mechanisms in order to surface context to Codex in order for it to do a good job. In the beginning here we really have agents.md which is this file that lives in the root of the repository that is forcibly injected into Codex. It's like what Codex CLI does is take the contents of that agents.md and give it into context for the agent And this is both good and bad, right? Things in agents.md we know are 100% reliably going to inform the agent's actions. But we're paying for that with context window usage. And with these models, context window is a hard constraint. You cannot fight against it. There is only so many hundreds of thousands of tokens you get. I will say that auto compaction in GPT-52535455 is so so good I never run out of context these days Sort of like a crown jewel of research here to have good auto compaction It is truly amazing to be able to go on any size of ticket completely end-to-end on a single session.

**Aakash Gupta** (00:34:05)

It's magical But still you do have to contend with things getting paged out of context even with auto compaction so agents.md is a tool but one that we want to kind of be constantly trading off from this scarce resource of context so what we do there is we put an operating model for codex in there basically a sort of like three-step four five-step plan of how you should think about doing a task and what that means for us is You ground the decisions that you make in the documentation we have in the repository. There's a big docs tree. It includes everything from what it means to write performant react to writing reliable networking code to all the design docs and critical user journey flows that we have in the app. That's important to have as part of the operating loop because we don't inject that stuff all into the agents.md up front.

**Aakash Gupta** (00:35:03)

Instead, we just tell codecs in the agents.md, you have all these resources available to you. They are of X, Y, and Z shape, and they live here. You decide whether or not to look at them. which is nice because we can like deterministically steer the agent toward the context we want it to discover but we let the magic of these models reasoning decide what is important what it actually thinks should pull into context this is sort of the outset of the task so ground yourself in the documentation that we have the app as it is written and then move into implementation During implementation, the thing the agent is naturally going to do, the thing it is trained to do, is write code and make tool calls. So we have to figure out ways to use those two mechanisms to inject our context into the agent. This is kind of a silly thing, but actually the code in the repository is prompts.

**Aakash Gupta** (00:35:58)

Codex is going to pull code into its context window in order to figure out What business logic do we have? How do we do things here? What database adapter am I using? Am I using Jotai on the front end for state management? So actually having the repository enforce that the code is all the same or uses the same patterns or is structured similarly allows you to efficiently and sort of like in parallel across the code base apply context you've read in one file to other files. It means that the agent is able to more effectively cargo cult. I love to cargo cult stuff. This is how I have worked in big brownfield codebases when I'm new, right? I'm like, the team has probably done this before. Let me kind of like poke around and copy and paste some stuff. And we can let Codex be lazy too by making it do the hard work of making the codebase homogenous.

**Aakash Gupta** (00:36:55)

But another way we can inject context into the agent over the course of doing these runs is to take all that human judgment around what good looks like and basically make it fail tests if the code doesn't match. A stupid one that I do is to fail the build if there is any text in markdown files or HTML that does not use the curly quotes because our design team loves that proper typography in our user facing strings to have the smart curly quotes and apostrophes and this is probably a thing that is like unevenly adhered to I think in most code bases if at all but Because this kind of like irked our designer a couple of times, had him vibe code some tests into existence, we don't really care about the quality of this code, right? So long as it actually does the job and prevents the code from becoming misaligned with the user intent.

**Aakash Gupta** (00:37:55)

We have a lot of tests like that that do probably weird things, maybe things you would consider low leverage, but collectively improve the quality of the software that we're delivering, which I think is pretty cool. And then on the back end, right, we've got Sort of the agent executing grounded in the documentation we have in the repository, which is this accumulation of all of the team's historical work and knowledge. We've got taste refining the output as we go via these tests and lints and the code itself showing the agent what good looks like. And on the back end, kind of take all of that same context and give it to a review agent. In that docs repository, right, we have frontendarchitect.md, reliabilityengineer.md, appsecengineer.md. And for each one of those, we have this big matrixed CI job that says, you review for frontend architecture. Here's your guardrails.

**Aakash Gupta** (00:38:50)

Here's the diff. Identify all the P2 issues with this thing and leave some feedback on the PR. This feedback, more context, just like those tool call error messages that we're giving the implementation agent to say, you must address this, right? We found some issues where you are misaligned with the way we expect things to be produced. and with sort of all of this effort in prompt injecting the agent with the collective human judgment on the team my synchronous involvement here can basically move all the way to the back of this process where the code is presumably already reviewed and approved and aligned by all this machinery that we've put in place over the course of executing producing the change and then my job is to say okay we've got this change it looks good but I think it's misaligned in ways x y and z and then once the those things are addressed in the moment my job is to close the loop by taking all this feedback that I had to give and making it so I don't have to give it next time and then back into the harness it goes so

**Ryan Lopopolo** (00:39:55)

we got the high level now of what it involves can you go really glint granular show your actual codec setup show what's on every engineer PM designers machine and how to put this all together practically

<!-- sponsor -->
**Aakash Gupta** (00:40:10)

I would say that The way I have steered my team has been intentionally friction full so that we don't want them staring at the computer looking at their agent which means they have largely been booting up codecs in the CLI going to multiple tabs where it's actually painful in order to pay attention to these things because we don't we don't want them to if I were doing it again today this is probably not what I would do right that the app is quite fantastic and is a thing that we are seeing meteoric growth in I think it was just past 400 or 4 million weekly active users and all the good parts of the workflow that i'm describing are in the app right i would package all that collective designer taste into a plugin that you know my team has a little shared marketplace of that i can just suck all of that expertise into the app that's going to pre-wire figma which means the place my designer naturally works is going to be a thing that is directly addressable by codex in the same way that I have access to Figma and maybe I'm unreliable at refreshing my knowledge of the current mocks.

<!-- sponsor -->
**Aakash Gupta** (00:41:22)

Codex is just going to do that because these agents will follow instructions well that is that is a core part of how they are built so these plugins which bundle the skills include those instructions on these are the tools we use these are how they are built so I think the app today as sort of the central coordination mechanisms of teams gives a much more user-friendly affordance for distributing these sorts of things plugins are definitely the future and what I would lean into today

**Ryan Lopopolo** (00:41:53)

All right, can you show us what this actually looks like inside of Codex, how someone would set all this up?

**Aakash Gupta** (00:41:59)

Sure, let's get into the nitty-gritty of it. This is my favorite part here. So, right, we started with an empty repository, right, which means we had a high degree of freedom to start structuring the code in a way that Codex most natively understood. And this is how we kind of came to the pattern that all the things we want Codex to know need to live in the repository itself. This was its workspace, this was its brain. In order to mise en place, get the agent set up, we wanted it to have the easiest time and the thing that Codex loves to do is search code with ripgrip. So we put everything in one place. And what that looks like in practice is this big docs directory that has a ton of different content in there. We make heavy use of a thing called an exec plan, which you can find on the OpenAI Cookbook, which is essentially a skill you can give Codex in order to write a good implementation plan phased with milestones and deliverables so it can track its and make sure that it is continuing to make progress against sort of high-level and tricky implementation plans.

**Aakash Gupta** (00:43:05)

And we kind of keep every single one of those that has ever been produced in the repository. They form a durable log of the implementation choices we have historically made. Similarly, every design doc ever written, rather than being buried in Slack threads and Google Docs, live in the code base, which means these things are actually continuously kept up to date to reflect the actual state of our app. They're sunset and archived when they become irrelevant or features get removed. We have also built code and tests around this documentation tree. All these markdown files cross-link to each other. They embed git repository revisions of when they are current as of. If Codex ever touches one of them to update it, the build will fail unless all the cross-linked documents are also updated to reflect the current state of the world. This is what it means in order to have the harness self-maintained to have the test prompt injecting codecs with what it must do.

**Aakash Gupta** (00:44:05)

We don't rely on codecs knowing that this is how it maintains the doc repository. A test will tell it what it needs to do, how it must proceed in order to get the build to green. The agents are super trained in order to get the test to pass. So if we can figure out ways to build context injection primitives into failing tests, we're not fighting the harness here. This is not a thing that will be obsoleted by the model capability improving. This is just a very neat way of aligning what must be done with the scarce resources of context with the actual thing the model will and always do, which is call tools and run tests. Similarly here, you can see in this references section, we have a bunch of these llms.txt. I don't know if everybody knows this, but like a lot of programming projects will publish a, you know, plain text version of their documentation at llms.txt.

**Aakash Gupta** (00:45:01)

And this strips away all the tokens from the HTML and it's just like Markdown. Stripe has these, OpenAI Docs have these, UV which is a Python runtime has these, our internal design system has these, and we check these directly into the code base which basically give Codex a full reference manual for all of the big, chunky libraries and components that we depend on. And we point to those. Our documentation on the design system highlights the key components that are probably going to be used most of the time and how to look for them in this llms.txt. Here you can see these persona-oriented documentation that we talked about earlier, right? What it means to write secure code. This product-sense.md is how we think about encoding what it means to document a feature, how to turn a PRD into code in a QA plan. And this is the sort of thing that I doubt any teams are writing down today.

**Aakash Gupta** (00:46:00)

It's just a thing they kind of, you know, talk about together and maybe whack each other on the nose when they don't do this when producing a PR. But figuring out a way to actually durably document what it means for the team to operate is necessary for these agents, which every time they spin up, have a blank slate in terms of context. Another neat thing here is this qualityscore.md which is sort of a meta way for codecs to diagnose the state of the codebase. We have it keep notes here every time it writes code because Over the process of making a change, it's going to pull a ton of code into context. Maybe code that hasn't been touched in a month, but our guardrails have changed. So this is a way for Codex to be continually assessing the quality of the codebase, doing some gardening, and spinning up some tasks for later on how we can keep aligning the codebase to baseline.

**Aakash Gupta** (00:46:56)

Another neat thing we can sort of talk about here is what it means to close the loop. When we're working on this app, we split it into a back-end and front-end pattern, which means they could be tested independently. And we tried to house as much of the business logic as possible in our back-end. And that means codecs should be able to validate the behavior of our business logic headlessly, right? You don't need to drive a UI. You can hit APIs and look at the database to observe the side effects that you were hoping to have. And normally, for almost all of my career when I'm working with services in local dev I run them in my terminal and I get this never ending stream of logs in the console that like I have no idea what to do with and it's kind of impossible to use because they scroll away so quickly.

**Aakash Gupta** (00:47:44)

What we've done instead is permit Codex to spin up like something approximating a production observability stack. I think giving Datadog to Codex for every change that it makes and this allows it to use like Normal observability tooling for metrics and logs the same things your engineers would be using to diagnose issues in production and we let Codex use it to diagnose issues in local dev, right? Shift left, validate the change and exercise it end to end. And we do the same thing with the UI itself. We mount the UI into a local browser shell that pre-wires up Chrome DevTools. Today we would do this with computer use to allow Codex to actually inspect the app, drive it, click the buttons, observe that the loop is closed, that the feature is implemented, and that it can attest that it works end to end. So I mentioned a little bit how being super overly architected in the application was a point of leverage for the engineering team.

**Aakash Gupta** (00:48:46)

And the reason that is because we've actually limited statically the plausible places that code can go. You see this kind of represented here as sort of a package layering stack. One common pattern in hypergrowth codebases that is a failure mode is that business logic kind of just gets spewed everywhere and it becomes a sort of codebase that approximates a ball of mud. These are very difficult to deal with and evolve because there's a ton of non-local side effects from touching any bit of code. But I mentioned that we have these nice isolated business logic domains that are able to take all their dependencies as fakes and make it safe for us to prototype new features. And the only reason we're able to do that is because we actually with code enforce that these things are hard separated with package boundaries between them you cannot possibly create a ball of mud in the first place which basically means that for the engineers we permit them to write packages at any layer of the stack they can write database code config parsing you know react code in the front end business logic our PM we kind of by norm and convention said you can write business logic and UI code but try not to touch these lower level primitives in the app and to get that painted door invariant for our designer had him focus largely in the UI layer of the app with you know some affordances for stubbing out APIs on the back end so that we could get those usage signals that we cared about Which is kind of neat to be able to think about reflecting sort of like ACLs on who is permitted to touch what code and the actual structure of the code itself.

**Aakash Gupta** (00:50:35)

Like this is actually by folder paths that we're able to determine whether changes are allowed or not.

**Ryan Lopopolo** (00:50:41)

This adds up, and I think you have a really

**Aakash Gupta** (00:50:45)

hot take on how it should add

**Ryan Lopopolo** (00:50:47)

up. You've said that if you're not using a billion tokens a day, you're basically negligent. Now that's two to three thousand dollars per engineer. How does an engineering leader at a normal company build the case for that internally?

**Aakash Gupta** (00:51:02)

The idea here is that the more tokens that you're running through these models, the smarter they get, the more intelligence you are able to extract from them. This is sort of like the realization behind why we have reasoning models in the first place. If we give the model more effort to do inference, we're actually able to get greater results out of this. And we see this time and time again with longer time horizons that agents are able to execute over. And I think it is the case that In order to have this sort of lofty coal of being a token billionaire, right, you kind of have to find ways to get the agent to do more work on your behalf, to execute in parallel more autonomously. And because I believe that GPT-5 is able to do the full job, having that as a North Star constraint means that I am constantly looking for ways to get the agent to do the hard parts of my job that take a lot of my time.

**Aakash Gupta** (00:52:06)

and constantly being surprised in ways this frees me up. One sort of insane thing is not just a billion tokens a day, but sometimes it can be 350 million tokens on a single PR. There was a time a couple of months ago where I was buckling my laptop into the back of my car, going back and forth to the office, tethered to my corporate phone in order to have the agent continue to cook while I was commuting to work. This is like a 60 hour Codex CLI session that like I was like please don't go to sleep laptop and this is a PR that probably would have taken me three weeks in order to do like one of the hardest refactors I have ever done in my career and took place over the course of three four days and did as good a job as I would have here because of the investment we've put into letting the harness prompt inject the agent and manage its context efficiently over that 60 hours I only had to provide two prompts in addition to my first prompt that we gave the agent which is truly magical it means that it was actually approximating a human engineer on my team I did not have to synchronously bash it on the head in order to make progress it just went heads down and did the work the way I would

**Ryan Lopopolo** (00:53:26)

Okay, so 60-hour running long task, I think that points to something that if people have their conception of these models five, six months ago, it's really outdated. It's what's recently become possible that's enabling this new way of working. How would you describe it? When did that happen?

**Aakash Gupta** (00:53:45)

Yeah, so there was a huge uplift in capability when GPT 5.2 came out, and the rate of progress with each additional point release of the model has been much bigger than what came before. GPT 5.2 came out while I was on holiday for a winter break. And when I came back, without any additional investment, we were getting one or two PRs more per day per engineer on the team, which had this very strange effect where folks were looking for ways to do more work with the agent. It was kind of like adding another lane to the highway. It was like, how can I put more cars on this thing right now? Because we had done so much work in order to get Codex to operate over those long horizons, the next sort of frontier was to go in parallel. We just blogged yesterday about a sort of agent orchestrator that came out of my team called Symphony, which Once we saw the uplift in capability with 5.2 and invested in this additional orchestrator, allowed us to further 10x the PRs per engineer per week.

**Aakash Gupta** (00:55:06)

That investment in increased parallelization is only a thing we were able to do because we were confident in the code that was being produced already by the agent, right? If I'm 10xing the number of PRs I am producing a week, I cannot possibly look at all that. I couldn't possibly look at them all before. So the only way we could do this safely is with these techniques in order to eliminate classes of misbehavior and have confidence by default in the code that's being produced. But yeah, we continue to see these huge improvements in autonomy and confidence with each model revision. One of the most interesting things about 5.5 is with computer use, There's much less wrangling we have to do in order to get the agent to actually see and drive the app. This was a significant point of friction for us early on. We were having to figure out ways to wire up FFmpeg to Docker containers to give Codex a virtual X server so it could drive the app.

**Aakash Gupta** (00:56:08)

This is all a ton of low-level goo and plumbing nonsense that was slow to develop and ultimately undifferentiated. With Codex now shipping computer use, a tool that's natively post-trained into the model, we kind of get to throw away all that bespoke code, keep the same process of having Codex drive the app and do it much more efficiently with better image understanding, ability to faithfully replicate wireframes and mocks, these sorts of things. Truly amazing.

**Ryan Lopopolo** (00:56:43)

You mentioned one of the hardest refactors in your career. You've worked at the regular companies, the Brex, the Stripe. These types of companies, if you are an engineer at this and you're looking at this new way of working, what is the new engineering job?

**Aakash Gupta** (00:57:00)

The new engineering job, I think, is to have everybody be staff engineers. And the role of a staff engineer, the primary role, at least for me, is not to be producing all of the code, but to be empowering my team to produce the code. And today, it is the case that every single engineer on this planet, modulo token budget, has access to 550 or 5000 concurrent hands-on keyboards. Not being able to leverage that amount of parallelism today is largely a reflection of not having put in the work to harness those resources. One experiment we're running internally in order to drive toward this amount of parallelism is to tell teams that they have been forced to hire five interns named Codex. Part of their success criteria is judged on how effectively they incorporate these resources into their team. What does it mean to make use of this capacity that the organization has given them?

**Aakash Gupta** (00:58:03)

Part of success is being able to use those resources. If we think that with access to these lovely models and compute being available to use them, Letting those GPUs idle is in a way not having hands on keyboards. So my job is to figure out ways to saturate these things, to have them doing productive work, to have them not waste cycles, to have fewer PRs that we throw away because they are high quality by default, to have fewer cycles back and forth in CI, fewer reviewer agents having to repeatedly burn cycles for the same feedback, that sort of thing. It is very much a systems thinking sort of mindset where in a way you're playing Factorio with your codebase and figuring out ways to build the token factory.

**Ryan Lopopolo** (00:58:56)

You're describing essentially being totally divorced from the code and really focused on using these interns. But I guess a lot of engineers, they prided themselves on being the best at writing code. That has been their output for so long. I imagine people on your team have struggled with this mental shift. What is the right way to think about it?

**Aakash Gupta** (00:59:18)

This is a thing I have struggled with too. For a long time because The primary function of the job was to produce code in order to achieve, you know, our product and business objectives. It's very easy to fixate on the production of code itself as the job, but ultimately the reason we work in tech is to deliver product into the world. And initially kind of like having this hard break in mental model of what it means to do work was a little bit like weird on the ego sort of thing, but where I have gotten to is Latching onto the same creativity, the production aspect of things, ultimately the thing that motivates me is to get product into the hands of users and see their delight and how they're able to improve their lives with the tools we build. I'm still able to do that today.

**Aakash Gupta** (01:00:11)

I'm able to do a lot more of that today. And I kind of like puzzles. You can have puzzles in how you structure the code, or you can have puzzles in terms of how you put teams together to produce it. To me, these skills and challenges are pretty transferable between each other. So I think there is a new art to be found, a new craft in terms of how you effectively assemble a virtual team to go solve these things.

**Ryan Lopopolo** (01:00:39)

Okay, so let's move into the roadmap. Your counterpart at Brax or Citadel or Stripe, they want their PM shipping 100,000 lines of code. What's the Monday morning roadmap that they need to take so that they can get started right now to move to this way of working over the next six months?

**Aakash Gupta** (01:00:57)

I'm so looking forward to the Monday Morning Roadmap. You have no idea. I was super excited to divide this slide into existence with Codex because this is the hook right here. This is why we're talking. So I think those... Map, or those phases of the code production process that we talked about, map pretty clearly to sort of what the Monday morning roadmap should be. You need the repository to be legible to the agent. It needs to know all the things that your team does. right the process of bringing product into the world to producing code to having good design has a ton of implicit context around what good looks like hundreds or thousands of little decisions that we all We all make by default because we cut our teeth the hard way, gaining experience. But the agents don't have this, right? Well, they do, but they have every possible permutation of all those thousands of decisions because they have seen so much code and so much product over the course of their training.

**Aakash Gupta** (01:02:03)

So it's our job to take the specific choices that we as a team would make Write them down, give them to the agent, and starting with this simple technique of putting a map in agents.md on where the agent should look. I really like having a documentation tree as sort of the entry point for making this happen for your code base because it's super easy for humans to think about just writing stuff down. And it's also really easy to use some of the tools that we have to do that. It's very often the case that, you know, Agent will produce code we didn't like or there's a bug in production. have a slack thread as a team where we discuss what went wrong how we think it should be done differently and it's really easy at the end of that to just do at mention codex you know update docs x y and z to reflect these new guardrails this new taste we have discussed and you know that kind of removes us from the loop entirely from maintaining the legibility we just kind of get to talk and we let codex maintain it for us and This is a way too that I think sort of by default in larger teams you can kind of sort of build a flywheel around improving agent behavior and build sort of cultural norms and processes around having this happen as a default way of doing the work.

**Aakash Gupta** (01:03:25)

The other next step is to make validation cheap. Validation is happening at all parts of the code production pipeline that I talked about. on the review side of looking at those guardrails over the course of writing the code with all these lints and tests, being able to actually close the loop and exercise the app to see that, yes, the search box that was in the PRD actually appears in the UI, and when I click on it, it shows a pending set of results that are our best guess, and it has very nice type ahead without any jank in the box when we type. are kind of the squishy, ill-specified parts of the task, but kind of providing proof of work to the reviewer agents and the humans looking at these PRs is necessary in order to build confidence. This is what it takes in order for me to not have to shoulder surf the codex in the same way I'm not going to shoulder surf my teammates in VS Code or Cursor.

**Aakash Gupta** (01:04:20)

And finally, it's important to have the users of this harness be more than just the engineers themselves. The exercise here is to empower all of the team in order to write code safely. So having a tight collaboration loop with the other members of the team, product design, user ops, your DevOps folks, allows for really high bandwidth feedback between these different roles and it allows you to do more work, different types of work, extract different domain expertise from the folks on your team and reflect it all back into the repository for the benefit of everyone. One sort of like emergent property we had here that I thought was really, really cool was we hired a new engineer onto the team who had formerly been a PM. And he noticed that we had no documentation in the code base for what product features we had. and this is kind of an important thing because it grounds all the engineers all the designers all the product the reviewer agents everything and what we are actually trying to achieve what are we shipping here and Codex is very good at crawling through a code base and figuring out what the product features are and writing them down and surfacing them for human review but what fell out of that was a set of QA agents that are constantly booting the app running it through these critical user journeys and asserting things work which means that when it comes time for deploy we have to do less manual smoke testing because we actually have sort of these just-in-time generated runbooks around what it means to have acceptance testing.

**Aakash Gupta** (01:06:08)

And all of that came out of a single person with domain expertise and an idea of what good looks like. And sort of the rest of the work we had done made these higher level correctness verifiers kind of fall out of that one thing.

**Ryan Lopopolo** (01:06:28)

We're actually full circle all the way back to the beginning of the discussion. Now that people understand the harness, they understand the Monday morning roadmap, what does the product team of 2027 look like? How are these individual functions working together if everybody has access to the code?

**Aakash Gupta** (01:06:48)

I think we're going to see a lot more prototyping in the world, a lot more diversity of products as a result. I think, too, in this new wave of computing with AI and agents, we are currently at the early part of the technology curve where a lot of the products you see today are low-fidelity text interfaces. When I think about where I sit in OpenAI, working on Frontier and deploying to businesses, in order to get the machine to do the work, there is a fractal nature of work. Different surfaces, different ways of working to wedge these models into the nooks and crannies of the hard knowledge work that happens. So I'm really excited to be able to rapidly experiment with different modalities and different ways of delivering this technology. All right, so

**Ryan Lopopolo** (01:08:08)

We're into the home stretch here. I want to ask you a couple quick questions. Is that okay? Yeah, sure. Let's do it. What's one skill a tech lead who's trying to move to this way should build this weekend?

**Aakash Gupta** (01:08:19)

I really think it's important that you figure out a way to get Codex to be able to see your app and drive the business logic. In the absence of any other modularity or investment, the ability to actually close the loop and observe the behavior that you're changing is what it takes in order to know that you have completed the job. I see this all the time where folks will vibe something up and not be able to attest that it solves the problem they set out to do. And in order to convince the rest of the team to accept the code in the first place, you got to be able to prove somehow that the code meets the brief that does what it says on the tin. And the way to do that is to invest in closed verification loops, the highest leverage of which is the full end-to-end integration test.

**Aakash Gupta** (01:09:13)

Click the buttons, observe the side effect, that sort of thing.

**Ryan Lopopolo** (01:09:17)

It's funny how it comes back to some of the fundamentals, but now applied to AI. What's the biggest mistake engineering leaders are making with AI coding tools right now?

**Aakash Gupta** (01:09:27)

I think Having the tools in your head or in a box as these things that are tools that must be driven synchronously by a human is limiting the amount of creativity in terms of deploying these things widely. Ever since GPT 5.2 came out, my belief is that it is as capable as me at doing the full job, and it's sort of my job to figure out ways to have it do as much of my job as possible. a lot of that means I can't be sitting in front of it because I don't sit in front of my teammates so there's this whole metagame of building confidence in the code that these agents are producing so that we can have it do more and more of the job to execute on longer and longer time horizons to be more and more independent and this is necessary in order to unlock that true parallelism, that 5,000 engineers worth of compute that I talked about I can't possibly do that if I'm locked behind two tabs in the app or three panes in my Tmux in my terminal.

**Ryan Lopopolo** (01:10:34)

Final sort of meaty question here for you. We've been talking about GPT 5.2. At the same time came out Opus is 4.6 roughly. And the whole discussion really changed in that December time period. If a team can only pick one, the Anthropic stack or the OpenAI stack, what's the case for picking the OpenAI one.

**Aakash Gupta** (01:10:57)

Our models are optimized around that full agentic behavior to being able to do the full job. I am super easily able to delegate entire swaths of work to the GPT-5 series without having to constantly poke and prod it. And this is the fundamental unlock for me that has gotten to that parallelism. Symphony, this agent orchestrator that we have released, is fundamentally very uncomplicated. It is a thing that advances linear tickets through states and gives the ticket text to codex and expects it to produce a PR. There's very little magic to it, which is why I think that sort of these GPT series of models that we have are the ones that are going to unlock the true power of agentic software engineering in your organizations. Additionally, the pace of product delivery on the model capability side in order to get more and more of that loop closing in place has just been fantastic.

**Aakash Gupta** (01:11:58)

Things like parallel tool calling and background shells in GPT 5.3 to ever increasing auto compaction capability to computer use and the ability to have multimodal understanding at high fidelity with built-in image generation capabilities in the latest 5.5 means that What would normally have been two or three people on the team handing off between them means that instead those two or three people can encode all their leverage into one tool which is then able to do the full job. There is this kind of neat story that I have been telling that in multi-agent systems the Correct amount of agents to want to optimize toward is not multi, it is one. Because one agent is able to have full addressability over the entire task and its entire context, which means being able to do design backend and frontend in a single agent means you're going to get higher quality results than having these lossy, frictionful handoffs between them.

**Aakash Gupta** (01:13:03)

and that experience comes from me having built agents for knowledge work with handoffs in them and seeing the massively increasing capability of the GPT-5 series over time. I want a single agent to cook and do the full job and we have done a fantastic job I think at increasing Codex's ability to address all parts of the SDLC in a single agent.

**Ryan Lopopolo** (01:13:28)

Wow, there's so much information in there. If I want to get more, if I want to get more of Ryan, where can I find you online?

**Aakash Gupta** (01:13:37)

I tweet a lot on X. My handle is at underscore LaPopolo. And me and the team should have more content coming on the OpenAI blog. And I am doing a bunch of conference tour over the summer. I am next going to be at AI DevCon in London. We'll see you there.

**Ryan Lopopolo** (01:13:59)

All right, guys, follow him on Twitter. Check out his amazing blog post on the OpenAI blog. And we'll see you guys in the next episode. It's

**Aakash Gupta** (01:14:08)

been a pleasure, Akash. Thank you.

**Ryan Lopopolo** (01:14:10)

Thank you. I hope you enjoyed that episode. A couple of things you can do to support the show. One, comment. Two, review. Those ratings and reviews really help other people understand the value and the production that we are putting into this, right? This wasn't an easy episode to produce. We put in a ton of pre-work. We edited it for you. We brought in the best guests. If you don't mind sharing a rating and review, sharing the episode with others, making sure you are subscribed, that really helps the show do bigger and better productions. I'll see you in the next episode. Here's one of those that YouTube thinks would be a great fit for you.
