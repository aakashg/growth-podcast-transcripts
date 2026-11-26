---
title: "She went from IC PM to CEO of $550M AI company Descript in 3 years"
subtitle: "Laura Burkhauser went from IC PM to CEO in 3 years. Here’s a deep dive into the AI features she shipped, and how you can do the same."
date: "2025-12-15"
host: "Aakash Gupta"
guests: ["Laura Burkhauser"]
speaker_names: "substack"
substack_url: "https://www.news.aakashg.com/p/she-went-from-ic-pm-to-ceo-of-550m"
youtube_url: "https://www.youtube.com/watch?v=LR_WOmcE9WI"
duration: "00:44:30"
word_count: 7906
source: "Substack episode transcript (aired audio)"
sponsors:
  - name: "Maven"
    url: "https://maven.com/x/aakash"
  - name: "Pendo"
    url: "http://www.pendo.com/aakash"
  - name: "Vanta"
    url: "http://vanta.com/aakash"
  - name: "NayaOne"
    url: "https://nayaone.com/aakash/"
  - name: "Kameleoon"
    url: "http://www.kameleoon.com/"
---

**Sponsors:** This episode is brought to you by [Maven](https://maven.com/x/aakash), [Pendo](http://www.pendo.com/aakash), [Vanta](http://vanta.com/aakash), [NayaOne](https://nayaone.com/aakash/) and [Kameleoon](http://www.kameleoon.com/).

# She went from IC PM to CEO of $550M AI company Descript in 3 years

*Laura Burkhauser went from IC PM to CEO in 3 years. Here’s a deep dive into the AI features she shipped, and how you can do the same.*

**Laura Burkhauser** (00:00:00)

The best products out there, they don't just do a job for you. They transform how you feel about yourself.

**Aakash Gupta** (00:00:05)

How did you get promoted from VP to CEO? What do most PMs who want to rise miss? You started as an ICPM and ended up becoming the CEO at Descript. Meet Laura Burkhauser. She shipped AI features at Descript that were so successful that Andrew Mason, the founder of Groupon, made her CEO. How did you measure success for the AI tools?

**Laura Burkhauser** (00:00:23)

We looked at adoption and retention.

**Aakash Gupta** (00:00:25)

How did you roll this out to users and develop confidence that this should go out to everybody?

**Laura Burkhauser** (00:00:29)

A lot of it was human driven evals. I'm going to test this out a bunch of production data and see if I would use the result as a customer.

**Aakash Gupta** (00:00:37)

What is the role of the PM on an AI feature like this?

**Laura Burkhauser** (00:00:40)

You and only you are qualified to write the eval criteria for what like a good job looks like.

**Aakash Gupta** (00:00:49)

How did you land the job to begin with?

**Laura Burkhauser** (00:00:51)

I did what you do when you don't know what you're doing with your life in the Bay Area and I started a podcast and that's how I found Descript. I emailed them and I just asked if they were hiring PMs. I hadn't been in AI before and I thought that I had some skill in product management and leadership and strategy.

**Aakash Gupta** (00:01:06)

What are the tips you have for PMs in managing that founder relationship?

**Laura Burkhauser** (00:01:10)

You need to have the humility to understand that they probably do know their customer a lot better than you do.

**Aakash Gupta** (00:01:19)

Really quickly, I think a crazy stat is that more than 50% of you listening are not subscribed. If you can subscribe on YouTube, follow on Apple or Spotify podcasts, my commitment to you is that we'll continue to make this content better and better. And now on to today's episode. Laura, welcome to the podcast.

**Laura Burkhauser** (00:01:39)

Thanks so much for having me. Excited to be here.

**Aakash Gupta** (00:01:42)

I want to get right into it. What were the features that you shipped that led to you getting promoted to CEO?

**Laura Burkhauser** (00:01:50)

Yeah, well, for folks that don't know, Descript is an AI video editing tool that allows you to edit your video just like a doc. And that's how I would have introduced it a few years ago when I joined. I didn't really know what I was looking to do at the time. And I started a podcast with my friend. And when I went to go edit that podcast, I found this software that I totally fell in love with, Descript. Suddenly, I was a podcast editor. Then I became a video editor. The best products out there, they don't just do a job for you. They transform how you feel about yourself. And that's what Descript did for me. So I knocked on their door and I said, hey, are you guys hiring product people?

**Aakash Gupta** (00:02:31)

So what was the timeline of this feature? When did you guys realize, okay, retakes is one of the first use cases we want to build. How did you guys experiment with LLMs and the prompting to figure out, okay, we can actually solve this? Because I know, especially back then, one of the big concerns was like context window. Can we even put in a whole podcast transcript into an LLM? It was a lot less possible back then. And then how did you guys eventually roll it out to users and have the confidence to ship it to everybody?

**Laura Burkhauser** (00:03:01)

Right. Like with the context window, how we had to solve that problem was like, can we send it over in chunks? And then like, okay, that works for remove retakes, right? Because usually you can send it over in chunks that are meaningful enough that you can detect retakes. But that was a problem for, for, uh, for buttons that you would assume would be able to contain a longer context window, like something like rewrite, where really to rewrite, you probably want to understand the complete journey before you rewrite it. We definitely had to understand the limitations of the technology at the time. You asked, how did we decide on the use case? Well, I think one of the great things about Descript is we already had a really deep understanding of customer problems, right? At this point, we had been around for a couple of years. We had watched people person after person, you know, go through the multi-hour process of editing a video.

**Laura Burkhauser** (00:04:07)

And we kind of understood, okay, you have like your script readers and you have your improvers. Script readers will have one of two problems. Either they're reading off a script like this, in which case the problem that they have is that they're not looking at the camera. or they're reading off a script and then like looking into the camera and delivering just that one sentence and often screwing it up. And so for that first kind of reader, we looked around and found a model called eye contact that we integrated into Descript.

**Aakash Gupta** (00:04:39)

Okay. If I'm somebody trying to take the lesson from this, we have our clear mental model of what are some of the user problems that we aren't solving today. In this case, some of them are eye correction and removing retakes. And then we're looking at what becomes recently possible with the advent of LLMs, maybe like being able to actually identify what those retakes are and this new model being released around eyes. incorporate that into our product. How did you roll this out to users and develop confidence that this should go out to everybody?

**Laura Burkhauser** (00:05:12)

Yeah, so for AI tools, what we did was, you know, if you have a toolbar, you need more than one thing to be part of that toolbar. So when we announced the idea of Underlord, which is what we used to call this, but when we announced the idea of the AI toolbar, we thought like, what are six killer apps that could be part of this toolbar based on problems that customers have, problems we think we could solve well with the technology or problems that we don't think we can solve well with the technology today but we think that over the next few months as the context window increases or whatever like the existing like we were at an age then also where it felt like every two weeks things got step change better i feel like now we're sort of in like the boring part where it's like things are pretty good and each new model release is just like incrementally better than the last.

**Laura Burkhauser** (00:06:07)

I hope I'm wrong and we get another banger in a month or two, but I feel like the last few it's been like, eh, okay. Anyways, things were changing so quickly that we also did have a rolling backlog of like, this is a really great idea, but it's blocked because of technological limits right now. But we've already thought through a lot of how the product will work so that as soon as the technology is ready, boom, we're ready to go. And so we kind of had that mapped out in our mind and we had six that we wanted to go to market with. I believe those were edit for clarity, remove filler words, remove retakes, add chapters, and then a bunch of these published ones because they're really easy, right? From like a technology perspective, you need to write a good prompt, but like drafting a title, summarizing, show notes, YouTube description.

**Laura Burkhauser** (00:06:58)

social posts, blog posts. Those are pretty easy to do. The brainstorming ones, somewhat easy to do too. Those were the ones we went to market with first. You asked how we made sure they were good enough. This was before there were a gazillion thought pieces about how evals ought to work. But a lot of it was human-driven evals, but by another name, where you're like, okay, I'm going to test this out on a bunch of production data and see if I would use the result as a customer, and I would ship it, and if I wouldn't, don't ship it.

<!-- sponsor -->
**Aakash Gupta** (00:07:41)

Today's episode is brought to you by Maven. The problem with most courses online, like Udemy, is there's no live component and the instructors aren't experts in their fields, they're professors. At Maven, you get direct live access to experts and operators from the world's best tech companies. You can't get that access anywhere else, in any university, and you usually can't find them on YouTube either. I featured so many of Maven's experts in the newsletter and podcast for that reason. To help you out, I've put together a collection of courses I recommend at maven.com slash x slash Akash. This includes courses like AI prototyping for PMs, product sense for PMs, and getting an AI PM certification. Visit it now at maven.com slash x slash A-A-K-A-S-H. Today's podcast is brought to you by Pendo, the leading software experience management platform. McKinsey found that 78% of companies are using Gen AI, but just as many have reported no bottom line improvements.

<!-- sponsor -->
**Aakash Gupta** (00:08:41)

So how do you know if your AI agents are actually working? Are they giving users the wrong answers, creating more work instead of less, improving retention, or hurting it? When your software data and AI data are disconnected, you can't answer these questions. But when you bring all your usage data together in one place, you can see what users do before, during, and after they use AI. Showing you when agents work, how they help you grow, and when to prioritize on your roadmap. Pendo Agent Analytics is the only solution built to do this for product teams. Start measuring your AI's performance with Agent Analytics at pendo.io slash akash. That's p-e-n-d-o dot i-o slash a-a-k-a-s-h. so did you guys stage the rollout did you create like a closed beta or something because sometimes that production data is the most important thing and creating synthetic versions in your room you don't always replicate the funny things a user might do out in the field

**Laura Burkhauser** (00:09:31)

yeah now we have a lot of production data that we can that we can work with right um we use descript a ton we're like very intentful users and and i'd say like For these ones, they were pretty straightforward. So yes, the answer is yes, we did launch them as a beta. We didn't do private beta. We felt good enough to immediately go to public beta. But honestly, these were pretty straightforward. And while we continued to tweak them and sometimes ran A-B tests when we tweaked them, that felt much safer than when a year later, this past year, we launched this, we launched Underlord, your agentic co-editor who can do things in objective-based, who's kind of like an open-world agent. And when you have a truly open-world agent where people can type whatever they want to into Underlord, the really great part of that is the emergence.

**Laura Burkhauser** (00:10:30)

My favorite part about building AI products is emergence and having the kind of product that allows for emergence. But if you're allowing for emergence, you're also allowing for a lot of like whack stuff to happen in your product. And so that's where production data is really important.

**Aakash Gupta** (00:10:50)

So before we get even deeper into Underlord, which we have to really diagnose for people how you guys built this open world agent, how did you measure success for the AI tools?

**Laura Burkhauser** (00:11:00)

Yeah. So we, you know, we looked at adoption and retention, um, obviously like more complicated than that. We have like, I don't know if I got one of these, we have like a little, did you, we have a thumbs up, thumbs down, um, that we can also use for training. Um, but, but mostly what we did was what success meant was, does this have, uh, remove filler words was the very first, uh, action that we launched and it actually used to live elsewhere. And it was one of our most popular features in the product and just a big success commercially for us as well. And so we use that as our baseline, like how does edit for clarity compare with remove filler words when it comes to adoption? And then even more importantly, when it comes to retention, because if this is a useful, if this is a useful AI tool, then people will use it over and over again.

**Laura Burkhauser** (00:11:53)

And the other thing that you can look at is like, not just did they apply it, but did they export with it, with whatever it did in the export?

**Aakash Gupta** (00:12:03)

So was it up to their quality by that they wanted to include it in their final product, which makes a lot of sense. So what were the teams behind this? How did you guys staff this and how should people be staffing it? Because I keep hearing a lot of concerns around what is the role of the PM? Is it blurring with designer and engineer? What does the PM specifically own on an AI feature like this?

**Laura Burkhauser** (00:12:26)

Yeah, it's a really fun time right now in EPD because just theories abound about like which of these jobs are going to make it, which of these jobs are going to become the same job. Are we going to need engineers in the future? Are we going to need PMs in the future? Are we going to need designers in the future? Anyways, whole long, beautiful monologue we can go off on. there, but I do think our roles are changing. And the role of the PM in a product like this is the same and different. So as a PM, you always need to understand your customer and what success looks like for your customer, what the job they're doing is, what the needs they have while they're doing that job are, how they solve that problem currently, right? All that good product thinking. And because you have all that good product thinking of job, circumstance, needs, alternatives, You and only you are qualified to write the eval criteria for what a good job looks like, what a you did the job, but I'm not going to say you did it well job looks like, and what a you broke my product, you broke my video looks like.

**Laura Burkhauser** (00:13:41)

You're the one who is best able to really codify that.

**Aakash Gupta** (00:13:45)

So like we've been hearing from a lot of people, the PM is really important in evals, although they may not be the only person involved in evals. They, like many other products, they need to bring the right experts in to look at those things. Maybe it's an audiophile, in your guy's case, for audio features. What exactly is the output of a PM? You mentioned evaluation criteria, because there are these evaluation platforms nowadays and observability platforms, and there's the system prompt for the LLM judge that you're literally using. What is the evaluation criteria should pms be writing out what good examples are a few shot examples what what should that tangibly look like

**Laura Burkhauser** (00:14:23)

i don't think that it is doing anything in a tool um personally like at least like we have our um our engineering team our research team kind of handles like literally setting up the the tool to do the eval but where the the role that the pm plays in setting up our evals is in setting up the decision criteria for what pass what high pass, pass, and fail looks like for different queries. We randomly select representative queries across real production data and don't share those with engineers, but we do share them with the PM who then says, for these randomly selected queries, here's what success looks like. Then this goes into training eventually the LLM judge. First, we have a human judge it and make sure that they really like the criteria. Then we have a human and an LLM both judge it and we see, does the LLM agree with the human or does the LLM disagree?

**Laura Burkhauser** (00:15:23)

In which case we may have a tiebreaker. Tie often goes to the human for now. Maybe I look forward to the day that I'm like, actually, Alex, I think the LLM had this one. Then eventually we delegate to the LLM. Okay.

**Aakash Gupta** (00:15:43)

And then were there any lessons in the audio tools feature sequencing or any failures along the way that we could learn from? I

**Laura Burkhauser** (00:15:52)

mean, I think that... Yeah. There. Okay. Yes. I have a good, I have a couple of good failures. You can, you can learn from here. One of them is, you know, I told you that we used to have this real audio file, um, who was just using judgment. And then when he left vibes, as we call it on the internet. And then when he left, uh, we tried to turn that into a, uh, a list of criteria. And one of the things that we realized after getting to what I think was a worse model is that we were not clear about what the use case was. So I believe, given the information that I have now, and I reserve the right in AI to update my perspective every day, certainly every quarter, Right now, I believe that there will not be one model to rule them all, but that we're going to find that different models handle different specific use cases better and some worse.

**Laura Burkhauser** (00:16:55)

And so with Studio Sound, we got to what I think was a worse model for our users because our evaluators were using sample data that was really bad audio. Like, wow, someone is vacuuming in the room while I'm doing this podcast. And what's going to help remove that right next to Laura person vacuuming? And it turns out that the model that is the best at making terrible sound sound good, and the model that is the best at making okay sound sound good are different models and what I mean by okay sound is like hey I don't have a sure microphone what I have is a laptop and I'm not wearing headphones and I'm kind of just talking into my computer like this and studio sound is best for that and that's the most common use case right like that's why people use it it's because like I'm recording my podcast and I don't want to buy a $900 microphone and so What we needed to do was make sure that we had sample data when we did the evals that was representative of what our actual use case that we wanted to nail was and to care a little bit less about like, wow, there's a jackhammer right outside my window going.

**Laura Burkhauser** (00:18:10)

Does that make sense?

**Aakash Gupta** (00:18:12)

Yep, 100%. So that's AI tools. As you previewed Overlord, your agent is really the next frontier. This was as agents, everybody is now trying to ship an agent to their product. So talk to us a little bit about how you guys developed this feature and what the life cycle was of getting it out into the public.

**Laura Burkhauser** (00:18:33)

Yeah, so this is a much harder thing to build. So Underlord, just quick correction, Underlord, not Overlord. Oh, wow. Because nobody wants an AI overlord, right? But couldn't you use an AI underlord to do your bidding? And that's how we like both positioned underlord in the market. And that's how we find that a lot of people want to work with an AI assistant in creative spaces is like, I am the creative and Underlord, you can be my brain buddy and you can execute on what I say, but I'm in control and I want to maintain creative fulfillment from building this thing. Creative fulfillment is really important for our customers. But so what Underlord does is, whereas an AI tool can do 28 things really well, as soon as you start to want it to do something else, you're just SOL, like you have no options. And so where this really started to come to a head was with this very popular feature we have called Create Clips.

**Laura Burkhauser** (00:19:34)

And what Create Clips does is if you have a long form video, a webinar, a podcast, probably you want to create some social clips to complement that to help you market it.

**Aakash Gupta** (00:19:45)

Okay. And so how did you guys roll this out and iterate and improve on this over time? Were there failures along the way?

**Laura Burkhauser** (00:19:54)

Yes. So yeah, this is a much harder thing to build. And I'd say like, we are still, I think like, we're still in the middle of building Underlord because it's pretty good now. But I think, well, I don't want to get too technical, but I think right now it's on a harness that is still too brittle for it to be as open world and to be able to take advantage of leaps in general intelligence enough for it to be like, yeah, exactly what we want. And so we call this the mouse version and we're building the mammoth version. There's like a company right now that's trying to incubate a woolly mammoth. And the best they've done so far is a woolly mouse. And so I'm like, this is like a woolly mouse. It's cute. It's useful. I love it. But it's not majestic yet. And the mammoth is what we're trying to build right now.

**Laura Burkhauser** (00:20:52)

So what was the process to doing this? Well, first, we needed to decide on the scope. And is this going to be a depth agent that can do one thing with great depth? Or is this going to be a breadth agent that can really work across all of the tools into script? And we decided on the harder one, as we often do. One of our core principles is that we're not a point solution. Descript should be a video editor that can really address every kind of video, whether it's a short, whether it's like long form horizontal, whether it's like a podcast, all of those things should be supported by Descript. And so all of those things need to be supported by Underlord. Well, okay, so now what you need to do is you need to give your agent the level of context that it needs to understand and work with the customer.

**Laura Burkhauser** (00:21:46)

And then you need to give it the tool coverage that it needs to be able to do all of the things that you want Underlord to be able to do. And then you need to build a report card or eval system so that we can know where it's good and where it's bad. And eventually, it can teach itself to get... better, right? That's the dream. And I'd say we're like, we're on that on that journey right now.

<!-- sponsor -->
**Aakash Gupta** (00:22:13)

Okay. Today's episode is brought to you by Vanta. As a founder, you're moving fast toward product market fit your next round or your first big enterprise deal. But with AI accelerating how quickly startups build and ship, security expectations are higher earlier than ever. Getting security and compliance right can unlock growth or stall it if you wait too long. With deep integrations and automated workflows built for fast-moving teams, Vanta gets you audit-ready fast and keeps you secure with continuous monitoring as your models, infra, and customers evolve. Fast-scoring startups like LinkChain, Writer, and Cursor trusted Vanta to build a scalable foundation from the start. So go to Vanta.com slash Akash. That's V-A-N-T-A dot com slash A-A-K-A-S-H to save $1,000 and join over 10,000 ambitious companies already scaling with Vanta. Today's episode is brought to you by Naya One. In tech buying, speed is survival. How fast you can get a product in front of customers decides if you will win.

<!-- sponsor -->
**Aakash Gupta** (00:23:16)

If it takes you nine months to buy one piece of tech, you're dead in the water. Right now, financial services are under pressure to get AI live. But in a regulated industry, the roadblocks are real. Naya One changes that. Their air-gapped, cloud-agnostic sandbox lets you find, test, and validate new AI tools much faster. From months to weeks. From stuck to shipped. If you're ready to accelerate AI adoption, check out Naya One at nayaone.com slash akash. That's N-A-Y-A-O-N-E dot com slash A-A-K-A-S-H. Today's episode is brought to you by the experimentation platform Chameleon. Nine out of ten companies that see themselves as industry leaders and expect to grow this year say experimentation is critical to their business. But most companies still fail at it. Why? Because most experiments require too much developer involvement. Chameleon handles experimentation differently. It enables product and growth teams to create and test prototypes in minutes with prompt-based experimentation.

<!-- sponsor -->
**Aakash Gupta** (00:24:16)

You describe what you want, Chameleon builds a variation of your webpage, lets you target a cohort of users, choose KPIs, and runs the experiment for you. Prompt-based experimentation makes what used to take days of developer time turn into minutes. Try prompt-based experimentation on your own web apps. Visit chameleon.com slash prompt to join the waitlist. That's K-A-M-E-L-E-O-O-N dot com slash prompt. So these are the features. They really worked. I'm curious, what can you share by the way? Like what sort of metrics are you guys seeing? Like uptake adoption of these? Like, how did you really quantify success?

**Laura Burkhauser** (00:24:56)

Yeah. So, um, We didn't start to try to quantify success until we got to like a public beta, until we released it to everyone. I think that our stages were, first we had a series of regression tests that we ran across. When we decided we wanted Underlord to be a breadth agent, we came up with a whole bunch of stuff that we thought it ought to be able to do that covered the extent of what a person might want to do in Descript. Obviously, that can't be 100% representative. And like I said, it never will be in a world of emergence. But we have a framework for how we think about the kinds of jobs that customers do in Descript. And so first, we started with just like, you know, your classic PM, like, customers should be able to blah, blah, blah, blah, blah, blah, blah, blah, while we were just building tool coverage.

**Laura Burkhauser** (00:25:56)

Then we really rushed to get into a private alpha. So we were building with real customers because it's really hard to build this stuff well as long as you're using toy data. You need to get real data from real people who will talk to your agent not using the language that you, a person who works at Descript, does, but using the language that a person out there in the world will. And we purposefully tried to get an alpha where we had some people who were quite sophisticated at video editing and some people who were not at all sophisticated at video editing and some people who were quite sophisticated at AI. and some people who were not at all sophisticated at AI so that we could understand like, oh, if a person is really sophisticated about both video editing and AI, this is the kind of experience they might have.

**Laura Burkhauser** (00:26:51)

If someone is not very sophisticated about either, their prompt might just be like, edit this video and make it better. And it's like, okay, what do we do with that prompt? Right? So once we got real customer data, then we were able to organize that customer data into a series of regression tests to be like, okay, when people want to apply layouts, here's like 30 representative queries that they might ask. And this was pre evals. These are just regression tests. So we showed those to engineers and we actually just like ran bug bashes on those queries for a while. And that helped us understand like, OK, where is this agent getting things wrong? Where do we need to tweak the prompt or tweak the way that we would like set up the tool in order to get these things to work? Now, what anyone who built these things will tell you is like, that's great, but you're probably overfitting to the prompts that you're exposing to your engineers.

**Laura Burkhauser** (00:27:47)

And indeed, we did. But that also meant that we had something good enough that we were starting to see that our beta users really liked it because it was working for their use cases. So then we're like, okay, let us try this out with new customers and see if it helps them activate. Because as you know, video editing is hard, right? It's hard. And the biggest problem that we have as a piece of software, as an app, is that A lot of people really want to edit video when they get to Descript, and they try, and they just can't get over the hump. And so we're like, OK, is the agent, is Underlord as it exists now, better at getting new users over the hump than the activation experience that we have right now? And it was. And so we were like, okay, then we should give this to new users.

**Laura Burkhauser** (00:28:50)

And so for a while, we gave it to new users, and then we had it so that any user could opt in, right, if they wanted to. And so we had it in that state for a while. And then that gave us even more data and more time to like start setting up our evals and start automating those, make the agent better, and eventually make it kind of the default experience for everyone.

**Aakash Gupta** (00:29:15)

Wow. And now I believe if I go to the Descript homepage, I'm going to be seeing Underlord, that chat box, as the top thing. So it's really elevated itself to the central part of Descript's experience.

**Laura Burkhauser** (00:29:24)

Yeah, I'd say that right now we have a bifurcated set of customers. So there are people who don't use Underlord at all, right? And these people often... already, like they're using Descript because the editor that we have, the human editor that we have is like exactly what they want. And we love those customers. Some of them then become hybrid users where they could do everything themselves, but they find like, wow, if I need to change 17 transitions, I would really rather just tell Underlord, can you make all of the transitions wipes instead of crossfades? And Underlord is great at bulk editing like that. Or like a podcaster might say, every time Laura is monologuing for more than 30 seconds, can you just show her? But then for the rest of the time, show both her and Akash or whatever. Whenever she's referencing something on the screen, can you make sure that the screen shows up?

**Laura Burkhauser** (00:30:21)

Otherwise, never show the screen. That's like something that's very useful that Underlord can do, even if you know how to do it, because like you don't want to do that for 45 minutes of tape. Then you have this new group of customers that are just like Underlord native. That is how they think about Descript. And they're willing to prompt and reprompt like three to four times because they don't wanna learn video editing. And I know who this customer is because this is me and how I use cursor, right? I'm never gonna suddenly become a software engineer. I'm just gonna keep talking to this thing, keep talking until I get the result that I want, you know?

**Aakash Gupta** (00:31:02)

love it so taking some models from those other successful agentic products in the coding space applying that mental use case to your own product then seeing how to apply it to your product so that about completes it into our deep dive into the features that's one element of making it from icpm to ceo but it's not all just about your track record a lot of it is about you and so i want to dive into you and i actually want to start pre-Descript. What are the relevant things about your career history? You were a management consultant, you worked at Twitter. What were the relevant points and things that really set you up for the success you saw once you got to Descript?

**Laura Burkhauser** (00:31:44)

Yeah. So I think like, you know, we're all PMs and we know that the pathway to product is windy and strange. And we all come, some of us come from engineering, some of us come from you know, design. I love to shock people by telling them that I majored in German literature, which just feels, you know, to many people in tech, like the most useless thing you could possibly do with four years of your life. I loved it. And when I found out I did not want to be a German literature professor, though, I did what a lot of kind of smart generalists did at the time. And that was I went into management consulting. And I think that management consulting was a really, really great place to start my career, even though, oh my gosh, I did not much like the job after I kind of learned it.

**Laura Burkhauser** (00:32:37)

I think either you've got like consultant's blood in you or you don't. And I'm someone who just like has too much of a desire to like own and like operate to like be okay leaving it at the slide deck. I think some people much prefer to leave it at the slide deck. They're like, great, I came up with a strategy, like bye. But in any case, I was a management consultant, and I think I really learned how to be strategic there. Basically, your job, if you're a junior management consultant, is to sit in the room and take notes while smart, very senior people talk a lot about how they're going to make difficult strategic decisions. I think that just teaches you how they think. That's actually their talent model. So it's a really great place to start your career. But then I'm so thankful, I'm daily grateful that I was put on the weirdest project that you could be put on in a management consulting firm, which was to help spin up an online learning platform for this firm so that they could reach people that weren't ready or able yet to get five people on site co-working with them.

**Laura Burkhauser** (00:33:41)

but still wanted some of that strategic information. And as I went to build this learning platform, I was like, first of all, I just moved to the Bay Area. I was like, here's how I was thinking we could build this because I'm reading a book right now that's telling me about this. What if I built a prototype in two weeks and we just kind of showed it to people and found out what they liked and didn't and then adjusted it. And I had like an awesome boss who was like, yeah, you should you should do that. That sounds great. And in so doing, I think we built a really great product for the firm I was working at. And I realized like, oh, I would like this job so much more than I like that other thing I was doing. So what is this? Can I just do this for the rest of my life?

**Laura Burkhauser** (00:34:23)

And here I am. So I think that was really meaningful, both the experience to get that strategic kind of like, here are the kinds of questions that leaders struggle with, but then also to get that experience of like, here's what it feels like to ship and have customers and have them tell you that they love you and they hate you and have that drive you to feel better. Yeah, so that was a really, really important first part of my career. Then I found start, like the second chapter is probably finding out that startup to me was where my heart went. I think like one of the decisions you need to make in your career is like, am I a big company PM or am I a small company PM? And you're just gonna feel that in your gut as soon as you try both. Uh, you know, so you'll end up at the job you end up in, but if you start small and it doesn't feel right, you should go to a big company next.

**Laura Burkhauser** (00:35:15)

Uh, if you start big and it doesn't feel right, go to a small company next. I worked at Amazon, uh, and was like, no, this is so, this is too big. I could get hit by a bus and like, no one would even know for 11 months because that's how small my scope is here. Even though I love the people there. Um, so then I worked at a seriously startup as the first on the ground PM. And I was like this, I'm addicted to this feeling of like having my fingerprints on everything and building really quickly and being experimental and seeing what works and not having bureaucracy. And so I took that train as far as I could take it. But then I kind of hit this barrier where I wasn't learning as much as I needed to to be as good as I needed to at the job that I had at the time, which was an org leader.

**Laura Burkhauser** (00:36:01)

By the way, like org leader is a classic crisis moment in a PM's career. because probably you're a pretty good PM, largely self-taught. I was a pretty good people manager, largely self-taught. That's just like I thought about it and had empathy or like I thought about it and did good work. Once you're an org leader, That job is really hard. There's not like a clear one right way to do it. And there's often not a lot of people to learn from, especially at the startup. So I had to go to a big company to figure out how to be an org leader. And I'm grateful to the org leaders I learned from there at Twitter, where I was for three years. But after three years, I like being at a big company for that long. I knew I needed to get back in, back in the game, back in the startup game.

**Aakash Gupta** (00:36:47)

that's when you already referenced you knocked on the door of descript i think there's an interesting story in there how did you land the job to begin with and what was the role

**Laura Burkhauser** (00:36:56)

yeah um i think my advice to uh to product managers at least if you're like me is don't be strategic about your career at all you know just go where your heart takes you um but that's actually um the second time in my career that i just cold called an org and said i love your product give me a job please And what had happened is I left Twitter and I didn't really know if I even wanted to be in tech anymore because this was right before ChatGPT came out. And so sort of presciently, I was like, is anything interesting happening in tech anymore? Like, what's going on? I didn't want to be in social. I didn't want to be optimizing for clicks and likes. I was tired of that game. It pays so well. I was not interested in it. And so I did what you do when you don't know what you're doing with your life in the Bay Area.

**Laura Burkhauser** (00:37:43)

And I started a podcast. and that's how I found Descript. It was that feeling for me of just like, wow, this is why I got into product management. And so I emailed them, and I just asked if they were hiring PMs. I'd been a director at Twitter, but I really wasn't optimizing for title, and I wasn't optimizing for money. I was optimizing for learning. I hadn't been in AI before. I hadn't been in this deep workflow software before, even though I loved being in it as a customer. And I thought that I had some skill, though, in product management, in leadership, in strategy, in measurement, that I could lend to a startup that's kind of building out its PM bench. And so they hired me, and pretty quickly I became the VP of product.

**Aakash Gupta** (00:38:38)

Tell us a little bit more about that progression from IC to CEO. Obviously, you're the one who's making the progression, not the one judging the results. So you're going to have your own point of view. But from your point of view, what were the things you were doing well that gave them increasing confidence that we should keep giving her more and more responsibility?

**Laura Burkhauser** (00:38:57)

Yeah, I mean, I think at like a founder-led startup, a lot of it really just comes down to, are you someone who can understand the founder's vision and help make it better and make it happen, right? And I think that this is something like a lot of founders, when they're hiring their first head of product, don't know Totally what they're going to get into and what it's going to be like to share power with that person, because like a lot of founders are the head of product. Yeah. And I think what really worked about like Descript and like with me and Andrew is like. He didn't hire me as a head of product and then run into all of these weird power struggles. He hired me as a PM and I think found that he liked having me in the room when he was making decisions about the product strategy.

**Laura Burkhauser** (00:39:50)

And when you're in the room and someone likes having you in the room, after a few months, you permanently belong in the room. And so I think that that's kind of what happened is I got hired as an ICPM and then found myself invited to more and more rooms until I was invited to the room, right?

**Aakash Gupta** (00:40:10)

A lot of ICPMs, they're trying to do that, right? They're trying to get invited to the room, but reality sets in like, you know, they ship a feature where the founder gave them some latitude and it wasn't close enough to the founder's vision. Then the founder starts to micromanage their roadmap a little bit more, and it usually spirals out of control from there. What are the tips you have for PMs in managing that founder relationship?

**Laura Burkhauser** (00:40:38)

Yeah, that's a really good question. I mean, I think that you have to ask yourself, if I'm the founder of something, why in the hell should I trust you more than I trust myself? You didn't build this, right? You didn't sacrifice the things that I sacrificed to build the first seven versions of this. And so you need to understand that what you're coming into is someone who has gotten very far by trusting their own instincts. And you need to have the humility to understand that they probably do know their customer a lot better than you do. And they know the product better than you do. And so you have to ask yourself then, how do I gain the credibility that this person starts to trust my instinct as well? And I think that's by like using the product, use the product, know the product, be able to speak credibly to what it feels like to use the product, talk to customers, be able to speak credibly to what existing customers want and what the customers that you wish were using the product want.

**Laura Burkhauser** (00:41:43)

Right. And so like a lot of it is just like get smart, earn your way into the room by like learning the hell out of the product and learning the hell out of the customers and learning the hell out of the business. And I think like so that's probably not satisfying, but I think a lot of people try to skip that step and just like be really impressive and like work really hard. It's like, OK, first get command, get enough command over the product and the customer that you earn the trust. And when you say something, someone just like mentally puts in their head like smart. Uh, and, and then they'll invite you into more rooms. And then I'd say like another mistake people make though, is they're so eager to get into the strategic rooms. They start doing a lot of strategic work and they let this part of their job, like kind of like fall apart where it's like, oh yeah, I'm doing a lot of strategic planning, but I actually don't know what the engineers on my team are working on.

**Laura Burkhauser** (00:42:34)

I think we're going to have that done in Q3 and it's just like unacceptable, right? Like you need to be deep in the details of like the ICPM work that you're doing and excelling at that before you're really going to come in and be invited to like plan out what next year looks like. And so like that's the other way that you earn credibility is like you ship, you ship, you got to ship.

**Aakash Gupta** (00:42:56)

which is why we spent the first 40 minutes of this episode on what Laura shipped. Laura has given you guys all the masterclass, okay? This is how you build AI features, AI products, an AI company that's valued at over 550 million, and I bet if it raised now, it would be worth several billions. My words, not hers. And so if you want to do that, if you want to rise to VP of product, to CEO, take some of her lessons to heart. Don't necessarily be so strategic about your career. Make sure that you love the product. You really understand the product and you ship features that just rock, that just work. We use those features at the podcast for that reason. Laura, thank you so much for building those features and thanks for being on the podcast.

**Laura Burkhauser** (00:43:38)

Thanks for having me. Really awesome conversation. All

**Aakash Gupta** (00:43:41)

right, everybody. See you later. So if you wanna learn more about how to shift to this way of working, check out our full conversation on Apple or Spotify podcasts. And if you want the actual documents that we showed, the tools and frameworks and public links, be sure to check out my newsletter post with all of the details. Finally, thank you so much for watching. It would really mean a lot if you could make sure you are subscribed on YouTube, following on Apple or Spotify podcasts and leave us a review on those platforms. That really helps grow the podcast and support our work so that we can do bigger and better productions. I'll see you in the next one.
