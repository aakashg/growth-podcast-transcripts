---
title: "A FAANG PM's Guide to Practical AI Evals"
subtitle: "Mahesh Yadav worked at Google, Amazon, Meta, and Microsoft. Today he walks you through how to build AI evals practically in Microsoft Foundry."
date: "2026-11-24"
host: "Aakash Gupta"
guests: ["Mahesh Yadav"]
speaker_names: "substack"
substack_url: "https://www.news.aakashg.com/p/practical-ai-evals"
youtube_url: "https://www.youtube.com/watch?v=MnGPn36NgK8"
duration: "02:15:26"
word_count: 21997
source: "Substack episode transcript (aired audio)"
---

# A FAANG PM's Guide to Practical AI Evals

*Mahesh Yadav worked at Google, Amazon, Meta, and Microsoft. Today he walks you through how to build AI evals practically in Microsoft Foundry.*

**Aakash Gupta** (00:00:00)

What is the compensation specifically that AI PMs can make? If you don't bring people with these skills and compensate them, the kind of compensation I'm talking about, you are not going to get the leverage in this new AI world, which I think is an existential crisis for pretty much Agents, creating agents, kids play now. It's like Claude Kovac can build any agent. It's basically a skill at this point, but evaluation is stopping people to go to production. Out of all the agents created in companies, only 15% are going in production now. Meet Mahesh Yadav, former AI PM at Google, Amazon, Meta, and Microsoft. Half of your team is new to AI or even 80% they are new to AI. And if you cannot be the fountainhead or brain for this AI team, you're not going to ship products which succeed in customer hands.

<!-- sponsor -->
**Mahesh Yadav** (00:00:45)

So if you're that person, you're that mid-level PM in that geography, what is Mahesh's roadmap? How do I go from 80,000 euros to 1 million USD? So I think first we need to understand Before we get into today's show, please take a second to check that you're subscribed on YouTube and following on Apple and Spotify podcasts. If you want access to all of my favorite AI tools, I've gotten them to give you an entire year of their paid plans. Check out bundle.akashg.com for an entire year of Bolt.new, Airtable, Speechify, Descript, Magic Patterns, Linear, Dovetail, Arise, and Mobbin. And now, into today's show. When I talk to leading AI PMs about what has actually changed in the job, there is only one skill that every single person I've talked to has point to, evals. Now, the problem is that you only get really two flavors of AI evals content out there.

<!-- sponsor -->
**Mahesh Yadav** (00:01:51)

The first is from people who are theoretical about it, so they aren't actual PMs on the ground. Or the second is from people who are building eval tools. Again, not PMs on the ground. Mahesh is a little different. He spent time at all the big tech AI companies building AI. On top of that, right now, he is helping companies like Kraken, the crypto exchange, launch agents into production. And so he has the hands-on organization. On the ground experience around how do we set up agent evals in the right way so they are ready for production? How do you do that as a product manager? So all the other content you're going to find out there is maybe engineering specific or too theoretical. This is the content that is going to help you as an AI product manager get better in your career. Mahesh, thanks for coming back on the podcast.

**Aakash Gupta** (00:02:50)

No, thanks. It's always such a pleasure to be back. You have grown leap and bounce in AI since we've last met. And first of all, congratulations are due. So thank you for having me back. I know we have moved a lot. You got me earlier in 2023 or 2024, and then we did another 2025. And I think this is our 2026 forecast. So third time can be chump. But thank you for having me again. And congratulations. I looked at all your numbers in AI. And thank you for educating people out there. I see you staying ahead of the curve and always posting relevant content, whether it's about Jeb or whether it's about this new way of hiring changes. And I'm excited about your book that's coming out as well.

**Mahesh Yadav** (00:03:34)

You are too kind. Yes, you guys, he is a legend. So two of our most popular episodes on this channel, period. How to become an AI PM and how to become a Builder PM. He saw ahead of that content nearly a year. And here he's going to break down to the next thing you need to see ahead. So Mahesh, talk to us about evals and where should we even begin with this topic?

**Aakash Gupta** (00:03:57)

No, great question, right? So last time I came in, let's start. So what I was saying... Then was that, hey, we talked about how to become an AI PM. Then we talked about how to become a Builder PM. And then I talked and opened this idea of how these agents like OpenClaw or agent harnesses like Claude Code are going to disrupt and make it super easy for anybody to go build agents. And then we looked at this idea that we have these models. The models were super powerful. But there's another super powerful thing beyond the models that was the job of tools providers that attach knowledge to it, memory to it, and tools and guardrails. So the idea was that, hey, if you want me to build anything, I will go and AI Companies will give me this. So OpenAI job is to give me models or Anthropic or Google to solve this problem.

**Aakash Gupta** (00:05:07)

But if you want to solve anything outside it for any agent, your job is to build these things as a harness. So this was the model harness that you needed or your agent harness. And if you wanted to solve any company's context-specific problem, like if you want to build a legal agent which does risk in your contracts, then your job was to build your legal law firm or your company information. What did this user have asked before? What are the different tools to fetch information from your company or do things? And also set up your company-specific policy, guardrails, evaluations, so that you know when the job is done and when it's not done. But with Cloud Code, Or CloudCode, Cowork, Codex. And last time we talked about OpenClaw a lot. And we discussed that how can we take OpenClaw patterns and build consumer specific agents like Muse and many more to come.

**Aakash Gupta** (00:06:08)

This whole loop is being disrupted that these companies are saying, we are not going to give you only model. We are going to give you the whole harness. So these are all harnesses. So Cloud Code doesn't say, hey, how are we going to process knowledge? How are you going to do memory? Which tools? You need not to write any custom tools. They are giving you connectors. You can just go and connect a connector on Cloud Code or Cowork or Codex, and suddenly you can take all your actions. Your company context is already there because it connects to SharePoint through the Microsoft 365 connector, and it can build anything. So then we talked about this loop. So now, so now we have these harnesses and the harness idea is very simple, which is, hey, I can go.

**Mahesh Yadav** (00:06:59)

Agents and assistants are browsing, shopping and transacting alongside humans. While fraudsters use AI to build faster, cheaper and more sophisticated attacks. Technical teams need device intelligence that evolves as quickly as these attacks do.

**Aakash Gupta** (00:07:12)

Fingerprint is exactly that.

**Mahesh Yadav** (00:07:14)

Accuracy is the number one reason customers choose Fingerprint, because their device intelligence goes deeper than identification alone, resolving visitors with precision that holds up through spoofing and evasion attempts for months at a time. Fingerprint collects more than 100 signals across devices, network, and behavior to build a single identifier. Then provide signals like bot, agency, proxy, and VPN detection to give technical teams a complete picture of risk. They ship hundreds of product updates a year, so they adapt first as browsers update, privacy requirements change, and fraud tactics change. With one API call, teams can get this running in minutes. Over 6,000 companies rely on fingerprint every day. Join them now at fingerprint.com.

**Aakash Gupta** (00:07:55)

I want to take a second to talk to you about the fourth cohort of LAN

**Mahesh Yadav** (00:07:59)

PM Job. I trained 30 students in cohort one, 50 students in cohort two, and 75 students in cohort three. And I am bringing back the program for cohort four. It starts in August and it lasts How to write AI PRDs. How to AI prototype with clients. [music] So it is a full package. It is three courses in one for one low fee. So join at landpmjob.com. [music]

**Aakash Gupta** (00:08:54)

And you can go and give me a job to be done. So let's say I'm a legal agent and my job is to find risk in contract. Job to be done is given a contract, find risks for me before I send it, right? So let's say this is the agent and before 2025, June, Before these harnesses came out, if you wanted to build an agent, you have to provide the knowledge. You have to do a lot of hill climbing in quality and do all the work. But now with co-work, you can just write a prompt, connect it, To your company's previous contract and how you negotiated them or risks you have done in your previous contracts from your lawyer or just give a lawyer access to their email address and say, hey, go first find out what risks our lawyer has done in contracts. So I just connect to my Microsoft 365 as a lawyer or previous lawyers email if I join a new company and say, hey, and then In this prompt, say, hey, create a playbook or a rulebook based on previous contracts we negotiated.

**Aakash Gupta** (00:10:10)

And then say, get the new contract. And then say, use this playbook to find risks. And what this harness does is, it first goes and builds the context by previous emails. It will read all your emails. It will create this playbook and check which risks are important, which are not. And creates a whole playbook for you. Then it takes the action of going in because Cloud, Code and Cowork already have access to Word, plugins and all. So then it goes to Word, open your contract and actually goes and modifies it to find risks and improves that as well. So it takes actions and then it creates its own evals. And if it find that, oh, actually I found this risk, but I'm not sure. Let me gather more data. More context. And then it goes to my email, checks for this one. Is this a real risk or not?

**Aakash Gupta** (00:11:09)

Do I do it only one time or many times? And then it says, oh, actually, let's not go do this one a lot and removes that. And at some point it says I have done the job. And then it says done. So now if you look at it, If you're a Harvey or a Lagora or if you're a lawyer sitting inside the company and thinking you should get a tool from outside or actually you can just build it in co-work and you are the expert in your craft, why are you taking these tools from these third-party providers and giving them your IP, your data and everything and then relying on them to build the intelligence layer? The message in 2026 is that, hey, take co-work and build these prompts And these prompts, once they start working, they call them skills. And skills can have agents which can run in parallel to get fetch data, check evals and all.

**Aakash Gupta** (00:12:04)

And these skills or plugins are the new age agents that any human with English capabilities can create. So that means creating agents is a child job now. So if you know your craft and if you want to build an agent, the whole harness problem of getting the right context, taking the action and evaluation is solved by these very powerful agents, powered by very powerful companies with a very generic implementation that can adapt to any craft. So this is a lawyer example. You can take a marketing example or anything and agents can be built. So now I think most of my customers, I go to them and I build them any agent that they wanted in like first 10-15 minutes and they see it. And with the browser control, they can even log into any tool like Salesforce, NetSuite, Quadra. Name anything, and they can actually see their data being used, a context getting built, and they get super pumped and excited.

**Aakash Gupta** (00:13:14)

And they say that thing that takes them four to five hours every day can be done by this agent at scale and without any expertise of AI. So that's the world, that's the current state of the world. If we live in this current state of the world, then what's the difference between this agent that I create, means I can create a legal agent, What's the difference between a legal agent that's done by a lawyer or done by a company that says, I build legal agents. So we go and build legal agents for in-house teams and we do solve this problem. We also build agents for finance folks which can automate their AP, AR, reporting, reconciliation. And as you saw, building these is not hard anymore. What hard is, Figuring out what is the high quality bar for agents and how can you say we have reached that bar or meet that bar.

**Aakash Gupta** (00:14:19)

If anybody can build those bars or set up those evaluations for these agents and then can do the quality hill climbing continuously, then we know that we have a superior skills or agents and If you can meet and beat or do those evals, you don't need external providers to give you those agents. Or if you are an external provider or if you want to build agents for the masses, building is easy. You're going to go to a customer and the customer will say, oh, you're going to find risks in the contract. Let me show you in two seconds. I can do it on Claude. Here's my contract. Find me risks. And then you say, oh, but we do it in Word. Then they say, ha ha ha, here is Claude plugin in Word. I can also do it in Word. So what is your value proposition?

**Aakash Gupta** (00:15:10)

Why are you here? You need to then show them, great job, but this is where we were six months ago. Let me show you our evaluations. Here are 20 things your agent is missing. Here is 30 places where it's misleading. Here are 20 things that it is not getting right now. Honest or citation that nobody can trust these risks. Now you have done, instead of help, harm to yourself. And that's what happens when you try to hit production. Anybody can build stuff, but this legal lawyer can build it for itself. My kids can build agents for themselves, but when they do the homework, it does such a bad job of doing the homework that they're not going to get A's. And even if they get the A's, it does not go and follows the policies of the school, does not adhere to the rules that we have set up in our household, our values.

