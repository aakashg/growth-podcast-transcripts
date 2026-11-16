---
title: "Claude Code + Analytics = Vibe PMing"
subtitle: "I got Amplitude Principal AI PM Frank Lee to give a masterclass on Vibe PMing with Claude Code, Cursor, and Your Analytics Data"
date: "2026-02-25"
host: "Aakash Gupta"
guests: ["Frank Lee"]
speaker_names: "substack"
substack_url: "https://www.news.aakashg.com/p/frank-lee-podcast"
youtube_url: "https://www.youtube.com/watch?v=WK0bZrS8pVs"
duration: "00:53:00"
word_count: 11590
source: "Substack episode transcript (aired audio)"
---

# Claude Code + Analytics = Vibe PMing

*I got Amplitude Principal AI PM Frank Lee to give a masterclass on Vibe PMing with Claude Code, Cursor, and Your Analytics Data*

**Frank Lee** (00:00:00)

What is the most powerful AI workflow you've seen? I think the most powerful thing is managing my product process in quad code and cursor using a bunch of MCPs. What does that mean in plain English? So basically you can service all of your product contacts into your agent or tool of choice. What can you do with this? Oh man, I think you do so many things. You can analyze charts, you can automate your weekly reporting, you can synthesize a huge amount of qualitative feedback, you can turn all of those insights into a bunch of specs, and then you can even push them to quad code or cursor to start prototyping directly in code.

**Aakash Gupta** (00:00:28)

So I've got one of the heads of AIPM at Amplitude, the principal PM in charge of their agents and MCP products here today. And we're going to walk you through everything you need to know to master analytics and cloud code.

**Frank Lee** (00:00:40)

I automate a lot of my weekly business reporting using a bunch of dashboard agents. I can easily analyze, run successive queries, pull in a bunch of data and just run a bunch of analysis on my product data. Wow. They made this conscious decision on like, how do we make the most powerful agent or what are the most powerful features and set of context that can provide the model so that People can code in ways that they've never been able to do before.

<!-- sponsor -->
**Aakash Gupta** (00:01:00)

What is the biggest mistake people make when using MCP? where if you become an anal subscriber to my newsletter, you get a full year free of the paid plans of Mobbin, Arise, RelayApp, Dovetail, Linear, MagicPatterns, DeepSky, ReforgeBuild, Descript, and Speechify. So be sure to check that out at bundle.akashi.com. And now into today's episode. Frank, welcome to the podcast.

**Frank Lee** (00:01:40)

I'm stoked to be here. Thanks for having me.

**Aakash Gupta** (00:01:41)

My pleasure. What is the most powerful AIPM workflow you have seen people use these days?

**Frank Lee** (00:01:47)

It's got to be managing your whole product process out of cloud code, cursor, and hooking it up to some product analytics providers like Amplitude's MCP.

**Aakash Gupta** (00:01:55)

What does connecting cloud code via MCP really mean in plain English?

**Frank Lee** (00:02:00)

Okay, so there's two different tools. Cloud Code, it's a terminal-based coding agent with access to a bunch of different Cloud models, but has some pretty cool stuff like MCPs, skills, a bunch of other actions. MCP, it stands for Model Context Protocol. And the simplest way to put it, it's the easiest way to connect your AI models with any external tools, action, and data. So we've used MCP a lot at Amplitude to connect a bunch of tools and data that we have to a bunch of external AI clients. So big ones include Cloud, Cursor, ChatGPT, and we use that to power a bunch of pretty complex coding and product workflows.

**Aakash Gupta** (00:02:33)

So what does this setup allow PMs to do?

**Frank Lee** (00:02:35)

So this setup lets you do a lot of things. So I automate a lot of my weekly business reporting using a bunch of dashboard agents. I can easily analyze, run successive queries, pull in a bunch of data, and just run a bunch of analysis on my product data, I can deeply investigate different trends that are happening in charts. So while I used to be creating a bunch of manual charts, the model is doing all of that for me now. It's really easy for me to explain why my metrics are moving because I can pull in all of the underlying feedback data to try to hypothesize about why things are changing. I can drill into specific account health of our users and also some timelines about what people are doing within our product just to see what their behaviors are like. I've been actually using these models to draft a bunch of PRDs based off of this analyzed product context that MCP makes so accessible in Cloud Code.

**Frank Lee** (00:03:22)

And then if you're really venturous, you can actually take some of those insights that you're generating, convert them into PRDs. If you want to route them to a human, you can push them into JIRA or linear via MCP. But if you're really daring, you can also push them directly into Cloud Code, Cursor, and try to draft some prototypes on your own.

**Aakash Gupta** (00:03:38)

Okay, so it's really the gateway drug to all of the 10x AIPM workflows that people talk about these days. Before we really get into this, can you show us how to set all this up?

**Frank Lee** (00:03:48)

All right, sounds good. Let me walk you through how this is set up. So I'm actually going to jump the cursor. If you see this repo, I've spun up my own Amplitude product repo. So on the left-hand side, I have a bunch of contexts that I've already actually aggregated about all the different product lines that I work on. So for example, we've been working on agents, agents, AI feedback, Ask AI, like a lot of our enterprise control features, MCP. So I have specific folders and contexts and files detailing about some of the initiatives that we might have within our roadmap, some of the specs that I might be thinking about, and also just a bunch of these different learnings and verbiage that refer to the specific parts of this product. So within Cloud Code or within Cursor, I can easily refer to some of those pieces of context, brainstorm about it, draft new spec.

**Frank Lee** (00:04:30)

But I think the most interesting thing from the most recent changes in Cloud Code and Cloud Iterating on this new protocol called skills. So I'll just jump into a specific example. But I've created this specific skill. And the way that I simply think about this is it's a clear name about what the skill is. There's a little description about what the skill is and when to perform it. So that's some metadata that the models can use to determine when to use that function. But at the simplest nature, this is just a prompt. There's a prompt about what is this specific task that I'm accomplishing? What is the set of heuristics or steps that I might take? And then also you can configure what set of tools you might use that is connected to MCP in order to accomplish that objective.

**Aakash Gupta** (00:05:10)

And

**Frank Lee** (00:05:10)

so we actually had this model, this tool released recently called Auto Insights, which I can point it to a specific chart. We'll pull anywhere from 20 to 30 of charts that are similar to that based on relevant properties. And then we'll do a bunch of analysis, try to find the specific segments or the specific group buys, and then try to figure out why things are changing, hypothesize about what the biggest drivers are. And for a human, that would have taken hours for me to spin up all these charts. We've actually replicated a lot of that using this cloud scale. So I taught like this model basically, hey, look at this chart, pull this data from using MP2's MCP on the URL. You can basically, here's some heuristics about like how to identify and like look at specific patterns. So look for spikes, look for seasonality, look for anomalies.

