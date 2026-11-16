---
title: "Best AI Prototyping Tools in 2026: Lovable vs Bolt vs Replit vs v0"
subtitle: "This isn’t just another talk about AI prototyping. We’re building an app with features, live, right in this podcast. Yes, LIVE. Using all 5 of the major tools. "
date: "2025-02-28"
host: "Aakash Gupta"
guests: ["Colin Matthews"]
speaker_names: "inferred"
substack_url: "https://www.news.aakashg.com/p/ai-prototyping-for-pms"
youtube_url: "https://www.youtube.com/watch?v=Gp6tMkCr_0w"
duration: "01:18:14"
word_count: 14593
source: "Substack episode transcript (aired audio)"
---

# Best AI Prototyping Tools in 2026: Lovable vs Bolt vs Replit vs v0

*This isn’t just another talk about AI prototyping. We’re building an app with features, live, right in this podcast. Yes, LIVE. Using all 5 of the major tools. *

**Aakash Gupta** (00:00:02)

You have been helping so many hundreds, I think even thousands at this point of PMs prototype with AI. So I'm really excited to break into that topic today. Why should people care about AI prototyping? What

**Colin Matthews** (00:00:15)

it's about is just getting through more solutions faster. Maybe it takes you three months or six months to test an idea. AI prototyping, hopefully what you'll see today is you can do the same thing maybe in a few hours or a maximum of a week. And why should PMs specifically care about AI prototyping? It actually empowers PMs the most. You can go ahead and add new features basically on top of your existing product, get direct feedback from customers, use it as an internal tool for alignment. Awesome. So let's do a live cooking session. Yeah, for sure. I'll go ahead and share my screen and we'll walk through it. I have nothing prepared for today. Actually, we're going to start from the very beginning and walk through from the back on how this is going to work. Do you want to see AI build a prototype in minutes?

**Colin Matthews** (00:00:57)

In this episode, we put AI prototyping to the test. We start with Bolt, watching AI build an entire UI from a screenshot in seconds. Then we dive into Cursor, an AI-powered IDE that helps us debug and refine the experience. Lovable takes it even further, turning a Figma design straight into code with just a click. We explore Replit, where AI builds full-stack prototypes with real databases. And finally, we dive into V0 and explore shipping AI-powered apps at lightning speeds. It's hands-on, it's live, and it's going to change how PMs and teams build products.

**Aakash Gupta** (00:01:43)

Really quickly, I think a crazy stat is that more than 50% of you listening are not subscribed. If you can subscribe on YouTube, follow on Apple or Spotify podcasts, my commitment to you is that we'll continue to make this content better and better. And now on to today's episode. Colin, welcome to the podcast.

**Colin Matthews** (00:02:04)

Yeah, excited to be here.

**Aakash Gupta** (00:02:06)

I have been following your content. I think you had that really legendary post on Lenny's newsletter about why PM should be more technical last year. You followed it up with the banger on AI prototyping this year. I saw you on Peter Yang's podcast. You have been helping so many hundreds, I think even thousands at this point of PMs prototype with AI. So I'm really excited to break into that topic today and kind of like unparalleled depth today for folks and really tactically show them how they can AI prototype. So why should people care about AI prototyping?

**Colin Matthews** (00:02:41)

Yeah, that's a great first question. I think really what it's about is just getting through more solutions faster. So in the past, maybe it takes you three months or six months to test an idea, get it out to your customers, see if they actually like it in the flow of the product, not just in a mock-up. And kind of like generate some ideas or feedback based on that. And I think with AI prototyping, hopefully what you'll see today is you can do the same thing, you know, maybe in a few hours or a maximum of a week rather than it taking you three months, six months or whatever that period of time is. And why should PMs specifically care about AI prototyping? Yeah, I think it actually empowers PMs the most out of, let's say, the set of PMs, designers, and engineers. Because once you get good enough at this skill, you can go ahead and add new features basically on top of your existing product, get direct feedback from customers, use it as an internal tool for alignment, to talk to your executive team about something you want to ship, or your engineering team about something you want to ship, and basically just use it as that communication tool.

**Colin Matthews** (00:03:42)

which is really the role of a PM most of the time is to kind of build that alignment, make sure everything's working as it should. And so, yeah, I think PMs can benefit a lot from AI prototyping.

**Aakash Gupta** (00:03:52)

I guess a picture is a thousand words, maybe a prototype is 10,000 words. Yeah, I think that's a great way to put it.

**Colin Matthews** (00:03:59)

And kind of one thing you'll see again as we go through live, but there's a big difference between looking at something in Figma mocks and actually being able to interact with it, really getting into the flow of how it's going to work in that product. And I'm sure some of you have had experiences where you've done something in a mock-up and you thought it was going to work one way in the product. Maybe it actually came out looking a little bit different or the flow was a little bit different than what you were expecting. And so really, you can get into that level of depth very quickly when you're doing it with AI prototyping tools as opposed to Figma. And again, Figma and all that still has its place, not to take those tools away, but it's just another tool in your toolbox for these types of ideas.

**Aakash Gupta** (00:04:38)

Awesome. So let's do a live cooking session. Yeah. Let's say I am somebody who's working on a product like Apollo.io, which is B2B SaaS for sales teams. It was most recently valued at two and a half billion dollars. Let's say I want to prototype paid booking links. So it has a meeting scheduler, very similar to Google Calendar's meeting scheduler or Calendly's meeting scheduler, but they want to make it paid, kind of like intro or square space. Can you walk us through that?

**Colin Matthews** (00:05:10)

Yeah, for sure. I'll go ahead and share my screen and we'll walk through it. And I have nothing prepared for today. Actually, we're going to start from the very beginning and kind of walk through from the back on how this is going to work. Cool. So let's go ahead and take a look at Apollo first. I have the page pulled up here. So this is what we're looking at, right? We have our meeting scheduler, and then we have the ability to kind of pop into here and edit and set some preferences. And kind of what I'm imagining here is that somewhere we have a UI element for setting the price. And then later on, when we're looking at the preview for this booking page, we can actually set that price, or I guess agree to it, and then pay for the meeting. Is that kind of what you were thinking?

**Aakash Gupta** (00:05:48)

Exactly. Those are the two most important things, capturing the user input when they're setting up the meeting, and then when somebody's booking, being able to pay. Cool.

**Colin Matthews** (00:05:57)

So we'll go ahead and start just with this screen here. We're going to use a couple of techniques throughout. I think generally what I'll do is I'll get started first, and then I'll explain what I did and why I did it afterwards, just because Bolt is going to take some time to build as we're talking. So the first thing I'm going to do is actually just take a screenshot. So I'm just using the built-in screenshot tool here. Grab that. and hop over into Bolt. And Bolt is one of many different tools. So there's Replit and Lovable and V0. It's one that I like for a number of reasons. One of them is that it's pretty customizable. So you can kind of set up different ways of using Bolt with different configurations. And so I have Bolt set up the way that I like to use it.

<!-- sponsor -->
**Aakash Gupta** (00:06:36)

Today's episode is brought to you by Gibson AI, the future of backend development. Imagine a world where designing, deploying, and scaling your database is as intuitive as having a conversation. Gibson AI makes that a reality. Gibson AI is your very own AI database engineer. In just minutes, you can chat with Gibson to design production grade data models, automatically generate secure REST APIs, and even eliminate technical debt that's been holding your team back. Whether you're launching a brand new product or modernizing an existing app, Gibson AI handles everything from data migrations to integration, so you can focus on building what matters most. Gibson AI is built for the modern engineering team, empowering you to accelerate development, reduce tedious coding, and deliver powerful solutions faster than ever before. Head over to gibsonai.com slash Akash to experience the future of automated data modeling. That's G-I-B-S-O-N-A-I dot com slash A-A-K-A-S-H.

<!-- sponsor -->
**Aakash Gupta** (00:07:35)

And use code Akash50 for 50% off your first 12 months. Trust isn't just earned, it's demanded. Whether you're a startup founder navigating your first audit, or a seasoned professional scaling your GRC program, proving your commitment to security has never been more critical or more complex. That's where Vanta comes in. Businesses use Vanta to establish trust by automating compliance needs across over 35 frameworks like SOC 2 and ISO 27001. centralized security workflows, complete questionnaires up to five times faster, and proactively manage vendor risk. Vanta can help you start or scale your security program by connecting you with auditors and experts to conduct your audit and set up your security program quickly. Plus, with automation and AI throughout the platform, Vanta gives you time back so you can focus on building your company. Join over 9,000 global companies like Atlassian, Kuora, and Factory who use Vanta to manage risk and prove security in real time.

