---
title: "Behind v0 (Top AI Prototyping Tool): Tutorial and Story from the CPO in 2026"
subtitle: "In today's very special episode, we sit down with the CPO of Vercel to learn how they build product, the future of AI prototyping for PMs & designers, and a tutorial of v0. "
date: "2025-06-11"
host: "Aakash Gupta"
guests: ["Tom Occhino"]
speaker_names: "substack"
substack_url: "https://www.news.aakashg.com/p/tom-occhino-podcast"
youtube_url: "https://www.youtube.com/watch?v=-n8T6S_sD7Y"
duration: "01:15:15"
word_count: 13191
source: "Substack episode transcript (aired audio)"
---

# Behind v0 (Top AI Prototyping Tool): Tutorial and Story from the CPO in 2026

*In today's very special episode, we sit down with the CPO of Vercel to learn how they build product, the future of AI prototyping for PMs & designers, and a tutorial of v0. *

**Aakash Gupta** (00:00:00)

Tom O'Kino, you are the CPO of Vercel, one of the hottest companies in AI and the makers of vZero, which everybody I know is talking about for AI prototyping. How big is vZero? What numbers can you share with us?

**Tom Occhino** (00:00:13)

Yeah, vZero has been used by about 2 million people since last year, and we're growing really, really fast. Even if you're not an engineer, even if you're non-technical, the era of personal software is absolutely upon us. And this has been the most exciting thing for me. I really don't think about the competition. I think about our customers and delivering as much value as I can. And I also think about my own use case. What are the other AI things you're using as a CPO in your

**Aakash Gupta** (00:00:40)

day-to-day that help you? Why should I watch this episode?

**Tom Occhino** (00:00:45)

In this episode, we're going to talk about V0 as a tool, how to use it to transform not just the way you do your job. And then we'll talk about how the team that builds V0 built it, how they use it themselves, as well as more generally, Vercel's strategy for and approach to product development. An AI

**Aakash Gupta** (00:01:03)

startup valued at $3.25 billion. In today's episode, we're gonna walk through a live demo of their hit product V0, which is one of the leading AI prototyping tools on the market. We're gonna talk about how Vercel builds product, how V0 uses V0, and the future of product management in the era of AI prototyping. So if you're a product manager, designer, or engineer, or even just someone founder using AI prototyping tools, there's a lot to learn. So let's get started. Really quickly, I think a crazy stat is that more than 50% of you listening are not subscribed. If you can subscribe on YouTube, follow on Apple or Spotify podcasts, my commitment to you is that we'll continue to make this content better and better. And now on to today's episode. Tom Occhino, you are the chief product officer at Vercel, one of the hottest companies in AI and the makers of V0.

**Aakash Gupta** (00:02:04)

And what I wanted to know is how big is V0 now? Can you share in terms of users or revenue how much you've grown?

**Tom Occhino** (00:02:12)

Yeah, nearly two million people have used vZero since we launched last year. We're growing fast. It's sort of exponential here, and the uptake has been really, really exciting to watch. Of those people that have used vZero, many of them are deploying what they've built. We've had over two and a half million deployments to Vercel from vZero, so building things that are out there and in use.

**Aakash Gupta** (00:02:36)

Not just prototypes, which is, I think, the most common use case I've been talking a lot about, but actual apps. It's pretty amazing. So can we show people how vZero works and how you can build apps?

**Tom Occhino** (00:02:48)

Yeah, absolutely. And I'd love to show some of the stuff that I've built for myself that I use on a daily or weekly basis. Let me share a screen here. So where do you want to start? So...

**Aakash Gupta** (00:03:01)

I love LinkedIn, of course. It's how I built basically this solopreneur business. But what if I wanted a better version of LinkedIn's newsfeed?

**Tom Occhino** (00:03:11)

I see. A better version. Let's actually enhance the prompt here and see if we can create something that is a lot better. So the first thing I did is I just said, look, my prompt was silly, but maybe you can embellish it a little bit. And now we're going to let v0 cook. Let's see, it's coming up with a plan. It's got a project structure. I actually love looking at the thinking. So while it's actually like authoring all of the code, I'm like reading in, let me see the plan. We need some layout, navigation, a feed with different post types. OK, we're going to have post interaction components, user profile card and detail view. So the whole plan here, Great. I didn't have to put any of the plan together. And now it's cooking over here on the side. So we'll watch it write some code.

**Tom Occhino** (00:03:59)

It's actually created a whole app with multiple files.

**Aakash Gupta** (00:04:02)

Document for us.

**Tom Occhino** (00:04:04)

Yeah, basically put together a very lightweight PRD. And yeah, now we're authoring some code over here. It looks like we're building a nav bar. We've got our layout, our page. There's going to be a profile component. I'm excited to see what it looks like.

**Aakash Gupta** (00:04:18)

And we just let it go without a screenshot. Is that how you often prompt?

**Tom Occhino** (00:04:23)

Yeah, I think I do a mixture. If there's something that I'm inspired by that I want it to be something that looks like this, but with that change or with this tweak, I'll start with a screenshot. And I think we should look at an example of that. Actually, maybe we can. Let's do that in parallel here. While we're cooking on our LinkedIn in the first one, let's actually use a screenshot. So you had sent me a version of your logged in home page.

**Aakash Gupta** (00:04:50)

Yeah, so looking at Apollo.io, where I was last VP of product.

**Tom Occhino** (00:04:54)

Yeah, cool. So let's see. Do we want to make any changes or just create a clone of what's there? So I think

**Aakash Gupta** (00:04:59)

what we want to do is customize the homepage based on the product that people are using. And since Apollo, like all SaaS products has like 10 products that people are using, for instance, me, I'm not using it to send emails. I'm using it for meetings and booking meetings. So for me, it should customize and show the upcoming meetings that I have. But if somebody's sending a bunch of emails, it should show, hey, these are the emails you've sent and the performance of those emails.

**Tom Occhino** (00:05:31)

Let's try this prompt. So we'll take our screenshot that we've uploaded here. You can kind of see a little version of it. And we'll try to take it, just emphasize upcoming meetings for this specific user, and let's see what we get from a screenshot while we let it cook. Why don't we go back and see what's going on with LinkedIn over here? Okay, we're creating a pretty sophisticated application. There's going to be a feed. There's going to be suggested connections. Like, this is pretty amazing. And we did not really give it much direction, so I'm very excited to use this. It's amazing how

**Aakash Gupta** (00:06:09)

much effort it will go off and do. A human would never go out and do that much effort in one shot.

**Tom Occhino** (00:06:16)

Yeah, exactly. And I think there's a few different ways to do this. One is you can just get started and build and then iterate really quickly. And I like the iteration velocity of just tweak this, just add that. But if you want something that feels more full-featured, that feels like you could actually start from something you can actually use, and then you want to tweak from there, I think we can really let it cook here. And again, that prompt enhancement really turned this into a proper PRD with a lot of features. It also obviously knows a little bit about the LinkedIn product offering. So it's building out mock data now so we can actually fill in the news feed, which is awesome. Over here, we already have our version of the Apollo homepage that puts, let's see, scheduling meetings first. We've got a view all meetings

<!-- sponsor -->
**Narrator** (00:07:02)

view. Let's see, some email stats and meeting activity.

**Aakash Gupta** (00:07:07)

So it pretty much followed it exactly. And it took a little bit of the Apollo styling element. So if we wanted to ask it even further, like replicate the Apollo nav.

<!-- sponsor -->
**Narrator** (00:07:18)

Yeah, let's do it.

**Aakash Gupta** (00:07:22)

Po.io navigation as well. And then my traditional approach has been to do these feature enhancements one step at a time. If we had another feature enhancement, like I want us to, once we click into that, be able to look at whether people have paid us or something for the meeting. Would you recommend doing that separately, like I typically do, or doing it at once?

**Tom Occhino** (00:07:45)

