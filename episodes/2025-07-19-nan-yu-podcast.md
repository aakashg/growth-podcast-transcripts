---
title: "How Linear Built a $1.25B Unicorn with Just 2 PMs"
subtitle: "Linear's Head of Product Nan Yu goes deep on the Linear Method."
date: "2025-07-19"
host: "Aakash Gupta"
guests: ["Nan Yu"]
speaker_names: "substack"
substack_url: "https://www.news.aakashg.com/p/nan-yu-podcast"
youtube_url: "https://www.youtube.com/watch?v=e_T8Sn8s46M"
duration: "01:00:27"
word_count: 11359
source: "Substack episode transcript (aired audio)"
---

# How Linear Built a $1.25B Unicorn with Just 2 PMs

*Linear's Head of Product Nan Yu goes deep on the Linear Method.*

**Aakash Gupta** (00:00:00)

Linear just raised their Series C at a $1.25 billion valuation. Nan Yu is the head of product at Linear. OpenAI, Perplexity, Cursor. Why are all the AI companies using Linear?

**Nan Yu** (00:00:12)

When they were first getting started, the thing that mattered the absolute most of them, and still is today, is just speed of operations.

**Aakash Gupta** (00:00:18)

And Linear has always been built for speed. A lot of it comes down to how you guys build product, this Linear method. So how would you summarize, what's the 60 second pitch for what the Linear method is?

**Nan Yu** (00:00:29)

The core of the linear method is just directness. If you look at a lot of the practices that's very prevalent in the software industry, they're all strangely indirect, right? Like things like user stories where people kind of like tell, you know, they have this format and they say like, you know, the actor and the desired action, all this kind of stuff. They'd say it and it's just like, yeah, but like, what do you actually want me to do? Well, I want you to, you know, when you click a button, it sends an email. It's like, why didn't you just say that? I'm going to give you a quick demo of how AI agents work on linear. The whole thing should be done in less than five minutes. And then the first thing it's going to do is it's going to self-assign the linear issue. Agents are just like other users.

**Nan Yu** (00:00:59)

You can add mention them in comments. You can assign them to issues. You can add to the products, all this kind of stuff.

**Aakash Gupta** (00:01:03)

I think there's this tension people feel between speed and quality. To me, that's something

**Nan Yu** (00:01:10)

of a, it's almost like a false dichotomy. I think OKRs are a tool that makes sense in certain circumstances, but I think they're largely overused. A lot of times it's like, deliver this feature. That's their OKR. It's like, that's not an OKR. That's somebody shoehorning in the direct thing that they want to say. You don't want to be in this weird process of sprinting and being exhausted and sprinting and being exhausted again so that when new information comes, you're not ready to handle it.

**Aakash Gupta** (00:01:34)

really quickly i think a crazy stat is that more than 50 of you listening are not subscribed if you can subscribe on youtube follow on apple or spotify podcasts my commitment to you is that we'll continue to make this content better and better and now on to today's episode non welcome to the podcast

**Nan Yu** (00:01:55)

uh great to be here

**Aakash Gupta** (00:01:57)

One of the craziest things that I've seen in your guys' rise, and I have to admit, I've been following you since way before you were a unicorn, is how many of the AI companies are using you? OpenAI, perplexity, cursor. Why are all the AI companies using Linear?

**Nan Yu** (00:02:15)

I think, like, you know, when they were first getting started, the thing that mattered the absolute most to them, and still does today, is just speed of operations. And, you know, linear has always been built for speed. Speed in every sense of the word. You know, people kind of On the surface level, all the interactions are very quick, but they're also very direct. So whenever you're taking any kind of actions that have linear, things are very obvious in terms of what to do. You don't have to kind of sit there and figure the system out. You just kind of get in and out of it quickly and then get back to the thing that you're actually focused on, right? For them, it's actually building their companies.

**Aakash Gupta** (00:02:52)

I think that part of it also is that linear seems to be part of the new tool stack. Like the best new companies are using linear versus companies that were started like 10 years ago, there was a different tool stack in place. It seems like you guys are part of the new generation.

**Nan Yu** (00:03:10)

Yeah. I mean, I think that's, you know, that every, every so often, you know, you kind of, step back and take a look at your tooling and really like the values that people have in terms of how they want to get their work done and what they prioritize have, you know, kind of changed very dramatically. You know, something that we kind of really recognize is that people have been doing this software development thing for a while. If you think of the entire history of the discipline, it's still very young, but we're at a point where a lot of the core skills are kind of baked into the muscle memory of people's workflows. So we can build new tools assuming that baseline. People are not clueless anymore. They're ready to go. Everyone knows how to use Git. We're kind of ready to start from there as a starting point.

**Nan Yu** (00:04:02)

So I think linear comes with a lot of those assumptions baked in.

**Aakash Gupta** (00:04:07)

you had to summarize like linear's functionality how would you summarize that

**Nan Yu** (00:04:12)

um you know fundamentally we're a project management tool for uh software development teams um a lot of the primitives inside of linear uh you know are really optimized for that right like things like every single issue come with like a like a you know a preset branch name so you don't have to like stop in the middle of your process and make sure you're like following all the naming conventions and all that kind of stuff right so like a lot of those uh, little rough edges that people run into, you know, and are very accustomed to, honestly, like every day, we don't, we try to sand those off and kind of make the process even smoother for you.

<!-- sponsor -->
**Aakash Gupta** (00:04:44)

AI evals are one of the most important skills for PMs. And I know you know they matter. The question is, are you doing them right? Most teams are winging it with basic metrics and hoping for the best. Meanwhile, the teams that actually ship reliable AI, they've cracked the code on systematic evaluation. Today's episode is brought to you by the AI evals for engineers and PMs course, by Hamal Hussain and Shreya Shankar. This live Maven course will teach you the battle-tested frameworks from Hamal and Shreya, who are the engineers behind GitHub Copilot's evaluation system and 25-plus production AI implementations. Four weeks, live instruction, next cohort starts July 21st. Start shipping AI that actually works. Enroll at maven.com with my code ag-product-growth for over $800 off. That's ag-p-r-o-d-u-c-t-g-r-o-w-t-h. Today's episode is brought to you by Vanta. As a founder, you're moving fast toward product market fit, your next round, or your first big enterprise deal.

**Aakash Gupta** (00:05:52)

