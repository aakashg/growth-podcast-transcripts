---
title: "The AI PM’s Guide to Building AI Agents, with Warp CEO Zach Lloyd"
subtitle: "Warp is adding $1M ARR every 10 days - here's the founder's roadmap to building agents successfully"
date: "2025-09-27"
host: "Aakash Gupta"
guests: ["Zach Lloyd"]
speaker_names: "substack"
substack_url: "https://www.news.aakashg.com/p/zach-lloyd-podcast"
youtube_url: "https://www.youtube.com/watch?v=qMfdPodjfmA"
duration: "00:39:24"
word_count: 6642
source: "Substack episode transcript (aired audio)"
sponsors:
  - name: "Vanta"
    url: "http://vanta.com/aakash"
  - name: "Kameleoon"
    url: "http://www.kameleoon.com/"
  - name: "The AI Evals Course for PMs & Engineers"
    url: "https://maven.com/parlance-labs/evals?promoCode=ag-evlas"
---

**Sponsors:** This episode is brought to you by [Vanta](http://vanta.com/aakash), [Kameleoon](http://www.kameleoon.com/) and [The AI Evals Course for PMs & Engineers](https://maven.com/parlance-labs/evals?promoCode=ag-evlas).

# The AI PM’s Guide to Building AI Agents, with Warp CEO Zach Lloyd

*Warp is adding $1M ARR every 10 days - here's the founder's roadmap to building agents successfully*

**Aakash Gupta** (00:00:00)

Warp is adding 1 million ARR every 10 days.

**Zach Lloyd** (00:00:04)

The rough size of our user base, which is I think as of this month, there'll be close to

**Aakash Gupta** (00:00:08)

700,000 active developers who are using Warp. AI agents and specifically AI coding agents are the number one trend in product development right now.

**Zach Lloyd** (00:00:17)

One very, very powerful new primitive, which is intelligence.

**Aakash Gupta** (00:00:20)

How do you build a good agentic product? How do you code well with AI agents? Some people are making tons of money. Most people are getting lost in the shuffle. I'm so excited to share this conversation with CEO

**Zach Lloyd** (00:00:30)

and

**Aakash Gupta** (00:00:31)

founder of Warp, Zach Lloyd.

**Zach Lloyd** (00:00:33)

What's particularly challenging, and you'll see this with Warp and with Claude and Cursor and like everyone is trying to figure out how to price this stuff. What's cool about this is when I go into this, I immediately get into the agent flow. Now I'm asking, I'm like, probably for the first time I'm seeing like, oh, wait a second. Warp can just like use an agent to fix my thing for me. So as I previewed at the beginning,

**Aakash Gupta** (00:00:54)

some people are making money with agents. You guys have figured out how to do it. Others are lost. So who's actually winning and what business model innovations work for agentic products?

**Zach Lloyd** (00:01:04)

The typical SaaS pricing mechanism of a fixed price per seat subscription, I think it doesn't work that well.

**Aakash Gupta** (00:01:12)

Wow, more than 19x growth in a single year. So you're really in that explosion that's happening.

**Zach Lloyd** (00:01:17)

If you are in a business where you are less about like improving productivity, but you have a more measurable outcome where you charge for much closer to the value that's being provided.

**Aakash Gupta** (00:01:29)

How big is work? What revenue and usage numbers can you share with us? Really quickly, I think a crazy stat is that more than 50% of you listening are not subscribed. If you can subscribe on YouTube, follow on Apple or Spotify podcasts, my commitment to you is that we'll continue to make this content better and better. And now on to today's episode. Zach, welcome to the podcast.

**Zach Lloyd** (00:01:57)

Thanks for

**Aakash Gupta** (00:01:58)

having me, Akash.

**Zach Lloyd** (00:01:58)

It's

**Aakash Gupta** (00:01:59)

awesome to be here. How big is Warp? What revenue and usage numbers can you share with us?

**Zach Lloyd** (00:02:06)

So I can share our growth rate. So as you said in the intro, we're adding, it's now over a million dollars in ARR every 10 days, and that's accelerating. And that's up, you know, we just started monetizing Warp. Like, basically, we're you know, close to nothing at the start of the year. And so it's been very, very cool to see the acceleration. And then the other thing I can share is just like the rough size of our, um, of our user base, which is, I think as of this month, there'll be, you know, close to 700,000, uh, active developers who are using warp, which is pretty cool. And that's also growing quite

**Aakash Gupta** (00:02:42)

quickly. Insane numbers and revenue is up 19 X this year.

**Zach Lloyd** (00:02:48)

Yeah. Or more, I think at this point. Yeah.

**Aakash Gupta** (00:02:51)

wow more than 19x growth in a single year so you're really in that explosion that's happening we're seeing it with some other tools similar in the space whether it's lovable or replit what was the turning point for you guys from almost nothing to now this explosion

**Zach Lloyd** (00:03:08)

Yeah, so it really had to do with finding the right interface for AI within the product. And so the history of Warp, just very briefly, is we started off as a re-imagination of the terminal, so of the command line UI. And we spent a lot of time building what we thought was the most usable and accessible and powerful version of just doing command line work. And it turns out that that interface is incredible for doing agentic work. And you started to see that at the beginning of this year with all of these CLI-based agents that have come out, so things like Cloud Code or Gemini CLI. And we had actually, even before those tools came out, started to make it so that instead of using warp as a terminal, you could use it to run agents. But it wasn't until we really went fully in on the agentic features and made them front and center and even repositioned Warp from being a terminal into what we now call an agentic development environment.

**Zach Lloyd** (00:04:10)

And we did that launch in June where we really started seeing the growth accelerate super quickly.

**Aakash Gupta** (00:04:19)

Wow, that's the power of building AI agent products well. You've been a CTO multiple times. You worked at Google for years. So you are very familiar with PMs and founders. For any PM or founder watching in 2025, how critical is understanding agentic AI? Are we at a learn this or get left behind moment?

**Zach Lloyd** (00:04:42)

I think so. I mean, I think it'd be hard for me to imagine... building a product today and not thinking about how you can apply this technology to whatever problem you're solving. I would just be like surprised if there's a problem out there that is a software problem where it wouldn't benefit from some amount of intelligence. And that's like really what I think of as like the thing that's changed is that there's this sort of new primitive available where if you're someone building a product Um, you now, you know, it used to be like, if you're building a product, you could sort of pick like a database or external APIs that you want to rely on, or just like a whole technology stack for building it. And now there's this one very, very powerful new primitive, which is intelligence that you could have in your app.

**Zach Lloyd** (00:05:34)

And so whether you're building a productivity app, you're building a consumer app, uh, you're building something that's much more on like, you know, for helping go to market people, like, I think every kind of app out there at this point would benefit from having agentic features.

**Aakash Gupta** (00:05:50)

So let's get tactical, right?

**Zach Lloyd** (00:05:52)

I

**Aakash Gupta** (00:05:52)

promised our audience we'd reveal how to build good agentic products. Most people are building AI products that feel like gimmicks.

**Zach Lloyd** (00:05:59)

So

**Aakash Gupta** (00:06:00)

what's your framework for identifying where AI agents add value versus where they're just tech for tech's sake?

**Zach Lloyd** (00:06:07)

Yeah, so I think it's like the same fundamentals of product development as if you're building an app in the world before agents apply if you're building with agents. And so you need to start with the problem, in my opinion. So, like, what problem are you trying to solve for a user, for a customer? Yeah. Is it a deep problem? Is it a nice-to-have problem? Once you've kind of identified that there is a problem that you want to solve, and in Warp's case, that problem is like, it takes a ton of time and is very expensive and hard to develop software. It's like a very kind of general problem. But problems like that exist in a ton of different domains. You start with the problem, and then I think you start to explore the solution space. And you need some hypothesis around like, okay, you know, I think that if, you know, I'm trying to solve this problem for some user that if we inserted intelligence in this particular workflow, it might make that workflow faster and that would be useful for people.

**Zach Lloyd** (00:07:13)

And so, like, I'm trying to think of a good hypothetical without just totally focusing on warp. But, like, let's say I'm building a calendaring app or something. It's, like, it's probably useful to have some intelligence with, like, when meetings are scheduled. It's probably useful to have an LLM be able to understand the patterns where you like to work or your coworkers are available and factor that into the scheduling algorithm. And it used to be that for something like that, you would have to code it as an algorithm. And what I mean by that is you would probably set up a bunch of specific rules, like this person likes things in the morning, that person likes meetings in the afternoon, and this person doesn't want a meeting with more than five people or whatever. And what's different these days is you don't necessarily have to write an algorithm.

**Zach Lloyd** (00:08:07)

You can simply provide a bunch of context to an agent, and the agent will... give you an intelligent answer. And so, you know, as you survey, like the space of solutions for whatever problem you're solving, you have this incredibly powerful new way of solving the problems. But you still have to start with like a problem that actually matters.

**Aakash Gupta** (00:08:30)

Walk us through your own development process. We know

**Zach Lloyd** (00:08:32)

that

**Aakash Gupta** (00:08:32)

this was the inflection point, right? How did you decide how to what to make agentic and how to package it in this way?

**Zach Lloyd** (00:08:41)

Yeah, so we actually went through a number of iterations with AI and Warp. I think this is instructive because I think it follows kind of like the market as a whole. So even before LLMs and ChatGPT came out, we actually had some AI features in Warp. We had one that would let you like sort of type in English and in real time we would translate that English into a command. And that's kind of the most obvious way of doing it. So if you're a terminal user, you'll realize it's hard to remember commands. Like, how do I search for files on my computer using a command? And so we're like, okay, well, here's an easy solution to that. You type the command you want. You don't type the task. You type the command, and you're like, what's the command for finding files? And it gives you back this thing that's like find-name.

**Zach Lloyd** (00:09:29)

Like, whatever. And so we started with that. And then when ChatGPT came out, we were like, there's a more general purpose thing that would be useful here where you can just ask an agent questions and get answers. And we're like, we'll make it really easy to provide context from your terminal session. And so we put a chat panel into Warp. And I think this is where a lot of apps started. It's like, well, okay, it's ChatGPT. It's obvious you can have a conversation with it. What's a cool, lightweight integration? We can get this into our app. And so we did a chat panel. And then the more we thought about it and looked at it, we were like, this is not a native integration to the app. And for our case, there's actually like... you know, a much sort of, uh, more native way of integrating the AI.

**Zach Lloyd** (00:10:25)

And this is what I would encourage people to think through, which is the terminal or the command line is already, uh, oriented around, like it's an interface where you tell the computer what you want it to do. And you just tell the computer what you wanted to do in, um, in terminal language and computer language. But with LLMs, it turns out you can actually just tell it what you want it to do in English. And so that was like the big unlock for us from a product standpoint is like, you know, take the native interface of the command line, which is a very powerful interface for like executing things. and just have it execute your English, essentially. And that mindset shift, which we did like a little over a year ago, we actually did it way before all the CLI coding agents, and we actually called it Agent Mode, which has become a very, we were the first to do that, which has become like a kind of standard name for these features.

**Zach Lloyd** (00:11:20)

That was like when we first started getting our initial revenue traction, because people were like, okay, this is cool, I'll tell my computer to do things, And that insight, that like very native way of interacting with AI has been just like this front door to all of this other stuff we can do. Because once you have this, you know, way where you're telling the computer what to do, it becomes a question of like, how do you add then the right tools so the computer can actually do what you're asking it to do? And so for us, at first there was only one kind of tool. So in Warp, if you ask an agent to do something, it could just run terminal commands. And that's actually pretty powerful because terminal commands are very flexible. But since then, we've started to add a whole bunch of other tools.

**Zach Lloyd** (00:12:06)

So it can edit files for you. It can read web pages. It can read files from your file system. But it all took that main thing of, okay, what's the right... entry point in the app to actually interfacing with an agent in a way that feels natural and that's been our our biggest product unlock

**Aakash Gupta** (00:12:26)

i think Talking to a lot of people who are building AI agent products, this is always the thing. There's always this UX challenge around how to deploy the agent correctly for

**Zach Lloyd** (00:12:38)

your

**Aakash Gupta** (00:12:38)

workflow.

**Zach Lloyd** (00:12:39)

So

**Aakash Gupta** (00:12:40)

how would you extract out the learnings you had for a general purpose? How do I solve these UX challenges around agentic products? What is the right process for me to really deliver an agentic experience that feels integrated?

**Zach Lloyd** (00:12:54)

Yeah. Um, great question. I can just think of some other examples that I think are good to maybe like inform this a bit. Um, like there's a, a new set of spreadsheet products that I think are interesting. And so I, I used to work on, uh, I used to lead the engineering for, for Google sheets when I was at Google. And so I've always been, you know, for a long time, not very interested in spreadsheets and the, um, The like, again, the first iteration of AI that I saw in like Google Sheets was like this Gemini button that like sits off in the corner that pops up in a chat panel. And it's like it's almost like don't do that. And and what I what I have seen recently, which I think makes much more sense. is the ability to have AI populate cells. And so you're like taking the like fundamental UX of like what the app was already for, which was like, you know, working with data, working with lists, and you're having the insight that, okay, one of the like, challenging things about working in this interface is either getting data into it, so you can use AI for that, meaning I wanna have a whole column of where the AI is bringing data into it, or it's working with the data that's already in it, and again, you can work with that data by learning a ton of crazy spreadsheet formulas, or what the AI enables is like you to go one level up in abstraction and just say what you want in English.

**Zach Lloyd** (00:14:30)

And so any place where the sort of like prior solution involved expressing something complicated using like some sort of, you know, either spreadsheet formulas or code or like a scheduling algorithm, I think that's where you should be looking for like, okay, is there a native way that I can do this with an agent?

<!-- sponsor -->
**Aakash Gupta** (00:14:53)

Today's episode is brought to you by Vanta. As a founder, you're moving fast toward product market fit, your next round, or your first big enterprise deal. But with AI accelerating how quickly startups build and ship, security expectations are higher earlier than ever. Getting security and compliance right can unlock growth or stall it if you wait too long. With deep integrations and automated workflows built for fast-moving teams, Vanta gets you audit-ready fast and keeps you secure with continuous monitoring as your models, infra, and customers evolve. Fast-scoring startups like LinkChain, Writer, and Cursor trusted Vanta to build a scalable foundation from the start. So go to Vanta.com slash Akash, that's V-A-N-T-A dot com slash A-A-K-A-S-H to save $1,000 and join over 10,000 ambitious companies already scaling with Vanta. Today's episode is brought to you by the experimentation platform Chameleon. Nine out of ten companies that see themselves as industry leaders and expect to grow this year say experimentation is critical to their business.

<!-- sponsor -->
**Aakash Gupta** (00:15:57)

But most companies still fail at it. Why? Because most experiments require too much developer involvement. Chameleon handles experimentation differently. It enables product and growth teams to create and test prototypes in minutes with prompt based experimentation. You describe what you want, Chameleon builds a variation of your webpage, lets you target a cohort of users, choose KPIs, and runs the experiment for you. Prompt-based experimentation makes what used to take days of developer time turn into minutes. Try prompt-based experimentation on your own web apps. Visit chameleon.com slash prompt to join the waitlist. That's K-A-M-E-L-E-O-O-N dot com slash prompt.

**Zach Lloyd** (00:16:38)

And what I would think is, like, not necessarily the right path is the, like, let me put chat in my app. Because, like, you know, I think that chat is, like, like chat GPT has that and the browsers have that. And, you know, Siri is going to have that. And like an overlay of chat is like a very kind of thin differentiator or moat, but something that's very deeply like native to the UI of your app is, which uses intelligence and might not look exactly like chat, but lets a user express their intent in English or in images or in video is a really powerful way of getting the agent natively to help you do whatever your user is trying to do.

**Aakash Gupta** (00:17:26)

And I think this speaks to why AI agents are so powerful, actually, is because they're allowing us to realize the full vision of AI, where we always felt like chat was a limitation on the UX. The agent, you're giving the LLMs tools, you're giving it the ability to plan, think, react.

**Zach Lloyd** (00:17:42)

Yes.

**Aakash Gupta** (00:17:42)

That is allowing you to embed it into your actual normal workflows.

**Zach Lloyd** (00:17:47)

Yeah. I think that's right, too. So another way you can think of it is like, what would you have a human doing for this job? Which is, again, it's a crazy new thought as someone who's developing products, And you could be like, okay, well, if you had a human to assist you or to assist your user in doing the task, what would be the most useful way that the human could do it? And it could be that the human just like sits over your shoulder like a co-pilot and tells you what to do. But I think a lot of times you'd want to put the human to like work. And, you know, agents are kind of those virtual workers where if you can find a way that they can like do the job in your app, that's going to be really powerful. Um, and you can see this, like, uh, I think if you look at the sectors that have the best product market fit right now for agentic products, it's like coding products like warp and it's, uh, where the agent is helping write the code, which is what a person might do.

**Zach Lloyd** (00:18:50)

And it's like customer service products. So companies like, uh, Sierra or Finn or I think Decagon it's like and you're you're literally for the first time ever it's like you can have an agent do something that only a human could do before which you know has like some you know I share concerns about like replacing people's jobs that's not where where, uh, you know, we're not trying to do that, but like as a business owner, I think, um, just having the ability to like, be like, okay, I could have a, something of human, like intelligence, use my tools and help my users. That's really valuable.

**Aakash Gupta** (00:19:29)

So as I previewed at the beginning, some people are making money with agents. You

**Zach Lloyd** (00:19:33)

guys

**Aakash Gupta** (00:19:34)

have figured out how to do it. Others are lost. So who's actually winning and what business model innovations work for agentic products?

**Zach Lloyd** (00:19:42)

Yeah. Great question. So let me think about how to answer this. So I think like, you know, the, the first thing that you want is you want willingness to pay. If you don't have willingness to pay, you're gonna have a problem because these, um, you know, the LLMs cost a lot of money. So I would start with that. The second thing that you're going to want is retention. Um, and so there, you know, we're in a time where I think there's a lot of like people kicking the tires on a lot of different, um, agentic apps. And so, you know, you, you want to make sure you're keeping a revenue you're getting and that you're, you know, on a cohort basis, improving. The third thing is margins. And this is probably the hardest thing if you're at the app layer right now. It's, I think, notoriously hard for agentic coding companies in the sense of, like, just a very expensive service to run.

**Zach Lloyd** (00:20:49)

And what's particularly challenging, and you'll see this with Warp and with... claude and cursor and like everyone is trying to figure out how to price this stuff so like the typical sass pricing mechanism of a fixed price per seat subscription i think it doesn't work that well with agents because um People use these things in kind of highly variable amount. You really want something where as the usage grows, you make more money, not less. So that's like a problem with these fixed price subscriptions, which by the way, Warp has. So we have these fixed price subscriptions. And it's like we're in this awkward position where it's like the more someone uses it, the more it costs us. And so you can end up being in a spot with your business model where you're trying to make money off of like the breakage, like the unused part of the subscription.

**Zach Lloyd** (00:21:54)

And so this kind of stinks. So you wanna, you know, again, it's like we're iterating on this. On the flip side, The consumer expectation is often a fixed-price subscription, and if you do a pure usage-based thing, which is kind of the obvious solution to this, then you end up in this – you know weird place where the consumer is kind of like always like watching their meter and like feeling like i don't want to spend more money on this thing and so this is like the art of it and so right now our kind of best guess on this is like a fixed price subscription plus an overages model that is more usage based um i don't know where it will totally land now There are better ways to do this. If you are in a business where you can, where you are less about improving productivity, but you have a more measurable outcome, especially one where it's an outcome that the agent can do on its own, like resolving a customer service ticket, then you're in a very, very cool spot because you can do something closer to outcome-based pricing where you, you charge for the science much closer to the value that's being provided in the coding world.

**Zach Lloyd** (00:23:22)

It's just really hard to do that. Like, um, you know, you, you know, like lines of code created as a famously horrible proxy for how much value an engineer is creating. And so like, it's really hard to measure. And so you end up, you know, charging based on like, how much people want to use it. And so usage is closer. But yeah, that's like the challenge of pricing. And then there's this other challenge, which I think is really interesting, which is like, where's the value accrue in the stack? And so you have... llm providers um who are so actually just going all the way down you have apps that are paying llm providers that are paying hyperscalers that are paying nvidia it's kind of like how i would look at it uh and so nvidia is doing really quite well uh and like everyone takes some margin and so the question is like who's going to be able to capture the margin.

**Zach Lloyd** (00:24:26)

And like, I think it has to do with where is there going to be differentiated value. And, you know, right now in the coding space, there is differentiated value at the model layer. Like I would say at this very moment in time, probably Anthropic has the strongest models. Although GPT-5 is really quite good and like is competitive. Gemini at the moment, like, they're going to release something. I'm sure it will be competitive. But the more that there's a competitive dynamic at the model layer, the stronger the position of the app providers. The more that an app provider, sorry, the more that a model provider has like uh sort of like a real differentiated advantage in a particular vertical with their model kind of like anthropic encoding uh they sort of get something closer to like you know pricing power and that's a that's a difficult spot to be in so you know i've said this before publicly i'll say it again it's in our best interest that there's like a competitive a model provider layer, even that there would be open source models is really, that are competitive would completely change the dynamic, but even just having like, Something where it's competitive at the layer of G Cloud, AWS, and Azure are competitive.

**Zach Lloyd** (00:25:44)

There's not one cloud hosting provider. That puts enough downward pressure that I think at the app level, you can build something that has differentiated value.

**Aakash Gupta** (00:25:54)

I think the information released a crazy chart, which looked at gross profit. And I don't think they were able to verify all the accounting, but

**Zach Lloyd** (00:26:00)

at

**Aakash Gupta** (00:26:00)

the high level, it was like... Anthropic, 50%, OpenAI, 45%. And as you move more towards the app layer, like a lovable, it almost gets down to like 20%. Is that grok? Do you think that those numbers are probably accurate?

**Zach Lloyd** (00:26:15)

I think that's – yeah, I think that's today's world. I believe that the model providers are taking more margin than the apps built on top of them. But I don't think that that's necessarily a forever thing. I think, like, you know, there's one other dynamic which is at play, which is that – over time, and I think it's something like in the last year, the cost per token at any given level of intelligence has gone down by 100X. It's either 10X or 100X, and I think it's 100X. And so it just depends. If that's the case, again, then there will be value at different layers. If someone's able to maintain a durable lead at the model layer, then I think they're going to get a big portion of the profits, but I, I think it's more likely just honestly, even putting my bias aside that it turns more into like at the model layer, it's all about scale, scale, scale.

**Zach Lloyd** (00:27:13)

And like the margin is like slightly lower. And at the app layer, it's like differentiated value moat. Like, um, you know, do you have, um, you know, switching costs, those types of things that, um, that get you lasting value. But I don't know, it's all, it's changing really fast. Like I think the, like the answer to this question, like a year ago, I was going back and listening to some podcast was like app layer, app layer, app layer, and like models are commodity. And now it's like, I think it's more like model layer, but, but I, I, I would just focus on building something that people find useful, want to pay real money for. And that the important thing is that there's margin somewhere right now. Like if there's no margin in any place in this whole business stack, I would say find a different thing to work on.

**Zach Lloyd** (00:28:03)

And that would be like the Uber and Lyft situation where I think the margins are sort of fundamentally limited by like, well, what do you have to pay? a driver per hour. And like, there's no more efficiency that you're getting out of that. Whereas for us, it's like, you know, the actual, it's a, it's a, it's some combination of software and hardware, but fundamentally it's like efficiency of compute. And that's a thing that historically is like gotten way better over time.

<!-- sponsor -->
**Aakash Gupta** (00:28:31)

Yeah, we've seen it just get way better. That cost per token at that particular intelligence level, that's the most telling. So where is all this heading? What's your most contrarian take about the future of AI agents that other founders would disagree with? Today's episode is brought to you by Amplitude. Building great digital products is hard. You know that better than anyone. Getting teams aligned, measuring what matters, and scaling your product strategy isn't easy. But what if you had a clear framework to guide your next steps? That's exactly what Amplitude built. They studied the best product teams to understand what really drives impact. and turn those insights into the Digital Experience Maturity Assessment. In two minutes, you'll be able to see where your team stands and what you can improve to build better products faster. Click the link in the caption to take the free assessment and get a clear path to product growth.

<!-- sponsor -->
**Aakash Gupta** (00:29:20)

AI evals are one of the most important skills for PMs. And I know you know they matter. The question is, are you doing them right? Most teams are winging it with basic metrics and hoping for the best. Meanwhile, the teams that actually ship reliable AI, they've cracked the code on systematic evaluation. Today's episode is brought to you by the AI evals for engineers and PMs course by Hamil Hussain and Shreya Shankar. This live Maven course will teach you the battle-tested frameworks from Hamil and Shreya, who are the engineers behind GitHub Copilot's evaluation system and 25-plus production AI implementations. Four weeks, live instruction, next cohort starts July 21st. Start shipping AI that actually works. Enroll at maven.com with my code AG-product-growth for over $800 off. That's AG-PRODUCT-GROWTH. Yeah, it's a great question.

**Zach Lloyd** (00:30:26)

I think there's three phases, and I'll speak to the coding world if that's okay. But I bet you this is true in other domains as well. So the first phase was autocomplete. And, like, Cursor crushed it. Like, even before Cursor, there was Copilot, which... was a good product, but frankly, I think it's, I love that a startup came along and was just like, we're going to do this way better. And like, basically like in like literally the difference between cursor and copilot is that cursor suggestions are faster and better. And it's crazy to me that they just like out competed Microsoft on that. Um, but that was, that was phase one. I think we're in phase two right now, which is what I would call interactive agents. And so these are agents where, a person behind a keyboard is saying, do this, do that, make this change for me, solve this, you know, debug this server crash for me.

**Zach Lloyd** (00:31:29)

And it's really like a human orchestrator. And I think, actually, I think we're early in that phase. I don't think that that's like, if you survey most developers in the world, maybe they've tried to do this a little bit. I don't think it's their bread and butter workflow, but I think over the next year, um, the majority of development tasks are gonna start with a prompt, which is a pretty crazy change. Keep in mind, I've been doing this for 20 years, and for 19 of them, when I wanted to build something, I would just open up my code editor and start typing, and now I'm just like, you saw me, I'm literally speaking to warp, which is crazy. And then I think phase three is kind of like real automation of some subset of simpler tasks. And again, I think you'll probably see this pattern in like, in, I don't know, I'm going to say like legal tech, like it's probably right now, like the state of the art legal thing is probably like someone using Harvey and like being like, summarize these documents for me or draft this contract for me.

**Zach Lloyd** (00:32:34)

And there's a person driving it. But I think that the, the, the step that comes after is like, okay, I don't know, lawsuit was filed. Let me, an agent's going to start doing discovery or something like that. Or like, you know, uh, like I think that that will, that will happen when that happens. I don't know what, um, I don't know what it means for knowledge work. Like, uh, I, I don't really believe the timing estimates. So like I listened to a podcast with a couple of folks from Anthropic, um, and they were like, There's not gonna be any knowledge workers in three years or something. I was like, I don't think so. I don't agree with that because I think there's an underestimation of how difficult it is in certain industries to deploy technology. So like, like in healthcare or whatever, I don't think it's going to be all agents.

**Zach Lloyd** (00:33:30)

Um, but I think that you will see in some, um, you know, in some areas of knowledge work specifically at startups and in non-regulated industries, you're going to, it's going to be super disruptive. And I guess that's not a super contrarian take, but like I, I, I, I don't think people get it. For most of the year these days, I'm living in New Mexico, and I don't think most people in my town know what an AI agent is, and I don't think that's going to last for that long.

**Aakash Gupta** (00:34:03)

Yeah, it's actually crazy how low the adoption and awareness of AI agents is for people like you and I who are just living and breathing this. I

**Zach Lloyd** (00:34:13)

asked

**Aakash Gupta** (00:34:13)

PMs, like, how many of you are using an AI agent in your day-to-day work? Which is a little different than developing AI agent products, which is what we're talking about today. But 2% of PMs are using AI agents to improve their work.

**Zach Lloyd** (00:34:25)

Yeah, that's going to change. I don't think... but it's it speaks to two things so one it speaks to like me and you are in some crazy tech bubble where all we talk about all day long is ai agents which is you know it makes sense given what we do but um it also i just think it speaks to like how early we are in the game of like this stuff truly being deployed um but i don't know like i'm i'm I'm not a big hype guy, but I am like, this is a very fundamental, foundational new technology that humanity has discovered and it's gonna change our lives. Even if we don't get whatever AGI or ASI very soon, it's already the power of these models to do really useful stuff is very, very high.

**Aakash Gupta** (00:35:22)

Yeah, I wasn't sure, like, as a content trend, I had hopped on many different content trends over my content writing journey, whether it was crypto or NFPs or metaverse, after having gotten burned by all of those. AI is another one of those. But it's obviously proven itself not to be.

**Zach Lloyd** (00:35:41)

It's not.

**Aakash Gupta** (00:35:44)

A lot of PMs are now sold on this. They've watched, they've listened to us for an hour. For a PM who wants to skill up,

**Zach Lloyd** (00:35:51)

like,

**Aakash Gupta** (00:35:52)

they want to build like a 90 day roadmap to get better at building agentic develop agentic products. What should they do?

**Zach Lloyd** (00:35:59)

So first of all, they should like get hands on in a tool. Um, I mean, obviously I'm biased towards warp and warp is great for this, but like it doesn't have to be warp. Um, you will be amazed what you can do by simply telling, uh, a tool to do it. And so a really cool way of doing this is to like, you know, instead of writing a PRD for your next thing that you are, you know, product managing, or maybe there's a thing that you think the team should work on and people aren't even bought in, maybe build it or build like a simple version of it or a lo-fi version of it. Um, we've had this happen on our team a bunch, uh, with our designer, who's awesome. And like, there have been times where we were like, we were like, you know what, building that thing is going to be such a pain in the ass.

**Zach Lloyd** (00:36:54)

We're not going to build it right now. And this was like, We wanted to build a better natural language classifier in Warp, which is not a simple thing to build. And our designer, he knows how to code a little. I don't think he'd be offended if I said that. He's not an expert coder, but he was like... you know what? He's like fearless. He's like, I'm going to sit there with warp and I'm going to like do it, do it, do it until I have a prototype version of it that I can prove to the engineering team can actually be better than what we currently have. And he did it and it was crazy. And so it's such a like empowering thing that like my first step would be like, try and build something with the technology. The other reason to do that is like, It will give you a feel for what is and isn't possible, which will inform the types of features that you are advocating for people to build.

**Zach Lloyd** (00:37:56)

Meaning you want to build a really, really good instinct around how good are these models, for instance. What can agents do? Can they actually... you know, organize your calendar or are they going to do some really stupid stuff? And like the way that you can get that feel is by using them in a very interactive context in your day to day. So I highly recommend that.

**Aakash Gupta** (00:38:18)

Couldn't endorse that advice anymore. This has been a masterclass. Thank you so, so much, Zach.

**Zach Lloyd** (00:38:26)

Thank you for having me, Akash. This was really, really awesome and really fun to come on. So thanks again.

**Aakash Gupta** (00:38:33)

All right, everybody. Agentic AI, you have me saying it, is the number one trend right now that you need to learn as a product manager. Warp is proof. They're adding 1 million ARR every 10 days. We have made the playbooks public in this episode. Go act on this. Like and subscribe for more complete courses on AI product development, and we'll see you in the next one.

**Zach Lloyd** (00:38:56)

Amazing. Thank you.

**Aakash Gupta** (00:38:58)

I really hope you guys enjoyed that episode. It would mean a ton to me and the team if you could please subscribe on YouTube, follow on Apple and Spotify podcasts, and leave a rating and review. Those ratings and reviews really help grow the show and help other people discover the show. And they help fund the production so that we can do bigger and better productions. Can't wait to share the next episode with you. Until then, see you later.