Yeah, I'll usually, just because I like the changes to be atomic, I'll say, like, let's do this and then let's do that. And then I can roll back individual changes, et cetera. But it's very good at taking, like, five different things and breaking it out and saying, OK, here's the five things I need to do and doing them all at once. So it depends on if you want those incremental states or not. But yeah, personally, I will do one thing at a time. And it feels more like a pull request to me. Okay, my next pull request is going to be adding the calendar widget. Then my pull request is going to be look at this component. Got it.

**Aakash Gupta** (00:08:21)

So when you use some of your competition, you're like choosing like a specific model that you might use like in Windsurf. You'll say, okay, I want to use Claude Sonnet 3.7 or 3.5. For you guys under the hood, you guys are using, I'm guessing, like multiple different models for different use cases.

**Tom Occhino** (00:08:38)

Yeah, that's right. One of the things we don't want to do is expose all of the underlying sophistication. We really want to pave a happy path. So our model, we call it an online model because not only is it using the underlying LLMs, but it's then doing a bunch of work on top. Something like 85% of the code that the LLMs give back to you won't run by default yet. And they're getting better and better. So we then iterate on the code that comes back and tweak it and fix it up based on everything that we know. And we do that on top of a bunch of different models. Okay, let's see. We've got a new nav bar here. This is great.

**Aakash Gupta** (00:09:20)

It looks exactly

**Tom Occhino** (00:09:21)

like

**Aakash Gupta** (00:09:21)

our screenshot, so it's really good at copying design. I think that's why it's so useful in this prototyping use case we have here because let's say I was the VP of product and I had asked the PM about this feature, they can come back with a prototype literally five minutes later.

**Tom Occhino** (00:09:36)

That's exactly right. And this use case is really, really powerful because even if you're not an engineer, even if you're non-technical, you can demonstrate the idea that you have in your head with extremely high fidelity and very, very little

<!-- sponsor -->
**Aakash Gupta** (00:09:48)

time. This episode is brought to you by WorkOS. If you're building a SaaS app, at some point your customers will start asking for enterprise features like SAML authentication and SCIM provisioning. That's where WorkOS comes in, making it fast and painless to add enterprise features to your app. Their APIs are easy to understand so that you can ship quickly and get back to building other features. Today, hundreds of companies are already powered by WorkOS, including ones you probably know like Vercel, Webflow, and Loom. WorkOS also recently acquired Warrant, the fine-grained authorization service. Wern's product is based on a groundbreaking authorization system called Zanzibar, which was originally designed for Google to power Google Docs and YouTube. This enables fast authorization checks at enormous scale while maintaining a flexible model that can be adapted to even the most complex use cases. If you're currently looking to build role-based access control or other enterprise features like single sign-on SCIM or user management, you should consider WorkOS.

<!-- sponsor -->
**Aakash Gupta** (00:10:51)

It's a drop-in replacement for Auth0 and supports up to 1 million monthly active users for free. Check it out at workos.com slash Akash to learn more. That's workos.com slash Akash. Today's episode is brought to you by Jira Product Discovery. We'll be right back. That's A-T-L-A-S-S-I-A-N.com slash product dash discovery. Jira Product Discovery. Build the right thing.

**Tom Occhino** (00:11:58)

I'm very interested in going back to see where we're at with our LinkedIn clone because this thing I feel like is probably a pretty full-featured app. We actually have images in here. That's fantastic. Trending topics. We've got a post composer. Okay, this actually seems to work pretty good. Okay, let's see what else we have. I almost, okay, there was one. I could choose to fix this route with v0. It's like, oh, I haven't implemented that one, so I can ask it to fix it. But I'm interested in exploring what we do have. It implemented, we have notifications. We can click through those. Let's see. This is like a pretty sophisticated application. I'm going to ask V0 to fix that runtime error next, and we'll just see what that flow looks like. So that was me going to the profile me route. And I'm going to say, OK, let's try to fix this one while it cooks.

**Tom Occhino** (00:12:50)

It says the code returns the following error page not found for profile me. It's like, oh, let me look and see what's happening. I don't have that route. Let me implement it for you. So this iterative, you know, I'm exploring the thing that we're building and then kind of building it interactively I think is a pretty fun way to do it.

**Aakash Gupta** (00:13:08)

Yeah, and how does v0 work with databases?

**Tom Occhino** (00:13:13)

Yeah, one of the things I'm very excited we added were these integrations. So right now we have a number of integrations from the Vercel marketplace that work sort of out of the box with zero need to go off and create accounts and all this other stuff. The integration is really seamless. It's a couple of clicks. So if I wanted to back this with a proper database and then fill the database with mock data, I could connect, you know, Neon. I could create a store. I could also connect not just databases, but other AI providers. So if I want to add features from, you know, AI features to my generation, I can connect those seamlessly as well. So very excited, especially about, you know, Grok by XAI coming in here and offering like a a very generous offering to get started and really explore what AI looks like to add and what these marketplace integrations look like to add.

**Aakash Gupta** (00:14:04)

That would be fun to do. So could we try to add like a Grok powered post composer? What would that look like?

**Tom Occhino** (00:14:11)

Let's try to do it. Let's, let's add a, we're going to do it live. Let's add, we'll create a new store. I'm going to try on the free tier to start. We'll continue. Start with that, install it. Our product was created successfully, so we're done. We're back in our application. And now, let's see, it's thinking on maybe our previous request as well. Here we go. I see you've added the Grok integration to your product. What would you like to build within your Newsfeed application? Let's add an

<!-- sponsor -->
**Narrator** (00:14:50)

AI-powered post composer in the start post flow. Let's see where it goes.

**Aakash Gupta** (00:15:02)

Hopefully some LinkedIn PM tries this.

**Tom Occhino** (00:15:05)

Yeah. I mean, this is, you know, I really do like the, somebody else has designed something that works really well, and I can start with that as my starting point. And you don't have that blank canvas thing. I'll never have that again. But yeah, LinkedIn has a model that works pretty well. We can start with that. You can also add storage or AI to our other generation over here. While that's cooking, I could also walk through some of my own generations. I don't know if that's interesting for folks.

**Aakash Gupta** (00:15:34)

Yeah, as a CPO, what do you get time to generate? What is useful? What have you been generating in v0?

**Tom Occhino** (00:15:40)

So one of the things, yeah, this is like my favorite thing. I don't really have time to sit down for hours on end and code anymore, but I still have ideas and I still have little personal software that I want to exist. One that I created somewhat recently is I just want to go back and look at all of our blog posts and changelogs and just filter them by, like, you know, various things, various topics. So, like, I wanted to look for all the observability changelogs. And so, great. I, like, built this thing that consumes an Atom feed. It was, like, a handful of prompts, and now I use this in order to pull together the, like, summary from a different product area. I can filter by, like, start dates. It built all of this... UI for me, and here's the two observability-related changelogs we've had in April.

**Tom Occhino** (00:16:24)

So this is a tool. I actually use it. I love it. I was on a call with an e-commerce prospect recently, and they were like, how could V0 help change the way that we build things? And I did this. This was ridiculous to me. It one-shotted a sneaker store. This is literally the full prompt, right? And I did enhance prompt again. But this is only one prompt. I haven't touched anything. And the biggest thing that I wanted to demonstrate was real-time filtering. Because I feel like most e-commerce stores have filters that, like, you have to wait for a page refresh. It's really clunky. And this does real-time filtering based on price, brand, attributes. And they were like, oh, my gosh, I could plug this directly into my back end and just use this with all of the media coming from the back end. And I'm still kind of in shock that this was a one-shot.

**Aakash Gupta** (00:17:12)

And what's the workflow that somebody will typically use for that? They'll export this code into Windsurf or cursor their IDE of choice, or how do they typically go from here?

**Tom Occhino** (00:17:23)