But with AI accelerating how quickly startups build and ship, security expectations are higher earlier than ever. Getting security and compliance right can unlock growth, or stall it if you wait too long. With deep integrations and automated workflows built for fast-moving teams, Vanta gets you audit-ready fast and keeps you secure with continuous monitoring as your models, infra, and customers evolve. Fast-scoring startups like LinkChain, Writer, and Cursor trusted Vanta to build a scalable foundation from the start. So go to Vanta.com slash Akash, that's V-A-N-T-A dot com slash A-A-K-A-S-H, to save $1,000 and join over 10,000 ambitious companies already scaling with Vanta. So it's a red ocean market, right? That's a space that we all have tried tons of tools in. But you guys are winning. And I think a lot of it comes down to how you guys build product, this linear method. So how would you summarize?

**Aakash Gupta** (00:06:52)

What's the 60-second pitch for what the linear method is?

**Nan Yu** (00:06:56)

Yeah. I think for us, the linear method is it's not just how we build products. It's how we help our users and our customers build products. So it's a little bit kind of self-referential and meant it that way. But the core of the linear method is just directness. If you look at a lot of the practices that have been very prevalent in the software industry, they're all strangely indirect. Right. Like things like user stories where people kind of like tell, you know, they have this format and they say like, you know, the actor and the desired action, all this kind of stuff. They'd say it and just like, yeah, but like, what do you actually want me to do? Well, I want you to, you know, when you click a button, it sends an email. It's like, why didn't you just say that? Well, you know, because all this other stuff.

**Nan Yu** (00:07:39)

And I think that that scaffolding that. you know, people, you know, have like traditionally done. It's been there because the business stakeholders didn't understand how software works or people just unfamiliar with how computers work and things like that. Like I said before, we are at a moment where like we can rebase, right? In a universe where everyone's online by default, like the internet is like the main place people hang out, like people know how computers work. So if that's the case, then what are the new assumptions that we get to make?

**Aakash Gupta** (00:08:09)

And you obviously aren't new to product either. You were a CTO at Everlane. You were a VP at Mode. What struck you as you've spent the last couple of years at Linear as different about how you guys build product?

**Nan Yu** (00:08:24)

I think if you look at the newer wave of companies, there is this desire to keep the company as small as possible. And I think that linear is definitely an example of that. The question we always ask is, okay, here's what we need to do. How few people can we hire in order to do this effectively? And I think that that's partly a function of the funding environment that we grew up in and the sort of new tools that are available to us. But I think the biggest difference that I've seen between previous eras that I've worked in and now is like no one brags about how big their company is anymore, right? It's like, it's kind of the opposite.

**Aakash Gupta** (00:09:16)

So I want to pull up the linear method website because a lot of people have actually pointed me to this website when I asked them, oh, how are you guys building things? And I say, we keep coming back to this website. It's this beautifully designed page, right? So if I go into these principles and practices here, can you talk us through these a little bit? How did you guys come to these principles and what do they mean to you?

**Nan Yu** (00:09:38)

Yeah, I think, you know, the overriding things that these principles try to get at is be really, really direct and be very fast, right? You know, when we talk about meaningful direction, being purpose-built, these are ways to directly solve people's problems. You're not building for yourself. You're building for somebody else. You're solving real problems for real people. And then creating momentum, right? It's like, how do you get to, you know, how do you maintain enough flexibility, but also keep enough of a pace to, you know, react to things that you learn in the wild, right? If your users hate a feature, if they really love something, you're gonna take that information and feed it back. And the only way to do it effectively is to you know have some kind of baseline velocity right have momentum so that you you know you're ready to to react to it but you don't want to be you know in this weird process of like sprinting and being exhausted and sprinting being exhausted again so that you know when new information comes you're not ready to handle it you're just like exhausted from the previous sprint and you're not ready to to go so like that's what we know we really try to uh you know try to try to embrace right be direct and also kind of keep uh keep the momentum going so that you know you're ready to react to the wild

**Aakash Gupta** (00:11:00)

I think there's this tension people feel between speed and quality. How do you guys negotiate that tension?

**Nan Yu** (00:11:11)

I think, to me, that's something of a... It's almost like a false dichotomy, right? Those are very overloaded words. And I think when people say that there's a trade-off between speed and quality, what they're really trying to say is they don't want people to... don't want people to cut corners right and they're like don't take shortcuts don't put in hacks don't do those kinds of things um but i think for for software especially if you have a high quality code base and you know really strong abstractions and good concepts in there uh you don't really feel a need to put in hacks and i and i i think that that's that's that's the sort of conundrum that you're dealing with. If you find yourself in a situation in which you're tempted to take these kinds of shortcuts, there's probably something wrong upstream about the quality of the software to begin with that kind of put you in that situation.

**Nan Yu** (00:12:05)

So what we try to do is kind of think through these things and not get ourselves into a point where we actually have that kind of temptation.

**Aakash Gupta** (00:12:14)

One of the most powerful principles I think you guys have here is say no to busy work. How do you implement that day to day?

**Nan Yu** (00:12:23)

I think, you know, a lot of busy work is a result of indecision and it's a result of like, like lack, like once again, like lack of clarity, lack of directness. So, you know, if you think about busy work, it's like, what do you want to do? Well, we're going to collect a bunch of data. We're going to run a bunch of AB tests. We're going to do all this stuff. And usually what that reflects is, um, There's some lack of clarity in the first place for, you know, what you were trying to do. Because, you know, like a lot of times if you think about what's the best way to understand the world is to like have some mental model of it and then act really aggressively in a way that's very falsifiable. If the world does not operate how you think, it will tell you very quickly and very loudly.

**Nan Yu** (00:13:16)

And if you were able to do that, then you don't have to waffle. You don't have to do a bunch of make work and do a bunch of analysis or whatever it is. You can just build the thing and then see how the world reacts. And if it reacts poorly, then you can change your mind. You've learned something.

**Aakash Gupta** (00:13:32)

One of the things that I heard listening to these principles and I think I had a misconception of prior to this interview was around roadmaps. What's your guys take on roadmaps?

**Nan Yu** (00:13:43)

I think, you know, roadmaps generally are useful tools, right? They're an expression of intent, right? And they help, like, align a lot of people who are, you know, who otherwise, you know, everyone's got their own idea of, you know, what the current consensus is and where we're going. So I think as a tool, you know, very useful. I think... you know, the one aspect of roadmaps is you kind of have to be ready to change the meta moments notice, right? Because it's an expression of intent and your intent is going to be completely a function of like what your latest information is and what your best information is. So if you get a bunch of new information and somehow your roadmap stays the same because that's I don't know, someone's idea of what ought to be. I think that that's where the problems start coming around, right?

**Nan Yu** (00:14:29)

