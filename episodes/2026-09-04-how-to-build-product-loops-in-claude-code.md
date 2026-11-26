---
title: "How to Build Effective Product Loops in Claude Code, with Chief AI and Product Officer at JobNimbus, Tyler Folkman"
subtitle: "People keep saying loops are the new prompts. Here’s a practical walkthrough of what that actually means for PMs and product builders"
date: "2026-09-04"
host: "Aakash Gupta"
guests: ["Tyler Folkman"]
speaker_names: "substack"
substack_url: "https://www.news.aakashg.com/p/how-to-build-product-loops-in-claude-code"
youtube_url: "https://www.youtube.com/watch?v=XsnSvFo4MHQ"
duration: "01:08:51"
word_count: 13363
source: "Substack episode transcript (aired audio)"
sponsors:
  - name: "Customer.io"
    url: "http://customer.io/productgrowth"
  - name: "Ariso"
    url: "https://ariso.ai/aakash"
  - name: "Viktor"
    url: "http://viktor.com/aakashgupta3"
  - name: "Bolt"
    url: "http://bolt.new/aakash"
---

**Sponsors:** This episode is brought to you by [Customer.io](http://customer.io/productgrowth), [Ariso](https://ariso.ai/aakash), [Viktor](http://viktor.com/aakashgupta3) and [Bolt](http://bolt.new/aakash).

# How to Build Effective Product Loops in Claude Code, with Chief AI and Product Officer at JobNimbus, Tyler Folkman

*People keep saying loops are the new prompts. Here’s a practical walkthrough of what that actually means for PMs and product builders*

**Tyler Folkman** (00:00:00)

We talk a lot about vibe coding, but we don't talk as much about vibe PMing.

**Aakash Gupta** (00:00:04)

Everybody keeps saying loops are the new prompts. What does that actually mean?

**Tyler Folkman** (00:00:08)

I honestly believe it's a very powerful skill for engineers to develop. In five years, I'm not sure we'll refer to ourselves by functions. There's nothing magic about being an engineer or a designer and that being in our title.

**Aakash Gupta** (00:00:20)

Tyler Folkman, the Chief AI Officer and Head of Product at JobNimbus, which just raised Utah's largest Series B round ever at $303 million.

**Tyler Folkman** (00:00:30)

I know we talk a lot about AI versus people and replacing them, but I am a huge believer that with AI, it's more people-centric than it's ever been.

**Aakash Gupta** (00:00:38)

That's kind of like career reputation suicide, I feel like, for a PM at this point, right? Like, do not ship anything. So should every PM, designer, and engineer be aspiring to upskill themselves into a product builder?

**Tyler Folkman** (00:00:51)

In my opinion, yes, unless...

<!-- sponsor -->
**Aakash Gupta** (00:00:56)

Before we get into today's show, please take a second to check that you're subscribed on YouTube and following on Apple and Spotify podcasts. If you want access to all of my favorite AI tools, I've gotten them to give you an entire year of their paid plans. Check out bundle.akashg.com for an entire year of Bolt.new, Airtable, Speechify, Descript, Magic Patterns, Linear, Dovetail, Arise, and Mobbin. And now into today's show. Everybody keeps saying loops are the new prompts. What does that actually mean for product managers? How do you actually build a loop that's effective? What are the steps to improving that loop? Today, we brought in somebody who has the data scientist He has a scientist and engineering background. He is the chief AI officer. He leads up product and engineering at one of Utah's most exciting startups, JobNimbus. Tyler is going to walk you through not only how to set this up, How to improve these loops, how to think about these loops.

<!-- sponsor -->
**Aakash Gupta** (00:02:00)

Nobody is teaching you how to do loops specifically for product work. If you are an engineer, if you are a designer, if you are a founder, you're going to learn so much about how you can potentially vibe PM. If you are a product manager, you are going to learn how to make loops and use loops. So I hope you enjoy this episode as much as I did. Tyler, thanks for being here.

**Tyler Folkman** (00:02:19)

Yeah, thanks for having me. It's great to be here.

**Aakash Gupta** (00:02:20)

So let's get started. How do PMs and product people use loops?

**Tyler Folkman** (00:02:25)

Yeah, it's something we talk a lot about. I feel like AI more than most things has a lot of hype and not a lot of action. So I'd love to just show you kind of what we do and try to be really safe that I don't show anything I'm not supposed to. So what I've got up here showing is the action It's an actual system that I use every day to do loop engineering, context engineering, whatever you want to call it, and we'll talk a little bit about the differences. But the system I'm in for people that want to follow along is called Herder, which lets you essentially orchestrate agents And was built with a ability to essentially run itself. So I've built this thing called Orchestrate, which I can then tell it to spin up another agent to research contractor needs in 2028. And it actually knows in Herder, which you'll see it do in a second here, how to spin up an agent, how to open a new pane on the side here, which I can move between.

**Tyler Folkman** (00:03:21)

You see I'm working on some different leadership stuff, hiring, And these green dots actually tell me what's done. Like this one's ready for me to look at. This yellow is it's moving. And then this one I've already looked at. So to get to your question, this is really the pane of glass that I use to manage multiple loops, which is kind of starting with getting an AI helping you.

**Aakash Gupta** (00:03:45)

Why would I use Herder instead of VS Code or Cursor or Claude Code in the terminal?

**Tyler Folkman** (00:03:51)

Yeah, it's a great question. I think, and I was actually pretty skeptical maybe a year ago about terminal-based coding agents, but they've gotten so powerful and the systems around them like Herder have also been made in such a way that's powerful that it feels so... It's super native to work in the terminal where it can access what it needs to access. I get that this isn't as maybe sexy as VS code, but for me, I can actually just have like a terminal open that's an editor. If I'm doing some coding, I can also in that terminal spin up an agent In Herder, I can even split panes and do all sorts of work. So it's easier for me to have control over the agent loop cycle as opposed to having to rely on VS code to release things at the pace that the industry's moving. And that's one of the things that's really fun about the community tools because most of them are using AI to help build the tool.

**Tyler Folkman** (00:04:42)

They move very fast and tend to evolve very quickly as AI improves.

**Aakash Gupta** (00:04:46)

And then we're using this term agent. I feel like agent is like used on so many things. What makes it an agent here versus just another Cloud Code instance?

**Tyler Folkman** (00:04:55)

Super solid question. For me, the difference is an agent is doing something on its own. And making decisions versus you consistently prompting it. So like GPT, chat GPT came out and most people are interacting with it at a level of question answer, question answer. I've heard people refer to this as almost like smarter Google search. Agentic is more you're giving it a task with a way to verify itself and asking it to execute on that by itself as much as possible. So you're taking yourself out of the loop more than you are with just like a prompt. That way you can actually scale yourself. Where I think prompting kind of got hard is you're kind of constantly in the loop and you're not really feeling the gains from what you get from agentic.

**Aakash Gupta** (00:05:39)

Amazing. So what do we do next with this research contractor agent?

**Tyler Folkman** (00:05:42)

Yeah, so it's off, it's doing its thing. It's actually gonna report back when it finishes. I believe it made it in, let's see, right here, Customer Research. So if I click this, it's actually doing research and drafting some thoughts for me, which isn't really the point yet And to kind of show what I was thinking outside of Herder with Loops, one of the things I was super interested in is like, can I use Loops or Agents to help me prepare for this podcast, right? Like that's the most meta thing I could possibly do. So I pointed at like a bunch of stuff And so what I'm doing actually is kicking off a predefined skill or agent that I've built that knows the things I want to talk about. We'll then kind of walk us through some different examples. So one of the things I asked it to do, which makes it a little bit more of an agent loop, and you'll see that some of these things I'm not actually passing, is it's doing a pre-flight check before I record.

**Tyler Folkman** (00:06:40)

Like, am I showing anything sensitive? It's saying, yeah, you might be showing some sensitive stuff. We're okay. Is the repo in a good state? I'm not actually in a sandbox, which I feel okay about, actually. It's got some fallbacks that are a little bit overkill, and then some manual things I'm supposed to do, like did we connect to Riverside and all that other stuff. I did this on purpose to kind of show a few things. One, AI, when you ask it to, can be a great partner to help you do better. Like I wouldn't have thought about half these things and it's kind of forcing me to check them. And I did run this before and I kind of decided I didn't care about like a sandbox. We're okay for this podcast. But every time now, if I ever wanted to use this in the future, that loop is starting off with conditions that I've told it are required for success.

**Tyler Folkman** (00:07:26)

And now it's asking me, is this a rehearsal or is this actually a live run? And we're live. Let's say it's live. Do we want to start at segment one or start where I finish my rehearsal? Let's start from the beginning. And you can see, in my opinion, how this goes beyond kind of prompting and building an actual system to help me prepare or do work in a way that I feel good about and isn't just like AI slop.

**Aakash Gupta** (00:07:50)

And you called it a loop specifically. What makes it a loop?

**Tyler Folkman** (00:07:52)

Yeah, which we'll see in the end here, but one of the things it'll do, assuming it all runs as planned, is towards the end, the way you close that loop is you feedback information into the AI to make this whole system better. And I actually have a little graph we can run through in a minute. It'll pull it up. Looping kind of assumes that you learn and it builds like this flywheel. So any good loop has this end that says, hey, let's review what I did. Let's look at the log of all this back and forth. And how do we take that and improve it? So that's really where the loop comes from. If you hear people talk about looping, it's... This idea of self-improving agents as opposed to a static skill, that the skill could just sit here and be the same forever, or we could take this entire experience and feed it back into the skill and have the AI improve it.

**Aakash Gupta** (00:08:44)

And I guess what I get nervous about there is, is it going to save all the intermediate versions? Am I going to be able to easily revert back if there was some version of it that I liked before?

**Tyler Folkman** (00:08:54)

Yeah, for me, Git is the main way I handle that. So very normal for engineers, a little less normal for product people, though I think that's changing. Git lets you version control these things. So actually, one of the questions that popped up was saying, hey, your Git is unclean, what do you Oh, here he goes, I pulled it up. But I think that that is the right way to think about it, which is you can go back in time, like Git, maybe someone will make something more agentic and there are companies working on this than Git. But with Git, I can kind of commit and move back in time. And those beeps you're hearing is actually telling me I'm done with something. So if you hear those through the podcast, that's how I manage it. And one of the things I'd love to talk about is the importance of having your system so that you can roll back and also adapt to new models.

**Tyler Folkman** (00:09:39)

Because what we're seeing is these loops that you might build or these skills or agents or whatever you want to call them. Different models perform differently and you might go to a better model like Opus 5 or Fable 5 and find that your skill gets worse. And that's kind of a paradox to work through because sometimes you might have forced things that don't need to be forced anymore.

<!-- sponsor -->
**Aakash Gupta** (00:09:59)

Yes, I felt that way about a lot of my core skills. Here's a quick word from our sponsors. I used to think I had a retention problem. Turns out I had a messaging problem. I was sending the same onboarding emails to every new user whether they activated on day one or never logged in again. I had no idea who was slipping or why. Customer.io changed that. Every message I send is now based on The AI agent makes it fast. I describe the campaign I want and it builds the full journey form. Triggers, timing, copy, even And when I want to know how something is performing, I just ask the agent directly and it tells me what to do next. They also have an MCP server, which means AI tools like Claude can see directly what's happening in your Customer.io workspace. Your segments, your customer data, So instead of explaining your business context every time you need help, Claude already knows it.

<!-- sponsor -->
**Aakash Gupta** (00:10:55)

Notion used customer.io to personalize their onboarding and hit nearly 50% open rate. Improved conversion by 6-7% with localized candidates. The idea is simple. Customer.io helps you deliver more impact from every message you send. If you're a PM or founder and your onboarding is still one-size-fits-all, try Customer.io at Customer.io. If you've worked at any company bigger than 30 people, you know this one. The CEO sets strategy. By the time it reaches the people actually doing the work, it goes through three or four layers of translation. Half of it gets lost and nobody finds out until the quarter is over. That's the problem Ariso is built for. This is my operating partner for every manager and team. It connects to where work actually happens, the meetings, the messages, the docs, and it turns

**Tyler Folkman** (00:11:42)

all that fragmented activity into a clear picture of execution.

**Aakash Gupta** (00:11:45)

Managers get real coaching grounded in their team's actual work, not generic advice. Teams stay aligned with strategy as it changes, not as

**Tyler Folkman** (00:11:53)

it was last

**Aakash Gupta** (00:11:53)

quarter. And leaders see where execution is drifting in weeks. Not in the postmortem. One shared memory for the whole org. Everyone finally working from the same picture. If you lead a team, check out oriso.ai. That's A-R-I-S-O dot A-I slash A-A-K-A-S-H. So what are we looking at here?

**Tyler Folkman** (00:12:11)

Yeah. So when I was preparing for this, I started to ask myself some of these questions. What is a loop? How can we visualize it? And working with AI, obviously, this is what I kind of think of is like part one is you kind of fetch your own stuff as much as possible. So you can see in the thing I gave before research X, I didn't actually go do the research for it and give it to it. I said, go figure this out. It does some amount of work. Then there's usually a gate if you can have it, which is how do you validate that that work was correct? This is almost always the most important part. As much as possible, being able to make this deterministic is critical. There is this idea of like LLMS judge where it can decide and sometimes that's necessary. But we're seeing like with this idea of mirror coding that if you have a lot of really solid tests around a piece of code, AI can actually replicate that code pretty agentically.

**Tyler Folkman** (00:12:59)

And the learning from that isn't that like, let's replicate all this code that's already been written. It's AI is really good with clear boundaries and clear definitions of done and success that it can work through. So that's kind of like the part three. And then if you look at how it shapes it, it kind of writes out that thing and then allows it to learn and iterate and improve upon itself, hence making it a loop. If you miss the learning piece, then you're mostly just running what I would call like a skill, which isn't a bad thing. A skill goes to a loop when you feed back the learning so that it continues to improve.

**Aakash Gupta** (00:13:32)

And so is there a step in here like before it creates the next version, I guess, between create the artifact and fetch its own inputs that it is pushing to GitHub or something?

**Tyler Folkman** (00:13:43)

Yeah, exactly. So generally what I would do is if it passes the gate, then you would push a PR to GitHub for a human to review, which if you're just yourself building your own skill, that would be you. You'd kind of look at the decision-making it made, how it wants to update things, and then merge that into the canonical main branch such that you are always using that going forward. But to your point before, have a way back if something needs to go back because you don't like it anymore.

**Aakash Gupta** (00:14:08)

And are you often needing to revert back? How often does that happen?

**Tyler Folkman** (00:14:11)

You know, I tend to with AI not revert back as much anymore because I can often, what I think of as revert forward a little easier, which is to say if I don't like something, I almost tweak it forward as opposed to go back because often it's less of, it's unanimously better in the past. It might be more of, there's this thing that I used to like that I'm not quite getting enough of that I want to tweak the new version with. So I just fix forward.

**Aakash Gupta** (00:14:37)

Okay, awesome. So conceptually, I get it. How does this work in practice?

**Tyler Folkman** (00:14:41)

Yeah, if we kind of go next here, which the AI will kind of walk us through some of the things we do. What we do at JobNimbus to kind of convert this into practice is we try to think of how we develop products. And I think of products pretty holistically. That could be a product for our customer or if we're doing something internally like Using AI to develop our products or write code. How do we think of it as a loop? And if we kind of go back to this, this loop of fetching its input, doing work, the gate, writing an artifact, this all works pretty efficiently if it's code. But what do you do when you need to get like the gate is a human or a customer that doesn't work in your company? And right now it's kind of working on showing this, but how do you really get that into the loop so that it's fast?

**Tyler Folkman** (00:15:27)

Because I think a lot of what companies are finding out is you might have a billion ideas, right? You can generate ideas faster than ever, prototype them, even build them in some cases. But is that something that's valuable and viable for the business? You know, if you go to kind of Marty Kagan's four risks, that's still really hard to figure out. And a lot of times it's because you're missing a clear gate. If we go back to this picture, there's not a clear defined gate that you can quickly iterate on because it's your customer. You can't just constantly lock them in a room and say, hey, do you like this? Do you not like this? And even if you could, you have a bunch of customers. So how do you manage that is... A challenge. And one of the ways we're trying to adapt to that is actually one, being way more customer centric than we've ever been before.

**Tyler Folkman** (00:16:10)

Like using the savings that AI gives us on other things and spending it with the customer. And two, trying to mind anything they've already given us. With the most AI or efficiency in tech we can. So like we have a bunch of recordings and calls and interviews and that might've been a whole team that had to work through that. And now with, you know, Cloud Code, you can point it out all those transcripts, pull stuff out and really more efficiently build that gate to at least filter out some of the bad ideas. And that's sort of what my AI is working on right now. It's actually using our product skill, which the first step is to build a bunch of prototypes. So it's actually going through and building just some random prototypes around payment follow-up Not really anything we're particularly building right now, but as an example, it's going to build me three.

**Tyler Folkman** (00:16:54)

And I just kind of wanted to showcase if you think about that loop is doing something at the first step. While I'm not even doing anything other than talking to you, my AI is doing actually a lot of work to build ideas. The hard part of the loop is going to be validating that it passed the gate.

**Aakash Gupta** (00:17:08)

Wow. So where did this prototype come from? I missed that part.

**Tyler Folkman** (00:17:12)

Yeah, the AI just, it's still working on the, it's going to build three of them, Variant C and B. And just when I said, keep going, it started working on it. So this was built while we were talking.

**Aakash Gupta** (00:17:22)

And what did we do to kick this off? Like, why did it know to start a prototype? Can we look inside that product skill?

**Tyler Folkman** (00:17:27)

Yeah, I go, and that's not in here because I kind of demoed it and I can go find it. And in fact, this is a good example of herder. So if I wanted to spin up my own kind of pane here, I just say new, and then I can go into our product area. Wait, not that one. Really the best one to show would be like forge. And it might be a little bit hard to walk through the exact skills, but if we look at all the things in here, you will see this dot clod. And this .clod has actually got a bunch of skills and commands that let us do a lot of this stuff. So we essentially built our own prototyping system. And by we, I mean the UX team here is awesome, it kind of being at the cutting edge. We've got a bunch of skills that let us do really cool things like create an iOS prototype, an Android one, port components, pull requests, run content.

**Tyler Folkman** (00:18:21)

And there's more outside of this. This is just kind of an example. But really what these skills do And then we can say to the AI, use this skill to generate 10 prototypes to solve this problem for our customers. And then we can start iterating on the feedback loop.

**Aakash Gupta** (00:18:46)

Got it. And I think this is an important point. You're having your domain owners create skills for their specific area. And so the UX team is creating the prototyping skills. And I guess the product team creates the product skills?

**Tyler Folkman** (00:19:01)

Yeah, exactly. And you can see it kicked out two more. So like we tried to get it to spin out variations of an idea. And these ones are pretty basic for speed. But you can see like payment follow up. Then there's like a crew schedule one. There's a different crew board idea. Here's another one about what you might need to know today. Because the idea with AI is how do we actually test a lot of ideas very quickly? Because AI is really good at that without building.

**Aakash Gupta** (00:19:28)

Yeah.

**Tyler Folkman** (00:19:28)

As opposed to building the thing we think is right and then just doing the normal product cycle. If you're mostly using AI to build in production, that's valuable. But man, can you use AI to build prototypes way faster? Instantly, anyone can build a prototype and go talk to a customer about it.

**Aakash Gupta** (00:19:45)

So now that I have these prototypes, what do I do next?

**Tyler Folkman** (00:19:49)

Yeah. So for us, the next step would be, and unfortunately we don't have this skillified quite yet in a great way, but we've injected all of our customer research calls, transcripts into our data warehouse. So you'll actually have an opportunity to synthetically kind of have a customer inspect the prototype through AI. So it will kind of try to think like our customer. We get, you know, for anyone that might be a customer that that's not the highest bar, but it is a good bar to catch some maybe low hanging failures that we missed, right? And the reason we like that is it lets us very constantly. You need a gate. And so we can quickly go from maybe 100 ideas down to the five best ones. And then we start getting with our customers, setting up calls, talking to them, getting into the office with them or on the field so that we go from, Bunch of ideas to some ideas to a few ideas to hopefully the one that we then finally go build and then do A-B testing within production.

**Tyler Folkman** (00:20:46)

But the idea is you lowered the amount of effort until you get more and more validity of your idea from the customer.

**Aakash Gupta** (00:20:54)

And so who would be running these customer outreach? PMs, engineers, designers, anybody can do that? Or how does that work exactly? Because sometimes like the UX research function in particular has like a very strong point of view about who can run those and how they should be run in order to get accurate insights.

**Tyler Folkman** (00:21:11)

One of the things we're working on, and this is newer muscle for us, because traditionally it has been more of a UX product run thing, like most companies, really trying to maintain the standards and do things right. And that's really important. But we're trying to build the muscle of everybody doing this weekly, if possible. In fact, we try to aim for like twice a week. We're not there. We're still working towards that. But If you think about with AI where the new bottlenecks come, this is going to be one of them, like getting in front of customers and talking to them. And if you try to gate that too much, it's not going to scale with the speed of AI. So we're trying to figure out how to really invest in our people such that anyone can start to talk to the customers and know some of the obvious traps of leading the witness or biasing them too much.

**Tyler Folkman** (00:21:59)

The only thing worse than no data is really bad data, so we don't want that. But we really believe it's possible with AI skills and training and really leaning into the people side that we can get anyone to talk to customers and really validate ideas. And that is a new muscle. Like some people have never done this, might be a little uncomfortable, but we think that's okay.

**Aakash Gupta** (00:22:18)

Makes sense. So what has it done next?

**Tyler Folkman** (00:22:20)

And you can see as we go through this, if you don't use Claude as much, it's doing what they call hooks. So it's trying to make sure it does everything that I've asked it to do, essentially. Ah, so now it's showing you kind of a representation of the onboarding that we do here, where, you know, we talked about how we really onboard with AI and want people to have a good experience. And what we found is a lot of having a good experience is having like a clear roadmap. So like stage one is like setting up all of your stuff. Stage two is like understanding the customer market for where your team is, the different strategy and principles. We've got that all codified, the product process, the loops that exist or the skills and actually shipping something. And so these are just some of the high level buckets, We actually can basically build a simple doc that explains the person, their role, what team they're on, who their mentors would be, who they need to connect to.

**Tyler Folkman** (00:23:15)

We feed that to AI. In fact, AI really interviews us for that because we've codified it. And then it generates a whole onboarding flow for them that they can work through. We use linear for our project management, so it creates them a linear board. They come in on day one. And we still talk to them like, don't worry, there's a lot of human elements here. But for when they're kind of on their own and working through what to do, they don't actually have to remember from the conversations. They have clear, hey, you should be with these people. This is your mentor. This is where you start reading about the product strategy and our process. And we found that the onboarding is way more efficient and also just way more enjoyable because you're not spending so much time just trying to get up to speed.

**Aakash Gupta** (00:23:54)

So how do you build an onboarding like this? Basically, it's like a HTML walk me through getting onboarded on my job.

**Tyler Folkman** (00:24:02)

What we found is AI is really good at systematizing existing process. So if your onboarding is already kind of wild and all over the place, the first step is to write down what you want the process to be. Then you can start thinking about where AI can help. So for us, like the key pieces were like setting up your laptop. Okay, cool. We can totally codify that into the onboarding. Setting up meetings with people. Actually, the AI now will just use my calendar and set up the meetings for you. So that's just automated. I just tell it who you need to meet with in the first week and it finds time and sets it up. Another one was customer research in the product, like really understanding the product. So we built a product tutor. We put it into our repo. So when you come in, we say, hey, go here in the terminal, run this skill, and it will actually walk you through the product.

**Tyler Folkman** (00:24:50)

And then if you have questions, you can get answers right there. And so it's going to be different for everybody depending on But if you can write down your system, then it kind of usually becomes pretty clear, okay, this AI could help with, this it can't. Like, talking to customers, we don't want that just happening in docs. We want you out in the field. Talking to customers. So we'll have that being set up, but not AI-ified. Thinking through some of the pros and cons is something we want humans doing. But there's a lot we found, especially in onboarding, that's just process. It's just getting onboarded. It's just kind of being up to speed on everything that's already been done.

**Aakash Gupta** (00:25:29)

And my worry with long documents like these is that AI will create this fancy thing and ultimately you just spend more time editing it. To get it to be accurate than you would have if you had just done like a simpler version yourself. So how do you build this in sort of like the right compounding way?

**Tyler Folkman** (00:25:49)

Yeah, one of the things we're still working through, honestly, is managing that because, yeah, everyone got this like crazy writer that can write anything for them in as much detail. And a lot of companies historically valued that in some way, even if it wasn't explicit. Like if you showed up to a meeting with like a big document, it kind of implied you did a lot of research, right? So as humans, we seem to have associated value with length. And I've got, I can't even tell you the number of documents shot over to me. They're like 10 to 20 pages of AI. And I'm just like, yeah, that's not happening. That's going straight to my AI, which kind of defeats the point, right? So what do you do? What we're thinking about is something should be AI written for AI, in my opinion. Like part of the onboarding that we've done is not for you to read.

**Tyler Folkman** (00:26:37)

It's to give context to the AI to essentially walk you through the things and answer your questions. So if you want to know, like, why did we make this strategic decision and we give all that context to the AI, that's a lot. And if we give it as much as we can, we would never expect a human to read all of that. But then it provides context for the AI to answer. So that's essentially docs for AI. What we've found is now, and this is more of a newer thing, we're leaning towards more visual, more succinct docs for humans. And AI could still help you, but you've got to spend a lot of time as a human really cutting it down, maybe adding more visual components that people wouldn't read but actually understand, like a graph of data or even a picture that would have been really hard because most of us aren't designers can really help.

**Tyler Folkman** (00:27:23)

So now if someone's sending me something that they expect me to read as a human and not have an AI ingest for me, I kind of think of one to three pages as the max. Prefer it comes across as like an HTML and somewhat visual. And then if they really want like a ton of details, I think it's okay to think about AI as kind of an interpreter for that. And then there's a rare case where you actually want the humans to go really deep into like a 10, 20 page document. I think that still exists, but... If the person used AI and not a lot of their own thinking to generate that document, I don't think it's reasonable that the other people will use their own energy to consume the document.

**Aakash Gupta** (00:28:01)

Yeah, that's got to be the most frustrating thing is that sometimes it feels like people are spending roughly as long as it took me to read this as to write it. And nobody wants that.

**Tyler Folkman** (00:28:11)

Nobody does. A lot of times I think you're kind of almost kicking the effort over to another person, right? Like you just keep bouncing the level of effort around where it's like, oh, I need you to do this thing. Okay, I'll have AI do it and then I'll send it back to you. And you're like, okay, I mean, I could have done that. So like, what was the value add?

**Aakash Gupta** (00:28:31)

Exactly. So how do we create like a non-slop loop? Maybe you can help us like program a loop from scratch.

**Tyler Folkman** (00:28:38)

And non-slop is kind of interesting because you hear the word slop thrown around a lot. And I would argue that some AI slop is actually better than human slop that I've seen before AI. And so one thing I like to remind people is before AI, we did not live in a perfect utopia of only good documents and good code running around the universe. A lot of stuff was bad. People don't like to remember, but we used to copy and paste code from Stack Overflow, right? It was not that different than AI, just less efficient. So for me, when I think about writing a good skill, and we could even go through this, go back here, I'll just make a temp directory. So if you're gonna make a skill, honestly, one of the first things you can do And I'll just type here, but I actually think if in the best case, you're going in here and we'll just do skill.md, which is very basic.

**Tyler Folkman** (00:29:34)

It's not including any code. I would write the first pass by hand. There's actually a lot, not a lot, but I've read some papers that suggest that skills authored by humans are often better than the ones authored by AI. And I think the reason for that is you know more and can express more of like what you want this thing to do. And if you offload that to AI, you might tell yourself it's kind of like, you know, e-bikes are kind of popular. People are like, yeah, I got an e-bike, but don't worry, like I still want to get exercise and we'll pedal. Once you get on the e-bike, you're not pedaling. Like that's just the truth for most people. So with AI, once you kind of get on the AI loop, it can be really hard to be like, now I'm going to inject my thinking because the loop's moving so fast, right?

**Tyler Folkman** (00:30:17)

It's like you're on the e-bike and it's moving and it's fun and you're getting the dopamine. It can be a little bit hard to get off that treadmill. So how do you start? I'd start like a human and just be like, help me make good decisions. I specifically struggle and I'm just going to make stuff up with decision fatigue and would love someone to use more what's like a good word for this contrarian thinking but also help push me to make a decision. And you can tell I suck at typing now since AI when enough thinking has been done. I also like to know latest research and have a partner that questions, pushes me, uses the Socratic method, and calls my BS also be succinct. I always add this because, man, if you use Opus 5, the thing likes to talk.

**Aakash Gupta** (00:31:28)

The average length of responses between like Sonnet and Opus 4.6, they're like in one realm and then Opus 5 is just like

**Tyler Folkman** (00:31:37)

so wordy. It's so wordy. It definitely for me regressed. It sounds more like AI than any AI I've used. It's insane.

<!-- sponsor -->
**Aakash Gupta** (00:31:45)

Quick thought experiment for you. Is there anything in this video you should be trying on your own? If there is, try it, take a screenshot, post it on LinkedIn or X and tag me. I'd love to see what you're learning. Now a quick word from our sponsors before we get into the back half of the pod. I used to live in Report Purgatory. Every team had a different number. Every weekly review started with someone reconciling spreadsheets. We stopped hiring more analysts and gave the reconciliation to an AI employee instead. Victor is an AI employee that lives on Slack and Microsoft Teams. It connects to 3000 plus tools your team already uses, ships real deliverables, And every action goes through your team for approval first. It's the closest thing I've seen to a small team running like a much larger one. Let me share three things that Victor does that changed how my team operates.

<!-- sponsor -->
**Aakash Gupta** (00:32:34)

First, Ask Victor has replaced our Monday Second, scheduled tasks run the work that no Nobody wants to remember. Every morning, Victor checks overnight support tickets, drafts replies for the on-call to approve, and escalates anything mentioning churn. Nobody had to ask for it. Finally, spaces ship internal tools in minutes. Ask for a renewals dashboard, Victor builds it. The team can stop opening four tabs to get the same view. So stop chatting with AI and start working with it. Get started at victor.com. There's $100 in free credits with no card required at VIP. Quick question. Does your AI coding tool have a design system or a theme? Because there's a massive difference. A theme is a few hex codes, a font and a logo. You paste it in and your AI built app sort of looks like your brand. Sort of. The buttons are wrong, the spacing is off, and if your engineer tries to use the code, they're rewriting every component from scratch.

<!-- sponsor -->
**Aakash Gupta** (00:33:46)

A design system is your actual component library,

**Tyler Folkman** (00:33:49)

your buttons, your modals, your token definition.

<!-- sponsor -->
**Aakash Gupta** (00:33:52)

The code your engineers already ship with. Bolt.new's design system agent ingests your real system, upload your NPM packages, your CSS, your documentation. The agent builds a complete design system from your actual code. Every project on Bolt.new uses your real components. So when engineering pulls the code, they see their own primary button, their own design tokens, their own architecture, nothing to rewrite. Every other AI tool gives you a costume. Bolt.new gives you the actual uniform. Check it out at bolt.new slash akash. Imagine learning AI product management, AI product strategy, AI product leadership, advanced PM with Claude Code, all from frontier leaders at OpenAI, Anthropic, and Google for less than $10 a day. Actually, you don't have to imagine it. That's exactly what Product Faculty's AI Builder Fellowship gets you. One yearly membership, six live cohorts. Not recorded videos or another content library you never finish. Real live sessions with frontier AI leaders, hands-on AI build labs, executive Insight sessions, capstone projects, unlimited retakes, and continuous access to new programs as the AI landscape evolves.

<!-- sponsor -->
**Aakash Gupta** (00:35:09)

You'll also get every new certification they add while you're a fellow at no extra cost. The goal is simple, help you master Frontier AI skills to become an AI native product builder and operator, not just someone who talks about AI. Purchased separately, these programs are worth more than $19,245. The lowest price certification alone starts at $2,700. But founding members can join the entire fellowship for less than $3,600 per year. That's less than $10 a day. Soon, the price increases to $5,000 a year. So if you're serious about becoming the person your company turns to for AI, this is one of the highest ROI decisions you can make this year. Join the AI Builder Fellowship at productfaculty.com.

**Tyler Folkman** (00:35:53)

And so we can go a lot further on this and there's like a lot more depth to skills. But if I just do that and I, you know, write quit and then the way Claude looks for skills is you can make a dot Claude. And we can move that skill to .clod and we'll just make it decisions.md. Pretty sure it'll find that. So we've got there, you don't see because it's a hidden folder. And then if we go open clod, okay, help me decide whether to invest in robots for roofing. I'm just making stuff up using our decide skill. And so if this worked correctly, you can see that it pulled the skill to side, right? So we're starting the loop off with a skill, which is essentially like something to help us start interacting with an AI in a way that we've kind of defined the boundaries.

**Tyler Folkman** (00:36:43)

And so you can see it's starting with I didn't even say phase zero. It's just kind of inferring that. I need to know what invest means here. So it's using some of that Socratic things I said. It's asking me questions. So it's asking me clarifying questions. In a perfect world, we'd actually just be talking to it. So if you use voice, that's really efficient. But we could talk through and say it is reversible and the blast radius. Well, maybe not reversible now that I think about what I asked it. It is not easily reversible. Man, don't take spelling for me. The blast radius is large and cost of weight small. Let's just throw that in there. I picked this because it's not something we're thinking about right now, so it's cool. Completely just out of nowhere. And it's kind of like a big question. So it's saying one way door, high blast radius, low urgency.

**Tyler Folkman** (00:37:35)

And you'll start to see that it's using tech type words because it's trained on all this corpus of the world. So two way doors, it's thinking about, it's thinking about the blocks, radius, the urgency. That combination is the textbook case for not deciding yet. And I tried to purposely give it something to try to push it in that way. So this doesn't go on forever. So it's like saying, Okay, you probably don't actually decide now who owns this call. And I can say the CEO And then after this, what you would do to close the loop in the most simple way possible, and you can build all this into like systems and go to level 10. But you can say, based on this conversation, how should we improve our skill to be better and more effective next time? So this is kind of where the loop's coming in more manually, where we're saying, hey, we just had a conversation.

**Tyler Folkman** (00:38:26)

You've seen the conversation. I don't know what it's going to recommend because this is a very short conversation to kind of show the point. But it'll come back with something. We will riff with it on that and say, okay, yeah, yeah, yeah. Let's do this. Let's not do that. And if we go back and look at the skill, it will surely be a lot better and a lot more involved in the ways that we failed before. And that's really where the loop happens. And this can be hard to remember. And so what I've seen a lot of people do is build in hooks, which essentially is like before AI closes out the session or when it's closing out the session, it will force a kind of improvement loop. And that's something you can build in claw that's called clawed hooks. So yeah, it's giving me some changes.

**Tyler Folkman** (00:39:09)

And now it's saying, do you want me to apply those changes? And this is where I would say, again, this is the time to get off the AI treadmill. Use your brain. Think about what you actually want to put into it because AI will always have suggestions on how to improve things. It's never not going to say that. And if you always accept what it says, it will become too much. The skill gets too opinionated, too much context, too many tokens, and it kind of dilutes the whole value.

**Aakash Gupta** (00:39:33)

Yeah, it tries to create like mega skills that have like 10 use cases into one.

**Tyler Folkman** (00:39:37)

Which is completely not what, if you look at like the best practices, even from like Anthropic themselves, is like not the way to do it. The AI just really seems to like that.

**Aakash Gupta** (00:39:45)

Wants to solve all the problems with a given skill. So how do we turn this into a loop? Like I got the, basically we had the human gate and then we gave it feedback and then it improved itself. But do we want to set it off to go autonomously on its own now and start making decisions around roping robots or what happens from here?

**Tyler Folkman** (00:40:02)

Yeah, And then you can set this up as a loop and ask me what you need, including a learning hook before... Closing out sessions that learns from the log. Yeah, totally. The one thing Claude actually supports is looping, which if you do slash loop, you'll see it run a prompt or slash command on a recurring interval. So I personally think loops are more than just like a cron job. But one of the things of a loop is you want it to run on a schedule. So you can actually tell Claude, hey, Do this for me or help me know how to do it. And that's one of the best advice I think that I give people is if you don't know how to do something, ask AI. That's not like always the end point, but it can often get you further along and help you kind of at least know the questions to ask.

**Tyler Folkman** (00:40:48)

You said, hey, can we make this a loop? I said, yes. And I told AI to do it. And I know it knows how to do this. So it'll go set it up. It can set up the hook. It can set up the loop. It makes the skill better. And then In a few minutes, we've kind of gone from a one-off kind of prompt skill to a system that loops around one specific thing here, which is like making decisions around robots on roofs. But you could imagine doing that for a lot of things. I know people that use it for like preparing for the day. Every day goes off, does its thing, takes any feedback, updates the loop, and goes back. So you come in with like a fresh set of like, here's what I need to get done today.

**Aakash Gupta** (00:41:24)

Okay, these prototypes are pretty cool. How did it decide on these particular prototypes?

**Tyler Folkman** (00:41:29)

Yeah, so if you look at this demo skill that I've made, and this is where I'm cheating a little bit, the skill has step-by-steps that it's running through. So when I told it to go next, you'll actually see that it's going through here. It's reading the skill. It's then got some prompts, which is saying to create variants for some specific prompts. And these are really basic prompts. Like if we go back to the actual... Things that it generated. What I said is create a crew schedule prototype for a contractor in a product like JobNimbus. So really basic prompt. And you see it working through that. So the demos or the prototypes were not already built. It's building them live. So every time I run this, it's a little different, but the skill itself had the boundaries of this type of prototype, how many to make, and you can see it's variant A, minimal, variant B, full-featured, and C, creative.

**Tyler Folkman** (00:42:22)

And that actually does reflect We do in our internal system where we try to have at least three variants and of different types. One that's a little bit more full, one that's more basic and one that's a little bit more creative. So it's reflecting into more of a demo state, but this is exactly how we do it on our side. We just spend a little bit more time kind of refining the context into the prototype or here I just gave it a few sentences on what to build.

**Aakash Gupta** (00:42:45)

Yup. I have a morning planning loop. What other loops and hooks should PMs be building? Like what's the ideal set of them?

**Tyler Folkman** (00:42:53)

One that I've really valued for myself is customer outreach loop so that it every day or week or whatever the cadence is that makes sense for you. Is actually identifying customers from your data, whether that's like from Pendo or Amplitude or a database that you should be reaching out to. Maybe they've had change in product usage. Maybe they're using a product that you're working on and you can even just have it email them if your company is okay with that and you feel like you've set up the right guardrails. It's a really good way to keep close to the customer without having one of the biggest challenges, which was just the time to go find who to reach out to and send them a message. One of the best loops I think you can do as a PM just to stay close to the customer. Another one I see that comes up a lot is just like a project management loop.

**Tyler Folkman** (00:43:37)

Pull tickets from linear, Jira, whatever you're using, see where they're at, when they were last updated, what risks there are, who's not got work in progress or needs things, and kind of synthesize that down so you're never having to go do all that manually.

**Aakash Gupta** (00:43:50)

So I got two loops. Those both sound brilliant. What other ones do I need? And also, what hooks do I need?

**Tyler Folkman** (00:43:56)

Hooks that I find useful is one I did already talk a little bit about, which is like a post. You can set up a hook when Claude closes a session to do specific things, and that's It's just really valuable. It's storing all the logs on your machine so it can inspect the logs, the things that have gone through. And it's essentially like building out your own kind of evals for your own harness. So one of the things you can do is like build a, hey, this thing Yeah. Yeah. Other hooks are like startup hooks that are useful. So like when it starts up, you might want to know things like what repo you're in, where it's at on the Git, like is it which branch, is it the main branch? And then as you're in the work, you can actually set up tool hooks. So... One that I think a lot of companies have, including us, is if you try to run rm-rf, remove everything, it won't do that.

**Tyler Folkman** (00:45:04)

It'll catch on that hook. As opposed to telling Claude not to delete everything in a prompt, the hook is actually deterministic, and it'll trigger on specific things, like a bash command, and stop that. Or sharing credentials, right? You're not allowed to share credentials, so... We have a hook that if you're trying to do anything that kind of looks like that, it'll stop you or stop Claude more importantly because maybe it thinks it needs to do that. So that's just kind of some of the ways. It adds some determinism into the looping of Claude because Claude itself is a loop, right? It's essentially asking you for something, taking it, iterating, and then coming back to you. And so at each kind of phase of that loop, they let you inject Claude. Code through hooks. So it will always happen. Whereas in a prompt or a skill, you say, never share a password.

**Tyler Folkman** (00:45:49)

Claude can just be like, eh, I didn't read that today. I know we've all experienced this where Claude's like, yeah, you're totally right. You said that and I forgot. Doesn't do a lot of good if all your data got blown out of the water.

**Aakash Gupta** (00:46:01)

So you create a bunch of safety-related hooks, it sounds like. The key loops, just to review, I don't know if I remember them all off the top of my head, but there is one around work in progress and things happening in linear. There's one around customer outreach. There's one around synthesizing support and what feedback you're getting. What other ones should I be thinking about after that?

**Tyler Folkman** (00:46:21)

Yeah, some of the big ones I'm trying to think on the product team that people use. This one's less of a loop and more of, I'd say, a straight skill because it's not necessarily looping as much. But we've tried to start building skills around thinking so that it's less about doing and more about pushing the thinking of the people on the team. So like if you're on doing more of the product work. It's like pushing your thinking on like, did you talk to customers? Did you look at the benchmarks in the industry for these things? Where does the data come from? Did you think about this risk or feasibility? Because we're almost trying to force you off this AI treadmill at certain points. As opposed to just say, hey, Claude, the CEO told me to go build this feature. Can you go do all the research and tell me what to build and why to build?

**Tyler Folkman** (00:47:11)

That's not actually a terrible place to maybe start. But I find that because it's so addicting that you actually just finish there. You get all this stuff back and you're like, I can't possibly go and evaluate this. So I might as well just send it up the chain and see what happens. That's not doing product work. That's more kind of outsourcing your thinking.

**Aakash Gupta** (00:47:32)

That's kind of like career reputation suicide, I feel like, for APM at this point, right? Like, do not ship anything that just AI just, like, developed and start to pass that up the chain. You're just offloading the work to people above you who are even busier than you.

**Tyler Folkman** (00:47:47)

Right. And it's not, like, to be clear, like, I don't see that happening on our team. I think we've had some not, like, go all the chain, but there's been things that may have gotten higher than you'd want to see. And I think it's not because people don't want to do quality work. They're feeling like they have this tool that helps them move faster and so they want to keep moving faster. Because now everyone's using it, people also aren't unaware. If you went back like a year and you were doing this, people maybe were like, holy crap, this guy's insane or this girl's insane. Now people are like, that's just AI. Like, I know. This is not like thoughtful. So think about it. Use AI to help you do research, to push you to think, have it even give you its ideas. But... If you end up in a meeting and your answer is Claude said that or told me that or did this thing, outside of just like normal data gathering, like it's like a code machine or a searching machine for you, that's bad.

**Tyler Folkman** (00:48:38)

And I hear that from time to time. People are like, yeah, Claude said it would take... This long to build this feature. I'm like, whoa, Claude does not know how long it will take. And that was more like six months ago that I would hear that when Claude was newer on the scene, especially for PMs. I'm like, no, Claude does not. You ask Claude how long it'll take six months ago. And it's like, oh, a week. And they'd say, go build it. And it'd be like built.

**Aakash Gupta** (00:49:01)

It was crazy. It would overestimate everything. Okay. So I think I got a good sense of what loops are, what hooks are, when I need to use them. Talk to me a little bit about from product to engineering, what engineering loops should be out there, what engineering hooks should be out there, and then PMs.

**Tyler Folkman** (00:49:24)

Some of the most important loops for engineers right now are quality loops. The thing that people don't talk enough about, in my opinion, is if you ship, let's say, twice as The customer doesn't experience your defect rate. They experience the number of bugs. And so more things go wrong at the same rate. And we've seen that. And so we've really started and tried to invest in quality improvements through loops for engineering, like our standards, checks, automated end-to-end type testing. There's a billion things you can do there. But if you don't have AI working on the quality side, you're going to move faster and your customers will feel like you've gotten worse at building things, even if you didn't. Because they will experience the velocity of more bugs. So that's where I would start. If you're looping, loop on quality for engineers.

**Aakash Gupta** (00:50:37)

And should PMs be pushing PRs? Where does that go till? Should PMs be working on engineering tasks at all?

**Tyler Folkman** (00:50:45)

I think it's definitely appropriate for PMs to work on engineering tasks where it makes sense. Like, let me give an example. I don't know if I'd put a PM working on like our backend billing system and making upgrades to it that could impact people's money flow and all that. There's a lot of like important decisions to be made there that are more architectural. I think it's fairly reasonable to push some front-end changes where we have good decoupling from the back-end, good APIs, where we have good CICD, good quality testing. The more you trust your system to do a lot of that checking, the more I think it's okay for anybody, UX, PM, Eng, to push. And so like I kind of mentioned before, you are at the mercy of your systems before AI, right? Great systems do really well with AI. If you're a company that had really bad systems and relied a lot on humans and slowness to kind of protect you, you don't want PMs coding in there because you barely want probably your engineers coding in there.

**Tyler Folkman** (00:51:41)

But great systems, I think there's no reason PMs can't jump in and help. And the one thing I would be careful of is make sure it's agreed upon in the team because it can create some shadow work for engineers because you want code reviewed. That's the same for any engineer. And I've seen PMs be like, yeah, I just pushed this. I was working on the site. Can someone take a look? And now you've generated maybe hours of work for someone that wasn't planned on. And you might get frustrated because you're like, hey, I'm trying to ship stuff. And they're frustrated because it wasn't like agreed upon that that would be part of their workload. And as an engineering community, this is one of the things we're struggling with is how do we manage the code onslaught? Because you could have AI generate basically infinite code. So how do you do that?

**Tyler Folkman** (00:52:28)

Systems is one thing people are thinking about, but the dirty truth is most companies' engineering systems weren't perfect before, so they're not perfect now. And I tend to push quality, like I said, on the loops, because I almost think that the quality advantage of AI can beat the velocity advantage because it lets you ship safer.

**Aakash Gupta** (00:52:49)

Okay, so that's one part of it, which is PMs doing engineering work. It sounds like PMs shouldn't be trying to become engineers, but if they're doing some front-end changes where, again, they have put in probably more time on it than the reviewer would need to, then it might make sense. What about the other side?

**Tyler Folkman** (00:53:10)

Which is engineers doing Vibe PMing. The failure points of Vibe PMing are interesting because failure points of Vibe engineering can be potentially more obvious. Like you shipped a bug, you created a problem. So anything like what's the failure mode of Vibe PMing? It's It's essentially shipping something that people don't want, right? Or spending time going down a road that's not viable for the business or not feasible or not valuable. If you think about the four risk factors that I often come back to, feasibility engineers already know that we're good. Usability is generally handled more by design. So we can think about that in a minute. So then you've got like, Vibe PMing is more thinking about is it viable for the business, which can they make money? Like, is it a high margin or a margin you need? And is it something people actually want and would pay for, the value side?

**Tyler Folkman** (00:53:57)

So how do you vibe PM? In my opinion, engineers are more empowered than ever to have AI help them mine data, right? To go out into the industry, to see what competitors are doing, to look at calls, to even go find customers that they can talk to, right? You can very easily do all that. The risk is that they do it poorly, right? And you go down a path that doesn't make sense. One of the ways you can kind of mitigate that is speed, which if you have a bunch of ideas, but you're very quick to throw them away, then it's kind of okay, like cool. So I think if you're an engineer thinking about doing more product stuff, one of the advantages you have and where I would suggest starting is you can generally build pretty fast, especially with AI. Get a space where you feel comfortable working That's a two-way door, kind of to use the AI decision.

**Tyler Folkman** (00:54:46)

And go try to do some of the PMing thing. Talk to the business. How do we make money? Talk to the customer. What do they need? Don't overthink it. Get something out there behind a feature flag and get it in front of a customer and talk to them. That is very low risk. It's like the version of shipping a button color change or something for a PM in code. I think there is a vibe PMing. Where I don't want engineering's vibe PMing is like, hey, we need to make a strategic decision on how to invest money that could impact... And so in the same way, I think of engineering, there's this gradient of, hey, we really need best in class, trained product thinking, but not all problems are that way, just as not all problems are like really hard engineering problems. And so if I'm thinking about where I want engineers to lean in, it's like, hey, We wanted to make this change.

**Tyler Folkman** (00:55:45)

We heard customers complain about this thing. It's on the roadmap for us. It's not a huge thing, but we need to kind of figure some of the things out. Can you do that? And the reason that's so powerful is if you as a person can go end to end from, hey, here's a problem to, hey, here's a solution that's making the business money or the customer happy. Again, your leverage has gone up exponentially in the company and the speed to value went up exponentially. All those human bottlenecks internally go away, all those different decision points and like getting people together. That was a de-risking thing, right? We did the triad to de-risk things because things took a while to build. If you can build things instantly. You don't need as much de-risking. You still need some because your customers aren't okay with constant change and giving you feedback is their main job.

**Tyler Folkman** (00:56:37)

But the bar, I do think, has changed because the time to build has gone down, which is why Waterfall existed, right, in manufacturing. It's like the time to create something physical takes a long time. So you spend a lot of time de-risking it up front.

**Aakash Gupta** (00:56:51)

And we placed a lot of emphasis on this episode, too, on de-risking in terms of creating divergent prototypes and putting those in front of synthetic users, putting the best ones in front of users. How important is that for what features do you need to do that and which do you skip that?

**Tyler Folkman** (00:57:08)

Never skip it in my opinion. It's the kind of corollary to engineering is we used to talk about like what your test coverage is. And now my opinion is just be 100%. It's basically free. Like to tell the AI on the unit test side, that's not all tests, but on unit tests to tell AI to write 100% coverage is basically free. Why not do it? Before, we did it because it costs time and energy, and there are good reasons. If you're doing product work, why would you not take 10 minutes and have AI spin up a few different ideas for you to consider, push your thinking a bit, do some synthetic analysis. Don't just take it what it says, but see if it's got some points. You're like, oh, yeah, I didn't think about that. Our customers have said that, and that's the thing I would have missed.

**Tyler Folkman** (00:57:50)

It's just insane to me. I mean, we know from research from, I think, out of Microsoft that a third of the product things we release won't deliver value. Like, no, a third will. So, like, two-thirds of the thing either flat or don't do anything for the business. So, why would you not take some time to basically get more at-bats for free? And that's where, like, the synthetic stuff can be useful. That's also where, like, having really good relationships with your customers is so, so useful. Just get some more reps because AI makes it free. It wasn't free before. You had to have someone design this stuff. If you're newer to your career, maybe you haven't experienced that. It definitely used to take a lot more time.

**Aakash Gupta** (00:58:30)

So we touched on the PM and the engineering loop side of it. The other portion of the triad, of course, is the design. What loops are they building? How did these all come together to

**Tyler Folkman** (00:58:39)

vibe product develop? Biggest loops you'll see on UX is prototyping. Like they were doing a lot of that anyways through like Figma. I, you know, Figma was like a darling in tech and I think that AIs really hurt them because Like claw designs come out. A lot of people I know are kind of vibe coding internal tools like design tools to work with their systems. And so I see design really leaning in heavily on like how do we iterate faster in a way that matches how we think about design and our components. And so you can totally build that into loops. And I think of like, what is vibe design? The one we haven't talked about. It's really like a PM or an engineer spinning up something that's designed in a way that wouldn't make your design team immediately like throw up. And the goal again is like, it's, there's a gradient.

**Tyler Folkman** (00:59:26)

Some things need a lot of design and really be thoughtful. Some things don't. But we used to always go through design for that because they had the skills, the tools. Now with AI, if you have a good design system, like it'll use our component library, use our system. So if you're wanting to make some changes to the front end, like I think you should totally be able to do that. And having your design system know those boundaries is helpful. So when people use it, you're like, yeah, that's something that we feel comfortable non-design experts kind of riffing on. But you'd never learn this if you don't try. And so when I think about the triad, it's really more coming together and what people might be calling like a builder. And I think that coming together is going to take longer than we think. It's not like some people want to act like today everyone's a builder.

**Tyler Folkman** (01:00:10)

Like it takes time. It takes time to learn new skills, to build systems, to do all that stuff. But there are people today. That have found a way to merge design product and engineering into one person themselves with AI that are creating tremendous value, whether it's for a company they're in or their own business. I bet you probably, you know, running your own basically product catalog of podcasts and newsletters. You probably feel like you've merged a lot of skills that you didn't have before. That I think is an exciting future. And we got to get there. We got to train people. We got to build the tools. We got to invest there. It just doesn't come for free. But I really think designers are in a very powerful place where they, more than anyone, often understand the customer, which is the hardest thing to replicate with AI.

**Tyler Folkman** (01:01:01)

AI can code. AI can do the research, but they can't really replicate the customer. So if you have that knowledge and you're willing to think a bit more about the business and how they make money and a bit more about how to build things, I think you can totally go end to end as a designer. And even if you don't do that, your prototypes will become so much better and you can get them moving so much faster because of all these AI tools. So yeah, I'm a huge fan of this idea of like design, product, engineering kind of coming together and people will still have expertise for sure. And that's important, but it's just fun to work across the whole stack on certain problems that make that a reality.

**Aakash Gupta** (01:01:41)

And have you hired any of these full stack product builders? Are you still hiring specialists?

**Tyler Folkman** (01:01:46)

Yeah, we hire a lot of them actually now. So we hosted a hackathon. I think it's the largest hackathon in Utah when we did it. This probably still is because it wasn't that long ago. And we got hundreds of people to show up. And the person, one of the people that won it is now an SVP at our company. And he's a builder, like he built a product with a small team end to end in like two days, like we asked them to build an actual product for our user base. And it's crazy. And then another person that I think got like third, we hired two onto a team. And what we're actually finding is not that skills don't matter, like engineering skills matter, design skills matter, all these things that people learn matter. But if you have the ability to take those skills and then inject AI in the right way and kind of push a little bit maybe outside of your traditional comfort zone, it just opens up a world of opportunity for you to create so much value that wasn't really possible before.

**Tyler Folkman** (01:02:44)

So I'm super pro this builder mentality. Some people take that as like, oh, he doesn't believe skills matter. I think they matter more than ever. But I think because they matter and with AI and systems, you can actually upskill yourself more than ever.

**Aakash Gupta** (01:02:58)

So should every PM designer and engineer be aspiring to upskill themselves into a product builder?

**Tyler Folkman** (01:03:04)

In my opinion, yes, unless you find yourself in a very specialized role. For example, like on engineering, if you're like a security engineer or like you're working at database level research at Google on like how to build the next, you know, high scale, high throughput backend or database, whatever it might be. Those type of specialized roles really need special people with special skills that are going to always be important. A lot of SaaS companies don't have those. They tend to generalize better. And if you can become a product builder, they will love you because they want to solve problems that people will pay for and love using. And often that's not a incredibly complex engineering problem. It's not often a credibly complex design problem or a incredibly complex product problem. It's the merging of all of those things in the right way. That's the hard part.

**Tyler Folkman** (01:04:00)

It's not like Like if you looked at most companies' code base, no one would be like, wow, this is like the Picasso of code. And most things are not designed in a way that we're like, wow, put this on my wall because it's so beautiful. So it's kind of like that super nexus of all those things. And that took three people before, and maybe it takes three people forever. I don't know. But one of my bets is it doesn't for all things going forward. And I mean, I can't predict the future, so I'm not putting money on it, but that's what I would say.

**Aakash Gupta** (01:04:29)

So what's amazing is how quickly you ramped up on all of this, even at the C-suite level, when you probably have to spend 90% of your time in meetings and with stakeholders and those kind of things. So for the other leaders out there, how do you ramp up? How do you personally find the right time to do this, build this skill set? Because if you're going to start asking this out of your team, you obviously have to lead by example like you are doing.

**Tyler Folkman** (01:04:53)

Yeah, one of the things that I benefit from is I've always enjoyed tinkering, so I spend a lot of my free time outside of work doing stuff, so that helps, like I won't lie. Spending extra time learning is always a good thing. The thing that I think we've done that's actually been really good and our CEO really pioneered this was we don't – we're in person Tuesday through Thursday, and what we've done on Monday and Friday, which is remote, is we really – Discourage meetings. And it's actually the first place I've worked at that's done this somewhat well. So usually on Monday and Fridays, I don't have any meetings, which, you know, my team's like almost 100 people. So that's like not a bad place to be if you're leading a team of like any amount of size where usually you're just moving through meetings. So let me tell you, if you get in a room for eight hours with a lot of time and AI and a lot of things you want to learn and explore, you can do a lot of damage.

**Tyler Folkman** (01:05:45)

It's really... Cutting that time into your schedule. So most people don't have that luxury or that culture. What I would recommend is treat it as important to your role and to the adoption of these tools. Saying it is shown. I mean, a lot of companies are doing research on this, like McKenzie saying things like use AI. It doesn't do nearly as much, if anything, versus this is how I'm using AI. And if that's what you need to accomplish in your role, the best thing you can do is use it and show the team you're using it. And then you start to learn, too, where the failure modes are. Because often... High level leaders can talk about things that they read on like X or probably your newsletter. Like, hey, they're talking to this guy, Tyler, and he said, everyone's building. Why aren't we building? Right. And there's just so much nuance, even what I'm saying about how we did this, the pain, what we're still learning.

**Tyler Folkman** (01:06:34)

You really got to experience it yourself to be able to speak to it. I feel like every leader now needs to just carve out some icy tinkering time. And most leaders love it. It's like so fun.

**Aakash Gupta** (01:06:44)

Yeah, it's way more fun than being in meetings all day. This has been amazing. If people want to learn more, if they want to find you online, where do they go?

**Tyler Folkman** (01:06:51)

So, biggest place, Substack. I have a newsletter that I kind of write my tinkering about. It's called The AI Architect. You can find my name, Tyler Folkman, or The AI Architect. I am on LinkedIn. LinkedIn, I feel like has suffered from AI more than most places. So I do post there. I'll be honest, I don't read it as much. So if you engage with me there, it takes me a little bit longer. But yeah, reach out. I love chatting with people. Like one of the things I'm really passionate about is community and bringing together people. They're just having a good time. Like I really love AI, local AI, tinkering, building. So if that's your thing, definitely reach out. And if you're in Utah, like we're always looking for great builders. So JobNimbus is a super fun place to work here.

**Aakash Gupta** (01:07:25)

Sounds like a place where you can actually improve your AI skillset instead of being stuck in meetings, which is another bonus to subscribe to the AI Architect. You will see the link in the show notes or down below in the description. Tyler, thank you for being so generous

**Tyler Folkman** (01:07:39)

with your learnings and time today. Yeah, thanks so much for having me. It was super fun. See you guys in the next episode.

<!-- sponsor -->
**Aakash Gupta** (01:07:43)

I hope you learned as much from today's episode as I did. If you can do one thing that's totally Check that you've left ratings and reviews on those platforms. Check that you're subscribed on YouTube, leave a like and a comment on this video, and then share it with your friends. Trying to make better and better podcasts. After two years, we think we've gotten something pretty good going. So let us know what we can do to make it even better, who else we should interview, and we will put on the best shows we possibly can. Finally, don't forget my offer. For the bundle, you get an entire year of my paid newsletter, plus my favorite AI tools, Bolt Up New, Airtable, Speechify, Descript, Magic Patterns, Linear, Dovetail, Arise, and Mobbin. That's $27,000 worth of value for just $150. So check that out at bundle.akashgu.com if it interests you, and I can't wait to share our next episodes.
