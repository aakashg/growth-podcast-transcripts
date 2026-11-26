---
title: "n8n CEO: Why we aren’t dead, how to build great AI products, and what I look for in an AI PM"
subtitle: "Do you even need n8n anymore?"
date: "2026-10-05"
host: "Aakash Gupta"
guests: ["Jan Oberhauser"]
speaker_names: "substack"
substack_url: "https://www.news.aakashg.com/p/n8n-vs-claude-code"
youtube_url: "https://www.youtube.com/watch?v=PkoX6R5sn8Y"
duration: "01:09:05"
word_count: 12379
source: "Substack episode transcript (aired audio)"
sponsors:
  - name: "Customer.io"
    url: "http://customer.io/productgrowth"
  - name: "Kameleoon"
    url: "https://www.kameleoon.com"
  - name: "Bolt"
    url: "https://bolt.new/solutions/product-manager?utm_source=Promoted&utm_medium=email&utm_campaign=aakash-product-growth"
  - name: "Jira Product Discovery"
    url: "https://www.atlassian.com/software/jira/product-discovery"
---

**Sponsors:** This episode is brought to you by [Customer.io](http://customer.io/productgrowth), [Kameleoon](https://www.kameleoon.com), [Bolt](https://bolt.new/solutions/product-manager?utm_source=Promoted&utm_medium=email&utm_campaign=aakash-product-growth) and [Jira Product Discovery](https://www.atlassian.com/software/jira/product-discovery).

# n8n CEO: Why we aren’t dead, how to build great AI products, and what I look for in an AI PM

*Do you even need n8n anymore?*

**Jan Oberhauser** (00:00:00)

Meet Jan Oberhase, the CEO and founder of NNN, which was just

**Aakash Gupta** (00:00:15)

If you want to build something

**Jan Oberhauser** (00:00:19)

that's reliable, audible, and you can pass to your teammates, you really need N8N. This tweet went viral

**Aakash Gupta** (00:00:26)

from John Ennis. Remember N8N? Went irrelevant pretty quickly, huh? Do you need N8N anymore?

**Jan Oberhauser** (00:00:33)

I think we have been called dead probably a thousand times. I don't remember half of the things that killed us over the years.

<!-- sponsor -->
**Aakash Gupta** (00:00:39)

You guys actually existed before ChatGPT and you talked about in a podcast how you said you were scared a little bit. N8N was literally the hottest AI tool in the world in 2025. Now people are declaring you all dead. Before we get into today's show, please take a second to check that you're subscribed on YouTube and following on Apple and Spotify podcasts. If you want access to all of my favorite AI tools, I've gotten them to give you an entire year of their paid plans. Check out bundle.akashg.com for an entire year of Bolt.new, Airtable, Speechify, Descript, Magic Patterns, Linear, Dovetail, Arise, and Mobbin.

**Jan Oberhauser** (00:01:31)

And now into today's show.

**Aakash Gupta** (00:01:33)

N8N was the hottest tool in my newsletter last year. I wrote about it over 25 times. You can use it to learn the basics of AI like rag and fine tuning. You can use it to automate your workflows. You can use it Today we have on Jan Oberhauser, the CEO and founder of N8N. We're going to get to the bottom of what can What can N8N do that Claude Code and Cowork can't? What is the role for N8N this year in 2026 and 2027? How should you think about using N8N versus these other tools? We'll also talk about how They build product at N8N, what their new latest metrics are, and much more. Jan, thanks for being on the podcast.

**Jan Oberhauser** (00:02:25)

Thanks for having me. Excited to be here. So N8N was literally the hottest AI tool in the world in 2025.

**Aakash Gupta** (00:02:32)

Now people are declaring you all dead. I looked at the Google search trends and there might be something behind it if you look at these trends here. Then this tweet went viral from John Ennis. Remember N8N? Went irrelevant pretty quickly, huh? Do you need N8N anymore? There's a lot to unpack there.

**Jan Oberhauser** (00:02:51)

I think first, probably important to call out that we, I think we have been called dead probably a thousand times. I don't remember half of the things that killed us over the years. We're still here. So I think that probably doesn't hold that too. Also quite exciting, quite interesting. I think if you check out half of the other tools out there and type into Google Trends, I think you see very similar trajectories. I think it's just there's obviously a hype cycle where it gets a bit overhyped and then it kind of goes into this kind of more normal framing again. I think that's also where we are with the most products there. But yeah, I think my first thing is to talk a little bit more about Cloud Code and other ones. I think it's an amazing tool and really deserves to be out there. But I think the most important thing is like NNN and Cloud Code are very, very different products.

**Jan Oberhauser** (00:03:33)

It's like you need both in the end. Cloud Code is more like the genetic tool. It runs entropic models in your terminal. And at end, you can see more this kind of orchestration there that really connects your tools, your LLMs, your data sources, and it offers you this kind of visual canvas For systems to really run reliably and securely. This is especially important for business critical use cases where technical and non-technical people really collaborate. I generally think it's also more important than ever for this, especially business critical use cases. Where reliability, security, and audibility really matters. Where we want to be 100% sure that you know what is running, like you can inspect what's running, you can see what did run. Where you cannot just rely on it's working 95% of the time, It has to be 100% sure that it really works. And I think that's again where our visual canvas kind of really shines because it shows exactly how it works, what it's done.

**Jan Oberhauser** (00:04:30)

And also when you work with other people, they kind of talk about what is actually running. Like if you have something like a cloud code, it generates literally 10,000 lines of code that nobody can inspect and nobody knows if it's actually doing the right thing. Also do we see actually a lot of people that use it together, like they're very often prototyped with cloud code because Again, you can get something started very, very fast, but then actually kind of migrated afterwards to something like NNN for the reasons that I already mentioned again, especially for the audibility. When you want to handle like large or complex data processing pipelines, they want to be like able to kind of more precisely define what actually should happen. And also self-hostability really matters because like people care more and more about data privacy and security. And also one important thing to be aware of, actually, multiple of the model companies are using Aniden as well.

**Jan Oberhauser** (00:05:24)

And I think that also makes sense because in the end you want to use the right tool for the use case. And actually using us for things like security or compliance use cases, because that's again where we really shine. And also if you look like in our stats online, you still see like crazy growth, like we cross. 200,000 GitHub stars recently. We have one and a half million active users. We have over 1,200 enterprise customers. And I'm not talking about enterprises using NNN. I'm talking about 1,200 enterprise customers using our enterprise solution out there. We have 300 ambassadors out there. There's literally one NNN community event worldwide every day. Like in September alone, we have over 50 events happening worldwide in a single month. We increased our revenues 10X over the last year, I think the median number The number of enterprise instance users more than doubled over the last month.

**Jan Oberhauser** (00:06:15)

So definitely we still see a lot of growth. And I think one last thing to probably call out, I think there's still two very critical things that kind of made me very I'm very confident about the future of NNN. One is the kind of model flexibility. It's like what people really care more and more about is kind of being able to switch models for the simple reason, because new models appear literally daily and all of them have different capabilities, all of them have different People really value kind of this, this flexibility of NNN to kind of really use the right model for your use case. And we see generally kind of models and kind of intelligence being more and more commoditized. And this again means that the value kind of shits more and The other thing is also like when you want to kind of connect multiple models together.

**Jan Oberhauser** (00:07:00)

Again, I say, hey, maybe you want to use for X use case, I want an OpenAI model or for that use case, I want to use an entropic one or here I want to use an open source one. And the last one is really this kind of the community and accessibility. We talked about the hype cycle before and obviously NN started with the kind of very early adopters. We talked about this like 0.1% of these people and now we are kind of moving more into this kind of 99%. And who are like moving away from this early adopters, but really the people that actually want to get things done, that we kind of lower the entry barrier more and more. We just really make sure that this technology we can only build within it, but literally anybody who can use a computer. That's literally our mission is defined to give everybody who uses a computer and tech superpowers.

**Jan Oberhauser** (00:07:44)

And that's what we're thriving for these days. And again, it just really feels like it's just getting started. There's so much opportunity out there. So I'm really excited.

**Aakash Gupta** (00:07:52)

Wow. So I'm going to be paying attention when you show this to us in a little bit around privacy, security, auditability, reliability, to really understand what those words mean. Because I feel like sometimes when we hear those words in abstract, it's hard to really understand what that means in the product. So I'm going to be on the lookout for that. But I want to Dig in a little bit more on this detail around specifically the rise of Cloud Cowork and Cloud Code. I had on the founder of Lindy, who I used Lindy personally for some of the similar things I would use N8N for, like automating agentic workflows. He admitted Cloud Cowork had a really significant impact on their business. Did Cloud Cowork, Cloud Code, the rise of Codex have a noticeable impact on N8N's business?

**Jan Oberhauser** (00:08:37)

In the end, going back to the things where we got killed, I think that at some point, OpenAI launched their own agent builder. I think the best week ever is when we got killed by them. I think the nice thing And what I'm thinking about all of those opportunities is that people talk about it more and see more opportunity. And so, yeah, that's, that was quite exciting. And we definitely, I think every company these days like, and I think people again hype things up and, and they see that the future of those products, I think what we definitely What we're seeing is where the use cases change. I think a lot of the use cases in the past is where people started to use end and end for this personal use case. They say, hey, again, write me an email summary. And what's changing more and more is, again, that people say, hey, these users cases are great and I need them, but where they really use end and end more is for those kind of business-critical use cases.

**Jan Oberhauser** (00:09:31)

And that's definitely probably the biggest shift we are seeing there.

**Aakash Gupta** (00:09:34)

So I was trying to find some numbers on 8-8-N. Just in May, you guys announced your strategic investment from SAP, where you mentioned you had hit a $5.2 billion valuation. Startup Riders earlier this year put you at $100 million ARR. You just had mentioned that you guys had 10X'd your ARR over the last year. What can you tell us about your users and revenue now?

**Jan Oberhauser** (00:09:59)

Feel free to break any news. I used to think I had a retention problem. Turns out I had a messaging problem. I was sending the same onboarding

**Aakash Gupta** (00:10:25)

Emails to every new user, whether they activated on day one or never logged in again. I had no idea who was slipping or why. Customer.io changed that. Every message I send is now based on what users actually do in the product. Someone hits a key activation moment, they get nudged to the next one. If someone goes quiet, they get a different path entirely. Their AI agent makes it fast. I describe the campaign I want and it builds the full journey for me. Triggers, timing, copy, even branching logic. And when I want to know how something is performing, I just ask the agent directly and it tells me They also have an MCP server, which means AI tools like Claude can see directly what's happening in your Customer.io workspace. Your segments, your customer data, your attribution, all of it. So instead of explaining your business context every time you need help, Claude already knows it.

**Aakash Gupta** (00:11:10)

Notion used Customer.io to personalize their onboarding and hit nearly 50% open rate, improved conversion by 6% to 7% with localized campaigns, and pushed open rates up another 20% through A-B testing. The idea is simple. Customer.io helps you deliver more impact from every message you send. If you're a PM or founder and your onboarding is still one size fits all, try Customer.io at

**Jan Oberhauser** (00:11:33)

Customer.io.

<!-- sponsor -->
**Aakash Gupta** (00:11:34)

Today's episode is brought to you by the experimentation platform Chameleon. Nine out of 10 companies that see themselves as industry leaders and expect to grow this year say experimentation is critical to their business, but most companies still fail at it. Why? Because most experiments require too much developer involvement. Chameleon handles experimentation differently. It enables product and growth teams to create and test prototypes in minutes with prompt-based experimentation. You describe what you want, Chameleon builds a variation of your webpage, lets you target a cohort of users, choose KPIs, and runs the experiment for you. Prompt-based experimentation makes what used to take days of developer time turn into minutes. Try prompt-based experimentation on your own web apps. Visit chameleon.com slash prompt to join the waitlist. That's K-A-M-E-L-E-O-O-N dot com slash prompt.

**Jan Oberhauser** (00:12:26)

I think you had said 1,200 enterprise accounts? Exactly, yeah. This is well. I think like the exciting thing is definitely kind of just seeing what kind of enterprises are adopting in and in. It's like, again, talk about SAP. Again, they're literally, they're not just made investment that you talked about. With 5.2 billion valuation but also they actually added NNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNN Like setting up anything else without adding billing information, anything else, they can just use this out of the box. So it means like really it kind of makes NNN this kind of AI layer instead of SAP where you can really kind of build your agent automations inside of the product. Also like customers like Mercedes, which probably talk about how they're using NNN and how they see the company getting transformed through it. I think this is the really exciting things like I think a lot of the numbers people are showing, a lot of that is a lot of hype, but actually it's an interesting thing when you actually see real usage of a product and especially really delivering real ROI.

**Jan Oberhauser** (00:13:32)

Because I think like people like in the past like Webny was great because like Webny was very close to actually also kind of real value. But I think there's a lot of decoupling happened there. And I think what our customers see very strongly is that we really deliver a real ROI for them. It's like they're not just burning money. They actually see that getting something back there. I think why that is happening is I think another thing that's maybe important to call out about end-at-end is this kind of combination of AI with deterministic logic and human error loop. Like, I mean, we talked about it before. AI is amazing. It offers so many possibilities, but at the same time, it's not a solution for everything. What you really want is kind of... Kind of link AI with deterministic logic, because again, it's much cheaper to use, so simply if it's much faster and it's 100% reliable.

**Jan Oberhauser** (00:14:21)

And then you still need human in the loop. It's also something again, I'll demo you later, because how it works instead of end at end, because for certain use cases, you always want to make sure there is like a human still in the loop. Again, I think that is probably the things people should look out on LinkedIn, like not just the numbers that actually share, but actually the real users behind it and the ROI, it gets delivered for those customers.

**Aakash Gupta** (00:14:43)

So, I asked Claude to go through my newsletter archive and it said I had written about NADM 25 times in the last 12 months, which surprised even me. It also found that when I did my AI tool ranking a couple months back, we put it in the A tier, above Zapier and Make. Now my audience, I've been spending a lot of time talking about PM operating systems in Cloud Code. So what they typically do is, you know, they would open Cloud Code, connect some MCP servers and have a working agent in a couple minutes. What does N8N do for that person that they can't do themselves?

**Jan Oberhauser** (00:15:21)

So actually I think it's probably easier to simply show you how it works. This is the starting screen for all users right now. I think maybe the first important thing to call out there is like what you see here is our AI assistant, which the idea about it is to kind of, I talked about before that what we're looking for is kind of really give everyone who uses their computer technical superpowers to really kind of lower the entry barrier. And that's exactly what it's doing here. Like you can do the same thing you can do in a cloud code. You can just describe literally what you want to get built and it's going to build it for you. But actually I have something prepared but before I show you how it got built and maybe show you the outcome and to give you a better understanding how anything looks like and how it feels like.

**Jan Oberhauser** (00:16:02)

Here you can see an AI assistant which actually works with your Google Calendar and your Google Gmail account. How generally it works is you get as a trigger node something that starts a workflow in this case you have here an agent and it gets a response and as well you have again different AI models it's important to call out Here you have for example we use Claude Sonnet by default. It actually does get used via our own gateway so you don't have to sign up for separate accounts if you don't want to. If you want to you can obviously still use your own one as well. We even have a fallback model like We know this provider is always very reliable, so it's always good to have a fallback in case they don't respond. And then we have a lot of different tools, like in this case here, list emails, you can get a single email, you can write emails, get information from your calendar, and so on.

**Jan Oberhauser** (00:17:03)

Here, you can also see that here we have further actions, like for example, sending an email. That is something I don't want the AR model to do by itself without asking me. So we have here this human loop step. They can define literally like only execute So you can select that tool if you got approval before. You can define how it should be approved and how the output should be, what it displays you. Then they give you a demo like how it would work. In this case, you can use it externally or you can also So you can just say, what is my next call? And now I can also see this audibility piece. You're not just seeing how the whole workflow is built. You can also see how it actually executes. So you can see here the agent did run. Then it kind of used a model.

**Jan Oberhauser** (00:17:50)

It called certain tools here. It also got a memory. And also here you can go through literally each step, what information got sent in and what information came out of it. And you can see here, my next call is actually tomorrow, Thursday at 11 a.m. till 11.30. Then you can say now, for example, please create another meeting with my VP of sales tomorrow at 3 p.m. And now again, you see each node executing. If something goes wrong, you would see it red. Then you can very easily debug and say, hey, I now fixed that one thing. Again, you can see what it's actually doing, how it's executing. And now you can see exactly that. If you go over here, you see now it's waiting here. You can see it's not doing anything further. And now it says, I'm about to create a calendar event with a certain information.

**Jan Oberhauser** (00:18:55)

Am I actually allowed to do that? Now I can either cancel it or say add event. If I say add event, it goes in here, actually creates the event, and it's done. I think that is generally how anything works. Obviously, it looks now quite technical. People probably wonder how can I actually create that? Again, that's where the AI system comes in. And I can show you how it was built. Here I can, for example, see The prompt here can generate me a workflow agent, personal projects, you kind of see what it was supposed to be doing. Get emails, archive an email, search for events and so on. It kind of get prompted like similarly like you would be doing in Cloud Code and other solutions. And then it starts thinking, it asks some clarifying questions like which model should be used and something else. And then it actually thought for eight minutes, again, very similar to Cloud Code.

**Jan Oberhauser** (00:19:50)

And after eight minutes, it kind of came back to you with the answer, what it built. And you can see here literally Again, that's the workflow we were just working at right now. What you can also be doing, again, it gives you some more information about digital tools that you used, also again, where you used the approval step, and then you can also kind of make additional adjustments, and maybe that's something else to maybe also demo here, where we maybe just say, hey, that's great, but I, for example, very often want to schedule one-on-ones with my people in the team. So I just tell it, hey, please now extend that workflow, Make sure I can schedule this one-on-one meetings. They should be 30 minutes long. You should add always a Google link. The agenda should always be in the description and I should only pass like what's required.

**Jan Oberhauser** (00:20:38)

And also like it should get information from Google contacts. And now you can see exactly that. Now it's going to keep on thinking for a little bit and then it's going to come back to us. Again, in the meantime, maybe just again, go back up here just to see actually like while it's thinking can still, for example, like interact with the workflow here, you can still ask questions. As well and kind of keep on working and it kind of keeps on working in the background and we can just ask further questions there. And then we can anytime go back here, see what it's doing, trying to see while it's figuring things out in the end. I don't know, it's probably going to take a few minutes. I'm not sure you have enough time. But at the end, what you will see is that it adds additional tools to that workflow.

**Jan Oberhauser** (00:21:25)

It will add, again, another tool that you can get contacts from Google contacts and another additional tool to add actually specific calendar events for my one-on-ones. And I think that is, again, I think it shows the power of anything. And especially, like, if you imagine now this one, I can very easily hand over to somebody else because, like, Like, again, even if you're not technical, you can still at least go in here and kind of very easily understand, hey, actually here is an agent. You can see what is the system prompt actually has been defined. You can see again what model it's using. You can see how they are defined. You can see here it actually creates a draft of an email. You can see what things get auto-defined, like all the things that are simply totally impossible in code because, again, it's just too much output or, again, if it's done 100% by AI, It's a black box.

**Jan Oberhauser** (00:22:20)

It can do the things for you, but you have no reliability that the thing that worked yesterday is still going to be working tomorrow as well. That's again the reason why we are again great for anything where compliance is important or where anything is really business critical for you because you can really rely on those workflows because of the combination again because of AI, but still deterministic logic as well and again human the loop step and so on.

**Aakash Gupta** (00:22:45)

So I want to make sure I define for everybody watching those key terms we talked about. So starting with reliability, one element of reliability you just talked about and you showed us is, hey, Claude, they barely have four nines of uptime right now. You can put a back stop model. If Claude is not available, use this other model. Is there any other component of reliability that people need to make sure they understand?

**Jan Oberhauser** (00:23:10)

There's probably multiple ones. Another one to call out is literally it's running So it means like if you talk about you can actually like edit and can run on your infrastructure you can actually self-host it so if you want to make sure like it's close to your own data like there's no internet problems that can really cause any problems there you can run it there and you know like for example like all the other tools like for example get email tool or anything else is literally The code we created is literally tested and we maintain. So even if the API changes anything like that, literally all we have to do is we change the code one time. It gets changed for everybody. We know it's reliable. A reliable piece of tool that works for everybody and not something that literally any person worldwide has to reimplement every time and certain edge cases are forgotten.

**Jan Oberhauser** (00:24:05)

Like we can really think very deeply about the quality there. On top of obviously we have like this kind of whole platform. They not just again create workflows but you can also deploy them on. So again, like if something goes wrong, you can just have retries, you know, where the data gets stored and so on. I think there's a lot of things where it simply takes out a lot of the worries and the thoughts you normally have to think about when you employ something else or just get code written by another solution for you.

**Aakash Gupta** (00:24:37)

So another word we talked about was auditability. And I think the way I'm seeing it, although I'm curious if this is like technically accurate, is that when you build these things in cloud code, the fundamental sort of unit, the source of truth is, It's a bunch of files that kind of live in some Python scripts, some random markdown. It's kind of like, kind of like built on a brittle house versus here. What we have, I think, and how I experienced the product as a power user is the core is this workflow like editor. And everything is thought of in terms of more stable components, where each of these lines and nodes in the workflow is something that you guys really put your foot behind. It's stable, it is working, and it's something that somebody can see versus just income.

**Jan Oberhauser** (00:25:29)

Exactly. Especially like this audibility piece. I think that again, there are multiple things that like next to what we can see what has been built. Again, it is the workflow itself. Again, you can also see how did it run in the past? Like say, Hey, like here are the last executions built. So you can see literally here step-by-step how did it actually run. Again, it started here, it called an agent, it called those different tools. Again, you can see the information that went in and out of the product. And you can literally identify everything the AI really did for you. Again, with code, you see the input and you see the output of the whole thing. But what really happened in there, you have no idea. Like, why did it take certain decisions? For example, we could now add here, for example, between the output of the agent and the output like an additional node that adds, for example, the tinnistic logic and say, hey, If it outputs like, again, something that's smaller than 50 or larger than 50, do something very differently.

**Jan Oberhauser** (00:26:32)

Like you can be, again, a hundred percent sure it's always doing this. And you can then also, after it's inspect, why did it take a certain path? Because like that number actually was the output. Then it went there. And if it didn't go to a certain thing, you know exactly again how we can debug it and change it. And then you can literally rerun half of the workflow from the data point, from that point in time, and can then get it to the kind of state and the quality you actually require.

**Aakash Gupta** (00:26:58)

So another thing that you had mentioned that's important about N8N is this idea of being able to pass it to somebody. So can you show us like, what is the, if I wanted to give this, let's say I'm a manager and I want to give this to somebody on my team, you should also have this workflow. How would I do that?

**Jan Oberhauser** (00:27:15)

You can literally maybe add a few pieces there. You can literally share your workflow with other people because they just invite them there and then they can access it and kind of change it themselves. Other few other important pieces, you can literally have a version history. You can just kind of see how it changed over time. Again, it means a person can actually go through and kind of see, hey, okay, who made changes and what went on there. You can even have things like, again, publish certain verses where you kind of describe what changed between and similar to Git. Another important one is, actually, where did it go? You can even very easily export them, so you can literally send another person an email, a workflow via email if you want to. And we also have something that's not in this version yet here because I think it's an older version, so I didn't update it, is what we have is kind of review steps.

**Jan Oberhauser** (00:28:06)

You can actually say, hey, I made this change, please review that workflow, see if it does the right thing for you, and then you can approve it and only then it gets, for example, published.

**Aakash Gupta** (00:28:17)

Okay. What is making enterprises like the model companies themselves use it? Here we've shown the email and productivity assistant. I guess for me, I feel like other products could also do this. What are those use cases that N8N is so unique

**Jan Oberhauser** (00:28:34)

Certain ones are, for example, the more important reliability and security is obviously the more it shines. Again, we have definitely quite a few companies using it for use cases like it's a survey of security. Security orchestration meaning like every time an email arrives with an attachment scan it then archive it if there's something is going wrong inform certain people or make something certain get started or anything that relies on Like more sensitive information, it could be employment data or could also be even things like and off boarding employees where you don't want to have anything go wrong because you don't want to have half on boarded employees or you don't want to have even less than half off boarded employees either. We have people using us for DevOps use cases. There's definitely a wide variety, I think, if you think about anything where you really want to be 100% sure that it really gets done and not just half done.

**Jan Oberhauser** (00:29:38)

And so it means more or less anything that is not a private use case that is very often why people normally choose NNN over other solutions.

<!-- sponsor -->
**Aakash Gupta** (00:29:46)

Here's what I did last week that changed how I think about AI coding tools. I built a full internal dashboard in Bolt at noon. Took me about two hours. Looked good, worked well, had all the functionality the team needed. Then I did something you can't do in most AI coding tools. I sent the actual source code to my engineer. In Base44, in Lovable, in most of the tools, the code lives inside the platform. Your engineer can't pull it. They look at your prototype, say cool, and rebuild the whole thing from scratch. Bolt.new is different. The code is pullable. Real, production-grade, front-end code. My engineer opened it, reviewed it, and started building on top of what I'd already made. No rebuild, no start from scratch. The prototype became the product. I use Bolt.new every single day. I built my entire paid cohort platform on it. 75 product managers log into something I made in Bolt.new.

<!-- sponsor -->
**Aakash Gupta** (00:30:34)

Try it yourself, Bolt.new slash A-A-K-A-S-H. That's Bolt.new slash Akash. Today's episode is brought to you by Jira Product Discovery. If you're like most product managers, you're probably in Jira, tracking tickets and managing the backlog. But what about everything that happens before delivery? Jira Product Discovery helps you move your discovery, prioritization, and even road mapping work Out of spreadsheets and into a purpose-built tool designed for product teams, capture insights, prioritize what matters, and create roadmaps you can easily tailor for any audience. And because it's built to work with Jira, everything stays Jira Product Discovery. Build the right thing. Do you know how to take an AI product from idea, to development, to evaluation, to deployment, and eventually to scale? That's exactly what Product Faculty's AIPM certification helps you do. I even took the course myself. You'll learn directly from Rohan Varma, the Product Lead working on Codex at OpenAI.

<!-- sponsor -->
**Aakash Gupta** (00:31:54)

You'll go deep into AI prototyping, evaluations, agents, AI-native workflows, cloud code, openclaw, latency, cost, guardrails, rag, routing, fine-tuning, and production systems. You'll even build your own AI product as your capstone with unlimited one-on-one support. So if you wanna stop just learning AI and actually build AI products that work, join Product Faculty's AIPM certification on Maven. 5,000 plus students have graduated and they have 1,000 plus reviews. Use code AKASH550 to get $550 off your enrollment. I feel like you guys have so much power that sometimes it's almost hard for people to figure out, at least when I talk to them about it, about like, what is the specific thing that I should go do next? So we've showed them the email and productivity assistant. We've given them a preview. This is amazing for security and compliance use cases. If you're a product manager, you've built the email productivity assistant.

<!-- sponsor -->
**Aakash Gupta** (00:32:50)

What is the like second, third, fourth thing you should build in any of them?

**Jan Oberhauser** (00:32:53)

And I think this is probably more a question for the person is like, I think There's a problem with a very hard standard platform like ours because you can do everything. In the end you want to do the thing that will be most impactful for you. In the end you want people to think about what's the thing I'm doing literally every day. What is something where I'm using multiple applications, where I'm very often copy pasting things between applications, where I don't know, maybe I'll get information from one place, put it into like ChatGPT or Cloud and then do something with that, create a PDF report. Anything where you think like, hey, I feel like I'm wasting time, then at least you can get it started for your personal use cases. For kind of company-wide use cases, I think that is very often, again, normally it suggests people to start with something small.

**Jan Oberhauser** (00:33:43)

Like we have a lot of companies that just want to start with something huge. They say, hey, how can I totally transform X? And then they spent literally building and building and building for four weeks. And it's a very hard thing because at some point, if you don't have experience yet, you maybe think things the very wrong way. And I think what they have seen that sometimes workflows that literally tasks contain like an agent, a few other nodes, they're actually very often the most impactful ones. And again, not always do you need actually AI for everything. Again, AI is one tool of very many. Like we have one company that literally used NNN to kind of do password resets of employees. They have a lot of employees, a lot of them forget their passwords regularly and they were locked out for literally hours. They cut down the time immensely and it saves them like literally multiple full-time employees a year in time saved.

**Jan Oberhauser** (00:34:38)

So I think it's not about the craziest one, it's really the one, hey, where can I get started easily? What do I think is the most impactful one? And then build your way up from there. Especially other simple ones are great to kind of show off to other people. You say, look for what I built. See what's possible. I spent literally two hours on that, and that's the impact. They get other people involved. And then a very interesting thing is like, especially in an org, is like the more you talk with other people that actually build, you get other ideas as well. Ah, like I built this. Ah, yeah, that's a very similar use case I have as well. And you adopt it. And on top, we also have our template library online. There's over 10,000 workflows for people there. So you can just go in there, say, hey, I'm using tool X, Y, and Z.

**Jan Oberhauser** (00:35:24)

Or you can say, hey, I'm in sales. You can literally see hundreds of them, workflows and agents other people have built. You can either use them to get inspiration or literally take them simply as they are at your own credentials and you can get started there.

**Aakash Gupta** (00:35:42)

Can you show us the template library and maybe give us some inside information about some of the popular ones and the ones that PMs should be looking out for?

**Jan Oberhauser** (00:35:51)

Here you see the templates page. As mentioned before, you can get started saying, hey, I want to use Google Sheets. And then you see like a lot of, in this case, for example, 4,000 workflows that use Google Sheets. You can then say, hey, I'm in sales. Now you see all the sales use cases if you use a Google Sheet. What we, for example, see very often is a lot of people use also edit-in for web scraping. Just get information from web pages, get information from different data sources in which it in a certain way save it in this case for example to google sheet and then send that information to to Slack or we can go over to remove everything here and go for example marketing maybe actually let's get in IT ops maybe this one interesting ones The last thing about N at N is going back to the reliability piece.

**Jan Oberhauser** (00:36:51)

If something goes wrong, you can get informed in whatever way you want. You can get informed by an email, you can get informed via Telegram. And then here we see like somebody used it for monitoring here, they for example drag, hey, are S&L certificates on my server still up to date? And then it kind of alerts them on Discord, it sends It also to Notion. So there's a million use cases out there as you can see that you can use for literally anything. We definitely see a lot of monitoring use cases in there as well again very often also in combination with the AI because I think that's again where you want to react very fast. The reliability piece again matters where you can say hey again if by default Just inform me and then maybe try to autofix it, then use AI, but you can really kind of very clearly define again the different steps that it should be taken first and then you can Make sure again, again, for example, the informing piece always happens to 100%, but this kind of auto-fixing part with AI, for example, only happens later.

**Jan Oberhauser** (00:38:00)

And again, I think that's, again, one of the things where NN really shines. And I think I just advise anybody to just look through there and kind of get some inspiration of people, what people are actually building within it.

**Aakash Gupta** (00:38:11)

Yes. A lot of scraping use cases. I also have used N&N a lot to teach AI. Like it's a really good place where you can very easily fine tune a model. You can very easily set up a rag system. You can set up a vector database. So if you want to learn the fundamentals of AI, I think it's also really good for that outside of just workflows. So one of the areas we talked about was the ease of use. So can we see how the AI assistant has done on extending our personal productivity workflow?

**Jan Oberhauser** (00:38:39)

Actually, okay, here we see the prompt, see how I thought about it, and then it said extend it here, it actually also asked a question in between, and now we can maybe go into the workflow, we can see on the side, let me extend it actually a bit more, and now you can see how it extended it. So what it actually added now is, for example, this lookup. So it means like it can now look up context on Google. You also can see it actually executed because what it's doing is part of the process already tries to kind of test the workflow for you and runs it. You can also see here this approval for one-on-one. So if you want to book a one-on-one, you can also see here the same thing again. It says I'm about to book a 30-minute one-on-one. It will include a Google link.

**Jan Oberhauser** (00:39:28)

Are you okay if it gets added to the Google Calendar? And only then, again, it does that.

**Aakash Gupta** (00:39:33)

Okay. So it took five or six minutes, it looks like. But in the end, you're going to get an updated workflow. That actually makes sense. That works with your tool. Exactly. So your episode is coming right after Wade Foster, CEO and founder of Zapier. So we have to ask the obligatory question, Zapier versus N8N. What can N8N do that Zapier can't?

**Jan Oberhauser** (00:39:57)

I think the great thing about end-at-end is that we focus from the very beginning about power and flexibility. When you get the most value out of end-at-end is you don't want to be locked You want to start with something simple and then you want to build on top of that and build it up. That shines very strongly because we have this power and flexibility built in. We have things like code nodes where people can fall back to code at any time. Complex agents can be building again it's not just basic agents you can actually add your own memory you can put out you can add outside passes to make sure the output is always a certain format you can have again as I mentioned before you can have different models you can have fallback models you have this human loop steps I think a lot of the things that I think when it becomes A little bit more complex rather than simple use cases.

**Jan Oberhauser** (00:41:04)

Wade is a great guy. I've always enjoyed talking to him. I think Safe is a great product. But again, as I mentioned before, there's always the right use case for the right product. And I think like, especially if it's about where you need power and flexibility and a very deep integration to AI, it's when end at end really, really shines. And again, obviously, I think it's probably worth mentioning, but I think obviously if you want to self-host it and things like that, that is where obviously EnidN is, I guess, where they say, I guess, can compete considering their SaaS solution there.

**Aakash Gupta** (00:41:42)

That's an important differentiator too. So I want to learn more about your guys' growth because you have a pretty fascinating history. We talked about how many times people have called you obsolete. You guys actually existed before ChatGPT. And I think that might have been one of the first times. And you talked about in a podcast how you said you were scared a little bit. But sprinkling AI on top would only give you 10 to 30% growth, not the 10x growth that you guys have been seeing year after year since. How did you make that call? And can you break that down for us a little bit more? What does it mean to sprinkle AI on top versus make it core?

**Jan Oberhauser** (00:42:23)

Sprinkly AI on top is what I see is like somebody tells you add AI and you say, hey, here and add this AI button somewhere, it does something with AI. Where I see again, what we have with it is like really think about like how can we become part of the value chain? How can you really kind of not just add AI to the product, but really kind of make sure people actually build within it. Meaning like when the idea was like how, when people think about if I want to build an agent, like they should be built, want to build an agent within it. So we're actually seeing that you can actually get the real value for people out there and I think the thing is probably when people get asked to add AI to their product or build an AI agent or And like we want to be the solution that kind of helps them to do that because that's where the real value lies and where you can again see a 10% or a 30% growth, but literally like last year we grew literally 10X exactly for that reason because we were part of the value chain and we kind of empowered people and we kind of provided real value for them.

**Aakash Gupta** (00:43:28)

I think a pretty crazy stat you guys released is 80% of workflows on N8N now use AI agents. Obviously that would have been zero at the beginning of 2023. So is that your 2022 users adopting AI? Is this a new crowd? If so, what happened to the old crowd?

**Jan Oberhauser** (00:43:47)

It's actually people adopting. I mentioned before, our users are tinkerers. They're very interested in checking out the latest. And kind of really making their day-to-day more efficient. And obviously AI is the tool to do that. And all of them were super interested in actually adopting AI and kind of really making it part of their daily usage. And I think that's how we became And

**Aakash Gupta** (00:44:23)

how you've grown this thing is very different. The average company doing this type of growth, they would embrace per-seat pricing, they would have lead gen targets. You killed your lead gen target and you refused per-seat pricing. Why?

**Jan Oberhauser** (00:44:37)

The thing is like we are in this very lucky situation that you can think very long term. It's like I think that most AI companies out there, they maybe grow their AR very strongly, but at the same time, they're just losing a lot of money. So it means like you have to kind of show a lot of growth to kind of get more money from investors. But what forces them to kind of really think very short term like how can I get more ARR now to get more money tomorrow and then the whole cycle repeats because of the way and it is built like we are actually Sustainable, like right now, we're actually creating a profit. So it means like we don't rely on investor money anytime soon or at all, if you keep on doing what we're doing right now. Rather, we can think about like what sets us up for success in the long term.

**Jan Oberhauser** (00:45:21)

And I think right now, like being able to kind of just capture a lot of the usage and not think about again, how to increase revenues as fast as possible, but how to really kind of Create the best product out there and how can it create a lot of value for our customers and how can it capture as much as possible of the opportunity out there. That's why it's obviously a very much easier decision for us to do something like that than for many other AI companies out there right now.

**Aakash Gupta** (00:45:49)

So the lead gen and per seat pricing, those are pretty public for anybody who's studied NNN like me. What might be some other metrics you've deleted or a metric you're going to delete that people don't know about?

**Jan Oberhauser** (00:46:00)

Metrics we deleted, maybe I can talk about it. The internal thing we are focusing on very strongly is like, one thing is obviously like what we want to achieve like in certain goals regarding users and AI in the long term. But the other thing is like how we want to kind of build the How do we think edit-end should function? And we set this internal goal like we want to reach a billion users with less than a thousand employees. It means we don't want to grow our headcount. We obviously grow it because we have to, but it's the opposite of what we're interested in. We want to build this very efficient org. The idea behind it is very simple. Organizations come to us to help them to kind of transform the organization to become more efficient, to use AI better, to automate more and so on.

**Jan Oberhauser** (00:46:51)

And if you're not kind of doing it internally and like you're literally hypocrites, like that's horrible. Like I hate nothing more. And especially, I think we cannot do a great job. We can only help them transform if you actually transform internally as well and kind of had our own, learned our own lessons, know what worked, what didn't work, what was impactful, what wasn't impactful. And for that reason, again, we're not talking about like how fast we have grown our headcount over the last years because there's literally nothing we think is... It's a positive thing right now. We're actually doing the opposite where we kind of try to stay as lean as possible and really try to kind of build the organization of the future to again help our customers and our users do exactly the same thing as well. Maybe another thing to point out is like what we're not What we're not caring as much about is like obviously as kind of this freely available product, you have obviously users that pay you and users that don't pay you.

**Jan Oberhauser** (00:47:47)

And we obviously could always kind of, for example, focus on how do we get people that currently don't pay us to use our free version that self-hosts us to our hosted solution that we actually earn revenues. There's nothing we're doing at all because it doesn't matter for us. Like all we care about is that they're using NNN. And we know it, like we're generating value for them at some point, or we work for an organization where they're going to want to pay us at some point in the future, but again, we don't care about if they're paying us right now or not. All the matters for us is then the happy end users, they keep on using us in the long term.

**Aakash Gupta** (00:48:19)

Fascinating. For somebody who was a VP of Growth at Apollo.io, where I was just focused on free-to-paid conversion, free growth, that's very interesting and very different for people who might not realize a way to approach those free users. You mentioned the employees, and I actually wanted to talk about that. I think at some point you had said, You want to be the first billion dollar company under 500 employees. I think your career page puts you at around 160 employees. But LinkedIn, it seems like a bunch of people are wanting to associate themselves with N8N. And you have like over a thousand people listed working at N8N on LinkedIn. So how many people really are working at N8N right now?

**Jan Oberhauser** (00:49:00)

Currently we are around 370 people in the org and we are hiring. We're probably going to be around 500 by end of the year. You're right, that's the reason why the number is so inflated because we obviously have a lot of partners and agencies working with us and they then very often appear Also the other thing you mentioned is our old goal was a billion ERR with less than 500 employees. We changed it for two reasons. First, we did much more on the enterprise side of things and we realized that as long as people As long as the buying side is not done by AI, we cannot do the selling side by AI either. It's still a people game. People don't sign a half a million dollar contract without talking to anybody. So it's going to stay very people heavy for a long time. And the second thing was also that we realized Like I mentioned before, like what matters in the end is for us adoption.

**Jan Oberhauser** (00:49:55)

And they kind of talking about like the, the, the 1 billion EAR was, was not set because we said, Hey, we want to make a lot of money. It was set to kind of, as it's kind of my sort of being like a big impactful organization. But at the same time, it still confused people internally or even externally saying, hey, it's just about money. And we kind of wanted to be very clear saying, hey, it's not about money, it's about adoption. That's why kind of this value switching away from ARR to really actually use this made much more sense for us.

**Aakash Gupta** (00:50:27)

I have one more question about how you guys grow because it really is different from everyone else. Let's say like Whisper. I think they're like a company that I put in your similar category, like AI, they're just taking off like crazy. So they launched their note taker. Their entire focus was viral growth. They even bought like rickshaw ads in Delhi and things like that. You guys have been perceived as much more quiet. Is that like a strategy? Is that your personality? What's going on there?

**Jan Oberhauser** (00:50:57)

Yeah, I think it's probably also part of my personality. I'm not the person that has to be literally anywhere. I'm more the introvert kind. So this kind of things don't come naturally to me and I'm not the person that really has to be anywhere on stage. So I think there's definitely also a component about me there. But generally, like as an org, I think I can be also a European organization. I think we are probably more that kind of Under-promise, over-deliver kind of people. So we don't really are in the business of kind of really kind of buying any kind of viral growth there. Again, like we think more long-term again, like we became not viral because we paid people to talk about us. We became viral last year because we had people being excited about it and then getting a lot of value out of it.

**Jan Oberhauser** (00:51:40)

They wanted to share it. We had people that kind of created their business around and kind of Generated own money like that. And I mean, this obviously kind of makes it even more interested in actually talking about it because it's this nice win-win situation. It's like the more they talk about it, the more visible they are, the more visible they are, the more visible we are, and then obviously they get more contracts. So it's this nice... Pista as well again we had from the very beginning this very strong community focus. I talked already before about again having an event literally every day on the world somewhere about anything that is again this kind of more long-term thinking we know hey like invest in the community is nothing that kind of gives you growth. Tomorrow or next week is again, I think that takes many, many years, but once you have it and once it works, it's amazing.

**Jan Oberhauser** (00:52:27)

And also by now still, like most of the enterprise users actually comes from our community people. Like they literally use it privately. A lot of value out of it that say, hey, I actually work for this huge org, Norma X, whatever, and then I have also a use case there. So I can actually automate things there and then do the first internal use case. Then they get other people excited. We have literally communities inside of Large orgs that are like over a thousand people big and that have their own internal community events inside of large organizations, inside of the system integrators. I think that's just amazing. It's nothing you can, again, do very fast, but I think it is this kind of more long-term sustainable things that, again, worked out very well for us.

**Aakash Gupta** (00:53:09)

Very European indeed. Although if you think about like a lovable or something, they are more viral. So I think there is also a component to your personality and how you have grown this thing. So that's how you've grown this thing, which is just amazing. I want to talk a little bit about product. You said 370 employees. How do you structure your product team?

**Jan Oberhauser** (00:53:29)

Right now we have like squads, which are like between three and five engineers. One to two PMs and one designer. We have a VP of product, underneath we have a director and then we have underneath our PM teams and then there are Engineers report to an engineering leader, again, and designers to theirs. I think that works actually very well for us. We have these very small units that can kind of work very fast and efficiently and kind of get things pushed out quite fast without a lot of the overhead.

**Aakash Gupta** (00:54:04)

When did you hire your first head of product and how did you make that decision?

**Jan Oberhauser** (00:54:10)

We probably hired him around April 2021, so it was around the same time we raised our Series A. Then we had multiple engineers already and I was obviously totally involved in But I also realized it's important to have somebody who has the experience to lead a product or who can spend more time on it, who can go deep on the problems. And I met him and from the very beginning, I think he I mentioned the past NNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNN So what did you hand him and what did you refuse to hand over? Originally, I stayed very close. I was still very involved in the product development side of things. I literally still merged every PR. We reviewed everything that was happening there, but it obviously changed more and more over time. Very early on, we owned the roadmap, but again, we always talked about all the things that were happening I was learning about literally every single feature at the very beginning and discuss things, how we think they should work.

**Jan Oberhauser** (00:55:42)

And again, as the product team grew more and more, actually I became for a lot of the things more removed. I still have, for example, Like for example, check-ins with the design team. We had this case where after at some point they built a feature and they made certain decisions that honestly went against what I thought was the right direction to go in. I realized actually I probably have been too far away from the product at that point in time. And then I said, hey, now actually I have to kind of go back there. We have still to this day, we have regular meetings every week with the design team where they kind of show me what things they're exploring, what things they're thinking about. I can give feedback there. They can hear me what I'm thinking about things. I can get feedback very early on.

**Jan Oberhauser** (00:56:31)

And it just gives me a better idea where everything is going. And just apart from that, obviously, I just want to be very close to it and kind of understand what's going on there. And again, just make sure it's always on the right level. And then there's obviously certain things where it matters less and other things where it's worth to kind of really go a little bit deeper and understand how exactly you're thinking about things and what direction

**Aakash Gupta** (00:56:55)

it's moving. So when a PM is talking to you these days at the CEO level, what are the ways they should be talking to you?

**Jan Oberhauser** (00:57:03)

What are the mistakes they might make? It's like it has to be obviously on the right level where it really matters in the sense of like, it depends what they're coming to me about. Is it about a certain direction they want to be going in? I think that's exactly the right kind of level where it says like, We think we want to go in that direction, we want to explore those things because then very early on I can give feedback, I think it's right or we can obviously say very early on it's not the right direction and can also give feedback there and we don't waste time and But again, everything is always happening very closely with David because he's the product leader. I trust him literally unconditionally. He's just a super smart guy. But I think it's always good to kind of bounce his ideas off.

**Jan Oberhauser** (00:57:49)

Obviously, where it's less helpful very often is if it's obviously just in the detail. I still like the design demos because again that's literally where I want to be in the detail because like I think that is important for me but if the last thing again any senior leader wants if they get involved for every small decision because most of them don't matter And I think like if it's about that, hey, should we put the button here or there or any kind of smaller things that don't really kind of make a substantial difference for the product experience or the opportunity? I think that's probably not what you want to be talking with any senior leader.

**Aakash Gupta** (00:58:23)

100%. So I went and found an opening. For N8N, I wanted to just see what are you guys looking for for your PM? And a couple of things stood out to me when I was looking at this. Obviously, it's a very empowered job. You own the strategy and roadmap, but where I wanted to go was what do you require? Some of the things you talked about here, two to three years on platform, well, that's because it's a platform role.

**Jan Oberhauser** (00:58:50)

You talk a lot about technical depth.

**Aakash Gupta** (00:58:52)

Some of the words we were just defining earlier in this podcast, reliability and scalability trade-offs, holding your own in an architecture discussion. It seems like a very technical role. How technical do you have to be to be a successful PM at N8N or more broadly an AI PM these days?

**Jan Oberhauser** (00:59:13)

Like the experience we made is the more technical the better and honestly almost every role we hired. Like also our designers are very technical and we also expect them to kind of use cloud code, create function demos and just get a good understanding there. So like I think the more technical the better because you just get a I think you can have much more impact. You also kind of understand, especially under recently, our user base was quite technical. So it was even more important than now. And I think also now where again, we talk about power and flexibility, the thing we never want to give up is this power and flexibility that people should never kind of I think technical people are great for that, especially because they really understand very deeply what's possible, how much work is really something we need to do there. Generally, we always look for the rising stars.

**Jan Oberhauser** (01:00:03)

I think that worked very well for us. Also, we look for really passionate builders. One of our values is literally a culture called VR Builders. We want people that are tinkers. We have people that have home automation running at home and get very excited about those things. Because again, they are very close to our users there. And also people that kind of understand what it really means to kind of build something that scales and something that really is again, reliable. Again, that's why we wanted people actually not just build a basic agent, but actually understand, hey, you want to probably go deeper. You also want to think about evaluations. You want to think about how does it scale? How to kind of improve it? How do we kind of make sure it's really reliable? And all of those things. And I think all of those, if you find that this kind of treats in people, which understand, hey, they're not just able to operate very high level, but can also go deeper if they have to, that is normally a very good sign for us.

**Jan Oberhauser** (01:01:01)

And that are good PMs. So again, we found some very amazing ones, but we also had always kind of a hard time finding the kind of more technical PMs out there over the last years.

**Aakash Gupta** (01:01:12)

I keep hearing this from AI CEOs, even less technical products than you that they want, these pretty technical PMs. One thing I don't see on this list is evals. What do you think about evals? It's one of the hottest topics in product. Should PMs... Be owning the evals or at least defining, you know, the golden set. What is the role of evals for PMs at N8N?

**Jan Oberhauser** (01:01:36)

We actually have an own team. It's called the AI Trust Team, which actually owns them. And they literally also have built an internal product around it as well to actually make sure EVOS run the right way like especially like a complex product like NNN where we again where you want to test against and not just a simply input output but we want to see in case for example if NNN like to have the right tool spinning And so on, it becomes even more important actually not just get something that just again works for half the people out there, but we really need something very specific. So again, people have to understand evals very, very deeply and I think actually evals are, I think People talk about them a lot, but people don't really use them as much as they should because I think they're probably not very fun to create.

**Jan Oberhauser** (01:02:25)

They're very hard to create. I think there's definitely still a lot of opportunity in that space as well. And honestly, also still a lot we could be Doing much better at NNN. We also have obviously an eval product in there as well. Like you can create your own evals in NNN. I think they're very valuable. But honestly, I would love if more people would actually ask for them and actually create more evals. Because I think that's, again, when you talk about being able to kind of run things reliably, evals are the way to actually ensure that especially if you want to switch, for example, a model or other things like that, For no matter whatever, it's just a time reason, faster throughput or price or whatever, you need evos to kind of just get very fast a good understanding if the performance is the same way or how we can change the prompts very easily to kind of maybe make it work for those models as well.

**Aakash Gupta** (01:03:13)

So a lot of people who are watching this podcast, they're seeing this role and they're like, I want this role. So if they want this role, I have a two part question. How do they get noticed by N8N? Like what are you looking for to interview people? And then how are you interviewing people?

**Jan Oberhauser** (01:03:32)

Notice, I'm not directly involved at that level, but I think like what's definitely always helpful if you just see people being active in the space, maybe having built something like that already, just understanding what it actually means. Again, especially, again, we talk about them having to be technical. Again, like if you can literally very easily see that again by having built something or just seeing how they kind of present things, how they think through those things, it's definitely very helpful.

**Aakash Gupta** (01:04:02)

And the second part, sorry, the first thing was how they get noticed. And then how do they succeed in the interviews? Like there's so many different types of AIPM interviews these days. What are you guys running? How are you guys separating, you know, the pretenders who just use Cloud Code to show We found that they're really able to go deeper. It feels like they're repeating things they heard online without really understanding what it actually means.

**Jan Oberhauser** (01:04:25)

And I think this happens a lot. Again, by just asking the right questions, we are very lucky in the sense that a lot of the The things that actually become problematic at a certain point, we actually also experience internally already. So we know what kind of questions we can ask and what kind of answers to expect there, which actually kind of A person would answer if they actually thought about a problem more deeply versus the person that actually just repeats what they heard and it seems like it sounds good but actually there is nothing behind it. I think like but even then like I think with AI, I think it definitely becomes like we also kind of have tasks for each role. I think that becomes even more and more important there. Definitely seen in the past that a lot of tasks, especially take home tasks, It is yeah obviously if you never know it was AI involved or other people involved like even pre-AI we had cases where some other people simply helped out there so like something like a live session where you just go through a problem and kind of try to kind of see like how would you work through the problem together it actually tells us much more.

**Jan Oberhauser** (01:05:58)

We also had problems in the past that Like you can obviously have people that kind of worked in the same space before and people that never heard about a problem. And I think it's very hard to understand sometimes if you have some person already worked on the problem before and if they actually had the right quality, they just again Are they actually at the right level or did they just again experience it before? That's why they perform much better than people that never thought about it and it's just a very hard thing honestly. Very often you have to still work with them for a month or two to really understand hey did they really meet the bar and I mentioned before like Having this goal of reaching a billion users with less than a thousand employees, that obviously makes very clear that talent density is really important.

**Jan Oberhauser** (01:06:45)

If you have only a thousand people at a certain scale, you can only have the best ones. And they're kind of really ensuring that the quality is as high as possible. Obviously, it always means you kind of really have to always kind of keep the hiring bar high. But again, if something doesn't work out, I think it's the best for both sides if you also kind of sadly let them go. Because I think it's obviously not going to be great for N&M, but it's also going to be bad for the people actually to leave them in that role because they're not set up for success. It doesn't mean that they're bad in any way, but they're not the right fit for the role we need them in the organization.

**Aakash Gupta** (01:07:18)

Wow, what a wide ranging conversation. We covered N8N's growth, N8N versus Cloud Code and Zapier. We showed you guys how to use N8N to create a personal productivity assistant and get other use cases from templates as well as how they grew. Jan, thank you for all of the alpha you dropped today.

**Jan Oberhauser** (01:07:37)

Thank you for having me. I really enjoyed the conversation. See you.

**Aakash Gupta** (01:07:40)

All right. And if people want to find you online, where should they go?

**Jan Oberhauser** (01:07:43)

Honestly, I'm only active on LinkedIn. I left X and so only on LinkedIn.

**Aakash Gupta** (01:07:48)

All right. Find him on LinkedIn. Obviously, go try N8N. If you haven't, I have other videos that go

**Jan Oberhauser** (01:07:53)

deeper on N8N, which I will link right up here. And see you in the next episode.

**Aakash Gupta** (01:07:58)

I hope you learned as much from today's episode as I did. If you can do one thing that's totally free that would help the show, it would be to check that you're following on Apple and Spotify podcasts. Check that you've left ratings and reviews on those platforms. Check that you're subscribed on YouTube. Leave a like and a comment on this video, and then share it with your friends. We're trying to make better and better podcasts. After two years, we think we've gotten something pretty good going. So let us know what we can do to make it even better, who else we should interview, and we And I can't wait to share our next episode.