Like you can't treat the roadmap as, you know, somehow it's blessed and it's sacred and you can't touch it. You know, you have to assume that it's just the reflection of your best knowledge at the moment.

**Aakash Gupta** (00:14:43)

What type of roadmaps are you creating then? Are you mainly focused on the short term, like this quarter or the next couple work cycles? How granular are you getting?

**Nan Yu** (00:14:54)

I think we plan for maybe three quarters out at all, and then with dramatically less certainty as it gets further out.

<!-- sponsor -->
**Aakash Gupta** (00:15:06)

Today's episode is brought to you by the AIPM certification on Maven. Run by Mikdad Jaffer, who is a product leader at OpenAI, this is not your typical course. It's eight weeks of live cohort-based learning with a leader at one of the top companies in tech. OpenAI just doesn't stop shipping. And this is your chance to learn how. Run along with product faculty and Mo Ali. The course has a 4.9 rating with 133 reviews. Former students come from companies like OpenAI, Shopify, Stripe, Google, and Meta. The best part? Your company can probably cover the cost. So if you want to get $500 off, use my code AAKASH25 and head to maven.com slash product dash faculty. That's M-A-V-E-N dot com slash P-R-O-D-U-C-T dash F-A-C-U-L-T-Y. Today's episode is brought to To help you out, I've put together a collection of courses I recommend at maven.com slash x slash Akash.

**Aakash Gupta** (00:16:24)

This includes courses like AI prototyping for PMs, product sense for PMs, and getting an AI PM certification. Visit it now at maven.com slash x slash A-A-K-A-S-H. And what does that planning process look like? Your average company, they're taking maybe like a month of time where everybody's all hands on decks on this large planning exercise. How do you guys run it internally?

**Nan Yu** (00:16:54)

I've always been puzzled by those very large planning exercises because it almost assumes that you're kind of starting from zero knowledge whenever that happens. And I think for us, we're constantly thinking of these things. So when we think about we have our hands on some stuff where we're developing it and we're really learning a lot and prototyping, putting stuff in front of customers, And then for the stuff that's further out, we have an idea of what our priorities are and we're doing whatever we can to learn more about those ideas and to sort of matriculate our thoughts around it, our point of view, our mental model of how the world works in relation to those ideas. And by the time that the next quarter rolls around and we're ready to kind of move on to the next set of things, we've already done a lot of the thinking and a lot of the planning.

**Nan Yu** (00:17:44)

I think if you put that off, until like the start of the quarter or the half or something like that, you're, you're really putting yourself at a disadvantage because like you can do all the intense research in the world, but like doing it even in a, in a, over a month, it's just, it's just not enough time to hit all of those things at the right amount of bandwidth.

**Aakash Gupta** (00:18:01)

Like an always on planning, sort of always on discovery process. Is there any particular rituals or ways of communicating your learnings in the always on process that you guys use?

**Nan Yu** (00:18:17)

So we have like a sort of, I guess you call it like a backlog, right? Of ideas that we've accepted. Like we think that this is a problem that's worth solving. And now it's up to us to develop some points of view, right? On how to solve this problem. So we have maybe like, I'm gonna guess like 30 or 40 of these areas where we're like, look, we have some, you know, develop point of view on this. It might not be fully mature. You know, we might not feel good about it yet. But if anything on that list comes up in a conversation with a customer, that generates a conversation with a product team, right? So if I'm, you know, like in customer success or sales or support or something like that, a customer asks about a thing and it's on that list, like their job is to escalate it into the product organization so that we can like dive deeper and try to learn something from it.

**Aakash Gupta** (00:19:13)

Makes sense. So one of the things people tend to do to operationalize these quarterly plans is build OKRs. What does you guys take on OKRs?

**Nan Yu** (00:19:25)

I think OKRs are a tool that makes sense in certain circumstances, but I think they're largely overused. And, you know, if you ask like OKR proponents, like, hey, who should use OKRs? They're going to say something like, oh, everybody. Every startup should do it. Every major company, every big company should do it. And I don't think that's the case. Right. And it gets back to this idea of like directness. OKRs are a very indirect way of aligning your team. Right. You can you look at it. I mean, like the the official issue to do is just look at a number and you're going to have this very huge error bar on trying to hit that number. It's supposed to be a stretch goal, all this kind of stuff. And and this this this is it's good if you have just like an absolute ton of different divisions and apartments and that kind of stuff.

**Nan Yu** (00:20:11)

And you're OK with like duplicate work and people stomping on each other because that's going to happen anyway. And you're like, look, at least they're aligned on pointing at this number and trying to achieve that kind of financial outcome, more or less, like for the company. And I think that when you're not at massive scale, that you can say things that are much, much more direct than that. And this shows up all the time. We interview a lot of customers and we ask them about their planning process. And we're like, hey, can you show us your OKR? It's like, what are your OKRs this quarter? And for dev teams, a lot of times it's like, deliver this feature. That's their OKR. It's like, that's not an OKR. That's somebody shoehorning in the direct thing that they want to say, which is just like, ship the product, ship the feature.

**Nan Yu** (00:20:53)

Here's the five features that really matter to our customers because we've been talking, our sales team's been talking to them, and it's just clearly obvious. So do it. And they can't contort themselves into making an OKR because that's the wrong tool to use at that level of granularity.

**Aakash Gupta** (00:21:10)

Is there... If you had to take the opposite side, when should teams use OKRs?

**Nan Yu** (00:21:17)

I think that there are certain very high level managers for which OKRs are. probably more appropriate where they are really, really responsible and they have a lot of budget in order to achieve a particular fiscal outcome. Whether that's like a growth team, where again, their goals are largely numeric to begin with, finance team, marketing, those kinds of teams. where it's, it's, it's inherently a very measurable, you know, kind of outcome to try to achieve in the first place. And that, you know, they, they have a lot of flexibility in terms of how to deploy their organization and their budget in order to achieve it. I think in those circumstances, you probably don't want to trickle it down as much as people typically do. They try to like trickle down all the way to like individual contributors. And it's just like, come on guys, like this one marketing analyst is not going to be able to affect anything.

**Nan Yu** (00:22:14)

They, again, They're okay, it's like, deliver these reports. It's like, That's just their job. You're just describing their job. Honestly, where OKRs lose a lot of credibility is when people try to shoehorn it like that, and then everyone's day-to-day experience is like, well, we're pretending here, guys. What are we even doing? So it's better to use them at the level of elevation for the right purposes, and then they're very useful, and not try to force it down everyone's throats and try to get it all the way, cascade it down to the most granular parts of your company.

