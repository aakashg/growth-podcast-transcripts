---
title: "Model Context Protocol (MCP) Explained for Product Managers in 2026"
subtitle: "Zapier's CTO shows you how to turn AI models into real agents using MCP and Zapier to send Slack messages, draft emails, and automate workflows without writing a single line of code."
date: "2025-04-01"
host: "Aakash Gupta"
guests: ["Bryan Helmig"]
speaker_names: "substack"
substack_url: "https://www.news.aakashg.com/p/ai-draft-email-mcp"
youtube_url: "https://www.youtube.com/watch?v=a9wO6GSAoGk"
duration: "00:42:32"
word_count: 7819
source: "Substack episode transcript (aired audio)"
---

# Model Context Protocol (MCP) Explained for Product Managers in 2026

*Zapier's CTO shows you how to turn AI models into real agents using MCP and Zapier to send Slack messages, draft emails, and automate workflows without writing a single line of code.*

**Aakash Gupta** (00:00:00)

Why should people watch this episode?

**Bryan Helmig** (00:00:01)

Well, if you're curious about using AI for work day to day, I think this is going to be a cool one because you're going to see some neat ways to inject it into email or Slack automation, things like that.

**Aakash Gupta** (00:00:11)

Oh, interesting. A lot of people watching, listening, they're engineers, designers, product managers. So I want to hear kind of behind the scenes how you're building AI tool features at Zapier.

**Bryan Helmig** (00:00:22)

We started our AI kind of like journey back in like the GPT-2, GPT-3 days when it was like really early. I think the first thing that you're going to find out building with AI is it's not the most reliable thing.

**Aakash Gupta** (00:00:33)

So let's play with some other Zapier AI features.

**Bryan Helmig** (00:00:37)

With Zapier, we have ChatGPT integrations. A few weeks ago, this is like one of the fastest growing apps on Zapier ever. If you're a product manager, you want to be thinking about that. You want to be thinking not about the happy paths, but also the sad paths. Love it. So if you've been playing around with ChatGPT or Claude or any of these tools and you're thinking like, hey, I want to go and do a little bit more with it. Yeah, you can definitely do things like that. You can pop in here and see a couple. Let's see if there's a couple off the shelf ones that we have here. So send AI generator responses in Slack. Let's give a shot.

**Aakash Gupta** (00:01:05)

That's actually mind blowing. So

**Bryan Helmig** (00:01:07)

you can see kind of how this works. We've even got our little co-pilot over here. You can ask AI to help you set that up. I'm just going to kind of walk through so that we can actually see sort of how it works.

<!-- sponsor -->
**Aakash Gupta** (00:01:17)

Really quickly, I think a crazy stat is that more than 50% of you listening are not subscribed. If you can subscribe on YouTube, follow on Apple or Spotify podcasts, my commitment to you is that we'll continue to make this content better and better. And now on to today's episode. today's episode is brought to you by amplitude building great digital products is hard you know that better than anyone getting teams aligned measuring what matters and scaling your product strategy isn't easy but what if you had a clear framework to guide your next steps that's exactly what amplitude built they studied the best product teams to understand what really drives impact and turn those insights into the digital experience maturity assessment In two minutes, you'll be able to see where your team stands and what you can improve to build better products faster. Click the link in the caption to take the free assessment and get a clear path to product growth.

<!-- sponsor -->
**Aakash Gupta** (00:02:10)

Today's episode is brought to you by Maven. The problem with most courses online like Udemy is there's no live component and the instructors aren't experts in their fields, they're professors. At Maven, you get direct live access to experts and operators from the world's best tech companies. You can't get that access anywhere else, in any university, and you usually can't find them on YouTube either. I've featured so many of Maven's experts in the newsletter and podcast for that reason. To help you out, I've put together a collection of courses I recommend at maven.com slash x slash Akash. This includes courses like AI prototyping for PMs, product sense for PMs, and getting an AI PM certification. Visit it now at maven.com slash x slash A-A-K-A-S-H. Brian Helmig, the co-founder and CTO of Zapier, Can you educate us a little bit? What is MCP?

**Bryan Helmig** (00:03:06)

Yeah, MCP is like definitely on kind of a hype cycle right now. And it is a cool kind of technology. It's sort of like an old idea kind of brought into this AI agent assistant like era. And what it is, is it's a protocol to let your AI agent or AI assistant list tools. What's available? Can I send a Slack message? Can I find a ticket? And then call those. Now there's some other things that it can do. Like it can list resources like, hey, what files are on my file system? different things like that. But I really think kind of the killer use case is that opportunity to have this sort of structured tool calling which devs have been using all the time to build these cool products and actually bring it to like your sort of day-to-day as you're driving through ChatGPT or Claude and have it go out and do things in the world.

