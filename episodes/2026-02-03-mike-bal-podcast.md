---
title: "How to Build An AI Native PM Operating System with Mike Bal, Head of Product at David's Bridal"
subtitle: "Here’s how to build a composable OS that connects everything through Cursor and Claude Desktop"
date: "2026-02-03"
host: "Aakash Gupta"
guests: ["Mike Bal"]
speaker_names: "substack"
substack_url: "https://www.news.aakashg.com/p/mike-bal-podcast"
youtube_url: "https://www.youtube.com/watch?v=1C0daBcDBig"
duration: "01:01:20"
word_count: 12211
source: "Substack episode transcript (aired audio)"
---

# How to Build An AI Native PM Operating System with Mike Bal, Head of Product at David's Bridal

*Here’s how to build a composable OS that connects everything through Cursor and Claude Desktop*

**Aakash Gupta** (00:00:00)

Where should PMs actually be

**Mike Bal** (00:00:02)

using AI tools in their workflow? I think exposing users to context limits for the models are BS. On the back end, you know, most of them are handling this better anyway, and you can see that even in tools like Cloud Code. There's a much better way to handle it. I ended up going from Manus back to GPT for ancient mode and then immediately switching back. It's just infinitely better.

**Aakash Gupta** (00:00:20)

mike ball is leading product at david's bridal which is undergoing a massive digital transformation so he has been testing out all the ai tools i have been testing out all the ai tools we have put our heads together in this episode to create the ai native pm operating system we've been talking a lot about claude claude claude

**Mike Bal** (00:00:41)

why

**Aakash Gupta** (00:00:41)

not chat gpt

**Mike Bal** (00:00:42)

GPT with 4.0, I think the last two model releases, I felt like got more towards lazy and less useful. So I just don't spend as much time in there. I just feel like Claude's more reliable for me. Wow. If you're stuck behind corporate structure, enterprise tools, and your organization's not really supporting, here's how you can kind of think about working around it with your own tools and projects. That's a way better method than most people do.

**Aakash Gupta** (00:01:06)

Before we go any further, do me a favor and check that you are subscribed on YouTube and following on Apple and Spotify podcasts. And if you want to get access to amazing AI tools, check out my bundle, where if you become an anal subscriber to my newsletter, you get a full year free of the paid plans of Mobbin, Arise, RelayApp, Dovetail, Linear, Magic Patterns, Deep Sky, Reforge Build, Descript, and Speechify. So be sure to check that out at bundle.akashg.com. And now into today's episode. Mike, welcome to the podcast. Thanks for having me. Excited to be here. What makes an AI native PM?

**Mike Bal** (00:01:48)

I think there was a term floating around for a while that I think was on the right track. I'll say thinking prompts is kind of this like fundamental thing that sounded silly at the time. But when you start doing this day to day and you're actually integrating tools, I think it's how you end up working. right? Like, what is the thing I need to get done? What is the best way to do that thing? And if you're thinking about AI as like an extension of yourself, you're thinking like, what are the instructions? What are the steps? And if you're reflective, like you probably do that to yourself at some level anyway, you have your inner dialogue, right? But I think that's the biggest thing is the AI native PMs are actually working from what do I need to do to what are the steps that I need to get done, to what are the best tools to get me those things.

**Mike Bal** (00:02:31)

And they're pushing themselves beyond that mental block that's like, oh, that's too technical. Oh, that sounds too hard. Oh, I'm not sure how to go about doing that. And they're working their way up to that, even if the thing's maybe outside their comfort level. So can you show us what the best operating systems really look like? Yeah. I mean, it should be a pretty familiar view for most people who are playing with AI right now, for example. So let me bring up my screen. We're going to jump around to some different tools. But the first thing we worked on together is kind of this map, right? That I think takes this idea. And the more I thought about it, the more was kind of obvious to me that it's not necessarily a set of strict tools, right? And that's why you mentioned operating system. You were actually operating with a layer of abstraction from UI, like logging into 20 different tools for a bunch of different tasks throughout the day is a bunch of time wasting that kind of happens that people aren't going to have a lot of patience for.

**Mike Bal** (00:03:28)

So what I see more and more people doing, especially a lot of the thought leaders who are kind of teaching and educating others in our space right now, you have your kind of centralized tools like cloud desktop or cursor. And you're connecting those to everything else. You're either bringing things into it, like context, data, whatever else, or in some cases you're having it interact with the other tools that you maybe use like a Jira or a GitHub. So maybe I'm in working on a PRD and I'm not sure if something got completed or if something actually shipped or if that was in the backlog. Instead of opening a tab and checking JIRA or looking through the PRs, I can actually say, hey, can you check and see if this issue on this project was completed? I think it was, but I'm not sure off the top of my head.

**Mike Bal** (00:04:10)

Or, hey, I know there was a PR waiting for this. Did that ever get pushed? We've been waiting for a bug fix and prod or something. I don't have to leave the tool that I'm in right now to get an answer for that, which is nice. I can just kind of stay in my flow state without changing the UI for anything, which is pretty cool. There's other things that I think happen outside of the OS, right? Like maybe some design concepts or brainstorming, like I'll use tools for research. And we were talking earlier about not all the research you get right away is something you want to bring into your actual project. So there's maybe an intentional layer of abstraction, but most of the work work I'm doing is happening in this middle area where between either cursor or a cloud desktop. Awesome. Can you demo

**Aakash Gupta** (00:04:50)

for us how this all gets put together?

**Mike Bal** (00:04:52)

Yeah, for sure. So let's start with like a really simple, more technical task. So if you're not familiar with cursor, there's kind of three areas to this. There's, this is collapsed right now, but this is the cursor agent. And you can kind of see conversations I've had about how to troubleshoot or different things that were happening in the past. You can collapse that down. This middle area, you have two things, which is your file that you're editing or looking at, which you don't actually even have to have up. Most of the time I don't. I have cursor setting, which is telling me I have some kind of MCP configuration errors, and we'll talk about this. And then down here is terminal, where I use to interact with cloud code. The left side is your file search. So again, I don't really actually use the IDE like most developers would for the files.

**Mike Bal** (00:05:38)

I'm using cursor to connect tools to either the agent that I showed on the right side, or I'm strictly using the terminal inside cursor so that I can navigate between files and interact with cloud code. So for example, this was a case where some of the content for all the wedding planning tasks and our thing where it wasn't a spreadsheet and it was driving me crazy. So I want to start moving it into actual content management system. Um, so I can ask like whenever I start a new session, for example, again, I have something like most recent changes. And Sanity. Sanity is the CMS. I have the MCP connected already.

**Aakash Gupta** (00:06:20)

And for people who don't know, CMS is like a content management system. It's often like the backend for a blog or something like that.

**Mike Bal** (00:06:27)

