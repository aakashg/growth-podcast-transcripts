---
title: "How to build a Company Operating System with Hermes and OpenClaw"
subtitle: "Claude Code is just the start of what a Company OS can do. Here’s how to take it to the next level."
date: "2026-08-28"
host: "Aakash Gupta"
guests: ["Mikhail Shcheglov"]
speaker_names: "substack"
substack_url: "https://www.news.aakashg.com/p/company-os-hermes-openclaw"
youtube_url: "https://www.youtube.com/watch?v=zocznD8Z-6k"
duration: "01:06:22"
word_count: 9737
source: "Substack episode transcript (aired audio)"
sponsors:
  - name: "Bolt"
    url: "https://bolt.new/solutions/product-manager?utm_source=Promoted&utm_medium=email&utm_campaign=aakash-product-growth"
  - name: "Customer.io"
    url: "http://customer.io/productgrowth"
  - name: "Viktor"
    url: "http://ref.viktor.com/aakashgupta3"
---

**Sponsors:** This episode is brought to you by [Bolt](https://bolt.new/solutions/product-manager?utm_source=Promoted&utm_medium=email&utm_campaign=aakash-product-growth), [Customer.io](http://customer.io/productgrowth) and [Viktor](http://ref.viktor.com/aakashgupta3).

# How to build a Company Operating System with Hermes and OpenClaw

*Claude Code is just the start of what a Company OS can do. Here’s how to take it to the next level.*

**Mikhail Shcheglov** (00:00:00)

Agents are actually building most of our features. Any stakeholder can talk to an agent and validate any feature request they want. Our agent is an operating system because it's hooked into everything from Google Workspace to Granola, Confluence, Jira. Meet Mikhail Shcheglov, the CPO at OLX Classifieds, formerly CPO at Azerbaijan's biggest e-commerce marketplace

**Aakash Gupta** (00:00:21)

and GPM

**Mikhail Shcheglov** (00:00:30)

We've built everything, our entire stack on top of OpenClaw and Hermes agentic scaffolding. I use this knowledge graph to understand how well teams are doing with customer discovery and how well they are connected to the entire organization. What's gonna happen to my job? What actually will happen is that teams will be smaller, leaner, and faster. Not only it's gonna change, the lines are gonna blur.

<!-- sponsor -->
**Aakash Gupta** (00:00:55)

What's gonna happen to the future? Is product management going to exist in the future? I have good news for you, I think. Before we get into today's show, please take a second to check that you're subscribed on YouTube and following on Apple and Spotify podcasts. If you want access to all of my favorite AI tools, I've gotten them to give you an entire year of their paid plans. Check out bundle.akashg.com for an entire year of Bolt.new, Airtable, Speechify, Descript, Magic Patterns, Linear, Dovetail, Arise and Mobbin. And now into today's show. I know you guys are overwhelmed with guides on Hermes and OpenClaw and Clodcode and ChatGPT. It seems like there are a million AI tools out there. And more and more of you are reporting to me that you're not even feeling more productive. And Mikael is one of those people. What he has built... At OLX Classifieds is an entire operating system.

<!-- sponsor -->
**Aakash Gupta** (00:02:10)

If you've been hearing about buzzwords like OpenClaw and Hermes and saying there's no value for PMs, this episode is the one that will change your mind. He has got his entire team hooked Aakashgupta.com

**Mikhail Shcheglov** (00:02:43)

Alright, so if you think about this, like what's the core goal of having AI native teams? Is to be able to automate as much knowledge as we can. Because like in previous, I call this old paradigm. Like you used to have a knowledge worker, like an employee who has built a context around a certain domain. Let's say it's a deep expertise domain like search, recommendations, ML and stuff like that. And then all of a sudden this person decides to leave the company and takes all the knowledge with him or with her. He's a bottleneck effectively, a knowledge bottleneck. And the core thing that we're trying to prevent here is the leakage of that knowledge. Because if you could have a single storage of this entire business, customer, product, technical knowledge in one place, then it would increase the entire value of your organization. That's just one angle to it.

**Mikhail Shcheglov** (00:03:42)

And another angle is... The better your AI knows your context, the more autonomy you can give it, the higher level tasks you can delegate to it. And let me explain how it actually works in our case. So what you see here is the entire knowledge graph of our company that has been formed over like five months. Like five months is basically nothing. And you can already see this like web of interconnected particles. And these particles, they cover everything from our contacts, who talks to whom, To which projects we're working on, to which customers we're talking with, which businesses we've reached out, even our funnel metrics, basically everything. And you can see in the top right corner, like there is a specific metric, which is a product context coverage. And this is one of my personal KPIs, because the higher this percentage of coverage, the more, as I mentioned, You can delegate to it.

**Mikhail Shcheglov** (00:04:51)

Because right now, what this means is that it understands our industry, like classifieds, our market, our business, our business model specifically, the top line, the bottom line, the drivers behind it, our customers. And the value drivers for them at the level of 54%, which already means that it can operate as a capable, I would say, junior to meet product manager and even make backlog level decisions. The more this coverage grows, like at numbers of 70 to maybe like 90%, I would not be surprised if this knowledge graph would enable you to do some strategy level work and help business Navigate decisions. It's a question of when we're going to get there, but we're definitely going to get there. Let me maybe zoom in a little bit on the elements of this knowledge graph. So you have three layers. So the first layer is the product. So all the nodes that are connected to the product side of things.

**Mikhail Shcheglov** (00:05:58)

And you can see like product has been very involved into everything. You have the contacts, which is basically all the people talking to each other in different parts of the organization. And there are like personal things that I share, like my thoughts, my reflections, and the personal things that some of the other people share, like, of course, fully anonymized. Then another layer is the teams, right? I don't really go at the level of actual, like say, cross-functional teams. It's more of a clusters or divisions, right? So if you take buyer and seller experience, you can immediately see how interconnected they are within the organization or like the platform teams or like the pay and ship teams. And you can even drill down at the level of a specific product manager. And you can see on a team level, what's their knowledge of their existing context, which for me is a very strong predictor of how good the team is in terms of customer discovery.

**Mikhail Shcheglov** (00:07:02)

Not only that, there is another angle to it. If the team isn't really well connected, and you can clearly see that this team has very little nodes, overlapping nodes with the buyer and seller experience, even though a platform is a horizontal layer and they should be, ideally they should be intertwined with each other. You can clearly see that there is some instances of silos happening. Which means that teams should talk more with each other. And two, I would also raise the question of the stakeholder management. Like are stakeholders really being involved in the processes within the teams and so on? And that's kind of my core tool that I'm using because it shows me the quality of the output of the entire organization.

**Aakash Gupta** (00:07:58)

This is like the coolest visualization I've ever seen. So what tool is this? How are these metrics working? How are they measuring things?

**Mikhail Shcheglov** (00:08:06)

So you can use like tools like Obsidian for this. I personally created this one from scratch using Fable because it was like a two-liner prompt basically. The important question that you asked is like super important one, which is how do we measure this? And we have a very specific prompt that asks an AI. What percentage of knowledge around industry, and you have to be very specific, what do you imply by industry? In our case, we have five verticals, we have real estate, we have auto We have good sales, we have services and jobs. What percentage of knowledge around the business, meaning the business model, the actual P&L, the drivers, and what percentage around customers, like different buyers, sellers, customers, segments, even on a cohort level, marketing, and so on. Which percentage of knowledge do you have at the current point in time taking all of your memories loaded into you directly?

**Mikhail Shcheglov** (00:09:15)

And what we've seen is that AI has been quite accurate in digitizing this abstract request into a specific number as an output. And what I'm also observing is that the more active product managers are, and they typically come with, I would say, transcripts or research studies or like RFD documents, and they load it directly into our agent, into its memory. And I'm seeing that the metric is actually improving over time. It doesn't mean that it's a single source of truth. And I think each organization should come up with a specific context metric that would be highly specific and relevant to them. But this is something that I found directionally works.

<!-- sponsor -->
**Aakash Gupta** (00:10:03)

Here's a quick word from our sponsors. I need to say something that most AI coding companies don't want to hear. Their tools are not built for enterprise. Think about what happens when 20 people in your org start building with AI. Marketing makes a dashboard. Product prototypes a feature. Sales builds a demo tool. Each one looks different. Different components, different styles, no shared design system. And none of the code is pullable. Engineering can't integrate any of it. You've got 20 AI-powered prototypes and zero production-grade output. Bolt.new solved this with something called Design System Agents. Upload your actual design system, your NPM packages, your CSS files, your component library. The DS agent builds a custom system from your real code. Now, every person building in Bolt.new across your entire org is using your components, your buttons, your tokens, your brand. And when engineering pulls the code, it matches what they already ship with.

<!-- sponsor -->
**Aakash Gupta** (00:10:54)

That's the difference between an AI tool and an AI platform. Check it out at bolt.new slash akash. I used to think I had a retention problem. Turns out I had a messaging problem. I was sending the same onboarding emails to every new user, whether they activated on day one or never logged in again. I had no idea who was slipping or why. Customer.io changed that. Every message I send is now based on What users actually do in the product? Someone hits a key activation moment, they get nudged to the next one. Someone goes quiet, they get a different path entirely. Their AI agent makes it fast. I describe the campaign I want and it builds the full journey form. Triggers, timing, copy, even And when I want to know how something is performing, I just ask the agent directly and it tells me what to do next.

<!-- sponsor -->
**Aakash Gupta** (00:11:35)

They also have an MCP server, which means AI tools like Claude can see directly what's happening in your customer data workspace. Your segments, your customer data, So instead of explaining your business context every time you need help, Claude already knows it. Notion used customer.io to personalize their onboarding and hit nearly 50% open rate. Improved conversion by 6-7% with localized candidates. The idea is simple. Customer.io helps you deliver more impact from every message you send. If you're a PM or founder and your onboarding is still one size fits all, try Customer.io at Customer.io.

**Mikhail Shcheglov** (00:12:14)

Okay, so this is a totally different

**Aakash Gupta** (00:12:16)

way to view a product team. Most product teams, most PMs aren't used to this. If they want to build this, it sounds like there's two things they do. They define the metric and then they create the visualization with Fable. Let's take a step back here. What is the role of a CPO? In an organization like this, what is the new agentic CPO doing here?

**Mikhail Shcheglov** (00:12:42)

That's a great question, Aakash. I think what has changed significantly is that in the past, the whole team was responsible. Outcomes were measured in how much your metric has moved and outputs, how much RFD documents, how much code, how much prototypes, Figma mockups like your team has been able to produce depending on the function. Right now, what has changed and changed pretty significantly is that the cost of this output is negligible. But what becomes more important is the quality and the token consumption. So what do I mean by quality? Quality for me is the amount of AI outputs that have significantly moved or moved the metric. So it's essentially outcomes, but outcomes that were driven by And this is how I measure it in terms of the metrics. In terms of the actual tooling, I think previously what CPU was responsible for is building a procedural scaffolding on top of the organization.

**Mikhail Shcheglov** (00:14:01)

What it means is that you have certain, like, hiring principles, right, your vision. Then if you go a level lower, you have certain processes, like a planning cadence, like a yearly strategy, then a quarterly strategy, then a sprint planning. And then you have, like, different reviews, like design reviews, product reviews, and so on. And this allowed the organization to function. But right now, what is more important, it's not the process itself. It's creating an operating system within which AI could be a collaborator of product managers and where AI could not only help to kind of come up or challenge ideas, but it could autonomously make decisions. And the best way to achieve this Is that is by owning the entire agentic scaffolding architecture and creating specific rituals, creating specific processes and enabling the team to be in touch with those agents all the time, training the team to use it actually.

**Mikhail Shcheglov** (00:15:09)

Let me know if you'd like to go deeper into any aspects of this.

**Aakash Gupta** (00:15:13)

How does this manifest in the PM process? Where are the savings had for teams? Why should a CPO suddenly be spending so much time as an agentic orchestrator?

**Mikhail Shcheglov** (00:15:24)

The biggest reason for this, if you break down the time that product managers on average used to spend, Probably, not probably actually, I estimated this based on my previous experiences, around 50% of the time of a typical product manager was spent on processes and rituals. You have different business reports, weekly reports, stakeholder management reports, different demos and so on. And this is a repetitive type of task. That doesn't really require much cognitive input in many cases. It's just something that you have to do manually. And if we abstract all of this and start delegating this part of work to AI, then essentially what you end up with is you have a product manager that is solely focused on discovery, like where the biggest leverage actually is. And a single product manager could actually do the work of two product managers because he doesn't have the burden of all the processes that a typical corporate environment imposes on him.

**Aakash Gupta** (00:16:49)

Wow. Okay. So we've seen the knowledge graph. We understand the role of the CPO and what it There are multiple buckets of tools that this agent can solve and we constantly improve it. So the first bucket is status reporting.

**Mikhail Shcheglov** (00:17:13)

Like you can ask it, like, what's the status of a specific project? Let's say, uh, what's the status of auto, spare parts, catalog, integration, uh, respond in English because he might get finicky. Okay. And while we're waiting for this, there are multiple other things. So status can be, you can get a response in whichever shape or form you want. Directly in Slack, in Google Doc, in Confluence, Whichever format is more convenient for you. Second thing is, it is integrated into all of the workspaces. Google Workspace meaning Calendar, Gmail, and so on. I don't read my email anymore. An agent does it for me and pings me. I don't manage my calendar anymore. And it's especially difficult when we live in this interconnected world where everybody is remote in different parts of the globe. And just setting a single meeting. You can clearly see it's all there.

**Mikhail Shcheglov** (00:18:21)

Scope, Listings Automated. You can clearly see what's the status. It's quite straightforward.

**Aakash Gupta** (00:18:28)

Nice. And did you like, have you been tweaking the prompts on how it gives status updates? Because this is like a pretty good one.

**Mikhail Shcheglov** (00:18:35)

Yeah, yeah. So it has a massive library of rules and imperatives. I think like 700 lines or so. To give you the cleanest and the most factual output without hallucinations.

**Aakash Gupta** (00:18:50)

Very cool. So we'll go into how people build that. What other use cases should they know about within Slack that they can accomplish here?

**Mikhail Shcheglov** (00:18:57)

Like one angle to this, let's say you're a stakeholder, right? And you have a certain feature that you just assume is important to have. By whatever reason, like a typical route for a stakeholder in this case is to go directly to the product manager and harass a product manager with feature requests. But now we have a gatekeeper, which is our agent running under the hood. And we train our stakeholders to interact with an agent before reaching out to a product manager. And let's say, yeah, I just woke up and I have a feature request. I urgently want to have a video submission for autos, a story like in Instagram. Of course it's fancy.

**Aakash Gupta** (00:20:02)

Cause I saw somebody else doing it. Right. That's always the reason.

**Mikhail Shcheglov** (00:20:06)

All competitors are doing it. We are behind. Yeah, for sellers, yes. And this is just like a typical feature request, which doesn't have a problem framing, it doesn't have any impact estimates, it doesn't have any rationale behind, and it doesn't respect the actual priorities that have already been defined for the organization. And by doubt, we'll just give it a little bit of time to think. It will respond with a list of clarifying questions. And in case, if after answering all the clarifying questions, an agent decides that this feature isn't worth building, then it will politely say so. If it is worth building, then this feature will be added to the backlog and escalated to the responsible product manager. An agent has all the organizational structure mapped out internally. So he knows exactly who the owner of a specific domain is.

**Aakash Gupta** (00:21:12)

Wow. And do you consider yourself the owner of the Saul Goodman agent? Yes.

**Mikhail Shcheglov** (00:21:20)

I think it's a great point and it's a dangerous way to go. I think you should own this for two reasons. One reason is the speed of iteration. Own this and you're constantly improving and I'm getting feedback every single day. What works, what doesn't work and so on. And I immediately like open my IDE or my cloud code and I make the changes right off the bat as we go. It's super fast from feedback to deployment. Secondly, this actually has an impact on the organization because one, it saves time and two, it stirs decision-making, which means it might have an impact And I think CPO should own this. If you delegate this to an engineering team or if you delegate it to another person who doesn't have the skin in the game, then you're not going to get the same level of speed and impact. Okay.

**Aakash Gupta** (00:22:20)

So CPOs should be building this. Now they want to know how. Can we open up the covers and show people how they build something like this?

**Mikhail Shcheglov** (00:22:28)

Absolutely. Absolutely.

**Aakash Gupta** (00:22:30)

Let me open up my IDE.

**Mikhail Shcheglov** (00:22:32)

Actually, I will show you two ways. This is just to give an overview. I will kind of walk you through the architecture, the brain, the memory, the tools, the skills, and I'll explain it all as we go. So for the architecture here, what we're using is a combination of OpenClaw and Hermes. Why those two? Because OpenClaw is just a great scaffolding. It has everything available out of the box and great engineering support. But Hermes has a unique feature to it, which is an automated skill generation. And I've actually tested it. Across five core topics that my team works and I've seen an improvement in a recall metric, which means that it was way more accurate in responding using those skills by 31%, which was a dramatic improvement. So I decided to blend both of those scaffoldings together in a combination. And it's jacked in terms of the capabilities because we've been improving it for like five months continuously.

**Mikhail Shcheglov** (00:23:48)

When it comes to memory, it has three layers of memory. So the first layer is what you've seen is a knowledge graph, it's like an entire It's a high universe of interconnected knowledge and everything. And you can see the code here and so on. But what is plugged in there, it's a second layer, which is a vector database. And the vector database is essentially every single Piece of knowledge that an agent receives gets immediately converted into vector. And you need this because most of the requests are fuzzy. And in order for you to get good retrieval, you do need to have vectors because You might ask some random stuff, right? That is not related to any specific keyword. And an agent needs to be able to match your request to a specific point, to a specific number in your knowledge graph. And the third layer... And what I've seen makes agents the most robust and they don't lose context is every single conversation is stored in transcripts.

**Mikhail Shcheglov** (00:24:55)

You can clearly see that every single day the agent stores everything into MD files. And not only this encompasses granola transcripts, because all of our meetings are transcribed, but also all of the conversations that I had with an agent and all of the reflection that an agent has. So those three layers of memories, persistent memories, they create this robust knowledge base, which improves every single day.

**Aakash Gupta** (00:25:23)

Wow. How does that exactly, how do you architect that properly? So obviously you get a Granola Enterprise license, you have that coming in and recording every single meeting, but I guess you don't want to just save all the meeting details. You want to strip out some of the personal conversation out of meetings and then you want to write these more condensed synthesized MD files. How do you go from raw transcripts that might have personal information to useful synthesized output?

**Mikhail Shcheglov** (00:25:50)

That's a great point as well. And that was my assumption that you actually have to summarize and synthesize the output to be useful. But we tested this in multiple ways. And it turns out that summarization actually hurts a retrieval. For two reasons. Like one is when you summarize something, you lose granular details. And the devil is always in the nuance and the details. And another reason is that when you summarize, you impose a certain template onto whichever conversation that you had. For instance, like the tasks that were solved, the tasks that remain, what is important, what is not important. And then on top of this, on top of this template, you try to kind of shove your transcript into this template. And we've noticed like a huge fidelity loss and I think it was like 20-25% worse recall. That's why my personal architectural decision here was, let's just store every single transcript, every single conversation that we had in a raw form.

**Mikhail Shcheglov** (00:27:06)

Quick thought experiment for you.

<!-- sponsor -->
**Aakash Gupta** (00:27:07)

Is there anything in this video you should be trying on your own? If there is, try it, take a screenshot, post it on LinkedIn or X, and tag me. I'd love to see what you're learning. Now a quick word from our sponsors before we get into the back half of the pod. Do you know how to take an AI product from idea, to development, to evaluation, to deployment, and eventually to scale? That's exactly what Product Faculty's AIPM certification helps you do. I even took the course myself. You'll learn directly from Rohan Varna The product lead working on codecs at OpenAI. You'll go deep into AI prototyping, evaluations, agents, AI-native workflows, cloud code, OpenClaw, latency, cost, guardrails, rag, routing, fine-tuning, and production systems. You'll even build your own AI product as your capstone with unlimited one-on-one support. So if you want to stop just learning AI and actually build AI products that work, join Product Faculty's AIPM certification on Maven.

<!-- sponsor -->
**Aakash Gupta** (00:28:05)

5,000 plus students have graduated and they have 1,000 plus reviews. Use code AKASH550 to get $550 off your enrollment. I used to live in Report Purgatory. Every team had a different number. Every weekly review started with someone reconciling spreadsheets. We stopped hiring more analysts and gave the reconciliation to an AI employee instead. Victor is an AI employee that lives on Slack and Microsoft Teams. It connects to 3000 plus tools your team already uses, ships real deliverables, and every action goes through your team for approval first. It's the closest thing I've seen to a small team running like a much larger one. Let me share three things that First, AskVictor has replaced our Monday Metrics scramble. Someone types, flag any customer, whose usage dropped 40% week over week, and draft an outreach loom for the account owner to approve. 90 seconds later, the next step is ready.

<!-- sponsor -->
**Aakash Gupta** (00:29:03)

Second, scheduled tasks run the work that nobody wants to remember. Every morning, Victor checks overnight support tickets, drafts replies for the on-call to approve, and escalates anything mentioning churn. Nobody had to ask for it. Finally, Spaces ship internal tools in minutes. Ask for a renewals dashboard, Victor builds it, with authentic database, and post the link to your channel. The team can stop opening four tabs to get the same view. So stop chatting with AI and start working with it. Get started at victor.com. There's $100 in free credits with no card required at viktor.com slash akashgupta3. You can find that link in the description. I want to take a second to talk to you about Three months where you're going to have intense sessions, a Monday morning session where I go over your resume, behavioral interviews, LinkedIn. On top of that, Bart Jaworski is going to be teaching you the PM fundamentals in 2026, how to write AI PRDs, how to AI prototype with Google.

<!-- sponsor -->
**Aakash Gupta** (00:30:12)

All of the key skills you need to freshen up your knowledge for this market. And Ankit Vermani is going to be teaching you AI product management. He is an AI product manager at Uber, and he is going to teach you how to build AI features that actually work successfully. On top of that, Prasad Reddy is going to be doing one-on-ones with you for market reviews, LinkedIn review, candidate market fit review. So it is a full package. It is three courses in one for one low fee. So join at landpmjob.com. Wow. And Hermes and OpenClaw on their own can figure out how to get into which meeting and which meetings are relevant context and they won't just fill up their context window with random meetings.

**Mikhail Shcheglov** (00:30:50)

Yeah, absolutely. Because like what happens is that when you ask a request, what it does, it does a search query. And it's a blend. It's a hybrid search query. It tries to do exact keyword matching. If it's not successful at this, which I think 75% it's not because it's hard. It's a very ambiguous raw context. Then it does the vector search. And vector search allows you to do this exactly fuzzy retrieval based on probabilities. And that pretty much handles like the remainder 75% of use cases. So it only retrieves the relevant pieces of data that is highly specific to your request. And it doesn't really overload the prompt with tokens there. Very cool.

**Aakash Gupta** (00:31:44)

So that's the memory component. What else do people need to know to build this?

**Mikhail Shcheglov** (00:31:47)

I think the thing that after deciding on the architectural aspects of this, it is hugely important to create a list of imperatives. And as you know, LLMs are very biased because of how they are trained. And more specifically, they are focused on the resemblance of good output. Rather than the actual results. And you can do workarounds to solve this. And the best way is to have this list of imperatives. For instance, what for me is... What's super critical is that there's no fabrications. If you look here, it's just a huge list of different imperatives that we've created over time. It's who you are, it's your voice, it's think before You act because that's a terrible thing I've noticed. LLMs do a lot. They provide you the output that looks plausible, but there wasn't that much thinking behind it because it's full of contradictions. Then there's always facts over guesswork and anti-patterns.

**Mikhail Shcheglov** (00:33:06)

Another angle which super pissed me off a lot, I call this fake helpful. For instance, if you ask your agent to book you a meeting, and suddenly your tokens in the Google workspace has expired, and then the agent says, well, I'm sorry, I cannot do this, but it's super easy for you to do. Just open up a calendar, type in Google Calendar, Name your meeting, choose your time. I mean, it's useless. I mean, it's an obvious advice. You don't even have to waste tokens explaining this. And I call this fake helpful. And if you are able to put it as an imperative, it will save you a lot of time as we go. But you can clearly see we've made a lot of tweaks over time.

**Aakash Gupta** (00:33:51)

So for people who don't know, we showed ClaudeMD and SolMD. What's the difference between those files? What should be in what? SolMD, I believe is a part of OpenClaw?

**Mikhail Shcheglov** (00:34:01)

Yeah, it's a part of OpenClaw. It gives, uh, effectively, uh, like it's, um, a specific context that is being loaded into every single prompt. Um, and ClaudeMD has just the highest priority of them all. And SolMD is the second in order of priority for OpenClaw.

**Aakash Gupta** (00:34:18)

So your CloudMD, it seemed like you kept that under 100 lines, which I think is the advice that Boris Cherny, creator of CloudCode, gave. The StoleMD though is like 800 lines, so that can be longer?

**Mikhail Shcheglov** (00:34:28)

Yeah, it's longer. And you might argue that we are overloading the context and some of those lines might even be contradictory. But what I've noticed was that that's the most robust way that gives me the most accurate Output with the best recall. And we test every single imperative. We actually test on the basic queries to see across the most important topics that we raise in the organization, like how good it is or how bad it is.

**Aakash Gupta** (00:34:59)

All right. What else do people need to know to set this up?

**Mikhail Shcheglov** (00:35:01)

So another angle is you need to have tools, right? And it has a lot of tools. So since it's interconnected with all of your workspace, it is deeply integrated into Google. So it's a separate tool. It's integrated into Atlassian. It's a separate tool. It has automations, and automation, like the one that we currently have, it just consumes all of the mobile reviews. It writes a digest, like a typical supportability team would do. And it even tags the people that are responsible, and it can even raise red flags in case it's necessary.

**Aakash Gupta** (00:35:37)

And these are all Python files. You just prompt these with natural language in the IDE to clod and clod writes these? Or how does that work?

**Mikhail Shcheglov** (00:35:46)

Previously, I used IDE, but now I'm doing this for showcase purposes mostly. I'm using clod app. Because it allows me to do this on the go right here. It is accessible from my mobile phone in case if an urgent thing appears and I want to change anything within the agent.

**Aakash Gupta** (00:36:07)

So do you basically create a GitHub repo that Cloud Code can access?

**Mikhail Shcheglov** (00:36:12)

Yes, exactly. So every single change is immediately committed into GitHub repo. Awesome.

**Aakash Gupta** (00:36:17)

So you do everything via GitHub, via Claude app. That's so powerful. So you can configure, people kind of have this mistaken thing that they need to use the OpenClaw gateway, but you can actually do everything through Claude and it can manage it on top of Hermes and OpenClaw.

**Mikhail Shcheglov** (00:36:33)

Absolutely. So the only benefit IDE gives you is that you can clearly see the structure of the project.

**Aakash Gupta** (00:36:40)

Yes. And you went through two IDEs actually. So you showed us anti-gravity and cursor. Talk to us about when you should be using the Cloud app versus anti-gravity versus cursor.

**Mikhail Shcheglov** (00:36:50)

My use case are the following. So everything that lives in the cloud and doesn't require If I require, I would say, access to my computer, I'm using, I'm interacting with it through CloudApp. But any specific use cases that I have that require my And mostly these are around browser use via different MCPs or Excel use if I want to load a file and get some immediate feedback or data research if I don't really want to load it into agent and I want to do something ad hoc, I use an IDE for this. And why do I have two IDs? Simply because it allows me to have two autonomous separate instances of agents running at the same time.

**Aakash Gupta** (00:37:41)

Okay. I think I understand the Open Claw setup part of this. It's mainly through the SoulMD plus Open Claw is what's giving you that gateway to the Saul Goodman agent in Slack. Explain the Hermes part of this. You had said it's related to the skills and the recall.

**Mikhail Shcheglov** (00:37:56)

So, um, the beauty of Hermes as a scaffolding. It comes with a unique advantage over OpenClaw, which is it automatically generates skills based on the tasks that you most frequently request the system to perform. And what we've noticed in testing was that the recall has improved significantly. Well, I mentioned 30% with those automatically generated tasks, skills, sorry, versus without them. So we have it running under the hood all the time. Like for instance, team hiring evaluation, immigration, like case building, because we have like different people who are relocating locally. So I have a lot of questions around it, then it made a decision that we should Have a skill for this. The same team hiring evaluation also made a decision. Why do, why do I continue doing repetitive tasks? Why not just create a skill and offload all of this onto an agent? So it even kind of takes this meta part of the understanding whether or not you need the skill and makes a decision for you.

**Mikhail Shcheglov** (00:39:05)

That's, that's an amazing part of it.

**Aakash Gupta** (00:39:07)

Awesome. And how did it help with the recall? You mentioned it also helped there.

**Mikhail Shcheglov** (00:39:10)

Plus 31%. So what does it actually mean? So we have five core topics. Those topics are market, it's a business model, it's product, Key growth levers, selection, price, buyer activation, trust. Then we have more tactical things like funnel and so on. And we have a set of different questions. We asked 10 questions for each of those areas and we compared the non-skill response versus the skill response. We also looked at how accurate the response in each of those categories for each of those questions was. And what we've seen was that having those skills in place gave us plus 31% more accuracy, which was a deal breaker.

**Aakash Gupta** (00:40:12)

How did someone set up like the metrics to measure something like recall?

**Mikhail Shcheglov** (00:40:17)

You can do it. And basically yourself, I'm doing this as a CPO because I think outside of knowledge graph and percentage of context digitization, so to say, you should also be able to track more tactical metrics, which is recall. Claude or whichever system you're working with or your agent directly, tell me which areas are the most frequently asked or which I most frequently interact with and come up with 10 questions. Questions per each of those areas which are the most frequently asked. And then let's do a comparison. Basically like one control group versus the treatment group with the skills and see what's the difference there.

**Aakash Gupta** (00:41:11)

That's pretty much it. To use sort of a derogatory word, but not in a derogatory way, you're vibing the metric. You're in natural language, you're explaining exactly how you want it to work, and then it's creating the metric, and it can go off and measure it for you.

**Mikhail Shcheglov** (00:41:26)

That is correct. But I mean, for the first pass, you have to at least visually look at the results. But once you have a methodology set up, then you can delegate the evals fully to the system.

**Aakash Gupta** (00:41:41)

All right. Amazing. So now people know how to set this all up. Can you show us some more use cases? What are the best, most powerful things people should be using this for?

**Mikhail Shcheglov** (00:41:50)

One cool thing is this is this is also around skills, but I think this would be Highly practical for people, especially in C-level positions. So I have a board of directors that I'm in constant touch with and they make investment decisions, right? How much money we As a company should receive at which point in time, what would be the payback and so on and so forth. And there are multiple people in the board and they have different perspectives. But the beauty is the agent was able to abstract their mental models into a set of principles. And we called it the board skill. So in case if you have a pitch deck, And you want to defend the strategy for the next year. Then the first thing I do is I run this pitch deck through the board skill to kind of poke holes and give me brutal feedback on what could go wrong with the defense of this strategy.

**Aakash Gupta** (00:42:54)

Fascinating. So your granola meeting transcript is automatically recording your board meetings. Hermes has automatically created a skill around the profile of those board members. And so when you're creating a board deck in Claude, let's say you use Claude Design and you would put in your input. Towards the end of that process, you're going to hit it with a prompt like, Use the board skill to see how the board would respond so that we can refine this. Is that right? That is exactly right. Fascinating. That brings up an interesting point for me. We as CPOs, we may not want to let our PMs see. What's going on in a board meeting? How do we make sure that information is locked down so that the right groups get access to the right information?

**Mikhail Shcheglov** (00:43:40)

Well, that's a great question. And two things. So the first one, it all boils down to scope of ownership. And the agent has different access rights depending on the person reaching out. And that access rights will define the context which this person or employee is able to retrieve and the tools which this person would be able to work with. For instance, board skill is available only to me and to the executive committee within the company. And the second thing is the privacy aspect, right? Because not all people really appreciate that their personal meetings are transcribed or recorded. So unless you willingly provide this information to Granola, We will not train the model and we will not create like the skills on top of this. So every employee has a say in this, of course. I'm personally a part of the experiment. That's why I'm completely transparent and I don't care about my privacy at all.

**Aakash Gupta** (00:44:48)

Okay, so if you slip in that you were taking care of a sick kid during the weekend, you're okay with that, hitting a transcript. But if a particular employee doesn't want it, they can elect to take it out. Absolutely, absolutely, yes.

**Mikhail Shcheglov** (00:45:01)

From the get-go, we don't really store the personal transcripts of people's meetings because I think that violates privacy. So unless you willingly provide us this information, we will not do this.

**Aakash Gupta** (00:45:16)

So you can select, like... This is a product trio meeting. This obviously makes it in. This is a product review, but this is just a one-on-one between me and my designer.

**Mikhail Shcheglov** (00:45:25)

This is not going to make it in. Exactly. Exactly. Got it.

**Aakash Gupta** (00:45:28)

So Bordex is one really cool use case. What else should people be using this for?

**Mikhail Shcheglov** (00:45:33)

Let's see. I'd respond it in a different language, but the thing is, so we asked it, I want a specific feature and instead he created a prototype. Whoa. Let's see. Yeah.

**Aakash Gupta** (00:45:47)

That's quite agentic and autonomous.

**Mikhail Shcheglov** (00:45:50)

It's agentic and autonomous. And it sometimes gets finicky, depending on which language we interact with. And we use different languages, so that's why it might get frustrated at times and it requires an imperative. But here, I think it created a prototype, which is very close to our actual design system. Okay. I mean, it's not great in terms of UX, but as a one-shot pass, I think that's an okay thing. As a one-shot? I mean, it's just so much stuff, it's done. Yeah, pretty much so. And it's very compliant with the actual Nexus design system, which is an OLX design system at play.

**Aakash Gupta** (00:46:34)

And do we know what underlying model it hit? Did it hit Fable or do you have intelligent model routing?

**Mikhail Shcheglov** (00:46:40)

How does that work? So the thing is there is an agentic orchestrator which makes a decision on which model So if it's a complex request or if it's a specific domain area which has high sensitivity or error blast radius, most likely it will assign Fable onto it. If it's just an execution type of work or a status report writing, I think it will assign Opus 4.8 most likely. For low level work that doesn't require super accuracy, it will assign Sonnet. So talking optimization becomes important here.

**Aakash Gupta** (00:47:24)

So mostly it builds on the anthropic stack. You're not throwing in a codex or a GLM yet.

**Mikhail Shcheglov** (00:47:30)

So it's also a great point. Our engineers actually do. Because if we look at the typical triad, so engineers have their own agentic stack, product has their own agentic stack. Of course, they communicate with each other via the same reg and MCPs.

**Aakash Gupta** (00:47:47)

But when it comes to product management,

**Mikhail Shcheglov** (00:47:50)

We use code by subscription, pretty much so. And we don't really have that much of token spend at the moment. That's why it's not a critical metric for us to track. While for engineers, it is critical. And they actually have a totally different scaffolding and they have a blend of different models running under the hood. For the breakdown of tasks, which is typically considered the work of highest complexity, how do you break down an abstract EPIC They use the highest cost models like ChatGPT 5.6 or Fable. But for lowest complexity items, they use like smaller models or sometimes even locally deployed open source models.

**Aakash Gupta** (00:48:35)

How does this help you with things like your design system?

**Mikhail Shcheglov** (00:48:38)

Pretty significantly, let me show you Figma. So if you look here, right, the entire design system was built from prompt. Wow. And it's very well documented. And the Components are robust and what is more important was that the components are exhaustive. So for instance, you have all of the sizes of the components, you have all of the states, all of the relevant tokens. And it is continuously supported by the agent himself. So in case if during the conversation between engineers and a product manager, there is a disconnect, right, then because a certain component is missing or somebody tries to hard code a component, for instance, then an agent is well, is informed about this and makes a decision to create this component here in the system.

**Aakash Gupta** (00:49:36)

So it's automatically updating the design system based on the work different design teams and product teams are doing. Yeah, that is correct. And how do you make it auto-updating like that?

**Mikhail Shcheglov** (00:49:46)

So one is it has a certain tool on the product side that kind of collects all of the requests that are coming either directly via Slack or from a coding agent. And then it just fires up a development crown job to start building those components on time. Of course, there is a review process where a designer takes over and looks through the components, whether they are correct or not, like how well they are documented, are there any conflicts, are the states exhaustive and so on. But that's a review type of a job rather than execution job.

**Aakash Gupta** (00:50:33)

And is the review, is the design system skill in Hermes auto-improving? Like is the amount of review that the designer needs to do getting less over time?

**Mikhail Shcheglov** (00:50:43)

It's a great question. I'll have an answer by our next podcast.

**Aakash Gupta** (00:50:49)

Amazing. So that's design system. The next use case you talked to me about, which I think is fascinating and I really want to see, is on backlog and

**Mikhail Shcheglov** (00:50:56)

roadmap management. What do you use there? So, you know, the biggest problem with backlogs is that every single team Every single team has their own textbook. Every single team has their own Excel spreadsheet. There are many apps or tools that try to automate this, but I haven't seen a single successful case. That's why my understanding of a backlog is more of an abstraction on top of all of the Excel spreadsheets the team are working with. It's basically every single team has their own spreadsheet. I'm not going to like open them right now because of the NDA things, but the It's the typical type of a backlog, right? You have a project, you have a problem, you have a solution, different links, impact effort, ROI, and so on and so forth. Every single team has their own backlog and they're all interconnected. They're all connected into agent and an agent can fetch all of this information and can contribute directly to the backlog in case if a feature is definitely worth it and passes the ROI bar and passes the review of a responsible product manager.

**Aakash Gupta** (00:52:03)

Fascinating. What about personal assistant? How can you use this as a personal assistant?

**Mikhail Shcheglov** (00:52:08)

That's my favorite part of a flow. Let's maybe, I need to Plug in the meeting with execs for one and a half hour next week. Not too early, not too late. Suggest something. That's how you would typically talk to your personal assistant. So right now it does all the retrieval processes that we've talked about and the ideal response is he will come back with a list of different time slots that would work for all of the execs who all have busy calendars, who operate in different time zones all across the globe. And I would make a decision on which one to choose. If I'm too lazy, I can even delegate the decision making onto an agent.

**Aakash Gupta** (00:53:08)

So while that's running, you mentioned you aren't even checking your email anymore. You weren't checking your calendar anymore. So how is it managing those for you? How is it surfacing the right emails, the right calendar events, getting that prep going?

**Mikhail Shcheglov** (00:53:21)

So every single day I get to the Digest or what's important, what have slipped in terms of Slack messages or emails. I browse through it or you can clearly see Wednesday, July 22nd. Yeah. Clean a slot chief. Let's use it.

**Aakash Gupta** (00:53:39)

Wow. So it's applying intelligence. It's figuring out when those execs are available. It's looking across time zones. And you can even schedule the meeting directly to the app.

**Mikhail Shcheglov** (00:53:49)

Yeah. I don't need to open the calendar. So I'm getting the digest. I review the digest and I make a decision on which emails are actually worth acting on versus the ones that are not, or which tasks or messages I need And if I'm not feeling like responding directly, I will ask the agent to come up with a template response.

**Aakash Gupta** (00:54:10)

Amazing. I know the last area can be a bit of a headache for product leaders. On top of our own job, we need to keep the pipeline of really good PMs. How can this help with recruiting?

**Mikhail Shcheglov** (00:54:21)

Oh, actually quite a bit. So it has three tools integrated. So the first tool is LinkedIn recruiter. Let me try and see whether he will be able to respond. The number of product manager candidates we have in the pipeline, just the number. Okay. LinkedIn recruiter is responsible for reach outs. So if you have a question, I'd say, I don't know, I want a specific candidate with a very specific domain expertise with this many years of experience located If I meet it in this specific place, just go and find me. And if the candidate is found, then I will ask to do reach outs using predefined templates that we've agreed on with an agent before. The second thing is, it is integrated into our CRM. Different companies use different CRMs. Greenhouse is probably one of the most popular And I don't really interact with the CRM anymore because I do all of the work via the agent.

**Mikhail Shcheglov** (00:55:43)

I just type in who is in the pipeline or I provide the feedback directly to an agent. An agent posts this feedback or moves the candidate along the funnel. Or if needed, I can even build the funnel statistics to see where the gaps are in terms of the hiring. And the third aspect to it, which is quite amazing, which is the interview process. Because all of the interviews are transcribed, you can get immediate third-person opinion on whether or not the candidate really lived up to your expectations. And in case if not, of course, you are the final decision maker, not the AI. It just gives you an alternative point of view, which is sobering in many cases. Then you can ask AI or you can ask an agent to draft a rejection letter and reach out to the candidate. So this automates probably like 70-75% of the recruiting workflow.

**Mikhail Shcheglov** (00:56:49)

And more importantly, it drafts beautiful tailored rejection emails with really deep focus areas for improvement that were derived from the Granola transcript. None of the recruiters that I know actually do this well.

**Aakash Gupta** (00:57:07)

So you get to deliver a much better candidate experience as well as making it faster and easier for you and potentially even making better decisions

**Mikhail Shcheglov** (00:57:16)

because you have the transcript. Exactly. Exactly. Yes.

**Aakash Gupta** (00:57:19)

This has been mind blowing. I want to talk to you about some hot Sure, let's dive into them. What's on everybody's mind right now, just in the zeitgeist, is what's going to happen to my job? He just showed me how, you know, you might be able to do the work of 2 p.m. with 1 p.m. So what's going to happen to the future? Is product management going to exist in the future? What's your take?

**Mikhail Shcheglov** (00:57:44)

I have good news for you. I think not only product management is going to exist, I think it's going to thrive. Because I think product management in large organizations became burdened with layers of hierarchy, with layers of corporate processes. And in many instances, product management is about compliance, performance, status reporting. So it's suboptimal product management, to be honest. And I think what AI really helps you to do, it doesn't remove away the decision making from the process. It gives you the juiciest bit. It removes a lot of the operational overhead from the work. And what product managers are now more focused on is the value discovery. Because what AI doesn't really know is what your customers want. Because AI doesn't really understand the customer journey well. Well, it has the funnel metrics, obviously, but it cannot really go offline and talk to a customer. You have to do this.

**Mikhail Shcheglov** (00:58:54)

And that's the funnest part in the job. Because you don't do all of this, you know, better anymore. You're only focused on delivering the real value. And I don't think it's going to go away anytime sooner. What actually will happen is that the teams will be smaller, leaner, and faster.

**Aakash Gupta** (00:59:15)

So do you anticipate that the ratio of PM to engineer is going to change from what it historically was?

**Mikhail Shcheglov** (00:59:22)

Yes, definitely. I think not only it's going to change, the lines are going to blur between what a product manager does and an engineering team or an engineering manager does. There's likelihood that they could overstep and be a support system. Because at the end of the day, if a product manager is an orchestrator of, let's say, the product quality and token budget, an engineer is an orchestrator of an execution quality and token budget. The same applies for the designer. Designer is responsible for the consistency of a design system. Which means that quality and token budget as well. So the boundaries between those roles would be very blurry.

**Aakash Gupta** (01:00:07)

So you're a CPO, you're thinking about maybe I need to create a new product team in a particular area. When I was a VP of product at Apollo, we would typically think about, okay, if we're going to create a new front end product area, we probably want five to seven engineers, we want a PM, we want a designer. When you're thinking about a new product area now, how do you think about staffing that?

**Mikhail Shcheglov** (01:00:28)

No, it's a great question. So I typically divide them into different groups. So the first group is high complexity and high error blast radius. I think for those specific domains, nothing has pretty much changed and it's all around monetization. It's all around algorithms like Search, ML, where a single tweak might have a dramatic impact on the conversion or on the outcome. Here you would need to have a dedicated owner. But for the remainder of the domains, like customer-facing domains, what I'm currently seeing is that teams can be easily scaled without adding people. You might have one product manager owning three, four domains across many platforms at the same time.

**Aakash Gupta** (01:01:26)

Okay. So the PMs you're hiring, they feel to me like... They're truly AI native PMs. Even if they're not building AI features, you're probably hiring people who are really AI forward. What's your process these days to hire PMs? How do you find PMs that are at this level of AI native that they can actually succeed in this environment?

**Mikhail Shcheglov** (01:01:47)

Great point. So I typically look at three things. I think the fundamentals haven't changed, but I also added additional qualifiers into the interview. So the fundamentals meaning problem solving and systematic thinking. Like if you could have both, you will adapt in any situation. But additional qualifier that I've added is a level of... Ah, craft when it comes to AI, right? How deep a product manager is in the AI? And there is a very simple way to test for this is I'm asking like, which of the use cases of your daily work you have automated using AI? And I get a spectrum of responses. If a response is on a level of, well, I'm talking with ChatGPT using like, I don't know, terminal, using like web interface. And so to me, that's kind of a low level of immersion or maturity when it comes to AI tool understanding.

**Mikhail Shcheglov** (01:02:57)

But on the other side, you might have a very advanced AI agent orchestrator, a product manager who has automated all of his professional work life, right, and build it entire using AIs and so on. And then I can drill deeper, like asking, like, how do you evaluate this? How do you make decisions on tools, on the brain, on the memory and scaffolding and so on? But I got to be honest with you, it's in the market where I operate, it's a rare skill set. So product managers who are able to effectively answer those questions, they get way more points.

**Aakash Gupta** (01:03:34)

You guys heard it from him, not from me guys. He is a CPO at one of the greatest companies I would say to work on, and he is running it in an AI native way. And this is the skillset you need, the skillset we taught today. If you haven't already, go play around with Hermes. Go play around with Open Claw. And if you're a CPO, steal Mikael's playbook. His team is operating at a level unlike many others. Mikael, if they want to learn more about you, get in touch with you, find your content, where can they go?

**Mikhail Shcheglov** (01:04:06)

Well, I do have a Substack newsletter. It's called Corporate Waters. You can reach out and get immersed in my thinking and the actual use cases. Outside of this, you can reach out to me directly over LinkedIn.

**Aakash Gupta** (01:04:21)

I highly recommend Corporate Waters. If you guys didn't know, Mikael and I did a really fun deep dive last year where he looked through all of the interviews he's done in his lengthy career, which by the way, before he was a GPM at Bolt, he was also an ICPM for over a decade at companies like Yandex. So he collected all that data. And we looked into what interviewers are looking for. So if you want to go see more information from Mikhail, you can find it in my newsletter or his newsletter. Thank you so much for sharing all this amazing sauce today.

**Mikhail Shcheglov** (01:04:54)

It was a pleasure, Akash. Thank you for having me.

<!-- sponsor -->
**Aakash Gupta** (01:04:56)

The biggest thing is that Mikael agreed to open source the information that he used to build all of this. So go check the link in the description for the GitHub repo on his profile. You can fork that and you can begin building this company I hope you learned as much from today's episode as I did. If you can do one thing that's totally free that would help the show, it would be to check that you're following on Apple and Spotify podcasts, check that you've left ratings We're trying to make better and better podcasts. After two years, we think we've gotten something pretty good going. What we can do to make it even better, who else we should interview, and we will put on the best shows we possibly can. Finally, don't forget my offer for the bundle. You get an entire year of my paid newsletter, plus my favorite AI tools, Bolt Up News.

<!-- sponsor -->
**Aakash Gupta** (01:05:57)

Airtable, Speechify, Descript, Magic Patterns, Linear, Dovetail, Arise, and Mobbin. That's $27,000 worth of value for just $150. So check that out at bundle.akashgu.com if it interests you. And I can't wait to share our next episode soon.