Yeah, you certainly can. I mean, we can connect to databases from right in the web browser. I love the web browser as a creation, not just consumption vehicle. But yeah, you can take this code base and you can export it into any editor, and then you can start to enhance it. We're working on making it seamless to flow back and forth between the editor and the creation experience in v0. So you can kind of like, you know, every change is an atomic sort of pull request or a git commit. And then you can actually bring that repository into your editor and bring it back into v0. It varies. Everybody's workflow is a little different, but we're pretty flexible about it. Very cool. What else have you built? One of the other things, I'm very excited to try our Grok integration over here. But one of the other things that I'm just really excited about is my wife used to ask me for this, I just want to know what neighborhood I'm in.

**Tom Occhino** (00:18:13)

We lived in New York City, and we would go out to dinner in certain neighborhoods. And she was like, I wish I could just see what neighborhood I'm in. We could kind of try to use Google Maps for this. There's some services. But I was like, I just want one button. So I actually turned this into a thing that I deployed, and I use this every week. I use this to figure out what location, whatever. It's just a super simple thing. But my wife loves it because it was software that was designed exactly to her specification, and I just have it pinned to my home screen on my phone, and we use it whenever we go somewhere. It's like, oh, this is a nice neighborhood. So this was a fun one I made for me.

<!-- sponsor -->
**Aakash Gupta** (00:18:50)

That's a really interesting future after... apps like v0 have hit the market right, which is that anybody can make personalized software. I love this. So it sounds like people can go to where.tomochino.com to try it themselves.

**Tom Occhino** (00:19:05)

Yeah, they can try it themselves. Absolutely. Give it a shot. The era of personal software is absolutely upon us. And this has been the most exciting thing for me. I used to have this list of all the things I wanted to build and no time to actually build them. And now I can build them again. Let's see what we did over here on our LinkedIn news feed with the Grok integration. User clicks start a post and clicks on the AI Assist button. OK, what would you like to write a post about? I actually do like this prompt. Share thoughts on recent tech trends

<!-- sponsor -->
**Narrator** (00:19:42)

in a

**Tom Occhino** (00:19:43)

LinkedIn style.

<!-- sponsor -->
**Narrator** (00:19:44)

I'm

**Tom Occhino** (00:19:47)

keen to see how it does. OK, let's see. Invalid API key. OK, this is great. Let's see if we can fix it with V0. My favorite thing is fix with v0, because usually what are you going to do? You're going to go search for how to fix something, and it's like, oh, we can just ask them. I'll fix the API key issue. The problem is we're accessing. Let's see. A discerning voice can probably find it. In project settings, we usually have API keys and things that we may

<!-- sponsor -->
**Narrator** (00:20:17)

need to pull. So I'll copy in case we need to put it in.

<!-- sponsor -->
**Narrator** (00:20:25)

And it's off chugging. AI

<!-- sponsor -->
**Narrator** (00:20:28)

module does not provide export name. We'll fix that one as well.

<!-- sponsor -->
**Narrator** (00:20:32)

Runtime error, OK.

<!-- sponsor -->
**Narrator** (00:20:37)

Yeah, the other, let's see, all my project settings. Yeah, I see no environment variables. Let's do that X API key. And I'm going to just burn this API key right after.

**Aakash Gupta** (00:20:57)

Don't forget that step.

**Tom Occhino** (00:20:59)

Right. Yeah, there we go. OK, this is trying to load an image that doesn't actually exist.

<!-- sponsor -->
**Narrator** (00:21:08)

I'd love to go back to here. There we go. Let's go back to this one and load this block.

**Aakash Gupta** (00:21:24)

Restore. Okay, so you're

**Tom Occhino** (00:21:26)

going to return

**Aakash Gupta** (00:21:27)

back to an earlier version? Yeah,

**Tom Occhino** (00:21:29)

I'm going to restore the previous version right after we added the integration because now I've also added in the API key. Okay. I may have gone back one click too far. Let's restore after. I

**Aakash Gupta** (00:21:42)

feel like that's one of the big tricks here of using this is these restore buttons, just scrolling back up a little bit.

**Tom Occhino** (00:21:47)

Yeah, I'm looking in my, like, different versions. This is the one that we restored. So we have our AI assist, and let's see if we've added our... Okay, the API key was reverted as well, so I have to get our API key going. But, you know, we'll fix some errors here, and we'll get it working. Over here... Let's see, I was wondering if we wanted to add any database or any integrations to this, but we can also continue the conversation.

**Aakash Gupta** (00:22:23)

I would be interested to see both database and deploying, what those look like.

**Tom Occhino** (00:22:27)

Yeah, we should deploy one of these. So let's add one of our database integrations here. I'm not sure what we want to store in the database, but we can fill it up with some data. I'm going to create a new Neon store. Maybe

**Aakash Gupta** (00:22:42)

just the meetings that we have coming.

**Tom Occhino** (00:22:45)

Yeah, let's do a toy here. We'll add a database for upcoming meetings, and we'll try to integrate the data from the database. So Neon gave us a database created successfully. It's thinking about the integration we just added. All right, let's see.

<!-- sponsor -->
**Narrator** (00:23:06)

Let's store upcoming meetings in the database. Please fill with mock content for the next month.

**Tom Occhino** (00:23:19)

And then we'll have to, we'll hopefully replace these upcoming meetings with Something from the database. So we're really like vibe coding here. I haven't actually looked at any of the code that's been generated. We're just kind of dictating what should be done. As an engineer myself, I like to actually go back and forth. I'll go and actually make changes to the code and say, no, not like that, just like this. And that's still fun. But if you don't have any coding experience, this is both a good way to still build amazing things and to learn how to code.

**Aakash Gupta** (00:23:49)

Yeah, I think so. Or just somebody like myself who hasn't been coding a lot in the last three or four years. It's a good way to get back into it.

**Tom Occhino** (00:23:59)

Exactly. I mean, this was my thing. I've been in management and leadership for a very long time. I haven't been sending pull requests. I can't support the code that I author, right? So this is a good way for me to be able to build again. Looks like we've created a meetings table. Yeah,

**Aakash Gupta** (00:24:17)

the one worry

**Tom Occhino** (00:24:17)

one of my

**Aakash Gupta** (00:24:18)

podcast guests had, he's a VP of product here. He was like, we're kind of entering the golden age of the feature factory because we've allowed all the C-suite to create these prototypes for us.

**Tom Occhino** (00:24:30)

It's true. And the C-suite does have a lot of feature requests. You know, you talk to one customer and you want to make their dreams come true. You're like, yes, absolutely. This is incremental. We'll add that. And now we sort of can. So we have to be discerning. You have to have strong opinions about what belongs in and out. We also can't let the XY problem thing happen. Customers ask for one thing, even though they really want something different, maybe more foundational. So we still have those strategic conversations and make sure we're not just YOLO shipping net new features all the time. Okay, let's see. We're going to populate the meetings table with some mock data now. Sorry, I could have been applying that while we were chatting. I think

**Aakash Gupta** (00:25:09)

that it's actually emphasizing the PM skill set though. Absolutely. Because

<!-- sponsor -->
**Narrator** (00:25:13)

now

**Aakash Gupta** (00:25:13)

everyone is getting into, hey, what are the things that actually are going to move the business outcomes that we want? What are just one-off customer requests versus actual problems lots of our customers face and figuring out that prioritization of what to put in?

**Tom Occhino** (00:25:25)

That's right. In a world where you can decrease the cost or time taken to build something, certainly you could try more things, but you really want to be strategic and thoughtful about what direction you go in, because it's very easy to go in the wrong direction now. It's very tempting to just like, oh, we'll just try a bunch of things. I think that strategic thinking, problem solving, Depth of ownership is really, really important. I mean, the biggest job that, the most important job that PMs play is the sort of deep owner of a product. And you still need that. You can't have other people YOLOing new features into your product. It has to be cohesive. It has to feel like, you know, you're taken on a journey and that it's solving real problems for you. So the PM skill set is as relevant as ever. 100%.

**Tom Occhino** (00:26:13)

Let's see, we've created our database. We're updating our application to fetch and display these meetings from the database.

<!-- sponsor -->
**Narrator** (00:26:19)

Okay.

**Tom Occhino** (00:26:21)