**Frank Lee** (00:05:55)

And then basically taking some of that context, trying to look at other tools, like within our feedback, within our releases, within our annotations on like some amplitude data. Can I explain that analysis? And then I give it a format, like tell me what happened, when this occurred, what is your primary hypothesis about what changed, some plausible explanations, your evidence, and then what this means for us as a business. And so I'm going to jump into Cloud Coded and Terminal real quick, where I can kind of show you an example of like where this ran.

**Aakash Gupta** (00:06:21)

All right. So I have sort of two separate follow-up questions here. Let's first start with the context. So what is, through trial and error, what have you learned is the right context you should be including here for CloudCode? Because I know there's always this concern about just using up your context window also. So there is a concept of too much context, but what is the right amount of context and how do you organize that so that CloudCode can ingest it well?

**Frank Lee** (00:06:47)

Yeah, I actually don't worry about it too much because you basically can refresh a lot of the context every time you start a different session, right? So within Cloud Code, you can, like, within Terminal, if I feel like I'm running out of context, I can just exit out and then basically it'll refresh the context. Similarly, with Incursor, if I wanted to spin up a new agent, I could just jump to the top, like, right, spin up a new tab and it basically refreshes, like, it forgets what was happening in, like, a prior thread and then I have a fresh set of context in order to do that. That being said, there is a bit of context management that you do have to think about. One of the trade-offs of MCP is that a lot of the tools that you might have loaded. So let me show you an example.

**Frank Lee** (00:07:23)

I have Amplitude's MCP hooked up. So there's a bunch of tools that are here. Same with Linear, I have that hooked up. So the context from what tools are available, the names, the descriptions, there's also some instructions tied to each MCP on what's the specific format that this MCP uses, or how do we want the data to be used, or some preferences on when or how the tool should get used. So that does fill up some of the context, depending on what MCPs you have loaded. That being said, most folks don't have a huge amount of MCPs loaded up. I think even with amplitude and linear loaded up, I might be using up anywhere from five to 10% of my context. So I haven't actually run into that many limitations when doing some of like this product specific analysis. That being said, if you are doing a really long analysis, so for example, pulling in a huge amount of chart data, doing a bunch of successive queries, pulling in huge reams of feedback, sometimes you might run into context issues.

**Frank Lee** (00:08:13)

The one benefit on Cloud Code is when you start running out of context, They have this feature called compaction where it starts trying to summarize some of what happened in that thread, consolidates that into some smaller summary, and then lets you move on given the fact that you had like reached the previous set of context. And then there's also just like a pretty big like bitter lesson take on it. You can worry about like context management now. The reality is in like the next few months, a lot of the new models release, they'll probably expand their context windows or have some different mechanisms with an agent client to handle some of that complexity for you. So just build for the future and like think about pulling in like what what's most relevant to give your agent like the best types of responses.

**Aakash Gupta** (00:08:50)

Yeah, you can use the slash compact command. They actually show you how much percentage of your context window you're using up in cloud code now. So I recommend for people when you're hitting that 90% or something, don't just rely on the slash compact. Actually, I ran into this problem at about 1 a.m. last night where it said conversation too long can't compact. And so my newest sort of hack is when I'm at like 90% or so, because I don't want it to just fail at compacting. I will say write a markdown file of your process and your progress and what you have left to do. That's a good way also to kind of transfer the context over if you need to. So you answered that we can put almost as much context as we want. So what context, like, can you walk us through specifically, like, what sort of methods are you using to get context, like meeting notes and stuff in there?

**Aakash Gupta** (00:09:35)

And how have you structured those folders and files in here?

**Frank Lee** (00:09:37)

Yeah, sounds good. At the simplest, like,

<!-- sponsor -->
**Aakash Gupta** (00:09:39)

I have a product folder. Today's episode is brought to you by Amplitude. Replays of mobile user engagement are critical to building better products and experiences. But many session replay tools don't capture the full picture. Some tools take screenshots every second, leading to choppy replays and high storage costs from enormous capture sizes. Others use wireframes, but key moments go missing, creating gaps in your understandings. neither approach gives you a truly mobile experience amplitude does things differently their mobile replays capture the full experience every tap every scroll and every gesture with no lag and no performance hit it's the most accurate way to understand mobile behavior see the full story with amplitude Today's podcast is brought to you by Pendo, the leading software experience management platform. McKinsey found that 78% of companies are using Gen AI, but just as many have reported no bottom line improvements. So how do you know if your AI agents are actually working?

<!-- sponsor -->
**Aakash Gupta** (00:10:35)

Are they giving users the wrong answers, creating more work instead of less, improving retention, or hurting it? When your software data and AI data are disconnected, you can't answer these questions. But when you bring all your usage data together in one place, you can see what users do before, during, and after they use AI. Showing you when agents work, how they help you grow, and when to prioritize on your roadmap. Pendo Agent Analytics is the only solution built to do this for product teams. Start measuring your AI's performance with Agent Analytics at Pendo.io slash Akash. That's P-E-N-D-O dot I-O slash A-A-K-A-S-H.

**Frank Lee** (00:11:10)

So these are some different product lines that I'm working on. So agents, AI feedback, ASCII, enterprise, features, MCP. So within each of them, I might have some context about what is our like Q1 plans. I won't show it because there's a bunch of stuff there, but for fans, like we're thinking about forms of memory, like ambient agents, different types of agents that we're thinking about. So these are basically specs that I've converted into markdown files that I can refer to pretty easily using like the at command. if I wanted to brainstorm from a given like PRD or just say, hey, we already have a bunch of planning within like our Q1 plan. Can you actually just fetch all of the specific items and then turn those into drafts of PRDs? And so as example, I have a few templates actually for some like pretty recurring types of tasks I might do.

**Frank Lee** (00:11:52)

So like, For example, draft short PRD. So give me a sense of the problem context. Talk through in narrative form what a solution or workflow might look like. Here's how I want you to format or break down that response. Here's some heuristics on how do you think and strategize about what to build. So there's some light heuristics that I typically might have on selecting features, emphasizing simplicity. It's okay to say no. Here's how to think about some of the design techniques. for like principles for some of these features and then taking some of those requirements that might be in the doc or might even live elsewhere and turn that into acceptance criteria here. So that's just a sample. But if, for example, in Cursor is like draft a quick PRD using the PRD template, So it pulls this into context immediately, knows what the format I'm looking at.

**Frank Lee** (00:12:38)

