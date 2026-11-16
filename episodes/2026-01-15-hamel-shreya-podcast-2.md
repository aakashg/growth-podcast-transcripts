---
title: "How to Do AI Evals Step-by-Step with Real Production Data | Tutorial by Hamel Husain and Shreya Shankar"
subtitle: "The step-by-step guide to error analysis, LLM judges, and shipping AI products that don’t suck in production"
date: "2026-01-15"
host: "Aakash Gupta"
guests: ["Hamel Hussian", "Shreya Shankar"]
speaker_names: "substack"
substack_url: "https://www.news.aakashg.com/p/hamel-shreya-podcast-2"
youtube_url: "https://www.youtube.com/watch?v=J7N9FMouSKg"
duration: "01:05:43"
word_count: 10624
source: "Substack episode transcript (aired audio)"
---

# How to Do AI Evals Step-by-Step with Real Production Data | Tutorial by Hamel Husain and Shreya Shankar

*The step-by-step guide to error analysis, LLM judges, and shipping AI products that don’t suck in production*

**Hamel Hussian** (00:00:00)

What are we going to do today?

**Aakash Gupta** (00:00:01)

So today we're going to walk you through how to do evals step by step. The real live example on real data.

**Hamel Hussian** (00:00:07)

Do we even need eval? I've heard Claude Code doesn't use evals.

**Shreya Shankar** (00:00:10)

Oh my gosh, this is a crazy controversy that's been going around.

**Hamel Hussian** (00:00:14)

There's way too much hype about AI. To build a really good AI feature, it's not just a demo. You need to build something that goes to production. I consider AI evals the number one most important new skill for product managers. Where do people at Anthropic and OpenAI go to learn AI evals? It's Hamel Hussain and Shreya Shankar. This is what your AI agents are actually doing out there in production. And that's why looking at the traces is so important.

**Shreya Shankar** (00:00:40)

We show so many demos in class where we just dump this trace into ChatGPT and we ask, was the assistant correct? And then ChatGPT will say, yeah, absolutely. But it will miss all of this nuance.

**Hamel Hussian** (00:00:51)

Do I need an AI observability tool? I already am paying for whatever Datadog or whatever APM tool I already have. What is the difference?

**Aakash Gupta** (00:00:59)

You don't necessarily need a tool. It's sometimes good to start with one, but if you want to, you can log to CSV file, JSON file, text file, whatever you feel comfortable with.

**Hamel Hussian** (00:01:09)

What are other mistakes like separating the prompt from the product manager that people might be doing in this process that we walk through today that is unintentionally inhibiting them?

**Aakash Gupta** (00:01:18)

The main thing that's inhibiting people is not doing the error analysis.

**Hamel Hussian** (00:01:27)

Before we get into today's episode, if you can do me a quick favor and check if you have a following on Apple and Spotify podcasts and subscribed on YouTube, these are free actions you can take that really help the show grow. And if you become an annual subscriber to my newsletter, did you know that you get access to over $28,000 of premium products? That's right. mobbin arise relay.app dovetail linear magic patterns deep sky reforge build and descript they are all free for an entire year if you become an annual subscriber to my newsletter so go take advantage at bundle.akashg.com and now into today's episode Quick note for my audio listeners, there are some things that we showed, which you can see on Spotify or YouTube, but we've edited this audio so that it's a really good listening experience nonetheless. Hamel, Shreya, welcome to the podcast. Thank you for

**Aakash Gupta** (00:02:23)

having us again.

**Shreya Shankar** (00:02:23)

Yeah, super excited.

**Hamel Hussian** (00:02:25)

What are we going to do today?

**Aakash Gupta** (00:02:26)

So today we're going to take you step by step on how to do application-specific evals.

**Hamel Hussian** (00:02:31)

Do we even need evals? I heard Cloud Code doesn't use evals.

**Shreya Shankar** (00:02:36)

Oh my gosh, this is a crazy controversy that's been going around. Absolutely, everyone needs evals. And some people are less rigorous about it because perhaps there's somebody else who's done evals for then upstream. For example, in coding agents, you know that people who are training the models are testing on a bunch of code. So maybe you can easily build a coding application based on religiously dogfooding your outputs. But for most applications that are not just naive applications of foundation models, such as what you're building, you're going to need some form of evals.

**Hamel Hussian** (00:03:09)

Couldn't agree more. Evals, it's about actually improving your product. Maybe you're doing that through dog fooding, or maybe you're doing it through the systematic process that we're about to walk you through, but you have to do them. So let's get started.

**Aakash Gupta** (00:03:22)

So today I'm going to walk you through how to go about evals using a real company that I worked with, NurtureBoss. And NurtureBoss has been very generous in allowing me to use some of their anonymized data as a teaching example. So what is NurtureBoss? NurtureBoss is a tool that allows property managers who are managing apartment complexes deal with things like tenant interaction and marketing and sales. And so you can see their website here, NurtureBoss.io, and you can kind of get a feel for some of their, you know, it's a mobile, you can have a mobile app, you can embed it on the website, but you can see here's an example interaction. Do you have any two bedrooms available? And the Nurture Boss application is interacting with the tenant for you, helping to show listings, schedule appointments, so on and so forth. You know, kind of all the different activities that you might be engaged in as a property manager, their application is helping you manage that with the assistance of AI.

**Aakash Gupta** (00:04:29)

So it's a really good example because it incorporates all the messiness of a real-world AI application. There is tool calls. There's RAG, multi-turn conversations. There's even multiple channels you can interact with the application through voice, text message, or text. chatbot and so it's kind of a lot of different messiness of the real world this is not a simplified example this is something that you will encounter you know in the real world your application might have these complexities so like how do you go about thinking about eval so when i started working with nurture boss they had something initially that worked But they really wanted to know, okay, how do we, number one, figure out what's going wrong? And number two, how do we improve the application systematically beyond just doing vibe checks? Because they already did vibe checks. They were using their own application. They had some design partners and some initial customers.

**Aakash Gupta** (00:05:34)

But they wanted to move beyond that and make it really good. Okay, so the first thing that you want to start with is some kind of observability. So the NurtureBoss application, they instrumented their code and they captured their traces. So let me just show you what a trace looks like. So this is an observability platform called BrainTrust. It doesn't really matter what you use. There's a lot of popular ones out there. Ones that I see are things like, okay, so BrainTrust is one. There's LangSmith. is another one that's popular. Arise is another one. It really doesn't matter which one you use. But the reason I'm showing you one is so that you get it. And before we even get