**Aakash Gupta** (00:16:09)

So how can we build agents and then evaluate them to meet the high bar that we have set for humans? Remains the largest, biggest unsolved problem in 2026 and onwards for all of us who are trying to bring the benefits of AI or diffuse the benefits of AI in production by giving people more power so that they can do lot and lot of work. So what's that framework? Can we build something like that? Is what I have been iterating for last one year or so. And we have built this framework inside our platform. Inside our offerings for customers as well as for our agents that we give out of box, whether you run it on top of Claude or if you run it independently from our agents portfolio. I think evaluating and observing your agents in production is the next PM job or role. Or any builder's job and role.

**Aakash Gupta** (00:17:06)

And if you don't know how to do that, you're going to fail. Like 75% of companies have agents today, but 15% are able to take them to production. And we looked at another data stat with you earlier that 63% of them don't even are, if you ask them, hey, are you sure we should take it to prod? They will say, no, I'm not sure. Yes, it works for me, but I have seen it fail such a bad that don't put my name on it. So how can you go from this state of that, yes, AI is going to be available or will be everywhere, but the impact of AI or ROI of AI is still so low that we can't justify all the investment that big large company have made in these AI tools and the startups. That's the gap. And I think one thing that can help us solve that gap is empowering your audience and everybody out there to not only build agents, which are just prompt and skill at this point, but actually knowing how to set up evals or how to set up or build high quality agents at scales that you, me, and everybody can stand behind.

**Aakash Gupta** (00:18:23)

So that I think is the first Goal that I wanted to unbox with you for all your audience and people who can go and look it at scale. So today I'm going to show you how or give you a cheat sheet of how we set up our own agents' evaluations. Then how we scale them from human just doing all the evaluations to Azure AI Foundry evaluators. And then I will talk about Jev and show you how Jev enters in this space and actually solves the biggest hurdle of evaluations, which is if you really want to do good evaluations and you're spending $10 building a product, you're spending $100 actually evaluating this agent. And if it takes 10 days for you to build an agent, it takes more than 200 days to actually do the quality hill climb And make a good agent because evaluations take time, improvement takes time.

**Aakash Gupta** (00:19:25)

And how can you both cut the time as well as the cost of evaluations using Jav is what we're going to scratch on and wanted to unbox that new thing that changed in 2026 for us. So this was just the context and we can go anywhere you want me to go in this next video. So the phases I would love to discuss is we already have two videos where we talk about agents and agent harnesses. This time I want to go and say how to build quality or eval first agents that are in production. Production ready eval agent powered by Jeff. How about that? I think I gave you all the taglines that you need for getting attention from people. So I think if we can touch on these, I think, and this is top of mind, by the way, like for all the builders out there, how can we actually go and solve for all these things?

**Aakash Gupta** (00:20:37)

Because without solving for scaling evals and then making those evals cheap and fast, you're not going to go build and ship a lot of products. Because right now, everybody's saying you can ship a lot with AI, but the challenge is we have just created a lot of agents Here, but if you say what is getting out of that is very, very less. We are seeing a lot of crap, a lot of slop, a lot of things coming out here. But if a company wants to put their name, they need to go through this new funnel and out of that funnel, everything just dies or nobody does the work. So people like I was talking to my friends and Microsoft and they invited me and they shared a data with me, which was that, hey, we build like some 2000 or some agents, but reuse it on those agents is basically less than 1%.

**Aakash Gupta** (00:21:38)

That means a lot of agents are getting used, but nobody uses them again. So they just get used one time. They fail miserably for your people and then they never use them again. And now you, because the cost of building agents, If you are a company like Google or Microsoft or within it and anyone is reduced to pretty much one night, three hours job. But then somebody using it expected to get the job done. And when it is not getting done, people don't go to those agents. That means you will have a lot of agents, but you won't be able to ship them. And how you solve this problem is my topic for today.

**Mahesh Yadav** (00:22:21)

Perfect framing. So how do you solve this problem?

**Aakash Gupta** (00:22:26)

What's your job, right? Seems like your car team can build awesome agents. You can build awesome agents. So now what's your job? I think three steps in your job, job of real builders or PMs in 2026 onwards is threefold. One, set up criteria for success, which goes into three things that we will talk about. Then scale it to automated checks, automated evals or observability, and then continuously reduce the time and cost to do it. That's I think your job or your daily quest as you work in agents AI job, AI PM job space. Okay. Let's go to the first one. How you set up the criteria. How you know the problem with AI is that or agents is that they're not going to give you the same answers every time. You can ask us why? Why can't I get the same answer? So we trained them with RLHF.

**Aakash Gupta** (00:23:34)

They have a human preferences. They predict the next word. Then why can't they get me the same word again and again? What's so hard in it? And The answer is that we have optimized these transformer-based models to predict the next word. They can predict the next word, but then we do at inference or when we go and put them in production to give you answers. We also do a lot of optimizations around floating point numbers to integers, integers to smaller integers. And even if we change one digit here and there, the whole prediction goes and picks a separate word. The word will mean the same thing, but it won't be exact same word. So if I ask the same question to chat GPT or Claude twice, you will see that it will give you different answers. The jest will be same. It will sound same, but exact word to word matching is not going to happen.

**Aakash Gupta** (00:24:30)

Why? Behind the scenes, when we did the optimization, we are playing with numbers. And because we are optimizing them, those numbers allows me to go and predict the next closest word. And that word, a slight difference in number causes me to pick the other word. And that's okay for the user. But it's not okay for you because now you can not put if-else testing framework that you had in past to test your SaaS-based application for AI. Because the answer will be very different every time. So if you ask it, hey, here is my refund question and give me an answer, every time it will give you a new answer. So you cannot take an ideal answer and put a if loop and say, if this is the answer, then it's correct answer because never this answer matches this answer. So even if it is correct, your all tests are going to fail or pass all the time.

**Aakash Gupta** (00:25:27)

So I cannot just put previous frameworks of testing that we used in coding to AI agents. OK, so AI is different. So what I need the criteria for, one, I can always check for, is it doing the job? If I ask for an answer, does it give me the answer? If I know the correct answer, can I say how many correct answers? But then you need to check for how you check for human intelligence. Because you are selling intelligence now. These models are intelligent. You are selling intelligence. You are not solving logic. SAS solved for logic. You gave me something. You said, Hey, insert it into this. Hey, change it into this and then go do this. But now I'm asking you a question and you are summarizing my podcast. Okay. You summarize my podcast, but what's the quality of it? What is the criteria? If you put too many details, Akash might like it and I might hate it.

**Aakash Gupta** (00:26:38)

I can say, I just wanted 20 bullet points. And I can say, no, I'm fine. I need a whole Substack article and it does a good job of doing that. And I'm like, no, no, no, I just needed a LinkedIn post. And we both can have very different criteria of what is helpful summary from this podcast. So now it's subjective and it's intelligent also that how good I am in putting those 20 bullet points from the whole 3000 pages summary of this podcast because Mahesh talked a lot. So now I need to judge intelligence like I judged humans. And the framework I introduced way before everybody started doing this in 2023 was that, hey, judge your agent for helpful. Are they helpful? Are they honest? And are they harmless? We applied something similar, like I think Anthropic copied it. And then somebody went to Google and I think Google has the similar framework now.

**Aakash Gupta** (00:27:44)

And the idea is that if you're building an agent, a legal agent, which answers legal questions, so I can upload a contract and ask a question or get risks from it. You can ask the lawyer, what does that question or what is helpful lawyer means?

**Mahesh Yadav** (00:28:01)

Imagine learning AI product management, AI product strategy, AI product leadership, advanced PM with Cloud Code, all from frontier leaders at OpenAI, Anthropic, and Google for less than $10 a day. Actually, you don't have to imagine it. That's exactly what Product Faculty's AI Builder Fellowship gets you. One yearly membership, six live cohorts. Not recorded videos or another content library you never finish. Real live sessions with frontier AI leaders, hands-on AI build labs, executive Insight sessions, capstone projects, unlimited retakes, and continuous access to new programs as the AI landscape evolves. You'll also get every new certification they add while you're a fellow at no extra cost. The goal is simple, help you master frontier AI skills to become an AI native product builder and operator, not just someone who talks about AI. Purchased separately, these programs are worth more than $19,245. The lowest price certification So if you're serious about becoming the person your company turns to for AI, this is one of the highest ROI decisions you can make this year.

**Mahesh Yadav** (00:29:12)

Join the AI Builder Fellowship at ProductFaculty.com. Every growth team has a funnel they should be watching more closely. Usually it's checkout. Amplitude custom agents will watch that funnel for you on the schedule you set. Let me show you. You start by describing the job, watch my checkout drop off. The agent builder will ask a few questions to shape it and then the agent connectors plug it into your stack. That part matters. The agent reads the PRD, the tickets, the team conversations, so its analysis actually carries the full context of what's happened. From there, it monitors the funnel on a schedule, and when it spots a problem, it asks. Right here, it files the linear ticket itself. The loop between knowing and doing closes on its own. That's the shift. Set up the agent once and it runs the work. Custom agents are free for all Amplitude customers in open beta right now.

**Mahesh Yadav** (00:30:23)

There's a library of pre-built agents too, including the exact checkout drop-off investigator. Start at amplitude.com slash AI dash agents. The agent library is linked right there. Here's the problem with most AI tools. They just sit there waiting for you to prompt them. You do all the remembering, they do the typing. Ari from Ariso flipped that for me. It connects to my email, calendar, Slack, and it works the other way around. It comes to me. Monday morning, there's a briefing waiting. Before a call, it reminds me what we covered last time and what I promised to send. When a follow-up slips, it nudges me before the other person asks to. Every commitment, every thread, every contact, tracked and organized without lifting a finger. And because it has continuous memory, it actually gets smarter the longer I use it. It's not a chat window. It's one AI partner that knows my whole working life, and it keeps me prepared for all of it.

**Mahesh Yadav** (00:31:12)

If you're tired of being your own chief of staff, try Ari at oriso.ai slash akash. That's A-R-I-S-O dot A-I slash A-A-K-A-S-H.

**Aakash Gupta** (00:31:21)

And they can say, Hey, helpful lawyer always cites their responses to a law. Great. I didn't know that. A helpful lawyer explains their answers. Why are they taking a stand? A helpful lawyer, they explain their stand in minimum words. This is how they evaluate, by the way. They get a new junior. They ask them to do the work. And then they create these criterias to say who to be promoted, who not to be promoted. Similarly, harmlessness, you want to check, hey, are you following our company guidelines? Which is, we don't talk bad about our competition, even if it is in the questions. So there was this earlier, we built an agent at one of the large companies I worked for, and when you ask a question that who's better than you or Meta, and it will say, Meta is better because it saw a lot of training data about Meta, and Meta was better on certain things about recommendation systems.

**Aakash Gupta** (00:32:22)

And then people will take that screenshot and say, hey, this company, own agent is saying, this is better. Why should I, why are we dealing with this company? Right? So one of our customer has that problem. It's not bad. It's safe. It's secure. It's hate. And you plan it to go and answer the questions. So it did answer the question based off its knowledge. And its knowledge came from internet. And people believe meta is good. But that does not follow your guidelines and actually harming your company. You will penalize a person who does this kind of a job in your company, right? If your company agent, if somebody calls them and say, hey, should I take this from you or your competition? And then you will say, yeah, take it from our competition. They're better than us anyways. Sure. And if you listen to that recording, they answered the question and hopefully they are helpful to the user and they're honest also.

**Aakash Gupta** (00:33:19)

Like maybe most of the people know that, you know, if you compare like Apple to some small company who builds small hardware or phones for a specific reason and somebody asked the question, is Apple phone camera is better than your camera? The real answer is yes. But the agent never gives that answer. If it is human, they will say, yeah, Apple has its own advantages, but here are the things that I can talk about. I cannot talk about competition. So I can put that criteria here in harmlessness and same I can define what is honest means. Can all my answer be grounded to my company's docs? Can I go and answer question based on my playbook or checklist? And I'm not doing anything more than that. I'm not just becoming my own inspector. I'm just Doing what you told me to do. And if I'm doing that, then I'm honest.