**Bryan Helmig** (00:03:54)

So if you've played with things like having to search the web or generate an image, it's kind of that. Those are like tools in a way. But MCP allows you to inject lots of different tools from all kinds of different SaaS apps you might use or the web out there, even like the computer use and things like that where computers are clicking around on your screen. That kind of stuff could be presented as a tool as well. It really just kind of opens up the ability for AI agents, AI assistants to leverage tools, call tools, and interact with the world. And MCP is just kind of a standard and a protocol to define and call those tools.

**Aakash Gupta** (00:04:33)

So Anthropic kind of made it viral right now with their announcement of it, but it doesn't necessarily only work with Claude. And where does Zapier fit into the picture?

**Bryan Helmig** (00:04:44)

Yeah, so Zapier has been around for a long time. We let you build workflows, so we call them Zaps, where you have a trigger, maybe a new email comes in, and maybe you have an AI step that parses that email and gives you like a summarization, and then you send it to Slack. And each of those are actions. So the way Zapier kind of plays into this is we're going to take all those actions, and we've got 30,000 of them, 8,000 different supported apps. And we're going to expose them as MCP tools. So you can go in and turn them on, off, and choose which accounts you want it to have access to, which channels, which inboxes, things like that. So now your AI agent not only can go out and do stuff, but you can kind of control what it's able to do as well.

**Bryan Helmig** (00:05:22)

So that's kind of why we're excited about something like MCP. And this is not our first go at it. We were working with OpenAI on plugins, and that didn't kind of really... nail it. We had AI actions was kind of a more dev tool sort of thing. So it's kind of a natural third time's the charm where MCPs come around. And yeah, we're really excited about it. Something we've been watching for a long time.

**Aakash Gupta** (00:05:43)

So why should people care about Zapier MCP versus what they broadly have available out there?

**Bryan Helmig** (00:05:49)

Yeah, so it's so early right now that a lot of the MCP servers out there are more dev oriented, right? You got to install like node packages locally. They're kind of running on standard in or standard out, which is just kind of the CLI terminal under the hood. calling those. And that is just like a little bit techy. So the reason like this stuff is sort of kind of picking up and gaining a little bit of steam is everyone can kind of see like, oh, this is going to go somewhere pretty exciting and kind of break containment of like devs using it through clients like cursor and what have. Like we know Claude's going to bring it, ChatGPT is going to bring it. So this is really going to be kind of expanding it beyond just purely kind of that dev. experience into kind of a wider business experience or consumer experience pretty soon as this protocol matures.

**Bryan Helmig** (00:06:38)

But it's still pretty early days, I'd say right now, like just maybe at the time of recording, like two days ago or yesterday, they announced like the next revision of the spec. So it's constantly being updated as people are giving them feedback and learning about how to use it and where it doesn't work and where it does work. So it's pretty active.

**Aakash Gupta** (00:06:56)

And what are we going to do today?

**Bryan Helmig** (00:06:58)

Yeah, so we'll try to do some really cool stuff. The use cases are really kind of crazy. Like you're always like playing around with this and discovering things. And as we play with it today, we might even discover a couple like, oh, that didn't work quite the way we wanted. Or maybe what if we tried this and added that? So it's really just so such early days that there's not like standard patterns for how you might use these things. It really is starting to be kind of a thing, but it's a very new thing. So we're gonna try a bunch of different things. We're gonna hook up things like Jira or Slack or some of our products like tables to kind of have like a database sort of a feel. And then you can kind of mix and match these and come up with your own.

**Bryan Helmig** (00:07:40)

And that's kind of the cool thing about it is there's no real like rules. You can really kind of create your own little world and environment for your AI agent to do stuff in, which is just really fun.

**Aakash Gupta** (00:07:52)

All right, so let's start our live cooking session.

**Bryan Helmig** (00:07:55)

All right, cool. So one use case that you can imagine using, as you're working with your agent, you're doing some sort of analysis, you're doing some work, you're chatting with it, and you want to share that summary somewhere. Maybe you've got a bunch of folks that are sitting in your Slack room. You've configured your action for that. For this, I've got a little channel set up for the testing MCP right in here. It's been sending poems and hello messages. Um, but you can imagine like, Hey, I've been doing all this work. I want to share it. Um, you can swap out Slack for anything, right? If you've got Microsoft teams, something like that, and you want to go in and say, Hey, can you offer this analysis to the team? Right. And you know, it might yell, uh, about what it wants to do. Um, Give an analysis of our MCP config.