<!-- sponsor -->
**Aakash Gupta** (00:08:32)

For a limited time, my listeners get $1,000 off Vanta at Vanta.com slash Akash. That's V-A-N-T-A dot com slash A-A-K-A-S-H for $1,000

**Colin Matthews** (00:08:43)

off. But for now, we'll just go ahead and get started here. And I'm actually going to start with kind of an outline of a plan rather than getting into the code, which is the first kind of major difference in the approach that most people might take. Rather than being like, hey, can you build this for me, I'm going to ask it to create a plan for me and just generally describe what we're doing. So give me a second to just type that out. Of course, you can ask a question as I'm doing that if you want. But I'm going to focus here and type that up for a second. OK, so here's what we have here. Let's build a prototype of this app. It's a meeting scheduler that allows the admin to create more than one meeting booking link. It should allow admins to edit with the detail page.

**Colin Matthews** (00:09:19)

And later, we'll be able to see a preview. And I asked it to create a plan and not to write any code. what we can see here that bolt actually returns first is a prd right so again this is a pretty big difference from kind of our normal workflow or maybe what you'd intuitively think you want to do here but basically what this prd is doing is it's describing not only what we're going to build but also how we're going to build it so we can see the admin user workflows the end user workflows here and then we have this admin dashboard we have our different you know phases to work for our workflow And then a breakdown of the different phases of phase one, phase two, phase three. We have our design system based on the screenshot. You know, we have spacing, fonts, components, and then some success metrics and additional notes.

**Aakash Gupta** (00:10:04)

Nice. And we didn't even tell it necessarily to create a PRD. We just told it to create a plan.

**Colin Matthews** (00:10:11)

Yeah, so this is part of the configuration that I have set up with Bolt is some kind of custom instructions to create a PRD first. I find that creating a PRD gives us something that we can reference back to. And so we can kind of just keep telling Bolt, yes, continue, keep building new features. And we don't have to try to maintain the context in the chat. I guess one kind of quick tip here is that the chat isn't the best at maintaining context for very, very long projects. And so having a file like this one, like a PRD, kind of helps you maintain that context over time. It's something you can reference back to.

**Aakash Gupta** (00:10:42)

Love it. PRDs are still valuable. Yeah, yeah,

**Colin Matthews** (00:10:45)

exactly. And this looks a little bit different. Obviously, this isn't what I would normally think about as a PRD, right? We have like styling and some other stuff in here that's pretty specific, but it helps guide our overall implementation. So we'll go ahead and kick off. We'll say continue with phase one and hopefully we get some implementation rolling here. So kind of while it's working on this, I'll just describe generally the approach here. So the first thing is to just break up these projects or these prototypes into components. If you try to just do the whole thing in one message, like build me this entire prototype, usually what's going to happen is it's going to fall apart pretty quick. And so you want to break it up into basically as small of chunks as you can within reason. And again, the nice part about this approach is that we already have that first step, and now we just have to continue with our additional steps.

**Colin Matthews** (00:11:31)

So really, we don't have much here. in terms of the content, but we're going to continue. One thing that I do want to ask Bolt to do here, though, is to actually try to match the design more closely before we continue. And this is a process that I call reflection, which is just, you know, giving it an opportunity to think about what it's done and then improve on that as we go along. Another quick tip is just asking it not to write any code. This basically allows you to take a look at the results first prior to it actually implementing those changes, which can be really nice if you want to make a change, right? Because you can see it's identified a lot of differences. Maybe there's something in here that I don't actually want to change, so I could remove that prior to continuing. Whereas if I just asked it to make these changes, it would have kind of gone on without me and made the changes, and I would have either revert them or try to undo something kind of as we went.

**Aakash Gupta** (00:12:21)

And I think the undo isn't that great.

**Colin Matthews** (00:12:25)

Yeah, so the undo is going to undo that whole last step. So let's say we implement something that has a bunch of things in it, like a bunch of styling changes or adds a bunch of components. If we try to undo, it's going to undo a big chunk. Rather than, again, if we wanted all of this except for we didn't want this toggle switch, for example, we could just say, OK, yes, implement that, but don't include the toggle switch. And we're a lot more precise with what we're doing by taking this approach. So yeah, now Bolt is basically working on the design changes to make the design match the screenshot more closely. You can see it's updating our layout. And then we'll have an updated design We have some new components here as well that are being created. And this is just going to split up the files to something that's a little bit more easy to maintain or is more readable for Bolt.

**Colin Matthews** (00:13:11)

And for a PM, you're probably not thinking too much about the structure of the code in your prototype. And I would agree that that's not super important. But there's general patterns that you want to see. And this is a good pattern where we don't just have one massive file, but we have a couple of small files. Again, it just makes it easier for Bolt to kind of maintain context. And so this is our second iteration. And I mean, it's a massive difference from the first iteration. It looks pretty similar to Apollo at this point, right?

**Aakash Gupta** (00:13:37)

It literally looks like Apollo. Yeah.

**Colin Matthews** (00:13:40)

Yeah. So pretty cool. So we have our first step kind of done here. And I think the next step is to work on the detail page. So I'm going to hit, well, maybe we'll add this edit first. So I'll grab a quick screenshot of this as well, just to provide that context to Bolt. And, you

**Aakash Gupta** (00:13:58)

know, a lot of this in terms of working with mockups or working with an existing product really helps it catch up quickly.

**Colin Matthews** (00:14:06)

Yeah, for sure. I mean, if you want it to look like something you already have, you know, including those mockups is, is a big deal, but obviously like you can get very specific styling almost one-to-one with what you have. And so for the purpose of prototyping, uh, really like it's going to feel similar to your users or to your internal stakeholders. So we'll continue on with that small feature, and then I think we'll implement the detail view after that.

**Aakash Gupta** (00:14:35)

What's amazing here is like we've basically already done like two steps, two pages this quickly.

**Colin Matthews** (00:14:42)

Yeah, we're doing pretty good so far. So this is actually, oh, we're still updating actually. I thought we had a little issue there, but this is a kind of a, I guess a quirk of Bolt. Sometimes it'll show you the preview before it's actually done updating. So you just gotta pay attention to the left side here, look for the check mark, and then we'll know that everything is good to go. So it's still updating our code here. All right, we'll give that a try. We can see that we have our edit. Again, almost looks identical, which is pretty cool in terms of the output here. And so now we'll continue on with our detail page. So we'll include a screenshot once again and ask it to include a detail page.

**Aakash Gupta** (00:15:23)

So behind the hood here is some really good ability to take an image and then screenshot specific elements and reuse them.

**Colin Matthews** (00:15:32)

Yeah, I think behind the scenes, they're using Sonnet 3.5 from Anthropic. They have some public blog posts with Anthropic. So it's basically Claude behind the scenes that's actually doing all the programming here for us. And Claude is a multimodal model, right? So it can both write and see things. So that's kind of how it's working behind the scenes.

**Aakash Gupta** (00:15:56)

It's not your OCR software of 10 years ago.

**Colin Matthews** (00:16:00)

Yeah, that's right. Yeah, it's come a long way. The other cool thing about this, you know, is Bolt, I think Bolt is less than six months old, maybe eight months. Someone could double check me on that one, but it's certainly less than a year old. And so you can just kind of imagine where this is going to be in a year or two years or five years if we can do this already with Sonnet 3.5. Like as we continue to get better models, this process will only get easier and easier and faster and faster, which is pretty cool. All right, so we have our next step done here. Hopefully when we click edit, yeah, we pop into this view here and I think we're good there. So I think the first thing I'm going to do is add in, we don't obviously don't have all the settings, but hopefully that's okay.

**Colin Matthews** (00:16:50)

You know, I could basically continue this process of taking screenshots, but just for the sake of time, I don't think we'll add every configuration that we have here. So we'll go ahead and add the price. And whenever I'm uncertain about how it's going to work, sometimes I'll just say, how would you do this? Don't write any code, just so I understand what approach it's going to take. And one other thing is, generally, if there's a plan, it'll do a better job, so it's less likely to create any issues or bugs for us.

**Aakash Gupta** (00:17:19)

That's an interesting quirk of LLMs. Forcing them to plan seems to help.

**Colin Matthews** (00:17:24)