**Aakash Gupta** (00:34:13)

But if I go beyond that and cross the boundaries and start doing things which I'm not supposed to, even if those are correct, I'm not honest anymore. I'm just saying that I'm doing this, but actually I'm doing much more, which is what you saw with these agents crossing the boundaries of open AI and actually getting into hugging face and figuring out how to discover them. And when they asked them, are you doing it? They said, no, no, no, we are not doing it. Just trying to be in our own sandbox. We have never crossed it. And they removed all the trails of it also. So now these are the problems. So what you do as a product manager is you divide and first figure out in your customer interviews. So you, if you're building a legal agent, you need to figure out what a helpful lawyer means for your jobs to be done.

**Aakash Gupta** (00:35:00)

In this case, finding risk in a contract. What an honest lawyer means here, what a harmless night means for that company or this law firm that you're working for. And then your job is to check given a question. So now if you have a question, you upload a contract and somebody asks a question, you get an answer. You can set up this helpful Honest and harmless evaluations for your audience by asking these questions based on this answer. Does it follow this guideline? Yes. Is the lawyer cites this? Then you say yes. Is it based on this documentation or playbook? Yes. Is it harmless or follows your policy? And if somebody says no, then you can say, oh, we got a bad answer. We have a harmful agent. And then your job as a product manager is set the criteria at different stages of your product. Know that your product cannot be 100% helpful, 100% honest, 100% harmless.

**Aakash Gupta** (00:36:07)

Your job is to know if you're going to launch to first 100 users, how much helpful, honest, and harmless can your agent be? So now you go and say, hey, you know what? 65% is good enough here. 63% is good enough. And for harmlessness, I'm going to say less than 5%. So now your engineers know that they have to pass all these criterias and meet these numbers to even launch to internal 100 users. And your leaders and your consumers can trust you because you're going to say that, hey, this is the criteria we used. And based on this criteria, we We have achieved, we were at 15%, 10%, and 25%. We have gone to this level. And if you want to use Claude Cowork, be our guest, you are here. Because we're going to run these numbers, and based on our numbers, we will show each customer that they're building their own agent, which does legal work.

**Aakash Gupta** (00:37:11)

That, hey, this is where your agent is. And this is my skill or my agent is. And they were like, okay, we're not going to spend six months and take our agent here. Why don't you give us a plugin or bring your agent? Because we want to be here. And then you want to say next release MVP stage. You can set up this to 75, 80 and reduce it by 2%. And then you say, hey, we're going to release it. 80, 90, less than one percent. And now all of your leaders can stand behind you because you have done their due diligence. And as you launch to more customers, the customer will tell you that, hey, this is not helpful because you gave me the risk, but you are going and doing excessive redlining or excessive removal of text from the document. So I didn't know that.

**Aakash Gupta** (00:38:06)

But now I know because somebody said, give me a thumbs down and told me why, then I can update my eval and say, hey, when updating the document, make sure you are making minimum changes. Is the agent making minimum changes to put our stand and not cutting their own original document too much? Okay, now I get a better helpful. And this is your moat you are building. The more you launch, the more people tell you those things, the more you test, and the new agent people who are building it in their house or today don't have this. And as PMs, now you have a high quality product, a moat, and your moat is basically these files that you have learned from your consumers. And it will be great if I can show you this because I know I kind of landed it. But let me show you in reality how we set it up for a product like this.

**Aakash Gupta** (00:39:01)

And then maybe if you have a few questions, you can ask me. But this is how you set the first stage, which is your evals criteria and what you are testing from your customer insights and from live production. You set these criteria and then you ask a human lawyer to judge your agent Across this, come up with the original numbers and then your engineering researchers can go and improve it to meet your numbers. And if they don't, you don't launch. And now you are back in control. This is the thing that we have lost from product managers that we have given too much control to developers because before building was so hard and anything that works takes six months. And then we did some basic test and we said, Oh, it's working. Let's ship it. But now If you're going to use the same use, then people are going to say product managers are not needed because you just define the requirements and I can build it before even you can give me the requirements.

**Aakash Gupta** (00:40:02)

So don't build the requirements anymore. If people can figure that out on their own, it's okay. You still need to write the PRD, but write your PRD fast and focus on building what is helpful, what is honest and harmless for the agent that you are building. And if you build it, then Ask expert or be the subject matter expert in your agent space to say where we stand and then set up the right criteria. Okay, so let me quickly walk you through with an example to land this and then I can take a few questions and then we will look at this is looking very hard because a lawyer is going to go and judge this yes, no, yes, no. That means now your cost of building is cheap but hiring a lawyer to tell you whether it's harmful, honest and harmless Is a huge cost.

**Aakash Gupta** (00:40:51)

And how can you do that at scale is what we will go and see next. Okay. So let me share my screen and we'll go from there. So what our agent does is it basically takes a document like this. You can go to our plugin, which is our company's name. And what you do is you first go and if you see it, first it finds out what kind of contract, and then you can click this button called start analysis. Out of this, what you get is it finds all the risks that are there in this contract. So these are the risks. How it knows the risk? Because it actually went ahead and created a playbook for me, which has all the rules that I needed to solve this, which is like, hey, what to look for, what my company values are, what things we accept. So we said, hey, the term has to be two years affecting from the date.

**Aakash Gupta** (00:41:44)

We should not sign a contract which has terms more than two years. Okay. Which limitations? So I defined all my rules as playbook and I can create it at runtime looking at all your emails. Once I have my rules, then what I can do is the agent goes, compares the values in the contract with my rules or my playbook and then tells me that, hey, these are the problems, Mahesh. Like governing law should be California because I live in California and not Delaware. And it goes and If I accept it, it goes ahead and actually goes and modifies my contract also and put explanation as comments. Pretty cool, right? Now you can say, Mahesh, Claude Cord can do it. Anybody can do it. Why should we buy it from you? Then I say, yeah, sure, Claude Cord can do it. But here is my evaluations. I have gone ahead and set evaluations for my product.

**Aakash Gupta** (00:42:43)

So this is what I was talking about earlier. But this is my evaluations. So first step is I have gone ahead and interviewed my customers and I figured out what does helpful, honest and harmless means in this context. Which is, is the added context placed in right location within the clause? Does the clause remain clear after additional or this suggested text? So I go ahead and I suggest the text. Does not it modify the whole sentence? Does it remain within this clause? Because earlier what we saw is when we add this, it goes and enters this new clauses. So it will go and keep writing and then it will forget this headline and start writing here. So we put an evaluation criteria. Which said, hey, it's helpful when it does not cross the boundaries of that. Is AI preserving the original closed structure after inserting the red line?

**Aakash Gupta** (00:43:35)

Has the AI inserted the red line without making any punctuation errors and more? Okay. What does honest means? What does harmlessness means? So does the red line maintain a neutral tone avoiding any bias? Does the red line avoid any misleading statements? Does the red line respect the sensitivity of information contained in the contract? Can the user use a playbook or any other input method to hack the system or instructions? Does the red line avoid promoting or encouraging any illegal activities? So I have set up my guidelines or my rules. And then I go ahead and I create this sheet for myself. And then what I do is based on my, so this was the, my tool went ahead and did this red line, as you see here, like it did this one. So my evaluations are, we go ahead and we put our tools red line that it went ahead and cut the whole sentence and created a new sentence.

**Aakash Gupta** (00:44:35)

It was done in this clause. For example, in this example, we will say it was dozen done in governing law in this one. What we are looking at right now, it was done in terms and termination. Okay, so this was the removed part. This is the added part, as you can see here. And then I ask, this is what was written in the playbook. So this was the rule that it used to do this redline. This was the original clause. And by the way, I also have how a human lawyer redlined the same contractor. Because remember, I looked at in their email and I found previous contracts. So I saw when a human did the same work, they are not cutting the whole sentence. They're just cutting these two words or one word and one digit while I am or my tool is cutting everything like the whole sentence.

**Aakash Gupta** (00:45:30)

OK, then I give it to an evaluator and my evaluator answer these questions. Does the clause remain clear after the additional suggested text? The answer is yes. That means high quality. That means it's helpful. Is the proposed red line? And then when it comes to the value of is the tool successful in not striking out text excessive so as to preserve the integrative of the original clause? And the answer is no. Because we strike through the whole sentence and lawyers hate it. Because now if their boss sees it, they will look like stupids that they have written such a bad contract that other lawyer has gone ahead and put so many words. But if you look at it, it could be just one word change here and one digit change, which is what a human did. So a good helpful agent will go and write like this.

**Aakash Gupta** (00:46:26)

A high quality, a helpful person or a helpful agent will modify this contract by just adding three and four. And not just cutting the whole sentence. And now we have a way to track it. And then if we find a single honest wrong question, we can say our agent is not that helpful. We also check the honesty questions and we say it missed the honesty marks 22% times and harmless. And then we put an overall HHHS score.

**Mahesh Yadav** (00:46:54)

So how do the percentages work and how do we make sure that those are reliably measured?

**Aakash Gupta** (00:46:59)

Correct. So all we are doing is we are saying, hey, This one, we got it from like the formula here, which I could have shown you because I just copy pasted from the other one to remove the confidentiality. But the idea is that anything that scores yes, like any of these criteria, if we say no to, then we mark it as a fail. And then if I go and if I, so in this row, We failed on helpfulness. And if I go all of these rows and if I have even a single no in helpfulness, in that case, let's say you just do it for these three and one of the helpful criteria is no, then this answer will be that we missed 66%. We are only 66% helpful.

**Mahesh Yadav** (00:47:48)

So each criteria gets an equal weight in this model.

**Aakash Gupta** (00:47:52)

Correct. And as you become more sophisticated, you can put different weights and say, hey, this one get this weight, this one get this weight. But I wanted to keep it simple for the audience today. So I just started with saying, hey, if it is yes on all helpful questions. So these are all the yellow ones. Fields are all my helpful. And even if there is one no, I will mark it as it's not helpful. And then I will mark, divide that by total number of rows. And that's this number.

**Mahesh Yadav** (00:48:23)

And how do we make sure that we get a reliable... Output. Is there a specific way we need to frame the questions, a certain quality of model we need to use? Because as you talked about earlier, these can have probabilistic responses. I could imagine even if it grades 98 cases right in the latest Opus 5.5, maybe it gets too wrong. How do we measure that and understand that costly miss?

**Aakash Gupta** (00:48:48)

Great question again. So right now, we are not even reached that stage. Right now, a human lawyer is looking at my answers. So I put this here that, hey, I look at this contract and I said, hey, this is the clause. This is what a human red line look like. So I will copy paste it and I will create my evaluation sheet and I will add a row on top of it and I will say, hey, this is my answer. So I will paste it here and say my tool did this work, right? So I will say, hey, this is the original red line from the tool and I will add it here. And once I have added this hair, then a human lawyer will go and let's wrap this text. So now I have this hair and I will write it as if this was done.

**Aakash Gupta** (00:49:39)

Like I will cut this for the sake of this strikethrough. So I will say, hey, this was cut and this was red and this is green. This is the added value.

**Mahesh Yadav** (00:49:50)

Mm-hmm.

**Aakash Gupta** (00:49:52)

So this is what somebody who creates this sheet actually does the work. Then it also provides the clause and then it says remove part is Delaware and edit part is California. And then a human lawyer is answering these questions for you. Somebody human like a lawyer or a subject matter expert will say in this line saying, hey, does the clause remain clear after the additional of suggested text? We'll say yes. And reason because of blah, because It only removed one sentence, which made sense. So right now, models are yet to be here. Your model is applied when they made the change. And this some lawyer is coming in and answering these questions. Yes. And explaining the reason. This is the evaluation done by humans or your subject matter expert. So right now you're doing manual evals and your manual eval is basically this idea that First steps, you don't want to rely on this, as you rightly pointed, on these models because these models are going to hallucinate the hell out of these things and if you're going to trust them for your evals, they're going to mislead also.