**Bryan Helmig** (00:09:00)

Send it to the testing MCP room. Thanks. And then hopefully, oh, it's going to go through. Use the tools. There it is. So this is kind of the experience you get whenever you have an MCP call happening. Now, as you can see, it It's gonna try to hallucinate the name of the rooms, but since we've already locked that down, it ain't gonna matter, right? So we have some safety on this front, and really the only thing that we're going to really encouraged the AI to do, even though it did some other stuff, was that text field when we had that set up. So we'll go ahead and just give this a quick little run. It's going to send it out there and go through. And, you know, it's kind of funny, like these different models all do different things. So it's kind of a bear to sort of test these because as you like, oh, it works great with 4.0, it might not work as well in Gemini or maybe it works great in Sonnet.

**Bryan Helmig** (00:09:59)

And it's just kind of one of those things you got to keep playing with to get it to do the way that you want. So you can see like, okay, we got a lot of information back. So it has some cool context. You could click on it and look at it, but we're just gonna hop back over and see if it's sent. So here we got, here's an analysis of our MCP configuration. And we've got all the information kind of coming out of that. What I would imagine people are gonna do here are, derivatives of this. So if you're like chatting with ChatGPT, you've got lots of work that you've been doing, maybe using things like deep research, you've been like doing all this work and you want to share that, you can imagine creating a Google doc that has that summary in there. You could imagine creating a draft email.

**Bryan Helmig** (00:10:45)

You can imagine sending it to Slack or MS Teams. There's a lot of different places where like, okay, I've got it. I've got it here. Now I got to get it there. Like that seems like a pretty like classic use case for something like MCP where you'd be able to send it off to another platform. So it's not just sitting in your chat client and you're copying share links for conversations around, but it kind of actually sits in whatever the rest of your team is, whether that be Notion or Coda or what have you as well. So those are the kinds of things I would imagine people enjoy doing with stuff like MCP, though it's just kind of sending information out there.

**Aakash Gupta** (00:11:27)

Okay, so we're kind of running up on the limitations of MCP through the demo and learning more. Basically what it can and can't do if you were to summarize now.

**Bryan Helmig** (00:11:39)

What it can and can't do, it's changing so much that it'll be out of date by the time folks are watching this. But what it's going to struggle to do is usually going to be limited by the model itself. That's commonly the challenge. The thing that I have experienced using this is that It'll work one time and then it'll like go off the rails the next time. So I think those are the biggest blockers you're gonna have. And I think everybody can kind of relate to that. Like you've been asked to be like, no, no, no, make an image that does this or make it that looks like that or has this in there. kind of gets it, but it doesn't quite nail it. And whenever you're trying to call these tools that have very precise values in them, that's where it'll get tripped up. So it'll be like, oops, sorry about that.

**Bryan Helmig** (00:12:28)

Let me try again. And it'll try over and over again. So those are the places I'd imagine people are going to have continued challenges on. The things that it's quite good at now, you can already see with models like Sonnet 3.7, it's pretty good at recovering from there. But again, that varies from one to another. The amount of... actions and apps that have support, it's kind of scattered right now. Some of the different ways that the protocol behaves, it's a little bit clunky to get set up like we were doing with this. So there's just a lot of a lot of warts I think right now that kind of leak through into the experience. You know, another thing I've noticed with something like a cursor as like a client is it doesn't have great reconnection. So if your internet blips for a second, like you've got to go in here and like refresh it because it's like it loses its connection and kind of gets a little bit stuck.

**Bryan Helmig** (00:13:30)

So there's just a lot of rough edges right now. as clients and servers all sort of do the debugging that's necessary for such an early product. So that's, if I were to say things that are difficult to summarize, the difficult things are gonna be just kind of the state of clients, the state of servers, the state of models. They all conspire to just make it a little bit of a sort of a tricky experience that has funny edge cases and sharp corners in it for now. But it has a lot of promise. It's pretty fun to play with.

**Aakash Gupta** (00:14:04)

So let's play with some other Zapier AI features.

**Bryan Helmig** (00:14:09)