Yep. And MCP is model context protocol, which is letting you connect these apps and tools like Cloud Code or Cursor to the other tools that you're using without having to do most of the coding and integration yourself. So it's going to check basically it has an API key that proves that I can access the information. It has kind of its own map to the API so it can go and find the information that I'm asking for. It's going to think for a second as it does this and try to get me an answer. So, well, this is giving me an answer about sanity's actual acquisition and changes that they're doing. Um, let's ask about get history instead. You see this. You are helpful assistant integrated with sanity through the model context protocol. I guess that's the initiation prompt whenever you mentioned MCP. Okay. So this is a little bit of like debugging behind the scenes for them.

**Mike Bal** (00:07:30)

I suppose we can share this with them later and let them know. Okay. Okay. So we can start this back up again. So now that it's awake, so usually what I'll do is come in here and actually start the project. So it's connected to my sanity studio or whatever they call it. It's giving me the information confirm it has access to these things. So it has a data set production project ID, yada, yada, um, So it's looking at found 10 total documents it's checking within sanity itself. And it's showing me changes to the actual tasks that we have at our, our planning thing. Um, so I could go and ask it, or I could ask him more questions about the task structure or things that we were working on, or I could go ahead and ask it to make changes. Like say if I wanted to add something to it, um, like, uh, a task for car rentals or something like that for the honeymoon.

**Mike Bal** (00:08:35)

I'll remember to undo this later. So instead of me having to go into sanity and spinning up, it runs the studio locally. It's pretty technical to get into and then going in and adding new tasks manually. It's just going to do that for me. So creating what I can planning test titled rent a car for your honeymoon. It's creating that document, which means it's creating the content. And then that goes into the tool. I don't have to go to the tool. So this is like a not super exciting task, but if you're editing different things and managing them, you can interact with a lot of these tools that have MCPs or, um, even APIs without having to leave your kind of home base. And that's conceptually how that part works.

**Aakash Gupta** (00:09:17)

very cool so this is the power of mcp connecting to whatever other tools you have and using the operating system as the home base to connect to things

**Mike Bal** (00:09:26)

yep and that's that's a really simple version of it i've done this with superbase for structuring you know database schema or even doing migrations on the fly Um, I've done it with hosting a little app. Like if you end up by coding something you want to launch live, you know, I was saying render has a nice MCP. I didn't have to know anything about DevOps to actually get it up and hosted and get it running, which is pretty nice.

**Aakash Gupta** (00:09:48)

Very cool.

**Mike Bal** (00:09:51)

So if we go back here, that was kind of the, you know, let's connect to technical tools via MCP and bring that into cursor. You can do the same thing in cloud desktop. If you want, like what I just did in the IDE, we could connect the sanity, uh, MCP to cloud desktop. I don't have it on mine right now because it would be duplicative, but you can, if you're more comfortable with this interface, right. You can do the same kind of thing. You can go into cloud settings. should be here you can go to connectors and then you can connect all these different tools they support out of the box and then you can also go and configure your own if you want to as well which just is a simple text file

**Aakash Gupta** (00:10:38)

Okay, cool. Powerful. So in this episode, we've been talking about how all these tools connect together. And one of the tools, the center of the stack for some of the best AI native PMs, well, that's today's episode sponsor, Linear. You just saw Mike pull from Jira and Confluence. But here's the thing. Linear has basically the best system of record for the top teams. There's a reason OpenAI, Perplexity, and Visele use it. Even Cursor uses it. Linear is built for speed and those teams need speed. And here's what makes linear different is linear built for agents. With linear agents, you can call something like a cursor agent to code for you or a cloud code agent to code for you simply on a task. This is a really cool workflow for AI PMs to actually make changes to production code. There's a reason already 60% of enterprise linear accounts are using these agents.

**Aakash Gupta** (00:11:28)

I spent six months doing a deep dive on Linear. I talked to their CEO, their head of product, their head of design, their COO. And what amazed me is that they are operating like teams from the future over a billion dollar valuation with just two PMs. And that's because Linear uses Linear to build Linear. And if you want to build like Linear or like OpenAI or Cursor, then you need to check out Linear.app slash Akash. That's L-I-N-E-A-R dot A-P-P slash A-A-K-A-S-H. The coolest thing is that you get a free year of Linear's paid plan, a $600 value, completely free for becoming an annual subscriber to my newsletter. So check it out. Either go get a discount at that link or become an annual subscriber and get a full year free of Linear. And now back into today's episode with Mike. And I noticed you had some custom instructions in your cloud.

**Aakash Gupta** (00:12:16)

What are your favorite custom instructions?

**Mike Bal** (00:12:21)

You know, at the project level, mostly what I do, so we just have a bunch of different initiatives. So I try to frame the context of the project rather than everything in the entire application, because it's all related in this case. Like this is my own account, so it has different projects in here. This is the wedding planning app specifically. Media network is advertising and partnerships that we have across like e-com and everything else. So having specifically, this is the app we're talking about, this is the app we're working on, or this is the ecosystem we're talking about, and this is the specific lens we're working on, or David's Rattle. I don't have one in there, but that's more of like overall architecture, tooling, internal things and initiatives, right? So I like try to set that for the specific ones that need to be differentiated. And then hope that it can maintain, but I also use like the memory MCP so that it has those relationships that it picks up over time to the different ideas.

**Mike Bal** (00:13:15)

Cause sometimes I'll have to say, Hey, I need you to actually look across project knowledge, or I'll need you to pull information from these two different projects to do what I need you to do right now too.

**Aakash Gupta** (00:13:24)

Oh, cool. Very cool.

**Mike Bal** (00:13:26)

and they're rolling out memory features and, um, with Claude, which I think helps with that too. But having the memory MCP was a thing that's let me do that for the past six to nine months or however long I've been using it now.

**Aakash Gupta** (00:13:39)

And some people might be asking, we've been talking a lot about Claude, Claude, Claude. Why not Chad GPT?

**Mike Bal** (00:13:44)

Anthropic ruled. I mean, they created the MCP framework and have supported it best. Claude desktop had it out of the gate and I think supports it well. They have their own team that rolls out supported MCPs and things like that too. OpenAI has MCP support, I think, via API, and maybe they're rolling it out in the chat app now. I was pretty happy paying for both or at least using some GPT with 4.0. I think the last two model releases I felt like got more towards lazy and less useful, so I just don't spend as much time in there. I feel like they started rolling out connectors in the consumer app. Like if you go in via UI, you can do it. So you could do all this stuff there if you want to. I just moved away from that because I think the type of work that I do is much deeper and requires a little bit more connecting and tooling.

**Mike Bal** (00:14:32)

I just feel like Claude's more reliable for me.

**Aakash Gupta** (00:14:34)

Yeah. I think Claude is also just a better writer and PMs are doing a lot of writing. So generally you're going to prefer Claude, but if you have ChatGPT at your work, they're starting to roll this out so you can do a similar sort of stack with ChatGPT at the center.