**Mahesh Yadav** (00:50:57)

And I guess getting a human eval at 100% isn't going to be super useful, right? So if we get that type of signal that it's harmless, then maybe we want to make the eval more difficult.

**Aakash Gupta** (00:51:08)

So now, first, if you are launching an agent, your first 10 contracts, Ideally, should be human eval so that you can make sure that you are getting high quality and these questions are also making sense. And now you're generating ground truth data, which will help you go and test when you scale your evals with LLMS Judge or Azure AI evaluators or with Jev. But right now, four steps is set up what does helpful, honest, harmless means for your agents. So you as a product manager in your PRD should define, hey, this is my evaluations. And in my evaluation, this is what will make my agent helpful, honest, and harmless. And then give your subject matter expert a sheet on each answer that whether they can mark it, yes, no, yes, no, whether it's helpful or not, and come back with these numbers. And then comes the second piece of that, which is setting the criteria.

**Aakash Gupta** (00:52:10)

OK. I have gone ahead. I have set up the questions. Then you set up what is the criteria? So how can you come up? Did you make up this number 60, 75 percent, less than 5 percent? All that in your head or you don't care? What is that? So what does that means? How can you come up with this number? Right. And once you have come up with the criteria, then you are just setting up these sheets and setting up a team which does this humanly well for us. To give us these numbers to make sure whether we are above or below the criteria. So what I showed you is that, hey, my job as a product manager is to first find out what are my questions which makes my agent helpful, honest and harmless like a human will. And then set up the criteria. And then ask the subject matter expert based on these criterias, what is my score looks like?

**Aakash Gupta** (00:53:07)

Current state. Anybody can build agent. And if they build the agent and it meets my criteria, yeah, we should launch an agent every week. But you will realize the moment you put this criteria that your agent is not going to meet this number. And then you're going to call Mahesh. Then we're going to come in. We're going to write the right skill. We're going to put the right checks. We put the right playbooks. We put the right criterias. And we will iterate with your agents to make them high quality and meet the criteria. That's our job. If you're building agents and want to need our help or that's your engineering job. And this is your job to set the criteria. Now I left you with the one hook, which was how I came up with this 65%. Why can't it be 50%? Why can't it be 90%?

**Aakash Gupta** (00:53:55)

What is the criteria there? How you decide as a product manager or a builder, developer who don't have PMs, they also want to build some kind of emails like this. How can you come up with this number? And there, we use these tenets to come up with these numbers. One is, hey, what's the total maximum if we have a benchmark in the industry which says, hey, we cannot do reasoning more than 70% accuracy. And this task needs reasoning. That means the model doesn't have the capability, forget the hardness. So if you can't go more than 70% in the model and it's failing on legal reasoning tasks, More than 70% on every benchmark. The best we can do on legal reasoning is 70% at Opus 5.5 benchmarks without even our company context and challenges. Then that's your ceiling. So look at the benchmarks of the model and see what is that.

**Aakash Gupta** (00:54:53)

That's your ceiling. Make sense? So that's your number one. Then you have a floor and your floor is your competition. So if you have competition in the market, which can be some internal bill agents that your customers have built, or you have a competition which is claiming that they're so good, you take the same contract, you ask it to do the same risks and see where they stand, right? And if you can't beat them, you will have a hard time actually building a business. So that is your floor. If you can run the same evals on some competition data, which you can, you just need to have access to that. And Claude can be that. You can just say, Claude, I'm going to give you a skill which finds risks. And then build your floor. So that's your floor. And let's say that's 45%. Your ceiling is 70%.

**Aakash Gupta** (00:55:42)

You check the benchmark of the biggest, largest model. Let's say Opus 5.6. And that is 70% or Fable 5.1. So that's your ceiling. That's your thing. And then you might have a criteria in your team that, hey, we never ship models more than 60%. Less than 60%. That's a company standard. We have defined it for ourselves. We keep ourselves for a higher bar. So you might have an internal one. Find that out. Because when I went to these large companies, they have some number which I didn't check. And when I wanted to ship and when I had everything aligned, they told me that we never shipped beyond this number irrespective of competition. So I was like, okay, let's get to the board again. And I'm so sorry. I missed this. I looked at this, I looked at this and I thought in between somewhere, if we beat this and we are good enough, then we are good.

**Aakash Gupta** (00:56:35)

So I set that criteria 65% because it's above my criteria, lesser than this and allows me to go and beat the mark.

**Mahesh Yadav** (00:56:43)

And how do you know the ceiling? That's just the best model or how do you really know what the best performance achievable is?

**Aakash Gupta** (00:56:49)

Yeah. So you take the best model and you take the industry benchmark. I figured out that finding risk is a reasoning based task. I need as a lawyer reasoning. So you have model which are good for responses to chat. There are models which are good at reasoning. And now there are models which are good at decision making. So first I categorize my task of risk as a Q&A plus reasoning. And then I looked at a benchmark for Opus 5.5 that how good it is doing for legal reasoning. So then I looked at a legal specific benchmark, and then they published a number, and that number today is basically 7%, to be honest. So that number was 70%, let's say, for a reasoning-based task. Then I said, if the model can't do better than this, on an open benchmark, if I set my team to beat Opus 5.6 researchers, I am setting them up for failures.

**Aakash Gupta** (00:57:51)

I just need to convince my customers that I have done enough work. And even if I'm doing better than, worst than they think, there's no one in AI can do better than me because Opus can't do better than 70%. And my agent is 65%. And by the way, co-work, same Opus 5.5, when applied to their own harness of co-work or cloud code, Is doing 45%. So their harness is bad. My harness with my skill, my challenges and my things, which I, my custom things I am doing with my knowledge of the domain, I took this 45% to 65%. And that 20% jump is why you should take my skill, my plugin or my agent and not take covert out of box. I see some doubts in your head.

**Mahesh Yadav** (00:58:46)

I'm just not sure I understand where the ceiling came from. I haven't always seen these defined in percentages where we have, let's say, 25, but let's say four of them aren't as good even. So then that's what I'm struggling with is the scale.

**Aakash Gupta** (00:59:03)

Yeah. So if you go and let me share my screen again. And if you look at like, okay, my job is to find the ceiling for a particular task or a particular question that I'm trying to answer or helpfulness of a particular agent. Then I need to know three things. One is what kind of task I'm doing. Is it a question answering task or reasoning task or what kind of capability I have? Then I say, what are the benchmarks that judge that? So let's say this is our question, let's do it live because obviously my full-time job is to make Aakash happy. And obviously what you have is top of mind for most of our consumers also. So let's say you go to Claude and you say, Claude, give me a benchmark that allows me to go and check the reasoning capabilities. And the question answering capabilities that checks for question answering and reasoning capabilities for models like Opus 4.6.

**Aakash Gupta** (00:59:58)

Also choose a benchmark where they have published these numbers, how they did on that benchmark. So give me two or three and then we'll go from there. So I can go and ask this quick question and it will go ahead and it will find me a benchmark which checks the model capability of doing question answering and doing reasoning. Once it gives me this benchmark, then I will check Then it says, okay, Mahesh, there's GPQA Diamond, Arc AGI, Abstract Reasoning, and Humanities Last Exam. Okay, so these are the benchmarks I got. And then I can see what is the score of that. And then I can say, hey, can you rank all the latest three model providers? Now, hey, can you take Humanities Last Exam and specifically look for The largest, biggest models like Opus Families 5.6, compare it to Gemini latest model and compare it to OpenAI models and give me how they did on humanities last exam.

**Aakash Gupta** (01:01:06)

So now what I'm doing is I'm saying on this benchmark, which checks for its reasoning capabilities or reasoning qualities, how am I doing Or what's my ceiling from the model layer when they tested the model on reasoning capabilities. They are saying Claude Opus 5.5 is 61%. Google is Argon, which they just released yesterday was 57%. GPT-Astra is 60%. So if you look at diamond subset, on reasoning capabilities, which requires a lot of judgment or a lawyer or a law bar exam like reasoning capabilities, The model cannot do more than the best model you have is at 61%. So I cannot set a task which requires a high reasoning effort like a lawyer to go more than 60% because the model has been failing four out of six times to come up with that kind of reasoning already. So that becomes my ceiling. So now I can say, if I have such a hard job, which humanity's last exam tests, Then I cannot go beyond 61%.

**Aakash Gupta** (01:02:16)

But if I'm just checking for answering question answers, hey, just check for GPQA with checks for question answering capabilities and go for the diamond one, which is the hardest benchmark. Give me the highest number across this family and put it in a table so I can compare. So that was for Reasoning capabilities. And that was the hardest benchmark. And I can now get a number. If you are doing reasoning that I can't go above 60%, that's the latest and greatest model can do. But now if I'm just checking for Q&A capabilities, then you can see the ceiling is at 96%, which is Google's latest for model. So I can achieve Q&A capabilities at a very high scale. But if I go and say I need A lawyer or a very high order thinking, like system 2, system 3 thinking, then my criteria cannot be more than 60%.

**Mahesh Yadav** (01:03:11)

If you're using humanities last exam, right? But I guess we constructed our own evals.

**Aakash Gupta** (01:03:16)

Correct. You constructed your own evals, but right now you have your own evals, but you want to see and give your team a dashboard or a target on your evals. Because if you concepted your own emails, you can't say that, hey, pass everything 100% of the time, else I'm not launching. If you set it like that, you will never launch. You have to give your team a room that, hey, this is our criteria and it's okay for us to launch at 70%. I am okay if you miss us three out of 10 times because our customers today don't have a way to automatically get risks. And even if we miss it three times or if we meet our high bar, doesn't meet that three times, it's still well. Like Opus 5.6 is super valuable to you, even if it is 60% as humanity's last examined reason.

**Aakash Gupta** (01:04:13)

So you set up your own evals, but your criteria cannot be 100% because that if you set it too high, you are never going to achieve it. And you are relying on the trajectory of these models to get better with time. So you have set the hardest criteria. So this is your humanities last exam, which you are setting up, which test your hardness capability to reason along. And you are setting the hardest exam for your agent. And then you don't want to go above the ceiling, which exists today for humanities last exam, just for an example.

**Mahesh Yadav** (01:04:55)

So basically, if your agent is going past the ceiling, you need to make your test harder. Is that what I'm hearing?

**Aakash Gupta** (01:05:02)

Yes, yes, yes. So you got it. So that's my ceiling. And my assumption or my hypothesis here was that my complexity of finding risk is same as humanity's last exam. But if you see that you're at like 90%, then maybe... Humanity's Last Exam has much harder questions on legal PhD level tests or physics level tests than what you are doing as a lawyer by taking a playbook and comparing and saying, does this match or not? Which basically is like type one problem, not even type two problem. So maybe Humanity's Last Exam does not apply. The complexity is lower. So then you can go and find another benchmark like which I was showing you GPQA question answering. Diamond level. And there you can take the ceiling as not 60, 70, 60%, but 96%, right? So if your job is, your agent capability is not doing deductive reasoning, like humanity's last exam, which you found out, you thought it is humanity's last exam, you set it up lower.

**Aakash Gupta** (01:06:11)

But reality was seeing it 90, 90%. Then you looked at humanity's last exam questions in legal, you saw your And then you say, no, no, no, actually the right benchmark should be GPQA Diamond. And then you say the criteria is 96%. Does that make sense?

**Mahesh Yadav** (01:06:28)

Got it. So how do we build these? How do we operationalize this beyond a spreadsheet?

**Aakash Gupta** (01:06:35)