Yeah, and I think we see that now with some of the reasoning models where it's basically built into the product with the new DeepSeq and OpenAI models. So it's an extra step for us to do it, but it still works just as well. And while Bolt's working on that, let me see how I actually find the preview here. There we go, preview. And I'll just double check that this new feature is working, and then we'll work on the preview as well. All right, so here's our payment settings. We have a little configure, a toggle that we check off. Then we can set our price, so let's say 50 bucks. Now there's some kind of, this is a number input. So, oh, there we go. Looks a lot better there. Maybe 50, around $50 works fine. And then we can save our changes. So everything works pretty decently there.

**Colin Matthews** (00:18:30)

We can see the price actually gets saved right on the front page. And yeah, so I think we have the admin side done. Anything you'd change so far? Wow. I'm like, I can't even speak. Yeah, it's pretty cool. Obviously, compared to Figma, maybe if you're proficient at Figma, this would be a little bit slower. But one of the cool things about this is that once you have this up and running, you can also continue to create copies. So the same way in Figma, you don't have to redesign your product every time you open it. You don't have to restart from scratch. You could create a copy of this and then basically restart from that copy. So you don't have to redo the work every single time. But we'll go ahead and continue with the preview. So I'll ask Bolt to implement the preview. And again, you can see a lot of the similar approaches.

**Colin Matthews** (00:19:15)

So how would you do this? Don't write any code. It makes a plan for us in terms of the components it needs, how it's going to set up basically the routing so that we can navigate between different pages, and so on. And so once again, we can just say yes, and we'll get that implementation kicked off. And then the last thing we'll need after the preview gets going is just adding in that payment processing on that preview. So maybe what we'll do is we'll just actually grab this view here with the select time so we can pick the time as well. And then we'll also at the same time add the pricing. I think we'd probably do that all in one request.

**Aakash Gupta** (00:19:51)

How do you typically judge what's a good size of a single request?

**Colin Matthews** (00:19:57)

Yeah, so it kind of depends on the types of changes that are being made. So I think anytime you're introducing a new feature, like a new page, it's best to get the minimum version of that page working and then add to it over time. Once you have that minimum page, let's say the preview page in this context, then something like the time selection plus a view for seeing the payment processing isn't a huge change, in my opinion. It's just not that many changes to the actual files or components. So I think that's kind of reasonable. You could also break it up if you want to be more certain that it's going to work, and there's a chance that it doesn't work. Generally, smaller is better. But I'm also sometimes a little bit impatient, and I try to patch things together where I can. All right,

**Aakash Gupta** (00:20:42)

so we'll actually go. Already so fast.

**Colin Matthews** (00:20:45)

Let's go to the preview. So there's our preview and we can select this. We don't have our time, but everything else looks pretty decent. So I'll ask it to implement the time selector. And then I'll say, also, can you add payment information? And I'll say the user should see the configured price. Anything else that you want here? Does that sound good?

**Aakash Gupta** (00:21:25)

I guess that's all we need on that page. Yeah.

**Colin Matthews** (00:21:29)

So hopefully that works for us. And then we'll be done. So it took us, I don't know, maybe about 10 minutes or so to go from nothing to the functional prototype here. Maybe speaking a little bit ahead of where we'll land, we'll see if everything works out okay. But yeah, 10, 15 minutes I think is pretty reasonable in terms of prototyping out a single feature. You know, obviously if you want to do something larger in scope, it takes a bit more time.

**Aakash Gupta** (00:21:56)

But this is the type of thing that if you, even if you're a designer, it would take you longer than 10 minutes to design in Figma.

**Colin Matthews** (00:22:05)

Yeah, that's for sure. Yeah. So our time selection's at the bottom instead of the side. So, you know, there's, there's a small change there.

**Aakash Gupta** (00:22:11)

Yeah.

**Colin Matthews** (00:22:12)

And then I don't think we actually got our ability to see the next screen. So there's something we have to fix there. Okay. Oh, it might be that I just didn't enable the price. Yeah, so this is a small thing, but it doesn't save between our iterations. So I enabled the price previously, but not the second time. So we just got to go ahead and re-enable the price here, save our changes, and then hit that preview one more time. Hit our time, and then let's see. Do we have our pricing? We do not. So this is maybe a good thing, and a good example of me trying to do too much in one go probably. So what we'll do here is we'll say something along the lines of like, I'm not seeing the pricing components. This is how I expect it to work. Can you tell me why it's not working this way?

**Aakash Gupta** (00:22:57)

OK. And these prompts are so natural language. It's not like you're applying some advanced prompting framework outside of encouraging planning and reflection.

**Colin Matthews** (00:23:10)

Yeah, exactly. It really doesn't have to be super complicated. I think it's better to have, like I said, lots of small changes rather than trying to get the perfect prompt up front. Because even if you did that, it's not going to be able to build the thing you're asking for. You can't just be like, build me YouTube. And if I build the perfect prompt, it's going to do the whole thing. It still has to be that iterative approach.

**Aakash Gupta** (00:23:34)

Seems like screen by screen or single element by single element is a good unit to think through each prompt roughly. Yeah, exactly.

**Colin Matthews** (00:23:42)

All right. So yeah, prompt years B is that I'm just not seeing the price and I want it to tell me why. And I once again said don't write any code and that I would expect to see it after the time selection. So I'm just gonna try this one more time here, I think. Let's connect to our project, make sure we're running correctly. And let's just try one last time here before I actually make any changes. So let's set the price. Hit save, and then hit preview. I think what might be happening here is actually that we're somehow losing the price when we hit save when it opens in the new tab, but I'm just going to double check here. This is a good example of debugging actually, and Bolt recommended some debugging tactics to us. Can we confirm that we're editing a meeting? We can see the price and list card.

**Colin Matthews** (00:24:40)

When you click the time slot, do you see any console errors? Can you try setting a price and enabling it for one of the meeting types in the edit form? So we can say yes, and then I'll do a check the console after. But before I do that, I'm going to say, can you open the preview in the same tab instead of a new tab? And again, this is just kind of my hunch based on the idea that every single time we're reloading, we're losing that we set the price. We could fix that as well if we wanted to. But I think that when it's opening in a new tab, we're losing the price on the new tab, and then it's not showing up in the UI. So we'll just give this a try first. And then if not, we'll go through the console and all those debugging tactics as well.

**Colin Matthews** (00:25:32)

So we'll try 50

**Aakash Gupta** (00:25:33)

here. Save. This is all happening so fast. Preview.

**Colin Matthews** (00:25:40)

There we go. Okay. So there's our payment information. So I was right. It was just based on the fact that we had the two tabs. So one way to fix it is what I did here, which is rather than it opening in a new tab, I opened it in the same tab. Another way to do it would have been to save that $50 in something that works across tabs, which would be called local storage for a web browser. And so I could have fixed it either way. But again, that was just a hunch that I had that that was the problem. And it turns out that it was. But anyway, so we have our payment processing here. Maybe we don't love this like workflow. So we want like... this card to appear after we pick the time rather than right below. But again, you can make these iterations however you want based on just natural language as we go along here.

**Aakash Gupta** (00:26:22)

Great. So we've debugged it. We have the prototype. Now we basically are ready to put it in front of users and actually see if they might resonate with this and get more data, right?

**Colin Matthews** (00:26:32)

Yeah. There's actually some really cool things. So because this is a product, you know, it's a code, you can actually hook up any type of product analytics tool that you like, like Mixpanel or Postdoc. So you could get product analytics events. You can watch recordings. Obviously, you can always just put it in front of a customer and watch them try to use it. That's probably the best way. But whatever kind of product testing ideas or frameworks that you like, they're applicable here as well.

**Aakash Gupta** (00:26:59)

It seems like there's a future where user research and design and product management are all using tools like this.

**Colin Matthews** (00:27:09)

Yeah, I could definitely see that. I think, you know, even what I just mentioned, there's, I think, third party tools that kind of plug into Figma where people can click through Figma prototypes and you can try to watch recordings of that. But This honestly just is very quick, both in terms of building and iterating and can plug into your existing tools that you're using for your real product. So I think, yeah, there's definitely a world in which this is just the norm. And as I mentioned earlier, if you imagine that this gets even better than it is now, then really anyone can do this. They have to be super technical. I mean, other than the fact that I had that one idea, one hunch about what the problem was, there was really nothing technical about what I did here, right? These were all pretty natural language prompts.

**Aakash Gupta** (00:27:51)

And I imagine we could have been a little bit less pointed in our direction with Bolt and just said, you know, this is the issue we're facing and it might've been able to help diagnose that too if we had described the user scenario.

**Colin Matthews** (00:28:02)