And then I could talk about, hey, talk about this specific topic or refer to this doc where we have a bunch of ideas and structure that into a better format. So that's one example. I guess the other thing, you touch a little bit on granola. I've been playing around with this. I use Cloud Code actually to try to create some of these light little automations or connections that I previously wouldn't have. So my understanding as of now is Granoladark actually does not have a dedicated MCP right now. So I try to hack Cloud Code to build some type of automation so I can adjust some of my calls. So if you see here, there's some notes, say like the year, month, and then there's some meetings that I've had. And so it tries to inject some of like the summarized notes there. So this, for example, this is like our MCP standup that happened.

**Frank Lee** (00:13:19)

I basically could run a command. Can you pull in my recent granola notes using the script we wrote? let's hope this works i haven't run this in the last two days but basically like that's that's also a part of my product repo where we have i use cloud code to create the script and it's going to run like this command terminal and then yeah you see there's a bunch of these meeting notes that like were previously ingested that auto get dumped in um so if you want you can refer to like the whole folder so i'm like hey at 2026 um or that's like a specific one but like the at 2026 01 folder here you You immediately pull all of those notes in context. If I wanted to say, summarize the main takeaways, give me the specific action items, I can put that into another folder.

**Frank Lee** (00:14:02)

But basically all this stuff is immediately accessible if you needed to, because it's all like consolidated in that one system.

**Aakash Gupta** (00:14:07)

Amazing. Love this use case. I think most people should be using this specific one. So how do you get around the MCP? He created this little function or skill or script in this case that he referred to it with cloud code so that he could access those granular meeting notes. And how are you using Obsidian and Conductor in your workflow?

**Frank Lee** (00:14:23)

To be quite honest, not too much. I think those are the powerful if there's specific nuances on, for example, Conductor, right? So I have it pulled up. Conductor is a great tool when if you have a bunch of coding agents that you want to run in parallel, the problem is oftentimes if you have one branch of your GitHub and you're trying to push changes, if you kick off a bunch of cloud codes in the same branch, oftentimes they might have a bunch of changes that conflict with each other. They're not really talking to each other. So the thing that they nailed on Conductor was they made use of this feature called a Git work tree, which essentially copies your repo into a separate like work tree. So then you can run multiple cloud codes in parallel branches. They won't conflict. And basically you can decide to change, like to merge some of those changes like together.

**Frank Lee** (00:15:08)

Going into the huge amount of agent orchestration workflows, if you're trying to run five to 10 of these coding agents in parallel, Conductor is probably the best in class tool that I've seen for that. I know there's a lot of excitement in the industry on what is this orchestration framework looks like, but this is the prettiest and best that I've seen so far. But for just a call for specifically product management, I don't really need too many tools. Like it's not a big deal for like this model to conflict. Like if I'm kicking off a task, like usually I wanted to create one PRD here for this team, or I want you to do an analysis here. So there's not as much of an issue where like the code conflicts within this branch. And so it's honestly probably easier to just do it directly within different tabs and terminal instead of having to spin up a bunch of Git work trees.

**Frank Lee** (00:15:48)

But if you're doing specifically these coding tasks, trying to do it all within the same branch is basically just going to lead a huge amount of messiness

**Aakash Gupta** (00:15:54)

and where does obsidian come into the workflow

**Frank Lee** (00:15:56)

yeah so it's it comes with personal preference obsidian basically has access to your file system the same way that a cursor also does if you hate staring at markdown then obsidian is like a pretty wrapper to directly make edits like it's more akin to like a typical text editor but me personally i love playing around with a markdown specifically i like I spend a lot of time coding myself and it reads pretty well to me. So it's kind of just nicer to have the same tool where I can push code, push changes directly and use the agents natively using cursor or within cloud code.

**Aakash Gupta** (00:16:25)

Yeah. And you can also just double click or right click on any of these MD files and hit open preview or I do up Apple shift V and you can look at these pretty. So I feel like the Obsidian hack, it's not really necessary. So yeah, we got people to set it up. What are the top use cases of cloud code and MCP with analytics for product managers and product analysts?

**Frank Lee** (00:16:47)

I think there's five things that I'm doing really heavily. So first one, anytime there's an anomaly or some type of big change in my metrics, I'm using some skills and tools within Cloud Code and our MCP to analyze and do some deep chart analysis. So I drop in a link and basically the agent can figure out exactly what specific segment or what little group buy or what specific related metric might hypothesize and lead to that change. So that saves me a bunch of time. I think the second thing is I've automated basically all of my weekly business reviews and dashboard reporting. At Amazon, I spend all of my Sundays just coming up with our metrics and explaining why things are happening. Now I've pointed this to Cloud Code and some of these like Amplitude dashboard agents and Monday morning I come, all of the five to six dashboards I look at are automatically synthesized.

**Frank Lee** (00:17:31)

I know exactly the three to five top insights for me and I know the one specific urgent issue to tackle with my team. I don't need to analyze the dashboards anymore. I can just start focusing on solutions with the team. And the third one is doing a bunch of deep qualitative customer feedback analysis. With Amplitude MCP and the AI feedback product, all of our tickets from Zendesk, Slack, Amplitude surveys, that's all unified in one place now. So I can just point cloud code, tell it to analyze the feedback related to AI, agents, MCP, and then the agent will navigate all of our tools, consolidate all the data, do its analysis and clustering, and then give me a clean report of exactly what the urgent issues are, what the bugs are, and then what's the single most thing that people love about our product that week. Fourth one, spend a lot of time taking those insights coming in from those dashboard agents or like this cloud code chart analysis.

**Frank Lee** (00:18:21)

And then given this context, can you think about what's the right set of actions or plan to do to resolve this space? So I've given this agent some heuristics on how I think about coming up with the solutions and the agent's The agent can go at length, explore a bunch of different ideas. I can drop in some images and then it can just turn that into a spec so that I don't have to write it anymore. So Opus is like the best thought partner that I've ever had on coming up with some of these like design and product ideas. And then lastly, I've kind of totally reshaped like how I think about what I route to the team to build versus what I just do myself now. I can take these PRDs or take some of these problem statements that the agent had surfaced. If it's easy, I just drop it into cloud code or cursor directly and then it could pre-draft some of the solutions for me while I'm in a meeting.

**Frank Lee** (00:19:03)

But if it's a really tough problem, I can go ahead and hit the linear MCP and say, hey, I want to route this to the AI capabilities team or the MCP team, file it under this specific project and assign it to this engineer and then assign it to Cursor as a courtesy to hopefully soften the workflow on their end. So these are the five things I'm doing the most frequently.

**Aakash Gupta** (00:19:22)

I love these. This is the new Vibe PMing workflow. These five use cases. Can you demo each of these for us? Just for context, this

**Frank Lee** (00:19:30)