**Mike Bal** (00:14:48)

I have a post somewhere about a deep dive on MCP on my newsletter. And there's a handful of like desktop apps and open source projects that you can run that kind of act as a gateway. So they'll let you connect MCPs and then they'll connect to whichever models so you can jump between them. I have one called, I think it's Fire, but it starts with a five that I've been playing with that is pretty cool. But it's like a project to get set up and going. But if you don't have the tools you want or they don't have the capabilities you want, you can actually kind of like hotwire MCPs in a weird way, which is interesting. Cool. What's next? Let's look at design concepts because you and I were doing this earlier and I thought this is a simple but pretty interesting use case when we were trying to conceptualize this.

**Mike Bal** (00:15:32)

So I opened up this, which is similar to what we just were showing on the other screen in Canva, right? Yeah. The bad thing about this is it's flat. So it's just an image. We can't edit it or tweak it without a lot of prompting and back and forth. So what I did, and I do this with some product design work and development too, is I just dropped it into Figma and I'll zoom in on this so we can see it a little bit better. I just did a blank file for this, but. What I'm going to do is if I right click this frame, you get the send to option and you can go to Figma make and I'm sure you can just go to Figma make and upload that too. But the cool thing about doing it that way is you can do this with any of the designs that you're working on with your team anyway.

**Aakash Gupta** (00:16:16)

Yeah.

**Mike Bal** (00:16:17)

So it's going to send that and I think it picks up in this case, there's not very many layers, but if you're sending a design file that has layers, it's also going to pick that up and make it better. Um,

**Aakash Gupta** (00:16:33)

Help me make this an interactive visual. I can edit

**Mike Bal** (00:16:40)

and rearrange, let's say. That's vague enough. I don't know what it'll give me, but let's just see what it does because I don't want it to work for 20 minutes while it's building this out. So I don't really trust Figma Make to code anything useful. I haven't seen it functionally finish anything to the level that I'm like, oh yeah, I can move this into GitHub and work from here so far. But I think it has a unique advantage in that if you're working on your product files that are structured in your design system, it's easy to move them in here and you can visualize like maybe a specific flow for a user, a variation or a new feature and see how you might integrate that and then bring that back to the designer because they're probably working on other things anyway and be like, hey, conceptually, like functionally, this is what I was going for.

**Mike Bal** (00:17:23)

What do you think? and when you bring it back i'll show you you just copy it and it's fully layered and everything so they can take the different pieces that they want from that and and just add it into the design create the new model create the different screen or whatever and bring it back into the same file so it's a it's a big time saver for

**Aakash Gupta** (00:17:39)

designers so if you're thinking about which ai prototyping tool is sort of most most designer friendly figma make is up there is that the air prototyping tool you generally recommend

**Mike Bal** (00:17:50)

I don't even use it for prototyping. I think I use it mostly for design variation. If in my head, and maybe you'll reply to this as a PM, if I'm like, oh, we really need to see this edge case, this error handling, this state for this functionally, and I also am asking the designer or that design team to start working on the next thing because we're trying to move pretty quickly, but I want to have it for the developers, I'll actually take the design we have and throw it into here. and then make it usually it's interactive at some level right so what you can do in here which is nice is you can edit these and then you can change the state of it so maybe i say i want drag and drop I don't know what it'll give me for this. This is kind of a weird use case, right?

**Mike Bal** (00:18:37)

But it abstracted the visuals and things that we had, but it gave us something we can at least play with it. And then if- Editable, but it's not nearly as

**Aakash Gupta** (00:18:45)

nice as what we had out of-

**Mike Bal** (00:18:48)

Right.

**Aakash Gupta** (00:18:48)

It will probably-

**Mike Bal** (00:18:49)

Well, there's little GitHub icons in here. Maybe it's still loading some of this in, but let's see what it does. while it's doing that say the nice thing about it is you get different states so say we have like an edit state right now we have this drag and drop i don't know what it's doing it's just letting me move it which is kind of weird so i'm not super happy with this but just for the sake of time let's say like i'm going to copy this design i'm going to go back to my figma file i'll zoom out a little bit And I can paste this in here. Now I said, the cool thing is now we can actually open this up and we have the entire diagram and canvas with the containers and all these different elements.

**Aakash Gupta** (00:19:31)

Yeah.

**Mike Bal** (00:19:32)

All the text bubbles and everything. So this, what you were doing in Canva was trying to create all these manually. Right. But if we wanted to go in here and say like change, any of these or how we organize them or whatever, it's actually easier doing it in here that it would be on, oh, there I have the edge of it in Figma maker, even in Canva from scratch. Right. So you get the different UI elements, you get the states that they were in or whatever. So it's just kind of a nice like shortcut to get the, the state, like the visual state that you want without having to sit down and be like, here's 20 screens. I need you to work on for this week that are all edge cases, the functionality we already agreed on kind of thing.

**Aakash Gupta** (00:20:10)

Yep. And what do you recommend for AI prototyping? If not, think of a make.

**Mike Bal** (00:20:14)

So personally, I think the last three months I've been blown away by AI studio. And what I mean by this, this is like Google's demine developer focused or AI developer focused team has AI studio as like a play space for developers. Right. And they've done a good job of also not alienating non developers. Like they're really encouraging people to get in here. But this is where you can test the newest models. You can get like a API key really quickly and for free to start playing around with some of these things. So if you're like, oh man, they just made a huge announcement. I want to go play with this thing. This is kind of the ideal place to go. On a personal note, I also feel like in terms of how they manage like chat context and memory and the actual experience, this is infinitely better than Gemini.

**Mike Bal** (00:21:03)

The app. because I'll go in there and ask for an image. And then if I ask for a variation of the image, it'll just give me the same thing again. Like it doesn't know that I'm asking like reference the first thing and give me this edit to it. And there's a lot of little contextual things like that in the Gemini app that I get frustrated with that don't exist here. I think the developer team just built a better experience for developers than the Gemini app did for consumers. So if you're in a studio and you got to build You can one shot, especially they have like a bunch of kind of pre-selected functionality or example apps. Um, but we did, my team was asking me to like prompt and create a bunch of, uh, like we had some dresses that were on sale and to come up with Halloween outfits, for example.

**Mike Bal** (00:21:46)

And instead of me manually doing that and trying to understand all the different like dress subtleties and stuff, which I'm not great at. Um, I was like, can we just spin up this app real quick? Right. and let them... It's not like a consumer-facing app in this case, right? It was just like, can we create a costume from this? And I think it should run. I haven't used it for like enriching the West. Okay. So I didn't connect this to my API queue or something like this, but it does by the updated or something, but we just use this to generate some marketing images that we launched. So it'll take the dress image. It'll take the prompt and it'll create like a costume image kind of mock up for marketing in this case. Which I did this in literally 10 minutes because somebody was messaging me in Slack like, hey, this is my prompt.