Yeah, absolutely. We kind of could have walked through that. I mean, it did try with some debugging tips here, but yeah, we could kind of try to ask Bolt to help us out and then kind of see where we land from there.

**Aakash Gupta** (00:28:15)

So we just use Bolt. What is the pricing on a tool

**Colin Matthews** (00:28:18)

like this? Yeah, Bolt's $20 a month, I think, at the lowest price. And you get usage, so it's 10 million tokens. Let me see what we used there. So I was at, let me just go into my subscription here. So I was at 26.6 before we started, now I'm at 26.3. So out of 10 million, we used 0.3 million for that one. So you could probably build 30 of these. Maybe that math doesn't quite add up, but something like that each month based on the $20 a month plan.

**Aakash Gupta** (00:28:50)

Wow. And what's the broader landscape of AI prototyping tools and when should you use Wedge?

**Colin Matthews** (00:28:58)

Yeah, that's a great question. It's definitely a confusing space. There's a lot of tools nowadays and people have both their own preferences, but, you know, Basically, I break it up into three segments of tools. So the first one is just basically your chatbots. So this is like ChatGPT or Claude. They can actually do some really basic prototyping if you want them to. So they'll, in response to a regular message, if you just ask them to be like, make me a mock-up or a prototype of something, they'll write some code and display it in the UI for you. Then there's the second classification, which is something like Bolt, where it's a web-based tool. It has everything built into it. So I can, for example, export my code. I can deploy it to a web link or a website. Everything is kind of built in here. So this is things like Replit, Bolt, Lovable, and V0.

**Colin Matthews** (00:29:45)

And then the last section would be IDEs, which is something a developer would use. So it's like Cursor or Windsurf, which isn't really like an AI development tool per se, because you can really just write normal code in it as well, but it's more AI enabled for developers. And I would say for most product people, you wouldn't want to be using Cursor or Windsurf, just because you have to set up everything on your own computer correctly. Whereas with Bolt, it's basically a little, environment that they give us where we don't have to do any setup.

**Aakash Gupta** (00:30:18)

And I think in your post with Lenny, you described how certain tools cover server code, client code, and database. How did those tools break down? Yeah.

**Colin Matthews** (00:30:29)

So what we just did here is a client-side only application, basically the front end, right? So, you know, if we wanted to actually use this, there's nothing behind the scenes. There's no server database. This data doesn't get saved anywhere or anything like that. If you want to build something that is more close to a real product, so you have authentication, you can store data over time, then you're going to need a database and a server. So Replit is the best tool for that. They offer that. You can also connect to third-party tools to offer the same solution, servers and databases, through Bolt and Lovable. So you can see up here, we have that Connect to Subabase button. That's exactly what that's offering. But I personally find for the purpose of prototyping, most of the time, I don't need to do that. I can just stick with the client side only.

**Colin Matthews** (00:31:15)

And it's really only when I'm building like personal software or something that I think, you know, is going to be a real product that I'd be using the server and database to do that.

**Aakash Gupta** (00:31:28)

So there is a certain degree of hype factor to AI prototyping for PMs. What do you feel like is the actual ways in your day-to-day as a PM you should think about, okay, this is a scenario where I should bring AI prototyping in instead of X that I was doing before?

**Colin Matthews** (00:31:49)

Yeah, well, one is honestly as a Figma replacement, I actually think at some point Figma should or will do something similar to what we just did because most PMs are not skilled enough at Figma to do what we just did. Certainly not in that amount of time that we did it, but just generally, like I know I'm not good enough at Figma to do what we just did. And so, yeah, just like prototyping an idea, testing your idea on your own. I think it's a really good tool for that. And the second one is... really like prototyping more of an experience rather than just the UI. So if you think about like an AI product where you have an LLM on the backend, right? Like chat, you know, chat CPT or something like that. You can't really prototype an experience like that and get user feedback inside of Figma.

**Colin Matthews** (00:32:36)

You need something where the person actually interacts with it, interacts with the AI agent or whatever it is, in order for you to get valuable feedback. And the cool thing about this is because this is code, you can integrate with an API and call an LLM and just build an actual AI feature into the product very easily. So if you want to test that idea, should Apollo have an AI chat that can do stuff for us, you could just actually build that AI feature on top pretty easily.

**Aakash Gupta** (00:33:07)

At some point, building is overrated. What is the line between, okay, I should be doing better discovery and talking to customers versus, okay, I should go prototype this?

**Colin Matthews** (00:33:19)

Yeah, that's a great question as well. So I think of AI coding tools like this one or AI prototyping tools as tools for communication primarily in this context. It's not about... Like the code that we have here, if we flip back over to this code, one idea you might have is like, oh, I already built the feature. Why don't I just hand this code over to the engineer? And they're going to be done so much faster. It's really not about what we've built here from the perspective of building the feature. It is really just about communication. And so the way that I think about this from building versus talking to customers is that you should be using these tools to talk to your customers. And that really like the faster you can build, doesn't mean that you should just ship more features, like ship 10 times the features or 100 features in the time that you could have shipped one, but instead that you should have 10 more or 100 more conversations with your customers and richer and deeper conversations with your customers where they can provide you with better feedback rather than just one conversation with your customers.

**Aakash Gupta** (00:34:23)

So if we're putting this all together, if you're an AI native product team, you're an AI native PM and you're trying to use these tools the best way, I guess we would want to put these together with our overall opportunity solution tree. So how does it all come together to create an end-to-end discovery process that is way more effective than the old one?

**Colin Matthews** (00:34:44)

Yeah, actually, I don't know if Teresa Torres listens to your podcast, but if she does, Teresa, this is a call out to you to, one, ask if you could put something together on this, but two, just thanks for all the work on Opportunity Solution Trees. So yeah, I'm a massive fan of Opportunity Solution Trees. And just in case anyone's not familiar with what they are, it's basically you start with you know, some opportunity, or sorry, there's some outcome that you want to go after, right? So typically it's a product metric that you want to change. You have a set of opportunities or problems related to that. And then you have a set of solutions that relate to each opportunity or problem. So maybe if our outcome is like, you know, reducing churn, an opportunity would be improving our onboard experience. And then a solution would be like how we improve that onboarding experience.

**Colin Matthews** (00:35:29)

So maybe it's like guided emails, or maybe it's an in-product guide. There's more than one way to improve the onboarding experience. Below those solutions is hypothesis, right? So like, you know, we have a specific idea we want to test. And what I think is that basically in that kind of solution hypothesis range, so, you know, you still start with reducing churn and you still have the idea of improving the onboard experience. But then the how part, you can test different methods of how can we improve the onboard experience much, much faster by using these tools. So it basically fits into that bottom section of solutions and hypotheses and basically testing those hypotheses quickly. And again, getting good feedback on your product experience by giving something that feels more real than a Figma prototype.

**Aakash Gupta** (00:36:14)

Amazing. I really think this is such an important thing for PMs. And I don't want PMs to only think that they have to use Bolt. So can we see now maybe another tool in action, perhaps cursor? It's kind of a very sexy tool. And in this case, maybe what if we try building AI sequences for Apollo? Yeah,

**Colin Matthews** (00:36:36)

sure, that sounds good. So generally speaking, moving between different coding tools can be a bit tricky. It requires a little bit more technical knowledge. So what you'll see me here do is basically export the code, get it running in Cursor. Generally speaking, I would say that this is a little bit trickier to do, but we'll go ahead and get that started. So first thing I'm going to do is just export that code, and then I'm going to open up Cursor. and open the same directory inside of cursor. And you're going to see cursor in case you haven't used it before. It's really like a code editor. It looks a little bit more intimidating than Bolt, which is one of the reasons that you might want to use Bolt or something similar. So here we have our code. Again, this is the exact same thing. If I kind of get us running here first, we just need to install our content.

**Colin Matthews** (00:37:22)

So I'm going to run a little command here to do so. This is installing all the libraries in the background that this project was using. And then if we run our command here to get our project up and running, now it's running on my local computer. So we can see localhost instead. Localhost just means it's running on my computer, but it's the exact same view basically that we had before. And then over in Cursor, they actually have something they call Composer. So Composer is very similar to Bolt, basically. It's a chat. And when I'm using Cursor nowadays, I actually don't write any code at all. I just use this the entire time. And the nice part about Cursor, just in case you're wondering why you might want to do this, is I personally find Cursor can be a lot more pointed in its solutions. So if there's a particularly troublesome bug that I can't figure out, I'll actually bring it down to the cursor to try to figure that out.