is one chart that I'm looking at on the MCP side. We're curious about like, what is the average number of tool calls that might happen in a given week? and i'm seeing this anomaly where like the average number of tools being hit is 8.1 for this week which is quite different it's something that's worth investigating because i need to figure out how do we manage the right tools the descriptions and make sure nothing's broken right so i can take this link if i jump into cloud code like i said i had a bunch of these different skills that i had so there was the analyze chart skill which i'll just preview real quick for you here Analyze chart. So remember, there's a name, description, and a bunch of heuristics on what to do about it. If I do the slash command, basically that can trigger that specific skill for you.

**Frank Lee** (00:20:10)

So analyze this chart and explain why there's a jump this week. So stepping in here. So this might take a bunch of time, but now the agent is... connected to the Amplitude MCP. So you can see here it's parsing the URL. It's starting to pull in some data on the chart. And then we have some tools that let you navigate the data. So there's a chart data. We can create the underlying data set. And then basically the model starts showing its work on how it's navigating your taxonomy, how it's navigating relevant charts. Maybe it's navigating the specific events and properties related to that. So this might take a few minutes. But basically, you can see the agent reason about which charts it's looking at, which events it's looking at, or what are some hypotheses about where this might change. And

**Aakash Gupta** (00:20:53)

so

**Frank Lee** (00:20:54)

it's navigating the properties. It's breaking it down by what it thinks might be that spike. Now it's pulled in a different chart. And if you think about the human equivalent of this, it's the same as me having five different versions of this chart. I had to go manually group and cut this by a specific property that I have in my head. Or I might have a create a separate chart where I look at a different event that's like somewhat related to it or like there's a bunch of this manually manual like iteration on the GUI that I had to do like creating a bunch of different these charts and now the agent is doing all of this just via via terminal so you can see here this is the format that I specified for it but it says here's the chart here's the time range I looked at here's the metrics that's analyzed and it walks you through like that a spike happened, when it happened, the underlying data that led to that, and then some hypotheses about it.

**Frank Lee** (00:21:38)

So detected that there's a change within the types of tools that we had analyzed, enabled. It has access to our experiments and feature flags data. So it saw that there is some changes within what feature flags we had enabled, which provides different tool access. And then, so you see some flag activity, there's some differences in historical precedents, and then hypothesized about something else that might have changed. Maybe it's data quality, a different power user. So basically like what I would have had to do manually to investigate and explain what's happening. The agent just, I think it literally did this in like a minute and a half. And this would have taken me probably like one to three hours, depending on how complex that query was.

**Aakash Gupta** (00:22:15)

Yeah. And that's with having a background as a data analyst. If you're just not having that background, it might take you half a day.

**Frank Lee** (00:22:21)

Yeah, and that's assuming you know which properties to look at. Basically, because at least on the Amplitude MCP side, we've done a huge amount of configurations on how do you simplify the names of the tools and the descriptors or how do we improve our underlying search infrastructure or how do we capture the right context about when to use a specific chart or when to use a specific dashboard or when to use a specific event. And that context is all provided to the agent via these MCP tool calls so that it can more accurately navigate that data for you. And so if you compare this to an expert of the taxonomy, it's probably the difference of this running in one and a half minutes versus them spending 10 minutes navigating the chart. If this was a person that did not know that taxonomy, they would have either gone the wrong answer or they would have had to spend like two days chasing down the right person in the org that could tell them what to look at.

**Frank Lee** (00:23:06)

This agent basically was able to figure it out itself, given a lot of this underlying semantic infra.

**Aakash Gupta** (00:23:11)

Very powerful. So deep chart analysis. I think I understand this use case. Really, the powerful thing here is you write yourself a skill and you teaching it how to navigate the MCP and make the right tool calls. Yep, exactly. Totally understand this workflow. What's the next workflow? That was around automating dashboards, right?

**Frank Lee** (00:23:27)

Yeah, the next one's around automating dashboards. So similarly, I have an analyzed dashboard scale. So here's when I use it, meaning prep, dashboard investigations, connecting quanta qual. And I can show, like, I instructed the agent to look for the URL, query the underlying charts, fetching them, like, three at a time, because there's some context limitations, like, when you're interacting with some of these tools. Look for these specific things. Like, if it's a KPI chart, like, look at this and the percentage change. If it's a bar chart, like, it concentrations of gaps. So teaching them some heuristics on, like, how I, as a human, would have thought about, like, this data. Mm-hmm. And then what's cool is now that this agent has analyzed a bunch of charts and figured out what's happening in the dashboard, I pointed it to, hey, go pull the feedback data recently and see if there's anything relevant there.

**Frank Lee** (00:24:10)

Or we don't have it here, but we also have access to session replays or experiments. So basically, depending on what data you have and whether it's relevant to a specific dashboard, you can instruct it to also query that as part of its agentic workflow. So this is, and then this, here's like the takeaway of like how I wanted it presented, just personal preference on what I think is helpful, some best practices. But in reality, like, let me, let me show you. So I'll, I'll start over just given the context piece, but here's Claude, analyze dashboards. Let's pull in. So we're talking about MCP. So can you give me a TLDR on my external MCP usage dashboard? And so this is different than last time, because like last time I gave it an explicit URL, which is and this time I'm kind of by giving it some like some natural language query.

**Frank Lee** (00:24:55)

Right. So if you are an MCVPN, you have to spend a lot of time thinking about, hey, a lot of folks are going to give you pretty ambiguous natural language questions. How do you like take those queries and then like teach the model to figure out how to use your search infrastructure or navigate your data so that it pulls the right thing? So I have a dashboard that's called external NCP usage dashboard. So it's quite, it's like, it's kind of cheating. But if I told it said, Hey, pull the MCB dashboard, you can teach it on the tools to be like, Hey, here's how you think about using like the search endpoint, or here's how to filter the data properly or run a few different like searches and then figure out like reason about what's the best response. So there's a lot of different little experiments you can do on like optimizing the tool.

**Frank Lee** (00:25:33)

But now you can see it started looking for external MCB usage, MCB usage. These are different search queries it was running on our search endpoint on the dashboard data. It identified the dashboard, and then it has a different tool for querying those charts. So it's pulling in those different chart IDs three at a time because that was the instruction I gave it. And then now, once it's pulled all of that data in context, it gives me a quick overview about what some of the metrics look like. So I won't spend too much time on the metrics because that's our metrics, but... You kind of see like, oh, once again, I could have spent the 10 minutes scanning through all of the charts in my dashboard. And then if I found anything that was interesting, I would have to copy paste some of those individual data points, pull them into a specific part of the bullet points that I would summarize.

**Frank Lee** (00:26:15)

I'd have to think about the narrative. I'd have to jump into my AI feedback and run a search on MCP and see if there's anything relevant. But the model, given those instructions, did it all in, what was that, like a minute and a half as well? Yeah. That saved my whole Sunday again.