**Hamel Hussian** (00:06:15)

there, some people might be wondering, do I need an AI observability tool? I already am paying for whatever Datadog or whatever APM tool I already have. What is the difference between those tools?

**Aakash Gupta** (00:06:29)

Yeah, you don't necessarily need a tool. It's sometimes good to start with one, but if you want to, you can log to CSV file, JSON file, text file, whatever you feel comfortable with. The reason I have it pulled up right here is so that we can read it together and kind of you know, have something to look at. But if you're using Datadog, feel free to log things to Datadog to begin with. The most important thing that you're going to want to have is to take notes on your traces. And we'll show you why in a second. One of the things that Shreya and I teach is actually to vibe code your own trace viewer. And we'll talk about that in a moment. I can show you, NurtureBoss did Vibe code their own trace viewer eventually. They didn't end up using this. But, you know, sometimes to get started, it is handy to use an observability platform, but sometimes it's not.

**Aakash Gupta** (00:07:25)

Sometimes, you know, depending on what you want, maybe you already have one. Feel free to use that. The key is, like, do the simplest thing you can think

**Hamel Hussian** (00:07:33)

of. Get started.

**Aakash Gupta** (00:07:37)

Yeah. Okay. So here's a trace. And you can see the trace just logs all of the different turns and all of the information that is shown to the LLM. And so what you have here is a system prompt. You are an AI assistant working as a leasing team member at Harmony, which is the name of a fictitious apartment complex. Your primary role is to respond to text messages from both residents and prospective residents. So it's very interesting. People will be text messaging this application. Hmm. And so, you know, you're engaged with the customer to answer questions about tours and drive applications. And there's a whole host of different rules about how to respond to the customer. And what you'll see here is you have some rules, okay, like how to interact with them, determine if the inquiry is from a resident or prospective resident. I won't read all of these for you.

**Aakash Gupta** (00:08:44)

There's some property specific information here, like, URLs. This is anonymized, obviously. The URL is not acme.com. But you can get the idea. And, you know, this is basically the system prompt. So that's the system prompt. You see the first user messages. You can see that there's like some kind of logging error. It's like don't know who this is or what apartment you're from. So you can see like it's, you know, this is a real world messy logging. But the first question is, I need a one bedroom with the bathroom not connected in floor plans. And then you can see there's a tool call of some kind where we're getting the individual's information. We're getting something about the availability. And the tool is returning a list of apartments here. You can see these are kind of like a list of apartments. And then we have the assistant responding with you know, these apartments here.

**Aakash Gupta** (00:09:48)

And, um, you know, it's saying, okay, we have like these three apartments with the link to this floor plans page, so on and so forth. Um... And then, you know, it's a text message. So this user is saying something about being sick and, you know, not being able to book tours. And something about a bathroom connected to the room. I'll check for one bedroom apartment so the bathroom is not connected. Thank you and you're welcome. Okay, so... So there's a lot of things that kind of went wrong here. One is what is going on here with, I want a bathroom connected to the room, but it just said, I'll check on that. But then it didn't do anything, right? So we would hope that it would actually do something or if it's not able to do it, hand off to a human. So that's kind of funny.

**Aakash Gupta** (00:10:52)

I do happen to know that, so this response up here is also in markdown. So you can see here, yeah, this is a markdown response and this is a text message. So it's gonna be rendered a bit weird in a text message because text messages don't have markdown. And so this is a bit problematic, too, with the bold and everything. It's going to come across, you know, potentially in a weird way. With like asterisks and stuff. Yeah, yeah, it's gonna have asterisks and it's gonna have square brackets

**Hamel Hussian** (00:11:26)

and stuff like that. If you've been enjoying this demo on how to do AI evals, you are going to love Hamel and Shreya's course. It is the top grossing course on Maven. It is taken by people from OpenAI to Anthropic to Google to Meta. All of the top AI companies are taking this course to improve their evals. I have secured a massive 35% discount for you guys. So use code AG-EVLAS so that you can get this course. You can learn even more in detail how to write great evals, how to build great AI products that are working in production. Check it out at maven.com and look for their course and type in code AG-EVLAS. That means it will only cost you $2,275. The next version of their course starts on October 6th. Today's episode is brought to you by Vanta. As a founder, you're moving fast toward product market fit, your next round, or your first big enterprise deal.

**Hamel Hussian** (00:12:24)

But with AI accelerating how quickly startups build and ship, security expectations are higher earlier than ever. Getting security and compliance right can unlock growth or stall it if you wait too long. With deep integrations and automated workflows built for fast-moving teams, Vanta gets you audit-ready fast and keeps you secure with continuous monitoring as your models, infra, and customers evolve. Fast-scoring startups like LinkChain, Writer, and Cursor trusted Vanta to build a scalable foundation from the start. So go to Vanta.com slash Akash. That's V-A-N-T-A dot com slash A-A-K-A-S-H to save $1,000 and join over 10,000 ambitious companies already scaling with Vanta.

**Shreya Shankar** (00:13:07)

One more thing is actually in the first message, the user said they wanted the bathroom and bedroom disconnected. Yeah, see, I need one bedroom with a bathroom not connected. And then the assistant's first message was, here are some bedrooms with bathrooms connected.

**Aakash Gupta** (00:13:24)

Oh, yes. See, there you go. That's a good observation. So it actually didn't really help the user. The user just kind of gently reminded them again, like, hey, I do want a bathroom connected to the room. I mean, this is like very messy. You could see like there's misspellings. I could almost not understand what the person was

**Shreya Shankar** (00:13:42)

asking. Yeah, the now should be a not. I do not want a bathroom connected to the room.

**Hamel Hussian** (00:13:47)

Yeah. So this is awesome. This is, guys, if you are PMs listening, this is what your agents are actually doing out there in production a lot of the time. And so your demo is one thing. It goes well. But then when it goes out in production, there's all this hairiness. And that's why looking at the traces is so important.

**Aakash Gupta** (00:14:07)