Great question. So now Akash is saying, Mahesh, this is great. You set up the criteria, you created the questions and now how are you going to go and actually Productionize it because in production, he will get maybe 100 contracts. And if we're going to take on every risk, it comes out on an average, every contract has 20 risks. And now I am evaluating maybe 50 questions per risk. That means every risk is now I have 1000 questions to be answered per contract by a human lawyer. And a human lawyer is charging you. This is the money that we used to charge at Bedrock. If you want us to hire a human expert to do your evaluations, the charges are 0.25 cents per question asked. So now you have thousand questions. So now you are paying me $250 per contract. And if you want me to evaluate 100 contracts, then you are paying me 250K.

**Aakash Gupta** (01:07:41)

25k. Just 100 contracts. And if you do it for 10 days, my bill is 250k. So, Akash is saying, Mahesh, are you crazy? I can set it up in the beginning. I can do it. I can have a human lawyer do it for 10 for us for free because there are lawyers. Or I can even get an expert. I have some budget because it's quality. It's important. We always spend money on testing and doing our work, checking our work, security, safety. So I can justify that budget, but Mahesh, go away. I'm not doing 100 contracts, 10 days, every 10 weeks even. That's what it will take for you to go and improve this quality at least 10 to, at least you will need 20 weeks of quality hill climbing and testing these contracts and again and again to meet these numbers. So if you're going to do that, your budget is 500k to run these.

**Aakash Gupta** (01:08:33)

Who has a half a million dollars to run emails? So what's the next step? Which is what we were discussing. So now all of you can understand the first step of setting emails, which is talk to your customers or look into your own places and find out what is helpful, what is honest, what is harmless. Okay. I set up the criteria. I set up the questions for HHH and I set the criteria for success. Which is 65%, 70%, 5%. Then I need to scale it. Okay, how can you scale your agents? For that, you need to have LLM as judges or Azure AI Foundry release a lot of LLM as judges which are already tested in production and available for you not to build your own, but you can take theirs. So how can you use Azure AI Foundry AI Evaluation Suite Rather than building some random arise, arise, or some other crap, you can just use the cloud providers all the way, Bedrock in AWS, Azure in AI Foundry in Azure, or GCP evals, I think are much more exhaustive, much more scalable, and much more production ready than any startup out there.

**Aakash Gupta** (01:09:58)

And no offense to them, it just... They have not solved anything new, which is already solved now by common cloud providers. Okay. How does that word looks like? So now I have my agent. So now if you build an agent in AI Foundry or if you have traces of the agent, so you can build an agent. We build this agent inside Foundry. You are an advanced contract designed to help legal procurement compliance team to analyze contract. Your responsibilities are these. You're looking for these terms. You need to find risky non-standard clauses. Exact same agent. We build in Foundry and you can just specify your prompts. You can bring your knowledge. You can add your memory. But building is easy. So we're not going to cover building today, but let's say you launch it and then people are using this. So you will have a lot of traces.

**Aakash Gupta** (01:10:49)

So we have launched this agent in production and now people are coming and talking to us. So you can go ahead and you can set up your evaluations. What is? So you can look at all these criteria or you have these quality evaluations. This check for either the answer is complete. Is the Retrieval Evaluator, is it based, it is honest because the answer is based on the playbook or the contract and it has not gone and drafted it. This one selects whether the tool selection was correct, tool called success criteria and then you have different criteria for safeties, quality, honesty and harmlessness. Quality maps to both honesty and helpfulness and safety guardrails meet to your harmlessness. So most of the questions you are asking and getting manual answers and paying 25 cents can actually be found here in evaluations. So how can I set my evaluations?

**Aakash Gupta** (01:11:48)

You go to Azure, you go to evaluations, you say, create my evaluations. You say, I'm going to do agent evaluations. You can actually do model or just data set. Say, I want to evaluate my agent. Then you can select your agent or you can bring the data set from your agent, which is nothing but your question answers. So I just created this data set. If you want to look at it, This is my dataset where this was the query that was sent to me. You are an advanced agent. Here is a contract. Find me risk. And this was the response that it gave me that these are the risks. These are the clauses. And these are the tools that it called. And this is the metadata of what is the state of that thing at that time. So either you can get your agent's query responses and what tools and what state, or you can just say, Evaluate my agent if you build it using Azure Foundry.

**Aakash Gupta** (01:12:41)

I select agent or I could have selected data set. These are the two which are interesting. Model is you are just evaluating your model and not your agent. You say next. You can evaluate full conversation if you go back and forth with agent in a conversation or you can just say individual turns. In our case, we just had one. We uploaded the contract and said give me risk and it gave us risk. So I'm going to just take individual turns. Then it says, hey, do you want me to do it one time or do you want to set it up? I can test it every day based on new traces or new data set. I can keep running it as you are improving and keep telling you how are you doing. I just say one time. And then data is interesting. It can generate your synthetic data or you can bring your existing data set, which is what I was showing you earlier.

**Aakash Gupta** (01:13:28)

So if your agent is already there, you can just bring the conversations, the input you gave or the output you got. So this is my contract and this is the risks it provided me. Or you can use existing traces. What is that? That if you build the agent inside Foundry, then you can say, hey, just look at and intelligently find conversations from my agent across different sampling. So this is intelligent sampling where I'm just finding the right different kind of conversations rather than just taking top 100 conversations. If everybody asks for refund, then I'm just evaluating one kind of conversation. So they've indirectly find The right conversation, different kind. So give you different kind of judges, your different kind of traces or different kind of conversations your agent had. And then you are basically set. So I just selected. Then you select your model. This is the model your judge or this agent will use.

**Aakash Gupta** (01:14:24)

So you want to select better model than what you used in the agent. So you can select a better model, but more better model will also cost you more. So I will just set it up for GPT 4.1 or GPT 5. Nano ideally, and then I will hit review and that's it. And now if you look at the criteria piece, then in your criteria, you can also see all those evaluators here. It also recommends you the text for violence, tool use, sexual content, hate and fairness, output quality, self-harm. These are all built-in agents. So you can go and check. So these are all the quality things that it can check. It can check for sensitivity, data leakage. It can check if you are looking for a certain thing in your ground truth versus what you have reality. So I can say this one, and then it can check for coherence.

**Aakash Gupta** (01:15:17)

It can text for text similarity. It can check if the particular... Answer has the string or not. It can score the model quality specific, a broader umbrella cut. If it goes through a probated action and all. So you got all these, you can just choose right now and you can create your own custom ones also. So I have gone ahead and created a few custom ones, which I said, Hey, for me, this completeness means that it has that data, which are in my criteria and I can create a custom evaluator also. So The things that I'm evaluating, I will create my custom evaluator if they don't exist here or I will choose different agents like is it doing tool calling successfully? Is it adhering to tools? All these like inside my agent evaluations I can pick out of box and if it is not there, I can build my custom also.

**Aakash Gupta** (01:16:11)

That is it. Once you do, you create your agent and if you have done that, you can run your evaluations. How it looks once you have done your evaluations, it goes ahead, it evaluates and gives you score across all these things. Across different dimensions and marks it yes or no. So you can look at similarity. And when you do it, it says, okay, I got this. And if you click on it, you will see all the details that, hey, this, what is the customer name? This was the customer name. It passed the coherence test. It passed the fluency test. And wherever it says pass, you can mark your sheet yes. And it says fail. You can mark it no. So now you have gone ahead and scaled your thing. And now it runs automatically every day. And the cost has gone from 25 cents per answer to 0.025 cents.

**Aakash Gupta** (01:17:06)

So you have reduced the cost 100X. That means now it costs you $5,000 rather than 500K.

**Mahesh Yadav** (01:17:16)

How do you eval the evals? How do you make sure that this is as good or better than what you were getting from the human lawyer?

**Aakash Gupta** (01:17:24)

Very good question. So what happens is you're saying, okay, you put the evaluator, you have your human lawyer. Now your evaluator is filling the sheet with yes, no, based on that pass, fail criteria. And you have the criteria for humans also. So I have these questions like, hey, is this complete? Does it do excessive redlining or not? And does it do excessive redlining? Does it change the clause? Does the clause remain grammatically correct? And let's say my layer said, no, yes, no. Right? And then I ran it with evaluators and evaluator came back and said, yes, no, no. Make sense? So I got my answers from here. Then we do something called a precision and recall of LLMs. What is precision and recall or what is this idea? So this idea is let's Let's talk about that. So what you do is you figure out and set the criteria before you put this LLM judge to production.

**Aakash Gupta** (01:18:31)

You say, hey, if this matches, that's a true positive. If it doesn't match, it's a false positive. Make sense? And then you can say, hey, the number of true positives devised by false positive and true positives is your precision. So now you are looking for more true positives and less false positives. Because you are penalizing false positives. So in this case, my precision is this one is true positive, one true positive divided by one, my false positives. How many false positives I have? One and two. So one and two. So I have two plus one. So I have 33% precision. Generally, that criteria needs to be more than 80% before you can go and deploy. So you also set that criteria for LLM judges because otherwise you are just Doing some hallucinated work. If they say yes, yes, yes, then you say it's passed because you don't have this anymore and you want to trust this.

**Aakash Gupta** (01:19:36)

So before you put your Azure AI evaluator to production, you want to compare it with the human and ensure that this precision number, which is true positive divided by false positive by true positive is above 80%. And if it is not, you tell your teams that we cannot scale our evaluations.

**Mahesh Yadav** (01:19:54)

And what about recall?

**Aakash Gupta** (01:19:56)

Yeah, the recalls, the idea is that you're going to go. So true positive, false positive. Then you have true negatives and false negatives. So the idea is that, hey, instead of penalizing your false positive, I am trying to get false negative out, which does not apply a lot here. But the idea was that false negative is something that I said is going to happen, but it doesn't happen. So if for a song like let's say for an example I'm predicting whether you will like this song or not and I propose this song from a list of hundred songs but if it is not there so I said you will not like it which is not true because in your list the song is there but if I produce it if I don't put it in the list It's a false negative. I know you're just nodding your head, but we need to double click on that a little bit more.

**Aakash Gupta** (01:20:51)

But in this case, just go with precision, which is, hey, do we have a true higher true positive rate or this matching of human? And then you can set the criteria. And if the criteria matches, then you are good to go. And the idea of recall is that instead of false positive, false negative, which is this idea that let's take a song idea if you want to double click on that. So let's say you are doing a prediction of songs. Given 100 songs, you need to put 10 songs in my playlist. So you are saying song one, song two, song three, song 10. That's my agent job. My agent predicts these songs. Cool. So now if I have these songs, Then if I say, hey, this song should be there out of 100, but the user also has their own song out of those 100. That's your ground truth.

**Aakash Gupta** (01:21:47)

That's your lawyer answers in above case. So they have this song called S1, S21, S3, S4. So if you don't even put it in my list, then it's a false negative that you failed to recall that thing. But if you put it and I didn't like it, it's not there. Then you miss my false positive. So if you do the criteria, which is, hey, is this value here? So my prediction versus my actual, if both are true, then true positive. If my prediction says, yes, it should be there, but my actual is not, then false positive. If my prediction says, That hey, it should not be there and it's actually not there, then true negative. But if my prediction says that hey, the song should not be there, but the song is there, then it falls negative. And precision is trying to minimize false positives, but this is going to remove the false negatives.

**Aakash Gupta** (01:22:57)

So the idea is that this can be explained better with the risk example. So I gave you risks in a contract. I said, here are 10 risks. And out of those 10 risks, actually five are the real risks and five are not the real risks. Right. So I have five true positive, five false positives. I am 50% precise. Right. But instead of giving 10, I gave you 80 risks. And all the 10 are there. Right. So I have my what my precision in that case is 100%. If you got true positives, which is 10, and my false positives is 0, my precision is 100% because I only am checking for what I got. So I gave you 80 risks and out of those, those 10 risks, which were actually there, were there. So now I got 100% precision. But what kind of product is this? It throws 80 risks at it, at me.

**Aakash Gupta** (01:24:05)