Yeah, definitely. Like one of the things that I like doing is with Zapier, we have ChatGPT integrations. This is something that has been, I think, I do believe as of a few weeks ago, this is like one of the fastest growing apps on Zapier ever because the kinds of things you can do are pretty exciting. Like you've already started to see a little bit of the flavors that you would get from things like, okay, I can chat. Now I can take action with something like MCP. It's still very early. It's got a lot of rough edges. It's pretty exciting. But what about like when I'm not at my computer and chatting, can I leverage AI to do things for me? And that's the exciting stuff that I see users doing with things like the ChatGPT integration. So here's like some example templates, right? You can create email copy with ChatGPT from new emails, right?

**Bryan Helmig** (00:15:03)

And save them as drafts. So you can imagine I get an email. I have ChatGPT suggest a reply, and maybe I have a bunch of prompts on like, hey, I wanted to always mention this or mention that, and then submit a draft that's a reply to that. And then whenever you are ready, you just pop into your drafts folder in Gmail and make a couple tweaks and send it. So there's interesting workflows you can start to use with ChatGPT in the middle, right? So it's kind of like a sandwich, right, where that's kind of the core part. And then you have a trigger that's doing something, getting at the data, and an action on the other side that's taking that data. So those are the kinds of use cases we've seen people do. And it's not just ChatGPT. We have Anthropic and Gemini, and we got all the models in here.

**Bryan Helmig** (00:15:49)

And that's like a really kind of classic use case. But is this something you want to try setting up?

**Aakash Gupta** (00:15:55)

Yeah, I mean, we all have too much email. Let's try to set it up so that it sets a draft email for us. Yeah,

**Bryan Helmig** (00:16:00)

let's

**Aakash Gupta** (00:16:00)

do

**Bryan Helmig** (00:16:00)

it. So you can see kind of how this works. We've even got our little co-pilot over here. So you could set up, you could ask AI to help you set that up. I'm just gonna kind of walk through so that we can actually see sort of how it works. So for me, I'm gonna go ahead and I'll just set up this one and we'll get it all connected. So this is kind of the classic flow you gotta go through. You gotta give Zapier access to your Gmail. But once you have that sort of set up, you can choose like, oh, which inbox do you want, right? So for this, it's just kind of a standard sort of inbox. All right, we're gonna go ahead and test this. And hopefully the email that comes through is nothing embarrassing. And what it's doing is basically it's going out to Gmail.

**Bryan Helmig** (00:16:52)

It's grabbing an example so that whenever we go to the conversation with ChatGPT, we're going to have an example for it to work on so that we can start to iterate on that front. So it's going out there. It's pulling things in. And let's see what embarrassing thing went here. Adventure Club is hiring assistant facilitators. Perfect. So this is like a newsletter. So you can imagine going in here and swapping this out so you only have like inbox or starred messages or something like that. So that's a common thing we see people doing is like, okay, I don't need to reply to every newsletter that comes in. I just need the ones that I've starred or maybe moved to a special kind of label, right? But we'll kind of continue on. We're going to set up something in ChatGPT as a conversation action. That is sort of like the ChatGPT you're familiar with.

**Bryan Helmig** (00:17:39)

You send it a message, it gives you a response. And that's kind of what we're doing here. So let's go ahead and choose this one. We're going to continue in... Now I'm gonna have a little prompt here. So I'm gonna say, do I wanna do it? Yeah, I'll do this. You are a helpful assistant who writes friendly replies to emails. Reply with only the body of the email. And then you can have your content mapped in here. So this is like the user message, if you imagine. It's kind of like an interesting thing that if you've worked with these APIs, all these like settings kind of make sense. But if you haven't really worked with the APIs for these AI services, it's a little bit interesting because there's a lot of capabilities that the APIs have that you're not gonna run into like just playing with ChatGPT.

**Bryan Helmig** (00:18:42)

Like in ChatGPT, you type your message, you get your response. But if you're familiar with going into like your profile in ChatGPT and you can say like, hey, this is how I want you to reply. This is the kinds of things that I do. Here's my role, that sort of stuff. That's what the insistent instructions are revolving around. So you can kind of give it a little bit of guidance. So if you wanted to talk like a pirate, you put it here, right? And then up here for the user message, I might say like email and I would do something like, let's just tag in the body plane. And then I would close that off here. Now I'm doing something like these like little XML tags just because I've done enough with LLMs to know that if you don't kind of like kind of like constrain and say, hey, here's the thing that I want you to focus on.

**Bryan Helmig** (00:19:33)

Sometimes they'll get a little bit kind of confused, right? And let's not use the mini one. Opening eyes famous for a great model naming. Let's use just kind of the standard 4.0. And let's go ahead and just continue and see what it does for the output. So we're going to run this and then see what it has for the response. Oh my goodness.

<!-- sponsor -->
**Narrator** (00:19:56)