Yes. And so this is exactly why you don't want to have generic metrics. If you try to put helpfulness score, conciseness score, whatever in here, or you try to have AI look through your traces, it's not going to catch stuff like this very well at all. Because there's a lot of context that you have as a PM. And a lot of things that kind of you have tastes that you need to reflect on and say, hey, this is not a good experience from a product perspective. And the language model is not going to know that because it hasn't been able to read your mind. Mm-hmm. And so...

**Shreya Shankar** (00:14:44)

This happens all the time. We show so many demos in class where we just dump this trace into ChatGPT. I mean, you can probably even do it now. Or Claude. And we ask, was the assistant correct? And then ChatGPT will say, yeah, absolutely. Sounds correct. But it

**Aakash Gupta** (00:14:59)

will miss all

**Shreya Shankar** (00:15:00)

of this nuance that Hamel and I and Akash have been mentioning because we actually put our product hat on and thought about the user experience a little bit.

**Hamel Hussian** (00:15:13)

Yeah, let's see what ChachiPT does.

**Shreya Shankar** (00:15:24)

Oh, look at that. So I found that one.

**Hamel Hussian** (00:15:26)

Okay, so it figured out that we didn't get the connected bathroom. But this

**Shreya Shankar** (00:15:34)

is hilarious. It says it doesn't filter by bathroom configuration. And the interesting thing is who knows if that's a filter that the tool provides.

**Aakash Gupta** (00:15:45)

Yeah,

**Shreya Shankar** (00:15:46)

this is certainly cherry picked three examples. I mean. Maybe that's fine for us, right? Like nobody wants to put all who went. But I don't want to see a text message of every single apartment. I actually only want to see a couple.

**Hamel Hussian** (00:16:07)

Yep. So chat GPT might help you a little bit, but you ultimately need to put your human touch on top of this and make sure.

**Aakash Gupta** (00:16:15)

Yeah, it won't it won't know that about the markdown, you know, so like I didn't catch. Yeah, you can, you know, I can change the format of this rendering, I believe, somehow to show you the raw. This is actually all rendered as markdown. But, you know, since it's a text message, but like, you know, chat GPT is not going to know that. And there's other examples that we'll see that, okay, you need to put your, you need to kind of have a keen eye about what's going on in the product and bring your whole product knowledge to bear. Um, and so, yeah, if you try to, it can, it can miss a lot of things. Um, And so, oh yeah, this is like the raw. This is another raw way of looking at it in YAML form. But anyways, that's not important. So what you could do from here is you need to write a note.

**Aakash Gupta** (00:17:10)

So I'm gonna go into review mode. So some issues here would be, you know, told user that it would check on bathrooms but didn't do it. Say like also did not follow user instructions and rendered markdown in a text message. And so what you really want to do is this can sound very tedious. Like what I just did, it sounds like it's very resource and time intensive, but it's really not. Like you just scan the trace. And, you know, if you're familiar with a system prompt, you don't have to read it. You're not going to read every system prompt because it's going to be the same, really, unless you need to. But it's really, you can, you know, within about 30 seconds or so or less, you can kind of scan this and say, hmm, Okay, you can get a sense of like what is happening and you can write some notes.

**Aakash Gupta** (00:18:09)

The perfection is not key. The key is like see what's going wrong in the trace and note what you see and move on. you don't have to catch everything, just catch the most important things. And so we can keep going. So let's go on to the next trace. And let's see, let me just, you don't have to edit this out. Let me find one with an issue. Okay, here we go. Here's one with the issue. So edit that navigation out. So we have, let me just hide some stuff here. So the user in this case is asking, this is a new trace now. Do y'all have one bedroom with study available? I saw it on the virtual tours. And there's a tool call to get information and availability. And it says, yes, hi, Priya. We currently have several one-bedroom apartments available, but none specifically listed with a study.

**Aakash Gupta** (00:19:00)

Okay. So, okay. It matches. She did ask for a study. Um, so I gave her one, uh, one bedrooms instead. And then the user asked, can you let me know when one with the study is available? And the assistant says, I currently don't have specific information on the available of a one bedroom. So, okay. Is this kind of, this is where you get frustrated, right? I asked the question, you just responded with some robotic, like I don't have that. Um, and so I would say, yeah, this is a, this is a product failure. Um, And what you want to do is say like, okay, um, you want to just note that real quick. So, um, should have handed off to a human or had have better lead nurturing. And there's no pun intended with the word nurturing. Just that's what came to mind. So, um, you know, anything else that you think is wrong with this particular trace?

**Shreya Shankar** (00:20:10)

Yeah, I don't think you have to get bogged down. It's a good question to ask, but typically we tell people, all right, think of everything that comes to mind, write them down, move on. You want to get into kind of a flow state here. You can debate every trace endlessly, and sometimes you see people get stuck in that. So try to just kind of avoid that. We got a problem. Thanks.

**Aakash Gupta** (00:20:33)

Yeah, I agree with that. Move on. This one I already did, but that's okay. We can do it again. So let's find the first user message. Let me scroll up. Sorry. Okay. So I'm in California. So, okay, we have to edit the part out where I scroll to this part, but we can start. So this is kind of the third trace we're looking at. So the user asks, I'm in California looking to relocate to Texas by March 15th, Boven. Thanks for sharing. Since you're planning to relocate, blah, blah, blah. I can help you explore available apartments. If you'd like, we can also schedule a virtual tour. it's like yeah that's great you know thank you and okay I'll arrange a virtual tour for you so you can explore community what's your preferred date and time tomorrow is fine for me 9am I can schedule a virtual tour for you that's fine it schedules a tour and then it says your virtual tour is all set looks good right Actually, it didn't go so well.

**Aakash Gupta** (00:21:50)

And so the reason it didn't go so well is because there's no such thing as a virtual tour for this apartment. And I don't think there's a such thing as virtual tools for most of their apartments that they have on the platform. And so the AI called the tour scheduling tool but it doesn't do virtual tours. So, you know, the platform is scheduled an in-person tour and maybe the user is confused and is like, oh, great, it's like going to be a virtual tour and it's kind of a little bit of a disaster. And so... Okay, that's fine. So that problem is there. And then the date they said, January 22nd, 2025, the user said, wait, today is the 22nd. Do you mean tomorrow? Because we can't do it today. It's like, oh, no problem. Your virtual tour has been rescheduled for tomorrow. But if you look, the schedule a tour tool was called again.