**Aakash Gupta** (00:26:30)

So that was the promise, right? We were going to save our whole Sunday. So if I recall, like I used to do this too, like when I was at Epic Games, PMs used to have a pretty, pretty much do the analyst hat as well. So I remember on Sundays for my Monday meeting, I'd spend like six hours going to various Tableau dashboards, having them load, copy pasting them, interpreting them, analyzing them. How do you put together that whole workflow of like, these are my 25 typical WBR slides. Go pull those all for me.

**Frank Lee** (00:26:54)

So we don't currently do WBSR anymore. I have agents that are automatically pushing these reports into every single product team's channel. So instead of having to sit now Monday and review the metrics, all of the main takeaways, all of the goals, all of the main deviations, there's already a draft of that there. And then basically each PM, myself included, we can have our own planning meetings with our specific clients. whether that's our stakeholders or within just my engineering team. If we want to talk about the metrics, we can, or we just spend the time more focused on like the tactical as opposed to like the reporting.

**Aakash Gupta** (00:27:26)

How do you schedule things here?

**Frank Lee** (00:27:28)

I do this via the dashboard agent that's in Amplitude. I don't know if you want me to show that real quick.

**Aakash Gupta** (00:27:32)

Yeah,

**Frank Lee** (00:27:32)

let's see it.

**Aakash Gupta** (00:27:33)

Yeah.

**Frank Lee** (00:27:33)

So this is like the, we've had this probably for a few months now, but this is the Amplitude agents like kind of inbox. And so you can see here, I have a bunch of these different scheduled, these different scheduled agents went to different dashboards across the company. So automated insights, the overall like AI native Amplitude dashboard, like analytics foundations, like website optimization, like there's a bunch of these specific agents that have spun up based off of dashboards i've created um so there's a dashboard agent i pointed it here i gave some context about like you can give it some context optionally like we have a pretty robust system prompt on how to think about this but if you want to do weekly monthly business reviews you can if you just want to report on a new feature there's a bunch of these little prompts that like basically we want to guide people on how to do it and surprisingly to me like i came from like a startup background most recently When you're dealing with enterprises, like most folks don't like, they're not super familiar with Asians.

**Frank Lee** (00:28:22)

They're not sure like what knobs they can turn when they're creating an agent. So giving them really easy understanding of how to create it, what system prompts, what the agent is steered by is extremely important. low agent creation flow until we brought in these starter prompts. And then we saw the relevance and like the agent creation conversion pretty dramatically improve once we did that. So this is just an example of like this within the agents page. These get pushed all like into Slack, into email. There's a bunch of folks that are consuming it there. People actually don't spend that much time on these asynchronous agents within the product. Like the idea for at least these specialized agents is let's get them into all the places where people do their work. So

**Aakash Gupta** (00:29:00)

on

**Frank Lee** (00:29:00)

Slack, if we wanted to push that into email, if we wanted to push that into Teams, or if we wanted to push these insights to the GitHub, there's a lot of work that we do on the agents at MCP front, whether that's via partnerships, integrations, et cetera, to get these insights to where they're most helpful at.

**Aakash Gupta** (00:29:14)

Makes sense. So I think I understand the second workflow. What's the third one?

**Frank Lee** (00:29:17)

The third thing that I do religiously on those Mondays, so we've pulled in feedback from a bunch of different places. So this is the new AI feedback product that we launched in November. We're pulling data from Zendesk, Intercom, Salesforce, Gong. There's a bunch of stuff coming in from public channels, G2, app stores, et cetera. And then it's not here, but we also have an integration with Slack that we're prototyping right now. So all that data gets piped into AI feedback. It gets auto-analyzed. But sometimes, like, it's not exactly what I want. Like, this is a specific tag or, like, insight that I have. But I might have, like, a specific pointed question I might have for it. So let's start the instance of Claude. So once again, I have a specific skill that I've created in the template for that. Analyze feedback. Pull in my agent's MCP and other AI-related feedback.

**Frank Lee** (00:30:03)

Give me TLDR. So when I was working on Anari, teams would basically do all of this stuff in spreadsheets. There'd be a huge amount of these customer surveys, or they would be copying, pasting messages from Slack, or they'd have to send this crazy integration with Zapier to pull in data from one place into another. Our product pulls all this in one place for you and exposes it via an MCP tool. So we have two different tools we've tuned for this. One is for those pre-processed insights that I showed you, we can provide access to that. And then we also provide access to the underlying feedback mentioned data. So you can see here that the MCP is looking at what is the set of insights that are already created, but also what is some of the underlying data that's most recent. And then it's going to use that to generate a quick response.

**Aakash Gupta** (00:30:47)

Mm-hmm. AI is writing code faster than ever, but can your testing keep up? Testkube is the Kubernetes native platform that scales testing at the pace of AI accelerated development. One dashboard, all your tools, full oversight. Run functional and load tests in minutes, not hours, across any framework, any environment. No vendor lock-in, no bottlenecks, just confidence that your AI-driven releases are tested, reliable, and ready to ship. Testkube, scale testing for the AI era. See more at testkube.io slash akash. That's T-E-S-T-K-U-B-E dot I-O slash A-A-K-A-S-H. I hope you're enjoying today's episode. Are you interested in becoming an AI product manager, making hundreds of thousands of dollars more, joining OpenAI Ananthropic? Then you might want to do a course that I've taken myself, the AIPM certificate ran by OpenAI product leader, McDad Jaffer. If you use my code and my link, you get a special discount on this course.

**Aakash Gupta** (00:31:49)

It is a course that I highly recommend. We have done a lot of collaborations together on things like AI product strategy. So check out our newsletter articles if you want to see the quality of the type of thinking you'll get. One of my frequent collaborators, Pavel Hearn, is the Build Labs leader. So you're going to live build an AI product with Pavel's feedback if you take this AIPM certificate. So be sure to check that out. Be sure to use my code and my link in order to get a special discount. And now back into today's episode. Here's the dirty secret about prototyping. You spend two weeks building a prototype. You validate your assumptions. Engineering loves the direction. Then what happens? You throw the whole thing away. Bolt changes this completely. When you prototype in Bolt, you're not building throwaway mock-up. You're building real front-end code that integrates with your existing design systems.

**Aakash Gupta** (00:32:33)

So when you hand it to engineering, they don't throw it away. They ship on top of what you've built. I use Bolt every single day. I host my LAN PM job cohort on it. And honestly, I'm up till 2 a.m. some days just vibing in the tool, having fun, and building. That's when you know a product is good. When you're using it past midnight, not because you need to, but because you want to. Check out Bolt at bolt.new slash akash. That's B-O-L-T dot N-E-W slash A-A-K-A-S-H. Link in the show notes.