And I need to fish through those 10 that are there. So then we put recall and recall is saying, yes, you got 10 correct. 10 positive. Good job. But you have 70 that are false negatives. So I am going to penalize the false negatives that you said that, hey, these are not supposed to be there, but they're there and I will add it. And now I have my number as I have only 15% recall that because I'm throwing 80 things, actually I'm able to recall only 10 out of those 80. So I have a very bad recall. So you want to measure both precision and recall to cover for your agent to not give you too many things to just get things right because you don't want to overwhelm the user with too many things. And at the same time, when you go shorten this, you want to hit the target also.

**Aakash Gupta** (01:25:07)

So you want to measure both false positive and false negatives. And the precision and recall is a way to control both of them. Because if you say, hey, I want to get only few options, but then your recall will be awesome. But then your precision will go lower because then you have very less window. You're going to give me only 15 options. Then finding that 10 will be harder in those 15. But at the same time, you can say, oh, Mahesh, actually give me a higher recall. Give me 100 things. And then you can find this 10 easy. So your research team or your engineering team will ask you as a PM that do you want a higher precision and recall? Because I can't do both. And as a product manager, you need to decide what is Important in that criteria. And that's what I was saying when I said in this one, let's just focus on precision.

**Aakash Gupta** (01:25:57)

Let's not worry about recall because we have already restricted the number of option to yes and no hair. So I can just focus on precision. And if I'm getting a higher precision, there is no room for recall because that's applies to how many risks I'm getting. But here risks are already there. I'm just checking if this answer is matching or not.

**Mahesh Yadav** (01:26:19)

Let's say I'm somebody who's new to evals. I'm following along so far. I understood the three H's. I understand, let's say we create the 25 questions. So each one of those gets 4%. I understand I set the difficulty so that it matches a public eval. So it's maybe in the 60 to 90% success range. I understand that I verify that with a human reviewer. I create an LLM judge. Now the part where I'm getting confused is we just layered in precision and recall for this LLM judge on top of the 3H. So maybe you are a master of simplification. Can you simplify? How do I understand how this all comes together?

**Aakash Gupta** (01:26:58)

Let's look at, forget about precision and recall. And we were not going to put it. So what you need to check is you're just checking how much of what your evaluators evaluate compared to what a human did and finding the accuracy of it. Forget precision and recall. It's that easy when you have a mood. So forget precision and recall. And let's just check the accuracy of your AI evaluator or LLM as a judge, right? And how you do that? You just take whenever this matches and you say, hey, if it matches, good. So how many matches? Matches are one. How many mismatches? Two. You're 50% accurate. So that can be one criteria. You can just lead with that criteria. But the good part is you want to know from here That, hey, you know what? I can be 50%, but I also, if you look at this, you're 50%, but you actually got something right also, right?

**Aakash Gupta** (01:28:07)

If I just go with this, you are saying, hey, half of the time you're wrong, which is not true. Because if you look at this, I have evaluated three things and I'm not getting rewarded for one thing I got right, which is this one, right? And that's why I have to give you that false positive and true positive equation. So that what I did is I said, hey, this and this is false positive. So false positive one. This and this is true positive one. This and this is false positive. Right. And then I calculated a new number. I said, I am not going to go and calculate this. Actually, I could have just 1 by 3 and then give you 33% also. So you can just use accuracy here. But the idea is that if I go now, I say false positives plus true positives, which is 3, I give you 66%, which is the true number.

**Aakash Gupta** (01:29:12)

But if I go and do this calculation, which is accuracy, which can be actually three hairs, so you can just get that. So just forget what precision and recall for these for the time being, and we'll just leave with accuracy.

**Mahesh Yadav** (01:29:24)

Okay, so simplify with accuracy and get it to 100%?

**Aakash Gupta** (01:29:29)

80% is good enough because you are trying to reduce the cost. And if you're going to reduce the cost, then you want to make sure that your cost is... Manageable because now you're shifting the burden of costing and building an awesome agent to building an awesome evaluator and you will be spending a lot of money improving the quality of your evaluator. So give it 80% and 80% is good enough for us to go roll out. That's the criteria we have used somewhere around 70, 80%. And that allows you to get enough of problems for you to go fix. And even if it misses 2%, you're doing it every day and you augment this with human evals also. So you are not going to just go and evaluate everything by these agents. You're still going to go and do human evals on 200 to 1000 samples every week.

**Aakash Gupta** (01:30:22)

Why do that? Because these evaluators only know the helpfulness, honest and harmless, which you learned in the beginning of your product. There are new things that are happening. People are asking you new questions and you are learning how your agent is behaving on those. And maybe it's not fitting your criteria. Maybe thumbs down comes up with new things. These LLMS judges are going to judge only what you have set up. They're not come up with new ideas or remove things that are always yes, yes, yes, yes, yes from your evals because there's no point testing it anymore. You want to keep and cut it so that you come up and test and then you take these, these answers that you got and you compare it with your evaluator. And live every week check, does your evaluator still behaving the one you tested in the beginning? And make sure that it remains in that 70 to 80% range.

**Aakash Gupta** (01:31:24)

So three steps as you scale. So if you want to scale your emails, then what you're doing is first find the LLM judges or AI evaluators in foundry that I showed you. Then get these LLM evaluators going. Then you are setting them for your accuracy of these and testing it to 70% and plus accuracy. Once you reach that, then you are also evaluating 200 to 1000 by humans and making sure that this remains consistent week on week and you have not gone bad or diverged because new, new conversations start happening. And this will also help you redefine your criteria for helpful, honest, and harmless.

**Mahesh Yadav** (01:32:08)

Makes sense. So this is how you actually build app production in evals. Where do people make mistakes in setting this up?

**Aakash Gupta** (01:32:15)

Yeah. So there are a lot of people, what they do is they take an LLM judge and never evaluate the quality of it. And they just say, Hey, here is my LLM as judge. And then say, yeah, because it's an LLM and because it's a judge and because it gives me results and It's very visual and it says completeness 100% green. Just trust it. They take a screenshot of it and then say we have achieved Nirvana. That's number one. Another thing people don't do is they don't reduce the criteria of their evaluators enough. So they are asking a broader question, which is like, hey, is this helpful? Yeah, it's not helpful. Then your SME may say this is why it's not helpful. And then you're going to make it helpful. Helpful is such a broader term. You need to break it down. What does helpful means?

**Aakash Gupta** (01:33:02)

And people don't do enough work in breaking down what does that helpful means to the last level of questions that anybody can say binary yes and no. And the explanation makes sense for a person who's going to go and improve it. So people don't break it down their evaluations big enough. That's one challenge in these evals. Then what I have seen also is that Okay, you have an LLM as a judge, you have your evaluators and tell people forget this manual step. They never go and check manually. Don't put the effort and energy. Without that, they are flying blind. And when this deteriorates, it was in the beginning 70%. But as you get real queries, your real queries are discovering or giving you even more challenges. And actually this has dropped to 20% week on week on week 10. So we keep hearing all about these new instant decision models, which are

**Mahesh Yadav** (01:34:19)

AI models, but they're not LLMs. Microsoft released its decision model. TypeSafe AI released JEV. On the back of that, they just got a $10 billion valuation. Cloudflare released their own. How can these new decision models help us in our evals? I think you had previewed that they could reduce the cost, maybe even the time. How should people be thinking about decision models and evals?

**Aakash Gupta** (01:34:45)

That's a great questions. And this is the new thing that we're going to unclose or unbox this time. So now you are looking at it and you are saying Mahesh, it cost me 25K and six hours to run my evals every week, even with Azure evaluators. And by the way, these are decisions Or yes, no questions because you have done the hard work of putting what is helpful into a simple question. Is this clause after modification? Follow all grammar rules. Answer is yes or no. Okay. It's a decision. So what TypeSafe JAV does or what decision models from OpenAI or Microsoft are doing is they are saying that hey, LLMs are trained with RLHF. To generate text that human love, generate text or create answers or summarizations based on human feedback. That means there's no way to go and build confidence in this because that also is a new because if you give me the answers, then you can give me the confidence and the confidence will also be a next word predictor, which is also trained with RLHF.

**Aakash Gupta** (01:36:05)

So it's human preference and not an objective truth. So yes, I can get answers from LLMs, which is in our evaluators, yes, no, whether it does it or not. But if I want to know with what confidence you are sure that yes, this clause is not meant, then it doesn't give me any confidence today. And even if I say, give me a confidence in my prompt, it will hallucinate on the confidence also. So now, This is because we have used RLHF, which is this idea that you will take humans to build a reward model and then you will use that reward model to incentivize your RL policy to behave like humans. So if human says, I'm confident, the model says, I'm super confident. And as you have seen all along, humans are very confident people. So that same bias is in here. And if you're going to go and ask it for confidence, you can get the answer, but you can never get the right confidence.

**Aakash Gupta** (01:37:08)

Without right confidence, you cannot go and say these evils needs to be reviewed by a human lawyer. Remember, I am taking random 2000 to 3000 because I cannot trust my LLM judge to tell me when it has gone wrong. If I can, then my right Right eval should be that I want to go and say, hey, AI evaluator or my LLM as a judge, give me an answer yes or no. And when you do that, also give me a confidence of how good you are. Make sense? And if the confidence is low, lower than 70%, I want these 200 to 1000 to be evaluated by humans. Which will be a perfect eval setup. But I can't do that with LLMs today. And types have said that you cannot do it with anything, by the way, because these LLMs are here to please you. Why? Because the technique we used is to generate the next word with human preference.

**Aakash Gupta** (01:38:22)

This human preference, which we encoded in the human feedback, It's used in the reward model and the reward model was optimized to do reinforcement learning. So it doesn't know what is a confidence. It doesn't do probability distribution or any math. It's what whatever human codes in it and human codes. Confidence is just a word for them. So they came up and use the techniques called reinforcement learning with RLCD, which is this idea that, hey, I am going to go a new training method. And with that training method, what I'm going to do is I am going to do reinforcement learning this one, but on distributions rather than human feedback. That means you need to tell me first, I cannot do generation text or anything because I don't know because I don't know what the answer is. But if you give me the choices, yes or no, Whether the contract is an NDA, MSA or Data Privacy Agreement.

**Aakash Gupta** (01:39:36)

I can tell you based on these questions. So in JAV, you need to provide the state, the context. Then you need to provide me the question and then you need to set up your choices, your score or whether you need yes, no answers. You need to first tell me what is the context. What kind of question you are asking me? And then you need to give me these options also. In choices, I can upload a contract and ask whether it's an NDA and I can say what kind of things are NDAs. I need to define what is an MSA. I need to define what is a DPA. And then all this model is trained to do is given these distribution, it gives me the best possible answer out of these based on what is as seen here. So it's a different technique of training. And when it does that, it also gives me a confidence which they claim that you can trust 99% which is more than what you could do with LLMs.

**Aakash Gupta** (01:40:42)

So finally, for last two months or so, we have a way to actually get the answers if we set our questions and state correctly and get the confidence value. And because it's not an LLM which has a job of human preferences, training, generation, all the crap, it can be a very small model or comparatively small model and it can run very fast. So what we did is we took the evals, what we just did with AI evaluators, and we set it up for GEL. And I want to show you rather than talk about it and show you that how it actually worked. So what we did, we already showed you that, hey, we have run these in Azure and we saw awesome results. So we set up this criteria. We set up these quality evaluators in Azure. We can go and set up these evaluations. I showed you all this.

**Aakash Gupta** (01:41:46)

We get the results. Now we have reduced our cost by 100x. Azure has built-in evaluators. You can also set up different criterias for monitoring these. So you can go and say, hey, if this particular evaluator value is going less than 5%, like let's say some people are sending security-specific harmless questions and your value is more than you are answering bad, you can also get alerts. So all this we discussed, you can set it live. You can also set up monitoring and configure live evaluations. So that was AI evaluators. Then we said, hey, instead of this, let's use the same sheet that we were producing. So I created the same sheet. I put my answers. And what I did is in Claude, I installed Jeb plugin. In there, if you go to their website, you can see Jeff's plugin. And I went ahead in customize. I went to plugins and I installed this plugin.