This tiny little screen.

**Bryan Helmig** (00:19:57)

Let's make it bigger maybe. Oh my gosh, we get to watch

<!-- sponsor -->
**Narrator** (00:20:03)

one tiny thing at a time.

**Bryan Helmig** (00:20:05)

Maybe Zoom level? Yeah, let's try that. There you go. There we go. Yeah. So here's the request. So you can kind of see what it's sending in. And then if we scroll down, we should be able to see the response. Thanks for sharing the flyers, right? Have a great day. So there you go. You got a decent little reply here. So let's go ahead and continue.

**Aakash Gupta** (00:20:24)

And it's not too verbose. I've pasted plenty of emails into ChatGPT where it gives me like seven paragraphs. So I'm glad to see that it's realistic. Yeah.

**Bryan Helmig** (00:20:33)

Yeah. So, I mean, if you wanted to like tweak this and be like, you know, make sure the responses are formal, right? You can always play around with this and then retest it. And then we can see like, okay, is this better? Is this like in the area of what I'm kind of going for? Which is now we're doing prompt engineering, right? This kind of thing you've probably heard, or maybe even experience where you're please do the thing I want, ChatGPT. That's kind of a classic thing where you're going back and forth, back and forth, trying to get it to do what you want. So as soon as OpenAI responds here, we should see the updated value.

**Aakash Gupta** (00:21:16)

So, and this is just built into like Zapier. Like we didn't need to go get an OpenAI API key to do this.

**Bryan Helmig** (00:21:23)

You would need to get an OpenAI API key for this action. But that's, I'm glad you kind of mentioned that because we do have a couple things that are off the shelf that you can use. They're using some of like the smaller, like cheaper models, like the mini models. But yeah, you don't need an OpenAI key in order... to do this uh but we do have support for all the different models so if there's you got a favorite one like oh i love using claude we have you can kind of plug that one in but you can swap them in and out but there's a couple options where you don't need to bring your own api key So here, let's go.

**Aakash Gupta** (00:21:55)

Yeah, Claude is definitely my favorite writing LLM.

**Bryan Helmig** (00:21:59)

Yeah, yeah. It's one of my favorites for sure. So here you go. Thanks for sending the latest flyers. So a little more formal. You can kind of play around with that. So hopping over to creating that draft. So if we're going to have a draft, you want to map in something like the body, right? So the body that I want to is, thanks for sending the latest flyers, and I'm kind of mapping that in here, right? So for subject, since we're just kind of doing a demo here, you'd have to like kind of configure this so that it actually replies to the message. But you would, who's it coming from, right? You could say from email, right? And then the subject, you know, re. And then this would be the name of the subject, right? And there you go. There it is. And then you'd send through, give it a test.

**Bryan Helmig** (00:22:57)

Now what this is doing is actually testing it. So it created a draft in my email. So let's take a look at what that draft looks like. Here we go. So here we go. So here's the kind of response. So if I'm happy with that, I can just go ahead and send it along. If not, I can make a tweak to it as

**Aakash Gupta** (00:23:18)

well. That's actually mind-blowing. I mean, if I could have Claude draft all my emails.

**Bryan Helmig** (00:23:24)

Yeah. This use case, I think, is a pretty powerful one just because it gives you a lot of time. And oftentimes, you can even kind of guide your AI in that prompting step. Hey, if it's about this, send them here. If it's about this, tell them to do this. If it's about that, tell them, you know what I mean? You can start to really give custom instructions to the AI that is not so oriented around the, like what is the default thing it's gonna write? Like you can reuse this with a custom sort of instructions instead of having all these generic sort of responses, right? That's something that,

**Aakash Gupta** (00:24:06)

So we hook up chat GPT to our email. Can we hook up Claude to our Slack?

**Bryan Helmig** (00:24:13)

Yeah, you can definitely do things like that. Yeah. So if you did Zapier Claude, you can pop in here and see a couple to see if there's a couple off the shelf ones that we have here. So send AI generator responses in Slack. Let's give a shot. So this use case is similar so instead of having a trigger that's based off of an email you get that comes in you're going to have a trigger off of a new message that's posted to a channel and you can kind of choose what that is so for us let's go ahead and let's do testing mcp since we just had that up and we're going to continue through and we're going to test so this again test is looking for that email uh coming in, or in this case, not email, the message. Yep. Let's see if we can pull it in.

<!-- sponsor -->
**Narrator** (00:25:08)

Why is it not doing that? There's messages in here.

**Bryan Helmig** (00:25:12)