**Colin Matthews** (00:38:14)

And the second reason is you can switch between different models. So one workflow that I do sometimes is I flip over to 01 rather than Sonnet 3.5. And 01 just seems to be better at more complex issues. But yeah, so we'll go over to our sequences. Oh, sorry, I literally forgot that I wasn't looking at Apollo. I clicked on sequences in this, but I meant to do it over here. It

**Aakash Gupta** (00:38:40)

looks that

**Colin Matthews** (00:38:41)

similar. So this is our sequences, and we can click create a sequence with AI, and then it generates a sequence for us. And let's say that I just want to improve this feature. And what I think would be an improvement would be that it asks me some questions before generating the sequence and maybe also uses some social proof in the sequence. So it says like 874 other people have used this sequence and gotten 57% open rates or something like that.

**Aakash Gupta** (00:39:09)

If you're enjoying this podcast episode with Colin, you'll love his course on Maven, today's podcast sponsor. The problem with most courses online, like Udemy, is there's no live component and the instructors aren't experts in their fields, they're professors. At Maven, you get direct live access to experts and operators from the world's best tech companies. You can't get that access anywhere else, in any university, and you usually can't find them on YouTube either. I featured so many of Maven's experts in the newsletter and podcast for that reason. To help you out, I've put together a collection of courses I recommend at maven.com slash x slash Akash. This includes courses like AI prototyping for PMs, product sense for PMs, and getting an AI PM certification. Visit it now at maven.com slash x slash A-A-K-A-S-H.

**Colin Matthews** (00:40:02)

um so you know it's compelling for me to use it like yeah i think this is a good sequence and also it seems personalized or hopefully it is personalized based on the information that i'm providing so we're going to do a very similar approach to what we did before

**Aakash Gupta** (00:40:17)

I love seeing an improvement to a feature I shipped.

**Colin Matthews** (00:40:20)

Yeah. So you can still paste images inside of the Composer here. Again, it depends on the model. So as I mentioned before, Sonata 3.5 is a multimodal model. This works just fine. 01 is not. So if I try to send an image to 01, it doesn't work. But we're going to start by saying, well, I guess one is, can you implement this? Yeah, so can you implement this view? This should appear when I select sequences. And again, you're going to see a very similar workflow. Overall, it's going to write the code for us. I'm going to apply the code changes, and then we'll see it show up. So there we are. Still working through it. But as I mentioned, behind the scenes, Bolt is using the exact same model. So this is actually going to feel very similar to using Bolt. So we apply those changes, pop back over here, go to Sequences, and we do not have anything on our screen.

**Colin Matthews** (00:41:26)

So we'll have to take a look at why.

**Aakash Gupta** (00:41:31)

All right, so now debugging in action.

**Colin Matthews** (00:41:33)

Yeah, that's right. OK, so the problem is that I actually made a mistake. And I make this mistake fairly frequently, which is I forgot to pass in the correct context. So one thing that's different about cursor is that you have more control over how it works, which can be a good thing and a bad thing. On the bold side, it decides for you what the relevant context is to send over, so basically what files are relevant. And I forgot to send any files as context. So I'm going to say, can you integrate this into my app? And this time, I'm going to press Command Enter, and you'll see that it sends my files over rather than not sending my files. So that was my mistake at the beginning there. So it's going to update my existing files, hopefully. And one thing that maybe would have been a better approach, I might still do this anyway, is actually to revert this first one because it made these changes or these updates with no context to what I was doing.

**Colin Matthews** (00:42:30)

And so I don't know if any of this code is actually valuable to us, whereas the second set would be based on our actual content. We'll give this one more try. And let's see what we have going on here. Yeah, so I think what I might do is actually just revert back. And you can see that we have a little restore button at the top here. So revert all files to before. Continue here. Double check that we can see our content from before. Basically, just ask the same question, but this time pass in the current context. And that's another kind of, I guess, quick tip is rather than doubling down on mistakes, it's best to just revert when you can. Because I could spend probably 15 minutes, 20 minutes trying to debug why that wasn't working, or I can just flip it back and fix it so that I send the correct message the first time.

**Aakash Gupta** (00:43:32)

And it's cool that you can just flip it back that way.

**Colin Matthews** (00:43:35)

Yeah, it's really not that hard. I mean, it's pretty intuitive. And so now we have something that looks correct. We have our sequences, and we want this button to do something. So we'll flip back over to Apollo, click here, and grab this screenshot. And what I'm going to do is I'm going to ask it to implement this as well, but with a bit of a difference. So let's start with, can you implement this for the AI button? Something like that. And then I'll say, before showing me the sequence, can you collect some data from me? That would help shape the sequence. And I'm not even going to tell it what to do. I think this is maybe one of the cool parts is, Normally, you'd have to say what I want. I want these data elements collected. I'm just going to give it free reign to decide what it thinks is relevant in this context.

**Colin Matthews** (00:44:49)

And I'll say, can you also add some social proof to the sequence at the end, like the number of users who have a similar sequence? And yeah, passing in the context is pretty critical. So I made sure to get it right the second time. But yeah, very similar workflow here. So it's going to add some questions for us. Again, I didn't decide what those questions were. Maybe they're not relevant. But I find most of the time, it actually does a pretty good job of figuring out, based on the context, what to do. And in some ways, this honestly replaces The PRD, right? Normally this would be part of your PRD is like figuring out what to do, what questions to ask. You can just prototype it directly in here and see how it does.

**Aakash Gupta** (00:45:42)

And people can give such better feedback if they actually see it in the product like this versus read it in a PRD and their eyes glaze over.

**Colin Matthews** (00:45:49)

Yeah. I mean, I'm sure many people have had this experience, but I've written long enough PRDs that I've been told by my engineer, like, oh yeah, I read half of it. Yeah, which definitely feels great. But if you can communicate the ideas with a clickable prototype, rather than that, your engineer is going to have no problem clicking through a couple of views and starting to have some questions rather than reading half the purity. So let's go back over here. So here's our new flow. So create with an AI sequence. I want to book more meetings. I am in health care.

**Aakash Gupta** (00:46:30)

This is legit. It's come up with a multi-stage quiz.

**Colin Matthews** (00:46:34)

Yeah, let's say VP director level and cost optimization. So it generates the sequence for us. And here's our social proof, right? So yeah, those are the changes we were targeting. And I'd say, I mean, I literally didn't give it any direction and it came up with what I would say is pretty reasonable implementation here.

**Aakash Gupta** (00:46:54)

Very nice. And we didn't really run into any issues. So people keep saying that debugging is such a big deal, but we didn't really run into any issues that were generated by cursor itself, just some user error that we went back and reentered something.

**Colin Matthews** (00:47:11)

Yeah, debugging is definitely a critical skill. I find that usually it looks a little bit easier when I'm the pilot just because I have some prior programming knowledge. And so I know generally what it's doing. There's definitely a strong skill to have in this context. technical skills somehow go out the window. In fact, it's kind of the opposite. Technical skills make you even better at doing this. But yeah, we got pretty lucky, I would say. Usually it's like 20% chance that something goes wrong on a given message. We also aren't doing anything on the server side or with the database. So we're minimizing complexity. And that actually goes a really long way as well. Just keeping things simple just increases the probability

**Aakash Gupta** (00:47:55)

that everything is going to work correctly. So for prototyping, if you can stick to prototyping and you're not trying to build a full functioning app, you can really reduce a lot of the errors and debugging steps.

**Colin Matthews** (00:48:09)

Yeah,

**Aakash Gupta** (00:48:09)

exactly.

**Colin Matthews** (00:48:09)

It's really when you're trying to integrate with APIs or external services or database or setup authentication where things get a bit trickier. But for just general prototyping, I would say this is pretty representative. um sorry i'm still just shocked like how good of a job it did like even like

**Aakash Gupta** (00:48:26)

the

**Colin Matthews** (00:48:26)

styling like the low like everything looks almost perfect but anyway um yeah yeah to answer your question directly yeah that's really right

**Aakash Gupta** (00:48:34)

I am shocked as well. I mean, these demos are going so, so fast. So I wanna do another one here. The other tool that, you know, is really sexy right now is Lovable. And I think Lovable is really useful for Figma conversion to prototype. So let's walk people through that. Yeah,

**Colin Matthews** (00:48:50)