Great. All right, we're missing our environment variable, so we'll have to get that auto-configured in the future. Neon database URL. I'm gonna go look at my URL. I'd like to stop sharing screen so I can

<!-- sponsor -->
**Narrator** (00:26:41)

move this over here. I can copy my database URL and we'll paste it in. Great.

**Aakash Gupta** (00:26:57)

All right. We had to add the environment variable here.

<!-- sponsor -->
**Narrator** (00:27:00)

Exactly. Now that we've got the environment variable,

**Tom Occhino** (00:27:07)

We're set up and recreate. Yeah, one of the things we're also working on is making incremental regenerations much faster, so you can only update the part of the application that you need. OK,

<!-- sponsor -->
**Narrator** (00:27:22)

very cool.

**Aakash Gupta** (00:27:25)

What is the overall team you guys have staffed behind vZero right now?

**Tom Occhino** (00:27:30)

Team is pretty small. We're split into three pillars on vZero. One is the research and language model. We have this dev one model that we use. We call it an online model. We're constantly iterating on that. We're also working on all of the fundamentals of the chat experience. This core experience that we've been using, And then the third pillar is around the periphery. So all of the administration and the, you know, billing and account settings and project settings. Team is pretty small. I would say there's less than 14 people working on V0 all up across engineering product and design.

**Aakash Gupta** (00:28:12)

Wow, super lean.

**Tom Occhino** (00:28:13)

Super lean, yeah. And really tight knit too. It's been really fun to watch the team cook.

**Aakash Gupta** (00:28:19)

That's awesome.

**Tom Occhino** (00:28:20)

How big is Vercel overall in terms of product design and engineering? Ooh, engineering, product, and design all up, probably right around 200. One of the benefits of vZero and many of the other teams is that they get to build on top of the foundations we've created for Vercel. So we didn't have to create a net new accounts system and a net new marketplace of integrations. Those things have existed, and then kind of bringing them together is much easier than building those things from scratch. The biggest one, obviously, is our deployment infrastructure. So at some point, we're going to deploy one of these things we've created. I can deploy something else that exists here. I don't think I ever deployed this sneaker store. But you can see that when I deploy this thing, Now you've got a decade's worth of managed infrastructure just wearing into action and creating a deployment.

**Tom Occhino** (00:29:17)

And pretty soon, I'll have this open to the entire internet. And then I can go further and customize my domain. I can add people to the project because this project will be backed by a Vercel project. So all of the everything you can do with a Vercel project, adding team members and customizing everything about it, backs every one of these deployments.

<!-- sponsor -->
**Aakash Gupta** (00:29:39)

AI evals are one of the most important skills for PMs. And I know you know they matter. The question is, are you doing them right? Most teams are winging it with basic metrics and hoping for the best. Meanwhile, the teams that actually ship reliable AI, they've cracked the code on systematic evaluation. Today's episode is brought to you by the AI evals for engineers and PMs course by Hamil Hussain and Shreya Shankar. This live Maven course will teach you the battle-tested frameworks from Hamil and Shreya, who are the engineers behind GitHub Copilot's evaluation system and 25-plus production AI implementations. Four weeks, live instruction, next cohort starts July 21st. Start shipping AI that actually works. Enroll at maven.com with my code ag-product-growth for over $800 off. That's ag-p-r-o-d-u-c-t-g-r-o-w-t-h. Today's episode is brought to you by the AIPM certification on Maven. Run by Mikdad Jaffer, who is a product leader at OpenAI, this is not your typical course.

<!-- sponsor -->
**Aakash Gupta** (00:30:48)

It's eight weeks of live, cohort-based learning with a leader at one of the top companies in tech. OpenAI just doesn't stop shipping, and this is your chance to learn how. Run along with product faculty and Mo Ali, the course has a 4.9 rating with 133 reviews. Former students come from companies like OpenAI, Shopify, Stripe, Google, and Meta. The best part? Your company can probably cover the cost. So if you want to get $500 off, use my code AAKASH25 and head to maven.com slash product dash faculty. That's M-A-V-E-N dot com slash P-R-O-D-U-C-T dash F-A-C-U-L-T-Y. And for people who don't know, Vercel, as you can hear with the numbers, 186 people focused on this core business because you guys started that, what, almost 10 years ago, and VZero is really one of the newer things that you guys have built.

**Tom Occhino** (00:31:40)

Yeah, that's right. And, you know, it's really nice for us to be able to bootstrap things internally. VZero sort of operates like a startup within a startup, but it gets to build on top of the foundations that were laid by everything else we built. So, yeah, this is... very related to how we build products is we want to lay the foundation, lay out a North Star for where we want to go and then use the foundation to build the incremental path to getting there.

**Aakash Gupta** (00:32:06)

And is this a totally different user for you guys? It sounds like it might be like a different user and buyer. How do you guys kind of think about managing the difference?

**Tom Occhino** (00:32:16)

Yeah. Is it okay if I stop sharing my screen? Yep. Yeah. It kind of is. Yeah. So I think Developers for forever. We are the developer company. We love building tools for developers. We are ourselves developers. But the definition of developer is getting a little bit wider. It went from anybody who could build things using traditional software engineering techniques to anybody who wants to build things. And that's been really fun to watch, especially internally. The evolution that vZero has provided is anybody who's sort of tech adjacent, anybody who knows this thing exists can build things. So we do a demo day every Friday. We do demo days. And demo days started out a couple years ago. Engineers would show up and demo stuff. Then designers came in. And designers would say, OK, we've got some mocks. We're thinking about some things. We're just demoing what we're thinking.

**Tom Occhino** (00:33:09)

Product managers would come in and demo end-to-end flows of certain things, not just features. But what's happened more recently is other parts of the business are coming in and demoing full-fledged applications. Here's my proposal for how we should build the new domains management experience. One of my favorites was an account executive came in and said, hey, usually I jump on a call with a prospect and we go through total cost of ownership of buying Vercel. And usually I will send them a spreadsheet. And the spreadsheet, you know, it's lots of rows and columns and numbers and tabs. This time I dumped all of that data into vZero and I created an interactive application for them to filter and look at their own growth of their company based on their success over time. I would never have been able to take the time to do this because I'm talking to so many prospects.

**Tom Occhino** (00:33:58)

But because I was able to build this one-time use software, The customer was so elated. They're like, I can see it. I can understand how this is going to pay dividends for us. So having account executives show up to demo days demoing products is amazing.

**Aakash Gupta** (00:34:14)

That's crazy. There's so much that's possible with this. But you're in a very competitive space. If I look at it, we had a Bolt CEO on the podcast. There's Replit. There's Lovable. We've

**Tom Occhino** (00:34:25)

done

**Aakash Gupta** (00:34:25)

some windsurf and cursor demos as well. How do you think about competing in this space?

**Tom Occhino** (00:34:31)

You know, I helped build React, and people used to ask the same question about React. How do you think about React's competition? And I gave the team the same direction always. I really don't think about the competition. I think about our customers and delivering as much value as I can. And I also think about my own use case. Like, I actually am building something that I am excited to use. So look, it's tempting. Some competitor adds this feature or that, and you're like, we've got to catch up. I don't want to play catch up. I just want to build things that continue to add value for ourselves. Seeing that account executive, that product manager, our head of internal communications builds things now. Her feature requests that enable her to do her job better matter more to me than whatever feature some competitors coming up with. So it's good to keep your finger on the pulse.

**Tom Occhino** (00:35:20)

You want to make sure you're not missing a wave. Our CEO, Guillermo, makes sure that we stay at the tip of the spear of all the latest trends, I promise. But I direct the team to really stay focused on delivering as much value as possible to ourselves as customers and to our customers of tools like vZero.

**Aakash Gupta** (00:35:39)

You mentioned React. You're really well known for that. If anybody searches you up, they'll find tons of things with you in React. What's interesting to me is that most of these apps, and VZero included, they tend to use React when they're building. It seems like, what does that make you feel?