Oh, it might be only including trigger for bot messages. Aha. So here's where I'm getting caught up. These are all bot messages. There's no humans that have posted in this room. So I need to post in this room. Hello, world. So there you go. So now when I actually test this, it should pull in a message, like a real message, right? And this is a good thing because this has actually really happened to us where we have a bot posting to a room and a bot responding in that room. So you can imagine the circles you run in there and the bills you rack up, which is always comical. So yeah, you can see like, okay, we got our message. We got our raw text here. Hello world, great. For this, let's see if I've got my, yeah, I got my Anthropic set up. Go in here.

**Bryan Helmig** (00:26:07)

Same sort of thing we just saw, right, where you have kind of the user message and the system message or the assistant instructions. You're an epic joke teller. find a way to make a joke about the incoming message. And then we have our hello world text that we're gonna map in as a user message. Let's go reply directly with the joke. Now you can imagine this being other stuff. Like you can imagine adding other steps in here too. Like maybe I wanna fetch a little bit of information and then I wanna feed not only my message, but some other information that I'm fetching to augment that message into Claude so that it actually has more information to answer that. So we've had people build like pretty sophisticated bots with something like this. Which model do you like? Do you like the new one? 3.5 sonnet is the best in my opinion.

**Bryan Helmig** (00:27:10)

Oh yeah? 3.5 sonnet guy? All right. Let's do that one. Cool. Let's go ahead and continue and let's give it a test. Let's see what it says. All right. Cool. So yeah, you can see that running this, you get a response. Why do programmers hate saying hello world? Because they don't want to start a new conversation thread. So... A decent, decent, decent attempt there. So again, you can play with this. If you don't like that, you want something else. I think the more common use case that you're going to run into is something like... hey, I want you to use my help desk to answer these questions for me, right? Here's my, I'm gonna paste in my guidelines, right? Like maybe you have a bot in one of the rooms that tells you expense guidelines or something like that. And then you paste your instructions here and then you tell Claude, hey, answer those questions based off that instruction.

**Bryan Helmig** (00:28:05)

So that's more of a common sort of use case, but this is I think a good one to just kind of show how it all connects. And what we're going to do here is send a channel message and we're going to have to do something a little bit funny where we have to connect. Oh, custom value. Here we go. Here we go. Enter a custom value here, which is the ID of that thread, right? So that's a little inside baseball on that one. And then what you're going to want to do is choose the same channel. Yeah, it's trying to warn me about that loop that you might have. So as we had that bot check mark, we got this one under control, but it's giving you a little warning there. But we want that joke. Let's get that joke. And then continue. And let's go ahead and give it a test.

**Bryan Helmig** (00:29:03)

So we should see a reply here. There we go. And then if you click this, you can even get into this app that created it. So it works pretty fluidly. So if you're like, okay, that's not a great response. You can hop in here and start to play with that prompt. Let's go ahead and turn this one on. I'm gonna publish this one and we're gonna give it a test. All right, so what's the joke topic we want here? Open AI and Claude walk into a bar. chat GPT here and let's see if we get a response so what it's doing is like that trigger is getting sent off that notifications going into Zapier claws running and then we're coming back to post it because they kept trying to order and prompt format I like the attempt. But yeah, this is kind of a good example of using AI to drive.

<!-- sponsor -->
**Aakash Gupta** (00:30:06)

Today's episode is brought to you by the AIPM certification on Maven. Run by Mikdad Jaffer, who is a product leader at OpenAI, this is not your typical course. It's eight weeks of live cohort-based learning with a leader at one of the top companies in tech. OpenAI just doesn't stop shipping, and this is your chance to learn how. Run along with product faculty and Mo Ali, the course has a 4.9 rating with 133 reviews. Former students come from companies like OpenAI, Shopify, Stripe, Google, and Meta. The best part? Your company can probably cover the cost. So if you want to get $500 off, use my code AAKASH25. And head to maven.com slash product dash faculty. That's M-A-V-E-N dot com slash P-R-O-D-U-C-T dash F-A-C-U-L-T-Y.

**Bryan Helmig** (00:30:53)

Some more of these kind of content free form use cases, which is pretty cool. One of the other things that's pretty neat and maybe a good one to do next if we got time for it would be something like structured generation. And that's where you start to get into more of the complex things like, hey, I want you to apply like a label to this or I want, you know, a specific value out of this instead of just kind of a blob of text, which can really help drive up the reliability of things so you don't have to say respond only with the joke well you can just have a joke field and then map that joke field uh in downstream steps which can really help it not go off the rails which uh elements tend to tend to do often