sure. Let's go through that. So let's hop it over into Figma. And we will pick up on a design here. So what I actually did ahead of time, and this is pretty funny, that this works as well. We'll see how well it works. I wouldn't recommend this workflow necessarily. Maybe we'll do one more afterwards. But I literally took a screenshot. This is like you can see in filming. This is just a picture. And we're going to try to convert this to code. So what I'm going to do here is I'm going to run the plug-in here. Sorry, the little screenshot thing was in my way. I'm running a plug-in called builder.io. This is another third-party company that has an integration with Lovable. So one is, I guess, shout out to Builder.io because this is so far the best Figma converter that I've seen so far. Two, obviously, you'd have to pay additional money to Builder.io if you want to do a lot of conversions or have some specific requirements.

**Colin Matthews** (00:49:46)

But generally speaking, you can install this plugin, create an account, and run this as much as you want to. I don't know if there's an actual limit, but I have never hit it. without really seeing anything other than this Figma screen and then directly over into Lovable. So what Builder does is it actually generates the first outline of the code based on the screenshot or the content. And then over in Lovable, we'll get the second iteration. So here you can see a couple of different iterations of what kind of came up with. And we get to pick which one we like. So maybe the bottom one. I think that's the closest. And then we click Open Levelable. And then this will take a little bit of extra time as well. But we'll actually get the initial screen of a functional prototype where you can continue to iterate it on over time, very similar to what we did in Bolt.

**Colin Matthews** (00:50:34)

We're going to just be on that first screen. And this is nice because This process gets you much closer to your actual designs than just the screenshot. Although, to be honest, the screenshot approach worked pretty well today. Most of the time, it gets close, but not quite as close as we did today. Today, it was like an outlier, honestly, from my perspective in terms of just how close we got with just the screenshot. All right, we got an error on that one. That's OK. Maybe I'll give it a try with the other approach here. And we'll take a look at an actual file that has some content here. I did actually do this once before, so maybe before we move on, let me all show you what it looks like. And we'll try the other way. So this is what I had from just the screenshot.

**Colin Matthews** (00:51:15)

We have kind of the import here. And again, you can see we have a very similar approach to what we had in Bolt. So this one looks a little bit different, but very similar to what we had before.

**Aakash Gupta** (00:51:28)

So screenshot can work, but Figma with all the proper sort of elements described and things like that is going to be better.

**Colin Matthews** (00:51:35)

Yeah, exactly. So let's hop over into this one here. This is a UI kit that I have, and it has some kind of prebuilt stuff we can use. So I'm going to grab a dashboard for us.

**Aakash Gupta** (00:51:48)

So this would be a really powerful workflow for, for instance, user research teams to be able to take a Figma design and convert it into a prototype to have a better working task.

**Colin Matthews** (00:52:00)

Definitely, if you want to get that one-to-one view of what you already have rather than something that looks similar, then this approach works a lot better. So we're going to do something very similar. You go ahead and click basically the screen that I want to convert, run that step one more time here, and convert this to code. And then this is actually using the proper Figma content with all the layers and all that content that you're used to seeing inside of Figma. So this will analyze the Figma layers, convert it over for us, and then we'll open it in lovable one more time here. And then maybe if we have time, I'll give the last one another shot just because it was working earlier, but we had a bit of an issue with the screenshot approach there. And yeah, this one can take a little bit of time.

**Colin Matthews** (00:52:44)

I find like the more content there is in the screenshot, the longer it takes. So this one might take like two to three minutes in total. But again, it does a pretty decent job of creating a view that looks similar to what we have in Figma.

**Aakash Gupta** (00:52:56)

So while we're waiting on that, how much do lovable builder IO and cursor cost?

**Colin Matthews** (00:53:03)

Yeah, they're all pretty much priced the same. So it's either $20 or $25. So you can definitely rack up a good bill if you subscribe to all of them. My general recommendation here would be pick one tool that you like and then just stick with it. The tools are changing so quickly anyway that you know, three months from now, they're all going to have different features and different, different, you know, tools within themselves that like, like, you know, this Figma conversion was new in the last month, for example, that's just picking one and sticking with it is probably the best bet so that you feel comfortable with what you're doing and not like switching between them based on like the newest feature. Because again, they just all change so quickly that they'll probably all have Figma imports in like three or six months or something like that.

**Aakash Gupta** (00:53:51)

It's insane that they're such young products, but so stable too. I've worked on mature products with more errors.

**Colin Matthews** (00:53:57)

Yeah, yeah, for sure. Yeah, they work really, really well. And I guess kudos to those teams on that, especially because these are non-deterministic products, right? Like it's using an AI model behind the scenes to try to write code. And I mean, I'm sure you've used LLMs before. They're not always the most reliable, right? So yeah, I mean, they work pretty well.

**Aakash Gupta** (00:54:19)

Lovable seems to be taking the longest time, but I think it's a lot related to how many elements are on this screen compared to the other screens we had.

**Colin Matthews** (00:54:26)

Yeah, I'd agree. Also, hopefully in two minutes when this is done,

**Aakash Gupta** (00:54:32)

what I'm about

**Colin Matthews** (00:54:33)

to say is correct. But I've found that this process does the best job of creating a one-to-one mock, like literally identical. If you take a screenshot and you put this into Bolt or something like that, it'll look similar, but not the same. This process in the past for me has done a fantastic job of imitating exactly what I have in Figma.

**Aakash Gupta** (00:54:54)

It's getting so much more metadata about your design.

**Colin Matthews** (00:54:56)

Yeah, exactly. Like a screenshot, really, you're not sending any data about the design. You're just sending in the screenshot to be analyzed by Sona 3.5 or by Claude. Whereas here, we're actually kind of like using the content inside of Figma, like the actual layers, you know, the metadata, but like, fonts and colors and all that stuff to try to build the mock-up based on that. So there's a lot more information that's being passed here between Figma and Builder.io and Lovable than just a typical screenshot would do. And yeah, it looks like we're almost there. Finalizing project, hopefully we can wrap up soon on this one. There's still going to be like, once we import it into Lovable, it'll probably take another minute once it's in Lovable. So again, this one's a little bit slower. But I think hopefully what we'll see is it's worth the wait.

**Aakash Gupta** (00:55:42)

This is how much time I expected everything to take. So it's really a testament to how fast Bolt and Cursor are.

**Colin Matthews** (00:55:49)

Yeah, that's true. Bolt is very quick as well. Out of the set, I think Bolt is the fastest. Cursor is really fast just because it's on my local computer. So there's less that it has to do in terms of the background. processing, whereas the other ones are all cloud hosted, so they have to do a bit more work because of that. But yeah, I mean, they're all extremely quick. The other ones, again, if you increase the complexity, it's going to take a bit more time. So if you have a database and you have to make database changes or something like that, then that'll take a bit more time as well.

**Aakash Gupta** (00:56:19)

And what's the scenario where you might want to do that?

**Colin Matthews** (00:56:23)

Yeah, so I mean, maybe while we're waiting here, I can talk through a couple of the other small things that I've done. Well, as I say, that we wrap up. But basically, if you want to launch a real project or real product, so I have a couple of things that I've built over time that I use on a day-to-day basis. I'm sure people know that I teach on Maven. And one example is that I built my own referral system. So students can refer other students. And it provides the person who's creating the referral code, this prior student that I've already had, it gives them their own unique link. I basically have authentication. It stores all their page views, like its own little referral product that I built. And I built that one on Replit. And that probably took me about a day to make. But not like 12 hours or anything like that, maybe six hours in total.

**Colin Matthews** (00:57:08)

But that's a good example where you want to have a database and that whole kind of set of features is where you're trying to offer a real product or something that resembles a real product rather than just the prototype.

**Aakash Gupta** (00:57:19)

a real growth factor for your life. That's amazing. I mean, the ROI on that six hours is probably so high.

**Colin Matthews** (00:57:26)

Yeah, I've actually already had my first referral sale, which is pretty crazy. I didn't think it would come in that quickly because I just shipped it, again, maybe a week ago. But yeah, no, it was a pretty cool system. And also, you know, just fun to see that I could ship something like that. That's a bit more complex. It has like a Stripe integration and all that in a relatively short period of time. But yeah, so here we have our new mockup. And it did a pretty decent job. There's some weird artifact on the left-hand side here in the navigation. If I open this up in a larger screen here, you can see something's not quite right there. But overall, it did a pretty decent job, I would say, of replicating that Figma mock we had. I'll just flip back for a second so you can see that here.

**Aakash Gupta** (00:58:07)

So how do we debug that artifact in

**Colin Matthews** (00:58:09)