**Aakash Gupta** (00:22:57)

So what this means is, Hey, like you just scheduled another tour. You didn't reschedule anything. So now the person has two tours. So, and, and, you know, maybe, you know, that's going to cause a problem for the apartment complex because now they have two tours booked that, which are going to be no shows. Um, And then, you know, there's some other questions. How can I go about getting a unit if I'm in California trying to relocate, blah, blah, blah. And it's giving some responses here. That seems okay. So, you know, I have written down the two issues here. We don't do rescheduling and we don't do virtual tours, only in-person tour. So I just wrote some notes. So the idea is that you just keep doing this. And so this actually, you can do this quite fast. You do this for, let's say, 100 or so traces.

**Aakash Gupta** (00:23:46)

Just write down what you see. Don't try to get into root cause analysis. Don't try to figure out what went wrong exactly. Just journal, observe freely. Just journal what you see going wrong, if anything. If nothing is wrong, you can just skip it. But when you do find something wrong, go ahead and write that down.

**Hamel Hussian** (00:24:05)

Mm-hmm.

**Aakash Gupta** (00:24:08)

Does that seem, is that clear, Akash, that process? Yep, exactly. Okay, great. So now you have what we call a bunch of open codes. And this is not, so, okay, this is the start of the most important part of evals, which is called error analysis. And something that's very approachable to everyone is actually, it's very important for product managers to be involved in this. Because a lot of times engineers don't have the context the full context to know if this is good or bad. And so what you end up having is you have, let's say, a bunch of these like notes. So I have a spreadsheet open right now with a collection of all the notes that I took. And, you know, let's say I did 100 of these. I actually found 40 or so different errors. You might find different number of errors if you're doing it.

**Aakash Gupta** (00:25:07)

But here's a collection of these notes. Okay, great. So up until this step, you've already learned quite a lot. If you look at 100 traces, you're going to learn and you're going to understand your system better than anyone else. And you're going to have a really deep understanding of what is wrong. And you might also have a pretty good sense of what you need to work on next already without doing any analysis. But it's really good to do analysis of these notes that you took. So how do you do this analysis? So the next step is you categorize these notes. So the term for that is called axial coding. And I'm gonna show you how to do this in a spreadsheet. So let me just zoom out a little bit. But first, one thing you can do is, okay, you can take these and you can put them into ChatGPT or Claude.

**Aakash Gupta** (00:26:04)

So what I did is I took sort of the logs And I said, okay, please analyze. I exported it from here. So, you know, there's, let me go back. So there's an export button here. And I said, okay, download a CSV. Downloaded it, put it in. Claude, and I said, hey, there's a metadata field which has a nest field called Xeno that contains all the open codes. And I use the word open codes because it's a term of art that LLMs understand. Because these terms, open coding and axial coding, which you mentioned, open coding is the writing of the notes. That's actually a term that's well understood in the field of machine learning, but also goes, it's been around before machine learning has been used in the social sciences. This kind of process of open coding, axial coding is a thing that LLMs understand. And so I just say there's a meditative field, which has a nested field called Zenote that contains open codes for analysis of LLM logs that we were conducting.

**Aakash Gupta** (00:27:16)

Please extract all the different open codes and then propose five to six categories that we can create axial codes from. And then it'll kind of go through and you can get these categories. So here's some categories like... You know, capability limitations, representation. Some of these I don't like because they're a little bit too broad. They're not actionable. I'm actually not 100% sure what that means. So I might look into it and rename it a bit. You know, human handoff issues. There's certainly some of that. That's when, hey, you want to escalate to human being or hand off to human being, but it's not doing it properly. temporal, contextual awareness, doesn't know what the current date and time is. You know, so there's some categories here. You can refine this. What I like to do is take it to a spreadsheet. So I like have some categories that I kind of have that I maybe have from ChatGPT.

**Aakash Gupta** (00:28:17)

And then I kind of look at them and edit them. So I kind of have these like categories that I sort of edited a bit. And I said, okay, let me just collect these into a list. So that's what this formula does. Is I just collecting these list of categories into a list. That's all that is.

**Shreya Shankar** (00:28:35)

I have a note here. So I think one of the things that's very interesting from looking at your clod is a lot of those axial codes are very vague, right? Like quality or temporal issues. And you kind of want to make sure your actual axial codes are not so vague because imagine you're giving them to somebody else to do some labeling with, right? Like Something like conversational flow issues might be a little bit better. Honestly, we could even make it a little bit more specific. But something like temporal issues, right? Like if Hamill told me to go label with temporal issues category, I wouldn't even know what he means. I would want to say like, you know, date formatting error or like something like that. Right. So I think that's another place where people get tripped up, which is, you know. just taking things out of the LLM as is and not really thinking about, OK, how do I refine that in a way that's going to give me meaningful error categories?

**Hamel Hussian** (00:29:36)

Jira Product Discovery designed for product teams, capture insights, prioritize what matters, and create roadmaps you can easily tailor for any audience. And because it's built to work with Jira, everything stays connected from idea to delivery. Used by product teams at Canva, Deliveroo, and even The Economist, check out why and try it for free today at atlassian.com slash product dash discovery. That's A-T-L-A-S-S-I-A-N dot com slash product dash discovery. Jira Product Discovery. Build the right thing. Today's episode is also brought to you by my cohort-based coaching program to help you land your dream PM job. I'm taking 30 elite PMs to land their jobs at Google, OpenAI, and other $700,000 plus roles. If you want in, check out landpmjob.com. Once all 30 seats are sold out, that's it. And already seats are going almost every day. So grab yours at landpmjob.com. Today's podcast is brought to you by Pendo, the leading software experience management platform.

**Hamel Hussian** (00:31:01)

McKinsey found that 78% of companies are using Gen AI, but just as many have reported no bottom line improvements. So how do you know if your AI agents are actually working? Are they giving users the wrong answers, creating more work instead of less, improving retention, or hurting it? When your software data and AI data are disconnected, you can't answer these questions. But when you bring all your usage data together in one place, you can see what users do before, during, and after they use AI. showing you when agents work, how they help you grow, and when to prioritize on your roadmap. Pendo Agent Analytics is the only solution built to do this for product teams. Start measuring your AI's performance with Agent Analytics at pendo.io slash akash. That's p-e-n-d-o dot i-o slash a-a-k-a-s-h.