**Aakash Gupta** (00:31:34)

Awesome. Well, if you've ever wanted to automate your communications, we just gave people a little bit of a guide into how. I think that does it for our live cooking session. I want to ask you some questions about this now.

<!-- sponsor -->
**Narrator** (00:31:47)

Yeah, let's do it.

**Aakash Gupta** (00:31:48)

So a lot of people watching, listening, they're engineers, designers, product managers. So I want to hear kind of behind the scenes how you're building AI tool features at Zapier. How have you guys kind of structured your vision and your teams around that?

**Bryan Helmig** (00:32:03)

Yeah, so we started our AI kind of like journey back in like the GPT-2, GPT-3 days when it was like really early and started building our intuition around this. I think the first thing that you're gonna find out building with AI is it's not the most reliable thing. So you have to sort of build these product experiences from the ground up to handle the inevitable failure cases. So I think if you're a product manager, you wanna be thinking about that. You wanna be thinking not about the happy, paths, but also the sad paths for these. Like whenever, like a good anecdote is we started building a feature, like a logical feature, like describe this app that you want to build in natural language, and then we'll go and create it for you. And it's just a little text box. You type it in, you click generate, and it gets started on it.

**Bryan Helmig** (00:32:51)

And we thought, oh, that's easy. That makes sense. That's what it'll do. But then we noticed that users were just typing in MailChimp or my spreadsheet is broken. And that's not a zap. But we were still trying to generate a zap for them. So they weren't really getting it. So there was kind of this weird UX issue we were having. But the AI was not able to properly kind of process and redirect that user and help them. So that was like a very early learning of like, oh, well, you've got to understand that. People are going to misuse this or misunderstand it, or the AI is going to go off the rails. And you want to kind of bake that in from the ground up. And it helps you kind of pinpoint the places that you can actually work with AI. That is probably the place to start.

**Bryan Helmig** (00:33:37)

And then if you get more in kind of the engineering side, like, okay, we got to build this thing. That's where you start to really lean on some of the tooling that exists. You got things like these APIs, which what we demonstrated is under the hood of our kind of Zapier editor there. There's a lot of API calls happening there where we send that prompt in, we get that response, and you do that over and over again. how do you get that to be reliable and how do you measure how reliable that is? And if you've been in kind of the AI ecosystem much, you probably heard the word like evals. Evals is like one of those things that you're going to reach for. And it's kind of like when, you know, engineers, like they want to build tests, unit tests. It's very similar to that with the slight difference that there's no, it's not a Boolean like, yes, that was perfect and no, that was bad.

**Bryan Helmig** (00:34:27)

It's a gradient, right? It's a scale. And that scale might be like, Well, we, you know, had a positive tone to that response, but that's very subjective. Like how positive we talk in here. And then how do you even grade that? There's no like, there's no like, uh, parsing of that text. That is a classic, uh, sort of technique that can tell you like, oh yeah, that's a, that's a positive sort of tone in the way that you want to describe it. So it just gets a little bit funny when you actually measure these things. So that's probably the next thing on the technical side, like when you build these, it's like start thinking through, okay, how are we going to score what a good response is and what a bad response is? And how do you bake that into the product shape and then also into the development cycle?

**Bryan Helmig** (00:35:12)

So that's certainly a big one. And then finally, the ultimate thing on the other end is like, how do you measure these things? One of the things that we've been doing a lot is using real quick kind of thumbs up, thumbs down sort of buttons. And that allows you to start to find hotspots. So we saw lots of thumbs down as people were typing MailChimp and we were just generating like random MailChimp zaps for them when they really were kind of curious, do you support MailChimp? What actions do you support? What triggers do you support? Or when something was broken and we're like offering triage zaps for broken things, but they really wanted like an answer to those sorts of questions. So we saw very quickly thumbs down and even some free texts like, hey, what went wrong? What did you expect? And that really helped us hone in and find the places where these things, they weren't working the way that users were expecting.

**Bryan Helmig** (00:36:02)

So those are probably the three things I'd be looking at. Plan for both the happy and sad path in your product. Make sure to think through how do you want to score, how these things work, are good or bad. And then how are you going to measure and track where it's failing? And that could also be kind of like classic measurement things of like, did you get some activation moment later on? But you really want to track all three of those things as you're building.

**Aakash Gupta** (00:36:28)

And how are you guys structuring your AI teams? We walked through a couple different features, MCP, standardized templates for ChatGPT to email, and Claude to Slack. Who are the teams that actually built those behind the scenes?