the navigation? Yeah, that's a good question. So basically, it's going to be a very similar approach. So we can go ahead and take a screenshot here, throw that into Lovable. And at this point, we're basically back over to where we were with Bolt. Obviously, a different tool, but very similar process of clicking through. And we can ask some questions here. The other thing you can do is you can actually select different elements. So you can see that it has an image or a div on the left-hand side. So I can say, can you remove this div? And that's one nice feature of Lovable that some of the other ones don't have is this kind of selector tool where I can select different elements of the page just to be a bit more precise with what I'm trying to do. Very cool. And yeah, we'll see if it works here, and then maybe I'll move on to it.

**Colin Matthews** (00:59:03)

Actually, I can walk you through that referral tool that I was mentioning earlier. One other thing about Lovable, just while we're here, is Lovable is in some ways more friendly to non-technical users because you can't actually see the code. So nowhere in here is there a code editor. That's a good thing in some ways. Obviously, it's a little bit less intimidating. I find that sometimes it's not as good if you want to see a little bit about what's going on. So if you want to learn how to code, for example, or just generally understand what's happening, then it's not quite as good to not be able to see the code. And so just pros and cons, depending on your preference. But in this case, no code available to us to actually see. And we can see that it removed something, but not the one that I actually wanted here.

**Colin Matthews** (00:59:53)

So I'm going to say, can you remove this div on the left side? And again, just trying to be more specific, more precise is good. It was probably too general. I relied a little bit too much on that selection being kind of all I needed. And all I said is, can you remove this div? And it didn't quite work. So again, just generally be more specific, be more precise, and you'll get better results.

**Aakash Gupta** (01:00:30)

That's a relatively minor thing anyways. For the purpose of your prototype or your prototype as PRD, as we're suggesting some PMs start to think about it, might not always be the highest ROI thing too.

**Colin Matthews** (01:00:42)

Yeah, I would agree with that. I would say this is probably a pretty small thing to change.

**Aakash Gupta** (01:00:46)

I think we

**Colin Matthews** (01:00:46)

got rid of the little gray coloring. You can see I'm kind of just having to iterate through. So there's still this little, whatever this artifact is here. It looks like some kind of icon that's getting cut off. So we made some progress, right? We got rid of that gray color, but maybe we'll leave it there for now, just so we don't spend more time trying to clean up this.

**Aakash Gupta** (01:01:01)

Yeah, because we got to see Replit and what Replit can do, because it sounds like that's the one to go to. That's the final stage, I guess you could say. We got lovable, you don't even see code. Bolt, you see the code. Cursor is an IDE, and then Replit is an IDE with database capabilities.

**Colin Matthews** (01:01:20)

Yeah, that's exactly right. So maybe I'll show you one of the tools that I built previously, and then we'll hop into something new, perhaps. So I'll start with something simple, this Substack imagery size. Actually, you might really appreciate this one. So for whatever reason, I've never been able to figure out what image sizes Substack wants from me. Every time I put something in the preview image, it seems to get cut off in some weird way. And so what I built is this little tool here where I can just put whatever image I want in here. So let's just say this one here. And I process the image. And it resizes it to all these variants. And then I can use

**Aakash Gupta** (01:01:55)

whatever

**Colin Matthews** (01:01:56)

variant I want. So if I'm using the feature layout, I can use the feature one. If I'm using the cover layout, I can use the cover one. Just because I kept getting so annoyed that I was trying to fix this in Canva. My stuff kept getting cut off and I just hated it. You've

**Aakash Gupta** (01:02:09)

got to publish this to the web so you can

**Colin Matthews** (01:02:13)

use it. Yeah. This is one that just bothered me so much. It's just like a little personal tool that I built. Which

**Aakash Gupta** (01:02:20)

is hugely valuable. I think people might be sleeping on this, but one of the best SEO hacks in the world is to build tools like this.

**Colin Matthews** (01:02:28)

Oh, yeah, for sure. Yeah. Engineering is marketing is, I think, the word there. But yeah, stuff like this is great for, you know, marketing your product. But obviously, I probably couldn't monetize this, but I could maybe use this as an example, like for my course, right? Yeah. in some ways. This is a good example. And again, on the left-hand side, you're going to see that we have our code. This one is running both a client and a server. So we have a back-end server here. I'm not going to bother going through the code here, but that's what this is. And then our front-end view on the right-hand side, you can see the actual results.

**Aakash Gupta** (01:03:00)

Can we start from zero in Replit? I want to maybe just do something simple. What if we just did a database where it actually had the other element of the database for a to-do list or something just so

**Colin Matthews** (01:03:14)

simple? Sure. We'll do, can you create me a to-do list? And I'm just going to tell it to use React. What I'm doing here is specifying the technology. So most of these tools can only use JavaScript-based frameworks for building web apps. Replik can use Python as well. Python is really, really great for data-driven applications, so like imagery sizing or image conversions or stuff like that. For things that you want to look a little bit better, then typically I wouldn't recommend using Python. I'd recommend using JavaScript. And so me saying use React is me just telling Replit to use a JavaScript framework. So it doesn't recommend using Python instead.

**Aakash Gupta** (01:04:06)

Got it.

**Colin Matthews** (01:04:09)

Yeah, so we're going to get our to-do app. Replit actually kind of takes on bigger chunks of work with the agent here. So one thing that's a little bit different is they have two different chat modes. They have the agent and the assistant. Well, it's kind of like an automated developer, as I said. So it takes on very large tasks, and it does all the work for you, whereas the Assistant can basically be used to make small iterations. So if you want to just change a font or something like that, you'd use the Assistant. And what I've done over time is I just use the Agent maybe once, twice in the entire project. I really just use it to get going. And I use the Assistant most of the time to make small

**Aakash Gupta** (01:04:49)

iterations. People are always asking, what are AI agents in action? Here it is, in action.

**Colin Matthews** (01:04:55)

Yeah. Yeah, we have our to-do list here. And that works reasonably well. So at this point, I don't think we have a database set up. But if we want one, we hop over to database. We click the button, create a database. That's it. That's all it takes. And then we just have to ask it to hook up to our database.

**Aakash Gupta** (01:05:18)

So it's really easy and integrated in Replit versus in Bolt, I think we saw something about a Supabase connection.

**Colin Matthews** (01:05:25)

Yeah, that's right. So you have to connect to an external product, in this case, Supabase, in order to use a database or like setup authentication or anything like that. The nice thing about Replit is that It knows about everything that you're doing. It has context to the entire project. And so if you want to make changes, it can change your database very easily, or understand what's going on with that database. I always found with the Superbase integrations that's less true. they might make assumptions about what's in database or what's in Supabase. So they may make assumptions about how things are working, even though they're not configured that way. And so I would generally recommend using Replit for any type of full stack application that you have to build, so client server and database, rather than the Supabase integrations. If you are going to use a Supabase integration personally, I found lovables is the best out of the set right now.

**Colin Matthews** (01:06:19)

Again, this changes every two or three weeks. So it could be different three weeks from now. But today, lovables is the best out of the set. And that's fine. And actually, one kind of cool thing here. So it was running some commands for us. And then you can see it said that there's errors and it needs to fix them. And there's pros and cons to this, but Replit will just basically, you give it a task and it just goes. You don't need to interrupt it. If there's errors, it will detect the errors and try to fix them by itself. It just continues indefinitely. The good part about that is it just fixes problems by itself, which is great. The bad part is sometimes it just gets in a loop of it can't fix the problem. And so you have to interrupt it and try to get it to work yourself.

**Colin Matthews** (01:07:06)

So there's definitely pros and cons to the different tools. And yeah, so our app crashed. We'll see what happens here. Try to run it one more time

**Aakash Gupta** (01:07:18)

after

**Colin Matthews** (01:07:18)

that.

**Aakash Gupta** (01:07:19)

So this is the first time we're really running into the tool crashing potentially. And that's what we said. Once we add complexity, it's more likely to.

**Colin Matthews** (01:07:27)

Yeah, exactly. And I'm not sure what the reason is at this point. So we'll see in a second. You can actually see it's running a SQL command for us to check if there's any content in the database. So actually, if you think about this, this is incredibly cool. The agent is running a SQL command to look at the content in the database to see if our app is working correctly based on there being content stored. Like, I don't know, that just seems kind of insane to me that it's checking our database content by

**Aakash Gupta** (01:07:54)

itself.

**Colin Matthews** (01:07:55)

Yeah. So we'll try again. We'll do test. We have our content here. And then now if we look at our database, we can actually just click my data. And we see that our database record is right there. So now this is like a proper to-do app, right? It stores actual content rather than us losing it every single time we refresh the page.