**Tom Occhino** (00:35:55)

Yeah, it's humbling for sure. I think when we started creating React, one of the things we loved was that it felt like it was lowering the barrier to entry for development. And because it did that, you saw a lot more people building with React than were using other sort of libraries and frameworks at the time. And it picked up in popularity, I think, honestly, because it was more fun. But because it picked up in popularity, there's so many examples of open source React applications out there. And I think the models have ended up being trained on lots and lots of React code. You can certainly teach them to use other frameworks. And I think like even v0, you can say, hey, build this in SvelteKit. And it does a great job. But by default, it's like, well, I know the most about React because it's kind of ubiquitous at this point.

**Tom Occhino** (00:36:42)

So that was very surprising and humbling for us. But what I love about this next generation of tools is in the same way that React lowered the barrier to software development, these tools like v0 are lowering the barrier even further or dramatically further. And the framework is becoming more than ever before, somewhat of an implementation detail, if that makes sense. Frameworks were a construct that we made to enable the sharing of code and the ability for many people, humans, to iterate on the same code base using conventions and APIs. And now, if I'm more and more able to sort of build all of this stuff myself and iterate quickly without... fully understanding all of the complexity of the front-end code, or at least not understanding it first, then the framework becomes something that can be progressively disclosed over time. So yeah, anyway, back to your question.

**Tom Occhino** (00:37:40)

I think it's been really humbling to see how React has become the sort of substrate layer underneath all of this.

**Aakash Gupta** (00:37:50)

Yeah, almost every time I'm really looking behind the code of these apps that these prototyping tools are building and they're using React. Speaking of which, can we close the loop now? Because people really want to deploy apps and see the databases, can we look back at our apps and close the loop on that step? Oh, yeah, let's look. Let

<!-- sponsor -->
**Narrator** (00:38:08)

me get back into here and sharing my screen. Here we go.

**Tom Occhino** (00:38:19)

There we go. I think we've got it. Yeah, here you go. It looks like we've added a bunch of meetings that are in our database.

<!-- sponsor -->
**Narrator** (00:38:28)

Nice.

**Tom Occhino** (00:38:29)

We've added a meeting creation form. Oh, we've added a meeting creation form. Let me full screen this and we'll check it out. Of course we have. So let's do a quarterly review. This is a new meeting. We'll do it April 23rd from 9 to 10 a.m. It's going to be in person this time. Create meeting. Zoom link or meeting room. I'm in a room called Midnight, so let's do it in here. Then I'm going to add my personal email address and see if it emails me. I should not have disclosed that. Success. My meeting was created successfully. Let's see where it showed up. Meeting scheduled 15. Okay, we would have to implement the all meetings flow. I kind of want to deploy this one actually and just play with it for a while. Yeah, view all meetings hasn't been implemented yet, but I assume that's where that would show up.

**Tom Occhino** (00:39:34)

I'm tempted to go into the database as well. We also deployed our sneaker store here, so let's see. Okay, yeah, this just is live on the Internet at v0sneakerstore8.versell.app, so anyone can go play with that one. So we haven't left people hanging.

**Aakash Gupta** (00:39:51)

You can connect it to database. You can make it a live app. That ends it for our live cooking session. We showed you guys how you can build multiple apps. You can use it one-shot new design. You can use the prompt enhancement. And I think one of the key lessons here is that there is no particular right way. The way you've built the chat, it can handle a lot of different things. And I think that's part of the magic here is it's like ChatGPT in that way. You can give it a misworded response. You can have a typo in your prompt and it'll still work with it.

**Tom Occhino** (00:40:26)

Yeah, that's right. That sort of flexibility. And the fact that it kind of speaks to you in plain English, it's like, oh, here's the thing that was missing. Remember, I had to copy in my environment variable. Eventually, maybe we'll make even that step go away. But it kind of guides you, and you can ask it plain English how to fix certain things for you. But then, at the end of this, you can deploy real software to the internet. And that's what we did.

**Aakash Gupta** (00:40:51)

Somebody's watching this. Maybe they're not as technical as you and I. They weren't an engineer before. What else do they need to know if they want to take, let's say, that e-commerce store right there and make it into a million dollar app?

**Tom Occhino** (00:41:03)

Make it into a million-dollar app. One of the things I like that you mentioned earlier is the PM skill set is as relevant as ever. You've got to build something that people are excited about, and you can take that thing and you can iterate on it until it's something that you're excited about, and then you can share it with somebody else and get them excited about it. But all the rest of the work of creating something valuable still exists. This isn't a sort of like, oh, I've... I've just YOLO'd something out into the internet, so now I'm going to get a million users. I think actually what's going to happen as the time to development and iteration velocity goes up, time to development goes down, I think actually the products that deliver real value are going to be the ones that don't really play games. They're like, okay, this actually helped me do something now that I couldn't do before.

**Tom Occhino** (00:41:53)

So the PM skill set is as relevant as ever. And actually finding ways to deliver real value to real people is the only way to get adoption. So you'll, you'll do marketing, you'll do, you'll go talk to people, you do user research, you'll iterate on your product based on feedback. And the way that you iterate is a little different, but the rest of the job has to be done.

**Aakash Gupta** (00:42:13)

And what should people know about scaling and iterating? Should they stay within V0? Can it handle all of the scaling that might be needed to scale to that level, handling thousands or tens of thousands of users? Or should they eventually move into kind of like a IDE or something like that to handle a larger and growing code base?

**Tom Occhino** (00:42:33)

Yeah, I think it really depends. If you're starting out as a developer, you'll probably want to sort of eject into your editor, connect things, make changes, and iterate from there, collaborate with your team, back it by a Git repository, et cetera. If you're starting out as not a developer, you're just learning development, you maybe want to stay in the browser in v0 for as long as you can. But either way, what you deploy is real software. When you deploy from Vercel, from v0 into Vercel's managed infrastructure, This will scale to a billion users. And so it really is about attracting your users and building something that, you know, gets real traction. It's not necessarily about the tools themselves holding you back. The thing that I love about a vZero project is that, again, it's backed by a real Vercel project, which has, you know... OpenAI.com and all of these other Chick-fil-A's operations and UnderArmor.com, these are real products with real scale.

**Tom Occhino** (00:43:36)

And so they're all backed by Vercel's infrastructure the same way that the thing that you just vibe-coded would be backed by Vercel's infrastructure.

**Aakash Gupta** (00:43:44)

Awesome. So I want to peel back the curtain since you are the Chief Product Officer. It's rare to get an opportunity to talk to Unicorn's CPO, pick their brain, understand how they're running their product team. So what is unique about how Vercel builds product?

**Tom Occhino** (00:43:59)

Yeah, so by way of clarification, I think CPO entitled, but I run engineering product and design. So we can talk about engineering as well. And as a former engineer myself, I think that's kind of where that comes from. My counterpart is our CTO, Malta Ubel. He's an individual contributor and gets to go deep on everything. And so we partner really, really well. He goes deep on the tech, and then I help manage the org. Yeah, the way that we build products, where do you want to start?

**Aakash Gupta** (00:44:28)

Well, I guess planning is the most interesting thing. How are the V0 teams, for instance, planning? These are the big rock features we want to do. Are they doing it on a quarterly time frame? What fidelity? Are they building a V0 prototype to show it?

**Tom Occhino** (00:44:44)

Yeah. We do, first of all, organization. We organize ourselves into product areas. And we have somewhere between 12 and 15 product areas. Each of those product areas contains a number of products. Each of those products contains features, as you'd expect. And each of those product areas has a leads team. So there'll be the leads for the domains product area, and there'll be the leads for the compute product area. And what we expect of the leads, which are cross-functional, so engineering, product, and design in the leads for each of these product areas, is we expect that they are owning their roadmap and checking in very, very frequently. We do a more formalized planning process every six months or so just to kind of reset and figure out if everything that we're working on is still relevant, if there's anything that new we want to make sure we're missing a big boulder over here we want to go after, et cetera.

**Tom Occhino** (00:45:41)