**Aakash Gupta** (00:22:49)

Yeah, that really resonates with a recent conversation I had on the podcast with Anthony Maggio, who is VP of product at Airtable. And he talked about how he basically keeps the output metrics for like his senior directors who lead specific product areas because they actually have the capacity to impact that. But individual PMs, I think trying to shoehorn that in, that's when you really get into this performance play acting OKR symptom. Yeah.

**Nan Yu** (00:23:14)

Yeah. And it generates really weird outcomes, too, because if, you know, if a PM thinks that like they have to hit this OKR, this number, they're going to they don't have very much leeway to impact much outside of that. So they're just going to probably even overfit on that. Right. Maybe to the detriment of the the organization.

**Aakash Gupta** (00:23:30)

Exactly. Talk to me a little bit more about that. I think that OKRs can be a little bit the death of craft. Yeah.

**Nan Yu** (00:23:37)

Yeah. I think it's just, you know, it's, it's somebody deciding to, to kind of reset your incentives, right? They're coming in, they're dictating what your incentives are. And, Again, for some roles at some levels of elevation, that's a very natural fit. And it makes, you know, you were already thinking about your work along those lines, or you should have been. And I think for, you know, for the roles where it's, you know, how are you going to give a designer an OKR that really makes sense to them, right? They're trying to make something beautiful. They're trying to make something usable. And, you know, you could try to contort yourself and make some kind of usability metrics and that kind of stuff. But this is like, that's not... they're going to end up spending a lot of time not doing the thing that you hire them to do.

**Nan Yu** (00:24:24)

And I think that that's ultimately kind of the problem is that you take their incentives and you kind of pull it away from their core competencies into this very financialized, normalized kind of way to look at the world.

**Aakash Gupta** (00:24:38)

So what is the better way to set up incentives for IC designers and PMs? How do you guys give them goals to go after?

**Nan Yu** (00:24:47)

I think for, for us, for designers and PMs, right? Like the most important thing that we look for is have you established like a point of view and a story that makes sense to customers? And it's a, it's a very kind of like, you know, Boolean type of outcome. Like, is this like, is there a strong point of view here that's falsifiable, you know, from, from kind of like user response? And if you're able to do that, right, then we can, you know, we can get into, like, okay, are you able to generate, like, a wide variety of these things, you know, or, you know, can, you know, did we explore widely? Did we figure out, you know, how, like, what's our hit rate on this, right? Are, you know, are you consistently, you know, landing stuff? That's, that's fine, right? Those are, those are, like, the sort of, you know, in the long run, you kind of evaluate these things.

**Nan Yu** (00:25:38)

But, you know, Like in the sort of, you know, quarterly monthly kind of basis in terms of what you were thinking about it's, are we, are we pursuing a strong point of view about the world? Or if we're not, are we very clear about what information that we need to like go gather in order to establish that point of view? And then you're back at score one, which is like, okay, now how are you going to be like posture yourself in such a way that the world is going to tell you that very, very aggressively and very quickly.

**Aakash Gupta** (00:26:06)

So it sounds like you guys have a pretty high bar for what you build. It seems like you're trying to really encourage a lot of conviction around the user story for folks. Is it fair to say that you guys spend a lot of time making sure that things clear a high bar?

**Nan Yu** (00:26:24)

Yeah, we do. We have a lot of internal processes to help make sure that the quality level remains high so that we're kind of covering a lot of different angles when it comes to this. But importantly, we're leaving a lot of the... uh, you know, discretion to, uh, the, the contributors that are building the thing. So we have a process, uh, that we call roasts where, Hey, we have a feature. It's ready to go out. And we literally have the entire team sit down for like an hour and just like try to break it in every single way they can.

**Aakash Gupta** (00:26:56)

Right.

**Nan Yu** (00:26:56)

And, and kind of give feedback about like, you know, kind of bugs and technical issues, but also usability, you know, like opinions. Right. And it's like, and it always ends up generating like an absolutely enormous document of feedback from the team. No matter how small the feature is, no matter how well baked we think it is. And, you know, we don't expect them. We don't expect the team to address every single thing that's mentioned. Right. We expect them to sort of like read through it to. to help fill in their blind spots. Like, oh, I've never seen it that way. Okay, if I see it that way, then how should I think about this? Should we make this change? And then make kind of well-informed, balanced decisions based on that feedback, including one which is like, no, that's not our point of view. Our point of view is this other thing, so this is not a concern for us.

**Nan Yu** (00:27:43)

That's a perfectly fine response to a piece of feedback from me, from anyone at the company.

**Aakash Gupta** (00:27:51)

Have you ever taken a feature to 90% like that and decided not to launch it?

**Nan Yu** (00:27:57)

It usually doesn't get to that stage and it gets pulled back. We've definitely delayed stuff where I think we've uncovered a blocking issue that we've got to resolve first. What we actually try to do is kind of fail super early for those circumstances where you're like, look, the entire theory of this feature or this idea is wrong. We have a sort of incremental rollout system and the first increment is internal testing. where we produce the smallest version of the feature we can to just use internally in our day-to-day workflow. So by the time it hits the first beta customer or whatever, we've been using it for months. And so when things get really kind of U-turned or thwarted, it's during that first leg where things really get reconsidered.

**Aakash Gupta** (00:28:49)

Can you give us an example maybe of how you guys had like a grander vision, but then you built a smallest version that you could start testing internally pretty quickly?

**Nan Yu** (00:29:00)

Yeah, actually, let me let me think we had we've had like very recent examples of this. Oh, OK. Uh, so we, we, we have a feature that we're building right now, um, which, uh, you know, it was, it's designed to, you know, when you, when you dispatch an issue to an agent, um, you know, again, like the thing we talked about earlier, which is like, the responsibility of that dispatch is still on whoever assigned the agent, right? It's like, I can't be like, oh, I assigned it to Devin, and now it's Devin's problem, right? Like, Devin gets performance managed against this. No, no, no. It's like, I'm the engineer. This is still my responsibility, even though Devin's helping me out in building this. So that sort of initial model that we had about just assigning it to the agent user, that probably wasn't enough. It's more of like a collaboration or like a pairing kind of relationship.

**Nan Yu** (00:29:51)

So we're implementing the UI and the reporting, all that kind of stuff to understand like, okay, even though Devin worked on this, who were they pairing with that we can go to, to actually hold responsibility for the output. And the original vision for this was a lot bigger. The original vision for this was like, oh, man, we could dispatch this to like QA. And there's all these different roles that you can play. You can like you can like collaborate with, you know, pair program with other human engineers and designers and things like that. And we try to make a whole system work. And we realize that like, look, guys, let's solve a smaller problem. Let's just solve this like agents. Robots are not actually responsible for anything. So we have to like have a human on the end of it. Let's solve that problem. And then we can worry about these other kind of collaboration modes later.