**Mike Bal** (00:22:36)

Here's an image I'm trying to go for, but I keep running into X issue. I'm like, let me just put it in here quick. And it was usable in 10 minutes. And then I probably broke it afterwards,

**Aakash Gupta** (00:22:44)

tweaking it or something. Got it. So Google AI Studio for prototyping. How does that fit into the overall operating system?

**Mike Bal** (00:22:51)

So what I tend to do is go into build and work on some of these like rough concepts. Here's just like a general notebook type app I was playing around with, right? Of like it's infinite canvas, but it looks like a notebook. You can do something. I don't even remember why I did this at the time. um what you can do once you get to a point where like okay i want to play with this more i'll either push it to github or i'll deploy it to cloud run or both in this case so i'll download the zip push it to github and then i'll switch to cursor and just open it up and start working inside cursor to edit from then on get the local set up and start running it and then that way i have more of my normal workflow of like You know, I check my browser and see that app running locally.

**Mike Bal** (00:23:35)

I can kind of experience it. And then I go back in here and give it feedback or start describing the change that I want to make to it or whatever integrations that I want to do. And then it's just that back and forth, more like a true developer workflow at that point. But it has to be at a certain level of quality before I pull it into like my main operating system spaces.

**Aakash Gupta** (00:23:53)

Makes sense. What's next in the operating system?

**Mike Bal** (00:23:58)

Let's see. I think one of my favorites has been, uh, progress and knowledge. We'll combine the two in this case. Um, so I'm just gonna go to a new chat inside my, one of my projects. I'm just gonna ask like, what do my confluence say about the vision board, which is just like a feature that we launched a while ago on the MVP. So this is going to use the Atlassian MCP, which uses that new rovo AI search. And it's going to go through and check to see specifically, I'm hoping it's smart enough to know I'm in the planner. And so it should look in that space and confluence and find my doc. It's going to check for my requirements documents. And then it's going to give me some kind of summary for this. And then what I'll do actually is grab a Figma link at the same side or the same time.

**Mike Bal** (00:25:09)

And I'm going to show it should use the Figma MCP and I'm going to ask it to compare.

**Aakash Gupta** (00:25:23)

This is some seriously connected workflows. I haven't been working in this connected of a way and now I'm really seeing the benefit of the operating system concept.

**Mike Bal** (00:25:32)

Yeah, I think some of the trade-off, right? Like you were watching the screen as it was thinking and finding this information. It's pulling that in for me because this is something I've already written, right? Like it already exists. I just didn't want to open Confluence and try to find that page and copy and paste the specifics. But then what I'm going to do on my other screen while that was loading is go back to my MVP Designs. And I'm going to grab just the link. So the Figma MCP is kind of weird. Um, it uses a lot of context and usually maxes out Claude, which is a complaint I have. But if you give it a specific URL to a frame, so if you go into Figma and just kind of what I did earlier, but instead of saying send to make, you just grab a, a specific share URL, you can go to share and copy URL, um, or copy as they changed it now.

**Mike Bal** (00:26:18)

I don't know why they did that, but copy link to selection. So now I'm going to ask. I'm just going to ask it if I'm missing anything or if we missed anything from the MVP design comparison. And this is probably stuff I've already done, right? Like I've already gone through and I'm like, yeah, we're not going to do this. We are going to do this. whatever, but yeah, but it's going to go to that specific frame. And I think the way the Figma MCP typically works is it'll grab a screenshot of it instead of trying to pull in all that information. And if you saw it, ask me to allow it. So depending on what MCPs you set up, you can also set them so that they ask for permission every time they do something or they don't ask for permission to, uh, find content or read.

**Mike Bal** (00:27:08)

Uh, but they do ask for permission before they edit anything or push any changes, which is how I have it set up for the most part.

**Aakash Gupta** (00:27:15)

Nice. So you're using the Figma MCP. It sounds like very regularly.

**Mike Bal** (00:27:22)

Um, it depends on, I mean, if you think about product lifecycle, right? Like if we're working on something new or we're working on our version 2.0 set, there's kind of different waves. We're all get in Figma more. I spent a lot of time in Figma still too, uh, working with design on getting those things done. And then when I'm working on like refining my requirements before we get to the dev team, or when we're working on first, like pie in the sky designs, I'll definitely be pulling that into a cloud code or cloud desktop probably more often. Got it. And that's what I think is nice about the operating system approach is your tool stack can be very composable based on what you need. And so the whole pricing strategy thing from a SaaS standpoint is tricky, right? Because it might be, I'm going to pay for what I use as more people move in this direction.

**Mike Bal** (00:28:11)

That's kind of like a developer API usage-based billing for a lot of these services. Um, and it might be very fluid over time, right? Like it might be a specific use case where I need to use, uh, I have like a, a marketing type app that we're spinning up that uses super base and it uses a Google cloud and it uses something else. Or it might be something internally that has a totally different stack and I might need to be able to fluidly jump between them.

**Aakash Gupta** (00:28:37)

Hmm. Makes sense.

**Mike Bal** (00:28:39)

So here it's giving me a pretty good gap analysis, the layout, the icons, everything. Wedding style doesn't display, which is true. We actually don't display wedding style from the onboarding process on the vision board at all. Um, the documents say show bridesmaid only, which is true. I think we had wedding party versus we shifted a bridesmaid afterwards. So it's catching pretty specific things that are like little discrepancies in

**Aakash Gupta** (00:29:04)

design, right? So it's actually huge lifesavers. I mean, normally you're like pulling up the PRD, you're looking at the design or you just miss this altogether.

**Mike Bal** (00:29:13)

And second guessing yourself. And then like in this case, I'm still going to second guess myself and this and like double check it. But at least I'll have some context and like idea of where to point my time. And if people are like, you can't trust it. I think like I've done both, right? Like we've been around long enough to have done both manually. And like, I trust this as much as I trust myself going through a massive list and comparing every single module and things side by side, right? Like something might get missed or something might not get missed. And it just like, it's nice to have a second brain to rely on to gut check yourself.

<!-- sponsor -->
**Aakash Gupta** (00:29:43)

Yes, that's my favorite thing about AI is it's like my second brain. Sometimes I wouldn't have even asked a person for it, but I don't feel as bad asking AI. This episode is brought to you by Linear. You know what's broken about product development right now? It's not the coding. We've got AI agents for that. It's everything else. The planning, the feedback synthesis, the endless context switching between tools. You're drowning in PM busy work while the actual product work suffers. Linear started as that issue tracker that engineers actually want to use, which, let's be honest, is pretty rare. but it's evolved into something way more powerful. Your entire product development hub. Their new AI features are a game changer for PMs. Product intelligence automatically surfaces insights from customer feedback and support tickets. No more manually combing through hundreds of reports and tickets. and their AI agents will help draft PRDs, scope projects, and handle all those status updates nobody wants to take care of.