**Aakash Gupta** (00:31:46)

Exactly right. And that's a really important thing to pay attention to. That's why if you reflect on the categories I have in this spreadsheet, they're definitely better than the ones in the clod. Yeah, they're different

**Shreya Shankar** (00:31:57)

for a reason.

**Aakash Gupta** (00:31:59)

It's because I iterated on a bit. And that's an important principle. You never want to completely hand off the wheel to AI. You want to think about what it's saying. Maybe it helps you to different degrees, but you want to see, okay, like what are the categories here? And actually you might want to go back and forth. So what I did here is I went to those notes, which I have here. Every row is a different note. And, you know, you can use AI. So I used AI, categorize the following note into one of the following categories. Okay. And what I did is I... you know, had AI. And this is a formula in a spreadsheet. So you can see the prompt. And basically like classify each of these notes into one of those categories. And I went back and forth. It's like, hmm, this category actually is not the greatest for this particular note.

**Aakash Gupta** (00:32:51)

And I like went and edited the note. I went back to this category field, maybe like added one, deleted one, and like kind of fiddled with it till I was like reasonably happy. Like, okay, this is like a good set. It's good enough. One thing I should have added here is like none of the above, which would have been better. But, you know, I'm showing you the simple, stupid version, which is like get started. I don't want to overcomplicate it, but that's what you should do.

**Shreya Shankar** (00:33:19)

And none of the above is mainly like a means to the end. The end is really having these categories, but sometimes you might have like missed a category. So if you put none of the above here, and then your AI does a classification and tells you none of the above, then you can go read those traces again and wonder, maybe there's another category that I should add so I can classify those.

**Aakash Gupta** (00:33:41)

So when you get... So you have these classifications... And okay, let me just zoom out so we can see it together. Sorry about that. So you have all these classifications and now comes like the powerful part where you will put on, well, you will have like real superpowers if you do this as a PM, then you will go above and beyond and kind of be armed with information that a lot of people usually not armed with and it's counting so now you can count these issues and you know you can just use a pivot table that's what i did here is say okay like how many times did i see this So now you have taken a world where it's kind of messy and you don't really know what is going on. You know that there's some errors. And you have this kind of paralysis of like, what do I work on?

**Aakash Gupta** (00:34:38)

What do I fix next? What's the most burning problems in my app? and you know you have some data in front of you you know like hey you're having these conversational flow issues a lot in this conversational flow issue it's actually regarding situations where there's text messages so i happen to know that i can click on this um you know you can say like hey yeah there's like disparate messaging sent in-person tour link um okay there's there's different sometimes it's about text messages sometimes it's just like It's not being clear. And we can go back to the trace and look at that. Some of my favorite things about pivot tables, you can like double click.

**Shreya Shankar** (00:35:21)

You can also make it hierarchical. I like to do this, too. So sometimes I like to say I like to break down conversational flow into like three different categories, subcategories. Maybe some will be like repeated messages and some things will be, you know, the AI just should have handled this one particular thing that are I don't know. So you should I think this is kind of where the subjectivity and your product experience shines. Right. It's like you have to do this process in a way that enables you to make your product better based on the capabilities of your product or what your team can do. So, you know, if you can't have virtual tours, then you can't have virtual tours that has to somehow be encoded in your system. Right. So.

**Aakash Gupta** (00:36:10)

Yeah, definitely. And so, yeah, this could be made better. I think that's, you know, I didn't try to, let's say, make it perfect. But as Shreya points out, you can have, you know, subcategories, which can help you kind of refine what's going on more. Yeah. But you can take a look at this. You can say, okay, what do I think is most important? Like, hey, maybe the human handoff issue is not happening as much as the conversational flow issue, but let's say you feel as a product manager that is a catastrophic error and that the magnitude of that problem, the impact of that problem is so high that I'm gonna prioritize that as number one. But you have some data to back up that this is happening and you have an idea of what's happening. And now you have a reason to potentially write evals. Now you're not writing evals in the dark.

**Aakash Gupta** (00:37:09)

Now you can write evals in response to actual problems that you are seeing instead of like hallucination score. or some AI generated something or the other, you know, you can motivate this thing that you want to fix. Now, you don't have to write an eval for everything. There might be some of these things that might be easy to fix. Like, for example, there's this formatting error with output. You know, an example might be using markdown and text messages. You might be able to just fix that. Yeah. maybe there's no instruction in the prompt at all. And it depends like what kind of eval you need to write. So there's two kinds of evals. One is code-based, where you can test something without calling an LLM. So the formatting error with output, you might be able to use a code-based eval for that. Like, hey, is the format, do I see markdown elements in this output where there shouldn't be a markdown?

**Aakash Gupta** (00:38:14)

In which case, maybe you should write the eval because it's not going to be expensive. Whereas with the LLM as a judge, something more subjective like, hey, you should be handing off to a human. You might need an LLM for that. You might not be able to write an assertion in code. That's a little bit more expensive of an eval. And you have to have a judgment call like, okay, is that something that's trivial to fix? Like I didn't have that. I didn't have like, you know, something in my prompt that, you know, had this instruction. Maybe you've found like some dumb mistake that you made. Go ahead and fix it. You don't have to get caught up in evals. What you want to do is write an eval for something that you think you might want to iterate against. I don't know if there's a better way to say that.

**Aakash Gupta** (00:39:05)

I feel like that could have been... Shreya, you think there's a better way? No. Okay.

**Shreya Shankar** (00:39:10)

I think it makes a lot of sense, right? So already, as a PM, this is a secret sauce for your product. If you don't do this product, you can't... If you don't do this process, you can't kind of put your own taste or your company's taste into your product. Once you get to this point, that's kind of when paths diverge. I think that's what Hamill is trying to say. Maybe sometimes you figure out, okay, there's some errors that are higher priority than others. I'm going to go and fix those. Maybe you want to run these checks at larger scale. Like maybe you're meta or you're Google and you're like, I can't make a decision based on 42 traces and I need a lot of buy-in. So I'm just going to, you know, build a team, do a bunch of evals, or I'm going to write automated evaluators to check this at scale.

**Shreya Shankar** (00:39:53)