But then we check in very frequently. So six months worth of plans. I mean, everything is moving so quickly. There's no way that you could plan for six months at a time. So we'll do reviews a few days a week. We do at least two times a week. We'll have these reviews where teams can come in and do a kickoff check in. OK, here's our hypothesis. Here's what we're going to build. They can do an execution check-in. So they can say, OK, we've now been building for a little while. Here's what we're seeing. We're going to continue. Or they can do a pre-ship check-in. So we're about to launch. Here's all the things we need to consider from a pricing and enablement and go-to-market perspective. So we do very regular check-ins with these product areas. We organize our Slack around these things. We organize our meetings and our, you know, hack weeks and things around product areas as well.

**Aakash Gupta** (00:46:33)

Got it. Is there anything unique or interesting about your planning operating system? Are you doing it, you know, in Notion with lots of impact sizing? Are you doing it with OKRs or is it just pretty normal planning process?

**Tom Occhino** (00:46:48)

Yeah. We do use notion pretty heavily for this. And then, you know, projects that are enumerated in notion and we size them and we map them back to customer requests, et cetera. Then, you know, once, once we get into execution, we'll actually go into linear, um, both great tools for this. Um, I think Notion gives us the ability to connect to the rest of the organization. So one thing I like is we'll have a PRD that actually comes from the field engineering team that then maps into an engineering initiative or a product initiative. And so we can kind of cross-reference lots of different types of materials that all ladder up to a singular initiative. We take pride in our sort of Slack ops, so making sure that the relationship between Notion and Slack and linear is all very cohesive. But that's mostly about execution. I think for planning, we produce planned summaries for every product area, and then I create like a, you know, if that's the L3, then I'll create the L2.

**Tom Occhino** (00:47:43)

Here's my overall summary. Then I'll create the L1 for the executive team, which is like, here's everything you need to know that's happening. Some version of that we'll share with customers. It'll be customer-facing, and we'll take it to our customer advisory board, and we'll talk to prospects about what's happening soon. But yeah, our planning process is pretty fluid. We don't have a formalized OKR process. We tried one out about a year and a half ago. I don't want to say there was organ rejection, but I just want to say it was overfit for what we needed. Vercel is what I describe as lowercase a, agile. We are moving quickly. We are jumping from initiative over here to the next thing that comes up over here pretty, pretty quickly. And so a formalized process felt like it was actually holding us back from being able to move a lot faster.

**Aakash Gupta** (00:48:37)

So now I want to know how the V0 team uses V0, because I think AI prototyping has blurred a lot of the lines, right? PMs are getting into early versions of design. Designers are maybe iterating in V0 sometimes, not all the time in Figma, before they go to Figma. And then maybe engineers are even using V0 to kick off their engineering. Is that how it works on your team, or how are you guys using V0?

**Tom Occhino** (00:49:04)

Yeah, I mean, as a company, we're using it many, many different ways. On the V0 team, the way they're using it is obviously they do a lot of just building personal software and they're just tinkering and they're dogfooding and they're using it and giving each other feedback and making it better and better. But the other way that they use it that's perhaps different than what we showed earlier is they'll design one small piece of the app using v0. It's like, oh, I need the project settings drawer. And so they'll say, here's all the context on this project that we're building in. And then they'll end up generating something that they then import into the actual V0 itself. So V0 is a massive application, as you can imagine. You can't one shot a full fidelity V0, but what you can one shot is like the settings page that you then iterate on.

**Tom Occhino** (00:49:52)

And so you iterate rather than iterating in code, you can iterate in V0. So that's another thing that the V0 team does. More generally speaking, how we use vZero as a company, I mean, we went into some examples, but everybody's using it for stuff that we wouldn't have even thought about. We build slide decks in vZero now because it's easier to, you know, dump all the content that you want from a doc and then, you know, here, generate a slide deck for this, and then you can actually walk through a real slide deck without even going into, you know, a slide editor. So we use it for absolutely everything internally.

**Aakash Gupta** (00:50:25)

Okay. And specifically on the role of prototyping, like how should a PM think about prototyping? Should the prototype be replacing their PRD? Should it be after they have the PRD and it's been okayed in planning, then they go into the prototype phase? When do you really think about using AI prototyping to use it at its fullest?

**Tom Occhino** (00:50:47)

Yeah, in my mind, the sooner you can demo and validate your hypothesis, the better. PRD still play a role. I actually think that you can't capture all of the nuance and all of the edge case and the strategy in the demo. But I do think these things, the PRD can get a little thinner now, and it can be more high level, more strategic, more opportunity sizing, more analysis. And then the demo is what really, you know, a picture is worth a thousand words. The mantra that we have is seeing is believing. So, you know, you used to be able to do this in a PRD. You could embed screenshots and different views and things like that. But I think the real software will expose the edge cases a bit more quickly and kind of, you know, make it more real for people. I think it's also just more...

**Tom Occhino** (00:51:37)

it's more enjoyable to watch somebody give a demo of a thing versus just talk through either a slide deck or a doc so it's a more engaging feedback session when you're kind of demoing something but yeah there's there's kind of room for for both and they i think they complement each other really well

**Aakash Gupta** (00:51:54)

A picture is a thousand words, a prototype is 10,000 words, right? Exactly. You actually get to interact with the picture. It's the level up and that's why I've been encouraging more and more PMs, more and more designers to get their hands on tools like this. What are the biggest V0 features you guys have shipped recently?

**Tom Occhino** (00:52:13)

Yeah, I think integrations is the big one. I mean, that's very new. We tried two separate integrations, an AI integration and a database. But we're also bringing the full power of the Vercel marketplace here. So eventually, we're going to have things like observability off. Anything that your application, a modern application, needs, you'll be able to procure it through the marketplace in two clicks. And I think that, you know, we take it for granted now how quickly I went through the flow of creating a net new account with the underlying provider, provisioning a resource, wiring up billing. In my cases, I chose free to get started, but like billing was also wired up SSO. So integrations is the biggest feature we've added to vZero, and I think it actually really unlocks real applications versus the prototypes of even just a few months ago.

**Aakash Gupta** (00:53:04)

So walk us through in depth the story of that integrations feature. How did you guys roadmap it? Did the V0 teams pitch it back to you? How did you guys prioritize which integrations you're gonna build? How did you use V0 within that process?

**Tom Occhino** (00:53:17)

Yeah, so again, integrations builds on top of the Vercel marketplace. So we could do what you just described for that, which was a much bigger initiative from the past year, 18 months. But in terms of v0, I think what they actually did was they started with the foundations that already existed. And then they did. They went right into prototyping the flow. So with v0, they said, here's what we think. Here's where we think the button should go. And when you click it, here's the behavior we think you want. A big piece of what we wanted to make work was the generative UI piece of pasting in the URL. So if you saw that, it's like, sure, you could have directed me to go into the code and paste the URL into the code, the database URL. But we really wanted to make that seamless and inline.

**Tom Occhino** (00:54:01)

So there's a structured input for copying in environment variables. And we'll make even those even more seamless. But we prototyped that flow within V0. So it was just very meta. Yeah. But yeah, the team kind of had a list of all of the strategic new features that were either a combination of requests or things that we knew we wanted. And then we sequenced, we like ranked those. We have limited resources, so we ranked those features. And then we actually did do an early demo day of like, here's what we think it should look like. We had a review where we talked about what we think this would unlock and how we want to position it. And yeah, actually for that one, there wasn't a PRD for integrations. It really was almost exclusively demos and loom videos and conversation.

**Aakash Gupta** (00:54:58)

So demos, Loom videos, and it sounds like a couple key review meetings is how you were able to create all of the canvas for collaboration. You didn't even need a PRD. It was one of those features where people understood the impact. They understood the strategy. And so you didn't have to write that, which I think is the perfect example of how product development should look in this modern day and age. So let's say you were talking to your colleague. Let's say they're a CPO. at a slower moving company. Because it sounds like for sale, you guys are embracing AI, right? You guys build these key AI