**Aakash Gupta** (00:30:36)

So I think that's valuable to hear for people. Even you guys don't always get the initial scoping right. You started to go down the path a little bit of a bigger feature. But then you have that culture in place, going back to the linear method of thinking about, oh, what is the smallest feature? And so you guys kind of pulled yourselves back into, let's build this smaller solution to this smaller problem first. Love that. Now, what we've been describing here, this almost feels like a little bit of a long, drawn-out process, or it can, especially if you're from one of those cultures where sales is used to banging on the table, hey, we need this feature. Why is it here one month later? The CEO is knocking on your door six weeks later. How do you... How do you negotiate the pull towards, you know, move fast and break things that you're hearing from executives and Mark Zuckerberg and others to this approach of quality?

**Nan Yu** (00:31:33)

I think, you know, I don't know if, like, move fast and break things a little bit outdated at this point. I think even Facebook doesn't use that second bit. But I think, you know, moving fast is real, right? And I think, you know, one of the linear method concepts is, you know, keep momentum. And the way you keep momentum is you are constantly, you know, moving in a direction in a way that's like steady and that's like predictable. And a big part of that, right, is shrinking down the scope. So this, you know, the things that we talked about, about like, hey, look, if the scope was too big, like what's the smallest sub problem that you can solve? And if you are able to solve that sub problem really, really well, then you can always expand the scope afterward and you kind of incrementally, you know, expand the scope and, and, and kind of keep momentum as you, as you're doing it.

**Nan Yu** (00:32:23)

So that's, that's our, you know, it's like, honestly, it's our one weird trick, right? I'd like, I promise you it's not more complicated than that, which is just shrink the scope as aggressively as you can so that you can ship it quickly with high quality at the same time. And then as you, you know, understand more about the world, you can steer it in a way that's, you know, that's closer to what reality is telling you.

**Aakash Gupta** (00:32:47)

So I think we covered the essence of some of the key elements of the linear method. One we haven't quite talked about is build in public. How do you guys do that?

**Nan Yu** (00:32:56)

Yeah, we have a very consistent changelog that we put out into the world. And I think, you know, one of the things that we do to build in public that, you know, we've been doing since the beginning of the company's inception and it's really become a ritual for us is releasing a changelog every two to three weeks. And, you know, for us, it's like, it's a way to keep ourselves honest, right? If we ever come up with two a week and we're like, is there anything to put on changelog? Is there not? Okay, what did we do wrong? You know, it helps us be accountable to ourselves. Are we kind of consistently keeping our momentum? It's also a really great way looking back, right, to sort of see the story of how linear has evolved. And it kind of naturally produces this kind of documentation trail of how we got to the place that we got to.

**Nan Yu** (00:33:48)

Yeah. And every single time we have a change log out there, it's an artifact for our customers to share with each other. If there's a feature that they've been waiting for or that they find especially useful, it's a reference that's generally fairly small because every change log is incremental so that they don't have to send people to an enormous documentation repository or stuff like that. It's like, hey, look at this change log. It's what Linear just released. So it serves a lot of different purposes, and we found it to be very useful for those reasons.

**Aakash Gupta** (00:34:20)

What's your take on public roadmaps?

**Nan Yu** (00:34:24)

I think that they are, they are a little bit dangerous in a lot of circumstances. If you, you know, the thing we talk about roadmaps, which is like, look, you have to be ready for reality to tell you that your roadmap is wrong. And so when you put out a public roadmap, there's a lot of, there's a lot of kind of, it has an anchoring effect. Right. It's like, well, I put out this thing. I promise it to these people who are, you know, the people who are looking at your public ground up are probably going to be like your loudest customers. They're not necessarily your most important ones or the ones that you should be listening to the most, but they're going to be very loud. And so it just ends up being like a lot of social pressure to kind of like stick to it.

**Nan Yu** (00:35:06)

And, you know, it's it kind of. makes the incentives a little bit, uh, like a little bit messed up and in that way. So if you're, you know, if you're gonna make a public roadmap and you, you have a posture that you're ready to kind of like change it at a moment's notice, then, you know, that's, uh, you know, feel free to do so. Or if you're, you know, if you actually have a lot of certainty for what your roadmap is going to be because it's a bunch of table stakes features or something like that that you know you're going to have to do, I think that's an okay situation to be in as well. There's a lot of different, like, shades of gray for this, too. You know, like our sales team, for example, with our most important customers, they share, you know, like, some parts of our roadmap to make sure that like we're aligned with how they're trying to deploy linear at their companies and how they want to grow so there's a bit of that you know give and take but sort of like a full public roadmap that's like on the internet and open to everybody is uh it's you have to be a little bit careful because it could really screw up your incentives

**Aakash Gupta** (00:35:59)

And as a head of product, I know I was often called into those sales calls to talk to the roadmap, to preview it, especially with those big accounts or with big existing customers or churn risk customers. How do you handle those conversations?

**Nan Yu** (00:36:14)

I think, you know, with a lot of what's the what's the word with a lot of care. Right. And it's. For those very, very specific moments, a lot of it is trying to understand what it is that the counterparty wants to know. No customer has ever churned because of the lack of a single feature. That's never happened. I know it can seem in those circumstances that they're banging their fist on the table and this is the thing that's going to make her make the deal, but it's extremely rare that that's the case. And usually there's some underlying goal that the stakeholder is trying to accomplish or their company is trying to accomplish or something like that. And as long as you help them in every way that you can, partly it's about the roadmap, partly it's about educating them on how to best use the product or how to use a different product in conjunction with yours or something like that.

**Nan Yu** (00:37:04)

There's a lot of customer success kind of stuff that you need to do in those moments. And it typically turns out pretty okay.

**Aakash Gupta** (00:37:12)

That's how I like to approach it as well. It's like more trying to get into understanding, almost asking a lot of questions, even as a product leader, even if they've already told the sales leader again in the conversation with you so that you can go a little bit deeper then and figure out like, what is the problems you want to solve? I can share, you know, our thinking on how we're going to be solving those in the future, but try to avoid getting really specific with the public roadmap. Yes. This quarter, we're going to be shipping these features. Next quarter, we're going to ship whatever else. Yeah.

**Nan Yu** (00:37:42)

