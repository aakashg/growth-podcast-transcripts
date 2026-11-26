---
title: "8 months of Claude Code Lessons in 80 minutes, with Carl Vellotti"
subtitle: "Carl is back to show you workflows that will change how you work forever."
date: "2026-01-12"
host: "Aakash Gupta"
guests: ["Carl Vellotti"]
speaker_names: "substack"
substack_url: "https://www.news.aakashg.com/p/carl-vellotti-podcast-2"
youtube_url: "https://www.youtube.com/watch?v=59gy_24KIVE"
duration: "01:20:34"
word_count: 18601
source: "Substack episode transcript (aired audio)"
sponsors:
  - name: "Pendo"
    url: "http://www.pendo.com/aakash"
  - name: "Jira Product Discovery"
    url: "https://www.atlassian.com/software/jira/product-discovery"
  - name: "Miro"
    url: "http://miro.pxf.io/PO4WZX"
---

**Sponsors:** This episode is brought to you by [Pendo](http://www.pendo.com/aakash), [Jira Product Discovery](https://www.atlassian.com/software/jira/product-discovery) and [Miro](http://miro.pxf.io/PO4WZX).

# 8 months of Claude Code Lessons in 80 minutes, with Carl Vellotti

*Carl is back to show you workflows that will change how you work forever.*

**Aakash Gupta** (00:00:00)

I spend all day in cloud code because it can do more and more parts of my workflow. It gets to the point where as a product manager or anyone working with these tools, you never really have to even leave cloud code.

**Aakash Gupta** (00:00:10)

This will really save PMs a lot of time. My first episode with Carl Velotti got 30,000 views. It's been my most popular episode of the last couple months. So we have Carl back for a masterclass in advanced cloud code usage.

**Aakash Gupta** (00:00:22)

Opus 4.5 is basically HCI, where you can give it a task and you can kind of just trust it to like walk away from your computer and it will just keep going. Most of the work, of course, that a product manager does is going to be in the document world. So, you know, Google Drive set that up right away. Notion Confluence. That's the first one I recommend. But

**Aakash Gupta** (00:00:37)

you told me your workflows have totally changed. What have you discovered?

**Aakash Gupta** (00:00:41)

We're going to dive into how you can connect Claude code to MCPs so you can pull in and push out information from everywhere, go through the UI and click all these buttons and like kind of make sure everything's all organized. Whereas now with Claude, it can just literally create all those tickets for you.

**Aakash Gupta** (00:00:53)

Wow.

**Aakash Gupta** (00:00:54)

But when you're really as you kind of start to pay attention, just thinking about the whole system that you're building with Claude rather than just having to do individual tasks. Now let's see the cool thing. Let's see this in Google Drive. So it gave us the link here. And then one thing, whenever it pushes the Google Drive, it pushes the straight markdown. So kind of a pro move here is you can cut it and then paste from markdown and it will be nice.

**Carl Vellotti** (00:01:13)

Whoa.

<!-- sponsor -->
**Aakash Gupta** (00:01:14)

Because I have workflows for all those things already built, I can do it just all straight in one shot in like one morning. So it took our PRD and now created 19 engineering tickets. And it also gave them priority, which would be based on what was in that PRD.

<!-- sponsor -->
**Aakash Gupta** (00:01:27)

Is there anything else people should be exploring when they're thinking about cloud code for PM? Bye. If you get any value out of this podcast, do me a huge favor and follow on Spotify and Apple Podcasts and subscribe on YouTube. It helps the show tremendously. If you become an annual subscriber to my newsletter, you get access to nine incredible AI products for an entire year. This is an over $3,000 value across tools like Mobbin, Linear, Descript, Magic Patterns, Reforge Build, Relay, Deep Sky, Dove Carl, welcome back to the podcast.

<!-- sponsor -->
**Aakash Gupta** (00:02:23)

Hey, I'm super excited to be here. Our last episode was really kind of for me to like a good intro into using cloud code and really figuring out how to use it as a tool in its own right. And ever since then, it's kind of amazing. Even I think it's been about two months since we recorded that last episode. I've continued to use cloud code, continue to explore like more of its more advanced features. And now I basically just live in cloud code all day. I start my day in cloud code, I can do literally almost anything in cloud code. If I can't do it in cloud code, I figure out how to make it possible in cloud code. And they keep adding new features that just allow more and more powerful workflows. And we're at the point now where every time you know, you start something from scratch, you have to figure out how to use cloud code for the first time to do that.

<!-- sponsor -->
**Aakash Gupta** (00:03:04)

But then when you go from there, You build this workflow that the next time you do that task, it's faster. And then you realize a couple other ways you can improve that workflow. And then the next time it's faster. And it's at the point where there's just certain like many things where it would have taken me, you know, maybe a whole week of work because I have workflows for all those things already built. I can do it just all straight in one shot in like one morning. So I'm really excited to show kind of these more advanced features today. We're going to dive into how you can connect cloud code to MCPs so you can pull in and push out information from everywhere. And then we're going to look at some of the newest features. Skills are really exciting. Skills are a way for cloud code to basically automatically know how to do really complicated things without you even having to really prompt it.

<!-- sponsor -->
**Aakash Gupta** (00:03:44)

And then we'll do some like really advanced stuff where we'll show how if you have your PRDs and all your documents in a GitHub repo, how you can have Claude take actions in those repos automatically. So you can be out, you can be at the beach, you can realize, oh, I forgot this requirement. And then you can open up your GitHub app, you can make an issue at Claude. And then by the time you get back to your desk, it will already be done. So really excited. There's so much to explore today. And I think we're going to really do some more really good work today.

<!-- sponsor -->
**Aakash Gupta** (00:04:11)

There's this crazy news about Claude Code, which I'm not even sure exactly how Anthropic is figuring out what of its revenue is Claude Code versus regular Claude. But they have said that Claude Code has reached a $1 billion ARR milestone. If it hit that on December 2nd, it's been out for six months. That makes it pretty much the fastest ever to $1 billion ARR in less than six months. What's led to the continued success of Claude Code in the face of competition? We saw Google release anti-gravity. Obviously, OpenAI has Codex, which we've done an episode on recently. Why has Cloud Code continued to do so well?

<!-- sponsor -->
**Aakash Gupta** (00:04:46)

Yeah, I think what it really comes down to is, you know, you have kind of like the main frontier labs. We have OpenAI, we have Google, and we have Anthropic. And they're all taking their own bets on how to approach using their LLMs. So for OpenAI through ChatGPT, I think you really see kind of like general usage. So for kind of like regular people who aren't like necessarily using it all the time it's a very good like general tool like it's good for search it's good for images it can it can do some amount of coding that's pretty it's very good as well so they're much more general for google you see that they really have taken a lot of big bets on being the absolute king of multimodal so they can ingest i think it's still the only llm that can like watch a video and understand what's in it they have the best image generation now with nano banana pro but they haven't really gone in depth to like the super deep workflows around coding And they're trying with anti-gravity, but they're definitely kind of didn't start there.

<!-- sponsor -->
**Aakash Gupta** (00:05:34)

And that's not where their big bets are. And with Anthropic, they've really kind of focused on how can this be the best tool for coding and for work? And where I think and what I think is so powerful about that is that these are the types of things where I kind of was talking about earlier. I spend all day in cloud code because it can do more and more parts of my workflow. Like I don't need a general tool and I don't really need to be multimodal. I need to be really good at text and code. the tool so i think what they're getting is they're getting maybe fewer users but they are like absolutely just power users and as soon as you start using it it almost becomes addictive to where you just keep doing more and more stuff in it and so i think that's why they're just so successful is because they have a smaller part of the market but it goes so deep and it keeps getting deeper and um We're really at the point where the rest of the industry is just kind of trying to catch up.

<!-- sponsor -->
**Aakash Gupta** (00:06:22)

I think if you look at anti-gravity or you look at Codex, they definitely like most of their features are features that already exist in Cloud Code. And Cloud Code is just way ahead and keep shipping new things. And to see the extent where Anthropic came out with MCPs, they were the first kind of company to come up with a standard for how LLMs can connect to other services. They actually just donated that as part of like a agentic foundation or something where like anybody can use it. So they open sourced it. I think just today, Skills, which was something that we're going to cover today, And Anthropic kind of came up with first as a way for you to really give an LLM like clear tasks that it can complete. Now the rest of the world is adopting that same standard. So they're just way ahead of those advanced workflows to the point where competitors kind of just have to copy them to try to keep up.

<!-- sponsor -->
**Aakash Gupta** (00:07:03)

I can say from my personal usage, after our episode, I had to switch to the Claude 5X plan, $100 a month. I was like, oh my God, someone canceled some other subscriptions that I had to make the budget. And then I started using Claude Code and I hit the 5X limits quickly and I had to go up to the 20X plan. One of the things about Claude Code that makes it unique is it's basically limitless. Like with Claude, when you go tell it to do something, you're like, hey, I wrote. So one of the things I asked you actually was I said, hey, I wrote like 90 newsletter articles this year. I want you to like pull all this down. And I specifically want you to analyze like how my own style has changed over the course of the year. Normal Claude challenged at it. Cloud code?

<!-- sponsor -->
**Aakash Gupta** (00:07:42)

All right, let's do it. Downloading all the things. Even hit a rate limit error on Substack, but eventually downloaded all the articles. I told it to put it in a place. It was able to put them. It was able to analyze them. And so I think you're right. It's this power user functionality, which is insane. And that's what we're going to teach you guys today.

<!-- sponsor -->
**Aakash Gupta** (00:07:59)

Yeah, especially another thing since we last had our last podcast, Opus 4.5 came out, which is what I'll use today for our demo. And a lot of people are saying, you know, I think it's always this term gets thrown around all the time, but people are really starting to feel the AGI. People are saying Opus 4.5 is basically AGI, where you can give it a task and you can kind of just trust it to like walk away from your computer and it will just keep going forward in the task. And if it hits a block, it'll find a way forward. Of course, it's not perfect. And we'll talk about that some today. But it's really impressively powerful now.

<!-- sponsor -->
**Aakash Gupta** (00:08:29)

So what's the difference between people who are using cloud code and not being productive versus people who are actually getting productivity gains out of it? Because sometimes it can just seem like you're watching the AI thing. It's taking a long time. Am I actually doing something the right way and saving myself time?

<!-- sponsor -->
**Aakash Gupta** (00:08:44)

Yeah, I think the big difference between maybe cloud on the browser versus a beginner cloud code user versus an advanced cloud code user is that for an advanced cloud code user, you're really paying attention to what are the workflows that you're doing multiple times. And then how can you define, you know, files so that you can go step by step and really define those workflows so that the next time you do that, that it can run through all of that in like one shot versus I think when you first start using cloud code, it's easy to say, okay, do this. Okay, do this. Okay, do this. But when you're really, as you kind of start to pay attention, you see, oh, this is something I'm doing over and over again. Let me define like rules for that. So that the next time I can just point it at this file and it will know exactly how to approach it.

<!-- sponsor -->
**Aakash Gupta** (00:09:26)

So I think that's really what it is, is just thinking about the whole system that you're building with Claude rather than just having to do individual tasks.

<!-- sponsor -->
**Aakash Gupta** (00:09:32)

All right. Shall we just get started? I'd love to see this in action. Today's episode is brought to you by Amplitude. Replays of mobile user engagement are critical to building better products and experiences. But many session replay tools don't capture the full picture. Some tools take screenshots every second, leading to choppy replays and high storage costs from enormous capture sizes. Others use wireframes, but key moments go missing, creating gaps in your understanding. neither approach gives you a truly mobile experience amplitude does things differently their mobile replays capture the full experience every tap every scroll and every gesture with no lag and no performance hit it's the most accurate way to understand mobile behavior see the full story with amplitude Today's podcast is brought to you by Pendo, the leading software experience management platform. McKinsey found that 78% of companies are using Gen AI, but just as many have reported no bottom line improvements.

<!-- sponsor -->
**Aakash Gupta** (00:10:26)

So how do you know if your AI agents are actually working? Are they giving users the wrong answers, creating more work instead of less, improving retention, or hurting it? When your software data and AI data are disconnected, you can't answer these questions. But when you bring all your usage data together in one place, you can see what users do before, during, and after they use AI. Showing you when agents work, how they help you grow, and when to prioritize on your roadmap. Pendo Agent Analytics is the only solution built to do this for product teams. Start measuring your AI's performance with Agent Analytics at Pendo.io slash Akash. That's P-E-N-D-O dot I-O slash A-A-K-A-S-H. So shall we start with MCP servers?

<!-- sponsor -->
**Aakash Gupta** (00:11:06)

Yeah, let's go ahead and start with MCP. So I'm going to go ahead and share my screen here. And then so one thing to kind of call out is I definitely recommend if you haven't seen the first video, this one will still be good and you'll still see like a lot of good demos. And it's actually good because we're not going to cover too many features that we did in the first video. So in the first video, we've covered things like if you have a markdown file, how you can point cloud to it, agents that can run stuff in parallel. We're going to mostly cover new stuff in this video. Everything that we cover stacks with that first video. It's helpful to have that context, but everything here will make sense even if you haven't done it. The only thing I'll call out is there are lots of different ways you can use cloud code because it's kind of just, you know, it has the files on your computer and there's different ways you can show those.

<!-- sponsor -->
**Aakash Gupta** (00:11:44)

Last time we focused, we were mostly in cursor. I'm going to be in cursor this time. We're not using any cursor specific features. We're just using it kind of like as our IDE. So I'll just call that out. So we're in we're in cursor here. And let's go ahead and get started. And then the other thing, I'm going to start Claude. I pretty much always use Claude with the dangerously skip permissions turned on because I just I don't know, I haven't had any issues with it. So that's one other thing to call out. I'm not going to have to approve any like actions or files or things that it wants to do because I have this turned on. So with that, let's go ahead and fire this up.

<!-- sponsor -->
**Aakash Gupta** (00:12:15)

Also known as YOLO mode.

<!-- sponsor -->
**Aakash Gupta** (00:12:17)

Yeah, YOLO mode. All right, cool. Okay, so let's go ahead and get started. So we're in cursor here and we'll get going. So the first thing that I want to cover today is one question that people have is, okay, we're in Cloud Code and we're on our computer here, but... If I'm, you know, I'm a product manager, I need to write PRDs, I need other people to see those. How do I actually get other people to be able to like see my work? How do I get stuff that's in cloud code out into the world so that someone else can see it? And then if I have like stuff in Notion or have stuff in Google Docs or have stuff in confluence? How do I bring that into cloud code in a way that's not just copying and pasting it? So that's what we'll cover first.

<!-- sponsor -->
**Aakash Gupta** (00:12:55)

And the main answer is we're going to use something called MCPs. So this stands for model context protocol. And it's something that was invented by Anthropic. And it's basically just the standard for how LLMs connect with services. So like many companies now, they have built their own MCP servers that make it so that you can basically just say, hey, here's the MCP I want you to connect to, connect to it, and then it will give you a ton of options kind of with that. So we'll go ahead and we'll start and I'll show you just how to set up an MCP because that's a question that a lot of people have. We'll start with setting one up for linear. Are you familiar with linear, Akash?

<!-- sponsor -->
**Aakash Gupta** (00:13:31)

For sure. Yes. Linear is one of the presenting sponsors of this podcast. So that was an organic mention there.

<!-- sponsor -->
**Aakash Gupta** (00:13:37)

Yeah. Cool. So Linear, if anyone isn't familiar, it is a really sort of very modern. I don't know. I don't know the exactly approved way to say it, but it's basically a modern version of JIRA. It's a way for engineers to manage their tickets. And it's really nice. The thing I'm showing here, you could do a JIRA. I just don't have a personal JIRA account, so I can show you a linear, but all the concepts are the same here. So it's pretty easy. So I'm going to just show you almost like in general. And this is kind of like a mindset that you should have if you're a cloud code user is you should think, OK, I want cloud code to be able to connect to this thing. You can pretty much you can ask cloud code like, hey, does linear have an MCP server? And then it will search for you.

<!-- sponsor -->
**Aakash Gupta** (00:14:15)

Or you can, of course, just do our old school Google search. And linear does have an MCP server. And then on these on these pages, it will usually tell you how you can set it up. And so what I'm going to do here is this is the command. So it's just literally we're just going to copy this and then we're going to run it. And this will add this MCP into our cloud code. So I'm going to go ahead and copy here. And we'll go back to Claude. That was a that was like not a command that you put into Claude itself. You just put that into your terminal itself. So I'm going to go ahead and copy that. And then, okay, so what we see here is it said that it added it. So file modified. So basically, what it's saying is it just added it to the Claude JSON.

<!-- sponsor -->
**Aakash Gupta** (00:14:54)

So that when we go back into Claude, it will have now have access to it. So literally, it was just one command, many companies, they have it set up this easily. So you can do it like this. And then when we come back into Claude, one thing to know is you usually have to restart Claude for it to sort of pick up whatever changes there were to its settings. And now we're going to start Claude again.

**Carl Vellotti** (00:15:12)

And how'd you do that really quickly? What were the keyboard permissions? Oh, yes.

**Aakash Gupta** (00:15:15)

In order to just like, there's two ways to leave Claude or there's a couple of different ways. You can type exit, which will kill it. You can type, that's the main one or the way that you can kind of like cancel any command anytime you're in a terminal is you can do control C. So here it's saying, do it again and then it will kill it. So that's a way that you can always just like totally, if you want to just stop whatever's happening in the terminal, just control C will just immediately kill it. Okay.

**Aakash Gupta** (00:15:38)

I've been like creating new terminal windows. So you're going to save me a little bit.

**Aakash Gupta** (00:15:42)

Yep. OK, so now what we can do is we go to MCP and we see. So normally linear, I actually already had connected before we did this. What I'm going to do is I'm going to go ahead and this or I'm going to have to re-authenticate. And so that does is basically it just pops open a browser where, of course, if you are, you can't just say like, Claude, connect to linear. You're going to there's going to be some sort of authentication process. But here with linear, it's super easy. So I just approve. So now it's approved. We're in my workspace here. And we'll be using this kind of throughout the demo. So authentication successful. So when we go back to cloud code, now we see that we're connected to linear. And so we can do something like create a linear test issue. And so what's cool is now we have our linear, you know, our actual real linear board and you can be connected to your linear steam.

**Aakash Gupta** (00:16:26)

And what's awesome is that it will just now it'll be able to figure out like, OK, great, this MCP already have it. And it knows what MCPs it has. And then it's searching for it and it finds the tool. And now it's going to go ahead and basically create it. What's cool here, and we'll let that happen, we'll come back to it, but I'll start another one while we wait, is when you're looking at your MCPs here, so right now I have Google, I have linear, there's also linear server, which is just because I added it again, but we could delete that one, and then Reddit, which is a demo that we did last time. What's cool is that you can click on any of these, And what's really nice about an MCP is that they basically come with lots of tools that cloud code like will basically automatically understand how to use if you've turned it on.

**Aakash Gupta** (00:17:08)

So we can do here is we can go ahead and we can look at linear. And this is by connecting cloud code to the linear MCP. This is all of the tools that it gets. There's just a ton here. You can get documents. You can get issues. You can create issues. You can get like a list of projects and then you can get the information from those projects. So just right away, just by connecting to this MCP, we have 25 different tools that Linear has built to allow LLMs whenever they connect this MCP to basically tell it how it can work with Linear.

**Aakash Gupta** (00:17:37)

Yep. And this is basically the step one. Like you need to do this with your task management tool, your product analytics tool. What are the other major things PM should be hooking up via MCP here?

**Aakash Gupta** (00:17:46)

I mean, really, like I kind of said earlier, a good mindset is like, OK, I have to do this thing and I want to try to live in cloud code all day. What are their MCPs that already exist for it? So what we're going to look at today is I have a Google Workspace MCP set up. So that's going to be how we pull information out and push it into Google, anything with Google Drive. But it can also do Google Calendar, all that stuff. Slack has a good one. All the sort of like major document systems like Notion and Confluence, they'll have their own MCPs. There's one for Google search analytics. So for some of my websites where I have like SEO going, you can connect it to that. So there's lots of MCPs. And because it's the it's sort of the new standard now, most companies, if they want to an LLM to be able to interact with them, they're going to have their own.

**Aakash Gupta** (00:18:27)

So there's a lot. Those are some of the best ones I just mentioned. But in general, always just try to search to see if there is one that already exists.

**Aakash Gupta** (00:18:34)

So I guess if I were just to guess, right, like as a PM, you need to really care about insight and data from inside your company, like Salesforce, analytics, BI, product analytics, all those things, user insights, right? Like your dovetail, your interpret, whatever, your support desk, like your Zendesk or your intercom. And nowadays, all these products have an MCP. So you should really think about connecting your cloud code to all of those, I think, if you want to get the most out of it.

**Aakash Gupta** (00:19:01)

Yeah, exactly. And one kind of one thing that is worth keeping in mind as you connect your MCP to all these tools is MCPs, they do like automatically take them up some context window of the LLM as you use it. So you could you really could and you probably should have just like, you know, 20 different MCP set up to all the different tools that you use. It's good to kind of try to be smart around like when you have them turned on. So for example, right now, I only have linear and Google workspace turned on. I'm going to leave Reddit turned off because it will take up some of that context window. But if I was going to do something with Reddit, then I would be able to enable it. And one thing that's cool is Cloud Code knows what MCPs it has. So, you know, if I said to do something on Reddit, it wouldn't have access to those tools without this turned on, but it would know that it has Reddit.

**Aakash Gupta** (00:19:43)

So it could say, hey, would you enable that? And then it will have access to those tools.

**Aakash Gupta** (00:19:46)

So what's a quick win a PM could set up in like five minutes?

**Aakash Gupta** (00:19:49)

Yeah, I would say, you know, whatever the document system that you personally use or is using your company, set that up first, because most of the work, of course, that a product manager does is going to be in the document world. So, you know, Google Drive, set that up right away. Notion, Confluence. That's the first one I recommend, because that's just where immediately you're going to be able to do work on your computer and push it out so that people can see it.

**Carl Vellotti** (00:20:09)

Nice.

**Aakash Gupta** (00:20:09)

So one thing that's also worth covering about MCPs, and this is kind of like a natural question, and it's really important kind of throughout this demo, is MCPs are like kind of the new way for an LLM to be able to interact with all these different tools. But there's kind of the more traditional way, and that is with an API. So, for example, one thing that we're going to do later in this demo is we're going to use, like, for example, any time that you, if you want to build an application that you know, has an LLM embedded, like you want it to be able to, you know, ask chat GPT something, then you're going to get an open AI key, and then you're going to call the open AI API, and then that will get a response. So LLMs can also run commands through APIs and get information that way.

**Aakash Gupta** (00:20:48)

The way that I would think about like, when should you use an MCP versus an API? So for an MCP, as we saw, you get all the tools just automatically and LLM like right out of the box, it just knows how to use that MCP. Whereas with an API, you just like, for example, if I said, hey, here's the OpenAI API key, do something with it. It doesn't know what to do. So it needs to have like that context around how to actually use that API. And so today we're going to do some stuff with MCP and we're going to do some stuff with APIs. And you'll see that those are kind of like the two ways that you can connect your LLM to the world. And they're good for like different use cases. I just kind of want to cover that because that's the other main way you can have your LLM sort of get information from the world.

**Aakash Gupta** (00:21:25)

Okay.

**Aakash Gupta** (00:21:25)

So I think we're going to start with like an email summary demo.

**Aakash Gupta** (00:21:28)

Yes. Okay. So what we're going to start here is we're going to start our end-to-end demo. So we're going to work with a fictional company called Taskflow. You can think of it as a to-do app, kind of like Todoist. And we're going to work through a feature for a calendar integration. So you can imagine that we know that people want this. There's been like some customer support tickets. The CEO thinks it would be a cool feature. But we don't have any user research. So we're going to start there. We're going to draft a user research survey. We're going to get some mock data. We're going to have Cloud analyze it. We're going to create the PRD. We're going to create a deck. We'll create some images for that deck. We will write tickets that go straight into linear. We'll be able to create the PRD in a way that it pulls those tickets directly from linear through Cloud Code.

**Aakash Gupta** (00:22:07)

And then it will automatically update that PRD as engineers start that work. So we'll do an end-to-end flow. Just start at the very beginning. And we'll show how from Cloud Code, you can do all of it in here. and just keep the work in here, push it out, and then when you have stuff to pull back in, pull it in as well. So to start, we're just going to go ahead and we'll just start at the very beginning. We'll create a user research survey for a calendar integration based on, basically, we'll give it information around the feature in our feature context document, and then we'll say that we already have a template. So this is some stuff that we basically covered in the first video. Okay, so what it's doing is it's reading through those two, and now it's going to go ahead and it'll create that document, and then it'll save it to Google Docs.

**Aakash Gupta** (00:22:45)

One thing I know I'm going to have to do is I'll tell it to use my email. Sometimes when it uses this MCP, it like forgets who it's for. Once I tell it for the first time, it won't have that problem again. So MCP and please also put the markdown file in here. Okay. So what it's going to do is it's going to read those two files. It will create a markdown file in here that has a survey, but then it will use a Google Docs MCP to actually push that in to Google Drive. So It'll be pretty sweet by the end here because it'll actually have it in Google Docs. And then from there, you can imagine, like, you probably want to share that with your user research team or someone before you actually created the, like, sort of sent it out. So this is step one.

**Aakash Gupta** (00:23:25)

We're just going to start with some user research based on some documents that we have in here.

**Carl Vellotti** (00:23:29)

Makes sense.

**Aakash Gupta** (00:23:29)

Yeah. So we kind of see it running the tool here. And now it's also saving it in here so we can see this survey in here. And then one way you can always nicely view these, you right click and do preview.

**Aakash Gupta** (00:23:41)

Yes, showed this to another podcast guest who loved it.

**Aakash Gupta** (00:23:44)

Yeah, I saw that actually. There's also a shortcut if you do a command shift V and then I'll open it as well. Okay, great. So it's basically, this looks pretty good. It followed our own template here. And then, so this is here, but now let's see the cool thing. Let's see this in Google Drive. So it gave us the link here. And then one thing, whenever it pushes the Google Drive, it pushes the straight markdown. So kind of a pro move here is you can like cut it and then paste from markdown and it will be nice.

**Carl Vellotti** (00:24:09)

whoa yeah

**Aakash Gupta** (00:24:12)

i'll do that again just to like show it so we had a markdown file or everything's in markdown here but i think google docs knows that many more people are working in markdown files than ever before so they've added a feature where you can paste from markdown there's no hockey for it but you just right click and then do paste from markdown and it will take that and it will make it really nice so boom now we have our user research survey So the first time we've kind of seen it, we've actually pushed something out into Google Docs.

**Carl Vellotti** (00:24:38)

Nice.

**Aakash Gupta** (00:24:38)

Okay. So now let's say we send this out and we get responses from it. I have already created a sort of like a response. Like we got some survey responses from this. And then the next step is we're going to have Claude help us analyze that research. So first, I'm just going to go ahead and ask it to pull in the responses from this survey. OK, this is going to use that same MPC again. And I'm asking you not to do any analysis. We just want to pull the information in. One thing worth calling out. So there's sort of a step in between here where you'd actually want to, you know, draft that survey in a way that users could respond to it. So depending on the thing that your company was using, Qualtrics is like a very common user research platform. So then as a PM who's trying to be an AI native PM, what you should think of is, oh, I wonder if Qualtrics has an MPC server.

**Aakash Gupta** (00:25:22)

So let's go ahead and search.

**Aakash Gupta** (00:25:24)

And they must, right? So then you could basically automatically create the survey in MCP once you've gotten the feedback from a UXR team.

**Aakash Gupta** (00:25:31)

Yep, exactly. So there is, in fact, a Qualtrics MPC server. So in this demo, I don't have Qualtrics, but that is kind of the mindset is like, OK, here's the next step. Could I have CloudCo do it? And it turns out for many, many, many things, the answer is almost always yes, which is so awesome. OK, so it's

**Aakash Gupta** (00:25:47)

pulling that in. And if you are a stats tool that hasn't developed an MCP server yet, you might want to ask yourself, why not?

**Aakash Gupta** (00:25:53)

Yeah, it's true. Okay, great. So it pulled that information in. And then this is it's kind of just showing it here. One thing that if you if you ever have like these kind of ugly tables, it's usually just because you need to give it enough room.

**Aakash Gupta** (00:26:04)

Yeah, I face this a lot. They're using a lot of command minus right to go small.

**Aakash Gupta** (00:26:08)

Yeah. So there it is. Obviously, I'll zoom back in. But this is like a very long table. OK, great. So now what we're going to do, and this won't seem that amazing at first, but something cool is going to happen here. So I'm going to say synthesize the user research survey responses and put it into new.md. So notice that I'm not giving it any other instructions. This is kind of vague.

**Aakash Gupta** (00:26:28)

Is it going to put it in Google Docs too?

**Aakash Gupta** (00:26:31)

Even something even kind of cooler is going to happen. OK, so we're waiting. It says it's accomplishing. It's thinking really hard.

**Aakash Gupta** (00:26:37)

And if you guys are wondering why his cloud code is so much faster than yours, he had that bypass permissions, which many of you guys probably don't have on. Oh,

**Aakash Gupta** (00:26:45)

here we go. Okay. Really thinking hard on this request.

**Aakash Gupta** (00:26:49)

Yeah. 35 seconds for 300 tokens.

**Aakash Gupta** (00:26:52)

It's kind of a funny element of working with LLM sometimes. It's like there's a lot of just like really short amount of downtime. Okay. So, okay. It didn't do what I was hoping it would do. Let me, we'll start this again. I think it might be because we already had the chat going.

**Aakash Gupta** (00:27:06)

And why does yours fill for Claude Dangerously Skip Permission so fast?

**Aakash Gupta** (00:27:10)

Oh, yeah. Good question. I just have it, like, basically any time you just click up, it will use whatever you've used last time. And it will just cycle through all the commands. And

**Aakash Gupta** (00:27:21)

that actually works not even in cursor. That just works in any terminal. Yeah.

**Aakash Gupta** (00:27:24)

Yeah, exactly. Cool. Well, let's give it one more try because it would be cool if it gets it correct. OK, so from the original and sometimes if you're working in like multiple cloud sessions, you do just have to jump around a little bit to figure out where the things you want are. OK, so I think let's try this one more time. What we're going to do is so before we had asked it to pull in that information, what we'll do is we will ask it to just put it into a file for us. This will also make it look nicer when we pull it in. Okay, so I'll kind of spoil the lead here. So what I'm hoping happens is Claude has this very cool new feature called skills. And the way that skills work is I have a skill that is already uploaded into this project that is a research synthesizer skill.

**Aakash Gupta** (00:28:11)

And the way that this is supposed to work is you have a name for it, and then you have a description of that skill. And so what this does is that as soon as it uses this skill, then it has like a prebuilt sort of template for how it is supposed to analyze that information.

**Carl Vellotti** (00:28:25)

Yeah.

<!-- sponsor -->
**Aakash Gupta** (00:28:26)

That alone is something that we've kind of seen before. You could say, hey, Claude, analyze this information and use this file that has a template. The cool thing about skills and what I'm hoping that we see next. Okay, so...

<!-- sponsor -->
**Aakash Gupta** (00:28:36)

It's supposed to invoke the skill whenever it's irrelevant, but I found it's not always reliable. So sometimes I'm just prompting, like, use X skill and then do Y.

<!-- sponsor -->
**Aakash Gupta** (00:28:45)

Yeah, well, that'll be our backup. We'll try this one more time and see if it figures it out. But the way it's supposed to work is we have this very clear trigger. Triggers on requests to analyze, synthesize, or find patterns in user research. And then the prompt, oh, it might be, well, okay. So it's putting it into a new markdown. And then one thing you can do it with Claude is you can send it a message and then that'll basically queue it. So as soon as it has completed this, then it will do this. It's really nice if you kind of like know what the output is going to be and you know the next thing you want to do and then you like want to go do something else. You can queue up that message. Seems like Claude in general is being a bit slow today.

<!-- sponsor -->
**Aakash Gupta** (00:29:21)

Maybe lots of people trying to get some work done. on the

<!-- sponsor -->
**Aakash Gupta** (00:29:24)

end this might not be the most uh difficult query so if you're facing that issue and you're saying i need to go faster you can always switch to a sonnet or even a haiku

<!-- sponsor -->
**Aakash Gupta** (00:29:32)

yeah that's true and the way you do that is you type model and then you could switch it to another one but not while it's also going okay so created that now we can see all the responses from that file in Google Drive. And then now I asked it to synthesize. So now it says now synthesize the survey response to the new analysis document. We'll see if it finds a skill. If it doesn't find the skill, that's okay. I think there are some other examples from today where we'll see it use it more.

<!-- sponsor -->
**Aakash Gupta** (00:29:57)

In

<!-- sponsor -->
**Aakash Gupta** (00:29:57)

general, I think it's kind of an improving feature for Claude.

<!-- sponsor -->
**Aakash Gupta** (00:30:01)

Thank you. Thank you. That's A-T-L-A-S-S-I-A-N dot com slash product dash discovery. Jira Product Discovery. Build the right thing. Today's episode is brought to you by Miro. Let me ask you something. How many tools are you juggling just to get a single project across the finish line? One for brainstorming, another for planning, something else for tracking tickets. That's where Miro comes in. It becomes an all-in-one collaboration workspace. Whether you're consolidating user research from several interviews, developing and synthesizing product briefs or a wireframe, or project managing development. Miro brings everyone into the same space. It's fast, intuitive, and fully loaded with features like project templates, two-way Jira Sync, and integration with software like Draw.io and PlantUML. Miro's AI features can be used to synthesize elements in a board to develop a ready-to-review product requirements document in seconds. If you're tired of tab overload and scattered workflows, try Miro.

<!-- sponsor -->
**Aakash Gupta** (00:31:46)

Head to Miro.com and see why over 90 million users choose Miro to guide from idea to outcome. Skills themselves, though, are amazing. And I highly recommend people watching build skills. I built skills for like everything I do. And when it doesn't invoke the skill, I get very angry because the response is much worse.

<!-- sponsor -->
**Aakash Gupta** (00:32:04)

Yeah. What are some of the things you use skills for?

<!-- sponsor -->
**Aakash Gupta** (00:32:07)

So personally, I have just even for this podcast, I have a podcast production guide skill, which is like my lifesaver. Like after I create the production guide with my team, I put it into there and it always comes out much better. I also have a skill for editing. my newsletters, for editing my Twitter posts, editing my LinkedIn posts. Both of those are pretty good. What else do I have skills for? I have a skill for creating the takeaways from a podcast using a transcript. I have a skill for coming up with new newsletter topics. So yeah, so many skills at this point.

<!-- sponsor -->
**Aakash Gupta** (00:32:40)

yeah that's awesome yeah so that's that's like a those are all really good examples where you've probably done those things a million times and now you're like okay i should just invest in letting claude really give get all the power out of that skill of doing this every time i do it

<!-- sponsor -->
**Aakash Gupta** (00:32:52)

it didn't take as long as you might think like usually what i'll do is like let's say i want to do like an editor right i'll give like two or three examples here's version a and version final three times notice like how i edited it how i improved it take that down then you do it and then you can just run vibe checks like two or three times i'll just have it edit two or three posts i'll edit the skill two or three times and it's pretty much good to go after that

<!-- sponsor -->
**Aakash Gupta** (00:33:13)

yeah that's awesome and it's cool because this stacks too like if you had agents you could give the agents access to different skills and then when they're working they'll they'll have those skills okay cool so all right so we have this this synthesis we'll go from here okay so in general the concept of skills is that they're supposed to trigger when you do different things The question might be, okay, so we already had this skill in our kind of dot cloud here. What, where do skills come from? So you can, this one I already had, there's a couple of different places that skills can come from. So one is there are a lot of these, like people share them all the time on Twitter, on LinkedIn, there are like these big GitHub repos with tons of skills. So there are a lot of skills that kind of already exist.

<!-- sponsor -->
**Aakash Gupta** (00:33:50)

So let's say like this, this is a repo that just has tons of skills. And so what you can do is you can just kind of like look at one of these libraries and And you can choose.

<!-- sponsor -->
**Aakash Gupta** (00:33:59)

We want to warn everybody. You guys are very susceptible to prompt injection hacks if you are downloading a skill and running in dangerously skipped permissions. So be really, really careful about that.

<!-- sponsor -->
**Aakash Gupta** (00:34:08)

Good. Yeah, good tip. I should also keep that in mind. I think, yeah, definitely be careful. Maybe it'd be good to even like have Claude almost investigate your skill. Maybe you could build your own skill that's a skill investigator whenever you add a new skill. Literally not a terrible idea. But yeah, that's true. Some people will put stuff into these that can be especially for people like me who are just using them kind of willy nilly who knows what the triggers are and what exactly they do okay but there are just tons of different skills that people are building all the time so here we see an artifact builder an ios simulator an mcp builder there was one in here that i thought looked good we'll have i think it's a document oh internal comms so that's something that like you know as a product manager you might want this so we're going to go ahead we're just going to literally copy and paste this github link and we'll say to a new session of claude put and clear this

**Carl Vellotti** (00:34:53)

Nice.

**Aakash Gupta** (00:34:54)

And you guys can also find them from places you trust. Like in my newsletter, I have a PRD writer, a feature results writer, resume customizer. You can find all of those and there's no prompt injection tech there.

**Aakash Gupta** (00:35:05)

Yes, good, good point. Okay, so here it's going to go ahead and it'll just like fetch this and then it'll add it to the skills. So we'll come back to that. Another thing that you can do, and this is really cool. So basically Anthropic has built what are called skills marketplaces. And this is going to use a new advanced cloud code feature that we haven't looked at before called plugins. Okay, so this is saying discover plugins. And so what this is, is this is a bunch of sort of like packs of skills that companies have like built. So context seven, for example, is one where it gets you the most updated information on whatever like APIs or whatever you're using in your project. Most LLMs they have like when they're trained, they have past data. So context seven is one where it will always pull the most up-to-date information.

**Aakash Gupta** (00:35:47)

And so there's, there's a lot of these like prebuilt plugins. There's one for super base, super base for your backend, Figma. There's a lot of these. So what we're going to do is we're going to, there's a linear one. So these just give you like a bunch of different skills and, and MCP configurations and things like that kind of right off the bat. There's one that's really good that is built by Anthropic themselves. And so this one, it's just called, so we're going to slash plugin install, and then it's just document skills. So these are just a bunch that Anthropic has built themselves to allow Claude to do things like create PowerPoints and create Word documents. So, oh, it's already installed. So we're going to go ahead and look at our plugins. We're going to, up here, you see it says installed. We're just going to go click tab.

**Aakash Gupta** (00:36:24)

And then we have document skills already installed. And what you can do is you can kind of like look at all the stuff that comes with this one. So this is a collection of document processing, including Excel, Word, PowerPoint, and PDF. And then it comes with a bunch of sort of components, algorithmic art, brand guidelines, canvas design. The ones that are interesting for us, there's internal comms, there's a skill creator. So if you want to build your own skill, which we'll look at next, it kind of comes for free in this one. So if nothing else, I definitely recommend at least getting their Anthropics official skills, because these are things that as Claude works, it will be able to automatically create these like pretty nice things for you. especially the skill creator for anything else that you want to build.

**Aakash Gupta** (00:36:59)

I think I need that one because sometimes I create the skill and then it'll be like YAML front matter error and it will have added in like some extraneous field. So this is a good one.

**Aakash Gupta** (00:37:08)

Yeah, that's a good one. And then so let's go ahead and do it. So I talked earlier about how APIs are the main other way that you can have your LLM kind of interact with the world. And so what I'm going to go ahead and add to this file is... So an example of where you might want to use an API where there might not be an MCP, for example, is Google's Nano Banana Pro. So we're going to get the API for Gemini so that we can generate images inside of cloud code. So that's something that you might think you have to go to their tool, but because they have an API, we can do it in cloud code right in our terminal here. So the main things that you need to do that is we're going to go ahead and create. Oh, I think I already have one.

**Aakash Gupta** (00:37:44)

But we have our Gemini API key in here already. And so the thing with using an API is that you have to have a script that can run to hit that API.

**Aakash Gupta** (00:37:54)

And just so people know really quickly, he just created a .env file. That's where you put in your API keys. And that's how you keep them safe. If you're wondering, like if I'm ever vibe coding or something, you want to create these files.

**Aakash Gupta** (00:38:06)

If you have a .env file. So there's this other thing called a gitignore, which will pretty much come automatically with like repos that you create. This will have things that when you are committing to this, to GitHub, when you want to save your information, these things will not get sent. And so one of those is your dot end file. So that means that like if someone else, you know, you want to open source your code, you definitely do not want your keys in there because then someone else could use them. But in your get ignore, it'll automatically have that so that you're not committing that. But that's one good thing to check. LLMs are also pretty good about knowing not to commit that. But in this case, I have this with our Gemini API. So we're just going to say use just as a quick demo here, this script that already exists.

**Aakash Gupta** (00:38:45)

So use what should we make an image of

**Aakash Gupta** (00:38:48)

yeah i was gonna ask you like why is it better to you do it in cloud code i guess cloud code could like write a better prompt for you or something so maybe something that requires prompting like maybe we're trying to create an infographic that doesn't look like the normal nano banana infographic style but instead looks like something more professional and clean and maybe a different size

**Aakash Gupta** (00:39:08)

Yeah. So let's create a nice infographic professional for how to use Claude code skills.

**Carl Vellotti** (00:39:15)

OK,

**Aakash Gupta** (00:39:16)

so this is kind of nice because like in this case, Claude, of course, knows how Claude code skills work. So it'll be able to prompt the AI to with a lot of that information. The nice thing about doing this in Claude code is that, for example, if you have You know, let's say that you really want your images to always have a specific type of style or you want them to have certain colors or things like that. Then what you could do is you could save that as a file and then you could say, Claude, please create an image and then make sure that you use these brand guidelines. And then you could automatically have those brand guidelines here. Otherwise, like if you're in Gemini, then you have to like copy and paste those every time and you can kind of like see what works and then save it.

**Aakash Gupta** (00:39:52)

So the nice thing about doing it in cloud code is that it can like make a lot of those like sort of workflows or things like that. It can write the prompt for you and they can do it in here. It can also do other cool stuff. Like if you wanted to generate like four variations of an image at once, then cloud could literally hit the API four times in parallel for you, which is something that would be pretty hard to do on your own. So it just kind of unlocks like much more advanced capabilities for how you can use this once it's in code versus using like the sort of typical front ends.

**Aakash Gupta** (00:40:21)

Yeah. And in your experience, like prompting Nano Banana Pro, some people have been talking about JSON prompting and different things like that. So could it be useful to create like a Nano Banana prompting skill as well?

**Aakash Gupta** (00:40:32)

Yeah, definitely. That's a great example of like, help me turn this like natural language prompt into a JSON prompt. And then you can have a skill that would automatically kind of understand what you're going for with that. That's a really good example. Okay, so here's what it created. Okay, so created a cloud code skills infographic. Honestly, looks pretty good. Besides the

**Aakash Gupta** (00:40:51)

purple gradient.

**Aakash Gupta** (00:40:52)

Which is another thing. Yeah. The purple, the classic purple gradient, the LLM is just for some reason love so much.

**Carl Vellotti** (00:40:58)

Yeah.

**Aakash Gupta** (00:40:58)

Okay. So now let's go ahead and say, create a skill for image generation or product managers or user journeys or

**Aakash Gupta** (00:41:08)

OK, user journeys. Yep. PMs need to create those.

**Aakash Gupta** (00:41:12)

OK, so now what we'll see is that for this first one, we kind of had to tell it where that script was. But now what it's going to do is it will create its own skill so that next time we ask for it to create an image, it will know that it has that skill. And then this script that we had in there is part of that skill. So one thing that we've seen is like so far, all we've seen is like sort of just text instructions. But the other cool thing about these instructions that they can like point to other parts of your sort of whole system so that it knows like where to pull that information from.

**Carl Vellotti** (00:41:42)

And what script are we referring to again?

**Aakash Gupta** (00:41:44)

This is just the image generation script. So I'll open that here. So this is basically just like, how do we actually use that Gemini API? So it tells it like, okay, this is the model we want to use. Here's like the default aspect ratio. And it sort of just defines exactly how you can use that API to actually generate images. Makes sense. Of course, I had Cloud Code write this. So this is sort of, it's actually a pretty big script. So this is something that, this is an example of where using an API requires you to have like these scripts and the AI has to already kind of know what the API is capable of. Whereas with an MCP, you get like all of the tools that it has basically for free. Okay, and then now it's going to test that for us, which is the nice thing about Opus is it's very smart around, it does work and then it checks its own work, which is something that LLMs used to be so bad at, but they're getting so much better at.

**Aakash Gupta** (00:42:31)

So if somebody wanted to recreate that script really quick, how do they do that?

**Aakash Gupta** (00:42:34)

Yeah. So the easiest way would be to basically get the Gemini nano banana like reference documents.

**Aakash Gupta** (00:42:43)

Yeah, the API docs and then ask Cloud Code, create a Python file to pull to make get requests to the API or.

**Aakash Gupta** (00:42:53)

Yeah, exactly. So basically what I would do is I would just say, OK, here's the API docs for this. And then I would say, create a script for us to create images with the Gemini API. Here's the reference docs and then we'll read those and then it will create the script.

**Carl Vellotti** (00:43:06)

nice

**Aakash Gupta** (00:43:06)

yeah okay cool so that's that's kind of like a good coverage of skills so we've seen you can get skills from github you can get that from or like newsletters like akash's which definitely won't have any prompt injection you can get them through the plugins marketplaces which give you kind of a ton for free by just doing slash plugin or you can build your own and kind of like a combination of all of those is what you're going to do like as you build out your system you'll include more and more of these skills and skills are just they're awesome because they are they automatically trigger and what's cool is like if you give it a long running task when it gets to the points where it could use a skill it will automatically use that skill and it will do it sort of in a very specific way rather than sort of just whatever the natural way that it would do it which if you want to build these reusable workflows and the especially for long running tasks keeping the llm on a narrower sort of Don't let it go whichever direction it wants, because as soon as it starts to drift, it'll drift more and more.

**Aakash Gupta** (00:43:59)

Skills really help it keep on that same path so that it can keep the output really high, like the high quality all the way through. OK, cool. So now we have this new skill called PM Diagrams, which we'll go ahead and use a little bit later. Okay, so that was kind of like a big tangential exploration into skills. For now, let's kind of go ahead and continue with our demo of we're building this calendar integration feature. We got those survey results. We had them analyzed. So now let's go ahead and create a PRD based on those survey results.

**Aakash Gupta** (00:44:27)

Makes sense. So. Step one, you send out your survey for feedback to Google Docs. You can even set it up Gmail. You could have it send an email all via cloud code. Step two, you had it create that survey in Qualtrics using Qualtrics MPCP, again, in cloud code. Step three, you have it analyze the results. And now step four, create a PRD.

**Aakash Gupta** (00:44:46)

Yep. And then probably in this case, I don't have one, but it would make sense to potentially have a PRD writing skill, which would have your template in it. It just makes it like kind of nicer to use also. So you're not having to remember like, oh, yeah, what was the name of this markdown file that I had with the template, it will just automatically use that template. Okay, so it's reading the survey results. And then it will go ahead and write our PRD based on kind of all the information we've given it.

**Aakash Gupta** (00:45:08)

Yeah. How many times do you just go look for that latest PRD template or that latest example about this is a good PRD. I want it to look like if you put it into a skill, you can really stop that search.

**Aakash Gupta** (00:45:18)

Yeah, especially, you know, as you live in cloud code more and more and you build out more of your system, it's helpful to have more stuff happen automatically so that you don't have to remember exactly how every single thing works. OK, so I asked it to create a markdown file here and then also push that to Google Docs. So once that's done, we'll take a look at it. Cool. Okay, so we now have our calendar integration PRD.

**Carl Vellotti** (00:45:38)

It's the moment of truth. Is it any good?

**Aakash Gupta** (00:45:41)

Yes, let's see. We'll look at it in Google Docs when it pushes it out. Okay, so it found the MCP. Oh, it needs my Google email. One thing I should do that would make this faster. So as a reminder, right now, it keeps every new session, it keeps forgetting like what my email is, which it needs for the MCP. The way that you can have Claude just always know information is you create a Claude file. So what I really should do is I should create a Claude.md that says like whenever a user uses Google MCP, use their email, which is my email, call Velotti. Okay, so now we'll go ahead and do that. And then I think before that happens, we can also just look at the PRD here. OK, great. So now we see that it's actually creating it and that it was successful. So to give us the link in a second, I didn't really give it much of a template, but it is including the user research here, which is helpful.

**Aakash Gupta** (00:46:30)

And then it is also writing out the requirements. So OK, so now we have our PRD for this feature and then we have the Google Docs. So let's look at that.

**Aakash Gupta** (00:46:37)

So that's Opus 4.5 with no instructions. So much better than GPT-4. That's the last time you've done it, guys. Even just without anything, it's pretty good these days.

**Aakash Gupta** (00:46:47)

Yeah, 100%. And it's pretty nice. I mean, I'd have to read this more carefully, and I'm sure whatever company you work at and things. But if you give it a lot of context, then these things can be actually pretty good on their first pass. And so it's really showing that user research in here, which, you know, a lot of times you present to people. It's like, well, how do we know this is a problem? We've already gotten ahead of that with our user research. And we know now, like, what are the most important things for this? Okay, great. So now, like, the next step would be we have our PRD, but, you know, this is pretty tech savvy. So let's say that we wanted to create kind of a user journey flow for this document. Well, luckily, we already created a skill for that. So let's say...

**Aakash Gupta** (00:47:22)

OK, here's one more truth. Let's see if it remembers to use the skill. So I'm going to say add a user journey map showing the calendar integration flow. OK, so we'll see if this works and it'll be awesome. It should know that we created. Oh, well, let me try one thing. We're going to close this one thing. It might be that we hadn't restarted Claude. I'm not sure if you need to for it to pick up skills. So what we're going to do is we're going to, we're just going to restart Claude. A really good way to do that is you just close Claude and then you just type resume and then you can go back to that same conversation. So that's a nice way where if you need to restart Claude, but you don't want to like completely lose the conversation, you can just type leave, hit resume, and then that will bring you back into it.

**Aakash Gupta** (00:48:00)

That's actually one thing that I dislike about Cloud Code greatly versus Cloud is like discoverability of my prior chats. Is there any way to go back to like go see something like just today? I picked up a chat from two weeks ago.

**Aakash Gupta** (00:48:13)

Yeah. I mean, sometimes you want to do that. I think the only thing that you can do that's helpful with that. Okay. So it knows how to use it because of this, but it didn't use the skill again. So I think this is something, unfortunately for this demo, we're not seeing use those skills, but it is still like using the tools that we've given it.

**Carl Vellotti** (00:48:28)

Yeah.

**Aakash Gupta** (00:48:28)

So just I would say, folks, if you want to use the skills for now, just specifying your prompt to use the skill. That's what I had to do.

**Aakash Gupta** (00:48:35)

Yeah, I think that's that's good advice. I'm sure that that trigger will get better with some future version of Cloud, but not working well. But the concept is still the same here. To your point around, like, you know, having specific sessions that you want to find. One thing I just discovered that's kind of cool is you can you can actually name your sessions. Oh, so you can do rename. And then let's say that this is like we'll just call it test name. But what's cool is then when you type resume, you actually see instead of just showing you like whatever the first prompt from that conversation was, you'll have it here. And then what's cool is you can actually search. So now I can find that session in here. So that's one thing you kind of have to like it'd be nice to auto name them, which is kind of a surprising feature.

**Aakash Gupta** (00:49:12)

And I bet there's a chance that by the time people watch this video will be a feature. But for now, you can name sessions and then you can search for them and get back to them. So and it has basically every session you've ever done, which is pretty cool.

**Aakash Gupta** (00:49:22)

And when we're on the topic of things that is deficient compared to the UI, there's still no way to like select text from earlier in your prompt, right? Like if I just type something, I only know how to like go backspace. Oh,

**Aakash Gupta** (00:49:33)

yeah, yeah, yeah. It's very annoying. Like, for example, like I can't edit this.

**Aakash Gupta** (00:49:38)

Yeah.

**Aakash Gupta** (00:49:38)

It only goes. Yeah, that is definitely a deficiency of being in the terminal for sure.

**Aakash Gupta** (00:49:43)

Okay, so that's still a deficiency.

**Aakash Gupta** (00:49:44)

Yeah. Okay, cool. So we now have this user journey. Honestly, it looks pretty good. And then what you could do is you could take this and you could put it straight into your document.

**Aakash Gupta** (00:49:53)

If you guys become this AI Native PM, that thing is going to be one of the most annoying things. Yeah.

**Aakash Gupta** (00:50:00)

uh there's the only thing that helps is like you can if you like just getting really comfortable with like if you hold option it jumps words if you hold can command it like jumps entire lines that can make it a bit faster and then you can go up and down but yeah it's just just an annoying thing about being in the terminal

**Aakash Gupta** (00:50:15)

option is a pretty big hack actually right because then you can edit there

**Aakash Gupta** (00:50:19)

Yeah, you can do this. And then it also lets you like delete whole words at once. Yeah. OK, cool. So now where we're at is we have our PRD and we've also generated an image for it and things are looking pretty good. So let's go ahead and continue now. Let's say that we have presented or now we need to kind of get ready to actually present this to stakeholders. What we'll do is we'll go ahead and create a slide. And so what we're going to do now based on our learnings is instead of kind of counting on it to pick up its own presentation making skill, we'll actually tell it like check for your presentation skill and use that.

**Carl Vellotti** (00:50:49)

Yeah.

**Aakash Gupta** (00:50:50)

Oh, OK. So one other thing I wanted to cover before we do this, and this will just be a really quick example. So one of the other cool new advanced cloud code features is hooks. Have you done anything with hooks? Have you played around with them at all?

**Carl Vellotti** (00:51:03)

no

**Aakash Gupta** (00:51:04)

okay so the concept of a hook is that every time you have claude do something there's kind of like a bunch of different steps within that entire like life cycle so there's as soon as you do the prompt there's when the prompt ends i'll kind of look at like all the different possible triggers for a hook but the cool thing about a hook is that you can like set automatic actions for claude to take when you're set some point in that life cycle of when you give it a request so here we're just going to do a really basic example what we'll do and this one's actually very fun is um we're going to create a hook that gives us a notification and a sound as soon as it finishes in action so what that's useful is like i'm going to have it create a presentation next and presentations take quite a long time to make and uh let's say i don't want to just like sit there or even within this demo i think if you're following along there's a couple times that i was like oh we'll come back to that terminal and then i actually forgot And that's because there's no notification, right?

**Aakash Gupta** (00:51:56)

There's no way to tell. So we're going to actually create a hook that gives us a notification. And it's really easy to do. All we're going to do is we're just going to say, create a hook that makes a Mac notification. And we'll say sound as well when you finish a task. And Claude kind of knows how to create its own hooks. Actually, it's or it's going to be smart and it's going to look up when it doesn't know how to make a hook. So it's looking it up. What's cool is I think because we have the plugin for those, the Anthropic plugin, it like fetched from its own its own documentation without actually having to do a search, which is kind of like another cool thing that it's just very smart around knowing where to look for this stuff.

**Carl Vellotti** (00:52:32)

Mm hmm.

**Aakash Gupta** (00:52:33)

Okay, so it's seeing if there's a settings file. So while this is happening, what I'll do is I'll go ahead and I have kind of made this little graphic around all the different places that you can have a hook. Okay, so within Cloud Code hooks, there's like a bunch of different ones. And I'll cover like a couple examples where you might want to use this. Like as Cloud works, it does like a ton of stuff. So there's like when you start a session, you could have a hook that says, hey, as soon as you start a session, pull in all linear tickets for this project. And that might be helpful if you have like a specific repo that is just around, man, managing tickets or like a subfolder, then as soon as you start, it pulls in those tickets or as soon as the session is over or right before it uses a tool or right after it uses a tool, you might want to have like another agent or if it's like a specific tool around writing a document, you might have a another agent that triggers as a hook right after it does that so that it can review that work.

**Aakash Gupta** (00:53:21)

Or let's say you have like a long run coding task, then you might have something where every time it finishes writing some code, it also runs the test suite against that code. So these are very advanced. And like, I don't think they're, they're definitely kind of mostly more for coding use cases. But if you're creative, then there's like sort of some really interesting things that you can do with hooks. Another good one is like, so as if when you use cloud code for a long time, eventually it will compact and you'll kind of like lose all the session history before. And it's, it can be kind of actually hard to get back to unless you are like, Claude will literally clear it from the UI. So one thing that you could do is you could say every time before you're going to compact the conversation, I want you to automatically export it and put it into a folder as a markdown file so that if it messes something up after it compacts, you can still get back to that conversation history before it did the compaction.

**Carl Vellotti** (00:54:07)

very interesting

**Aakash Gupta** (00:54:08)

yeah so these are definitely more this is like real advanced and i haven't used these too much but it's kind of like a good feature to know and i think that there'll be some like really interesting setups with these hooks if you're like really trying to create like a very tightly controlled cloud code session Okay, cool. So let's test this. Now, anytime it finishes a task, which is really like anytime it finishes any sort of like message, it should make a notification. So let's see if it works. Oh my gosh, man, Claude is not helping me today. Sometimes live demos. I tested this before and it worked and then now, now not. That's the fun. Yeah, that's the fun. Okay, let me, let's, we're going to resume that session. We're going to do some live debugging here. So let's resume that previous session. And it says, it's saying that it already created.

**Aakash Gupta** (00:54:49)

So let's tell it to delete that. Okay. So while that's happening, we're going to do some classic Claude stuff. We're going to go back to our other PRD that we had written, which is here. So we can just give it the name of this. So please create a presentation. So this is going to use the presentation skill using your presentation skill. for PRD in Google. And then we know, use my email. OK, so one thing, as you use Claude, you kind of want to get very comfortable just jumping between sessions as it works, because there is always a little bit of downtime between them. So it's going to pull in that PRD. Actually, it says it found it locally, but it also found it through MCP. And then it will create a presentation. So we'll come back to this. And then let's see what's happening with our hooks.

**Aakash Gupta** (00:55:36)

The hook file is deleted. So now we'll ask it to recreate.

**Aakash Gupta** (00:55:39)

Yeah. OK, so I'll restart Claude, see if this helps.

**Aakash Gupta** (00:55:42)

So that what you're doing quickly is you're just doing control C up. Yes.

**Aakash Gupta** (00:55:47)

Okay, so now we're going to give Claude another chance here. We'll see. It's going to look it up again, and then it will create it. And then let's see if this other one. Okay, so, okay, perfect. So this time it looks like it is figuring it out. So it knows that as, oh, there we go. So it actually did use this skill. So this is the first time in this demo we've seen it sort of show a skill correctly. And so I think your tip of saying to just use this skill is probably the best way to use it for now. And so it'll look like this. It's just looking to slash document skills PowerPoint. And now I have pretty good confidence that we'll actually do it correctly because we know it's actually like in that skill and reading the instructions. And so now it's creating the slides using its own thing.

**Aakash Gupta** (00:56:22)

And it starts that as an HTML and then it converts it into a PowerPoint. OK, and now it's going. And what it's doing here, it's kind of cool, classic kind of cloud code stuff is we see that it is intelligently starting like multiple sessions for each slide instead of working on all of them. sort of in sequence it's just it's figuring out how to start them all in parallel so we're seeing some of that nice sub-agent features here

**Aakash Gupta** (00:56:44)

and regular cloud can't do that right

**Aakash Gupta** (00:56:46)

no regular cloud can't do that that's definitely only a cloud code feature

**Aakash Gupta** (00:56:49)

yeah so that's one of the big benefits is the parallelization

**Aakash Gupta** (00:56:52)

okay The only other thing I can think of of why this isn't working is that we might need to like close all the cloud codes for it to pick this up. But yeah, in general, hooks are something that's good to explore. And it's kind of like a good coverage when you're thinking about what are all the cloud code features. Hooks are a good one. And you can add like you can actually add sounds like the whole UI. Some people have really funny ones. Or you could like prank someone where they have it like make like all fart towns. Basically, anytime it takes any action. So that is like a kind of a good power feature to be aware of. Because you'll probably see that like on Twitter and things like that. Let's while we're waiting, maybe we can sometimes you can just. OK, so it's creating all the slides here.

**Aakash Gupta** (00:57:30)

It's not working. Do we need to close off? OK. We are making good progress on our overall demo. So we'll just kind of jump ahead in time. We'll look at these slides after they're created. But let's say that we've presented these slides, and now we've gotten feedback. And then now we need to go ahead and incorporate that feedback into our PRD. And then we'll move into the very last part of our demo, which is using that. Basically, now we have our full PRD. We've presented it to stakeholders. We have the information. And now we want to create the actual engineering tickets. And from the very beginning of this whole session, we set up linear. We'll see that come back into play. And we'll be able to create really good tickets for us that go straight into linear. And then as kind of like our very final step, what we'll do is we will, after those tickets are created, you know, stakeholders, you never really want them to be in JIRA or linear, like kind of checking out what's going on in your project.

**Aakash Gupta** (00:58:23)

You want to give them sort of a source of truth. And so what we'll do is we'll take it, once it's in linear, we'll pull it back into our Google Doc and have like a status update section. And then as a very final thing, I'll show you how you can make that update automatically.

**Carl Vellotti** (00:58:35)

Sweet.

**Aakash Gupta** (00:58:36)

Okay, cool. So let's go ahead and imagine that we have our feedback here. And for that, I think I pre-created stakeholder meeting notes. And then what we'll do is we will have it incorporate that into the PRD. Okay, so we saw that PRD from earlier, and now we will go ahead and update it with those meeting notes. Okay, so it found it locally, and then it will find it also in Google Drive. And now it's also going to find the stakeholder media. So that's one thing that's nice is like you can just really control so many parts of this whole sort of workflow just straight from here. You can just kind of tell it, do this and this and then do this. And if you give it the right tools, it will really figure out how to do all of that. And when it makes a mistake, it will kind of figure out how to fix itself.

**Carl Vellotti** (00:59:16)

Mm hmm.

**Aakash Gupta** (00:59:19)

OK, so still working on those slides. So it's kind of a long running task. So this is a good one where, you know, you'd want to definitely go do some other work while this is happening like we are now. Close this one. OK, so it is looking at its own tools and figuring out what it can do.

**Aakash Gupta** (00:59:34)

Yeah, improving your own ability to do like two things at once is so powerful here because there is like these micro context switches you need to keep making.

**Aakash Gupta** (00:59:42)

Okay, so in this case, for some reason, it's not able to use the MCB. So let's just get the stakeholder meeting notes. So in this example, this is like notes that you may have taken while you were in a meeting. And so basically, what are the key decisions? So, you know, you've presented your PRD, you've done a lot of thinking, hopefully you've met with your engineers before. And then, you know, when you're talking to your main stakeholders, they say, okay, we really need to make sure it's compliant, or we cannot ship this without SSO. So maybe you as a PM, you're trying to get it out quicker. You thought maybe you could do just like regular login, but then, you know, your head of engineering or your You know, head of sales or something is saying we cannot go out with this feature as SSO. So this kind of gives us more requirements for us to include when we sort of update our PRD.

**Aakash Gupta** (01:00:25)

So

**Aakash Gupta** (01:00:25)

hopefully you're using an AI note taker, too, so that you're truly native.

**Aakash Gupta** (01:00:31)

Yeah, yeah, exactly. Yep. That's a good example. Like Granola or one of those. Do you have a favorite AI note taker?

**Aakash Gupta** (01:00:37)

I like Granola because it doesn't follow you into the meeting.

**Aakash Gupta** (01:00:39)

How does it work? I actually haven't used it. Does it kind of sit on

**Aakash Gupta** (01:00:43)

your

**Aakash Gupta** (01:00:43)

computer?

**Aakash Gupta** (01:00:44)

So granola's the way, but it will just, it's like, it's like always there. So if you're worried about your privacy, don't use granola.

**Aakash Gupta** (01:00:52)

I know I've seen some pretty funny memes where someone will join a meeting early on purpose, and then everyone else's AI notetakers will join ahead of them. And then they'll just say super crazy stuff. And then as soon as people join the meeting, they'll stop talking. So then the transcript or the summary of the meeting will be completely insane. And people will be confused why. I don't think anyone has done that, but I actually do think that would probably work.

**Aakash Gupta** (01:01:15)

Oh yeah, that would be a good chaos monkey sort of April Fool's joke on your team.

**Aakash Gupta** (01:01:20)

Yeah, exactly. Cool. Okay, so now we see that it was able to kind of update everything here with what it found in those meeting notes. And then as our final step here, great. Okay, so it updated the PRD. It's kind of telling us what it updated. So now what's cool is at this point, This PRD is really good. You've worked with your team to write it. You've gone to the meeting with meeting notes. You probably talked to your engineer about those meeting notes. You've updated it. So now at this point, you really have a great PRD with all the requirements. So the final step is let's create the tickets. Creating tickets as a product manager depends on how your team is set up. Sometimes engineers do it. Sometimes PMs do it. But just in general, it's always such a painful process because you know the information and you just have to...

**Aakash Gupta** (01:02:00)

go through the UI and click all these buttons and kind of make sure everything's all organized. Whereas now with Claude, it can just literally create all those tickets for you. So let's say now create the tickets for this PRD in the project. Let me see if I already have a named project.

**Aakash Gupta** (01:02:17)

And if your team had a really specific way about how they wanted tickets, you could create a skill around that.

**Aakash Gupta** (01:02:21)

Yep, exactly. Okay, cool. So we have a task flow calendar integration project. So... And we still have that linear MCP setup from before. So now it is just starting the task. So it's going to break it into the engineering tickets and then create them in linear. Great. And what's so cool is that because we have that linear MCP setup, it knows exactly the tools that it has. And it is just starting to work on it here.

**Aakash Gupta** (01:02:46)

Yeah, we didn't play linear, right? It just knew linear is the system.

**Aakash Gupta** (01:02:49)

Yeah, exactly. I have all the information I need. Let me create a to-do list and then create the engineering tickets. So we're seeing that nice agentic-ness of cloud code.

**Aakash Gupta** (01:02:57)

and that's because the mcp was on for linear

**Aakash Gupta** (01:03:00)

yeah okay and then we saw our slides that we were having it create from before let's see how these turned out of course this is another area where like in that slide skill you could provide like more context but what's cool is like this is like a real this is like real google slides these are not images

**Aakash Gupta** (01:03:13)

whoa wait that's actually sick

**Aakash Gupta** (01:03:16)

yeah right and it like designed it kind of nicely

**Aakash Gupta** (01:03:19)

i don't think people know about this

**Aakash Gupta** (01:03:22)

And then anything that you want to change, it won't get everything 100% perfect, but it can be pretty darn good, and this is only improving. And so we have a pretty nice deck here, I would say. You might want to make some edits, but this is not a bad first pass at all.

**Aakash Gupta** (01:03:39)

This is saving you. This is my entire career. I would have to spend time like we'd create a PRD, then we create a deck. It would take an hour or two. Just turn that into a prompt. And if we had made this a proper skill that knew about your template and how you like your slides, it would be even closer to ready.

**Aakash Gupta** (01:03:55)

Yeah, exactly. So that's kind of the final payoff. And then going into our example, we had those meeting notes from these slides, which we're now making the tickets from. But what's so cool is that like this is like a real presentation. Like this is all editable. It made all the little like that's kind of why it was taking so long is because it was defining all these things in like HTML to see how big they should be. And one thing that's cool and I think this will be coming soon is you could actually have Claude like right now it can't really like see its work very well. So it knows like it knows how the code should be. But there's going to be a pretty cool feedback loops soon or I bet there's people who have already built this where you could have it use like a puppeteer or playwright or ones where it can kind of take a screenshot of its own work.

**Aakash Gupta** (01:04:35)

And then you could have it iterate. So this was basically its first pass creating these. But it would be pretty cool to just have it actually look and then make sure that things were aligned. Although it did do a pretty good job with all this.

**Aakash Gupta** (01:04:45)

You mentioned those tools. I think people might have heard about them and not know them. What exactly are Puppeteer and Playwright?

**Aakash Gupta** (01:04:49)

Yeah, so those are really good ones to be aware of. Like if you're doing... anything where you're like creating any sort of like visual UI, where you want Claude to be able to see its own work. And so they're basically just tools for it to create a page like this one, or we had, we had the one earlier where we were looking at hooks, it can build that page, and then it will screenshot it and then like send that screenshot to itself. So it can actually see like what its work is, and then it will can can make edits on its own. And so that's like a really good way when you're doing any sort of front end sort of development at all. Give it those skills so it can check its work. Because sometimes, you know, it'll say it's done and it'll all be all functional, but it'll look terrible because it just like doesn't really know or things will be aligned weird.

**Aakash Gupta** (01:05:32)

If it can see its own work, it usually is like very good at noticing those big discrepancies and fixing them on its own.

**Aakash Gupta** (01:05:37)

I can't emphasize how cool that feature is that we just showed guys. I mean, did we just kill Gamma for PMs with this podcast episode? Yeah, right. Pretty sick.

**Aakash Gupta** (01:05:47)

Okay, cool. So let's see. So it took our PRD and now created 19 engineering tickets. And it also gave them priority, which would be based on what was in that PRD. And it's saying that they're in this project. So let's go ahead. Moment of truth.

**Aakash Gupta** (01:06:00)

Did it do a good job creating these tickets.

**Aakash Gupta** (01:06:03)

Okay, so we can see all these here. They were all created today. And then we see them P1, P2. These are pretty nicely sort of like labeled. Like this is how I would do it as well. So let's like look at one of these P1s. Okay, overview, requirements, technical considerations, and then the acceptance criteria. And so these are still like slightly high level. I think that's because the PRD itself was high level. This would be sort of a great thing that you could hand off to your engineers where they might actually like add more information. But this is like, I think as an engineer, you're really getting a lot of that information around what exactly do you need to be able to build without necessarily, what would be cool is you could even like have Claude if you connect it to your code base, because here it's not connected to the code base.

**Aakash Gupta** (01:06:40)

So it really, it's just saying what the requirements are without saying, like how to build it or anything. But if it was connected to your code base, you could even have it include a lot more technical details. So then the engineer, when they're reviewing, they already kind of have like a great place to start off as they're going through these tickets.

**Aakash Gupta** (01:06:55)

And a lot of people might be wondering about that. How do you do that? How do you connect it to your code base?

**Aakash Gupta** (01:06:58)

Yeah. So in this case, that'll be kind of the last thing we look at here, actually. So we kind of just saw like some two awesome payoffs, right? We saw the ability to actually like where we're seeing is being in Claude, but then actually doing work like out in the world. We have these slides. We've had these documents. We pulled them in. We've created the tickets. The last thing to kind of talk about here is like, how can we actually have Claude work within a code base? So I think as a product manager, in order for that to happen, you'll need to get GitHub access, which I think, you know, two years ago, a product manager is getting access to GitHub would be weird. Like, what do you really need to do looking in the code? But now as more and more PMs are becoming AI native and using these tools and wanting to be able to explore the code base, I've already heard.

**Aakash Gupta** (01:07:40)

I went to a cursor for product managers sort of little meetup. And one of the questions that cursor asked was, how many of you have access to your code base? And it was basically all PMs that were at this meeting. And more than half said that they did have access. So that's one thing that you might just need to ask at your company. Otherwise, I think it'll be a thing that more and more product managers actually do have that access. And the easiest way to do it to give Claude access to your code base is you would just get the GitHub. You just get the link to your repo and then you would just point it at that repo and it could explore it.

**Carl Vellotti** (01:08:07)

Cool.

**Aakash Gupta** (01:08:08)

Okay. Very last thing. And this is very cool to kind of capability of Claude code and a way that as you're building out your systems at work or you're building out your systems like personally with your cloud code at home is actually sort of connecting like your local files to GitHub and then adding cloud to your GitHub so that you can have it take actions for you even when you're not at your computer. And this is what is just so cool. And I want to just kind of demo because I use this all the time. So let's go ahead and kind of move into our very final phase here. And what we're going to do is we will go ahead and let's have it sync everything up. So right now, all of this, all of this code and everything is already in GitHub. If you need it to be in GitHub, all GitHub is, is it's really just like a storage of files exactly like this.

**Aakash Gupta** (01:08:56)

Like if I were to download this project from GitHub, it would just have all of this information in it. And so I'm going to say, please. sync this repo was just like short for repository to GitHub. And it kind of already knows that it was like which GitHub is connected to.

**Carl Vellotti** (01:09:13)

Okay, so

<!-- sponsor -->
**Aakash Gupta** (01:09:13)

it's gonna check and then sync. And then the very last thing we're gonna do is we're gonna actually add Claude as an app to our GitHub repo. And I'll show you why this is like so cool. so right now it's saying there's nothing new in the repo so we're going to be go ahead we're going to be good to just go ahead and push everything into it so it's cool all of the work that we've done locally it's otherwise only on this computer that we just looked at all this on but by pushing it to github now it is like all of those files in the current state are saved in github so if we went to another computer we could just pull all that same information down work there push it back up so it's a good way for you to you know, transfer work between different computers, or if you had something collaborative, they could download it.

<!-- sponsor -->
**Aakash Gupta** (01:09:51)

So that's why it's so awesome for engineers. Okay, so it's now synced. So we can go ahead and open this. And then this repo, I will make accessible to everyone who's watching this video. So you can, it has all the files that we use throughout the whole team, whole time so that you can follow along. And so if you were on another computer, you could just copy this into, you could just tell Claude, hey, let's work on this repo. And it would pull all those files in. Okay, so the last thing we're going to do here is we're going to go ahead and we're going to add Claude as an app. And then I'll show you something cool that you can do with that. Okay, so the way it works is you go to github.com slash app slash Claude. So there's all different kinds of apps you can add to your GitHub repo.

<!-- sponsor -->
**Aakash Gupta** (01:10:26)

We're going to configure this. And then... I already have mine turned on so that Claude basically has access to all the repos. But then there's still one more step that you have to do, which is you have to go into that specific project. And so in order for Claude to be able to work in here, you have to add your API key. So what we're going to do is we're just going to add my Claude API key, which is anthropic key. And then again, I'll go ahead and delete this key right after the video, but we will include it here. Okay, so now Claude has been added to this repo. So what's cool is we can open up a new issue. So let's go ahead and test this. Create a new issue that just says say hello. Great. Then we're going to make a comment at Claude.

<!-- sponsor -->
**Aakash Gupta** (01:11:06)

Say hello. And now what's going to happen is Claude has been assigned that. So I could be, and I could do this from my app. I could do it from anywhere else. Right away, we kind of see this. Whoa, we get like a real emoji reaction here. Claude is telling us that he has seen it. And then now he's going to work this ticket and it will be a new comment. And the way that you can see these is if you go to actions. Oh, it actually picked that first one up too. So we go to our actions in GitHub and there's a lot, you know, as we kind of saw with hooks like when you get into some more of the engineering world there's like a lot of customization and setups you can do but this is just sort of the simplest thing where we're going to add Claude as an app so that it can take actions for us in the repo so now we can open one of these and uh oh my gosh could not man all these these demos are not working as well as I would have hoped today okay well One thing that you can do also is like with this repo, because we have Claude also here, we can say, look at the open issues.

<!-- sponsor -->
**Aakash Gupta** (01:11:59)

Why was Claude not able to work them? OK, so now our Claude that we have like on our own device is going to investigate and it will be able to look at the details and it will tell us. So this is like another good thing is like you can have and this is like a good workflow in general is let's say like as a as a real world scenario. So let's say that you as a product manager You have your PRD on your own device locally, and then you also have it in Google Workplace. But let's say you're at lunch and, you know, you're talking to your engineer and something comes up where it's like, oh, did we consider for that calendar integration feature? Did we consider how we should handle time zones? It's like, oh, yeah. I forgot Arizona actually doesn't have daylight savings. Then, you know, that's one of those things that you kind of normally you just have to remember when you're back at your desk, start a Slack conversation about it or something.

<!-- sponsor -->
**Aakash Gupta** (01:12:43)

But what you could do instead is you could actually just go into your GitHub repo on your phone or something. You could create an issue that says, make sure that we account for time zones in Arizona, you could create that and then you could act Claude. And then by the time you get back to your desk, it will have already worked that ticket so that you can then just pull it back down. And then you can see what it updated. And you can do all this stuff when you're like not even at your computer. One thing I personally use it for is I think I'm kind of a crazy person for doing this. But I have like my whole journal is like on GitHub. Luckily, it's a private repo. And I will just open an issue that's like a voice transcription of my day. And then I'll like at Claude and then Claude will add that to my journal for me.

<!-- sponsor -->
**Aakash Gupta** (01:13:24)

So there's all these kind of different things you can do when you are away from your computer with Claude, like accessible in the cloud. And that's just kind of the last thing I wanted to show is there's like step one of, you know, using Claude code while you're at your computer, but there's a lot more automations you can start to do if you add Claude into your repo. And then there's other stuff you can do too, where like, You can have it automatically run every day and then maybe check a couple of different sources and synthesize them and then add them into your repo so that you can pull them down when you're at your computer. So even though we covered fairly advanced features here, there's still like a lot more to kind of keep exploring with Claude and these automations when it's in the cloud.

<!-- sponsor -->
**Aakash Gupta** (01:14:00)

And since we've put people on GitHub, can you just give them the basics of using GitHub? Because I think a lot of people aren't going to know like pushing and pull requests and branching. What do they need to know about these terms that they've heard if they're going to use GitHub?

<!-- sponsor -->
**Aakash Gupta** (01:14:12)

Yeah, so GitHub is, it's just the best place to kind of like store your files. It's just the easiest way for Cloud to work with these files. I was reading something and it said that Cloud is fiercely competent with Git. And that's kind of, Git is like the language of using GitHub. And so like literally anytime you need to do anything with GitHub or with Git, you can kind of just ask Cloud and it will basically do it correctly. But the main things to know are... So we have our this is a repo or a repository with all of our files. If we want to get those files onto our own computer, then we're going to pull them. And then if we've done work on our computer and then we wanted to go back into the repo, then we're going to push them. That's the really that's like the absolute basics.

<!-- sponsor -->
**Aakash Gupta** (01:14:53)

And then one thing that Claude will do, for example, let's say that you have Don't work on your computer, but you also want to pull work in. It will make sure that it's very, very good. It is fiercely competent. I get sold to make sure no work is lost. That's that's really the basics. If it's like a private repo where it's mostly just your own stuff, then it's really just pulling and pushing. The one other thing to know is like, let's say you're prototyping or building your own feature. then you might want to before you actually like just push that code like all the way into like the main repo like let's say that we had a website that was reading from this and we wanted to make sure that the website was like working with the new code rather than just sort of like pushing it onto like our main live site then what you can do is you can open up a branch and what that is is it's basically like a branch of that code that has new stuff and you can push the branch, but that won't make it go to like, whatever is actually deployed.

<!-- sponsor -->
**Aakash Gupta** (01:15:44)

And then you can test that branch. And then the last thing to know is that once you said, okay, this branch looks good, then you can merge it into main, which is sort of like your main repository. But I would say for most use cases of product managers, you kind of just need to know that you need to pull files down and then you need to push them up. And that's how you're able to sync them.

<!-- sponsor -->
**Aakash Gupta** (01:16:01)

Cool. So it's simple enough. Pull it from your GitHub, push it back when you're done. If you do this at the beginning and end of your session, now you can use GitHub. Now you can have Claude as your remote worker when you're out on the go.

<!-- sponsor -->
**Aakash Gupta** (01:16:13)

Yeah, exactly. And we won't cover it here. But once you have Claude in your GitHub repo, then you can just have like your local Claude set up all kinds of cool stuff. You can have it set up workflows where it checks a certain website for you every day and then sends you an email with updates from that website. You can do kind of like all types of things. And once you kind of get into that GitHub world where Claude is up there, then you can work with your Cloud Claude and your local Claude to do just even more stuff.

<!-- sponsor -->
**Aakash Gupta** (01:16:39)

Powerful stuff. Awesome. So if we had to summarize, right, what we've taught you guys today is from the beginning to the end of the feature, how you can get your survey responses, write your PRD, create your slides, create your tickets, even potentially service some of those tickets with Claude as an agent on your code base. So these are the big use cases of Claude Code. Is there anything else people should be exploring when they're thinking about Claude Code for PMs? I

<!-- sponsor -->
**Aakash Gupta** (01:17:04)

think the main thing is just it's around everything that we've covered today. I kind of hope that it was really just like a good kind of inspirational example of seeing you can use Cloud Code locally. It can pull stuff in from anywhere. You can work on it locally and then you can push it back out. And anytime you're starting like a new task or something else, Just see, can I do it in cloud code is my best advice. Just can I do it in cloud code? And cloud is very good at understanding how cloud code works. And it will kind of help you figure out how to do that. And so the more you're able to do this, the more you build these workflows. And every time the first time will be done from scratch. But the next time you do it, you'll already have that workflow from the first time you did it.

<!-- sponsor -->
**Aakash Gupta** (01:17:43)

So just really have like a mindset of experimentation and know that the first time it won't be perfectly smooth. We didn't have everything work here perfectly today. But even just right now, from that demo that we just tried, now it actually just worked. Now Claude is saying hello. So it might not work perfectly the first time. But Claude is kind of there to help you and just keep that mindset of experimentation and keep trying to see how much more you can do. Because really, these tools are just going to get more powerful. They're just going to get more powerful. We have Cloud 4.5. By the time you see this, there might be Cloud 5 or Cloud 5.5, and it's going to be even more competent. And this is just the way that work is going to happen in the future. So I would say if you haven't started using Cloud Code, start using it now.

<!-- sponsor -->
**Aakash Gupta** (01:18:22)

And if you aren't using it for everything, see if you can use it for everything.

<!-- sponsor -->
**Aakash Gupta** (01:18:25)

That's our challenge to you guys. Try to do cloud code for more. And if I'm honest, you know, I don't use cloud code for everything. I use the UI for a lot of stuff, but I use cloud code for all of my big tasks, my tough tasks, the ones where I want to connect into various MCP servers, the ones where I want to use various context files, the ones where, like I said, I want it to pull down 200 web pages. So for anything powerful you want to do, try to use cloud code. Bring that into your way of working because the people who get ahead of these tools, the people who are really learning how to use these tools first, First of all, all your companies are now evaluating you on how you use AI. So you're going to do well on that. Second of all, you're going to become known as that person amongst your PM team, your product leadership.

<!-- sponsor -->
**Aakash Gupta** (01:19:05)

So when your product leaders have a question about cloud code, they'll start coming to you. And then finally, you yourself will become more productive. Some of these things, as we saw, they don't make you more productive. So I want you to be careful about where you use it. But... Figure out the intuition for when you should and shouldn't use it. Bring Cloud Code in. My guess is the way PMs work, what they spend time on five years from now will look nothing like what they're doing today, which already looks nothing like what it was five years ago. So stay ahead of this. And Carl, thank you so much for bringing us along the bleeding edge of it.

<!-- sponsor -->
**Aakash Gupta** (01:19:36)

Yeah, thanks for having me. It was great.

<!-- sponsor -->
**Aakash Gupta** (01:19:38)

Bye everyone. I hope you enjoyed that episode. If you could take a moment to double check that you have followed on Apple and Spotify podcasts, subscribed on YouTube, left a rating or review on Apple or Spotify and commented on YouTube, all these things will help the algorithm distribute the show to more and more people. As we distribute the show to more people, we can grow the show, improve the quality of the content and the production to get you better insights to stay ahead in your career. Finally, do check out my bundle at bundle.akushg.com to get access to nine AI products for an entire year for free. This includes Dovetail, Mobbin, Linear, Reforge Build, Descript, and many other amazing tools that will help you as an AI product manager or builder

**Carl Vellotti** (01:20:23)

succeed. I'll see you in the next episode.