Yeah, go for it. We're not going to cover that today. Take our course if you're interested in those techniques. But I think overall, I think it's super incredible. Hamill started with zero, right? Now we're at a place where we know what are the biggest failure modes in a sample of traces are, right? And most people don't get to this point.

**Aakash Gupta** (00:40:12)

Yeah. And so, okay, so going further from there, let's say you want to write an eval for the human handoff issue. Like, hey, you should be escalating to human being, you should be handing off. It can be really useful to write an eval to help you see all the traces where that flag, the traces where that might be happening and help you iterate on that problem. So let's go into how you would go about building that. So here is the prompt for an LLM judge. Now, this is just a very basic prompt. It could be made better, but I just want to keep it simple. And so, you know, you are scoring a leasing assistant, right? to determine if there's a handoff failure, return only true or false. So that's one thing that we teach is you want the LLM as a judge to produce a binary score.

**Aakash Gupta** (00:41:12)

Shreya, you want to talk about why?

**Shreya Shankar** (00:41:14)

Yeah, so... All right, I'll try to give a succinct answer for this. The short answer is that people run into a lot of misalignment when they try to use like a liker or a range face score. And that's because it's very tedious to check that every single possible LLM output aligns with your preference. Now, when you do a binary score, You only have to check that true aligns with your trues and false aligns with your falses, right? It's only two things that you have to check, which makes the process of checking for alignment easier. The other thing is when you're shipping products, right, you make binary decisions. Either this thing was bad or this thing was good. I should fix this or I should not fix this, right? It's not like... Even if you have a score of like this is 30 percent failing, that gets turned into a binary decision of how you're going.

**Shreya Shankar** (00:42:03)

Are you going to act on it or not? Right. So that's kind of why we tell people focus on a binary decision here. It's easier to align. And ultimately, your business decisions are yes or no decisions.

**Hamel Hussian** (00:42:16)

Yeah, there were some people who are trying to do like one through five skills and stuff, but it seems like LMs are not very good at those types of numbered skills. So it's much better to stay binary.

**Aakash Gupta** (00:42:27)

Definitely. We need to bring you into our consulting, Akash, if you can tell people that. So, okay, so we have this prompt and we have a list of things that... These seven things that we have where there is a failure. If there's explicit human handoff, that's request. Sorry. So we have these seven things. An example of one is the user asks to be sent to a human, but that's ignored. Or there's a policy that you should be transferred, but that's not. handled properly. There's a sensitive issue like billing disputes or legal issues that are not adhered to. Same day walk-in or tour requests. You want to hand that off to a human. So things like that. And then, you know, we have some notes about when there's not a handoff failure or It's important not to get bogged down in the prompt itself. So if you're thinking to yourself, can you send me this prompt?

**Aakash Gupta** (00:43:40)

Can I copy and paste this prompt? You're asking the wrong question. Because you need to, you know, so, okay, how do you write this prompt? You want to try to describe the rubric of, okay, what is a failure and what is not a failure? You can get LLM to help you bootstrap that, but you should try to edit it. And the key is iterating. Okay. It's not necessarily a recipe and you want to try to have examples. I didn't put examples in here. So you want to have a section of like maybe some examples. It's not necessary to begin with. In the simple case, you may not, you know, you don't need to have examples. I'm just, you know, trying to give you like the most dumbest LLM as a judge so you can get the concept. The idea is like, you know, you're going to write a prompt.

**Aakash Gupta** (00:44:32)

In our class, we do have a recipe of like what you can follow, but Zooming out from that, it's important to just iterate, honestly. That's what's going to get you the furthest. And so this prompt would be structured differently if it wasn't in a spreadsheet also. I'm kind of begging it to return true or false. I wouldn't have to beg it if I'm using an API, for example. I could do something else. So this is the prompt. And then what you can do is, okay, I have my trace here. This is a different tab of the spreadsheet. I'm saying, okay, this is the trace. And I have AI here. And it says, assess this LLM trace according to these rules. And I give it the prompt of my LLM judge. That's all I'm doing.

**Hamel Hussian** (00:45:27)

Nice. Now here's the key part. AI function built into Google Sheets. Isn't that just runs Gemini in the back end?

**Aakash Gupta** (00:45:36)

Yeah. Yeah, it's okay. I wouldn't say it's amazing. It's some kind of very fast model-ish. You know, it's good to get started, to get a mental model of what's going on, but I would, you know, I would be a little bit careful using this model for everything in real life because I'm not too sure about it. So don't get lost in the sauce of what I'm doing. I'm trying to show the exact, I'm trying to give you a mental model. But you might not actually, you might want to do something, you might want to use like a more powerful model potentially for LMS and Judge. So, okay, we have two columns here. column G and column H. So the column H is the score outputted by the LLM judge, true or false. And most people just stop here. They're like, okay, here's my LLM judge. I gave it a prompt.

**Aakash Gupta** (00:46:32)

Woo-hoo, we're done. The LLM judge says like, it's good. So we're good, right? And then what ends up happening is Stakeholders, they start to feel or observe that there is a dissonance between your evals and actual the product's performance. And they can lose trust in the evals. And they start to ask you questions like, how do you know this metric? What is this metric? And you tell them, okay, it's an LLM judge. I'm like, well, how do you trust that? A lot of people get stumped there. They're like, well, that's all we got. You don't want to do that. what you want to do is you want to measure the judge against your label. So you remember when we were doing the axial coding, you actually have your own human labels. So you know for these various traces, like, okay, if this issue existed or not.

**Aakash Gupta** (00:47:33)

And then you can compute metrics. You can compute how good your LM as a judge is. Now in this spreadsheet, I have three metrics, agreement, TPR and TNR. Now agreement is like the trap metric. The reason it's the trap metric is that's what you might gravitate towards, you know, in the naive case, you might say, okay, like we'll just measure the agreement between the judge and the human. You don't want to do that. The reason is, if this failure is only happening, let's say 10% of the time, you can have the dumbest judge in the world have 90% accuracy by just always predicting pass. In fact, your LM judge can just be like equals pass. You can introduce a bug that doesn't even call an LLM. It'll be 90% accurate. So you don't want to do that. It can be very misleading. It can mislead you.

**Aakash Gupta** (00:48:36)

So what you want to do is measure two things. How good is your judge at catching errors? You know, catching errors that exist and how good is your judge at... Sorry, let me rephrase that. That was good. Let's try to explain this one so I can give myself a break.