**Bryan Helmig** (00:36:42)

So it's a team of a bunch of folks. We're still actively hiring for AI engineers, trying to find folks that kind of have a touch for this and like doing this. But usually what it looks like is a couple full-stack folks work really well in this paradigm, but usually what you're gonna do is kind of classic sort of product teams. You've got a product manager, you've got a designer, and you've got a handful of engineers. And hopefully there's an engineer that kind of has a feel for the patterns that we just kind of talked about, evals, APIs. But these things also aren't that hard to learn. What I think is probably a common misconception and a shape that we don't necessarily

<!-- sponsor -->
**Narrator** (00:37:25)

have

**Bryan Helmig** (00:37:26)

or isn't required per se for these kinds of AI features or AI kind of product capabilities now with LLMs is like a hardcore ML engineer that's building out custom models. Because a lot of the models that you're using are just off the shelf. Now, that said, the piece of the pie on the kind of ML engineering side where you gotta wrangle all this data and make sense of it, that still has a place. So to the degree that you have engineers that have some experience running SQL, finding the data, know where that data is, that can be a massive benefit on a team. And we really look for that inside because we have lots of examples, and you do too probably in your company, of, hey, here's a user that's very successful, here's all the things they've created. those are really great pieces to kind of ground either evals on or build some scoring mechanisms on because you can say like, okay, we built some evals.

**Bryan Helmig** (00:38:23)

We know this is a really great customer. So if our system suggests the things that they already get a lot of value out of, we should see a pretty high score there, right? So those are good kind of touchstones for the team to have and why it's useful to have a couple people that have that experience, though it's not as particularly deep as it used to be. It used to be you had really deep ML experts on these teams to build these custom models and wrangle all this crazy data. Nowadays, it's a little bit more like a jack of all trades can really do a great job on this but otherwise like it's still kind of a pretty standard uh epd structure that we use as app here

**Aakash Gupta** (00:39:05)

all right and how do you how do you plug in how do the ceo plug in how do you give the teams enough direction like let's go sprint on an mcp feature versus allowing them to organically kind of come up with the right applications within zapier

**Bryan Helmig** (00:39:21)

Yeah, that's a good question. It's a little bit of both. MCP, our version of MCP came along as a long thread of investments, like the kind of the third incarnation of it. And it was an engineer that couldn't make it to our full team retreat that we held in New Orleans just like two weeks back. So he took it upon himself to like work on the MCP implementation and see if we could get something together. And it kind of came together and is something that we could launch. So it's kind of one of those funny moments where a lot of like effort and planning and structure went in to build this kind of foundation. But then like An engineer with a good idea and a little bit of free time was able to add something else that kind of met the moment now with MCPA billing so exciting.

**Bryan Helmig** (00:40:07)

So it's a little bit of everything here. You definitely want folks that have all these experiences and know how users want to get to value in your product. But you also need folks that have like a curiosity and like, oh, I wonder if this would work. you want to chase those feelings within these teams because there's like a new technology and it's not, you can't rinse, repeat things that you've done five years ago and leveraging this. And then every week there's new techniques and new different models to explore. So I think there are a lot of rewards for teams that, lean into that where it's like oh you have an idea like let's carve off let's give you a little time to spike that out and see if it works because there's so many low-hanging fruit right now with this technology that no one has all the answers so it's i think it's good to have a little bit of both in this instance

**Aakash Gupta** (00:40:59)

And I think what's really cool is you were able to ride the wave and release something quickly, whereas some people, I feel like they're taking like three months, they're hitting these trends a lot later. By having that engineer empowered to just go out and do that, it sounds like you have the culture where they are empowered to go do those little experiments and send those out. That's really cool.

**Bryan Helmig** (00:41:17)

Yeah. Another one that we quite like is themed hack weeks or even like hack days where you you get this pent up demand and curiosity from, uh, engineers or even product folks or designers. And nowadays with some of the, uh, tools like Claude artifacts, you can have people put together some pretty, pretty compelling prototypes, uh, and cool experiences that may not have traditionally been like the engineer mold. Uh, so I think this stuff can kind of come from all, all kinds of different places. And we try to structure things like hack weeks to try to give a little bit of space for that too. So you can, you can kind of manufacture it in your org as well with a little care.

**Aakash Gupta** (00:41:54)

All right, Brian. Well, I've learned so much about MCP. I feel like I learned a lot more than I did before. We even taught people how to automate their email and Slack. Thank you so much. Yeah, no problem. Great chatting. See you in the next episode.