Yeah, totally. I think asking if you ask our salespeople, they're like, what does not do in these calls? And they're like, he asked a lot of questions. That's what they'll say to you. Right. And then, and I think, I think that's, that's, that's true. Right. Like, it's like, it's ultimately, I mean, ultimately, they really do want to be heard. They're like human beings too. And you know, for, for us, like the people on the other end of it are in roles similar to ours. Right. They're like, you know, product leaders, VP of engineering, that kind of role. And they want to be heard. They want to know that they're understood. And so sometimes that's all you're there to do is to make sure that they know that you know what they're feeling.

**Aakash Gupta** (00:38:18)

So that's the linear method, at least as I see it as a lot of the core essence. Now I want to talk about how that linear method is applied to building AI features. maybe walk us through this AI agents launch. You know, I want to hear the stage gate processes. I want to see how you guys shaped it for craft and quality over time.

**Nan Yu** (00:38:40)

Yeah. I, so, you know, one of the things that we talked about with the linear method, right. Is clarity establishing a very strong point of view, right. And, and, and kind of being in shipping small increments. So the first version of our agent platform is, There's a very clear concept. Agents are just like other users. You can do anything with them. You can mention them in comments. You can add them to your teams. You can assign them to issues. You can add them to projects, all this kind of stuff. They just have a user account. And we're going to go from there. And then the world is going to tell us if that is the right model because nobody knows. Right. Like agents are a new species of artificial intelligence that exists. And like no one truly knows. Right. How you know what the long term is going to look like.

**Nan Yu** (00:39:21)

So we started with that. And, you know, and for us, that was that was that was a very clear spec. It's a very small spec. Right. Because all of the actions that humans can do inside the system are already established. So it's very clear. um and uh and we learned a lot immediately right we you know quickly learned about this responsibility thing that robots are not responsible for anything so you have to you have to put a human on the other end of it uh we quickly learned that they're very chatty so if you you know if you just use comments they're gonna throw a lot of comments into the world and it might be a little bit overwhelming so you might have to give them their own space to be chatty and then only have the comments be like the super important stuff that they say And also just even the, but then also they have these abilities that humans don't have.

**Nan Yu** (00:40:09)

They're able to kind of like look at your entire workspace and see every single issue all at once, right? No person can do that in like less than like, you know, instantaneously like agents can. So, you know, giving them that visibility helps them have the right context, right, to do their work. So like we learned these things Because these are the emergent kind of concerns and problems that we ran headfirst into. But that's the goal, right? We had a very strong point of view. Agents act exactly like humans. We put that out into the world. And we discovered that there were some inadequacies with that point of view. And we discovered them fast. And now we're addressing them quickly.

**Aakash Gupta** (00:40:49)

And when you created, I guess, that initial vision, like we're going to be working on AI agents, how did you build up the conviction that we were talking about earlier that this is a problem to be solved or this is an area we're going to be working in?

**Nan Yu** (00:41:04)

Yeah, the kernel of the idea came when we saw people starting to juggle multiple agents simultaneously. Because, again, unlike previous modes of computing, AI can take human clock-level time to do their work. It can take several minutes. It can take hours even. And that's like a new problem that like emerged. And, you know, all of a sudden the work with the computer becomes like very, very async. And, you know, we kind of looked at linear like, look, linear is the place where you're managing distributed async work. So we think there's a very good fit here. So that was the sort of original kernel of it. If people were just kind of using, you know, kind of like IDE based, you know, kind of live interaction type things in a single threaded way, I think there wouldn't be a fit here. But because, you know, like people are really, really starting to run like background jobs and things like that, like we're like, okay, there's probably something, you know, that's something that's a very close fit.

**Nan Yu** (00:42:01)

And also, you know, because people work in teams, they don't work necessarily in silos all the time, then like linear will be a great place to try to, you know, to try to be like the clearinghouse for this kind of information.

**Aakash Gupta** (00:42:13)

Okay, so I'm trying to contrast what I hear here with you guys not necessarily pursuing a lot of the flashy AI features before. And what I think is the difference then, like why you guys don't have, you know, a talk to me linear chat bot like every other company, but you do have the AI agent is you saw this happening naturally within users' workflows already, but you saw that there were some problematic elements of how that workflow was built. happening so you saw opportunity for you to solve that problem is that a fair encapsulation

**Nan Yu** (00:42:46)

yeah i think that that's uh that's fair and that that's very typical for us right like a lot of our features have you know are really evolutions of of internal tools that we see people building out in the wild right you're a large company you build this nice little tool for your team to use and we're like okay that that seems useful and then we can help you like you know actually make a productionized you know full-blown version of it

**Aakash Gupta** (00:43:08)

okay so the takeaway from how linear is approaching ai features versus your average company right is really focus on not what's flashy out there whatever the latest ai trend is but instead focus on what are a lot of my users doing on top of the product that might have some problematic workflows within it

**Nan Yu** (00:43:30)

yeah a big part of it is that you know the I think our core mantra for the linear method and for ourselves is really to solve real problems for real people. And there are so many real problems out there, so many that are emergent, so many that are existing, that we have plenty of space to cover. Rather than trying to do the thing that's the loudest possible feature, we're hopefully trying to make the most useful thing.

**Aakash Gupta** (00:44:02)

Love it. And I think there's a lot of lessons there for people. So go check it out. See how linear is not just like jumping on every feature bandwagon, right? Which I think that the average SaaS company is. And I think that goes to one of the things that people really love about linear, which is it's not bloated. Are there any like other key disciplines or takeaways people should take so that they can avoid feature bloat?

**Nan Yu** (00:44:31)

Yeah, I mean, there's the classic thing, which is take your users very seriously, but don't take them literally. And especially with a very wide product surface like Linear has, you know, people are gonna ask, you know, every single feature you could possibly think of somebody has asked for before. And a lot of the response really needs to be like trying to understand like what the user's goals are, what they're trying to accomplish, you know, what kind of frustrations they're having. And and how that overlaps with what you're hearing from other from other customers. And then once you understand that, then you can like, you know, begin to approach the problem space with, you know, with with some kind of solution exploration. You know, like a lot of times candidates and, you know, and, you know, people like ask us about like, Hey, you know, all these startups try to compete with like Atlassian and Jira and like, you know, they, they, they all, they all kind of become very similar to them.

**Nan Yu** (00:45:23)