**Shreya Shankar** (00:48:57)

Sure, sure. Oh, man. I mean, I think you've like said basically most of it. The point is, okay, if you're a product manager and somebody tells you you have high agreement, with your judge or they got high agreement with the judge, be a little bit suspicious. Ask them, okay, what's the alignment in the positives or the passes, trues? What's the alignment in the falses? And make sure both of them are pretty high individually. If not, then you have to rework your LLM judge prompt.

**Aakash Gupta** (00:49:30)

And if you were confused about this, if you're not convinced intellectually somehow that, like, why can't I just use agreement, Hamill? Why do I need to, like, measure positives and negatives separately? You should use the spreadsheet. You should get a spreadsheet like this. And you should, like, do some experiments and say, oh, okay, like, what if I just, you know, hard-coded this to false all the time? I think this confusion matrix, maybe not necessary, might confuse people. It's

**Shreya Shankar** (00:50:07)

going

**Aakash Gupta** (00:50:07)

to confuse people. It always does. You

**Shreya Shankar** (00:50:10)

can't teach the whole course in a one and a half hour thing, I think, which is cutter losses.

**Aakash Gupta** (00:50:15)

Yeah, yeah. Okay. So, you know, that's kind of, there's a lot of things that we didn't cover here. One key thing is how to split your data set so you're not overfitting your judge and you're not inadvertently cheating. That's way too much to get into in a one-hour podcast. There's no way we'd cover that. But just know that, okay, there's a lot of nuance here on how you do this correctly, how you build a judge, how you get confidence. There's ways to calculate your metrics. Use this TPR, TNR to calculate what your real accuracy is. We haven't gotten into that. there's a lot of nuance on like, okay, how do you analyze agents? Like how do you, you know, if you have lots of steps and lots and lots of handoffs, how do you tame that? And how do you do analysis of that to catch those errors?

**Aakash Gupta** (00:51:12)

Another thing we teach is how do you do analysis of retrieval? So retrieval is a kind of an Achilles heel of a lot of AI systems. And so a lot of times you have to kind of dive deep and diagnose what's going on with your retrieval step in your rack. And so there's a host of metrics and analysis you might want to do there. So there's a lot of things that we didn't cover here, but the reason that we gave you a taste of error analysis, because error analysis is the step that most people skip in evals and it's rarely talked about. And it's the thing that's going to give you extreme leverage. as a PM, and you can get there just with counting. I hope that I've convinced you by using the spreadsheet that it's within your reach. And, you know, I don't want to discourage you from using spreadsheets either.

**Aakash Gupta** (00:52:10)

Like, feel free to use whatever you're comfortable with. Sorry, go ahead.

**Hamel Hussian** (00:52:14)

So where do you go from here? Once you have this initial set of metrics, how do you go about improving once you have created your initial evals?

**Aakash Gupta** (00:52:24)

Right, so let's say like this handoff error eval that we created. What you can do is you can, now you have a judge, an LLM judge that you like. You feel good enough about this accurate enough. You can use it to score a large sample of all your production traces. And now you can learn more about what is going wrong in those situations. But secondly, you can iterate on this problem really fast. You can make some changes to your prompt. And you can calculate your error rate on these test cases that you curated and kind of iterate really fast and say, okay, like this prompt is working, this prompt is not working. And you will have a suite of these evals And you can test against all of them to see, okay, like if you are iterating on this problem, are you inadvertently breaking something else?

**Aakash Gupta** (00:53:21)

And you have some kind of way to, a system that you can use to sort of be confident in what you're doing rather than just guessing.

**Hamel Hussian** (00:53:31)

What does a holistic like end state eval suite look like?

**Aakash Gupta** (00:53:36)

Frey, do you want to talk about that? Like how many evals do you usually have in your...

**Shreya Shankar** (00:53:40)

Yeah, it's different for every application. And it's different for how high stakes the application is. Typically, I'll see like, you know, several code-based evals, especially in CI, maybe one or two LLM-based evals in CI, but not really... I do see some people, myself included, run LLM-powered evaluations, kind of like monitoring or online. Every week or so, I'll sample some of my traces, run my LLM-powered evaluators on them, and then kind of just look at the score, see if anything's off or whatnot. And often I'll see every few weeks that like, oh, there's this new distribution of data or this new cohort of people who are using the tool. Like I build AI-powered data processing tools. And so I'll see like, oh, there's different document types that have come in or a different... set of contracts. I do this for law a lot. So like there's a new type of contract or a new type of document that's come up.

**Shreya Shankar** (00:54:41)

And then now I need to like think about it. Right. So LLM powered evals, automated evals allow me to really quickly iterate out those. You don't need a hundred of them, like just a few is fine.

**Hamel Hussian** (00:54:51)

And what's the role of PM and AI engineer and AI researcher and all of this? How are you working together? Where are the handoffs happening? Like that quick iteration on the system prompt, who's doing that?

**Aakash Gupta** (00:55:02)

It's a really good question. You know, it depends on the size of the team and the company and the roles. Sometimes these roles are being collapsed into one. Um, in terms of, okay, so Jacob Carter, the engine, the CEO and, you know, also engineer of this product is the product manager and the AI engineer, um, all in one. So, you know, he is, has a pretty good pulse on like, Hey, is this interaction good or not? That's not feasible all the time. In other situations, you want the domain expert to be driving, especially the error analysis process, as much as possible. It might take some training in the beginning to get the right tools surfaced for the PM or get the PM able to access the data. And might need some engineering, like kind of co, what's the right word? Pair programming in a way or pairing.

**Aakash Gupta** (00:56:08)

So pairing on error analysis just to feel comfortable, but you should try to have one person do their analysis so it doesn't become onerous. And usually a product manager is pretty good at that because they have all of the domain expertise to actually judge if something is going wrong. So I would bias on the side of having the domain expert or the product manager do this error analysis. And as far as writing the prompt is concerned, you do want to try to make it accessible for the product manager to write the prompt. So what I've seen in a lot of tools is having an admin view where a non-technical person can edit the prompt. I actually have a screenshot of that here. One thing that... we talk about a lot in our course is you want to create your own tools to look at your traces.

**Aakash Gupta** (00:57:09)

