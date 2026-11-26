---
title: "The Ultimate Guide to n8n for PMs, with Pawel Huryn"
subtitle: "Pawel has built more n8n workflows than almost anyone. Here’s everything you need to master it."
date: "2026-01-06"
host: "Aakash Gupta"
guests: ["Pawel Huryn"]
speaker_names: "substack"
substack_url: "https://www.news.aakashg.com/p/pawel-huryn-podcast2"
youtube_url: "https://www.youtube.com/watch?v=Kj3KVV5yghc"
duration: "00:59:01"
word_count: 9457
source: "Substack episode transcript (aired audio)"
sponsors:
  - name: "Vanta"
    url: "http://vanta.com/aakash"
  - name: "Testkube"
    url: "http://testkube.io/"
  - name: "Kameleoon"
    url: "http://www.kameleoon.com/"
  - name: "Pendo"
    url: "http://www.pendo.com/aakash"
---

**Sponsors:** This episode is brought to you by [Vanta](http://vanta.com/aakash), [Testkube](http://testkube.io/), [Kameleoon](http://www.kameleoon.com/) and [Pendo](http://www.pendo.com/aakash).

# The Ultimate Guide to n8n for PMs, with Pawel Huryn

*Pawel has built more n8n workflows than almost anyone. Here’s everything you need to master it.*

**Aakash Gupta** (00:00:00)

In my opinion, N8N is the most powerful workflow automation tool. Pablo Hearn has been knee deep in N8N more than almost anyone else in the world. He has tried everything. He's made all the mistakes. He's learned all the expert workflows and tips and tricks. So in today's episode, he's going to teach you everything you need to know to master N8N. You

**Pawel Huryn** (00:00:19)

can learn a lot of things that matter without coding and without going too much into tech.

**Aakash Gupta** (00:00:24)

What are some of the use cases? Like, I understand the word workflow, I understand the agent, but like, what is this practically going to do for me?

**Pawel Huryn** (00:00:30)

That's all we need. Starting from simple business workflow automations, low fat bots, automatic competitors monitoring, multi-agent research systems, sky's the limit.

**Aakash Gupta** (00:00:40)

What are the other N8N skills people need to know? First best practice is to set up a dedicated workflow.

**Pawel Huryn** (00:00:45)

Another good practice is this max iterations. Another one setting this retray on fail. If we now try to execute this step, it should call perplexity six times for each of the roles and we should get six search results.

**Aakash Gupta** (00:00:59)

Would you need a pro version of N8N and perplexity to do this?

**Pawel Huryn** (00:01:02)

I'm using a free version of N8N.

**Aakash Gupta** (00:01:04)

Holy guacamole. If you get any value out of this podcast, do me a huge favor and follow on Spotify and Apple Podcasts and subscribe on YouTube. It helps the show tremendously. If you become an annual subscriber to my newsletter, you get access to nine incredible AI products for an entire year. This is an over $3,000 value across tools like Mobbin, Linear, Descript, Magic Patterns, Reforge Build, Relay, Deep Sky, Dovetail, and Array. And now, into today's episode. Quick note for my audio listeners, there are some things that we showed, which you can see on Spotify or YouTube, but we've edited this audio so that it's a really good listening experience nonetheless. Pavel, welcome back to the podcast. Hey Akash, it's great to be here. So why should people care about N8N?

**Pawel Huryn** (00:02:03)

In my opinion, NAN is the most powerful workflow automation tool that combines two perspectives. So one is automating traditional workflows, and the second perspective is building

**Aakash Gupta** (00:02:16)

AI

**Pawel Huryn** (00:02:17)

agents and multi-agent systems. And this is by far the most intuitive tool that you can use to automate any workflow, not specific workflows or simplified workflows that might work in some cases and not necessarily in others. NAN can do everything. So that's why it's my favorite framework. And we can, of course, dive into the deals.

**Aakash Gupta** (00:02:36)

What are some of the use cases? Like, I understand the word workflow, I understand the agent, but like, what is this practically going to do for me? What problems is this going to solve? What time is this going to save? What is this going to

**Pawel Huryn** (00:02:45)

automate? That can be automated, can be designed and mapped in NAN. So starting from simple business workflow automations, like we've been implementing for many years, even before AI, to what companies currently implement, like chatbots, automatic competitors monitoring, multi-agent research systems, some workers that monitor your inbox and based on, for example, new email, take actions in your systems. So sky's the limit.

**Aakash Gupta** (00:03:13)

Amazing. Well, can you show us it in action and teach us how to use it well?

**Pawel Huryn** (00:03:17)

Sure. I would like to, instead of starting with the theory, I would like to build a workflow together with you. And let's start from a classical workflow that will use LLM as one of the steps. And we will then increase the agency until we reach the NAIAgent level. Does it sound okay?

**Aakash Gupta** (00:03:36)

Yep, makes sense. Although some people may not know what we're talking about, so you're about to see this in action. Yeah,

**Pawel Huryn** (00:03:41)

let's just get into building. Just to start. Imagine that we have a product, but I actually have a product, which is Accredi, a digital courses and credentials platform, and I would like to monitor my competitors. So every, let's say every week, I would like to get an email summary of everything that happened. New features, marketing events, customer complaints that go viral on Reddit and so on. And to do that, we can use NAN. So the first step would be just to create a new workflow. And yeah, the workflow can start in different ways. We can start it manually, we can schedule it to run based on a schedule, or it can be an event in an external system that triggers something that is called a webhook, which is like an inbox for a web process. But in this case, let's start with a manual trigger. It will be the easiest to test.

**Pawel Huryn** (00:04:32)

And the first step, because I know that I want to monitor competitors, will be getting the list of competitors. Does it make sense? Yeah. Okay. So we need to look for some action that will connect to this Google sheet. And when I type sheets, and what I would like to do is to read the list of competitors so that I can do something with this list. So here it will be get rows in a sheet. I previously configured my credentials, so it means that NAN already knows how to connect to my Google account. And if you don't know how to do it, if you click create a new credentials, it will guide you and all the required steps. There are also docs that you can read and are not complicated. So the document that we are interested in is Accredia Competitors, so let's try to type it.

**Pawel Huryn** (00:05:24)

it found the document and the specific sheet in this document, there is only one sheet, so this will be sheet number one. Okay, no filters. So let's test it before we go further. I will save the workflow just so that we do not lose the progress. And now when we click Execute Workflow, we see the progress step by step. So it started with this initial node, which only means that We started the process and then it connected to Google Sheet. And if we open this node by double-clicking, we can see that it's returned some elements. So we see row numbers and competitor, which is one of the columns. Exactly what we have in this Google Sheet.

**Aakash Gupta** (00:06:02)

I wouldn't say that was the simplest Google Sheet ingestion. And I think that is one thing is that N8N is so powerful that you might have to overcome some initial anxiety with all the dropdowns and things that you see and just realize that I'm using a full functioning tool. I'm using a full powered power user tool. Some of these things might be a little bit scary, but once you overcome that hurdle and you figure out, oh, this is how we get the rows, it becomes really easy. It becomes like second nature.

**Pawel Huryn** (00:06:28)

Yeah, exactly. The next step, once we have this data, show you a trick so we don't have to keep asking when developing our software, developing this process. We don't have to query a Google sheet over and over again. We can just pin this data. And it means that for the development purposes, we can just use this collection and it will not actually connect to Google Sheet. We can continue from here. This will simplify everything. So how can we monitor our competitors? You could try to connect to some service like Brave Search to perform a Google query, perform a search based on some query. But what works best for me in most cases is just using perplexity. So the next step is perplexity, and you don't have to remember all those actions if you just type what you want to achieve. It's just the right node type, and the only possible action here is message a model.

**Pawel Huryn** (00:07:20)

I already have the perplexity account, so all I need to do, and I can leave the default options, is to send a message and tell perplexity what I expect. So in this case, I previously prepared a prompt. Let me explain it. If I click this small icon, we'll just extend this area. I explained perplexity that I'm conducting a market research, and the first thing I wanted to do is to find insights about a specific competitor. So here we have preview of one of the rows, and all you need to do to use this as a variable is to drag and drop this element here. And for every row, every competitor, it will send a separate request to perplexity search.

**Aakash Gupta** (00:08:07)

And I have

**Pawel Huryn** (00:08:08)

also instructed it what to focus on. So new products, capabilities or features, important updates, announcements, changes in pricing, partnerships, user complaints, and so on. And also I have asked to apply specific formatting so that we have a header with the competitor name and then relevant links and relevant information if There are no updates. It should reply with no updates. That's all we need. So if we now try to execute this step, it should call perplexity six times for each of the roles and we should get six search results.

**Aakash Gupta** (00:08:45)

Would you need a pro version of N8NN Perplexity to do this?

**Pawel Huryn** (00:08:48)

For Perplexity, you need an API key, which doesn't require a Perplexity subscription, but requires connecting your credit card. And cost of this call is like you can make hundreds of calls, especially with the model that is selected by default for one, two dollars. So this is symbolic. And I'm using a free version of N8NN. Nice. Okay.

**Aakash Gupta** (00:09:12)

So pretty much it's going to cost you, this workflow is going to cost you like if you're making hundreds of calls, a dollar or two, pretty cheap. Something like that. Something like that.

**Pawel Huryn** (00:09:19)

Yeah. To run it every week, this is, yeah, you can forget about the cost. Nice. Yeah. So what we got for perplexity, we got six responses and for every element, as we see, it generated a lot of text. Like we have citations, we have search results, we have some title of every page that it browsed and I don't need this information. And if we try to send this information to LLM to create a report, we will waste a lot of tokens. So to optimize costs, you would like to select only what matters the most from this response.

**Aakash Gupta** (00:09:55)

And

**Pawel Huryn** (00:09:55)

to do that, you can ask, I usually ask chat GPT how to do it. And there is a special node type that is called code. And you can ask HRGPT how to compress this information because like there is a lot of text and I don't want to send all this text, for example, to OpenAI. And the response will be that you can do it like here. So I would like to select only two elements for every website that it found. For every element, I would like to find the response. The response is, it's even difficult to find. It's this one, content. So this is a summary for a specific competitor,

**Aakash Gupta** (00:10:39)

what it actually

**Pawel Huryn** (00:10:39)

found. And I would like to also find citations, so the websites that allowed it to generate this response. And all those preview snippets are irrelevant. I only want a list of sources, and also I can drag and drop it here. And yeah, that's pretty much it. I never write those code blocks myself. I just take a screenshot and ask chat GPT how to do it well. So it will suggest in this case that you should write this expression and drag and drop selected fields here. And if we execute it, actually, let me pin the perplexity so we do not pay for... We are developing this workflow. We might need to run it multiple times. So there is no point in calling perplexity over and over again. Let's execute this step and see what we get. So now instead of all this information that we do not need, we just have a summary.

**Pawel Huryn** (00:11:34)

So for example, summary for... here for a credible and citations so what pages is grossed and similarly for credential net with citations similarly for certifier and so on and this is when talking about context management I don't want to complicate our conversation but when talking about if we were talking about Context engineering, I'm sorry, this would be compressing the context. So it means that we select only information that matter and we ignore everything else. That's how we can make it much more easy to process for an LLM.

<!-- sponsor -->
**Aakash Gupta** (00:12:10)

Today's episode is brought to you by Amplitude. Replays of mobile user engagement are critical to building better products and experiences. But many session replay tools don't capture the full picture. Some tools take screenshots every second, leading to choppy replays and high storage costs from enormous capture sizes. Others use wireframes, but key moments go missing, creating gaps in your understanding. neither approach gives you a truly mobile experience amplitude does things differently their mobile replays capture the full experience every tap every scroll and every gesture with no lag and no performance hit it's the most accurate way to understand mobile behavior see the full story with amplitude trust isn't just earned it's demanded whether you're a startup founder navigating your first audit or a seasoned professional scaling your grc program Proving your commitment to security has never been more critical or more complex. That's where Vanta comes in.

<!-- sponsor -->
**Aakash Gupta** (00:13:04)

Businesses use Vanta to establish trust by automating compliance needs across over 35 frameworks like SOC 2 and ISO 27001, centralized security workflows, complete questionnaires up to five times faster, and proactively manage vendor risk. Vanta can help you start or scale your security program by connecting you with auditors and experts to conduct your audit and set up your security program quickly. Plus, with automation and AI throughout the platform, Vanta gives you time back so you can focus on building your company. Join over 9,000 global companies like Atlassian, Quora, and Factory who use Vanta to manage risk and prove security in real time. For a limited time, my listeners get $1,000 off Vanta at vanta.com. That's V-A-N-T-A dot com slash A-A-K-A-S-H for $1,000 off.

**Pawel Huryn** (00:13:54)

And you might have noticed, Akash, or maybe we might have people that are more technical. People who are more technical might be used to creating loops. So usually when we get a collection of items, we draw a loop like for or while and then repeat the process and draw an arrow back to iterate over collections. In NAN, you do not need to do that because it automatically repeats the actions for every input item. So that's why I do not have to go back. It is possible, but it's just not needed in this specific scenario. And in most scenarios, you don't need that. But the next thing I would like to do is to send all this data to OpenAI and ask to prepare a report, to prepare an email template that I can send. But we have six objects, and I would like to have this one variable that I can use in my prompt.

**Pawel Huryn** (00:14:45)

To do that, we can use the default action, which is about aggregating responses. We would like to get all the data, all those six responses, and create one field. Instead of six items, we will have one, and we can now give all this information easily to an LLM. Should I repeat it, or do you have any questions?

**Aakash Gupta** (00:15:09)

See it. Let's move on.

**Pawel Huryn** (00:15:11)

Yeah. Okay. We will simplify it in the agentic workflow version. We started with the most basic one, which requires the most manual work. So the next step is to, I have all this information that I downloaded about my competitors, and I would like to give it to an LLM. In this case, it will be ChatGPT to summarize this information and prepare an email template. And for that, I don't need an agent. I only need to message a model, which should be here. Open AI, message a model, and it will send a prompt to an LLM. And in this prompt, let's open it here. I already prepared the prompt, so we will not waste time on it. I have very specific requirements. So you are a perplexity results formatter. Your task is to create a clean competitor monitoring report. I defined how the outputs should be structured, that every competitor, how the report should start.

**Pawel Huryn** (00:16:09)

So this is a header of the report. We should use headings for every competitor. and also how to format references that we shouldn't use. For example, those numbers that people wouldn't really understand what they mean. Instead, we should use a link from citations. Let me demonstrate it. So here I still have links like, you see this, like reference number two, and I would like an LLM to replace it with the right link from citations, so from the

**Aakash Gupta** (00:16:42)

list.

**Pawel Huryn** (00:16:43)

Okay, what else? So this is about how to create references and how to display links. What are the rules for the content, like normalizes phrasing, avoid speculative language, And an example of the report that I would like to get. I have used this example. This is mixing markdown with an XML so that LLM understands that this markdown is not the same as markdown used in the prompt. Mixing those notations works pretty well for me. Okay, and when it came to special expressions, and honestly, I didn't write it myself. I probably wrote the first paragraph and everything else was generated by ChatGPT. So I asked ChatGPT to generate a prompt and then I experimented with it. I probably also added this example, but everything else was generated by... LLM. Okay, and of course we need to provide the context, so it needs to know what the data is.

**Pawel Huryn** (00:17:43)

And for that, we will use one of the expressions that are critical to remember. If we have those structured objects, so objects with some structure, and we would like to convert them into text. So as you see right now, we have a preview, so it will be object, object, object, object. It doesn't make sense and LLM will not understand it. So we need to convert it into text. string and this is the special expression to JSON string and that way an LLM gets the content that it can understand. So

**Aakash Gupta** (00:18:16)

you use json.json to string and you just click into that by starting typing it.

**Pawel Huryn** (00:18:21)

Yeah, to JSON string it's one of the like three expressions that are important to remember.

**Aakash Gupta** (00:18:26)

Otherwise

**Pawel Huryn** (00:18:27)

you will not be able to get this object and send it to an LLM. Okay, and the model that I'm going to use, let's say it will be chat GPT-5. We probably don't need it, could use something simpler, but I want to later to compare it to Agentic Workforce and AI Agent, and that's why let's use the same model everywhere. One of the helpful options when working with LLMs, especially with OpenAI, is reasoning effort. So I know that in this case, I do not need an LLM to think a lot about the answer. Let's try to find it. So reasoning effort is low. Can we

**Aakash Gupta** (00:19:11)

use 5.1? Have they put 5.1 into it yet?

**Pawel Huryn** (00:19:14)

Yeah, they probably have. I saw it today.

**Aakash Gupta** (00:19:17)

I think 5.1 came out like a day or two ago. Yeah. Okay. We have.

**Pawel Huryn** (00:19:20)

Nice. Let's experiment.

**Aakash Gupta** (00:19:22)

So they're updating it pretty quickly because some of these tools I've used, it may take a week or two.

**Pawel Huryn** (00:19:26)

Okay. So, and that's everything we need. So let's try to test it again. Very nice thing about pinning this data is that right now, if I execute the workflow in this test mode, it will not connect to Google Sheets again. It will not send any requests to Perplexity. You can even modify this data by clicking a pencil icon, for example, to change the text. So that's really helpful. And let's try to test it.

**Aakash Gupta** (00:19:57)

So if I looked at this workflow so far and I had seen some of my other videos on like Lindy and Relay, I would say this was a lot more complex than those

**Pawel Huryn** (00:20:05)

tools. Yeah, but you can do much more and I will, in a moment, I will also demonstrate how you can do it

**Aakash Gupta** (00:20:13)

more easily. So wait, guys, it looks complex now, but we're going to show you something.

**Pawel Huryn** (00:20:18)

Yeah, once you start playing with it, it is not that complex, but the version that we are implementing right now is the most efficient. So it saves the most tokens and it will work the most reliable. So there is a very little space to hallucinate because all the LLM does is to create a report based on this data from perplexity. And if we use an agent with multiple tools, It can make a mistake, and it will think longer. Okay, so what we got from GPT-5.1, we have a response with the report that we asked for, with sources. Everything is formatted as a markdown. Okay, but we cannot send a markdown. Well, we can, but it will not look nice. Yeah. So we need to convert it to HTML. And of course, I could ask the model to create an HTML, but again, it will not be efficient.

**Pawel Huryn** (00:21:13)

Because HTML, it will consume much more tokens. So instead, we used a markdown formatting and now we will convert it to HTML. And we can do it by typing markdown. We will select the text, but first let's switch the mode. So this is markdown to HTML. This is markdown. Just drag and drop the text. It will produce an HTML, I hope. And we have it here. Okay. And the last step, if that was clear, let's pin the data again. The last step is sending an email, but not using the default functionality, but I would like to use the Gmail connection. Send an email, send a message. I will send it to myself. I already have connection to my Google account. Weekly competitor report. Email type is HTML. We have this HTML and the message. will be this we can see it in data so drag and drop and maybe instead of previewing it here i will yeah i will run the entire workflow uh so yeah let's do it like this and let's see if you get an email yeah i will check it i am using the second screen but i will present my email Okay, so it looks like this.

**Pawel Huryn** (00:22:29)

Competitor monitoring report, credly, no updates, no updates. Here we have a list of updates for certifier with the sources that should work. Not hallucinated, guys. Yeah, this really works. We have certifier, certify me. So right now...

**Aakash Gupta** (00:22:46)

Wow. So this is pretty powerful, although it took quite a bit of work. So what's the simpler version?

**Pawel Huryn** (00:22:51)

What was complex here? So first we need to understand the steps and of course get competitors from a spreadsheet, ask perplexity. So that was pretty logical. But then this code execution, aggregation, this is specific to NAN and the markdown conversion. This is my optimization. We could ask a model to create a HTML directly. Okay, another version would be to make it more identic and more identic. Let's build it here. I will just move the trigger below. More identity.

**Aakash Gupta** (00:23:26)

You can just have a floating workflow up there and it won't execute because there's no trigger. It

**Pawel Huryn** (00:23:30)

will not

**Aakash Gupta** (00:23:30)

execute.

**Pawel Huryn** (00:23:31)

more urgent question is to use AI agent and you can do it by just by searching AI nodes and there is I would argue that there is one key node type that you can you need to understand which is AI agent I will close it for a moment So what is an agent? Every agent to work needs some LLM. So LLM is a brain for an agent. And in this case, my favorite model for agentic applications is OpenAI. I have done a lot of tests and we can share them later, or maybe I can also demonstrate those results. GPT-5.1, right? So it's the same model here.

**Aakash Gupta** (00:24:10)

Supposedly the best instruction following that OpenAI has done yet.

**Pawel Huryn** (00:24:13)

Yep. And reasoning effort, let's again set a low reasoning effort because this is not very complex. Okay, another thing is memory. We could attach long-term memory or short-term memory if an agent had to understand previous interactions, but here it is not the case. It doesn't need to remember what happened, for example, an hour ago or a month ago, so we can skip that. But what's important is giving this agent some tools so it can pursue the goals, and we will define the objective, and an agent needs to use the tools to achieve that objective. And

**Aakash Gupta** (00:24:56)

the

**Pawel Huryn** (00:24:56)

tools are similar, although we will not use all of them. So the first tool is a tool to get competitors from, again, Google spreadsheet, Google Sheets tool. And if we click those sparkles, we can let an agent decide which document it has to use and which sheet and so on. But because I know that there is only one document that should be selected, I can just pre-select it and similarly I can pre-select the sheet so that we do not have to waste tokens for thinking because there is nothing to think about here. If it needs to get information about competitors, it should use this Google Sheet tool. Okay. Another tool that it will need is perplexity. Does it make sense? So it can perform some search. Yeah. Okay, previously we have defined a complex prompt for perplexity. Here we can skip it entirely and say that our model will decide what to put here.

**Pawel Huryn** (00:26:06)

So the prompt will be, you can think about it as a sub-agent, the prompt for these perplexities will be defined by our AI agent Ace. Okay, what other tools does it need? I will keep those two nodes just so because there is nothing to think about. If an agent creates a report converting Markdown to HTML, it can be done by an LLM, but this is wasting token, wasting cognitive abilities. So for those reasons, in this version, I will once again just use the agent output and convert it to HTML and send the message. And later we will add more agents Okay, but we have not told the agent what we expect it to do. So to do that, let's open an agent, define the system prompt, which is an extremely, extremely important part of the code agent.

**Aakash Gupta** (00:27:00)

Yeah, when it comes to building agents, the system prompt is like the most important

**Pawel Huryn** (00:27:04)

thing. So... And I also prepared the prompt previously, so I will just explain it. So you are a market researcher, your goal is to find competitor insights published within the last 30 days, what to focus on, so the objective for the agent to pursue. And many people, when building agents do it like this, that we define reasoning steps. So step one, instead of doing it in NAN, when we mapped the process, we map it in English. So step one, read competitors stored in a Google Sheet. Then for each competitor, use perplexity to find relevant information. It will have to decide what the prompt should be. Step 3, from the responses, take only citations and content to compress the context. So it creates this temporary artifact and doesn't focus on all the other information that comes from perplexity. And creates a final report, use markdown formatting, and follow other instructions.

**Pawel Huryn** (00:28:04)

So this is the second section, how to resolve. And the last is Report Formatting, and I just copied it from the previous version, and as you know, the previous version, the formatting was generated by ChatGPT, so there is not much to think about here. Formatting, Links Rules, Content Guidance, this is all generated and example. It is all generated by an LLM. I just added this additional section, report formatting, so that it is wrapped in the dedicated section. Okay, and let's try to... and one more thing, this is a good practice. We probably don't need it now, but I would like to demonstrate it already. By default, NAN agents can do no more than iterations. So if thinking, if it has a lot of tools and some of the tool calls might fail, each tool call will be an additional iteration. And if it iterates too much, it will just stop without achieving the objective.

**Pawel Huryn** (00:29:07)

So for that reason, I usually put the number 30 here. So it means that we just keep iterating. And even with a lot of tool calls, it will not stop prematurely. Makes sense. And safe just to make sure that we do not lose the progress and let's execute this workflow.

**Aakash Gupta** (00:29:27)

It's a pretty basic agent workflow with that sub-agent that you mentioned because it's determining its own prompt for that step.

**Pawel Huryn** (00:29:33)

Yeah, that's an agentic element here. Deciding calling the right tools and deciding what the prompt should be.

**Aakash Gupta** (00:29:41)

The other one wasn't agentic because it was all defined, even though it had a system prompt.

**Pawel Huryn** (00:29:46)

This is,

**Aakash Gupta** (00:29:47)

yeah. The other one is what we call a workflow and this is an agentic workflow. I call those, this

**Pawel Huryn** (00:29:51)

is a standard workflow. It, of course, it can have switches, it can check some conditions, it can have loops, but this doesn't really differ much from everything that we have been doing for years when automating different processes. The only difference here is using this LLM node, which is about sending text to LLM and getting a response. And similarly, perplexity. This is like an external service. You don't even have to think about that. There is an LLM inside, but there is an LLM inside. Yeah, for me, this is not authentic at all. This is just a workflow with an LLM. This one is more authentic, although the Agency is pretty limited here. It didn't send the message for some reason, but let's see what the agent did. By the way, we can see it in logs, so here we have a full breakdown of everything that happened.

**Pawel Huryn** (00:30:48)

First, it got our request, then it decided to call Google Sheets, then with those Google Sheets, as we see, it already has information about competitors in the prompt, and then it called perplexity, if we look at the times, time start, starting time and end time, those calls were done in parallel. not sequentially, and we have this final call where it gets all the information at the list of competitors, results for perplexity, this is quite a lot of text, and it generated this report. Okay, what is the difference? The previous execution was about 5 000 tokens and like I tested it before, we can then, we can test it later, but it's like 30, 40 seconds. Here, because it is more agentic, it is one and a half minutes at 12,000 tokens, and we will pay for every token.

**Aakash Gupta** (00:31:49)

Wow. Huge difference in cost. So that little bit extra setup. Yeah. You really reap the results on token cost and time it took.

**Pawel Huryn** (00:31:58)

Yeah.

<!-- sponsor -->
**Aakash Gupta** (00:31:59)

testcube scale testing for the ai era See more at testcube.io slash Akash. That's T-E-S-T-K-U-B-E dot I-O slash A-A-K-A-S-H. Today's episode is brought to you by the experimentation platform Chameleon. Nine out of 10 companies that see themselves as industry leaders and expect to grow this year say experimentation is critical to their business. But most companies still fail at it. Why? Because most experiments require too much developer involvement. Chameleon handles experimentation differently. It enables product and growth teams to create and test prototypes in minutes with prompt based experimentation. You describe what you want, Chameleon builds a variation of your webpage, lets you target a cohort of users, choose KPIs, and runs the experiment for you. Prompt-based experimentation makes what used to take days of developer time turn into minutes. Try prompt-based experimentation on your own web apps. Visit chameleon.com slash prompt to join the waitlist. That's K-A-M-E-L-E-O-O-N dot com slash prompt.

<!-- sponsor -->
**Aakash Gupta** (00:33:30)

Today's podcast is brought to you by Pendo, the leading software experience management platform. McKinsey found that 78% of companies are using Gen AI, but just as many have reported no bottom line improvements. So how do you know if your AI agents are actually working? Are they giving users the wrong answers, creating more work instead of less, improving retention, or hurting it? When your software data and AI data are disconnected, you can't answer these questions. But when you bring all your usage data together in one place, you can see what users do be before, during, and after they use AI. Showing you when agents work, how they help you grow, and when to prioritize on your roadmap. Pendo Agent Analytics is the only solution built to do this for product teams. Start measuring your AI's performance with Agent Analytics at pendo.io slash akash. That's p-e-n-d-o dot i-o slash a-a-k-a-s-h.

**Pawel Huryn** (00:34:20)

And yeah, it failed because I need to fix this field. So instead of using, yeah, probably the field is called differently, maybe like this. Let me pin this data and try it again. Okay. And here, if I run it again, it will send the message.

**Aakash Gupta** (00:34:39)

There we go. It's a live podcast, guys. Sometimes there are errors. It

**Pawel Huryn** (00:34:43)

would

**Aakash Gupta** (00:34:43)

be

**Pawel Huryn** (00:34:43)

suspicious if there were no errors at all. Let me check my inbox. Okay, it didn't send a message. The message was empty, like you see here. So let's take the correct HTML report from the previous node.

**Aakash Gupta** (00:34:59)

You can just drag it like that.

**Pawel Huryn** (00:35:00)

Yeah. And execute it again. It will skip the agent part because we pinned the data.

**Aakash Gupta** (00:35:07)

That pin hack is really a good hack that you guys should be using.

**Pawel Huryn** (00:35:10)

It optimizes costs and time. Okay. So as you see, I just got this email. It's formatted a bit differently. Perhaps my instructions were not precise enough. So I should probably go to ChatGPT or maybe... fix the formatting, fix the prompt manually so that we have the source that is clickable instead of inline links. But this is a problem with the prompt, not the problem with an LLM. Let's leave it like here, like this. Yeah, we would have to compare the prompts between the agent and the model to understand what is the difference. The last version will be the most agentic. I think I can just copy this one and adjust it. So

**Aakash Gupta** (00:35:53)

we're taking our agentic workflow and we're creating a true agent now.

**Pawel Huryn** (00:35:56)

Yeah, and what we have demonstrated so far is how people implement agents in like 90-95% of cases. True agency is not that common. And before Charged GPT-5, I would argue that it wasn't even possible. So now I would like an agent to do everything. Get competitors, call perplexity, send an email.

**Aakash Gupta** (00:36:20)

So you need to give it the send email tool.

**Pawel Huryn** (00:36:22)

Yeah, it needs that tool. I will freeze this. I would like to make sure that I'm using this email, but the subject and the message will be defined by the model. So there is no, nothing is predefined. And another thing that I would like to adjust, because like technically what I presented previously, you can call it an agent. For me, it's a bit like coding in English because, okay, we define the goal, there are reasoning steps, but yeah, it's like lead competitors start in a Google sheet and we fix the sheet so no decision can be made here. For each competitor, use perplexity. The only thing that an agent can do is to define the prompt, but other than that, this is coding in English. Then another step. Take citations, compress the context. So for me, an agent is something that gets the goal, gets a set of tools, and uses those tools to figure out how to achieve the objective.

**Pawel Huryn** (00:37:21)

If we define reasoning steps, of course it will work, but it's difficult to call it an agent for me, even though this is just an LLM call because LLMS also can use tools. The agency is extremely limited here. So a true agent will only get an objective. I have prepared the prompt previously. And let's see the difference. You are a market researcher. Your goal is to find competitors. You can find competitors using the spreadsheet. This was important because it doesn't know this. And use the available tools to send me a well-structured, scannable Gmail summary. I'm not explaining that it should convert those numbers into links, inline links, avoid unnecessary details, place inline links, everything else that is related to formatting, processing the results, an order in which tools should be used. This is up to an agent. So it will do everything. I assume, I hope that it will figure out that it cannot message perplexity if it doesn't know which competitors to ask about.

**Pawel Huryn** (00:38:29)

And similarly, it should send an email message after generating some kind of report. Let's execute it and see how it will work. But yeah, I have pinned the data. It doesn't make sense. So let's try again. The data was pinned because I copied it from another place.

**Aakash Gupta** (00:38:50)

So we would expect this to take a bit longer, just like we saw a time upgrade on the last one. Yeah, but we see the correct

**Pawel Huryn** (00:38:56)

order. So it's read the data from Google Sheets. I was thinking again. Now it's calling perplexity. It should do it several times. If we look into logs, it doesn't do it in parallel. I'm not sure this is a GPT 5.1 limitation or... a wrong choice, I'm sure that GPT-5 can do it in parallel. Maybe if we defined in the tool, we can test it in a moment. Sometimes it's important to provide the right tool descriptions so that the agent understands how the tools should be used and whether this tool can be called in parallel because perplexity, it can have some limitations on how many calls I can make, maybe just in case it did it sequentially. And the last step should be sending an email. And I have not explained how the email should be formatted. I

**Aakash Gupta** (00:39:54)

need to see what it'll look like.

**Pawel Huryn** (00:39:57)

Yeah, every time it will be a little bit different.

**Aakash Gupta** (00:40:00)

Right, we got workflow executed successfully. Moment of truth with the email.

**Pawel Huryn** (00:40:06)

So this is what we generated without my help.

**Aakash Gupta** (00:40:09)

Whoa, this is like the best one yet.

**Pawel Huryn** (00:40:10)

Yeah, it might be one of the

**Aakash Gupta** (00:40:12)

best. Oh, and look at that. So how many tokens and how long did it take?

**Pawel Huryn** (00:40:15)

Previously, it was like one and a half minutes, 12,000 tokens. 12,000, right? This one here, it was 90,000 tokens.

**Aakash Gupta** (00:40:25)

Holy guacamole. So it's eight times more tokens. And how long did it take?

**Pawel Huryn** (00:40:30)

A minute.

**Aakash Gupta** (00:40:30)

A minute 30. Same amount of time, though. Yeah,

**Pawel Huryn** (00:40:32)

a little bit longer. This can fluctuate. But yeah, overall, it will take a bit longer, but not that much.

**Aakash Gupta** (00:40:39)

That's a basic masterclass of the three levels of workflows. What are the other N8N skills people need to know?

**Pawel Huryn** (00:40:46)

There are different skills. So we will discuss best practices later, right?

**Aakash Gupta** (00:40:50)

Let's just go into it. Yeah, we don't have too much time left. We have about 20 minutes left.

**Pawel Huryn** (00:40:54)

So best practices. First best practice is to set up a dedicated workflow that will be activated when there is an error in my workflow. We can do it here by going to the settings and we can select the An error workflow, which is a workflow that will be called whenever there is some problem with the execution. That way you can send, for example, an email or an email notification or a Slack message when there is a bug on production. Another good practice one we already discussed is this max iterations. Another one will be in different tools and in AI agents setting this retray on fail because for example model might be not available for a brief period of time. We can try, for example, three times every second, and this drastically reduces the number of errors that influence the execution. A good practice is providing tool descriptions, and you can do it here.

**Pawel Huryn** (00:41:57)

You cannot do it in MCP, and that's one of the reasons why I prefer built-in connectors over mcp servers is that now I can tell the model this tool can be called in I don't know how to spell it like this so we can provide the tool description and often when you work with mcp servers or built-in connections connectors on different platforms those tool descriptions are inaccurate they lack examples they like correct examples and common mistakes to avoid and I like adding those descriptions every time I see a problem in my workflow. And another thing that we can consider is in some places you cannot click this icon and in that case there is the special expression, probably the second or the third one that we discuss here is from AI. This is just something to remember, and it informs an agent that it should come up with some value for this parameter.

**Pawel Huryn** (00:43:01)

So for example, prompt and prompt for perplexity. This is

**Aakash Gupta** (00:43:09)

not

**Pawel Huryn** (00:43:09)

very creative. It's red, but it would work in real life. I can just trust it. If we execute the game, it will be executed correctly. That's the right way to find it. In some cases, you might need it. In others, if this special icon is available, you can use this icon. A good practice, and you might not like it, Akash, is, of course, this report was the best. I tend to agree, but at the same time, the risk of hallucination, the risk of mistakes here is the highest. This is the most expensive solution, and in weekly competitors it doesn't make much difference, but If that was something that is run, the user is waiting for the response. We want to minimize this time, and the way to minimize this time is to define it like this. If you run some simple automations that you just want to run in the background, Or you can wait.

**Pawel Huryn** (00:44:12)

It's perfectly fine. But if you want a process that will run on production, if you have something that can be expressed as a code, it should be called. And we should leave agents for cognitive work. So if we really don't know how the process will look like, there are different tools. We need to serve a diverse set of questions like... we have a Trello agent and it can create a new list, create a new board, move cards between different lists, complex scenarios, and you cannot predict each possible scenario, then we should choose an agent. If we have one process that we want to run regularly, it's better to convert it into a workflow. As an individual, it doesn't make much difference. If you are running this on production and you have thousands of customers, that's the right way to do it. And yeah, use an agent only when you have to.

**Aakash Gupta** (00:45:04)

The agent seems fancy. We did it last. But actually, you want to do what we started with when you can. You want to simplify both for time and cost spent.

**Pawel Huryn** (00:45:13)

And you need to remember that when we are talking about Allen & Bauer, so people who use agents for their personal use cases will probably not see a difference. But if you have an LLM-powered product and you want to scale this product, you have to remember that this cost will scale proportionally to the number of the users. So especially if you want to have a freemium version, that might be tricky. One more example that I have prepared. And we can conclude or make some summary just to demonstrate what NDN can do. This is not only about simple workflows. I would like to demonstrate a multi-agent research system where...

**Aakash Gupta** (00:45:54)

This is the next level.

**Pawel Huryn** (00:45:55)

Yeah, this is the next level. So I often see infographics where people explain the difference between NAN and other systems and they portray NAN as this linear workforce platform. It is completely not the case. So you can perfectly, and this is an example of NAN used to map multi-agent research system by Anthropic. So this is from the paper that they published, how they implemented it. And there is the slit agent that gets the research topic and distributes tasks between sub-agents, and then each sub-agent performs a scoped research. At the same time, it is aware of the overall context of the research, it creates a report, and finally this lead agent, which is an orchestrator, creates the final response for the user. And I did the same in NAN. How many minutes do we have? 10 minutes. Just briefly. Give me research on Amazon. I'm using a simple interface, and this is an interface provided by NAN.

**Pawel Huryn** (00:46:59)

But you can perfectly combine NAN with Lovable Cloud or any other coding agent by creating something called a webhook. I will not be able to demonstrate it right now. so this first agent that i defined verifies if the question that i asked asked makes sense and it needs more information of course because it was extremely unprecise so here amazon market share 2020 2024 by region by continent and if i submit it So it has a memory. It remembers the previous interactions. So the next step is going to this lead agent, which orchestrates sub-agents. It creates a list of tasks. For example, give me Amazon revenue for Europe or give me Amazon revenue for and then each of those sub-agents will pursue the goals. As you see, we have like 10 sub-agents, each running simultaneously, something like this. Each sub-agent will use a brave search, will fetch website content, will use an additional LLM to compress the context, so there is a basic LLM chain, so we do not use the entire, the full HTML, but extract the most important information.

**Pawel Huryn** (00:48:21)

Each of those sub-agents gets like 3 to 10 websites, and we are not using perplexity, this is done manually. And finally, LitAgent combines all those reports, sends them to a copywriter agent, and the copywriter agent creates a file that is then stored in a Google Drive. So I do not have to wait, it will run in the background. We can see the previous report, for example, this one I created previously. So we have Amazon revenue, executive summary, and different sources that it browsed with tables. We could format it, maybe improve the formatting, but other than that, It does the research. So I also have versions that generated much more complex reports with like 10, 15 pages. It depends on the research topic.

**Aakash Gupta** (00:49:15)

Okay. So we walked people through all these levels of workflows. We have ended at the highest level, the multi-agent workflow. What are the most repetitive tasks that PMs still do manually that they should automate with N8M?

**Pawel Huryn** (00:49:28)

There are many examples. One of the examples is just automating work with the software that they access the most. So, for example, you can use NAN to summarize emails or draft responses to every email that you get. Move emails between folders. Competitor research is one of the examples. I also have agents that write PRDs based on the input that the user provides. And it can search Slack, it can search your files, like good drive, find relevant information. And then based on the prompt and your ideal PRD template, it can create this PRD. For example, as a Google Doc, there are many examples. I personally also use it for my to automate tasks for my products. So for example, I had to get information about exchange rates and import this information to my local database. I use it to import information about new subscribers to Substack and

**Aakash Gupta** (00:50:35)

yeah,

**Pawel Huryn** (00:50:35)

processes like this.

**Aakash Gupta** (00:50:37)

All on the free plan.

**Pawel Huryn** (00:50:38)

All can be done. Yeah, this all can be done on the free plan. There are certain limitations, like for example, the free plan has a limited history. So in theory, you can browse probably like 24 hours, but there is a simple workaround you can use to, to remove this.

**Aakash Gupta** (00:50:59)

Yeah. What hack do you have for this workflow limitation?

**Pawel Huryn** (00:51:02)

And most of this article is without, like, probably the entire article is without the paywall. For sure, the entire introduction is without the paywall, the ultimate guide to NAN. So this and the best practices, we will discuss them. I will remove the paywall because it doesn't make sense to keep the paywall. We actually link it in your video. Okay, webhooks, intermediate steps, error handling, you can read it later, but hacks. Remove the limit of one-day workflow storage retention, and I presented how you can do it in Docker. So basically, you need to, in Hostinger, which is one of the cheapest platforms to host NAN in the cloud, it's like $5 a month, and you get a virtual machine that can, with unlimited executions, that you can running the cloud and it can run 24 7, so it's better than running it on your local machine. All you need to do is to go to this editor and copy and paste this text.

**Pawel Huryn** (00:52:06)

So I demonstrated how to do it. And unless you are selling NAN to others, as long as you use it for your internal purposes, this doesn't break the license agreement. Another thing that is helpful is that in free version you do not have global variables, so you cannot do it, but you have a thing like tables so if we go here there are data tables and we can just create a table that will contain our global variables for example competitors even competitors can be global variable secrets let's say And here I can add columns, so it's like a spreadsheet, but it's stored directly inside NAN, and now every workflow can read it. Maybe another example. Yeah, those are some templates that are available for all the workflows that I have. So we do not have to use a paid version for it. And the last ethical hack for NAN is workflow history, because in NAN, in a free version of NAN, you only have the last version.

**Pawel Huryn** (00:53:14)

You do not have the full version history theoretically. As you see, it's limited to one day. And my workaround for it is to create an NAN workflow that will, let me just present it, that will just export NAN workflows regularly to a Google Drive. So I scheduled this workflow, which is executed

**Aakash Gupta** (00:53:36)

daily. This is such an awesome hack, guys. It's turtles all the way down. It's N8N hacking N8N.

**Pawel Huryn** (00:53:41)

N8N has an API and this API is free to use and it is available in the free version. So every day I get all workflow definitions. We can test it. I don't have to describe it. and next it iterates over those elements and saves those definitions as files, so you can later import them from file here. You just download the specific workflow, import it from this top menu, and that's all you need. And if we go to this folder, name, updated, add, so we can understand which files are the newest ones. We could also organize them into folders like a folder by day, but this is just a demonstration, so those are all my workflows. It was just exported. So now I could take this workflow definition, download this file, upload this to NAN, and we have a full version history for every workflow. Another way to organize it would be to create a folder for every workflow, and then for every day have a workflow history.

**Pawel Huryn** (00:54:42)

So that's pretty much it, and those are the most painful restrictions, and you can easily

**Aakash Gupta** (00:54:48)

We just covered 80% of N8N in 80 minutes. Should every product leader be getting their team a license to N8N?

**Pawel Huryn** (00:54:55)

It depends, because N8N license is like $20 a month, if I remember correctly, for 100 or 1,000 executions. In any case, it's pretty expensive. But you can go to Hostinger. Right now there is a Black Friday sale, but even without sales, frankly, this is like five, six dollars a month for unlimited executions. And if you climb the deal, you just select, sorry, self-hosted NAN. This is here. This is not a Black Friday sale. This is the price that will also be available after the Black Friday is over. So for example, this one, this is a powerful virtual machine with 8 gigabytes of RAM memory. And it will just create an instance. So this is what I see. So I have my own N8N. I can manage it.

**Aakash Gupta** (00:55:48)

How can we use N8N to learn and ramp up on AI PM?

**Pawel Huryn** (00:55:52)

That's a good question. So that's why I, that's one of the reasons I like it. because you can learn a lot of things that matter without coding and without going too much into tech. So you can understand starting from prompting and how to formulate precise instructions for your agents. You can understand context engineering because also I didn't demonstrate that, but you can easily include retrieval or generating embeddings and sending your documents to a vector store like Pinecon, which is also free. You will understand how to compress the context, which I already demonstrated in this multi-agent research or in competitor monitoring, so that you are careful about the amount of information that you provide to an agent. You will learn that the context matters, so sometimes instead of defining precise instructions, it is important to communicate the larger objective and the context in which the work is to be executed and how the success will be measured and Often an agent can figure out specific steps on its own if you describe the context well enough.

**Aakash Gupta** (00:57:03)

Yeah, we saw that

**Pawel Huryn** (00:57:04)

live. You can experiment with Rack, different Rack architectures. You can combine NAN to Lovable or to Cloud Code and the built interface so that you get RackShutboot or RackSystem. Virtually everything that AI PMs needs to do, even evals and guard device, are currently supported by NAN. So yeah, that's covers, maybe not prototyping, but other than that, everything that you need to understand about agents, about prompting, about managing context, about evaluating LLM systems, you will get this feeling and you will develop an AI intuition so you understand what are the practical limitations and what agents are good at and when they sometimes still fail. So that's

**Aakash Gupta** (00:57:51)

a

**Pawel Huryn** (00:57:51)

great platform to experiment and learn.

**Aakash Gupta** (00:57:53)

Well, this has been a masterclass. If you guys want to see more about Pavel teaching N8N and AI PM using N8N, check out our other episode. Pavel, thank you so much. We'll have to have you back again soon.

**Pawel Huryn** (00:58:06)

Thank you, Akash.

<!-- sponsor -->
**Aakash Gupta** (00:58:07)

And be sure to check out his newsletter, ProductCompass.pm. It is one of the best resources you can find on AI and product management. And we'll see you guys in the next one. I hope you enjoyed that episode. If you could take a moment to double check that you have followed on Apple and Spotify podcasts, subscribed on YouTube, left a rating or review on Apple or Spotify and commented on YouTube, all these things will help the algorithm distribute the show to more and more people. As we distribute the show to more people, we can grow the show, improve the quality of the content and the production to get you better insights to stay ahead in your career. Finally, do check out my bundle at bundle.akashg.com to get access to nine AI products for an entire year for free. This includes Dovetail, Mobbin, Linear, Reforge Build, Descript, and many other amazing tools that will help you as an AI product manager or builder succeed.

<!-- sponsor -->
**Aakash Gupta** (00:59:00)

I'll see you in the next episode. you
