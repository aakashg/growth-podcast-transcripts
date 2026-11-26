---
title: "What an AI-Native Product Team Actually Looks Like at Salesforce"
subtitle: "I sat down with the guy who runs the 700-person org behind Salesforce AI."
date: "2026-11-03"
host: "Aakash Gupta"
guests: ["Jayesh Govindarajan"]
speaker_names: "substack"
substack_url: "https://www.news.aakashg.com/p/salesforce-ai-native-product-team"
youtube_url: "https://www.youtube.com/watch?v=_jBa_YEobGI"
duration: "00:57:29"
word_count: 9491
source: "Substack episode transcript (aired audio)"
sponsors:
  - name: "Ariso"
    url: "https://ariso.ai/aakash"
  - name: "Customer.io"
    url: "http://customer.io/productgrowth"
---

**Sponsors:** This episode is brought to you by [Ariso](https://ariso.ai/aakash) and [Customer.io](http://customer.io/productgrowth).

# What an AI-Native Product Team Actually Looks Like at Salesforce

*I sat down with the guy who runs the 700-person org behind Salesforce AI.*

**Jayesh Govindarajan** (00:00:00)

You created this new term, ADLC. Yeah. If the software you're producing is not just an internal piece of software, but it's an agent, how do you build it? How do you test it? How do you evaluate it? How do you deploy it?

**Aakash Gupta** (00:00:11)

So what I want to do is kind of build people a recipe for becoming more AI-native. I feel like at the base, we've covered that tool layer.

**Jayesh Govindarajan** (00:00:18)

We are all in Slack all the time. That is really our primary interface and how we work together with each other.

**Aakash Gupta** (00:00:23)

The next layer is roles, and you just talked about it, PMs, and you also referred to it with evals. A lot of people are wondering, what is the future of the product trio? The PM, designer, and engineer roles, they all seem to be converging on

**Jayesh Govindarajan** (00:00:37)

top of each other. The lines that we draw don't really exist. I think we create them in our own heads and then we specialize around them.

**Aakash Gupta** (00:00:44)

I think that third layer now is the life cycle that all of this is under. I think the very last component at the very top of the pyramid is probably where you spend a lot of your time. How engineers, product managers, and executives who are really setting the strategy of what we're working on collaborate to build a roadmap.

**Jayesh Govindarajan** (00:01:02)

One piece of advice I have always is

<!-- sponsor -->
**Aakash Gupta** (00:01:08)

Before we get into today's show, please take a second to check that you're subscribed on YouTube and following on Apple and Spotify podcasts. If you want access to all of my favorite AI tools, I've gotten them to give you an entire year of their paid plans. Check out bundle.akashg.com for an entire year of Bolt.new, Airtable, Speechify, Descript, Magic Patterns, Linear, Dovetail, Arise, and Mobbin. And now, into today's show. Jayesh Govindarajan has spent over 25 years in the tech industry, rising up from being a software engineer to leading a huge 400-person engineering org at Avaya, starting his own four-person startup which was acquired by Salesforce, and now has worked his way up to leading a 700-person org which is responsible for Salesforce AI, And agent force. So he has a ton to teach you about how to build an AI native company, an AI native engineering team, and an AI native product team.

**Jayesh Govindarajan** (00:02:16)

Jayesh, welcome to the podcast. Thank you. It's a pleasure to be here.

**Aakash Gupta** (00:02:19)

If someone doesn't know you, can you walk us through what is the org you lead today? What are they responsible for? What do they do?

**Jayesh Govindarajan** (00:02:26)

Sure. So I lead the broader AI engineering org at Salesforce. What that means is we set the strategy direction, build and operate AI systems that span predictive AI, generative AI, and now agentic AI. Basically three flavors of AI that deeply embed into the Salesforce stack, enable our customers to change how they work using predictive AI at its core, generative AI at its core, and now building agents for many, many of our customers.

**Aakash Gupta** (00:02:54)

So you've been working on AI and AI products for over 20 years. What does it look like now here at the end of 2026 to be operating like an AI native organization?

**Jayesh Govindarajan** (00:03:07)

That's a great question. I'll color this based on kind of what we're doing at Salesforce, how we're organized, how we're structured. I think there's no better example of an AI native team than one that is building the foundation of an agentic system that Customers used to build their agents on. So broadly, the last two and a half, three years have been an incredible whirlwind of agentic systems as our customers have sought to become an agentic enterprise. And all of that sort of is We have this underlying agent force, which is our harness that we built about two years ago before the name harness came along. So from an AI native perspective, the way the team is structured is designed to be able to build harnesses, Build models to be able to use these models in context of a harness. And then I'll talk more about this later, this emerging life cycle of an agentic system that we like to call ADLC, which is how do you build an agent, how do you test an agent, how do you evaluate an agent, how do you observe an agent in production?

**Jayesh Govindarajan** (00:04:11)

So these are tools and systems that we build that our customers use to go build their own agents for the scenarios and use cases that they use it for.

**Aakash Gupta** (00:04:22)

So how has your organization changed in the last couple years? We see everybody talking about Cloud Code and Cursor. We see people talking about agentic coding really being the first breakthrough in AI that's really transformed the organization. What has that meant for the roles and types of people in your org?

**Jayesh Govindarajan** (00:04:43)

Great question. So I'll take a step back first. We need to color this from the lens of the kind of work people do. So we have teams that basically build and train and tune models. Their world has changed considerably given the kinds of models that they're tuning and Training and relying and working, partnering with Frontier Cloud, such as OpenAI, who is a great partner of ours, Anthropic and Gemini. That world looks a certain way. And then there's a team that is moving really fast and building the harness technologies, which is Which is how context gets engineered into an agent, which is how tool calling happens within an agentic framework. And these are all tools that we build within the agentic system. That team has a certain rhythm of operating with the tools that they have. How do you evaluate them in production at scale? How do you observe them?

**Jayesh Govindarajan** (00:05:32)

What happens when a long-running agent, a conversation is going off the rails? How do you correct it? How do you bring all of that sort of system back? That's sort of the three big layers. And if you look at my org chart, that's kind of what it looks like. I have a team that's responsible at the model layer called the AI Platform Team. And there's a team that's about that, which is building harnesses, which is building memory systems for harnesses. And there's a team on top of that, which is the whole ADLC and agent optimization team. And I think... All three teams are working very differently than they were before. We are obviously very AI-pilled here. Within our team, we use Cloud, we use Codex for our development processes. We are all in Slack, all the time. That is really our primary interface on how we work together with each other, how work gets done within a team and across teams.

**Jayesh Govindarajan** (00:06:33)

Increasingly, we are bringing some of our customers also into Slack using this feature called Slack Connect. Where they can actually work with us directly on some project. And that's kind of the communication part that's changed considerably with Slack at its core. And one of the great things about Slack is you can basically bring in your agents to come do work on your behalf. And we'll We'll get into more of that. But at a high level, our world has changed in every aspect. How we design products, how we work with customers on iterating on what it is that they need to do, that we need to build, how we get feedback. And then how do we break that into tasks? And then how do we get agents to help us with some of these tasks? I think broadly in one sentence, I'd say we've had people change how they think about work.

**Jayesh Govindarajan** (00:07:24)

And that change is, in essence, how do you manage a team of agents versus doing the work by hand? Does that make sense?

**Aakash Gupta** (00:07:32)

Yeah. I used to think I had a retention problem. Turns out I had a messaging problem. I was sending the same onboarding emails to every new user, whether they activated on day one or never logged in again. I had no idea who was slipping or why. Customer.io changed that. Every message I send is now based Triggers. Timing. Copy. [music] Even branching logic. And when I want to know how something is performing, I just ask the agent directly and it tells me what to do next. They also have an MCP server, which means AI tools like Claude can see directly what's happening in your customer.io workspace. Your segments, your customer data, So instead of explaining your business context every time you need help, Claude already knows it. Notion used Customer.io to personalize their onboarding and hit nearly 50% open rate, improved conversion by 6-7% with localized campaigns, and pushed open rates up another 20%.

**Aakash Gupta** (00:08:37)

The idea is simple. Customer.io helps you deliver more impact from every message you send. If you're a PM or founder and your onboarding is still one-size-fits-all, try Customer.io at Customer.io.

**Jayesh Govindarajan** (00:08:48)

Here's the problem with most AI tools.

**Aakash Gupta** (00:08:49)

They just sit there waiting for you to prompt them. You do all the remembering, they do the typing. Ari from Ariso flipped that for me. It connects to my email, calendar, Slack, and it works the other way around. It comes to me. Monday morning, there's a briefing waiting. Before a call, it reminds me what we covered last time and what I promised to send. When a follow-up slips, it nudges me before the other person has to. Every commitment, every thread, every contact, tracked and organized without lifting a finger. And because it has continuous memory, it actually gets smarter the longer I use it. It's not a chat window. It's one AI partner that knows my whole working life, and it keeps me prepared for all of it. If you're tired of being your own chief of staff, try Ari at ariso.ai.akash. That's A-R-I-S-O dot A-I slash

**Jayesh Govindarajan** (00:09:32)

A-A-K-A-S-H.

**Aakash Gupta** (00:09:34)

You mentioned a bunch of tools there, so I want to dive deeper on those tools. And from your perspective at the executive layer, when do you decide, okay, we need to get this tool into the organization? What are the proof points you need to see externally? How do you roll out a new tool? Let's say you talked about orchestrating agents. The new craze right now is GrokBot or HermesBotMode. So when you're evaluating... Okay, do I need to bring GrokBot into my organization? What is the thought process you're going through?

**Jayesh Govindarajan** (00:10:06)

Yeah. So firstly, I think there is, we have to acknowledge that tools are moving at a rate that is unprecedented. There's no doubt about that. What is that? That implies that one cannot make a bet forever, right? I think you need to make bets and you need to give them some space to play out. And then you need to back something and push that sort of tool and technology through, but remain open to change as an example. We started off using Cursor. That was the primary sort of interface of choice for engineers. Then Claude happened. And this sort of family of agents doing work, talking to each other, getting it done, In particular, cloud code, the harness for coding became something that our engineers loved using. The way I look at this is you need to give people a choice to pick the tool they want.

**Jayesh Govindarajan** (00:10:57)

And often the best engineers, the best PMs pick the best tools to get the job done. And then you look at data. Then you look at what's actually driving adoption more. And then you lean towards the best practices which emerge from just real usage on a daily basis.

**Aakash Gupta** (00:11:14)

So it sounds like you're of the camp that don't prescribe, okay, guys, we're all going to use Cloud Code now. Give people access to multiple sets of tools, whether that's Codex, Cloud Code, Cursor. If there's something new that comes up, give them access to that. And don't be super restrictive on your IT, corporate security policy. Is that fair?

**Jayesh Govindarajan** (00:11:38)

Be very, very careful about corporate security, but be open about the tools that are given to users as choice. So every single tool in the Salesforce ecosystem has to go through security. So we make sure that all the security Security criteria is met, but we give our teams a choice for a while, and then we watch to see what works. And often the best practices emerge from real usage. And as I said, things keep changing. It used to be that you'd, you know, The IDE of choice, I don't think it's changed in a decade from an engineering perspective. The tools that a PN has used, Excel, Docs, Google Docs, Figma, these tools haven't changed a whole lot in the last decade or so, but now they have. And not only have they changed, the change isn't singular. It's going to keep evolving. So I think you need to think of not just where you are on the graph, but what the slope looks like.

**Jayesh Govindarajan** (00:12:37)

And try to hug the tangent as the slope changes continuously. And the way to do that is to have a process and a methodology and some trust that your teams will be able to figure it out. So long as you give them access to the best tools that are available, and then watch what works, what doesn't. And that sort of served us quite well, actually.

**Aakash Gupta** (00:12:56)

One of the most interesting things that I think Salesforce has done recently is this idea of being headless. And you guys just recently announced Cloudforce. So basically where your users for your $60 billion revenue or $50 billion revenue business, they used to live inside your tools. They used to live inside Salesforce.com. But now increasingly they're living inside Cloud or like you mentioned, they're living inside Slack. What does that transformation look like on the ground for people internally? How do they make that shift towards living outside of the SaaS products they used to buy and then more living inside of these centralized operating systems, whether they're claws?

**Jayesh Govindarajan** (00:13:41)

Liberating, in one word. I think a lot of the Salesforce magic was never in the interface, although we did that well. It was always in the layer that powered the interface. So when we say headless, all of the metadata, all of the business logic, All of that is actually captured in the API. And when Cloud came along, it's really an unshackling of these subsystems that do powerful things, understanding what the flow of sales process looks like that ends up With a 70% probability of a close or a ticket resolution looks like that has an 80% chance of being resolved successfully with this ability to bring in a human at the right time. These are powerful workflows that have been perfected over decades. They've customized it for their own needs. What Headless does is it lets our customers bring that into Cloud using skills that we wrap these around and basically use it in any context that they want.

**Jayesh Govindarajan** (00:14:43)

So Cloud is doing this bit of bringing all of these things together into Cloudforce with this ability to build an interface that is very custom for their need. Again, I think the magic Was never just in the user interface. It was what was underlying the user interface. And what Cloud basically does is helps you code one up for your bespoke need, which is very specific to what you want to do. And you're basically using the same technology in the back.

**Aakash Gupta** (00:15:14)

So what I want to do is kind of build people a recipe for becoming more AI native. So we kind of talked a little bit about, you need to hug the tangent of how tools are adopting. Then we talked about you need to let people operate inside these centralized tools like Claude and Slack. And the first sort of thing that I worry about when somebody's using Salesforce in Claude is that it's not really as deterministic as Salesforce was. If you think about it, the way Salesforce is identifying how much open pipeline you have, there's clear data fields that it's referencing. But we all know using LLMs, they can be They can have variations, but you can't really have two pipeline numbers, right? You can't have 25 million and 20 million. Which one is it, right? You actually need to know. So if people are moving into these tools, how do you build the harness in the right way or how do you use Claude or Slack in the right way so that you can get to a ground truth?

**Jayesh Govindarajan** (00:16:15)

Yeah, so with AgentForce, we saw this need arise just as soon as we launched, which is this need to bring in some degree of control and determinism to an agent specification. What does that look like? A language that you can describe your agent in, which then translates into tool calls. It translates into context lookups, and it translates to reduced hallucination because it's relying on time. We designed the language around it called AgentScript, and basically it transpiles to plain English. So you can describe what an agent should do in plain English. It transpiles to AgentScript, which then has all the logic and the metadata for tool calling for getting the right context in the right place. That reduces solutionation rates by a massive, massive amount because you're not using Claude to generate code when there is already a piece of code on an API that is exactly what you want deterministically every time, tried, tested, and good to go.

**Jayesh Govindarajan** (00:17:22)

You are still using Cloud to bring the right systems together for that sort of task, right? But that's kind of the magic, which is in the agentic world with agent force, you can bring in more than that. You can bring in a set of controls with agent script to be able to pull all of that together.

**Aakash Gupta** (00:17:39)

So in our recipe card, it sounds like what's really important is giving the connections to the right data. But on top of that, Defining how those tool calls work and building the right skill files so that when Claude makes those tool calls, it does it correctly.

**Jayesh Govindarajan** (00:17:56)

Perfectly. Perfectly right. One other thing I would add, which is a really important... Insight that we gleaned away is if you look across my teams, we have teams that think eval first by nature. These are all the data science teams that have been doing predictive AI and generative AI and then into the agentic world. For them, they are what I call eval native. They look at a system probabilistically. They understand that it's not going to work all the time. So their test cases or evals that they've written tied to outcomes is a superpower now. And there are other teams that are more sort of code-focused, engineering-focused. They've built the infrastructure. They've always worked in the deterministic world. And very quickly, you asked, you know, earlier you asked, what are the big changes that you're seeing with the teams? This is one of the changes we're seeing.

**Jayesh Govindarajan** (00:18:52)

We're seeing a lot of people becoming eval first. And that means thinking through not just the test cases, but outcomes. Outcomes and having these custom scorers using both LLMs and other models to score the output. And these are not generic. These are very specific to the agent you're building or the code you're writing. This is the other sort of, this is a cultural shift. It is a tool set shift. It is a mindset shift in how you sort of design software that is probabilistic and you want it to work every time. So I'd add one more, which is the eval part around it.

**Aakash Gupta** (00:19:27)

Let's circle back to evals in a second. I want to close the tools component of this with Slack. Because I'd say a lot of people listening who are trying to come up with an AI native organization, they're probably still stuck in the Microsoft Teams world. They haven't, they don't, Even understand why Slack is important or what it enables. So can you talk to me about, as far as I understand it, people are spending, like you said, 50, 60% of their time in Slack now, whereas it might have been in an IDE before. So how do you get that setup correct? And what is involved in that setup so that you're doing so much out of Slack?

**Jayesh Govindarajan** (00:20:07)

That's a great question. I use Slack every day, and I am just a mad fanboy. So two things. One is, what's the one place that people are available asynchronously all the time? It's Slack. In most enterprises, that's where people are. That's where work is organized. That's where conversations around work are organized. That context is gold dust. Especially taken longitudinally over the long period of time, that just is the amazing bit of missing piece that's needed for getting something done. Serendipitous discovery is possible in such a system. Slack will routinely find someone that has that answer in some channel that is a public channel that I had no idea existed. And that's context for an agent to work on. So what does the toolset look like? It looks like a great implementation of Slack within the organization. It is a Slack where people are using it every day, which is super high utilization, which is leaving a lot of data traces behind.

**Jayesh Govindarajan** (00:21:15)

And then it is plugging in this agentic toolset within Slack. We ship with one that is magical called Slackbot. If you haven't used it, please do.

**Aakash Gupta** (00:21:24)

I want to take a second to talk to you about the fourth cohort of LAN PM Job. I trained 30 students in cohort one, 50 students in cohort two, and 75 students in cohort three. And I am bringing back a program for cohort four. It starts in August and it lasts Three months where you're going to have intense sessions, a Monday morning session where I go over your resume, behavioral interviews, LinkedIn.

**Jayesh Govindarajan** (00:21:46)

On top of that, Bart Jaworski is

**Aakash Gupta** (00:21:47)

going to be teaching you the PM fundamentals in 2026, how to write AI PRDs, how to AI prototype with So it is a full package. It is three courses in one for one low fee. So join at landpmjob.com. [music] Agents and assistants are browsing, shopping, and transacting alongside humans, while fraudsters use AI to build faster, cheaper, and more sophisticated attacks. Technical teams need device intelligence that evolves as quickly as these attacks do.

**Jayesh Govindarajan** (00:22:35)

Fingerprint is exactly that.

**Aakash Gupta** (00:22:37)

Accuracy is the number one reason customers choose fingerprint because their device intelligence goes deeper than identification alone. Resolving visitors with precision that holds up through spoofing and evasion attempts for months at a time. Fingerprint collects more than 100 signals across devices, network, and behavior to build a single identifier. Then provide signals like bot, agency, proxy, and VPN detection to give technical teams a complete picture of risk.

**Jayesh Govindarajan** (00:23:03)

They ship hundreds of product updates a year,

**Aakash Gupta** (00:23:05)

so they adapt first as browsers update, privacy requirements change, and fraud tactics change. With one API call, teams can get this running in minutes. Over 6,000 companies rely on fingerprint every day. Join them now at fingerprint.com. Imagine learning AI product management, AI product strategy, AI product leadership, advanced PM with cloud code, all from frontier leaders at OpenAI, Anthropic, and Google for less than $10 a day. Actually, you don't have to imagine it. That's exactly what Product Faculty's AI Builder Fellowship gets you. One yearly membership, six live cohorts. Not recorded videos or another content library you never finish. Real live sessions with frontier AI leaders, hands-on AI build labs, executive Insight sessions, capstone projects, unlimited retakes, and continuous access to new programs as the AI landscape evolves. You'll also get every new certification they add while you're a fellow at no extra cost. The goal is simple, help you master frontier AI skills to become an AI native product builder and operator, not just someone who talks about AI.

**Aakash Gupta** (00:24:20)

Purchased separately, these programs are worth more than $19,245. The lowest price certification alone starts at $2,700. But founding members can join the entire fellowship for less than $3,600 per year. That's less than $10 a day. Soon, the price increases to $5,000 a year. So if you're serious about becoming the person your company turns to for AI, this is one of the highest ROI decisions you can make this year.

**Jayesh Govindarajan** (00:24:46)

Join the AI Builder Fellowship at productfaculty.com. You can ask it questions. It can orchestrate other agents for you. It can bring you the right people. It can send emails. It can send other Slack messages. So you're basically building your agentic environment. Work environment within Slack. And you can build into being in third party agents as well. So that's sort of the tool set. From a developer perspective, we use Slack code quite a bit. For simple apps, you can write the spec there You can actually build a simple UI in there. How cool is it for a PM to be able to go create a small mock in a Slack thread with their customer and just ask him, is this what you had in mind? Versus writing a PRD, getting an engineer to go build it and then create a link for it and send it back to the customer.

**Jayesh Govindarajan** (00:25:41)

The customer kind of looks at it and goes, eh, not really what I want. So basically this whole cycle is sped up exponentially and it's just a joy to work

**Aakash Gupta** (00:25:49)

So I'm trying to build this recipe card. I feel like at the base, we've covered that tool layer. The next layer is roles, and you just talked about it, PMs, and you also referred to it with evals. So a lot of people are wondering, what is the future of the product trio? The PM, designer, and engineer roles, they all seem to be converging on top of each other. So... We humans are notoriously bad at predictions, but what are you seeing on the ground right now? Are you seeing when you're staffing up a product team that you need as many PMs as before, as many designers as before? How are you thinking about that?

**Jayesh Govindarajan** (00:26:27)

Well, that's a big question. And I think it's a really important one. Having been an entrepreneur for, I think the one thing that becomes very clear to you when you are an entrepreneur is that these lines that we draw don't really exist. I think we create them in our own And then we specialize around them. So then they do become real after a point. I think what the tool sets that we have available to us, what the large language models and the agents can do effectively now means that those lines are being blurred. They're being blurred in ways that are incredible to see. As an example, If you're a PM, if you're an engineer that has a customer-first mindset, and many do, many don't want to build systems that are never going to see light of day. They want to build systems. They want to put their heart and soul into things that has an impact that customers will use every day.

**Jayesh Govindarajan** (00:27:22)

How can they test that? Well, if they have customers that they can work with directly, they can start putting products out in front of them, get direct feedback. Do you need a middleman? I don't think so. Conversely, if you're a PM, your bottleneck may be waiting for that engineer. You've logged in the request for that engineer written a PRD and the engineer is working on something that was written before and you're waiting. You don't have to wait anymore. The product development lifecycle can be sped up significantly more. And now the bottleneck is, can you find customers fast enough to And can you get to customer success, concept market fit, product market fit quickly? And one of the great things about working at Salesforce, I truly believe this, and you've seen here the energy here at Dreamforce, we just have incredibly loyal customers and we couldn't be more thankful for that.

**Jayesh Govindarajan** (00:28:18)

You've seen the trailblazers that have come here. And who are these people? These are people that started out in, you know, You know, roles that were sort of fairly junior and implemented Salesforce and then grew with the company in implementing this. And now our customer service officers of the company, tremendous loyalties. And it's really easy for us to go talk to them because of the trust that Salesforce has built over decades and say, hey, will you try this? We've built something. We want some feedback. Will you try it? And it's super easy for us to get 10 pilot customers for anything we do. And we have that trust that once we build it, we will build it right. And we will make them successful with it no matter how long it takes. So I think that sort of bottleneck, you know, where you need to go find customers is completely non-existent and say, So then what's the new bottleneck?

**Jayesh Govindarajan** (00:29:12)

The new bottleneck is, are you able to cook with them fast enough? Are you able to get feedback fast enough? Are you able to test the concept fast enough? And yes, you have Slack. They can join your Slack. We can start to build simple demos in Slack. And if they love it, all you have to see the hard signs, count them, and go, great, let's go get this built out. And then we have 10 pilot customers, and then we go from there.

**Aakash Gupta** (00:29:39)

So just five years ago, that process took weeks, if not months, right? Executives and product managers would go off and they'd figure out this is the direction. Once they got buy-in from everybody, designers would create the prototype. Then it would finally get put in front of customers. Usually a user research team would be responsible for putting that in front of customers. So we had like Three specialists touching a prototype and putting it in front of customers. Now engineers can do that. Should engineers be doing that? When should you have a PM or a designer or an engineer be doing these different tasks?

**Jayesh Govindarajan** (00:30:23)

I mean, ideally we have a group that is doing it with customers. It's faster, it is more durable, and they each bring their perspective to design. The point is that the tools make each of them operate in each other's domains. Up to a degree, there is of course specialization. This ability to abstract out requirements by talking to four customers, having insight, having looked at the market where the industry is going. That's something that the PMs, especially an experienced PM can really bring to the table. Conversely, An engineer can just build it right the first time and now super fast, given the tools that are available to them. Same with designer. So we each come from a place where there is a strong skill set and an experience that we bring to the table. What the toolset's doing is that it's saying that you're not in that silo anymore.

**Jayesh Govindarajan** (00:31:19)

You shouldn't box yourself in that silo. That you can go take the first step with the customer and then pull in the expertise as needed. A good example here is that often you build something quickly, you get feedback on it quickly. The journey from zero to a thousand customers is a very different journey from a thousand to ten thousand customers where failure modes have Significantly bigger impact when you have 10,000 customers, right? So that journey is very different and you need different skill sets to be able to bring that into the fold. Would you over engineer something for 10,000 customers day one? You wouldn't. So what this does is it basically increases the pace at which we can innovate with our customers. Innovation comes from two places. It can come from groundswell, bottoms-up innovation based on new technologies that are coming And God knows we've seen enough of that.

**Jayesh Govindarajan** (00:32:15)

But when that's married with the customer need that exists, which you can quickly test with customers, and that's where the magic is. And those two things kind of come together. So an engineer that has a very deep understanding of tech And has an opinion on where this is supposed to go. Doesn't quite know whether the market is there or not. Can test it out. And can they bring a PM along? Sure. We're sort of designed that way. We have a scrum team. The smallest unit of work in our organization, my team, is a scrum team. So you have a PM. You have an engineering lead. You have a few engineers. You have a fractional designer. And they can go together and go get this sort of cycle sorted out pretty quickly.

**Aakash Gupta** (00:32:54)

Okay, so we still have that traditional unit of a scrum team. As you're making the shift to AI Native, do the ratios change or do the job descriptions change? It sounds like mainly the job descriptions change in that you're more in each other's lane, but the ratios are the same?

**Jayesh Govindarajan** (00:33:11)

I think it's early days. I don't think ratios have changed a whole lot. I don't think I've seen that happen. I've seen work bleeding across a little bit, which is great. And I expect to see more of that. What I really look for is the pace of zero to one. How quickly can we go from an idea to an implementation of that idea? And is it done in vacuum? I can go from an idea to implementation really, really quickly just by myself on my laptop with no feedback from anybody. Not a great idea. Don't recommend we do that, right? But if you're going to work with a team, if you have a set of customers, how quickly can we iterate with them? And I think our velocity has gone up significantly. We are producing more software than we ever were. And this is kind of a direct result of teens using the tools, having a democratic approach to the tools, and then bringing customers into the fold so you can integrate fast.

**Aakash Gupta** (00:34:15)

So what I've been talking a lot about in my newsletter and podcast is how a lot of PMs need to become AI PMs. AI PMs, compared to a regular PM, have two really important skills. Number one, AI prototyping, which you just talked about. Instead of waiting on designers and engineers to create prototypes, they prompt the AI themselves. In a Slack chat with the customer, they directly get feedback. Even before they're sharing it with a designer or engineer or UX researcher. And the second skill is AI evals, which is that they really become the subject matter expert to define, hey, this is our golden data set. These are the 100 input prompts. This is what I expect the output prompt to look like. It should be this quality. This output prompt would not be at quality. This would be an 8 out of 10. This would be what a 10 out of 10 output prompt looks like.

**Aakash Gupta** (00:35:12)

Would you say that's accurate? To become an AI native org, do you need to hire these PMs that have these new skills? And are those the right skills?

**Jayesh Govindarajan** (00:35:20)

You are speaking my language. This is exactly the two things that are absolutely key. Doing that upfront really is the magic bullet. I mean, I couldn't agree with you more is the short of it. I think these two skills are invaluable in PMs. So yeah, short answer is yes.

**Aakash Gupta** (00:35:41)

We need to do more of that. So we've built the tool layer. People now understand the roles. To close off the role layer, how do you hire this new AI PM? What are you looking for?

**Jayesh Govindarajan** (00:35:54)

One is nothing to do with technology. It's agency, which I think is going to be the new short supply thing. And beyond that, I would say just a deep theme What I mean by that is a mindset where you're not off doing the work, but you're sort of teaching an agent to do the work. Maybe do it once and then teach an agent to do it so that from then on forward, you are super fast in how you're responding to things and iterating on things. So that's one sort of skill set to look for. Second one is some degree of... Skepticism with the toolset where you love the power it brings, but you don't always believe it, right? The best ones still have that craftsmanship mindset. They're not producing AI sloth. They're putting the name to it and they do not like to put a name to something that has AI slop.

**Jayesh Govindarajan** (00:37:01)

AI slop comes in many different forms. You know, prototype that looks like any other prototype, AI slop. People just checking the box by sending a really long document, AI slop. So these are sort of clear do's and don'ts. I think there's no substitute for craftsmanship. There's no substitute for agency. I think those are two really important things to look for. Like, do they have attention to detail is a good example of craftsmanship. And then it's tooling. It is, how do you translate that skepticism into test cases and evals that are failing? When you build the system that you're building or testing the system that you're testing. Can you set a bar on what good looks like? Because that's what translates into evals. And then, like you said, I think access to all the prototyping tools, which I think is the easy bit now. I think that pretty much everyone gets.

**Aakash Gupta** (00:38:00)

Yeah, I think the tools are pretty easy. The roles we've given you some more clarity on. I think that third layer now is the life cycle that all of this is under. And you created this new term, ADLC. Yeah. Not the SDLC that we all know. So can you define those two terms for us and explain to us what makes the ADLC different?

**Jayesh Govindarajan** (00:38:20)

Sure. So SDLC is the software development lifecycle, which we all know and love that have been building software for years. ADLC is an equivalent for the agent development lifecycle, if you will. If the software you're producing is not just a deterministic piece of software, but is an agent, How do you build it? How do you test it? How do you evaluate it? How do you deploy it? And then having deployed it, how do you observe it so that it continually improves? So these five elements are taken together The Holy Grail, of course, is an agent that you've built and it's in production and can self-heal to some extent. And I'm not talking some fancy rocket science sci-fi stuff on self-healing. I mean simple things. Like you have an agent that's working fine in production, starts to drift a little bit. Why does it start to drift?

**Jayesh Govindarajan** (00:39:19)

Because it's grounded on some data on refund policies that just got changed. But somebody wrote it in a way that It's not very clear. Somebody updated the document. The agent's not working. Are you sending refund checks that are bigger than the amount that was needed? Can it self-heal? It can. It needs to detect what context was changed, whether that context was changed the right way or wrong way. That's the knob that you want to get to. You want to get to a point where if you've designed this right, there are two loops. There's the inner loop, which is you conjuring up an agent from your imagination, working with the customer to make sure that that's what they want, and then going and building it off. And then deploying it in that environment. And the outer loop, that journey starts once the customer starts to use the agent.

**Jayesh Govindarajan** (00:40:11)

What is the lifecycle once an agent is live? How do you evaluate in production? How do you update the agent in production? What does that loop look like? That requires a completely new set of tools that haven't been built or imagined. We're starting to see some of that come in. But in our world, that looks like a testing center for agents. That looks like an observability center for agents. That looks like we launched this at Dreamforce yesterday called Optimization Agent. It's the one that looks at all the agents in your AgentForce agents that are running in the org and looks for opportunities to optimize. Maybe by adding new context or refining a prompt that is not working great. So think of this agent as like this agent that's observing all the agents and looking to optimize. So that's kind of what I mean by the ADLC lifecycle, kind of playing on words with the software development lifecycle a little bit.

**Aakash Gupta** (00:41:08)

Does the ADLC only apply then if you're building agents?

**Jayesh Govindarajan** (00:41:12)

I think it's broader than that. I think it has to do with an AI development lifecycle, which has an eval mindset baked in, which understands that anything built on data can drift because data itself drifts. And then having the right tool sets to observe that drift in production and see if that drift can be corrected in production. Large scale AI systems predating agentic systems have this in droves. Like if you look at the search We are pulling all of that out and making it available at scale in this new To be able to understand what is drifting, to be able to be told what's drifting and then bring the human in to correct it, to steer it, if you will.

**Aakash Gupta** (00:42:18)

So it sounds like part of what is involved in the ADLC is moving a lot faster. If you were on a six-month ship cycle, it sounds like you need to almost go to a continuous deployment. It can self-heal whenever it wants cycle.

**Jayesh Govindarajan** (00:42:35)

Yeah, and I think there's a very good reason why the pace is this way. It's because often the substrate layer, things that you build on, don't change as fast as they are today. I think about it this way. The substrate layer for most software is a database. How often has the database changed? How often has the programming language to program the database changed? Hardly ever. SQL still exists. We are in a world where the substrate layer is a model itself and it's not staying still. It is evolving at a very rapid rate. The changes between what we saw in the current version So what happens to all the agents that you built that worked great on the previous one? You need to evolve them. You need to simplify them. And there are certain dimensions on which you need to simplify. Imagine being able to do that.

**Jayesh Govindarajan** (00:43:39)

With no ADLC. You have no test cases, no evals. How are you going to go flip the, you're just going to, if you didn't have all of that infrastructure built, the rate at which you move, the hugging of the tangent, if you will, it's not happening because you're mortally afraid of breaking something. But if you do, on the other hand, you can really go fast. And that's the mindset change.

**Aakash Gupta** (00:44:08)

Everything downstream has to change though then, right? Your product marketing, your customer support, everybody has to shift to this much more agile way of working. Some companies are still stuck in the past, right? They're still shipping every couple months. How does a company go from zero to 100, it feels like? How did they just completely turn around and how did you guys do it?

**Jayesh Govindarajan** (00:44:29)

Yeah, I think the first thing is, I think you nailed it. You have to be building and releasing continuously. You have to be doing that in discrete chunks that matter to customers. At the end of the day, we're shipping something that we want to have impact with customers, that adds value to customers. Release is just a packaging mechanism, is all it is. From every Scrum team needs to be pushing code and making changes to code as rapidly as they can, as safely as they can. This is the trade-off. The trade-off is you don't want to break systems. If all you're going to do is iterate rapidly, once you have the kind of customer base that Salesforce has, things start to break and then that slows you down even further. You want to be able to balance and do both.

**Aakash Gupta** (00:45:20)

People used to create lots of tech debt when they would switch to this way.

**Jayesh Govindarajan** (00:45:23)

Yeah, and often I tell our PMs, if you have tech debt on your teams, that's still your problem because you're going to eventually slow down and you won't know why because your engineers are fixing problems. And that means every engineer that's fixing a problem is not adding a new feature that the customer loves. So taking that into account, you have to account for what that means from a tech debt perspective. But for the first time, we can have agents help with tech debt too. How do you build this work we do with our amazing security team, this work we do with our release management teams for building agents that are specialized, that do code reviews? How do you pull a PR, a high-quality Quality PR really fast. What are the bottlenecks? The bottleneck is no longer writing code. The bottleneck is writing quality code, writing code that works all the time, having the test cases that fail before it hits production.

**Jayesh Govindarajan** (00:46:25)

These are now the bottlenecks, each of which, if you go really deep, you can start to build agents for and speed up by itself. Yeah.

**Aakash Gupta** (00:46:35)

Okay. So I think we covered the life cycle. I think the very last component at the very top of the pyramid is probably where you spend a lot of your time. How engineers, product managers, and executives who are really setting the strategy of what we're working on collaborate to build a roadmap. So what does that process look like? What does the planning process look like in this AI native organization? What do the different roles own?

**Jayesh Govindarajan** (00:47:03)

Great question. So let me take a step back first. I think at a high level, I'd say taste, judgment play a much bigger part than they did before. That's what forms the intuition on the broad Vector along which you want to move the organization, the team, the product. But I said broad vector. It's not a straight line, right? It's a broad direction. And then once you know what the broad direction looks like, you get a lot more refined using two mechanics. Mechanic number one is just getting customer feedback early. In whatever it is that you're building. And that feedback, as we determined earlier, isn't that hard to get anymore in a very visceral way. You can just put a prototype in front of them now. You don't have to have seven meetings where you're describing the idea. That is one dimension of getting that vector right.

**Jayesh Govindarajan** (00:48:00)

The second dimension is existing products that are in the market that are being used by customers and they're loving it, but they have some gaps. This is where sort of a four deployed teams are are incredibly useful in how they work with customers, not just to make them successful, but they are the first line of defense and see what our customers see. And because they're closer to product and they're part of the product, We have customer-facing engineers that work directly with customers. They bring back all kinds of feedback from paper-cut type things that shouldn't exist in the product, we should just fix it, to, oh, the way we thought about this particular feature Now imagine doing this at scale across many, many, many, many different teams. And you get a picture of how I don't know how that sort of looks like, but I feel like those are key things that we need to organize as a team.

**Jayesh Govindarajan** (00:49:10)

And from our perspective, as I said, we are in Slack all the time. We have great tools that summarize all of this, roll this up. We have fantastic reports We have a channel where all FDEs basically post exactly what's happening with the customer, what their pain points are, and is it a paper cut or is it a feature request? And we have PMs and engineering leaders looking at it all the time and matching it against that roadmap and seeing if something needs to change or we need to jump onto the customer side. We are working more with customers than we ever did before.

**Aakash Gupta** (00:49:47)

I want to return to that role there because you brought up the forward deployed engineer. It's got to be the hottest, sexiest new role in tech. And for my audience, it's the forward deployed product manager that's super interesting to them. What do you see? Are these roles replacing the traditional? Are they a supplement? How did they fit in to the broader picture we just described of engineer, designer, PM?

**Jayesh Govindarajan** (00:50:14)

Yeah, I think the reason the role exists is because we are deploying sophisticated technology and evolving that technology at a very fast pace. The pace at which we're building is not the pace at which the technology is being diffused. So we're solving it with expert humans in the middle. We are trying to catch up our customers and we're trying to catch up the diffusion rate of technology with the customer base. In a way that adds value to them, so it's righteous in that way, to the pace at which we're innovating within the company. That's the gap. And that's what we're trying to fill with forward deployed engineers, PMs, designers, whatever. Broadly, I think what that means is The main skill is twofold. One, really being able to immerse oneself into the customer's pain point. They bought us to solve a problem and then falling in love with that problem and then helping the customer solve it using the tool sets that are available to them.

**Jayesh Govindarajan** (00:51:20)

And often, maybe the tool sets are not sufficient. That's okay. The forward deployment team has the freedom to go find some other bit and be able to plug it in to make the whole work. And we've done that many times. Sometimes we build something custom with them. So do we need PMs there? Yes, because we just designed something custom with them. It'd be nice to have PM input on that, which has the added benefit at roadmap planning to see whether that thing was really custom, or do we think that All customers would need it. And if all customers would need it, how about we take a prototype, we already have one, and take it out to a bunch of customers and get feedback on it. So this sort of cycle of getting feedback in, bringing in PNs, designing it directly with a designer, or an engineer just working with a customer to go get it built out, making them successful, is really the lens that is different.

**Aakash Gupta** (00:52:16)

So what I'm hearing is that the forward deployed group is almost like doing a lot of this rapid prototyping on a custom scale, and then it brings it back to the core group to decide if we want to build it in the product for everyone. Is that right?

**Jayesh Govindarajan** (00:52:29)

That's right. Okay.

**Aakash Gupta** (00:52:30)

So you get to see a lot of customers who are going through this transformation from not AI native to AI native. They're basically hiring Agent Force to help them along that journey. What are the biggest mistakes that somebody who's watching this should keep in mind so that they can avoid those in their implementation?

**Jayesh Govindarajan** (00:52:53)

I'm a big believer in start simple. I'm a big believer in define value, then define metrics to capture that value and call it your ROI metric and get it built out end to end, scale it out, scale And then scale all. Often implementations don't take this flavor. It starts off as a whole full company transformation story and then very quickly breaks out into this massive plan across the board. And it creates a lot of pressure on the teams that are implementing, even customers that are trying to derive value. So I think one piece of advice I have always is start with your hardest problem. That's okay. But be very clear about what Value is going to look like. And then break it down into, we've talked about this before, clear ROI metrics, clear scorers on the agent, clear evals on the agent that tie to value and ROI.

**Jayesh Govindarajan** (00:53:51)

And once a team is Successful at building it. Keep in mind, this is technology that we have kind of built ourselves, so it's easier for us. But when I look at others building agents, I get the sense that technology isn't fully diffused. The teams that are implementing still need a lot of enablement. And what that means is starting with one success under the belt is super important. I'd say that is one key thing. The other one I'd say is there are a lot of variables when it comes to building the system. What models do we use underlying? Should one train their own model? Should one start with a harness? What is the role of implementing the right context? There are a lot of variables. And I'm also a big believer in saying that the very first implementation minimize the variables. Get the work done in the simplest way possible, lock amps razor, and then start to ask about what are the ways to make it more efficient.

**Jayesh Govindarajan** (00:54:55)

And there are many, right? The best ones that we work with start with two or three really critical implementations. And then they just go wall-to-wall with Agent Force. Deco, they were in Mark's keynote, and they're one of the customers I work with very, very closely. They're wall-to-wall Agent Force agents, all the way from the recruiting company based in In Europe, one of the largest recruiting companies in Europe, they have pre-screening automated with an agent that calls you and you can take an interview on a phone call. KeepState can ask questions, escalate to human, all of that data. They started with text, wall-to-wall, 17 different languages. They're deployed across Europe, and now they're going voice. So that's a good example of setting a high bar, but starting with one or two use cases and really going all the way and then expanding and going wall-to-wall looks like.

**Aakash Gupta** (00:55:53)

This has been a masterclass. Thank you. If people want to learn more about building an AI-native product team and organization, where can they find you online?

**Jayesh Govindarajan** (00:56:02)

Online, I am on LinkedIn. You can find me on LinkedIn. I'm on Twitter, Jay. And of course, you can find All About Agent Force on Salesforce.com. It's where I live pretty much all the time.

**Aakash Gupta** (00:56:14)

All right. Jayesh, thank you so much for being on the podcast.

**Jayesh Govindarajan** (00:56:18)

Absolutely. My pleasure.

<!-- sponsor -->
**Aakash Gupta** (00:56:19)

All right. I hope you learned as much from today's episode as I did. If you can do one thing that's totally free that would help the show, it would be to check that you're following on Apple and Spotify podcasts. Check that you've left ratings and reviews on those platforms. Check the I hope that you're subscribed on YouTube, leave a like and a comment on this video, and then share it with your friends. We're trying to make better and better podcasts. After two years, we think we've gotten something pretty good going. So let us know what we can do to make it even better. We should interview and we will put on the best shows we possibly can. Finally, don't forget my offer for the bundle. You get an entire year of my paid newsletter. Plus my favorite AI tools, Bolt Up New, Airtable, Speechify, Descript, Magic Patterns, Linear, Dovetail, Arise, and Mobbin.

<!-- sponsor -->
**Aakash Gupta** (00:57:08)

That's $27,000 worth of value for just $150. So check that out at bundle.akashgu.com if it interests you. And I can't wait to share our next episode.