**Aakash Gupta** (00:30:36)

Product teams from OpenAI to Vercel use Linear to build complex products at speed. There's a reason they call it magical. See for yourself at linear.app slash akash. That's L-I-N-E-A-R-A-P-P slash A-A-K-A-S-H.

**Mike Bal** (00:30:51)

Yeah, so we talked a little bit about, so we have prototyping, we have... kind of knowledge reference right like pulling from confluence and then gut checking it against figma we had an example where we took like a generated image and created a prototype and pulled it into figma so you could play around with different states um we haven't talked about research yet which we probably should actually done first but uh we can do that next

**Aakash Gupta** (00:31:14)

does

**Mike Bal** (00:31:16)

that

**Aakash Gupta** (00:31:17)

sound

**Mike Bal** (00:31:17)

good

**Aakash Gupta** (00:31:17)

research for is this setting up your project context or what are the right points in the life cycle to be using this

**Mike Bal** (00:31:23)

Yeah. So when I say research, I think ultimately what I tend to mean is context gathering. So if there's, there's a couple of different ways I usually go about this and I would say I pair, I used to use perplexity a lot more, um, because I think the good brain exercises, what questions actually matter to answer when you're working on something new. So, um, I'm not logged into that one right now, but everybody knows perplexity kind of works as you ask a question, you get some answers, right? Yeah. So you might ask something like the use case that I think I had up here right now is this one that I used to test reforge build when it was in beta mode. It was a app that maps out paranormal sightings. My kids are into this podcast and stuff like this, but functionally it's interesting, right?

**Mike Bal** (00:32:11)

Because it was a community app. So it's like people need to be able to post sightings. There needs to be like a governance or like in a workflow, like a queue where you can review or flag if it seems like it's spam or something like that. is you need to be able to plot these things out on a map. And then there was a time dimension of like, how did they play out over time and being able to filter that. So like functionally from an app standpoint, it sounds really silly, but there's a lot of really cool interactions that are there that like, if you're testing a vibe coding tool, this kind of is a good way to stress test it. Yeah. So in this case, right, like I was like, well, I don't I know what my kids tell me about this stuff, but I went through and I was like, this is all I gave it.

**Mike Bal** (00:32:49)

Manus is fantastic at this, by the way. I don't feel like with agent mode on GPT or any of the other tools, like even research from Claude, like it tends to max out pretty quickly and burn through a lot of your usage. So this is nice. We'll just run independently and let you know when it's done. And it gives you its entire trace of everything it did. Right. So all these different sources. And then when I say context gathering or research, what I also love about this is I can ask for specific deliverables and it's also going to show me. So it did like a sample set CSV, a combined CSV with different sites. It gave a data sources report and a markdown file. So I know where that data came from. It gave a quick start guide to be able to use it. And then it's giving me like a more human summary, but I can access all these files that it gave me.

**Mike Bal** (00:33:36)

So even if I really just wanted one of these deliverables, I can access every piece of them independently and use them elsewhere, which I really like about this tool. So maybe it gave me a specific set that I thought was more useful than that. So what I think I actually did in this case when I was doing this is I pulled this information in and then I gave all of it, like the raw information from that to Claude. And I asked it to give me, so I could test these tools, product requirements, user research and personas for it, and then like a technical strategy or approach for it. So I have these three different artifacts now in this kind of like joke project and I can pull these down. And that's how I typically would go into like AI studio, like we talked about before. and then give it those files as the requirements to build something new.

**Mike Bal** (00:34:25)

I did that for Reforge and it did a great job with the design. Or you can take those files and then work on actual requirements and refine them and then even build them from, if you wanted to go straight to cursor, you could, right? Or go into Figma and like try to work on some design concepts for it or something from that make screen. It just depends on how you want to go about doing it. This is a specific for me to test like vibe coding app, so. Would Reforge Build fall

**Aakash Gupta** (00:34:50)

in your top three AI prototyping apps then?

**Mike Bal** (00:34:53)

In terms of like where it got to from a, hey, is this functional? Does it match my requirements? And is it actually like from a product taste standpoint, does it match like some of the details I put in here about UX? I think it did a good job. I think Studio tends to be still where I go to to get it to a functional point, fast, easy, reliably, and then I can take that code and run with it. um or i can host it there and then i would say i i use replit for a long time probably early on before they dealt with a lot of issues and i just got really frustrated with that asian like to me about like oh i fixed this or hey i implemented this new thing and i spent more of my time being like why did you implement a new thing we had that working yesterday and then you go back into the code and you're like we were using python and now we're using python and there's node implementation that are fighting each other and the whole thing's broken or something

**Aakash Gupta** (00:35:42)

so i

**Mike Bal** (00:35:43)

just i i think like you can use those tools to get a concept up and running but i feel like they're designed um to make you feel like you're you're progressing when maybe you aren't and so if you're more technical or more capable maybe it's better to jump into something that lets you transition from concept to code a little

**Aakash Gupta** (00:36:00)

bit better Yeah. So Manus over chat GPT agent mode, reforged build and Google AI studio over something like a replet.

**Mike Bal** (00:36:10)

Yeah. And this is like even stuff for date nights, right? Like, you know, here's what we're into. Here's the weather. Here's where we live. Like, I want something within an hour drive out, hour drive back, something like that. So we're not gone too long. Like you can give it all these things and it'll just run and bring back all the research and different options and things like that too. so the the big reasons i jumped to this are a it's just good at running independently and being thorough and b being able to get um multiple assets right like this is a lot of different pieces to prove that it did the thinking right like here's uh Research on the open AI SDK that they rolled out to build an app inside chat GPT. And I said, make sure you review this documentation for the technical approach or whatever.

**Mike Bal** (00:36:56)

And it, and it does it like, this is capable of this. It's not capable of this. It has the details, but you can trace it back, which I really like.

**Aakash Gupta** (00:37:05)

Very cool. When do you use Manus

**Mike Bal** (00:37:09)

versus Claude regular? I still feel like my frustration with Claude is chat length limits and then usage limits. Even though like for work, I'm on the max plan, right? 200 bucks a month or whatever. And I don't really hit those as much anymore. But if you actually turn on research mode, I feel like it just runs and runs and it doesn't do a great job of showing its work or its thinking like Menace does. So if I have like something quick I'm working on in here. Uh, I don't even know what that would be off the top of my head. I think I've used research like twice in the last two weeks and maybe it was more technical or something by default. Um, or it was some kind of weird offshoot, like a rabbit hole kind of thing that came up. Uh, um, No, that was Figma.

**Mike Bal** (00:38:04)