**Frank Lee** (00:33:01)

Basically, there's a lot of people that have to do this, like the aggregation, like an analysis manually. So you can see this is a format that I specifically like, but you can also provide the agent freeform context of I actually don't want to look at like urgent issues and feature requests. I only want to look at praises or I only want to look at references for competitors. So just explain that in natural language and then the agent can kind of figure out its right response for that. This is actually what people are saying about some of the agent products. They want more contact. There's some inaccuracies. Sometimes there's degradation in quality. These are all things that we hear sporadically here or there in different channels. But having it all in one place, having it in a specific report, if I need to change it in a specific format, it's so easy via cloud code.

**Frank Lee** (00:33:43)

Or the next thing I'll demo for you is, OK, can you convert all of these recommendations into specs and place them in the agents folder? So let's see if this one rips correctly.

**Aakash Gupta** (00:33:56)

So this is that fourth workflow. Once we've gotten an insight from our customer feedback themes, let's convert it into actions or specs.

**Frank Lee** (00:34:04)

Yeah. So this is a light example. Typically, I should do this in cursor because I want to use my specific draft PRD template. Yeah. But you can also do this in Cloud Code because in Cloud Code, it's all tied to the same thing, right? I have this whole product repo in my GitHub. So you can navigate there. You can navigate it on Cursor. I typically find that Cloud Code is a little bit more powerful. It takes a bit longer, but the response quality is marginally better in Cursor. But the Cursor, there is some benefit of having a dedicated IDE experience, doing the app references, being able to swap between different models and testing around, seeing my specific file system and making edits directly. So I always get hesitant when people are saying it's one or the other. Like I use both extremely heavily.

**Aakash Gupta** (00:34:45)

Yeah, I pretty much use cursor because I can use their really fast models if I want to. And then I use Claude in cursor, which you can also do.

**Frank Lee** (00:34:53)

Yeah, so you can see I think there's starting to add a few within this folder. But yeah, you basically can create a bunch of specs using one or the other based off the templates that you have. And then like, so once again, I have a few MTBs connected. There's the amplitude one. There's context seven, which is makes it pretty easy for you to fetch docs from other repos to explain what's happening. And then I have our linear connected if I wanted to push tickets. So for like some of these long running tasks that I need to coordinate a lot with the team, I'll push into linear so that people can track it. We're also kind of in a weird era where there's a lot of tickets that I don't even push into linear anymore. Like I might just take this context and just message the engineer directly in Slack.

**Frank Lee** (00:35:31)

just removes one part of the steps or overhead there, so.

**Aakash Gupta** (00:35:35)

And it can even, Slack has an MCP, so you can even do that through here.

**Frank Lee** (00:35:38)

Yeah. So this one takes time. There's like six different things, but basically it's drafting these specs. It's putting them into markdown files. I didn't specify the specific PRD template, but like basically like the first draft of it is being generated based off of this analysis and this context that I pulled in via the feedback.

**Aakash Gupta** (00:35:54)

Can we look at one of those and see like realistically, do you think those are quality? Would you use those? And right now we're using Sonic guys, so it's a little bit faster, but it might be a little bit lower quality, but let's put it to the test. All right, so it's generating these specs. Can we take a look at some of these and see if they really hit our quality bar? Let's do it. And by the way, can you explain that branching GitHub toggle that you're doing in the top left for people who don't know?

**Frank Lee** (00:36:15)

Right here? Yeah. Basically, all of these changes that are happening in CloudCode or in Cursor, they're happening in a local branch on GitHub. So there's a copy of this whole repo that's on my local desktop. When I feel like I'm happy about the set of changes, I can just push it directly into like my the cloud, like my GitHub cloud instance of this repo. The same way you think about a code base, like I kind of just have my own product system that's in GitHub so that I can access it wherever. Because the other thing that this unlocks is if you're on cloud code on mobile, you can refer to your GitHub repo that's in the cloud and then also come up with ideas and kick off like asynchronous tasks as well.

**Aakash Gupta** (00:36:48)

Oh, that's super powerful.

**Frank Lee** (00:36:49)

Yeah, because you're not always going to have access to cursor on your phone or like cloud code and terminal on your phone. For example, like all this stuff about cloud bot, like I'd be hesitant to put that onto my work laptop and try to steer cloud code via like a remote branch. But if I have all of my repo and all my contacts in the cloud, I could just kick off cloud code directly within the cloud app. Nice.

**Aakash Gupta** (00:37:08)

Yeah. What's the command for somebody to set this up the first time? Duplicate my repo into GitHub or something? Just simple like that?

**Frank Lee** (00:37:14)

I had just gone into GitHub and created a new repository there. So when I set this up, I just follow the typical GitHub instructions that they have instructions on how to clone a repo to your local branch. I think you can actually just do it via cursor now. If you wanted to be like, for example, if I were to go on GitHub, first go on GitHub, I have this AMP product repo. So there's like a bunch of different ways that you can clone a repo to your local. But instead of following those instructions, you can either use Cloud Code or cursor and just say, let's say this was a fresh repo. I could say, can you copy this to my local branch and sync this to GitHub? And now since it has web in terminal, local terminal access, it can manage that whole set of instructions that previously you would have, you would have to do by hand, which is pretty tough typically for like a non developer.

**Frank Lee** (00:38:03)

But now like the agent, now that it has local like terminal access, it can, it can kind of do it for you.

**Aakash Gupta** (00:38:07)

Nice. So how are these PRDs looking? You're the actual PM on this. Is this a good PRD?

**Frank Lee** (00:38:13)

These ones are correct. They're too verbose. So I can go back to my problem and say, hey, dramatically cut down the words. Or the narrative of solutions is way too long. Condense this to the bottom one or two paragraphs. Or, hey, these might be too many acceptance criterias. Prioritize to think about the top three. So if I wanted to give this, there's command L. This is too long. can you make this way more concise so this is this total of ipm like how uh how big those instructions are but

**Aakash Gupta** (00:38:43)

and i think we probably could have made it better by using opus and pointing it to your prd template so this wasn't necessarily the first

**Frank Lee** (00:38:49)

way to do it like for the overall system but

**Aakash Gupta** (00:38:51)

Yeah.

**Frank Lee** (00:38:52)

This is kind of the reasons why I like sometimes doing it in cursor because you can also like highlight a specific section. And then if you do command K, you can give like quick feedback directly there. Or if you wanted to do command L, I can like basically the context in the agent is pointed to those specific lines in that file. So within terminal, it's a little bit harder to specify like what exactly like the change should be. But like within directly within the file, I can reference it here. Very

**Aakash Gupta** (00:39:17)

cool. This