Like, how do you, how are you going to prevent yourselves from doing that? And, uh, and I think the, um, the answer is like, you know, the way that, um, These incumbent companies, not just Atlassian, but a lot of incumbent software got to the way it is because they took their users very literally. They said yes to a lot of requests. And that might have even been the right thing to do in that era because all this stuff was new. They didn't have a better way to think about it. It's like, sure, are you just asking for it? Let's do it. But now we're kind of taking a second pass at this. We have the benefit of knowing that history and knowing what outcomes that leads to to try to avoid and try to think about things a little bit more critically.

**Aakash Gupta** (00:46:08)

I want to shift gears a little bit and talk about you. So I think a lot of people would want a job like head of product at a unicorn, let alone like at the unicorn that all the top new companies are using. What's the story of landing the job?

**Nan Yu** (00:46:30)

Um, you know, linear linear has a, uh, a work trial based, uh, interview, uh, system, right. Where, you know, every candidate comes in and they, they work with a team for some period of time. Um, and like for me, I, you know, kind of consulted with the company on, on a, on a sort of new feature set that they were, um, kind of exploring. I think, you know, I ended up working with the company for a pretty long time, like maybe like six weeks or something like that on this thing and working with the team. And it was enough of a positive experience on everyone's front where they made me an offer and decided to bring me on board. You know, it's very fortunate for me. But I think that, you know, that's a specific instance, you know, for us. But I think generally speaking, you know, for...

**Nan Yu** (00:47:19)

We are a fully remote company and there are very specific qualities that, you know, we look for that, you know, other companies might not, but just like very good async communication, like extreme clarity, like obviously like bias towards action, all that kind of stuff. But it's like, everyone says those things, but it's like, it's like doubly important when you're fully remote. So that's, I don't know, that's the kind of backstory.

**Aakash Gupta** (00:47:45)

So it sounds like you didn't have a full-time job at the time you did the work trial, right? How do people navigate that when they do have a full-time job? Uh,

**Nan Yu** (00:47:55)

you know, we, it's paid. So, you know, basically we're, we're trying, we're buying some of your PTO. That's the best way to think about it. Is that like, look, if you're willing to sell us some of your PTO, like then, you know, we can, we can do this work trial thing, but we're also very flexible. We understand people have different circumstances. So if they need to like, you know, kind of straddle a weekend to get a couple of days in there and stuff like that, we're, we're very open to, you know, making it work.

**Aakash Gupta** (00:48:16)

Okay. And how did the initial, like the very first process where you get in touch, I might be mispronouncing your CEO's name, Kari, but get in touch with him. Right. And like even clear the stage that he wants to do a work trial with you. How did it happen for you?

**Nan Yu** (00:48:35)

Um, it was, you know, it was actually a very long story. Like the, the, my first contact with Kari and the team was, was, uh, years ago, um, when they were kind of developing the very first version of the product. And I was, uh, you know, running an engineering team at a company called abstract, uh, and they, they were interviewing, you know, startups, right. And I was one of their, uh, uh

**Aakash Gupta** (00:48:56)

you know they're

**Nan Yu** (00:48:56)

interviewees so to speak right like you know i told them all about like processes and i had like strong opinions about this stuff so that was probably the first touch point i had with them um and then uh you know i kept in touch and you know when they uh you know when it's you know there's a little bit of luck involved certainly right they were like hey we were they were looking to explore their first analytics product uh, you know, to help people measure like what's going on in the, uh, in their workspaces. Um, and I had just, you know, done a stint as VP of engineering, as a VP of product at, uh, uh, a BI company, uh, called mode. So, you know, I had very relevant experience for that, uh, that kind of problem.

**Aakash Gupta** (00:49:33)

Yep. Okay. So the takeaways from your story, like keep in touch with people and make yourself available for that work trial if you need to. And then for somebody else, like somebody wants to become a PM on linear work under you, what would be your advice to them?

**Nan Yu** (00:49:50)

Um, I mean, we, we have a job rec open right now. So my job, my, my advice would be to apply for the job first. Um, but I think, you know, ultimately we are, um, We're looking for someone who can bring a lot of clarity and a lot of initiative to the organization. For us, PMs are the... they, they, they sort of do the most amount of work at the beginning and the end of the process, right? It's like the startup energy it takes to sort of like figure out the problem space and like get that initial exploration in place. And then when you're close to the finish line to kind of like make sure that everything kind of comes together and, uh, and we're really, really clear about how we're going to go to market for things. So those are, those are the kinds of qualities that we're, we're really looking for.

**Nan Yu** (00:50:39)

Um, and, uh, Definitely go to the job site and apply for the position.

**Aakash Gupta** (00:50:48)

What is the right way to prepare yourself so that you do well in the work trial?

**Nan Yu** (00:50:58)

I, you know, I, I, I think there's not, there's not any, there's not one thing, but if there's one piece of advice I can give people for honestly, for any interview process, but especially ours is you got to put your ego away. I think a lot of times PMs are, you know, we were, we're so used to like doing a bunch of research and like being right about things and having a reputation and things like that. It's just like, look, you're, you're in a, you're in a process where people are trying to evaluate. It's a very difficult thing, right? Most PM interviews are extremely, you know, kind of messy, you know, sort of evaluation processes. You really do need to put yourself out there and like have a lot of like, just be exposed because people need to know what they're getting into. Like a lot of the PM evaluations right here are just like, I need to know what I'm getting involved with.

**Nan Yu** (00:51:50)

And if you, if you, you know, if you have, if you're putting up protective screens and, and, and not really kind of like showing who you really are, then people can kind of see that. And then it just becomes like, well, I don't have enough information to make a, make a hiring choice here.

**Aakash Gupta** (00:52:05)

So kind of being willing to be yourself then.

**Nan Yu** (00:52:08)

Yeah, although Be Yourself sounds so mundane, right? It's not really that. It's just like, don't worry about being wrong. The worst case scenario is you don't get hired, which is like, that's fine, right? No one has 100% hit rate on applying for jobs. So it's just like, we count wins, we don't count losses.

**Aakash Gupta** (00:52:29)

Makes sense. And how do you organize your PM team?

**Nan Yu** (00:52:34)

So our opinion is very small right now, but I think one of the sort of more distinctive features of it is that we have product management and product marketing all reporting into the same structure. I'm a big believer in that those are almost the same role. They have slightly different responsibilities, but they ought to be a lot closer. Product marketing is much more closely related to product than it is to the normal marketing things like demand gen and performance marketing and things like that.

**Aakash Gupta** (00:53:03)

Okay, how many

**Nan Yu** (00:53:04)

PMs do you guys have right now? Right now we have one. Two including me, but one in addition to me and one product marketer. We have another product marketer coming on board next year, and we have effectively two PM roles open right now.