And so NurtureBots actually created their, I've coded their own tool to look at traces, to remove all the friction of looking at traces because it's so important. And so, you know, this is pretty simple. You see all the different channels, voice, email, text, chat bot. You can see like they hide the system prompt by default. You know, it's like a very quick and dirty interface on doing this like open coding and axial coding. And actually they have a step here that helps them automate the axial coding. You see like, hey, transfer handoff issues, tour scheduling, blah, blah. So, you know, that's worth noting. That's something to think about is that's how important error analysis is. So to get back to your question about, okay, how might you surface the prompt to non-technical people? So this is an example where you might have an admin view. So this is like a different real estate agent, like, hey, showing you real estate listings.

**Aakash Gupta** (00:58:21)

And you might have this admin mode. where then you allow someone to fiddle with the prompt. And so like this prompt experimentation is really key. And so having a way that people can interact with prompts is really helpful. Now, a lot of tools have like prompt playgrounds, The only thing that's limiting about most prompt playgrounds is they don't have access to your code. Because you might have various tool calls. You might have RAG. You might have these things. All your application code is not in those prompt playgrounds. And so that's why a lot of teams that I see have these interfaces where you can edit the prompt directly in your tool and then play with it and redo it and whatever. This

**Shreya Shankar** (00:59:11)

is so nice.

**Aakash Gupta** (00:59:12)

Yeah. So, I mean, whenever possible, you want to expose the prompt to the domain expert. The reason is because it's English. It's made for the domain expert. It's almost a tragedy to separate the prompt from the product manager because it's English.

**Hamel Hussian** (00:59:32)

What are other mistakes like separating the prompt from the product manager that people might be doing in this process that we walked through today that is unintentionally inhibiting them?

**Aakash Gupta** (00:59:45)

The main thing that's inhibiting people is not doing the error analysis. People want to jump straight to, hey, let me take an off-the-shelf metric that vendor gives you and just create a score. People are very scared of this error analysis. They look at it and they're like, oh, I don't have time for this. But it doesn't take that long at all. And it's kind of this thing. It's like a secret club. When you do it just once, you will forever keep doing it. It's just like getting over that hump of doing it the first time is just extremely scary for people.

**Shreya Shankar** (01:00:25)

Another common mistake is people will see this video or I don't know, they'll realize, okay, it's worth doing error analysis. But then they think it's worth some human doing error analysis, not them. So they'll just outsource it out, which again, huge pitfall. This is the error analysis is where you build your product, right? That's where you build your moat. So if you're giving it to someone else, then you kind of have no personal touch in your product.

**Aakash Gupta** (01:00:54)

Yeah, do not outsource this to developers. If you're working on a coding app, yes. The domain expert is the developer. But in most cases, the domain expert is not the developer. And a lot of people, a lot of companies are like, oh, this AI stuff is for engineering. The whole thing is engineering. Let me just shove it over there. They need to figure out whether it's good or not. That's usually the wrong approach. It's not

**Shreya Shankar** (01:01:25)

in the engineering skill set. I think that's another interesting thing about today's day and age for PM, especially AI PM. You can't expect engineers to be able to do all of these things. The people that have been successful at this process are very, very technical PMs. Or are engineers who are actually PMs and they just think that they're engineers and they don't realize that they're doing product work. So I hope people are kind of convinced that today's day and age, you kind of have to have your product knowledge, put your product hat on.

**Aakash Gupta** (01:02:03)

this error analysis is so powerful that, um, this is a video and we can put it in the show notes of this is Jacob Carter. And he just, we recorded like a two minute long conversation of how thrilled he was with error analysis. He's actually so thrilled with it that he just, he thought this is the best thing that's ever happened. Um, and he got so much value out of it that, yeah, like, He kind of stopped there to begin with and had so much work to do that he didn't need to build evals right away because he just found so many things, as you can see right here in this picture, that he was able to fix. So he did eventually build evals, but starting here gives you a really good grounding and lets you work through issues and get to evals for things that make sense.

**Hamel Hussian** (01:03:00)

Going back to our beginning, there's so much hype about what you're trying to sell that your AI feature does. But to actually deliver on that hype, you have to go through these errors so that when people are experiencing it in production, they actually get the experience you intended. And this has been our masterclass in how to do that step by step. If people want to learn more, where can they find you guys?

**Aakash Gupta** (01:03:25)

So the URL for the course, you can go to evals.info and you can find the course there.

**Shreya Shankar** (01:03:31)

Yeah. Or follow us on X. Our websites are on the internet. You know, if you just look us up, we're there. But check out evals.info. I think we've really tried to put together as much information that we can to be freely accessible and available to folks. So take a look where you can dive in and I'm sure you will learn things along the way.

**Aakash Gupta** (01:03:51)

Awesome. Thank you guys so much for being here. One thing I want to clarify is, so we mentioned like, hey, you need to look at traces in production. So you might be wondering, like, what if your application is not in production? What do you do? What if you don't have data? What if you don't have traces? Where do you get them? One, try to recruit some friends. Try to dog food your own app. That's the best thing. For whatever reason, if you're not able to recruit friends, you're not able to dog food your product, which would be kind of sad, but let's say, you know, there could be valid reasons you're not able to do that. You can generate synthetic inputs into your system. And there's a way to do that correctly is kind of what you're doing is you're pretending to be a user. You're having an LLM simulate that at scale.

**Aakash Gupta** (01:04:37)

That's one of the things that we go into in our course as well. So there's ways to bootstrap yourself, but you do need to look at data.

**Hamel Hussian** (01:04:43)

Amazing. Thank you guys so much for being here.

**Shreya Shankar** (01:04:46)

Cool. Thanks for having

**Hamel Hussian** (01:04:48)

me. I hope you enjoyed that episode. If you could take a moment to double check that you have followed on Apple and Spotify podcasts, subscribed on YouTube, left a rating, a review on Apple or Spotify and commented on YouTube. All these things will help the algorithm distribute the show to more and more people. As we distribute the show to more people, we can grow the show, improve the quality of the content and the production to get you better insights to stay ahead in your career. Finally, do check out my bundle at bundle.akushg.com to get access to nine AI products for an entire year for free. This includes Dovetail, Mobbin, Linear, Reforge Build, Descript, and many other amazing tools that will help you as an AI product manager or builder succeed. I'll see you in the next episode.