**Aakash Gupta** (01:08:15)

And then I guess the next level up would be to add like authentication. So how would we do that? It's

**Colin Matthews** (01:08:21)

actually really not that hard. This is how you do it. Add auth. And then it'll add authentication. Yeah, it's really not that complicated in Replit, to be honest. It has a lot of this stuff built into it directly. So if you want to do like Google authentication or something, that's a bit more work. But just like email password authentication, you just ask it to add auth and it will.

**Aakash Gupta** (01:08:45)

And for $20 a month with Replit, you can still build like 10, 20 apps?

**Colin Matthews** (01:08:50)

Yep. Yep. You can rebuild. I mean, I have a couple of apps. I'll maybe pop over to another tab here while it's working on that. So I have some deployments, which are these are apps that are running in production that users are using. So I have two deployments right now. And then I have a variety of apps that I built. You can see I have a bunch. I also delete these every once in a while. I try to clean it up. But yeah, I would say you can basically build as much as you want to build with this within reasonable limits.

**Aakash Gupta** (01:09:24)

And is there a point where you add so much complexity to the code base and it's such a complex app that the LLM just struggles with the context?

**Colin Matthews** (01:09:32)

Yes, 100%. So context is kind of the most important element of this whole thing. So as the app gets bigger, they just do a worse and worse job. For whatever reason, Cursor has done a good job of implementing a solution where it basically identifies the correct context for you. So if we flip back for a second, you see that when I sent those prior messages, well, it's not showing up now. But if I send a message with context, I don't have to specify what the context is. So I'll just say, tell me about these files. And I can just hit this button. And Cursor actually decides what the relevant context is. And they actually score, you kind of saw in the pop-up there, score based on some kind of weighted model, I assume, how relevant the different files are. So Cursor does a great job of managing that context.

**Colin Matthews** (01:10:25)

The other applications, like these ones, don't do as good of a job of managing context. They start to fall apart when the project gets too big.

**Aakash Gupta** (01:10:38)

I think that was what the cursor team was bragging about was like their inference tricks around context window. So there you

**Colin Matthews** (01:10:45)

go. Yeah. Yeah. And there's lots of little like interesting things because they actually use, you know, there's lots of different ways AIs integrate in the cursor. So, you know, we have the composer here. You can also like, let's say generate a command down here. You can highlight text and edit in line with AI. And these all use, from what I understand, use different AI models or basically different models or different tricks with those models to try to get the best performance at the minimal cost. It's not like you're talking to the same model for all of these different UI elements. They're actually different models depending on what you're doing.

**Aakash Gupta** (01:11:19)

And before this, I think some people had the perception cursor you couldn't interact with via chat, but as we saw in the demo, you totally can.

**Colin Matthews** (01:11:27)

Yeah, other than getting the code running, which you saw me do through some commands that I knew how to do, you don't have to be technical. And even at that point, it's kind of tricky, but you can ask cursor to run the commands for you. So if I come down here, I'll just show you really quick while we're waiting. So if I cancel this command, and rather than me typing the command, I generate a command and say, run my app, it wrote the command for me. So

**Aakash Gupta** (01:11:56)

I don't even

**Colin Matthews** (01:11:56)

need to know how to run the command. I could just say, do whatever I want, run my app, and it'll do it for me. And the reason we're waiting for just context is Replit's trying to fix something. So I said add auth. It's trying to set up the database. And here's a good example. It says it created a PostgreSQL database, but we already had one. It seemed like it maybe have dropped my to-dos for some reason. Let's refresh here and see if this is still in here. Yeah, so deleted my to-dos items for some reason. I don't know why. And so on. So this is a good example of what I was saying before. the agent will just go and do things sometimes. And I have no idea why I deleted all my to-dos. And I actually deleted them from my database, which is kind of scary, because I don't have a backup of that to-do anyway.

**Colin Matthews** (01:12:47)

And so this is a good example of where sometimes more is more. Let's say addAuth is a fine prompt. But for whatever reason, we ended up dropping the to-do list items as part of that. But theoretically, we have authentication now. So let's go ahead and sign

**Aakash Gupta** (01:13:04)

up.

**Colin Matthews** (01:13:05)

We'll throw in.

**Aakash Gupta** (01:13:06)

That's still very fast to adding auth.

**Colin Matthews** (01:13:09)

Yeah. So we just, we logged in now as test, just whatever. And then we can log back out and then hopefully log back in. we go so uh yeah sorry about all the pop-ups here from google but uh everything's working fine with our our login there so yeah now we have a database we have authentication i mean i could publish this app and this is a functioning to do app now that

**Aakash Gupta** (01:13:32)

yeah that's what i was gonna ask how do i publish this now

**Colin Matthews** (01:13:35)

yeah

**Aakash Gupta** (01:13:35)

again

**Colin Matthews** (01:13:36)

pretty straightforward so we click deploy in the top right wow we have you know some scaling stuff so max number of machines basically tells us like If we have 10,000 users who connect at the same time, are we going to scale or not? And if we choose not to, our app's going to crash, but we're not going to spend more money. So most of the time, I'd pick one machine if I want to minimize my spend. And then approve and deploy. And then it deploys it for us, and we have a URL that we're going to have there. So I'll deploy this for now, actually. Why not? And then I'll just turn it off later. And again, this takes probably an extra two minutes to work through that. So while we're waiting on that deployment, I'll walk through my referral app just for fun. So this was built in Replit.

**Colin Matthews** (01:14:22)

It also has authentication, obviously. But basically what this is is as a student, I can come in here, sign up, and generate my own referral links. You get a unique code that is tied to your account. And then you can also track view statistics. So whenever someone visits your link, I'm tracking the views on your pages. And then you also get referral bonuses. And this is integrated directly with Stripe. So when someone buys a product through Maven, my Stripe account gets notified. And then I have a notification that goes from Stripe to this product to automatically track the purchases that are coming through. So the reason I did it this way is because the alternative was for me to somehow track coupon codes and who's buying what and which referral and how do I apply that to the student? And that would have probably taken me like an hour a day to just check, did anyone buy the product with a referral code?

**Colin Matthews** (01:15:16)

How do I apply that to them? I have to email them to let them know like, hey, someone bought with your referral code. This took me six hours to build and I never have to touch it. It's just all automated now. So one is it's a great little growth loop in a way that I wanted to add to my course. But two is now I don't spend any time on it. It's all automated.

**Aakash Gupta** (01:15:37)

Wow. Insane. That's the power of Repli. And where does v0 kind of fit into all of this and compare to the tools we've looked at?

**Colin Matthews** (01:15:46)

Yeah, I'd say v0 is very similar to like Bolt or Lovable. So again, you know, you throw in a prompt, so maybe we'll just do a simple one like make a to-do app. It's going to do, by default, client-side only. It can do server-side stuff. You can actually deploy with Vercel. Vercel is a kind of hosting company. So they offer running servers and stuff like that for you. So you can deploy with them. You can set up a custom domain, all the same stuff. You can't have a database. They don't offer databases. So you have to integrate with a third party. So very similar, like you might pick Supabase for your database there. But yeah, I mean, you can see it's basically Very, very similar. They have some cool features as well. Maybe we'll just pop this open in another tab, like a community here. So you can see there's a bunch of pre-built things we can start with.

**Colin Matthews** (01:16:38)

This login page, I just click Open in V0, and now I have this login page. And so you can kind of cobble together different pages or components based on the pre-built stuff that they have. And this is pretty unique to V0.

**Aakash Gupta** (01:16:52)

Colin, this has been an amazing whirlwind tour through these tools. I feel like my mind just exploded with seeing the potential and how quickly and how well you've mastered using them. Thank you so much. If people want to approach your level of mastery, what are you putting on and what are you working up and cooking up for them?

**Colin Matthews** (01:17:13)

Yeah, so well, first of all, there's the course on Maven, AI prototyping for PM. So if you want to get to a similar level of mastery, be able to produce things pretty quickly with not too many errors. You'll probably still have some, but that's OK. You'll be able to get through those. Then you can check that out. And then also, just on my LinkedIn and Substack, I post content pretty regularly on this topic as well. So if you're just looking for some quick tips, then you can check that out as well. It's a good place to look.

**Aakash Gupta** (01:17:38)

Amazing. This has to have been one of my favorite podcast episodes yet. Colin, thank you so much. Yeah, it was great being here. Thanks for having me. See you in the next episode.