So, yeah, I don't really use research in here very much, to be honest with you, because I feel like it just burns through. Yeah. And that way. And the other reason I do that is because if menace gets something wrong and I don't agree with it or it finds information that I don't like, I can pick and choose. right? Like here's prep for this podcast. And I gave it kind of the notion content and was like, go through blog posts or here's what I'm thinking about this. Like how should we position it or how are we thinking about it? Like I had some decent ideas in here, right? And this is just like my notes, but I can pick and choose what I actually bring into my core operating system so that it doesn't give it the wrong idea or it doesn't start. Cause the bad thing about a lot of the LLMs is They'll pick and choose what's in the memory to really anchor themselves to.

**Mike Bal** (00:38:50)

And then they become like common assumptions or common beliefs. Like everything it responds to is based on a common belief that you gave it. So if you're not careful about what you feed it, I feel like you end up with like the equivalent of a conspiracy theorist, like LLM partner who is like running with random ideas that maybe aren't as important as some of the core information you gave it. Cool.

**Aakash Gupta** (00:39:11)

What else should we understand from the operating system perspective?

**Mike Bal** (00:39:15)

I think the conceptually, if you hear the word composable in like technical architecture a lot or like MarTech, where you can kind of, and it's kind of like modularity with furniture or whatever, right? You can kind of pick and choose how you want it laid out or how it's configured to meet your needs at that time. it's like these are all different kind of use cases and things that you deal with throughout your given week or month or whatever i think there's also things that come up that are you know i have a specific project or specific ask that has unique requirements i was doing something in the domain space tied to this next round of applications for new tld strings or top level domains which would be like a dot link for example or dot com or whatever And when you apply for these, there's a huge cost to apply for them.

**Mike Bal** (00:40:03)

And there's a really big list of like, uh, evaluation criteria that goes into it. So it was like, is there a patent or a trademark already out on the string that you're applying for? Is there like a cultural sensitivity or a significant geographic region that might have stake to that first? Are there any like language conflicts where in one language it sounds fine, a different one is offensive. And so there's this long list. And for that, it was like, you know, I wouldn't say that the API for the patent database is something I'm going to use again. Right. But at the time I can go get that. I can connect that via cloud code, for example, to the application that I'm working on or the process, the agent that I'm trying to build. And that's like a one time thing. Now, that wasn't even an MCP in that case.

**Mike Bal** (00:40:49)

I just had to go get the API key to be able to use it. But it's the same process either way. Like with the MCP, you configure it and you put in your API key. With this one, you give the API key to your coding agent or cloud code and it handles that part of it for you. So I'd say like as a big takeaway, there's lots of different things you get asked to do in any given day or week. And like the right set of tools is not constrained to the ones that you can log into and use, right? Like there's lots of different solutions out there for different things that are sometimes free, right? Like very generous free tier plans on APIs or things that don't cost money at all that can like make you more effective or make the solution that you're working on more valuable.

**Mike Bal** (00:41:29)

That makes sense.

**Aakash Gupta** (00:41:30)

Yeah, 100%. I think this is an incredibly powerful way to work. If we go back to the nano banana image, I think there was also something you had put in there around communications and email. How do we handle that side of it in the operating system?

**Mike Bal** (00:41:47)

Yeah, I think, so there's MCPs for Gmail, there's MCPs for Slack, there's MCPs for Calendar Connector. I actually think even in Claude, if we go to the browser settings, maybe there's native connectors just for this. Yeah. So they do this via cloud right now. So this is my other account. If I want to connect my calendar or something and ask it what I have coming up this week, or if I want to connect my Gmail and ask it to look up like, when did we schedule the podcast interview with Akash, right? It can do all those things for you. You just have to give it access to be able to do that. We can even do this

**Aakash Gupta** (00:42:27)

right now. I've never used this use case and I consider myself a cloud super user. I'm having so many epiphanies in this episode.

**Mike Bal** (00:42:35)

Well, that's, I have a hard time thinking of a lot of the automation, like N8N or even Zapier. Sometimes I'm like, what do I do often enough that I feel like there's a direct use case, right? That I'd want to configure something or I'd want to be able to do something. So then let's go back to chats and see, I'm trying to think of what I would even have in drive right now. Um, Oh, this is searching chat. Sorry. I

**Aakash Gupta** (00:43:07)

was going to say, you can do that too. Kind of. You had to do it from an actual chat. I see you've chose Sonnet 4.5. So kind of like the right mix of burning tokens, but effective, not opus.

**Mike Bal** (00:43:20)

Yeah, I think it switched. I was happy with 4, honestly. I think 4.5 is like a slight lift. But whenever it updated, it switched to 4.5 or I switched to 4.5 when it was an option. I just kept it there because I think it consistently does a good job. And maybe it's like slightly noticeably better. not i don't think it's significantly better right but um so for this one for example so the connector it'll let you add manually like if i want to look for something like this then you can pull it in but i think the connector should also search my google drive for me unless that needs to be configured separately as an mcp And they didn't have MCP in the browser version before, and they only had it in the desktop. But I feel like, okay, so it's searching Drive for me. That's

**Aakash Gupta** (00:44:03)

cool. Wow. Drive is so hard to search. Even though Google is a search company, I don't think its search is that good. So being able to use Claude is a huge win.

**Mike Bal** (00:44:14)

So this is the most recent one. This is what I talked about with the super guys about like planning that vacation. And when the memory MCP is like ended up being really useful to me because it was like, oh, your five-year-old likes crystals. There's a place you can go mine for crystals here. It's like 30 bucks for a bucket. And it's in between your stay in Lake Tahoe. So you don't have to drive four hours straight. Like you can break it up and get some exercise kind of thing. But yeah, it can get all this context. You can view the full document or pull it in or whatever. So it's pretty easy to use that. They are MCPs. They're calling them connectors because I think MCP is probably intimidating for less technical people. But they finally made the update. At first, it was just on desktop and you had to configure it there.

**Mike Bal** (00:44:53)

Now they're running it in browser and cloud, which is nice.

**Aakash Gupta** (00:44:57)

So let's say you weren't on the Google stack. You were stuck in Microsoft. Could you do this there too?

**Mike Bal** (00:45:02)

Let's see. I feel like they do have an Outlook connector. oh i broke it leave it to me i have that

**Aakash Gupta** (00:45:17)

is like a model launch yesterday but maybe they're a little bit bland

**Mike Bal** (00:45:23)

let's see if desktop is broken too yep okay you're supposed to be able to get there from from the actual app

**Aakash Gupta** (00:45:39)

Yeah,

**Mike Bal** (00:45:39)

there it

**Aakash Gupta** (00:45:39)

is.

**Mike Bal** (00:45:40)