<!-- sponsor -->
**Narrator** (00:55:29)

products. Moving fast. Makes

**Aakash Gupta** (00:55:30)

sense. But a lot of companies, they're not embracing AI, right? I'd say 80, 90% of companies, they're not. They're just now getting their engineers on the cursor, maybe. Whether their PMs have a V0 license, suspect, right? Yeah. When you're talking to those CPO friends, what's your advice for them? How should they be thinking about the new way of product development enabled by AI?

**Tom Occhino** (00:55:53)

I mean, the first thing that I would tell them is that it's actually really fun. So this isn't a stressful transformation you need to dread. Just start tinkering. Just build something, and you'll start to see it yourself. But I will say that the more existential thing here is everybody's moving really fast. And if we believe that iteration velocity solves all known software problems, or maybe all known problems, you're kind of going to be left behind if you're not at least tinkering and getting started. I think the idea that companies, you know, AI right now is being bolted on as a feature for lots of companies. That's not how AI is going to work. AI is going to be part of the fabric of how every company operates and every product they sell. Right now there's literally an AI button. AI has an icon, right? The little sparkle stars, right?

**Tom Occhino** (00:56:52)

But eventually, AI is not going to have a button. It's not going to be a thing that you plan, okay, what's our AI roadmap? It's just going to be what's our roadmap, and AI is going to be infused into all of it. So if you're not using AI and seeing the ways in which that it's transforming your own workflow and your own experience, how will you be able to transform your customer's user experience? in a sort of like tasteful and balanced and modern way. So yeah, I mean, my advice is obviously start tinkering yesterday and incorporate, you know, in small doses. You don't have to go, you know, 180 degrees. We weren't using any AI. Now we're doing everything with AI, but I think we should take this shift pretty seriously.

**Aakash Gupta** (00:57:37)

Are there any steps they should be thinking about if they want to buy their PM Team V0 licenses? What are the common concerns that come up and how you address them?

**Tom Occhino** (00:57:47)

Yeah, this is interesting. So in the engineering space, it's quite saturated. We started selling V0 licenses to enterprises, and they're like, okay, yeah, but we're paying for this other tool. We have this, we have this. But it turns out that there's significantly less friction for PMs, designers, and what I would describe as like dev-adjacent folks. So, um, we can do this like very start, very small, you know, we just have a couple of seats. We're going to just get some of our folks online and we're going to try this out for a while. Um, I would say start there. I think it's, it's totally reasonable to want to try something out before you commit and go all in for like years, times, thousands of people. Um, but I also think you can develop some conviction about the way that you'll use it, even just from the free tier.

**Tom Occhino** (00:58:34)

So you, um, Um, before you bring it into your company, you just start using it yourself. And then you think about the ways in which to transform your workflow. If you need to justify buying it internally, I think anytime anybody does the V zero demo of here's how my job gets a little bit easier and here's how I become a little bit more efficient. Um, it's always a no brainer. I mean, the value for price is just outrageous. So, um, Yeah, I mean, how do you get started? I would just say develop your own conviction about the ways in which it'll transform your own workflow. What are the integrations you'll use? What days will it show up? In what meetings will a V0 generation show up that previously you'd present a doc, a slide deck, or something else? And then that has turned into quite a bit of traction, actually, for our enterprise customers especially.

**Aakash Gupta** (00:59:25)

Awesome. So we covered V0, how Vercel builds product, the future of product management with AI. I want to talk a little bit about you. So you're an engineer for your whole career. You joined Vercel as a VP of engineering. Now you've become chief product officer. What was that transition like?

**Tom Occhino** (00:59:45)

Yeah, engineer by trade. I transitioned into engineering management, and then I was an engineer for about a decade at Facebook. Engineering director more toward the tail end, leading quite large initiatives. And so when I joined Vercel, it was really about bringing some of the infrastructure and developer infrastructure that companies like Facebook and Google had, bringing that to the rest of the world, and we can go into why. So starting as an engineering leader just made perfect sense. We already had a VP of engineering. We decided we were going to split engineering in two. The hypothesis was like, it's very logical to have an infrastructure organization and then a product engineering organization Platform, some teams call it that. And in my mind, that was the role. I was just going to help with engineering leadership. And I was excited about it. And shortly after I joined, we collectively, as an extended leadership team, identified a bigger opportunity.

**Tom Occhino** (01:00:40)

The bigger opportunity was to get engineering product design and a handful of other functions operating as a single unit. And there was no single threaded owner for all of this. And so you'd kind of hear different things depending on which function you talked to. And at the same time, G had been pushing us to become more design led, seeing as believing was a principle. But design was downstream of the assembly line process of development. Engineers are cooking over here and then sprinkling a little design on it. And hopefully product managers are shepherding some of this work along. So we actually had a conversation about restructuring all of R&D, which is engineering, product, and design, under me to sort of carve out these pillars but ensure that they're all operating as a single cohesive unit and serving the rest of the organization better. I think it's very hard for the go-to-market organization to know who to talk to.

**Tom Occhino** (01:01:35)

Should I talk to the head of engineering, the head of product, or the head of design? They're all telling me slightly different things. They're saying we're working on the same stuff, but they're framing it in slightly different ways. So yeah, we transitioned me into the chief product officer role, leading all of EPD. And since then, I think some things have been going a bit smoother. But yeah, I'm an engineer by trade. I have been learning product development. and designed to a lesser extent on the job and obviously supported by an amazing team.

**Aakash Gupta** (01:02:06)

What's your advice to engineering leaders who want to make a similar shift to become PM leaders?

**Tom Occhino** (01:02:12)

You know, the first thing, the moment I saw the light, I was actually still an engineering manager. I wasn't even a director. I saw the opportunity for me as an engineering manager to take certain work off the plates of my engineers that I thought was critical but which they didn't enjoy as much as I did. And at the time it was user research, talking to customers, writing up the document that explained the strategy for what the engineering team was building while they were burning through ticket lists, you know, like their task lists. And I just called that engineering management because my team happened to be a team that was building developer tools and we didn't really have many product managers allocated to developer tools. So when I eventually came into like leading a product organization, I sort of created a cleaner split between the roles and responsibilities.

**Tom Occhino** (01:03:04)

But one thing remains, the product managers have to be part of the team. You have to have complete trust of the engineers and your sort of counterpart, engineering management, tech lead, designer, et cetera. And so I really try to foster a relationship between, we were talking about those product area leaders. I really try to foster a very collaborative relationship there where the Venn diagram of jobs I'm good at and jobs that need to be done for each of the folks has a heavy overlap. But I do think about product management as an extension of engineering, or in many ways, it is the engineering, and then the programming is an implementation detail of the engineering, if that makes sense.

**Aakash Gupta** (01:03:47)

I love that framing. It is the engineering, especially in the V0 world that we just demoed for you guys. So I think that's really important. What's the story of landing this job? A lot of people want to land a VP job at a unicorn, an AI unicorn like Vercel. How did you do it?

**Tom Occhino** (01:04:04)

Yeah, I think my history in this space certainly helped quite a bit. I initially was not looking to go back to work right away. My story was there's a bunch of great people here that some of them came from my org. There was a couple of people from my org that had moved on. But some of which I've just admired from afar. So when I was thinking about going back to work, it was like, okay, there's really only a very small number of companies that I would entertain. And then it became about how do I complement the existing set of skills that you already have? What are the things that I'm good at? and that I enjoy doing. Those are different buckets. But what are the things that I enjoy doing and I'm good at that would actually complement and round out the rest of, for example, Vercel's leadership team was what I was looking at.

**Tom Occhino** (01:04:55)

And I think G and I are sort of yin and yang. He is much more technical than me. He is a much better engineer than me. But I'm technical enough to sort of influence and keep up with all of the technology and conversations there. But the thing that I've spent 10 years, well, now more than that, but at the time had spent 10 years doing was engineering management and people management and leadership and performance management and... cross-functional partnership. So as he was an engineer by trade and an engineer as a CEO, I was sort of like a people leader. I had designed and built organizations that were designed and built to serve a purpose and to build something. And so we complemented each other in that way. So to anybody else looking to land one of these roles, find the ways in which you complement the existing leaders on the team and you augment and sort of enhance in various ways that they wouldn't be able to do on their own, potentially.

