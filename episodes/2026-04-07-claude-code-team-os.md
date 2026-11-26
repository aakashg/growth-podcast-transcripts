---
title: "How to build a Team OS in Claude Code with Hannah Stulberg, PM @ DoorDash"
subtitle: "What it actually looks like when a PM checks in every document, every metric, every customer call into a shared repo - and the whole team queries it themselves."
date: "2026-04-07"
host: "Aakash Gupta"
guests: ["Hannah Stulberg"]
speaker_names: "inferred"
substack_url: "https://www.news.aakashg.com/p/claude-code-team-os"
youtube_url: "https://www.youtube.com/watch?v=0UArKLQ6bXA"
duration: "01:10:32"
word_count: 13873
source: "Substack episode transcript (aired audio)"
sponsors:
  - name: "Bolt"
    url: "https://bolt.new/solutions/product-manager?utm_source=Promoted&utm_medium=email&utm_campaign=aakash-product-growth"
  - name: "Jira Product Discovery"
    url: "https://www.atlassian.com/software/jira/product-discovery"
  - name: "Kameleoon"
    url: "http://www.kameleoon.com/"
  - name: "AI PM Certification"
    url: "https://maven.com/product-faculty/ai-product-management-certification?promoCode=AAKASH550C7"
---

**Sponsors:** This episode is brought to you by [Bolt](https://bolt.new/solutions/product-manager?utm_source=Promoted&utm_medium=email&utm_campaign=aakash-product-growth), [Jira Product Discovery](https://www.atlassian.com/software/jira/product-discovery), [Kameleoon](http://www.kameleoon.com/) and [AI PM Certification](https://maven.com/product-faculty/ai-product-management-certification?promoCode=AAKASH550C7).

# How to build a Team OS in Claude Code with Hannah Stulberg, PM @ DoorDash

*What it actually looks like when a PM checks in every document, every metric, every customer call into a shared repo - and the whole team queries it themselves.*

**Hannah Stulberg** (00:00:00)

I have spent now like 1,500 hours in Claude, and I am still iterating on my setup and improving it literally every single day.

**Aakash Gupta** (00:00:06)

So we've talked about Claude. There's Claude, there's ChatGPT, there's Cursor, there's Cowork. When should PMs be using Winch?

**Hannah Stulberg** (00:00:14)

There's not like a right or a wrong answer, although for most advanced PM work, you should be using some type of a coding agent.

**Aakash Gupta** (00:00:20)

Hannah Stahlberg is a PM at DoorDash and former Google APM. She spent over 1,500 hours in cloud code, wrote the viral cloud code for everything process, and uses cloud code all day at her work. Hannah, what's the biggest mistake PMs make when using cloud code for product work?

**Hannah Stulberg** (00:00:36)

I think the biggest mistake is that people give up too early.

**Aakash Gupta** (00:00:39)

What's underhyped versus overhyped in AI for PM?

**Hannah Stulberg** (00:00:43)

I think that underhyped is following your curiosity.

**Aakash Gupta** (00:00:46)

I, for one, had never heard of this. I think it's a genius idea. Can you just unwrap the covers and show us exactly what this looks like?

**Hannah Stulberg** (00:00:53)

This is what I call Team OS or Team Operating System, which is your team's knowledge base that helps everybody on the team move faster.

**Aakash Gupta** (00:01:02)

You said Claude Code is the most misleading name in AI. Why?

**Hannah Stulberg** (00:01:07)

Because it's not just for...

<!-- sponsor -->
**Aakash Gupta** (00:01:14)

Before we go any further, do me a favor and check that you are subscribed on YouTube and following on Apple and Spotify podcasts. And if you want to get access to amazing AI tools, check out my bundle. where if you become an anal subscriber to my newsletter, you get a full year free of the paid plans of Mobbin, Arise, RelayApp, Dovetail, Linear, MagicPatterns, DeepSky, ReforgeBuild, Descript, and Speechify. So be sure to check that out at bundle.akashi.com. And now into today's episode. Hannah,

**Hannah Stulberg** (00:01:46)

welcome to the podcast. Thank you so much for having me here. I'm super excited.

**Aakash Gupta** (00:01:49)

So I've been thinking a lot about the future of product management. And one thing I'm noticing across companies in every geography is that PMs are supporting more and more people. 1PM might have supported three or four engineers in the past. Now they're often being asked to support 10 engineers. And on top of that, where they might have just mainly concerned themselves with design and engineering in the past, now they have to interface with everybody. Sales, marketing, support, the list goes on and on. How are you dealing with this and what does the future look like for PMs in this world?

**Hannah Stulberg** (00:02:19)

Yeah, so I think the future looks like exactly what you're saying, which is that a singular PM is going to be supporting a broader set of functional roles and at a much higher number than in like the previous team sizes. At the same time, I think we're seeing in the industry that roles are starting to merge together. So it used to be that generally all product decisions were made by the PM and then engineers were just writing code and design was just doing design. But now what we're seeing is engineers are building products and maybe even like deploying them Without a PM, designers are prototyping and building product. And everyone on the team is starting to make product decisions. Similarly, as PMs, we're starting to do a lot more data analysis, also prototyping, making designs. And so we're starting to see a lot more blended functions where everyone needs to have the best context that used to be isolated within different roles on the

**Aakash Gupta** (00:03:12)

So your answer to this is to create a well-organized high context repo. I for one had never heard of this until I saw you writing about it and talking about it. I think it's a genius idea. Can you just unwrap the covers and show us exactly what this looks like?

**Hannah Stulberg** (00:03:27)

I can. Okay, cool. So this is what I call like team OS or team operating system, which is your team's knowledge base and storing all of your team's shared context in one place that helps everybody on the team move faster and do their job to the best of their abilities, especially being able to get context across many different types of functional goals. So what we see here is there's three main parts of the team OS. You have the .cloud folder. This is the folder where you might put shared agents, commands, and skills that are shared by everyone on your team, which we're going to talk about a little bit more. Then I have the product development folder. And here you're going to see a lot of different subfolders across different functions. And then we have a team folder. where you might have like team level documents, like onboarding guides or retros.

**Hannah Stulberg** (00:04:15)

And at the top, we have the ClaudeMD at the root level. This is the guiding route for Claude throughout your repository. And this has a few different key components. So the first is it has what's called a doc index. And this tells Claude how to navigate the repository. So Claude needs to know where to go to look up different types of information so that you can do natural language queries in the repo and get the answers that you need. The other two things that I like to have at the root level are who is on my team along with their handles in key products and then like key Slack channels or DM groups. And the reason for this is you really, when you're kind of doing all of your work in this repository, you want And also to be clear, this works with any type of coding agent.

**Hannah Stulberg** (00:05:02)

It doesn't have to be Claude. You could do this with Codex. You can do this in Cursor. You want Claude to know who's on your team so that you can just write queries like Slack, Alex about the bug that came up on the customer call today. And because the Claude MD file is loaded every single time, it's going to load Alex's Slack ID and it's going to be able to use the Slack MCP to send Alex a Slack. It's also really nice if you're talking about feedback or like meeting notes, because then when you're like, oh, I got feedback from Taylor, Claude knows that Taylor is your design partner and is going to be able to better contextualize that feedback without every single time you're writing, yes, like Taylor, the designer on my team gave me this feedback. And similarly for the Slack channels, by knowing all the channels and what the purposes are, you can write natural language queries like, hey, send this in the product channel, send this in the eng channel, and Cloud will know exactly what to do.

**Aakash Gupta** (00:05:50)

So how has your CloudMD file changed over time? What have you learned in the 1500 hours you've put in through trial and error and making mistakes?

**Hannah Stulberg** (00:05:58)

So I think this is actually what a lot of people get wrong about CloudMD, which is you don't want very much in your CloudMD file. So CloudMDs should be very, very, very lean, especially in a team repository like this. And generally, if we start looking through the repository, what we see is that there's actually multiple levels of CloudMD files. And so we'll see here, here's the root level. This one loads every session. The remaining files are going to start to load progressively as you type natural language queries, which is something that we're going to walk through. And this is really important because the way that this repo is structured is around the theory of context management. So I like to call this like context 101, but there's four like key concepts that you need to know about context. One is what is context? Context is the amount, is the information that is in a given session with an LLS.

**Hannah Stulberg** (00:06:50)

Like what is the information that the LLM can access at a given point in time? The next is the context window, which is how much information can the LLM hold? And there's all the frontier labs recently upped this to a million tokens, which sounds a little bit jargony, but basically means that it can hold seven to eight novels worth of text, which if you start thinking about it is a lot, but the amount of docs that are produced by a given team and company is a lot more than that. The next part is compaction. So when your context window gets full, So all that information needs to get compressed down so that the LLM can keep going either in the conversation or in the work that it's going to do. But when that happens, you lose a lot of fidelity. And so you have kind of a like compressed summary of the information, which is much less useful.

**Hannah Stulberg** (00:07:34)

And then the fourth concept is thinking room. And this is really important because thinking room is basically the difference between how much information you have in the conversation and how big the context window is. That is where the model can think and reason. And if you have a lot of information, the more and more information you have, just like a person, the less and less room there is to think and reason. And so the whole repository is structured around helping Claude read and use the right information at the right time in order to effectively work on the task at hand. And a lot of people don't know this, but I have this little bar in my status line, and it's actually going to monitor how much context I'm using as we write queries throughout the repo. And this is going to help us kind of see how much context is being consumed by the conversation.

**Aakash Gupta** (00:08:27)

Awesome. I hadn't actually seen the nested CloudMD files before. So what do those look like inside there?

**Hannah Stulberg** (00:08:33)

Yeah. So what we're going to see in the repo is that the CloudMDs are generally just doc indexes. So this is just telling Cloud, like, what in this folder and what is the purpose of it. And the reason for that is if you didn't have these doc indexes, clog would actually need to be running explore agents, like search the repository for any queries that you write. So I actually want to do like a couple examples to kind of show how this works. So in the product folder, you know, one of the things we might have is who our customers are. And what's really cool about how you structured this repo is I'm going to say like, who are my top customers? And what we're going to see here is we're actually going to be able to see how Claude navigates it. So it's loading these Claude MD files and using the doc inside.

**Hannah Stulberg** (00:09:19)

indexes to navigate throughout the repository and find the exact information needed to answer my query. And now it's starting to read, okay, in the customers folder, who are my customers? What is the account context that I've stored on them? And what you can see here is that we've only used 3% of the context window and Claude's not looking in the wrong places. Claude didn't go into the analytics folder. It didn't go into the data engineering folder. It didn't read a single unnecessary piece of information to answer my query, which means we still have a ton of room to think.

**Aakash Gupta** (00:09:50)

So the art of having good Cloud MD files is actually minimizing the amount of context that Cloud needs in order to answer a given question.

**Hannah Stulberg** (00:09:58)

It's minimizing the amount of context that's consumed and making sure that you're only consuming context that's relevant to what you are actually trying to do. If I'm asking about my customers, I don't need to go read a bunch of SQL queries.

**Aakash Gupta** (00:10:12)

Very cool.

**Hannah Stulberg** (00:10:13)

And we can also start to do more interesting things here. So I can say, who did I meet with over the last two weeks? And what did I learn? Because I store all my customer information inside the repository in a really structured manner. So if we go under my customers folder, I have a file for each of my customers. And in here, I actually have a Cloud MD on the customer.

**Aakash Gupta** (00:10:38)

And

**Hannah Stulberg** (00:10:38)

in here, this is where I'm saying, okay, what's the key con, like what you want in a Claude MD is things that you need on 80% of sessions. And so generally for like a customer, you might want to know, okay, who are the key context of that customer and what do they do? What's their segment? And then again, I have a doc index here. This is how to find key resources on this customer account. Now, Claude is like primed to know where to go for everything about this customer. And so now Claude's doing an analysis and saying, okay, today's March 25th. What was the last two weeks? There's a lot of calls. It's going to read them, but actually look here at what it's reading. It's only reading the summary files. It's not going into like every single transcript, which I don't know about you, but like my customer calls can be like more than an hour, right?

**Hannah Stulberg** (00:11:21)

Claude would not be able to go and quickly and easily synthesize, you know, 50 transcripts really quickly at high fidelity, which is why the repo set up that it only needs to go into the transcripts if the summary doesn't have what it needs to like answer my question.

<!-- sponsor -->
**Aakash Gupta** (00:11:36)

Here's the dirty secret about prototyping. You spend two weeks building a prototype. You validate your assumptions. Engineering loves the direction. Then what happens? You throw the whole thing away. Bolt changes this completely. When you prototype in Bolt, you're not building throwaway mockup. You're building real front-end code that integrates with your existing design system. So when you hand it to engineering, they don't throw it away. They ship on top of what you've built. I use Bolt every single day. I host my land PM job cohort on it. And honestly, I'm up till 2am some days just vibing in the tool, having fun, and building. That's when you know a product is good. When you're using it past midnight, not because you need to, but because you want to. Check out Bold at bold.new slash akash. That's b-o-l-t dot n-e-w slash a-a-k-a-s-h. Link in the show notes. Today's episode is brought to you by Jira Product Discovery.

<!-- sponsor -->
**Aakash Gupta** (00:12:24)

If you're like most product managers, you're probably in Jira, tracking tickets and managing the backlog. But what about everything that happens before delivery? Jira product discovery helps you move your discovery, prioritization, and even road mapping work out of spreadsheets and into a purpose-built tool designed for product teams. Capture insights, prioritize what matters, and create roadmaps you can easily tailor for any audience. And because it's built to work with Jira, everything stays connected from idea to delivery. Used by product teams at Canva, Deliveroo, and even The Economist. Check out why and try it for free today at Atlassian.com slash product dash discovery. That's A-T-L-A-S-S-I-A-N dot com slash product dash discovery. Jira Product Discovery. Build the right thing. So adding some more files in the form of summaries is actually going to help it collect the relevant information faster.

**Hannah Stulberg** (00:13:23)

Correct. So you basically are always wanting to think about how to structure information so that Claude can quickly and easily find what it needs to know in a format that's really easy to use, which kind of goes to another topic within the report. repository, which is your shared agents, commands, and skills. So when, if you want struck while LLMs like can work really well with unstructured information, it is obviously easier if information like shares a common structure. And so teams that are using this system. We ideally should try to organize information in a structured way for Claude so that, for example, all customer call summaries follow the same format. That means that when Claude needs to do a synthesis on like hundreds of different customer calls, following the same format, which makes it much easier for Claude to work with. And so that's why, for example, you might have a customer call skill and this, and then you would have everyone on your team who's summarizing a customer call, summarize it in exactly the same way, put it in exactly the same place.

**Hannah Stulberg** (00:14:25)

Then when you need to do cross customer analysis, even though maybe you had 10, 15, 20 different people taking those different calls with different customers, everything is organized in a very consistent fashion that Claude can work with super easily and super quickly.

**Aakash Gupta** (00:14:38)

So you're multiplying leverage by creating these skill files to take unstructured inputs. Maybe people have different ways of interviewing, but then structure the summaries in a similar way.

**Hannah Stulberg** (00:14:48)

Exactly. So then all of your summaries come out with the exact same format, even if maybe, you know, your company has a ton of different account managers who would all synthesize things differently.

**Aakash Gupta** (00:14:58)

Very cool.

**Hannah Stulberg** (00:14:59)

And so now we see, okay, we got like a pretty detailed analysis of the last few weeks. So it's going to tell me, okay, who I met with, who did, what was the customer? When did I meet with them? Who was in the meeting? What happened on each of them? Super fast. And then it also gave me like a quick cross-cutting theme analysis. And all of that was just off of a natural language query. I just said, you know, what happened in the last two weeks? What did I learn?

**Aakash Gupta** (00:15:22)

Super powerful.

**Hannah Stulberg** (00:15:23)

So kind of continuing to walk through the repository. So as you can see, there's a lot of different parts that you might have in a product folder. You might have some competitive research. Maybe you have your launch emails, meeting summaries, your PRDs, products. processes that you need to run, context about how your product works, things for sales enablement, strategy docs. Here you might keep like business context about the company or the landscape that you're operating in, who your users are and what they need to be doing. Your roadmaps, vision docs. And then workflows is actually a concept from Carl, who has also been on your podcast. These are like multi-step processes, like preparing for a biweekly update that you might want to run on, like that you might need to run. Let me try that again. A workflow is like a multi-step repeatable process that you need to do often on some cadence.

**Hannah Stulberg** (00:16:13)

And Carl has like a great system for getting this done that I've actually applied in a lot of my own workflows as well.

**Aakash Gupta** (00:16:18)

Got it. And what is that system briefly?

**Hannah Stulberg** (00:16:20)

Yeah. So basically, when you need to do a complex multi-step operation, the way to do the operation is stored in the Claude MD of the folder. And it's kind of similar. to having a command. And then there's different files that says how to execute each part of the process to then synthesize something into a final document. And so I find this to work really well for meetings where you might need to pull a bunch of different information together and then put it in a document in a repeatable workflow that you want to run on some cadence.

**Aakash Gupta** (00:16:54)

Got it. What else do we need to know about this repo if we were trying to create our own?

**Hannah Stulberg** (00:16:57)

Yeah, so we talked about the product portion, and we can go deeper into what each of the different folders are and what you might use in them. But I think it's actually also really important to talk about the other functions as well, because this is how everyone scales themselves and the most out of the repository. I don't view the team OS as like something to help everyone become a better PM or to be better at doing product. I really view it as a way for everyone on the team to scale themselves and help everyone to leverage what's best about all of their teammates. So for example, in your analytics folder, you might have like links to all your dashboards, all of your experiment analyses and the results of them, investigations that were done, and then I think the most important part is metrics, playbooks, queries, and schemas.

**Hannah Stulberg** (00:17:43)

So this is how you scale data analysis across the team. So I like to generally organize by topic area and then product area. So in this dummy repo, I made up a company called Forge Labs. They're bringing another AI prototyping product to market. And so these are different parts of the Forge Labs product. And here we start to see, OK, so here we've outlined all of the metrics for the billing part of the Forge Labs product. And then here, and what you'll see here is that here we've linked all of the dashboards that are relevant to this. And then we also have a link into where the queries are for these metrics. And then if you go under queries, under billing, then you would have all of the SQL queries for how to query the metrics related to billing. And then here in the schemas, we would have all of the table schemas that actually back these metrics.

**Hannah Stulberg** (00:18:40)

And so if I wanted to do data analysis, I would have all the references that I need as a PM to do correct analysis and have all of like, I basically get to have access to like the analyst on my team's brain and everything. everything that she's so amazing at and set me up for success in doing analysis correctly. And so we can do some pretty cool stuff here as well. So, for example, I might say I'm just going to use whisper flow. do we calculate generation success rate? Show me the metric definition, the SQL query and the table schema. And so now I get to know everything about how to calculate this metric, what data tables to use, how it's defined, what tables it comes from, and it's going to be able to give me all of this. And I think this is really important because especially if you're, once you have anything that's more than like a very, very early stage product, your data tables can get really complex, the right way to query different metrics.

**Hannah Stulberg** (00:19:40)

is not always obvious. And if you don't have the right guidance for Claude and you just point it at a database and say, hey, pull this stuff, it might not do it correctly. And so now here we see, okay, let's see if we can expand this. Yeah, so here, and this kind of goes to how the repository is structured. When I put that query in, it knew exactly what files to reference. So it went in the SQL, it went in the table schemas, it went in the metrics, and then it started reading everything about this part of the product. And then it actually was able to tell me, okay, how is this metric defined? And then what is the way to query for this? And then what is the schema that backs all of this? And if this was not like a dummy repo and like a demo instance, like you can actually have this hooked up to like Snowflake MCP or another analytics MCP, and you could actually start having Claude do the analysis for you.

**Hannah Stulberg** (00:20:31)

Similarly, we could say, okay, you know, what do we know about why users drop off during custom domain setup? And because in the repo, I have a playbook that would be an example of what an analyst might add into the repo for how to do the funnel analysis. And so, Claude is going to be able to know, okay, like how do we do this funnel analysis? Maybe this has already been investigated. It's going to find all the information in the repository and then use that to answer my question and answer it correctly. And so we become a lot less concerned with like hallucinations, inaccurate data, inaccurate analysis, because everything that you're using as a PM to do the analysis is something that's actually been checked into the repository by an analyst or a data scientist on your team. And you know that you're using like verified approaches to get the metrics.

**Aakash Gupta** (00:21:19)

Very cool. So you'd have like an analyst or data scientist really audit some of these playbooks and some of the table descriptions and join keys that we saw earlier.

**Hannah Stulberg** (00:21:28)

Exactly. So the repo is something that like the whole team should be building together. So on my team at work, the data scientist that I work with owns our analytics folder. And every time that we're building a new feature, her and I are aligning on, okay, what are the metrics for this feature? What are the backing queries for the metrics? What are the tables? And then we're making sure that all of it's documented. in the repository so that when we roll out a feature, I can actually check how it's doing without being reliant on a data scientist. Or our engineers can also check on how it's doing because they're empowered with all of the queries that they need to also do validation of the feature. in production. And the organization here is really important. And there's a reason to split out the metrics, queries, and schemas.

**Hannah Stulberg** (00:22:11)

And again, it goes to this theory of context management. So you might just have a question about metrics. You might just want to say, what are the metrics for the billing feature? And you don't want Claude to then go pull all the queries and all the schemas to answer that question for you. You just want it to know what the metrics are. And I find this really helpful for when I'm writing a PRD, for example, I can have Claude easily look up every metric I've ever defined for my product, figure out, okay, which metrics might we want to update? Which ones do we need to add in? Because I have all that context really well-structured by feature in the repository.

**Aakash Gupta** (00:22:45)

Love it. This is really speaking to kind of the future of how engineers don't want to have to be reliant on a PM to get a data report here. You're the PM is actually becoming the glue, making sure that analytics has agreed on these are the right things, put the right things into the repository before a feature starts. But then once a feature is launched, if an engineer is on call and the whole team is asleep, they can just clear it all by themselves.

**Hannah Stulberg** (00:23:11)

Exactly. And I think, and we actually make this part of our feature launch process. So when we're rolling out a new feature, the feature is not rolled out until the repository is updated because that's how we know that we're continuing to create that shared context so that everyone has what they need to like do their job effectively as our product, as our product grows more and more complex.

**Aakash Gupta** (00:23:33)

Awesome. Are there any other nooks and crannies people should know about of this repo?

**Hannah Stulberg** (00:23:37)

So I think the repo really benefits every function. So I just put an example of like what you might have in an engineering folder here. So I put some bug investigations and then we use the term RFCs for like technical design documents. And again, this goes to helping everyone to do their best work, helping everyone to have shared context and historical context. So you might store all the bug investigations across your product in the repository, because unfortunately, we usually have more than once, oftentimes in like the same part of the product. And so it's really helpful for the person investigating that bug to be able to see, okay, what are all the bugs that have happened here? What was the approach for, so here, like I saved, a bug investigation plan. And we can see, okay, like when did this happen? What were we investigating? What was the scope?

**Hannah Stulberg** (00:24:24)

What parts of the infrastructure did it touch? How was this analyzed? What was the root cause? How was it fixed? All the data examples and all of the queries. And so then if someone has to go investigate another bug here, they have all the context of how every bug was ever investigated. And this helps them and helps them to like work with a clod or another type of coding agent to really effectively investigate another bug.

**Aakash Gupta** (00:24:46)

Very powerful. And who owns basically the engineering folder, like your tech

**Hannah Stulberg** (00:24:50)

lead? So on my team, like everyone is an owner of our knowledge repository. So each of like the functional leads kind of takes ownership of like, okay, how, you know, how do we want certain things done within this area? But the team as a whole, needs to agree on the way to structure the information because LLMs don't work as well with unstructured information. And then it becomes the onus on everyone to be updating the repository and making the team's shared context even better. And I think that this is how teams become really high performing in an AI native era is everyone is working to improve the repository to make the team faster, right? Everyone should be writing shared skills that benefit the team, shared commands that benefit the team, agents that help the team. We as PMs, but also everyone on the team can also set up shared automations, which I kind of think of as the third pillar of this.

**Hannah Stulberg** (00:25:45)

This could be, for example, using the information in the repository to run a weekly report that synthesizes all the customer research and what you learned. And with the way that this repo is structured, you can actually have that just be an automation that runs every week, synthesize all the research, post a message in your Slack channel so that everyone stays up to date on customer learnings.

**Aakash Gupta** (00:26:06)

So I think we got the high level, the 80, 20 of the setup of the repo. You check in all your day-to-day product work into the repo. What does that look like tactically?

**Hannah Stulberg** (00:26:16)

So tactically, I only work in Cloud code these days. So I write every single doc first in Cloud. And then I check it into the repo and my team to review. And that's how everyone on my team works as well. So my whole design team works in Cloud. The engineers work in Cloud. We're all working in the shared repository. My data scientist is also working this way. And I think, sorry. People think that this is only for technical roles, and I think that that is a very, very wrong assumption. So actually all of my business operations, product operations, strategy and operations partners are also participating and sharing in this shared context repository, putting up PRs, adding their context into the repo. We're all collaborating together in this space every day.

**Aakash Gupta** (00:27:07)

What would that look like? So where would I, let's say I just completed the first draft of my strategy document for next quarter. What, where would I put that and how would I check that in?

**Hannah Stulberg** (00:27:17)

Yeah, so you would likely, if you were me, have actually written that whole doc in Claude. And if not, you could pull it in from a Google Doc using the MCP. And then under, you'd probably have a strategy docs folder here, or I might call it like vision, and you can start organizing it by quarter. So I would have different folders under here, and I would say, okay, you know, Q2, 2026, vision, and I would like have all the docs for that under there.

**Aakash Gupta** (00:27:41)

And then when you check it in or something like that, how do I put this up into GitHub so that other people can see it?

**Hannah Stulberg** (00:27:47)

Yeah, so you would just put up what's called a pull request or a PR. And that is how you, so first you would commit your work. When you're ready, when all the work is ready to review, you would put up a pull request and then you would put that up for your team to review. Generally, you'll have certain people that you would want to review certain types of work. So for example, if I'm writing a PRD that I know a certain engineer on my team is going to implement, I would put up the PRD within a pull request, and I would put them as the reviewer on the PR. that's really nice about doing all this in Claude is that you can have the GitHub command line interface or MCP hooked up. And because Claude knows who everyone on my team is, I would literally write a query that's like, put up a PR for Morgan to review this PRD with the name of the PRD and everything would just work.

**Hannah Stulberg** (00:28:33)

Never leaving Claude at all.

**Aakash Gupta** (00:28:35)

Wow. Actually awesome.

**Hannah Stulberg** (00:28:38)

And then because I also have like for my team configured that we have shared commands for creating PRs and our shared commands actually auto post a Slack message to our team's channel with like certain structures depending on who put up the PR, what is the contents of the PR, who should review it. So we actually like automated a lot of this.

**Aakash Gupta** (00:28:59)

This is pretty mind blowing. So you're basically saying that you don't just have a code base. You essentially have a code base of your team's context for clock. And you are like pushing, pulling and sending PRs for that context. And it's not just PMs doing it. It's analysts doing it. Designers, engineers, go to market partners. Everybody is participating in that overall product team's OS.

**Hannah Stulberg** (00:29:24)

Exactly. So like, for example, my strategy partner takes even more customer calls than I do. And she checks every customer call that she takes into the repository so that I can review what we learned. And that helps us to work super, super well together. And she's completely like, non-technical. Like she had never opened GitHub in her life two months ago, and now she is putting out PRs every single day. I think that's something that I feel like very passionately about. I feel like I see a lot of chatter online like, oh, this way of working is only for PMs or it's only for engineers or it's only for technical people. And I think that's very incorrect. I think this is something that anyone can learn how to do. And that when everyone does learn how to do this, we can all work so much better together.

**Aakash Gupta** (00:30:07)

And just so people who are scared of GitHub, like the command, at least how I do it, I'm not sure how you do it, is I would literally just tell it like, am I logged into GitHub? Do you have access under my name? It'll say yes. And then I'll say, commit this pull request for this issue and tag this reviewer, all in natural language. That's all you basically have to do, right?

**Hannah Stulberg** (00:30:26)

Yeah, basically. I would also say I have an amazing GitHub 101 guide on my Substack that has helped thousands of people learn how to use GitHub confidently. So I would also probably route you to that.

**Aakash Gupta** (00:30:37)

Cool. What's the 60-second summary of that that I didn't cover?

**Hannah Stulberg** (00:30:40)

Of how to use GitHub?

**Aakash Gupta** (00:30:41)

Yep.

**Hannah Stulberg** (00:30:42)

So the 60-second summary is all of your work should be on a branch. And the process is basically you put all of your work onto a branch. As you're working, every time you finish a certain milestone, you're going to commit it. And this means you're saying, I reached a stop. And I want to save all my work. When a given item is done, let's say, you know, you might write your PRD in chunks. And when the whole PRD is done, you're going to open a pull request and you are going to then open a pull request and ask for review. This is where you would tag a reviewer. They might give you some feedback that you might address. And then when everything is good, said and done, you will merge it into the main branch, which means that now everyone in all of their local repositories has access to your work.

<!-- sponsor -->
**Aakash Gupta** (00:31:27)

Today's episode is brought to you by the experimentation platform Chameleon. Nine out of 10 companies that see themselves as industry leaders and expect to grow this year say experimentation is critical to their business, but most companies still fail at it. Why? requirements require too much developer involvement. Chameleon handles experimentation differently. It enables product and growth teams to create and test prototypes in minutes with prompt based experimentation. You describe what you want. Chameleon builds a variation lets you target a cohort of users, choose KPIs, and runs the experiment for you. Prompt-based experimentation makes what used to take days of developer time turn into minutes. Try prompt-based experimentation on your own web apps. Visit chameleon.com slash prompt Today's episode is brought to you by Amplitude. Replays of mobile user engagement are critical to building better products and experiences, but Many session replay tools don't capture the full picture.

<!-- sponsor -->
**Aakash Gupta** (00:32:30)

Some tools take screenshots every second, leading to choppy replays and high storage costs from enormous capture sizes. Others use wireframes, but key moments go missing, creating gaps in your understanding. Amplitude does things differently. Their mobile replays capture the full experience, every tap, every scroll, and every gesture, with no lag and no performance hit. It's the most accurate way to understand mobile behavior. See the full screen. I hope you're enjoying today's episode. by OpenAI product leader, McDad Jaffer. If you use my code and my link, you get a special discount on this course. It is a course that I highly recommend. We have done a lot of collaborations together on things like AI product strategy. So check out our newsletter articles if you want to see the quality of the type of thinking you'll get. One of my frequent collaborators, Pavel Hearn, is the Build Labs leader.

<!-- sponsor -->
**Aakash Gupta** (00:33:35)

So you're going to live build an AI product with Pavel's feedback if you take this AIPM certificate. So be sure to check that out. Be sure to use my code and my link in order to get a special discount. And now back into today's episode. Awesome. That covers the main elements of the repo. I want to talk a little bit about creating high quality documents. How does someone use this repo to create a 10X PRD or product strategy document?

**Hannah Stulberg** (00:34:00)

Yes, so I think having a shared context repository helps with writing really high quality docs, but that's not the only piece of the puzzle. The other piece of the puzzle is knowing how to plan effectively with quad. Okay, cool. So let's talk about plan mode. I'm just going to clear this. For those who don't know, clear is a way to wipe the context of your current session. And it's really important to do this when you're switching tasks, because again, Claude is going to use the information in that conversation to guide its work. And so if you're starting a completely fresh task, you either want to open a different terminal window or you want to clear and wipe the context so that you're really focused only on the task at hand.

**Aakash Gupta** (00:34:43)

Got it.

**Hannah Stulberg** (00:34:44)

I wanna show kind of the difference between not using plan mode and using plan mode. So I'm gonna split my terminals here and because we're kind of doing this, like we have this imaginary AI prototyping company, I'm gonna use like Google stitch as an example, since they just had like a major release this month. So what I'm gonna put in here is I'm gonna put a basic prompt. I'm gonna say, you know, research the most recent Google Stitch release and tell me about what happened. And then in here, I'm going to say the same thing. Research the most recent Google Stitch release, tell me about what happened, and give me a proposal for what you're going to do. And now we're going to kick both of these off at the same time. And so here, this is just a basic prompt. And when you're doing this, you don't really know what Claude is going to do, right?

**Hannah Stulberg** (00:35:30)

Claude is making all the decisions here. And you're going to get back something. And I really like the junior employee metaphor for Claude. I think of working with Claude, like working with like a really, really eager and highly talented junior employee. And if you don't give that, when you have like a junior employee and they're not trained and they don't know what you like and how you like to work, then you don't totally know like what you're gonna get back from that employee. when you don't give them any guidance. And that's what basic prompting happens. So you're gonna get back something, but you don't know if that something is gonna be useful for you, if it's gonna be in the format that you want. And so that's why I don't generally recommend this approach. So here, so there's a more lightweight version of prompting where before Claude does anything, you just say like, what is your plan, right?

**Hannah Stulberg** (00:36:15)

You're kind of asking your employee, okay, like, what are you planning to do? And you're going to assess, are you like generally aligned on the direction? So here Claude did a little bit of research. told me what happened and it's giving me a proposal right and it's actually using the context from the repo to generate the proposal remember this was a completely fresh session i didn't load in any context but here it's saying this is a significant shift in the design to code tooling landscape here's what i'd suggest for the forge team right we should evaluate stitch for rapid prototyping we should see how it hooks up with our workflow we should see um if this is like competitive to what we're doing and we should share the findings in these two Slack channels, right? And it did this, it came to all these conclusions itself using the context from the repository against this natural language query that I had asked.

**Hannah Stulberg** (00:37:02)

Now, if I was writing a doc, this is still probably not what I would have wanted. And so that's where we go into plan mode. So to get into plan mode, you press shift tab twice, and then you're gonna see that plan mode is on. And so now I would say, okay, so now let's pretend that I need to write some, maybe like a strategy doc around this most recent Google Stitch release. So again, I'm going to start and I'm going to say, okay, research the most recent Google Stitch release. And what I'm going to want to do is write a strategy doc about how this impacts us as a company and what we should do. Now, the difference between, you might be wondering, well, you know, in that other terminal, Claude gave me a proposal of what it was going to do. We could go back and forth and keep chatting in the terminal.

**Hannah Stulberg** (00:37:50)

And that is a totally valid thing to think. The difference is that when you're using, think of LLMs are trained to have a bias for action in order to be helpful. And so the goal of the LLM is to get into action to help you as the user. But it's kind of like a horse that's chomping at the bit and it's like, please, let me just go run and help you. And that's not very good when And so what plan mode does is it takes away that bias for action. It's kind of like taking away the keys and saying, Hey, we're not going into action right now. We are going to only plan and you're going to get a lot better results. but people still don't like totally use plan mode effectively, which is what we're going to talk about. So now what it's saying, it's going to research Google stitch and my product context in parallel so that it can plan the strategy doc effectively.

**Hannah Stulberg** (00:38:41)

And so here it's actually researching the release and it's researching my code base at the same time. And this is how you can start to see that, okay, when you have all this context in your repository, then, um, you're already set up to load a lot of that context into your documents. Now we're going to like, wait for this to run.

**Aakash Gupta** (00:39:01)

It's interesting. It also shows like how much potential tokens are there, like 25K and 98K, but it's not like burning through 130K tokens. It knows where to look within those.

**Hannah Stulberg** (00:39:12)

Yes. And I think that's something that's really important because I talk to people. a lot who were like, you know, I put some queries into Claude and I burned like hundreds of thousands of tokens and I hit my usage limit within 30. And that's generally because people's work is not organized and optimized for Claude to easily traverse. So you're very, very inefficient in your conversations. And look, again, Claude is only loading the stuff that's relevant to my query. It didn't go into the analytics folder. It didn't go into the engineering folder. It went into my competitive research folder where it has access to my competitors. It looks like I have some information on Google stitch. Now it's checking my writing guide and my existing vision docs to understand like the expected tone and format. And so we're going, you can see that Claude is already having a big headstart in probably getting to what I would want.

**Hannah Stulberg** (00:40:03)

And it's also identified that my knowledge, like what I have in the repository is outdated because of this release. It's probably going to suggest that I make some updates. Cool. So now Claude is actually using something called Ask User Question Tool, where it's asking me some questions about what I want to do here. So who is the primary audience for this doc? Let's just say it's for leadership. And what's the focus of the doc? I think that we should maybe do a competitive analysis. I think that would be pretty interesting. Or maybe we should do both. So let's just do a full doc. And then yes, we also want to update our existing files. So this is a very important practice, which is you need to keep the context repository updated. Otherwise you have what's called context rock, which means plot is going to use context that's outdated.

**Hannah Stulberg** (00:40:47)

So we're going to update those. And now it's starting to form the plan.

**Aakash Gupta** (00:40:51)

And so when you probably up checking in this PR, it'll have two components, the strategy doc and the update to the competitive Intel.

**Hannah Stulberg** (00:40:58)

Exactly. The PR is going to contain every single thing that I've changed in the repo as it relates to this task. So now it's going to read these and then we're going to kind of go into the next part of planning. And I also think you actually raised a good point there, which is it in order for your work to be reviewable, you want to generally put like chunks of work together. So, you know, something that contains 85 file changes is going to be really hard for anyone to review. And so generally I like to segment my work for the person who's reviewing it. So let's say, at the same time, I might be working on a design brief for my designer, I might be working on a PRD for an engineer, and I might be updating a metrics file for the analyst on my team.

**Hannah Stulberg** (00:41:39)

I would actually open three separate PRs for those, and I would tag each different person as the reviewer on that work. That makes it much easier for the person to review and approve, and then me to merge all that information back into our central repository.

**Aakash Gupta** (00:41:52)

Fascinating.

**Hannah Stulberg** (00:41:54)

Cool. It's almost done. Now it's writing the plan.

**Aakash Gupta** (00:41:57)

And we're thinking with high effort here, you can change that, but I generally try to keep it at like the max settings. It looks like you do too.

**Hannah Stulberg** (00:42:03)

Yeah, I pretty much am always thinking with high effort, especially, I mean, you can use medium for some stuff, but generally if I found for anything that involves like writing or reasoning, you're going to get the best results with high effort. And so it's worth waiting. For the purposes of this demo, I might put us down to a lower effort, depending on how long some things take. But I also know we can cut this down.

**Aakash Gupta** (00:42:23)

And then I think if you're feeling frustrated about that, what I usually do in this downtime is I spin up my second agent. Yes. So usually I wouldn't have this downtime because I

**Hannah Stulberg** (00:42:32)

would go start working on something else. Oh, the other thing, I'll cover this afterwards, actually. Okay. So here again is where I see people. people not go right with plan mode. So these files can be pretty long. It's pretty hard to read them in the terminal. But what you can actually do is open it up and read it. And the most important part of having a good plan for Claude to execute is actually reading the plan, right? If you're going to send Which I have found that not a lot of people actually do. And if you're going to send someone off to burn a bunch of your tokens and have really high usage, you, again, probably want to know what your employee is going to do. And so I will always actually read through the plan. and make sure that I am aligned on it. And now we're going to talk about how we get into some more advanced planning techniques.

**Hannah Stulberg** (00:43:18)

So here it's having a structure for my strategy doc, and then it's going to update some competitive Well, you know, if I'm writing a strategy doc, I might not just want to research this most recent release. And so what I might do is I might want to say, okay, actually, what I want to do is I want to research anything that any any of my competitors have shipped in the last three months. And I want you to do a sentiment analysis on the news coverage that these launches received and help me understand which publications cover these releases. I then want to get a deeper comparison of basically how the landscape has changed in order to inform the strategy doc. And I want this research to be parallelized. Once the research is done, let's have a check-in to review it and then we'll write the doc afterwards.

**Hannah Stulberg** (00:44:10)

So what I'm doing there is like a couple of different things. So one, Claude does not naturally parallelize plans and I'm creating phases of work that I'm gonna have Claude start to work through. And I'm kind of broadening the scope of what I'm gonna do here so that I can get more work done at once. The other thing is like for this plan, after the research comes through, I might want to like actually review that research to sort of shape what goes into the strategy doc. So sometimes I'll create a checkpoint in the plan where I like to check in with Claude before we continue to the next phase. While we're talking through this, there's some other parts in the plan that I think are very important. So another part is verification. So verification is how Claude knows that the work was done and done well.

**Hannah Stulberg** (00:44:59)

I wish that it was not doing the search now. I should have prompted that differently. verification is how Claude knows that the work is done and done well. So here, what we can see here is there's actually like no verification on how the research is being performed. So if I was like doing this in real life, I might actually talk to Claude about how I want that research If it's making claims, I might ask for the sources to be cited. I might ask for URLs to like the news releases or something like that. It's important that I know how to check Claude's work and that Claude knows how to self-verify its own work before giving it back to me. Another example of like self verification is if you are building a front end feature, for example, you can have Claude use something like Playwright MCP to go in a loop and actually check the front end and validate its own work before it's telling you that the work is done.

**Hannah Stulberg** (00:45:50)

So the ability to tell Claude like what good work looks like and how to know that the work is done is a very key part of planning. I want to cancel this and it's not gonna let me do that. So we can see here that Claude is actually using six agents at once to do this research.

**Aakash Gupta** (00:46:07)

I'm so happy they created like the automatic parallel sub agents. It's so useful.

**Hannah Stulberg** (00:46:12)

It is useful when this didn't happen every time I practice this. But we will get there. So other things that I would do if this was a real plan that I was executing is I would actually go through the strategy doc structure. So Claude is proposing a structure for this doc, might not actually be the way that I want the doc structured. And so I would continue to give feedback to Claude about, okay, what are the sections that I want in the doc? What is the narrative of those sections in order to make sure that what I ultimately get back is what I actually desire. The other thing, while we are waiting for this to run, the other concept that I'm going to talk about is actually storing plan files within the repository. So what we're going to kind of see is like when you're doing like a longer and more complex plan, you're going to be putting time and effort into writing that plan.

**Hannah Stulberg** (00:47:10)

And what teams are starting to do is actually store the plan file itself in the repository. So what you'll see in the repository is I actually have folders for plans. And I have these in like most of the core folders, like in... simple like in my strategy folder i also have a file for plans for other strategy docs that i've written um and the reason to store these in the repository is again to help speed up everyone's work and have that historical context if you're going to spend a couple hours with quad figuring out how to do something, you might want, you might need to do something similar again in like a month or in two months. And you don't want to start from zero again. You would like to have a previous plan to reference for how you did that to save yourself time in the future.

**Hannah Stulberg** (00:47:57)

Or maybe somebody on your team needs to do something similar. and then they can go off of your plan. When you're doing agentic coding, this is also a way to track the work that's in progress as coding agents are working through different parts of the plan. So OpenAI actually published this recently in an article they wrote on Harness Engineering, where they talked about how they made the plan file first-class artifacts of the shared repository.

**Aakash Gupta** (00:48:20)

Very cool. So you and your plans, not just the final strategy docs. When you're, again, checking in that PR, you'd include the plan document in there. And do plan documents get summaries like customer calls?

**Hannah Stulberg** (00:48:33)

No, you don't want to summarize the plan because you want another session to be able to build off of that plan in its entirety of every single thing that you did. And when this finishes, I'm going to show you, I might actually just pull up. I have a different... have a pre-built plan for writing a strategy doc. Another concept that I want to talk about as it relates to planning is actually asking Claude to show you the agent prompts that it's going to use. So think about it. We're saying, okay, Claude is like a junior. employee, you want to be able to check its work and understand, are you aligned on the outcome that you guys are going to achieve together? And so when Claude, as part of a plan, is kicking off other agents, now you have a junior employee kicking off even more junior employees.

**Hannah Stulberg** (00:49:19)

And again, you might want to know how this employee is going to direct the work of the other employees, because again, you might be misaligned or you might not have the same goals. And so in my plan files, I actually like on complex plans, I don't do this on every I like to have Claude write out what it is going to prompt every single agent with. And so here I see the agent prompt in the plan file. What is that agent writing? It's going to use my writing guide. Okay. What's the context that this agent is going to give? what files is that agent gonna read? And then how is it gonna write that section? And this is really important because especially on writing tasks, if not all agents get the same context, or if you don't know, what files that agent is going to read, you don't know that they're going to have the right context to effectively write that part of the document.

**Hannah Stulberg** (00:50:11)

And the reason to split long doc writing across multiple agents is again, because of the size of the context window. Writing is actually pretty expensive operation. And when you're writing a very, very long form doc with all the thinking and reasoning and all the docs that you need to synthesize in order to write the doc, you generally cannot have one singular agent read 40 context files and go write a great doc. And so I like to be pretty directive of, okay, what are the different sections of my doc? What is the context that you need in each section? And then who's gonna write that section and then synthesize them all together with the orchestrating agent. Another big planning tip for this type of a plan is that you want all of the agents to write their output to temporary files, which you usually have to prompt odd into.

**Hannah Stulberg** (00:50:56)

Claude will not do this always automatically. And so it's something that I always check for as I'm planning with Claude. And the reason for this is that two things. So again, going back to the theory of context, Claude can only hold a certain amount of information. If you have maybe 10 agents running at the same time, and they all at the same time return their work to the parent agent, everything is going to crash and you will lose all the work that you just did. And so it is very important that you have each agent actually store its work in temporary files and then have your parent orchestrating agent work off of those files to like compile the final synthesis, for example.

**Aakash Gupta** (00:51:31)

Got

**Hannah Stulberg** (00:51:31)

it. Okay. So we finished some research. It's asking me more questions. And then the last thing that I wanted to quickly show, yes, we're going to save all of these, is how I like to invite Claude as a thinking partner. So you saw throughout the planning process that Claude was using the ask user question tool to ask me questions that it felt like it needed to ask in order for us to build out this plan together. But what I like to do is actually invite Claude to push my thinking and help me to be like a better PM. or consider things from different angles. And I'm going to show you how I do that if it will finish rewriting this. Another technique that I like to use because I find that having a lot of terminal windows open is very confusing is I actually name all of my terminals.

**Hannah Stulberg** (00:52:14)

So I would call this strategy doc. And then like, I would actually, you know, I would maybe name this like prompt example, and I like my work to be really pretty. So I will also usually like change the color of them. And I also might like set an icon as well. You can set custom icons too. I usually have like 20 or more terminals open at a given point in time. And so if they're not like named and color coded, then I usually can't find my work. And I found that a lot of people like don't know that you can do this.

**Aakash Gupta** (00:52:40)

I don't color code it or add a custom icon. I think I needed to get to that level.

**Hannah Stulberg** (00:52:44)

Yeah, I really like picking the different icons. Um, and sometimes I use it to like, I have like, you know, maybe this is like where I'm opening all my PR. So I'd put like a GitHub icon or something like that. Um, but yeah, I really like, um, I like to color code to know, be able to keep track of things and then also name everything. Okay. So now I'm going to open up the plan file again. Um, and here is where I'd really like to invite Claude to be a thinking partner for me. So now what I'm going to say is, um, use ask user. question tool to push me on my thinking and help me consider other angles that we might want to pull into this document, different sections that we might want to add to the final doc or other questions that you need to clarify my goals for why we're doing this.

**Aakash Gupta** (00:53:28)

This is by far the most comprehensive planning process I've ever seen.

**Hannah Stulberg** (00:53:34)

Um, and so now Claude is going to ask me questions and you can have Claude interview with you like pretty in depth. Like I might say, I didn't do it for this demo, but I might say, take as long as you need, ask me as many questions as you need. And we're going to, now it's going to start to ask me a lot more questions about what I'm trying to do here, which is going to help us to further refine the plan. And by the time all of this is said and done, we're going to have a really, really robust plan. Okay. So yeah, now it's saying, you know, what's driving the timing of this document. It's going to change the framing depending on why we're doing this. I'm just saying this is a strategic inflection point. And then it's saying, you know, there's some hard questions missing.

**Hannah Stulberg** (00:54:13)

What are other angles that we should have this doc address? Maybe there's fights that we want to walk away from. lot of pushes here. So let's just cover some of those. And then it's also calling out like other areas that we might want to add in. Okay. Yeah. I'm just going to say yes to this. And so yeah, now it's like pushing my thinking, right? It's catching gaps in my reasoning. It's pushing me to consider, you know, did I intentionally leave something out? Did I not? And now Claude and I are getting very crisp on what is going to be done here. And now it's asking me more questions. So I'm just hitting enter here for the purposes of this demo, but usually I would read them. I would think about it. I would usually give more feedback on these questions and usually dictate my thoughts until Claude really understands how I'm thinking about this problem.

**Aakash Gupta** (00:54:56)

So most people, they're rushing in. They're just letting it write the first draft, the strategy document. Then they're yelling at it and saying, you got this wrong. You forgot this frame. Your approach is, let me spend two to three hours

**Hannah Stulberg** (00:55:08)

getting the plan right

**Aakash Gupta** (00:55:10)

and then iterate on it.

**Hannah Stulberg** (00:55:12)

Exactly. Yeah, so now it's asking me more questions. And I think the other thing, which we touched on very briefly, is that I have different, so I have in this repo, like an example of your user level dot cloud folder. And here I have different like writing guides for different types of docs that I would write so that Claude can better write in my voice. These are just dummy guides. And so whenever I'm doing writing, I make sure always that in the plan, the agents are given my writing guide because they might not auto invoke the skill. Skills only have like a 70% or so like auto invoke rate. And when you're going to let something run for a long time, I don't see why you would leave anything to chance. And so I will always usually explicitly in the plan, if I want a certain command run or a certain skill called, I will make sure that that is specified in the plan document.

**Aakash Gupta** (00:56:00)

Yeah, I always say use X skill and triple check that that's there. The skill is like a lot of the alpha, if you guys haven't realized quite yet. So those dummy ones that she has right now aren't actually going to be super useful. It's like the value is when she has that skill then she goes to a product review sees some other PM at DoorDash wrote an amazing strategy doc she tells her skill hey I need you to go improve here's another good example and then she runs a whole process using this skill and she says I fell apart at this point go iterate and improve and then your skill itself improves over tons of iterations

**Hannah Stulberg** (00:56:35)

exactly Um, and so, yeah, now we're going to have a much more detailed plan. I don't want anybody scared. You don't generally need to spend two to three hours planning, but I think generally people are under planning and that's why you're not getting the output that you want because you left a lot of room for interpretation about what you were hoping to get. Um, and so now, you know, we have a much more detailed, um, plan file. And we're not going to read the whole thing here, but this is where I would keep going. I would read through all the changes. I would make sure I'm aligned with them. And then kind of a last important technique is a couple of things. So this should, oh, it already did the research. That's why. If a plan has phases, which this one doesn't totally because we didn't fully set up having it do the full research.

**Hannah Stulberg** (00:57:25)

I would actually outline the different phases in the plan and have Claude track when each phase is complete. This way, if you need to have a long running plan over multiple days and you have to compact or stop in the middle, Claude knows exactly how to pick up.

**Aakash Gupta** (00:57:42)

Kind of like writing those progress markdown files that you talked about earlier.

**Hannah Stulberg** (00:57:47)

Exactly. I usually keep this all in the plan file because the plan file gets reloaded after compaction. And what we'll notice here, so the natural plan files, they have these like really cute names from Anthropic. They all have like three words, but they are ephemeral. So they're stored in your dot cloud folder at the user level. You can actually open it up and see them. but they are wiped every 24 to 72 hours. So again, if you spend a lot of time on a plan and you want to save it, I will actually, as part of that plan, usually save the plan file down so that I can reference it in the future, even after the plan has been completed. So I'm likely going to be doing similar work.

**Aakash Gupta** (00:58:24)

Does everything get a plan? Every strategy doc, every feature results, right up every PRD are some things well enough defined via skills and other contexts that you don't need a plan.

**Hannah Stulberg** (00:58:34)

I don't think that there's a right or a wrong technique. I have generally found that anything that is relatively complex and requires synthesis or deep thinking where you want a certain output and you don't benefit from having a plan.

**Aakash Gupta** (00:58:50)

Yep. Makes sense. And it sounds like things that you're maybe a little bit less certain about, like we kind of approach this as like, we're not exactly sure even like what's relevant about stitch and the other competitors last three month launches. So it has to go out and do that first phase. There's more undefined. So that's where planning comes a little bit more useful. Sometimes you have a PRD where basically the team has already agreed on the whole feature and you have a meeting transcript, you can feed it. Then you might not need as much in depth.

**Hannah Stulberg** (00:59:17)

Exactly. If it's like a pretty straightforward task, you probably don't need, and also this is a very in-depth plan file. I don't do this for like all of my work. I try to tailor the level of planning to exactly what you were saying. What is the level of complexity and ambiguity? And then depending The more ambiguous and the higher complexity that something is, the more time and effort you should be investing in the plan. And that's also why I showed the technique here of just asking for a lightweight alignment proposal. I have still found that just doing this, you will get a lot better results because you can still be misaligned even on very straightforward tasks. And so I really like Claude to just quickly tell me If there's any level of vagueness, I like Claude to tell me what it's going to do. Usually I'll give a very quick correction and then sign off on it.

**Hannah Stulberg** (01:00:04)

And I feel like you get much better and much more consistent results with this methodology.

**Aakash Gupta** (01:00:08)

One of the practices you have that I think is really genius is how you are applying a beginner's mindset to learning and improving in Claude code. Can you walk us through that?

**Hannah Stulberg** (01:00:18)

Yeah. So I think honestly getting started in these areas can be like, it can feel very overwhelming and you can feel like, wow, I'm so behind and like, I don't know anything, but I think it's really important to have that beginner's mindset where you just feel really comfortable asking questions. Um, and so to do that, like I will usually ask Claude about anything I don't understand and ask it to teach it to me. So for example, I literally might say, you know, explain to me the benefits of why this repository is structured the way that it is, and also things that could be improved about the structure. And I would like do this and then Claude is going to like explain things to me. This is also how I improve what I'm doing. So Claude is like now going to analyze the repository and it might tell me some things that we didn't actually cover on this podcast about what could be improved.

**Hannah Stulberg** (01:01:04)

But I think that's the point. Like, well, I, you know, I've spent a lot of time using cloud code. I'm still learning every single day. Um, and I like to use Claude to help me learn and make sure that I understand why things are working, why things are not working.

**Aakash Gupta** (01:01:17)

So I use this similar prompt every day and I will say I have a slight tweak on hers, although hers is great. So what I do is I tell it first, I want you to go research everything that Anthropic has shipped in the last 90 days and create a calendar of all of the features. Then I want you to go read the top Claude Code influencers and the top posts that they've had in the last 90 days. Then I want you to compare my setup to the latest features and what influencers are recommending and tell me how I can 10x my setup. has just been huge for me because it's taking some of what we were doing with the planning on the strategy doc where it's going out and doing the research and we know that a lot of claude's data training data is quite stale it's like from 2024 at this point and so it doesn't even know about its own latest features sometimes i find so i think that that can also help it

**Hannah Stulberg** (01:02:05)

yeah and i think here's like another good example um So what's something we didn't cover in the earlier walkthrough is that I have a feature index in the repo and it's actually a YAML file. And so, you know, if someone was opening this repository and they didn't understand like why this was a YAML file, I would actually ask Claude to explain to me like the benefits of why this is a YAML file and why this structure is used and also what a YAML file is. And I would use this to like learn along the way. So I think oftentimes, you know, I see, you know, people right now on online are like sharing their skills and commands and agents with it, which is amazing. But then people are downloading them and using them and not knowing why these things work. And so I always, whenever I'm using anything, I always start by having Claude teach me why is this thing good or not good.

**Hannah Stulberg** (01:02:55)

And then that also makes me more comfortable iterating on the thing, because if you're just downloading and copying things and not understanding them, when it doesn't work the way that you expect, you won't know how to iterate on it or update it or improve it. And so now Claude gave me a really detailed explanation of what YAML is, why YAML is the right format for a feature index in your repository, and helped me to understand this topic and why this matters within the structure of the context of the repository.

**Aakash Gupta** (01:03:26)

This is how you all should be approaching these things. You're going to find more files that Hannah and I upload, other people upload that you're downloading. You're going to start cloning repos on GitHub. Make sure you do this process of learning about it. And that's why we included this segment in the episode, because the beginner's mindset is really important. Now we're going to cover a couple of the hot topics to make sure that you have a really well-rounded understanding of this. So Hannah. What's the biggest mistake PMs make when using Cloud Code for product work?

**Hannah Stulberg** (01:03:56)

I think the biggest mistake is that people give up too early. Like I think like learning anything new, it takes some time to learn how to use quad effectively to get really good at using quad code. And like you saw, building out this type of a context repository is not something that you're going to be able to do overnight. And so I think people try it for like a day. They don't get good results and they're like, oh, like this isn't for me. You know, I've I have spent now like 1,500 hours in Claude and I'm still iterating on my setup and improving it literally every single day.

**Aakash Gupta** (01:04:30)

And with the pace that this team ships at, they're constantly adding in new features, new things. And so just staying on the top of it, there's a lot to be done in terms of that constant iteration. So we've talked about Claude. There's Claude, there's ChatGPT, there's Cursor, there's Cowork. When should PMs be using Winch?

**Hannah Stulberg** (01:04:51)

I think there's not like a right or a wrong answer, although for most advanced PM work, you should be using some type of a coding agent. I think for chat, it's generally just if you need a quick answer that doesn't need like super high context. Otherwise, ideally, you're really building a context repository that you can use, that you can leverage with any coding agent.

**Aakash Gupta** (01:05:12)

If a PM only has two hours this weekend, what steps should they take to set up cloud code?

**Hannah Stulberg** (01:05:18)

So what I like to recommend for people is that the single biggest piece of leverage you have is freeing up your time to learn. Like I think especially right now, the most important thing that we can be doing is learning. And so if I had two hours this weekend, my question would be, What can I do to create six hours for myself next week? And I would find something to automate so that I can free up six hours to go learn things. And so generally, that's what I recommend for people is you should be trying to carve out at least an hour a day to just play with AI. And in order to have that hour a day, you need to automate work in order to free up your time so that you can learn and also help to uplevel your teams.

**Aakash Gupta** (01:05:57)

Amazing. What's underhyped versus overhyped in AI for PMs?

**Hannah Stulberg** (01:06:02)

I think that underhyped is following your curiosity. So I feel like there is a lot of pressure to always be on top of the exact latest news, like the exact latest release, and to get really good at whatever is being posted online on a given day. I think that we're all going to have a lot more fun and learn better if you're following the things that you're curious about. And so, you know, if AI evals don't get you out of bed in the morning, like don't start there, like start with automating something that frees up your time or start with, if you love design, like start playing with prototyping. And then, yeah, I think that the other thing that I think is under-hyped is building expertise in one area. So I think right now a lot of people are very shallow at like many different things, but it actually does take time and investment to like really learn a topic.

**Hannah Stulberg** (01:06:52)

And so I would say the other under-hyped thing is spending the time to go deep, even if that means maybe you're not learning some of these other areas right now.

**Aakash Gupta** (01:07:00)

You said Cloud Code is the most misleading name in AI. Why?

**Hannah Stulberg** (01:07:06)

I think because it's not just for coding, which I hope is what everyone took away from this podcast episode. While I do code and cloud code, most of my time is not spent coding. It's spent writing docs or doing analysis or building local HTML prototypes for my team or other types of prototypes, which actually we didn't get to show on this episode. I had a really fun one built. But I think it is not just for coding and it's not just for people who are technical. Again, my operations partners are also spending all day in Claude. They're contributing to our repository. It's really the best tool, I think, right now for doing knowledge work.

**Aakash Gupta** (01:07:46)

What should they have called it?

**Hannah Stulberg** (01:07:48)

Well, that's why I called my series Claude Code for everything. Because... I don't know what they should have called it. I do like the name Cowork. I think that was like a really great branding on their part. But yeah, I don't know if I have a snappy name for it.

**Aakash Gupta** (01:08:05)

What would you tell a PM who's scared of the terminal, scared of IDEs?

**Hannah Stulberg** (01:08:10)

I would tell them like, don't be afraid to be a beginner again. And there's, I mean, I hope what folks saw on here is in my mind, there's not a big difference between typing into a chat bot and like typing into the terminal. Once you've done it for like an hour or two, you'll probably start to feel pretty comfortable.

**Aakash Gupta** (01:08:27)

What MCPs do you need to hook your team OS up into in order to make it effective?

**Hannah Stulberg** (01:08:32)

Every single MCP that you can access. The limit does not exist. I am adding like a new MCP every couple of days at this point. But generally right, most companies are going to operate on like a certain tech stack, right? You're going to have a certain set of software vendors that hopefully have either MCPs or what's often under discussed are command line interfaces or CLI tools. Claude works really well with both of them. But the goal is any core piece of software that you use in your day-to-day work should be hooked up to Claude.

**Aakash Gupta** (01:09:04)

This has been a masterclass I have done, I think it's seven or eight cloud code episodes. And I was learning every single minute of this one. We covered how to create a team OS, how to set up that repo, how to write really amazing documents by creating a comprehensive planning process and how to have a beginner's mindset with cloud code. Hannah, thank you so much. If people want to find you online, where should they go?

**Hannah Stulberg** (01:09:30)

They should go read my Substack, which is called In the Weeds. You can find it at hannastolberg.substack.com. Awesome.

<!-- sponsor -->
**Aakash Gupta** (01:09:37)

I hope you enjoyed that episode. If you could take a moment to double check that you have followed on Apple and Spotify podcasts, subscribed on YouTube, left a rating or review on Apple or Spotify, and commented on YouTube, all these things will help the algorithm distribute the show to more and more Finally, do check out my bundle at bundle.akashg.com to get access to nine AI products for an entire year for free. This includes Dovetail, Mobbin, Linear, Reforge Build, Descript, and many other amazing tools that will help you as an AI product manager or builder succeed. I'll see you in the next episode.