Yeah. So they've got notion Figma. Let's see. Microsoft MS learn docs. No outlook as far as I can see, but I don't know if that's like a common one for cursor. Uh, no clarity. No, Microsoft is a little bit behind on getting this stuff out the door. Uh, you got Roussel post hog Netlify all these specific ones. You can connect to click up Chrome dev tools is sweet actually. Um, especially now that the cursor browser or the cursor agent has browser use, so it can go in there, it can pull dev tools report and it can actually like test new functionality that you're working on in your local instance. Not that I totally trust it blindly. Right. For testing anything, but it's a nice extra step instead of like go to the browser, copy the console error, paste it back in. Uh, but yeah, this is, I mean, this is a long list of all sorts of different tools.

**Mike Bal** (00:46:39)

Like fire crawl is a developer tool, but I've used it to pull data, like shape data and shape contacts for different tools and stuff too. Even pulling like our color swatches down, honestly, it's just easier amplitude. If you have product data in there, you can pull that in and kind of like, cause sometimes even if I'm in a coding space, I'll think in that coding space, right? Like what does the data say? And you just shift cloud code to plan mode instead or whatever

**Aakash Gupta** (00:47:02)

the case is. Awesome. So this is the operating system for AI native PMs. One thing that sticks out to me is this is a lot of AI tool licenses, a lot of IT requests, a lot of money to be spending. Can you just walk through what are the different licenses that teams should be getting access to their teams or product leaders should be getting access for their PMs here? Yeah.

**Mike Bal** (00:47:30)

Yeah, I think the big ones, right, like are what level of access you give to. So, and depending on how technical your PMs are, right, like maybe JIRA is enough or if you're in linear or whatever the case is, but I think like read access for AI tools versus write if you're conservative. I think... At a personal level, some of these are free, right? And some of them are being done separately, like using the Gemini app. I use that through my personal email, which is on Workspace, and I play around with that. Or AI Studio is free with any Google account. And as long as your team's aware of like, hey, let's not take a bunch of... ip or like private information or product specific things that are internal and bring it in there like you can still conceptually get a lot done outside right like if you're just trying to come up with ideas and then bring them into your tools like figma for example or set up your own sample app that's like an example or use case for what you're trying to do before you spin it up internally or have a developer start working on it or even start building up your own private repo for your own internal apps kind of thing so i think that's that's how i tend to navigate it is like 90% of some of this thought and planning work doesn't actually need a ton of private context or private data or company information.

**Mike Bal** (00:48:41)

But if you're actually working out of this day-to-day, I think your core tools, so if you have JIRA, you have Confluence, or you have Notion and you have Linear or whatever the case is, the easy first step for PMs to start working this way is just connect it to where the actual knowledge they care about lives. Like, what are my requirements? How can I get a pulse on dev progress? You know, like little things like that.

**Aakash Gupta** (00:49:03)

Okay. So to summarize the licenses you should be getting for your team, sounds like we can do the $20 a month Manus plan, probably the $100 or $200 a month Claude plan, potentially the free version of Cursor. Is that right?

**Mike Bal** (00:49:16)

Yeah. Yeah. I think you can, especially if you're paying higher end for Claude, I don't think you actually need the Cursor agent if you're not doing actual dev work. And even then you can use Claude code for most of it. And I'll say for the Claude paid plan, the way that we're handling this internally, even not just in product is like, why don't you start and show me that you're using it, right? Like that you're getting some value out of it on a $20 a month plan or whatever the case is. And then if you show me you're doing it and it's helping you and you're leveraging it in the way that's like moving things forward, happy to bump it up. And then if you start hitting limits on that, you're actually using it like we can bump it up again. and that way you're not just giving everybody a blanket 200 a month plan that can add up pretty quickly if they're not really using it but you have them like building habits that are using it productively and then it's 200 bucks a month is nothing right compared to how many hours of work it's saving them at that point

**Aakash Gupta** (00:50:08)

Nice. And then they might need access to the pro plan of Google AI Studio and Nano Banana Pro if they're doing a lot of generations. So potentially $20 a month. So the minimum viable AI native PM stack, what I'm hearing, $20 a month for Claude, $20 a month for Manus, $20 a month for the Gemini package. That's basically it, right?

**Mike Bal** (00:50:30)

Yeah, and I would even argue at some level, like if you're working with IT, right, like you can, everything in AI Studio, and that's part of the reason I like it too, if you're just connected to the cloud account and you can say like, use this API key. So like your IT team could go in there and spin up a project and give an API key that specifically has access for usage-based billing and give you permission. And then any of the stuff you do in there can just be billed to that. And then it is usage based and you're getting like wholesale rates essentially based on usage instead of paying like another software subscription. Right. So like if you want Gemini in the app, you can. But I like at this point, I almost prefer like, oh, I have an API key used specifically for testing.

**Mike Bal** (00:51:09)

Right. Yeah. And nano banana two five is like four cents an image. So I could go crazy someday for like a week or whatever and spend 20 bucks. And then I might not use it again for three weeks. And then I'm not on the hook for another three months and I'm not paying a monthly subscription for nothing. Right. I think like that's probably the way a lot of this will move. You just have to have the connector to your core core tools where your teams are working to be able to move that knowledge in and out.

**Aakash Gupta** (00:51:34)

Sweet. So let's say you're a PM and you're stuck where you don't have access to Cursor. You don't have access to Claude or Manus. How do you go make that case to product leadership and to IT to get access?

**Mike Bal** (00:51:49)

Yeah.

**Aakash Gupta** (00:51:49)

I

**Mike Bal** (00:51:50)

mean, I'm pretty bullish at this point. I think like everybody in leadership executive level, I mean, I work at that. So David's is a 75 year old wedding dress retailer. Okay. And so we've got a lot of old beliefs and processes and things. We've got a lot of old tools and everything like that. But when I talk to leadership and I say like, Hey, this is what my team has been able to get done. at this velocity and this is like our team is one quarter of the size of most other teams that are working on this right now right here's how we're doing it or if i say here's what this investment means and ultimately like what the unlock is for us to be able to get done this year you know, you have these different pain points, these different problems. And if you can show and build the trust of like, like shipping, I don't know anything about shipping and logistics and things like that.

**Mike Bal** (00:52:38)

Right. But I took some of the data and reporting and things like that. I'm like, here's three different ideas that might be causing us excessive overhead on some of this. And they're like, oh yeah, we hadn't thought about problem B. Like, okay, that took me 10 minutes. So imagine what a team of me could do if they're just asking smart questions. They tend not to push back on that. If they do, Like this is going to sound a little harsh, but I would be fairly concerned about any organization pushing back on people trying to use AI to be more productive and more impactful.

**Aakash Gupta** (00:53:08)

Yeah. Sadly, a lot of PMs I talk to are in that world. They're living, you know, whether it's automotive or finance or healthcare, where they seem to be living like five years in the past. But I think what you said there of maybe you create like a personal use case or you show the personal productivity or you show how it can get you more velocity. And maybe you chip away like one tool at a time. Like maybe you don't hit the whole operating system right now. I think in particular, like Manus might be one that you could potentially wait on, but you really can't wait on Claude, right? So you start with, okay, I need Claude. And then you can kind of move your way up. And if you're stuck on a particular stack, like a lot of people I talk to, it's just that they have access to ChadGBT.