**Frank Lee** (00:39:17)

one is like much more concise and more relevant. So yeah,

**Aakash Gupta** (00:39:20)

it goes back and forth. So let's go ahead and say you've iterated. The spec is good enough. I think we said the fifth workflow is either pushing these into linear or doing them yourself. So can you kind of show us both of those?

**Frank Lee** (00:39:29)

I'd be nervous to kick it off. But one example of something we have, we have this channel where we are basically calling out to cursor or cloud code within an open channel about some instructions that we want to push in our code base. I might take this PRD or like the specific acceptance criteria. And I can say like at cursor, like slash the JavaScript repo, make this change to the AI feedback page or make this like prototype this change there. And then you can spin up a background agent there. Or depending on if you have like a cloud code set up on your terminal, like this is like me pointing to our JavaScript repo. So if I wanted to like pull a cloud, I can basically pull a cloud and push a change there. Or lastly, like I had the job script repo as well. Like assuming I'm on like the relevant branch, I would just dump that into here and say like create a branch for that.

**Frank Lee** (00:40:12)

So I don't want to kick it off. Like basically I don't want to hand hold like the actual code being drafted. So that would be one route.

**Aakash Gupta** (00:40:19)

Yep. So basically, guys, that's the end to end workflow. Starts with the deep chart analysis. You've got your automated reporting. You've investigated customer feedback themes. You've converted that into an idea and then you take action. You might even code it or a prototype of it yourself. What is the biggest mistake people make when using MCP?

**Frank Lee** (00:40:35)

I think there's two big ones. One is just kind of the wrong expectation settings for MCP. Sometimes people think that MCPs can do everything. Just the simplest way to think about it is MCPs are easy ways for your AI to interact with external systems. They're not complex ways to do workflows. They're not complex tasks already. There's a bunch of other tools more relevant for that. But just when setting the expectation of just being able to pull in data, is the first step. I think the second problem is sometimes people get excited and they connect a bunch of MCP servers, somehow a lot of tools, some that are just totally irrelevant to a given workflow or that in that repo. And so this comes back to the problem with MCP where if you have a huge amount of MCPs connected, too many tools that are not being used, all of those descriptions about what tools are available, what descriptions they are, what formats are needed, they start being provided as context to the model on a bunch of different queries that might not be relevant.

**Frank Lee** (00:41:24)

And so that might lead to higher latency on a given response or slightly skewed or like inconsistent responses because the agent is thinking about these tools, even though it's not relevant to the task at hand. So just be thoughtful about when you decide to incorporate an MCP tool for stuff that's not as relevant. You can hide or remove those tools typically within purser, cloud code, etc. Like you can remove stuff. And then if you're actively developing yourself, you also need to optimize on what is the right set of tools that you want to make available in your MCP server? What are those things named? And then making sure that there's not ambiguity for the model on which tool to use. And there's like accurate descriptors and accurate like instructions on what formatting is required depending on what you're using it for.

**Aakash Gupta** (00:42:04)

What you just said there, these breaking the fourth wall behind the curtain insights of what it's like to be an MCPM have been one of my favorite parts of this conversation. So I think you're uniquely qualified to answer this question, which is that people say MCP is an unreliable or a bad standard. What do you say to that?

**Frank Lee** (00:42:19)

All right, I came prepared. It's a slide. So I see a bunch of things related to MCP. One, people just have been overhyped about what MCP can do. The second is MCPs waste a lot of context. The third is there's a lot of painful experiences on how people set up or have to deal with authentication when interacting with MCPs. And then lastly, and probably the most important thing, is pretty complicated on how to actually configure an MCP. So those are the four criticisms I see most frequently. And so I think the main response is set the right expectations for yourself on what MCP is used for. It is by far the easiest way to connect external systems with most of the AI clients that you're using. And instead of as a PM, I had to pull forward this huge roadmap of integrations and spend a lot of engineering resources building them out.

**Frank Lee** (00:43:05)

Most AI native tools at this point are exposing a lot of their tools, data and actions via MCP. By far the easiest way to get started. Second piece is MCPs require like some amount of optimization. Like you need to go back and forth on what is the right set of tools you want to make available in your server. You need to optimize the names of them, like data sets or actions you make available. And then whenever you're finding edge cases, it's similar to some of the eval-driven development that you see for agents. Once you find those edge cases, figure out how you can optimize the tool names, the descriptors. And once you come to the right set of tools, those servers and those integrations like work very seamlessly and like kind of power a huge amount of these like complex workflows and i think the last thing is most of these like ai clients quad chat gpt like herser everybody's all converged around like the same standard on mcp now like it's the standard most people have some type of managed connector flow where instead of having to deal with this like manual url setting that is in like the first version of these tools you can just click one button and like those mcps are set up for you assuming you're logged into the right tool that you're trying to connect to office handled.

**Frank Lee** (00:44:07)

So now that it's the native standard and everyone's converging on like the same like standard, it's actually pretty seamless to get started now. And so, and then lastly, there's been a lot of this criticism about like context rot when there's a huge amount of tools within the last month and a half, that's actually dramatically changed depending on the AI clients. There's like pioneers like cursor. They've done some experiments around like dynamic tool calling. So instead of having the tools all called every single time, they actually like use rag to find like the right set of tools to call given a natural language question. So you're not using all of your contexts all the time. Same within Claude, like they've adopted some, some type of similar standard for not using like all of your contexts across these tools. And then that's also one of the reasons why they built skills skills gives you some instruction on here's a specific task.

**Frank Lee** (00:44:53)

Here's the instructions and like the prompts that only gets loaded in context when the model thinks it's relevant to pull that skill. So you can kind of circumvent a lot of these problems with MCP by pairing it with like the right changes on the client side or with a skill to instruct when to use that specific tool.

**Aakash Gupta** (00:45:09)

Yeah, For My Money Skills is one of the most important releases. So we started with it. We're ending with it. Make sure you guys are learning those skills. All right. So we've talked a lot about MCP and Cloud Code. What else is Amplitude cooking up? What are the most powerful agents you guys are building and releasing?

**Frank Lee** (00:45:24)

So we're super excited about February 17th because we're bringing agents across the whole platform. I wanted to give some context about Appitude and its journey. And internally, we actually think about this launch as kind of our Cursor moment. And the reason why this matters is when we think about Cursor, they made coding accessible to so many folks that had never coded before. It was the first foray for a lot of folks on how do you spin up your own GitHub PRs or how do you pull in AI and agents into the coding workflow. And it brought so many people and raised the floor for a bunch of non-technical folks that were never able to code before. But what's interesting on the cursor side is when they think about product development, they're always trying to raise the ceiling of what's possible within software sharing. They made this conscious decision on how do we make the most powerful agent or what are the most powerful features and set of contexts they can provide the model so that people can code in ways that they've never basically been able to do before.