**Aakash Gupta** (01:42:45)

We'll give you a lab which shows you how can you get this type safe plugin. And now I can go and ask this plugin a question or upload my sheet and ask this guy to put that yes and no evaluations. And that's exactly what I did. What I did is for this demo today, I said, hey, I'm going to give you my APIs for Java, so we'll rotate them. But the idea is that, hey, understand Java, use the documentation, verify the connection. And once you have done that, for every Java call, output token, use this cost and save the skill. So I created a skill that allows me to go do evaluations. Then what I did is it said, okay, I've got it. I tried it. I got a skill called Java Evaluate. So I created a Jev evaluation skill and then I gave my same questions, this word adding analysis, which is exactly same what I had here.

**Aakash Gupta** (01:43:46)

And I said, Hey, take this contract. This is the contract name. This is the removed part. This is the added part. This was the playbook that it is based on. And then I created the evals for Jev saying, Jev use this. Build your context using row this, this, this, and then answer my questions in these cells and judge only single red line in row. And I gave it all my instructions to go do the judgment, gave it some example and just tell me yes and no probabilities. Cool. And then I said, if the confidence is less than 70%, then just ask for human review else just market. So It went ahead and it created my all red lines and it created the answers and it said okay and give me cost and time also. Then I actually gave it the answer keys, the human ones, the human lawyer ones and I said hey tell me how good you did and here are our results.

**Aakash Gupta** (01:44:51)

So Jeb took 214 seconds, JAV API cost not only that 25K, but reduce it now another 100K. So if you cost 25K, now it costs only $250 to run and it meets the accuracy. This was the same exact number we had with Azure. Azure AI evaluators were also failing on accuracy. It got only three failures there. Then JAV predictions of 20 years and two no's. So I got all my predictions and there are two that are not matching with human evals. And for each, I'm getting a confidence. Also, when it doesn't match, my confidence was not above 70%. And then I can see the second match. So I can put my criteria around 60% or so. And if it is less than that, I can ask for human reviews. So this is my evals. And then I ran it with Jeff. And if I ran it with Jeff, Then I can show you the comparison.

**Aakash Gupta** (01:45:53)

So we set up same criteria. We ran the same questions. We got our answers, which I was showing you. And then we did a comparisons on our emails compared to Claude. We also asked the same questions to Claude without Jeff. And then we said, use the GEV scale, which calls the GEV model to do the evals. And then we also compared the same with Azure AI evaluators. And you can see that the time is basically 1 10th or 20th than what this takes and 50 X lesser, same as cost. The cost is reduced by a hundred times and the token consumption. So JEV is the new way to go set up your evals and it meets the same quality. And on top of it, it gives you the confidence you need.

**Mahesh Yadav** (01:46:43)

And I'm pretty sure Microsoft will add their decision model to Azure. So you can probably see those costs come down soon too.

**Aakash Gupta** (01:46:50)

Correct. So it is not JEV's proprietary RLCD. The magic is the RLCD, which is reinforcement learning with common distribution. That's what is calling RLCD. Or making it possible for us to do these things in a new way because the LLM judge is making decisions. And decision models make the cost, time and gives you confidence. And if you have not done or not restarted your evaluations with RLCD based decision models, whether they are JEB, whether that's OpenAI Decision API or Azure Decision API, you are basically doing a lot of Costly evals which needs to be rewritten. That's our hypothesis. We are still validating it. So very early stage. We only got JAWS access last month and we are running a few cycles. We're very excited about what we have seen. We will let you know if something changes. But today I highly recommend everybody to go ahead and apply JEV to their evals and see if they can meet the same accuracy bar first.

**Aakash Gupta** (01:47:58)

And if it does, then move to JEV because JEV is going to cost you 1000x less, run faster and set the criteria of when to bring the human experts.

**Mahesh Yadav** (01:48:07)

So throughout this process, what are the components that a PM owns versus an engineer? What is the set of meetings I'm having with my engineering team across the lifecycle of this eval? Am I as the PM the one who's checking out, okay, the cost, time, and accuracy of Microsoft's decision model is better than GPT 5.5? So I want to switch to that.

**Aakash Gupta** (01:48:32)

Yeah. So you as a product manager owns the metrics. So what's the division of the cost? So I have, so your job is to make sure that, hey, so first of all, you as the product managers need to first come up with the criteria and questions. Same page. So this is nobody's job. You are updating the helpful, honest, harmless questions and you are setting the criteria. Got it. Then in this dimension, you are setting the cost targets and saying week on week, I want the cost of evals to reduce by 30%. You can say month on month. Week on week is a little harder. So month on month, I want to reduce the cost of evals by 30%. Because I want to go and give more tokens to my customers. That means right now we are spending that $250k first. Then we are spending $25k. And then with Jav, we are spending only $250.

**Aakash Gupta** (01:49:35)

Right? So if you set the criteria like this, this gives you a lever to have a meeting with your engineering and say, what are you doing about it? And smart engineers will do it what you did. Which is did the research, tried it, and it was not very hard. You saw that I can just create APIs in Java and we will give you a lab for it. And then run it in Claude and just give a prompt and a skill and it does the work for you. And you already have your sheet set up. So you are just giving and then you can show them that this is a art of possibilities. But you need not to. It's your engineering job to scale your evals and reduce the cost of it. Your job is to set this criteria. Which is, I want the cost of evals to reduce by 30 to 50% month on month.

**Aakash Gupta** (01:50:23)

Once you have set up, you will set up meetings. And in those meetings, you will say, hey guys, this is the cost last month. Are we going to meet or beat this target? And they say, Maesh, we're going to not meet this target. Then I'm saying, okay, what you tried? And they say, we tried nothing. Then I say, I can understand you guys are busy. Let me show you what I tried with Jev. And I don't know it will work, but seems exciting, guys. Are you excited? And then some of them will say, oh, but Jev, nobody knows it. We are on Azure. Azure doesn't have this. We can't use an open source model. You listen to that. You don't question. This is their territory. Then you wait for Azure. And then you say, hey, guys, I saw this Azure decision model. Do you want to try this?

**Aakash Gupta** (01:51:14)

And some guy will say, oh, Actually, Mahesh was not stupid. What he said, I tried it and it works for me. And next month he comes to you and says, hey, I took the OpenAI or Azure decision model and I reduce and beat this target by 1000% by reducing the cost 100x. And you gave them the ideas. You are basically the brainchild. You are the fountainhead in the team, which is giving all the ideas. But they are the ones who owns the evals and are responsible. But you are the one who is setting that this cost of eval cannot continue to increase. And I start with the humans. Then you give me Azure evaluators. Then you keep researching best way to do it. And if the best way to do it is decision models, then why are you not doing that? And if they are not, then you can go ahead and do it and show them the way.

**Aakash Gupta** (01:52:11)

So your job is set the criteria. Keep the cost and accuracy functions and set weekly or monthly targets on those and then have discussions. So the latest, greatest edge of AI is also in your products. And that's your new AI PM job.

**Mahesh Yadav** (01:52:29)

How important is this to the AI PM job? Is this like the biggest change in AI PM? Is this going to determine the success of your performance reviews? Is this what you're spending 30, 40% of your time on? What's the right context to understand this skill?

**Aakash Gupta** (01:52:44)

Great. So 40% of 40 to 45% of your new PM job is basically setting and evaluating your responses, those 200 to 1000. So I used to spend two days or I still spend two days looking at our evals. That means 40% What is the cost of evals? What are the problems I'm getting? And then bucketizing them behind the scenes with different teams, different agents, and having this discussion of, hey guys, we need to meet our criteria. So this was the another lever you have, right? That, hey, we have gone from 65% to 30% as we added this new customer. And then these are the buckets of problem. These are the helpful questions we are feeling more often that is causing this to happen. And then you create the data set and then you assign a Jira ticket to them saying, hey, I need it back at 65%.

**Aakash Gupta** (01:53:42)

Otherwise, I can't sell to this customer. So that's your daily routine or that daily rituals where 40% of your time is going into looking at your evals and seeing if they meet and meet the criteria that you have set up. And when not set up, you are providing all the requirements for the team to succeed downstream. And that is table stakes. The good PMs who are going to thrive in this world are also giving their teams ideas on how can they achieve this. Then they are also saying, hey, I saw that we have started failing on reasoning models and I saw that you guys are using F5.1 nano. Can we have open router specific logic that allows us to check whether it is a reasoning or non-reasoning call? And based on that, can we route some of this to 5.6? I know it will increase our cost, but that's one way I read on this paper that it can be done.

**Aakash Gupta** (01:54:39)

And you just stay there and you write like disclaimer. This does not mean I am recommending you how to do this. I read it, just wanted to share. And these are the PMs engineer wants to work with. Their life is so hard already. They have to figure out reliability, working and all that. And they don't have time to read all this. They may not even understand all this to the level you have. Half of your team is new to AR or even 80% they are new to AR. And if you cannot be the fountainhead or brain for this AI team, you're not going to ship products which succeed in customer hands. And that's why you will not have ROI in your agents compared to my agents. And that's why you won't be successful because you will not create the customer value I will create. Because I am guiding and leading my teams.

**Aakash Gupta** (01:55:33)

And that's the new AI PM or new builder role. That's what these guys like. If you listen to them, they are saying, we are doing that job. We are not coding. We are figuring out how our code is doing, where we are failing. Then we are looking at latest, greatest research and figuring out where we can pass again. And that's the iteration. We only have few cloud code type PMs who are always, by the way, the guy also worked as a PM. So he knows that he need to go do this job of finding out where things are failing for customers, have that empathy, and then bring that back to the way. And he has the research background so he can fill that gap. Can you fill the first and you need not to worry about the implementation? That's the new role.

**Mahesh Yadav** (01:56:20)

My biggest sort of challenge with all the evals content out there is that I don't understand why... The PM like owns the criteria and then doesn't implement the eval. Because as you said, it's so easy in these new harnesses to implement the eval. You can even just have a clawed browser use, set up all this stuff on Azure Foundry, which you had it set up. Through natural language prompts, you can do all of the evals. You can have it measure accuracy. If you want to throw away precision recall, you can throw away that, but you can also keep that. You can have it do all of that while being the same person that says the criteria. We could actually build the evals very easily now. And in the same way, the engineer could build the criteria and do the PM role. Like what's the point of the separation?

**Mahesh Yadav** (01:57:11)

Why do we have the separation? Is that just an artifact of the old roles? Are we just trying to justify the AI PM for no reason?

**Aakash Gupta** (01:57:18)

I think that's a very good question. The challenge is that eval, how you saw it also have code in it, also have prompts in it. That means they need to be checked in. That means they need to be maintained. That means you need to know the basic engineering tools like GitHub. Then you need to know like this foundry tools. Then you need to come up and do this structure reporting week on week on how you are doing and what you did to improve it and what additional tests you did to ensure. And PMs generally were abstracted from that kind of language, that kind of tool chain, that kind of tracking of continuous improvement. Like 90% of VMs don't know how to do GitHub check-ins or how to push code using Git-like tools. So the challenge is once you get into this continuous iteration where you are updating whether your system prompts of RLM evaluators or you are going and evaluating and setting the criteria on some basis like I was talking about reasoning, knowing what a human...

**Aakash Gupta** (01:58:22)

Humanities last exam is and all that. People don't have that. And I think that's the barrier. If you take that barrier away with cloud code, you need not to learn GitHub. GitHub is like kind of plugin and you can just say, check in this code and it does get pull, get push, get sync and all that. And you do not know, even if you get conflicts, it will go resolve them and do it for you. So if you If Claude Code or Claude Cowork becomes your new toolset, I see a very valid point that evals should be PM space and developing or writing the agent should be the right separation. And I think it's a great idea. It's just that we don't have enough capable PMs which are raising hands that saying that we will own the evals. And if you don't own it, everything that nobody owns falls to engineering.