**Tom Occhino** (01:05:54)

I also think you have to work on something that's true to who you are. In many ways, React has been my life's work. I believe that Next.js and Vercel are an extension of the problem that I was trying to solve with React, which was I want to level up the quality of software on the internet. I want open platforms to win. I want the web to win. And Vercel was just so aligned with all of that. And even if you watched Guillermo speak in the early days of Vercel and Next.js, it was always about the web and always bet on React and all these things. So I found a company that was very aligned with the work that I had been doing for so long and the leadership team of which I felt like I complimented and added something. It was a rigorous interview process, but at the end of the day, I think it was a very good match.

**Aakash Gupta** (01:06:48)

And how did it get started? Did they reach out to you? Did you apply? Because I feel like at these high level roles, it's all kind of shrouded in secrecy, nobody knows.

**Tom Occhino** (01:06:56)

Yeah, for me, it actually was, I was sort of a referral from somebody who was already here. And he actually orchestrated the first conversation for me to have with the CEO. And I think that person had known of me, obviously, because of my work and my experience. So, I was actually a referral from somebody that I had used to work with, and that person identified, hey, we need more of this. This is the type of thing that we're missing, and so that's actually where the conversation started. The hook was actually, the CEO was perhaps testing me, but he challenged me on something that I believed in, and sort of It compelled me to write a very detailed explanation of my position on something. And he was like, OK, you should interview for this role. And so I was being interviewed before I was being interviewed, if that makes sense.

**Aakash Gupta** (01:07:54)

Oh, very cool. So the old thing of impressing your coworkers when you work at a place like Meta, they end up going to awesome places. They recommended you. And then when somebody reaches out like Guillermo, thoughtfully responding because he's kind of interviewing you before the interview started.

**Tom Occhino** (01:08:12)

Yeah. And I wasn't looking for a new role at that point either. That was kind of the hook that made me say like, okay, maybe I'll interview.

**Aakash Gupta** (01:08:19)

Very cool, very cool. So you were at Meta before this, that was your life's work. What was a day in the life like at Meta?

**Tom Occhino** (01:08:29)

I mean, it really depended. I started out as a new grad engineer building user-facing features. I helped build the what's on your mind box, me and a guy named Kyle, back when we switched from having just text posts to having photo uploads and video and other events and things you could create. I worked on search. A day in the life as an engineer was we worked with a product manager. We burned through our task list. Eventually we would identify a lot, you know, higher level opportunities and products that we wanted to build. When I got into engineering management, I was very fortunate to work on developer tools. So I sort of moved away from directly influencing the product probably in 2011, 12. and started working on tools that enabled other developers to build products and move faster with higher quality. We had a team called Product Infrastructure that was all about, you know, a day in the life there was all about identifying bottlenecks for engineers and then figuring out ways to move them out of the way and speed everything up.

**Tom Occhino** (01:09:34)

Eventually, as an engineering director, I was overseeing React and the family of technologies that cropped up around it. as well as a team called WebCore. But the thing that seeded all of that was I created a team called JavaScript Infrastructure and built that team. That turned into React and so much more. And then also I inherited something called WebCore, and we rebuilt Facebook.com on top of the technologies that I was building on the other side. So a day in the life, you know, started out writing a lot of code, then it was a lot of meetings, then it was a lot of Meetings with PRDs and strategy sessions, but always working on developer-facing tools. I think my biggest contribution was probably convincing the company to open source React. I think it was at a time when people weren't convinced that open source was a good idea in general.

**Tom Occhino** (01:10:27)

I was very passionate about open source because of where I came from. So a day in the life like that was a bunch of meetings where I'm convincing the company that open source makes sense, and here's why. But yeah.

**Aakash Gupta** (01:10:39)

Maybe a little bit of a seedling for Mark to open source everything they're doing in AI later.

**Tom Occhino** (01:10:47)

Absolutely. I mean, their open approach to Llama has been seeded from the success of open source projects like React. Open Compute was transformative back in the day, if anybody wants to go look up Open Compute. And also PyTorch. It wasn't clear that PyTorch was going to be the way that we train AI. At the time, it was a pretty saturated space, but open sourcing it and really investing in the community is what made PyTorch so successful. So I think they're carrying that forward with open sourcing the models. I would love to see them open source even more.

**Aakash Gupta** (01:11:19)

So I want to end a little bit on future casting because I think you're uniquely positioned to do this. You've spent so much time in engineering. You now lead product designing and engineering at one of the hottest AI companies. What do you see as the future of engineering design and PM? We talked a lot about how those Venn diagrams are getting closer and closer. What does the future look like in the world of AI?

**Tom Occhino** (01:11:41)

Yeah, one of the things I'd love to see is the rise of the design engineer, and I think we're going to see a rise of the sort of PM engineer as well. I think that these roles are going to overlap more and more as the tools become more sophisticated and complement our existing skill set. I was an okay programmer. I love coding, but

<!-- sponsor -->
**Narrator** (01:12:06)

I was never the best. I'm sure you were awesome. Good in your career.

**Tom Occhino** (01:12:10)

Thank you. The way that I used to augment my engineering is I would work with other engineers that were better engineers than me and augment their engineering. So I would do integration and testing and migrations. And I was very obsessed with UX. So I would spend a lot of time on the pixels and the details. And so I had other humans that complemented my skill set. And together, the whole was greater than the sum of its parts. I think that AI tools are going to provide every individual with that complement. If you're very good at engineering, you're probably going to want to keep programming, but now AI is going to help you with design. If you're very good at design, AI is going to help you with implementation. So I think we're going to see the fusing together of these roles, and a lot of folks are going to be in these...

**Tom Occhino** (01:12:56)

interesting hybrid roles where maybe you don't own the entirety of the product yourself end to end, but you really get to focus more of your time on the thing that you're good at and that you enjoy and less of your time on the, what I used to describe as the tax associated with your job. Like, oh, I have to go write a PRD or I have to go make a mock or I have to go do this. So I think that's gonna be the evolution of a lot of industries. AI is gonna augment us and be good at the things that we are not as good at or that we don't enjoy as much.

**Aakash Gupta** (01:13:32)

So we talked a lot about V0 and AI prototyping and how they impact these things. More generally, what are the other AI things you're using as a CPO in your day-to-day that help you?

**Tom Occhino** (01:13:43)

Yeah, some of the tools I've been super impressed with, super impressed with Granola AI. I think it's like a very transformative way to think about meetings. The prompt is this, like, I wish I could go back and talk to that person and ask them for more details on this. You can ask questions about a past meeting. It's just, it's super powerful. I use ChatGPT just like everybody else. I love it for, you know, small things and big. It's basically replaced my usage of Google now. And I find that I don't need internet searches as much. I really want the sort of, you know, I'm just thinking about this or what's the answer to that. So using ChatGPT a lot. I mean, those are the big ones. I also have fun generating images and media and stuff. So I'm like tinkering with the fun side of things as well.

**Tom Occhino** (01:14:32)

V0 is the tool I use the most just because I love just tinkering and building stuff.

**Aakash Gupta** (01:14:37)

As builders, I think it has unlimited possibilities. Thank you so much for highlighting them today and being on the podcast.

**Tom Occhino** (01:14:45)

Thank you so much for having me. Great chatting with you.

**Aakash Gupta** (01:14:47)

Bye everyone. I really hope you guys enjoyed that episode. It would mean a ton to me and the team if you could please subscribe on YouTube, follow on Apple and Spotify podcasts and leave a rating and review. Those ratings and reviews really help grow the show and help other people discover the show and they help fund the production so that we can do bigger and better productions. Can't wait to share the next episode with you. Until then, see you later.