**Frank Lee** (00:46:15)

So with our agents launch, we genuinely think this is our cursor moment. There has historically been problems where folks, they're not super familiar with the data taxonomy or how to navigate the Amplitude UI or what actions or ways that they can improve their product are available on the platform. We've built an agent that's embedded across the whole platform. It has access to every single data point, every single action and improvement that can be taken in Amplitude. And we make it possible for people to navigate the whole product just using chat now and using this agent. So really basically raising the floor of what's possible for them. Yeah. But what's even more powerful is given how powerful these tools are, these actions are, we're actually seeing these 10x analysts, 10x marketers, 10x product managers that can do so much more than they used to, given some of those workflows that I showed you in cloud code.

**Frank Lee** (00:47:02)

And so more people are creating so many new guides and surveys or running a bunch of new experiments or being able to deeply analyze and understand trends that are happening across the data, all without the same amount of manual time. And also, navigating that data in ways that they were never able to do before. So there's these power PMs, these power engineers that have access to way more data that they've ever had previously and can accomplish and orchestrate some of those actions within Amplitude, but also within external places like Cursor, Cloud Code, Figma, et cetera. So just jumping directly into what we're shipping. There's four parts of this launch. One is this embedded Amplitude agent. So we call this a global agent. It lives across the platform. You can pull it in a side panel in chat. You can also just navigate on any single page.

**Frank Lee** (00:47:46)

It has access similarly to cursor of whatever's on the page and all of the underlying tools and data that we have available on the platform. We also have the second part of the launch, which we're calling sub-agents. So these are more of these specialized asynchronous agents. So there's a dashboard agent that auto monitors your dashboards for anomalies, automates your reporting. We have a session replay agent, analyzes hundreds to thousands of your session replays, understands qualitatively what people are doing in your platform, what bugs people are running into, what issues like They're stumbling on what conversion blockers and telling you exactly like what people are doing. And we've built a feedback agent that pulls in all this qualitative data, cuts it in different heuristics and tells you exactly what customers are feeling and saying. And then we have a website optimization agent that scrapes your website and understands ways to optimize your copy, optimize different components on your site, and then recommends you a bunch of different experiments you can run.

**Frank Lee** (00:48:37)

What's underpinning all of this is MCP. Like we have MCPs provided to these internal, like this Amplitude agent, these sub-agents, but we've also made all of these tools available externally. So if you want to spin up your own bespoke workflows in agents, you have access to all of those creation, those read, those edit types of tools across all of the data and actions available in the Amplitude platform. And so we've seen these power users build super complex internal workflows. They're mixing and matching data from one specific digital analytics platform with Tableau data. And then they're auto-piping these insights and anomalies into Cursor, similarly to how I shared you, and building a lot of these bespoke agents using your MCP. And then lastly, we want these agents everywhere in Slack, like everywhere that you work. The first thing that we're releasing like in February, this amplitude embedded agent is available in Slack.

**Frank Lee** (00:49:25)

You can ping it. Like I think about this as like the big short, you know, this is my quant. Like anytime I have a question about what data needs to be pulled, what analysis I want to run, I can just hit amplitude agent directly in Slack. It's going to run for a few minutes and it's going to tell me exactly like that analysis without me doing any of the work. I can link back to exactly what charts it looked at. And it can also change anything within the platform. So if I need to edit a feature flag, if I want to run a different experiment, if I want to watch a survey, like a session replay, you can kick it all off in Slack and then have follow-on conversations with it. Super powerful.

**Aakash Gupta** (00:49:55)

If people want to learn more, contact you. Where can they find you?

**Frank Lee** (00:49:57)

If people want to get started, you should jump to Amplitude.com. If you want to see what's happening within this launch, you can go to Amplitude.com slash AI. And once you're jumping into the product, regardless of what plan you are, you can interact with our agents, you can set them up in Slack. You could connect to all of our data within Cloud, Chai Chibuti, Cursor, Cloud Code using MCP. And then if you want to hit me up directly, I'm frank.lee on Twitter, but you can also hit me on LinkedIn.

<!-- sponsor -->
**Aakash Gupta** (00:50:21)

Frank, thank you so much for this masterclass in using Cloud Code, using analytics and the future of agency analytics. Thank you. All right, guys, so we've walked you through what I think is the future of PMing. We were joking off air. This is vibe PMing. Just like there's vibe engineering, vibe coding, vibe designing, all these different trends. This is vibe PMing. We walked you through five workflows using Cloud Code and MCP connected to your analytics tool. And by the way, if you don't have an analytics tool that is pulling in your Gong data and your Salesforce data and the other data, use those MCPs to pull in that data and your Zendesk data, etc. and inform your insights create specs even potentially code something like he showed you using a cursor or cloud code agent or create the relevant tickets in linear to get your engineering team to do it this is the future way pms are going to be working if you are not in an org that is giving you this access that is allowing you to do this stuff you should be making the request.

<!-- sponsor -->
**Aakash Gupta** (00:51:15)

And if you're a product leader, you should be using this video as an example to get everything through your IT departments because this makes PMs much more effective. When we talk about all PMs becoming AI PMs, this is exactly why. Everybody should be getting cloud code access. Everybody should be getting cursor access. Everybody should be getting GitHub access to the code base. This is what not just teams like Amplitude will be doing, but the Toyotas and the Fords and the UnitedHealth Groups and the Mount Sinai systems. In two or three years, they will be doing that too. And there's going to be a huge advantage if you are one of the teams that adopts this sooner. So if you need more help on this, be sure to check out my newsletter where we're going to have a deep walkthrough of everything he presented today. Check out my other tutorials on MCP, which is with the CTO of Zapier, with Cloud Code, with the Fullstack PM on this channel to learn more, to make sure you're comfortable with it.

<!-- sponsor -->
**Aakash Gupta** (00:52:07)

And send me what you built. Share the insights so that we can continue to create better content for you. And I'll see you in the next episode. I hope you enjoyed that episode. If you could take a moment to double check that you have followed on Apple and Spotify podcasts, subscribed on YouTube, left a rating or review on Apple or Spotify and commented on YouTube, all these things will help the algorithm distribute the show to more and more people. As we distribute the show to more people, we can grow the show, improve the quality of the content and the production to get you better insights to stay ahead in your career. Finally, do check out my bundle at bundle.akushg.com to get access to nine AI products for an entire year for free. This includes Dovetail, Mobbin, Linear, Reforge Build, Descript, and many other amazing tools that will help you as an AI product manager or builder succeed.

<!-- sponsor -->
**Aakash Gupta** (00:52:58)

I'll see you in the next episode. you