**Aakash Gupta** (00:53:51)

then i think what you do is you say okay let me try to do the best i can with chad gpt and then let me show them with my personal work how claude can upgrade that and then bring that to them does that sound right

**Mike Bal** (00:54:01)

yeah

**Aakash Gupta** (00:54:01)

yeah

**Mike Bal** (00:54:02)

i think it's like show that you're getting value from the technology first right like get buy-in on the fact that there's an opportunity there to move faster increase your impact overall to solve hard problems that maybe you weren't able to solve or you have different constraints around or whatever i think like organizational buy-in on the value of the technology is step one. Because a lot of people are stuck in, yeah, it seems like a cool toy, but how are we going to use it on the business level? We have lots of other things that are more important right now. There's always lots of things. If you show like, oh, it accelerates us, oh, it helps us tackle these hard things, or oh, it's unlocking talent, right? You have people sitting there who are capable of more and you're just giving them like... menial jobs or kind of like a lot of overhead work right and they're able to work around that that there's immediate value so from there you can say like okay from this tool here's what i can do here's what i've been able to do and here's where i'm hitting a wall here's what i could do if i had x tool instead of y tool and i think like at least if you have that case built up underneath right it's easy to justify

**Aakash Gupta** (00:55:00)

and

**Mike Bal** (00:55:00)

it's not too different from like a feature roadmap or like a product roadmap or a specific feature you're trying to pitch right like Did the user see value in the first thing that you shipped? Like what issues are they running into that we need to help them navigate? Like what are our goals that we're not hitting that we need to move past or what is the unlock for this? So like that's muscle memory that all PMs have. I think the pitch is ultimately the same. It's just like me getting things done instead of users having this experience or us hitting this metric, right?

**Aakash Gupta** (00:55:32)

Amazing. And then finally, before we go, can you just walk through like the life cycle of PM and when they should be using these various tools?

**Mike Bal** (00:55:42)

Yeah, I mean, I'm in the weird, you know, early, extreme early adopters and testing and playing with this stuff. My default is you should be using them the entire life cycle. I think there's a huge value or there's a ton of value in your upfront research and validation. And that's everything from like what we showed earlier about pulling a bunch of data in, right? Like what about this consumer segment versus this one? What about this use case? Is it as relevant to our target audience as it might be to this other audience that's kind of tangential? Um, getting actual numbers and finding what is or isn't available, what competitors already in the space, who's targeting, right? Like based on the competitors that are here and their recent marketing and the recent releases, who's, who is on a trajectory to go after the same thing that we're targeting, like who's going to be neck and neck with us.

**Mike Bal** (00:56:34)

Or even like, okay, I've done my research. I've talked to customers. Here's scripts from interviews. Here's like, here's like our, our whole justification, right? tear this thing apart like red team this thing tell me tell me what i'm missing be a skeptic tell me what what you think is wrong about it like give me every possible angle so that i'm prepared to defend it and that i actually believe it at the end of the day right and i think like up front everything and then throughout the process it's every interaction right like am i checking my design to make sure it meets requirements like we talked about am i Using it to shape the actual tickets that I'm putting into JIRA or linear or whatever to make sure they're very clear and very specific. Did I reference the GitHub repo for the code base to actually make sure that the ticket wasn't conflicting with how the thing is currently built?

**Mike Bal** (00:57:20)

If it's like an add-on feature or something. There's a lot of little things you can do that were not expected before, but are very easy to do now that add a lot of clarity and value for the entire team. So I think like lifecycle wise, even if you're branching into like prototyping and things like that, I don't see a place where AI actually hurts unless you don't know what you're doing

**Aakash Gupta** (00:57:39)

with it. Amazing. And along this lifecycle, what are the biggest mistakes PMs make with AI tools? I

**Mike Bal** (00:57:47)

garbage in garbage out still resonates with me. I think over prompting is one that I think backfires often really deep, really structured prompts that are meant to be reused and systematic, like a copy paste without understanding the subtleties of every time, like the things that you're doing differently, unless it really is just a repetitive task, like generating requirements. I don't feel like I need a prompt structure to do that because it depends on what I'm starting with or where I'm at or what stage of thinking I'm in. I think the data you pull, for example, I think laziness with AI, like you put a prompt in tool A, like Manus, you downloaded the files and you uploaded them without reading them in say like a Gemini and you prototype something out, like you're probably going to get something that's maybe along the lines of what you're thinking, but not very intentional, where you're kind of proving that that level of product management isn't valuable anymore, right?

**Mike Bal** (00:58:40)

Like taste is incredibly important. I think intuition is incredibly important. Being able to be like, being able to look at something and say, I did this for X reason, is 10x more valuable than like i put this dog together so being able to defend it and being really intentional about the end state of it i think is some people tend to let go of that too early on especially more people like that are junior that i've worked with tend to be like hey i put it in here like you said like i used ai i put this doc together and then i read it like but it doesn't make any sense like yeah you probably you probably did use it but like none of this ref like represents the information that we have or the interviews that we sat in like did you use any of those things or not right and they just don't check it or they don't question it like you have to be kind of skeptical with all of it i think

**Aakash Gupta** (00:59:27)

amazing this has been a master class truly one of the episodes that i've had the most epiphanies on in terms of the gaps I have in how I'm using AI, all of the connectors that you talked about, this concept of an operating system is an incredibly powerful concept. So if you are a product leader, start to think about, am I giving my team the access to the right tools? Have I taught them about this operating system concept? Should I go through a training on it? And then if you are a PM, are you using enough connectors? Are you building an operating system? Do you have cloud skills that are helping you? Do you have cloud projects that have the context? And then are you connecting it to all these tools? This is how you actually get the most out of AI. Nowadays, most of you guys are being evaluated in your performance reviews on how you used AI.

**Aakash Gupta** (01:00:13)

This episode has just given you a bunch of keys to get a better rating on that. Mike, thank you so, so much for dropping the sauce. No problem. Thanks for having me. All right. Bye, everyone. Take care. I hope you enjoyed that episode. If you could take a moment to double check that you have followed on Apple and Spotify podcasts, subscribed on YouTube, left a rating or review on Apple or Spotify and commented on YouTube. All these things will help the algorithm distribute the show to more and more people. As we distribute the show to more people, we can grow the show, improve the quality of the content and the production to get you better insights to stay ahead in your career. Finally, do check out my bundle at bundle.akashg.com to get access to nine AI products for an entire year for free. This includes Dovetail, Mobbin, Linear, Reforge Build, Descript, and many other amazing tools that will help you as an AI product manager or builder succeed.

**Aakash Gupta** (01:01:09)

I'll see you in the next

**Aakash Gupta** (01:01:09)

episode. you