**Aakash Gupta** (01:59:10)

And yes, it does have some engineering components like I need to maintain my evaluators, I need to improve my evaluators, which is same as maintaining my agent. So if you can actually build and maintain an agent, what is, evaluator, what is stopping you to go and build and maintain your agent? Because your agent is also a system prompt at this point. So that argument helps them win and say that these guys are not eligible. But if you want to have a team which have a very healthy relationship, you should give more and more control to the PM. I think that's a right logical new way of building these teams because then the evaluation is not biased towards what I wrote in the agent. And I don't even need to know that. And PM should be building evaluators for the competition and Us and just be an objective function inside of the team, which says this, I did exactly same thing with this competition or vanilla skill in Claude and your agent.

**Aakash Gupta** (02:00:10)

And these are the outcomes. And I will remain the creative mind to move it. But if you look at like what I did with Jav, there's code involved. You need to figure out how to set up Jav and all that, like the questions, the answers, you have to break it down. It's just the cognitive. Load that PMs kind of avoided for long and they continue to avoid. And that's why I don't think that it's going to go the way you and me are structuring it. But I think if we can change one thing, it's the right way to change it. And that's why I think more and more PMs are evaluated on how are you going to set up observability. Which is both the things which I talked about, that I'm going to set up these criterias first. And then these criterias will divide how you get to these evaluations.

**Aakash Gupta** (02:01:03)

And then I'm going to observe these continuously for the quality of the agent as well as the quality of responses it produces. And that will allow me to ship a high quality mode based products.

**Mahesh Yadav** (02:01:15)

All right. Somebody has watched this two-hour video. What is the light at the tunnel? What is the compensation? What can you actually stand to gain if you truly learned everything we just taught you about evals? If you go from, let's say, regular PM to

**Aakash Gupta** (02:01:35)

PM that is building AI features and AI evals. Great question. I know we have gone through everywhere. We started with how can you build easy agents? Then what do you need to do to evaluate intelligence? Forget about all this scaling, but what it takes to actually evaluate human-like intelligence. And then we said, actually, how can you scale it with existing tools, which are with every company like Azure Evaluators, rather than throwing something fancy at you. And then we said there is something new called Jeb. So I think five takeaways for you is, yes, there is a very structured, easy way to set up your evals, which is helpful, honest and harmless. Find the question, what does it means for your users and continuously update them. That's your new job. Then map those to the evaluators. And if it doesn't map, create custom evaluators to scale these and just know Just know right now that there is a way to 100x or 1000x reduce this cost with JEV and experiment with it.

**Aakash Gupta** (02:02:41)

And that's the four takeaways from today that building agents is easy. There is a structure way to set up your evals like human judgment, which test human judgment like agents. And there is a way to scale it with Azure. Decision models are going to be the next breakthrough to reduce the cost and give you the confidence that you need to automate evals which were not possible just six weeks ago.

**Mahesh Yadav** (02:03:08)

What is the compensation specifically that AIPMs can make? You've worked at Microsoft, Meta, these amazing companies, Amazon, Google. How much can you make working at these companies on these types of projects?

**Aakash Gupta** (02:03:24)

So if you are like talking about a principal level like level seven, level eight, even level six, we're looking at 750 to 1.2 million. If you're going to level seven upper band and level eight, we're looking at 1.5, 1.2 to $2 million. And if you take the stock options in and how they have multiplied easily, my friends are making 2.5 to 3 million. That's why our target is to make 3 million, which we were discussing yesterday, before we started the podcast, that I need to catch up with them. Because when I left, I was easily making north of 1.2 million. And I'm trying to see how can we meet and beat that number working outside. And that's a common number that you will make. And that's the compensation. The compensation of solving humanity's last problem Tech edge problems is that you will be the sought after PM and you can negotiate whatever price you think is right for your intuition because you are reducing the time it takes for them to go and ship agents with high quality.

**Aakash Gupta** (02:04:30)

You are also convincing their customers that it's not the right thing for them to do it themselves. They need your help and your company's help. And the cost of not hiring people like this or not hiring product managers with AI skills is that you will build vanilla agents and you will ship a lot of them, but you will never get your customers back. That's one. Second, you will never ship real good high quality agents because nobody knows how to set the criteria and scale those. Third, you will never be able to identify the right opportunities and price it right. Those two things we will talk some other day how to identify in the new world what's still left for agents to do or your company to build agents on and how to price this because pricing will be different for different customers, different agent workloads inside that customer or inside that workforce and this varies so fast Like we saw with decision models, how can you incentivize them or predict the future, right?

**Aakash Gupta** (02:05:35)

So you can give more than what your competition can give. And if you don't bring people with these skills and compensate them, the kind of compensation I'm talking about, you are not going to get the leverage in this new AI world, which I think is existential crisis for pretty much every company out there.

**Mahesh Yadav** (02:05:55)

What do these salaries look like across the globe? Because those sound to me like high cost of living salaries. And what really is the roadmap for someone to get a million dollars plus as a PM?

**Aakash Gupta** (02:06:10)

I think everywhere you need to, like if you look at my salary, it has in last three years, it has gone four times. So whatever your salary is, whatever your number is, I don't know how people get compensated in even India because I never got compensated. I only worked in very early careers before 2010 in India. So I don't know what the compensation numbers are in India, even although I'm from India and Europe. I have no clue because I never got paid in Europe. So whatever your number is, every year you can expect to make double out of it. And in four years, you should be getting two to three X if you switch to AI. So that's my first one. And what was your second question? So just take whatever number and if you come to AI, it will double or triple in next three years.

**Aakash Gupta** (02:06:55)

And if it is not, then you're missing the wave. And that's what the real compensation should be. And that's how you should position yourself because you want the top 5% talent and your company will be making 2 to 10x more. So you should be incentivized the same way to your people. It's not that you're just hiring these people and paying them more because AI is cool. It's because they are going to build these agents and give you this scale, give you this intelligence and give your customers a new way to look at their business, look at what they can offer. And that's going to produce 10 to 100x value. And that value should be given to the people who are going to make it happen to 2 to 3x. And that's what my equation says. And that's what I played out for all my friends who started in AI like 10 years ago.

**Aakash Gupta** (02:07:47)

And all of our compensated very well. They're working in research labs of entropic open AI matter.

**Mahesh Yadav** (02:07:53)

All right, you guys, he is here at six o'clock on a Friday talking about AI three hours into a podcast, and I'm going to ask him one last question, okay? So these numbers are just mind-blowing to many people. Like the average person who's watching my podcast, I would say, they might be making $150,000 to $200,000. They might be making 40 to 50 lakhs per annum. They might be making... In Europe, 80 to 100,000 euros a year. So the numbers you're talking about are just crazy. So if you're that person, you're that mid-level PM in that geography, what is Mahesh's roadmap? How do I go from 80,000 euros to 1 million USD?

**Aakash Gupta** (02:08:38)

Yeah. So I think first you need to understand how this agent harness actually, what is the agent harness and how is it built? That's the first thing. That's the basic. Ecosystem knowledge that might take you one to five days. Pick any harness like Cloud Code, Cowork and try to build agent with it. See the problem of context, actions and evaluations inside them. And you can just watch their logs when they do this and build a deep understanding of what is a harness and how a harness works. What are the limitations of an agent harness? That's your first five to three, five days to 15 days of work. Once you have figured that out, then figure out Where agentic AI actually deliver value and where it doesn't. And we have a framework where we say low cost of error to high cost of error on y-axis, explicit to tactical knowledge on x-axis.

**Aakash Gupta** (02:09:33)

And then you should be able to go to any company and say, here is a roadmap for you. To leverage AI. These are the things you should automate. This is where you should build a co-pilot. This is where you should build an audit agent. And this is where you should not do anything with AI because the cost of error is so high and the knowledge needed is so technical and the exams and the benchmarks are not going to meet any criteria. So you should be able to have that framework and build that AI product sense And that might require you five iterations in your industry with five examples and do that case study and publish that case study. Review that with your peers and the industry experts that you got it right. Those are the case studies that you will talk to in interviews when they say, hey, we have this, we are doing this.

**Aakash Gupta** (02:10:26)

It doesn't work. OpenAI is doing the same thing. How can we scale? And then you can show, oh, I have seen this problem. Let me show you. You are doing this wrong. This is not a co-pilot. This you should go automate. This is not an automation criteria. This needs to remain with humans. You can just help them with analytics to make this call. You're making the wrong choices. And here is my framework. And this is how I will make or restructure your AI investments. You need to become that. That's your next five case studies might take you where you are from once you understand the hardness to do. And if you do that, then you have another 15 days. You do one case study in three days, 15 days of work there. So 10 days of hardness, 15 days of that. Once you reach that, then you should be able to talk about evals, which we just talked about.

**Aakash Gupta** (02:11:19)

So yes, you understand Harness, you can identify and create roadmaps for these companies on how and where should they put their bets. Then you should set up these evals and talk about evals. So watch our three hours video. And then once you have your agent set up these evals and at least have two, three examples, Azure gives you $300 credits to create agents and set evals. So take those agents that you recommended in your case studies and actually build them and show the iterations saying, hey, first iteration was so bad. Then I improved it. And this is how I also improved my evals. I removed these questions because they were always passing. Once I looked at the traces, I found out that I missed these and I have these five iterations of evals. Once you have that, that will be another 15 days to 20 days of work.

**Aakash Gupta** (02:12:15)

Then think about go to market. Think about In a world where tokens are going to be the cost and it's going to be an arbitrary cost. There's no fixed cost in your side also anymore. A user, a heavy user of your agent, like our risk agent is going to consume million tokens or million dollar worth of risks. How should you price your product that your customer get enough value of what they are paying while you can keep your profit margins? For the same case studies that you identified, Build the evals, now build a pricing strategy or GTM strategy. And once you have those five examples and iterations, you can go and be the AI PM, which everybody claims, but nobody is. These are the iterations you will need and these are the four muscles I need. One, you have a deep understanding of what a harness is and you have build your harnesses.

**Aakash Gupta** (02:13:12)

You can build roadmaps of AI. You can evaluate any given agent and tell me how will you do it and how will you scale it. And you can help me with GTM and pricing the agent given all the variable components that comes with evals and continuous development across my user base of heavy users, mid users and low users.

**Mahesh Yadav** (02:13:33)

Guys, Mahesh has been super generous with his time with this podcast. Just think about all the nuggets of value got out of there and let's go storm all of his businesses with a bunch of people from Akash's podcast. This is his startup where he can help. This is his agentic AI product management certificate. This is his Claude Bootcamp. Go use the links that are below so that he knows that they came from the podcast and we can get him back to teach us how to price these AI products soon and have him back next year as well. Mahesh, thank you so much for being here.

**Aakash Gupta** (02:14:11)

Okay, such a pleasure. And thank you for giving me an opportunity again. Always a pleasure. And thank you for your curious questions. It helps me stay aligned.

<!-- sponsor -->
**Mahesh Yadav** (02:14:19)

I hope you learned as much from today's episode as I did. If you can do one thing that's totally free that would help the show, it would be to check that you're following on Apple and Spotify podcasts. Check that you've left ratings and reviews on those platforms. Check that you're subscribed on YouTube. Leave a like and a comment on this video, and then share it with your friends. We're trying to make better and better podcasts. After two years, we think we've gotten something pretty good going. So let us know what we can do to make it even better, who else we should interview, and we We'll put on the best shows we possibly can. Finally, don't forget my offer for the bundle. You get an entire year of my paid newsletter, plus my favorite AI tools, Bolt Up New, Airtable, Speechify, Descript, Magic Patterns, Linear, Dovetail, Arise, and Mobbin.

<!-- sponsor -->
**Mahesh Yadav** (02:15:05)

That's $27,000 worth of value for just $150. So check that out at bundle.akashgu.com if it interests you, and I can't wait to share our next episodes. [music]