**Aakash Gupta** (00:53:18)

Okay, and how big is the engineering team?

**Nan Yu** (00:53:22)

Gosh, I don't know for certain. It must be around 40 at this point.

**Aakash Gupta** (00:53:27)

Wow, so you guys made it to unicorn status with 40 engineers and two PMs. That's pretty efficient, that's amazing. Thanks. We try. So, like we said, you were CTO at Everlane. Why are Everlane clothes so expensive?

**Nan Yu** (00:53:53)

You know, it's funny, like, I think depending on your point of view, they could be very cheap. Everlane is a, certainly when I was there, it was a cost plus business. And the game was really just to, you know, you have a materials cost and you're delivering that as much value as you can in the materials to your customers with a, you know, kind of standard retail markup. And I think that that's completely a function of the quality of materials that were chosen at any given moment in terms of how expensive the clothing actually is. Importantly, it's not a lifestyle-driven or image-driven business. So if you compare it to something like, I don't know, like Coach or Berber or something like that, it doesn't have those kinds of margins. It has very, very reasonable margins. So if something seems expensive, hopefully that's because the materials that are being delivered have a lot of value.

**Aakash Gupta** (00:54:46)

Okay, so it's really you guys are just doing that cost plus method, but actually you're mostly reinvesting that price that somebody's paying into quality material.

**Nan Yu** (00:54:56)

Yeah, yeah, exactly. I think certainly when I was there at Everlane, like 70 to 80% of the cost of goods was purely materials. It wasn't cut and sew or labor or shipping or any of that kind of stuff. That was the other 30 to 20%.

**Aakash Gupta** (00:55:10)

What was the shift like from going to basically a cost plus lower margin apparel business into these companies like mode and linear, very product focused, totally different margin businesses.

**Nan Yu** (00:55:23)

Yeah, I mean, it's obviously it's like this kind of B2C retail, you know, kind of scenario to, you know, kind of a product led, but like, you know, obviously ultimately B2B and in some ways like enterprise business. I think on that front, there was a lot of learning, especially at Mode. Like I, you know, kind of learned to deal with sales teams, you know, in a really big way to kind of do all the kinds of like questioning and pushback that we talked about. And when you get sat in front of a customer and they're kind of like grilling you. So I think that part of it was really big shift. However, I'll say that, you know, a big advantage I had going into it was on the storytelling aspect. Like if you think about selling commodity goods in a kind of cost-plus way, the only differentiation you have is on brand.

**Nan Yu** (00:56:10)

And and on the story that users tell themselves in their heads. And, you know, something I discovered was that, like, I kind of naturally came equipped with that muscle in a way that a lot of the sort of B2B PMs around me, like, just had no familiarity with.

**Aakash Gupta** (00:56:27)

I made that shift a couple times. Yeah. B2C, B2B back again. I feel like some of the specifics, like you said, like there are specific skills, whether it's working with sales or working with customer success or dealing with enterprise clients that are specific skills. But a lot of the essence of it, of product management is still the same.

**Nan Yu** (00:56:47)

Oh, yeah, totally. And like Everlane, like I did a lot of the sort of B2B shaped things. Like we built a lot of tools for our merchants. And, you know, you dig in and you're taking requirements from like power users. You're like learning about their workflows and their business and things like that. A lot of that stuff is very, very overlapped. Ultimately, you're trying to produce some kind of theory of mind for your customers, like why they're making buying decisions, why they're coming to you in the first place versus competitors. So yeah, a lot of that stuff has a lot of overlap.

**Aakash Gupta** (00:57:22)

So you were able to successfully make the shift. I work with a lot of PMs who are job searching, and it feels like everybody right now is just getting pigeonholed into a particular industry. If they were in B2C apparel or even the more B2B-flavored aspects like you're working on, they still end up just being stuck in apparel. Or if they were in B2B SaaS, they're just stuck in B2B SaaS. Can today's PM really shift industries? And if so, how?

**Nan Yu** (00:57:49)

Yeah, I can tell you my story and I don't know how widely applicable it is, right? Like the way I shifted, because I did my stint at Everlane and I had to use so many SaaS tools in that process. I'm like, I'm really interested in this area. I wanna build tools for pro users. How am I gonna do it? And the way I did it was I took an IC engineering job at a B2B SaaS company. And I'm like, look, I'm good enough at this stuff where it's a smallish company. I'll get in the door here and I'll just be, I'll work my way into the right, into the right position. So that was, that was my, you know, sort of like get your foot in the door. And then especially if you're at a startup, like people will quickly recognize your ability to contribute in whatever way is, you know, best suited for the org.

**Nan Yu** (00:58:38)

Right. It's like, I know that getting hired is hard because everyone wants like the perfect candidate. But just just get hired. And then, you know, like if that experiment, you're working at a company, an engineer on your team shows a lot of, you know, kind of ability to think through product and is really good at it. Are you going to stop them from doing that? Like, no, you're not. You're gonna be like, no, do that more. Right. Like, like,

**Aakash Gupta** (00:58:59)

that's

**Nan Yu** (00:58:59)

great. So, like, put yourself in that position. Right. So if you think you got the chops, just get in the door and then you'll you'll figure it out.

**Aakash Gupta** (00:59:06)

I love that. So it sounds like, though, then you're you're probably taking at least, well, we know a level hit because you went from CTO to IC engineer, but potentially even a compensation hit. So you might need to be able to take that in order to make the long term move that you want.

**Nan Yu** (00:59:21)

Yeah, I mean, I think that's, you know, there are obviously a thousand different ways to do this kind of pivot. This is what happened to work for me. Yeah, I did take a level hit. I took a compensation hit, but it also was something where I feel like it was very explainable on my resume. You know, I'm like, hey, I did a CTO thing for like a while and I wanted to like, you know, chill for a second and take an IC role for a year or so. Like, that's a very explainable sentence, right? Like people, everyone will nod their head and be like, yeah, I get that. Okay,

**Aakash Gupta** (00:59:50)

all right. Well, non, I think we could keep going for another hour or two. Um, but I know you as a head of product are very busy. So thank you so much for being on the podcast.

**Nan Yu** (01:00:02)

Yeah. Appreciate it. It was a lot of fun.

**Aakash Gupta** (01:00:04)

If you guys enjoyed this conversation, you will love our YouTube video breakdown of linear AI agents, which Nan talked a little bit about when he was talking about downscoping a feature. And you will love the newsletter issue where I go further into some of the principles with Nan and we talk about in some more detail how they make products at Linear.
