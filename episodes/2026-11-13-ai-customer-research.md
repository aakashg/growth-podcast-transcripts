---
title: "How to Build an AI Customer Research Agent in Claude Code"
subtitle: "A practical tutorial, with the full kit to build your own."
date: "2026-11-13"
host: "Aakash Gupta"
guests: ["Greg Greiner"]
speaker_names: "substack"
substack_url: "https://www.news.aakashg.com/p/ai-customer-research"
youtube_url: "https://www.youtube.com/watch?v=JpyhPePe150"
duration: "00:58:53"
word_count: 9503
source: "Substack episode transcript (aired audio)"
---

# How to Build an AI Customer Research Agent in Claude Code

*A practical tutorial, with the full kit to build your own.*

**Greg Greiner** (00:00:00)

So back when I was a CPO at Bolt, I would have been

**Aakash Gupta** (00:00:02)

happy to talk to seven or eight customers a month.

**Greg Greiner** (00:00:05)

And now with AI, you have the opportunity to thousand X or even more how many customers you're able to engage with on a regular basis.

**Aakash Gupta** (00:00:12)

Meet Greg Greiner, former CPO at Bolt. And head of product at Uber for Business, now CEO at AI company Wolf.

**Greg Greiner** (00:00:19)

In the modern world, you should be using AI to create a scaled representation of yourself to talk to your customers for you. You should also come back with what it's learned and share insights with you on a regular basis. As PMs, we really need to get close to customers and this is how we do it. Essentially, it's scaled research with AI.

**Aakash Gupta** (00:00:35)

How has AI changed what VMs need to be able to do?

**Greg Greiner** (00:00:38)

I think it's now possible to actually have real back and forth conversations with thousands or even hundreds of thousands of customers every month in a way that would previously require an army of researchers, an army of support reps.

<!-- sponsor -->
**Aakash Gupta** (00:00:52)

You cooked it up in just 30 minutes. This is something I haven't seen somebody build before. What is the groundedness? What is the true data source? Before we get into today's show, please take a second to check that you're subscribed on YouTube and following on Apple and Spotify podcasts. If you want access to all of my favorite AI tools, I've gotten them to give you an entire year of their paid plans. Check out bundle.akashg.com for an entire year of Bolt.new, Airtable, Speechify, Descript, Magic Patterns, Linear, Dovetail, Arise, and Mobbin. And now, into today's show. Engineering is getting faster with AI. Is product management really getting faster? One of the ways I would argue it is, is by helping you talk to more and more of your customers. Now, of course, you've been using Claude to help you synthesize transcripts, but have you been using it to drive automated, proactive research with every single one of your customers?

<!-- sponsor -->
**Aakash Gupta** (00:02:04)

How might you actually do so? If you really want to get to that next level of customer research with AI, today's episode is for you. Greg, welcome to the podcast.

**Greg Greiner** (00:02:16)

Thanks for having me.

**Aakash Gupta** (00:02:18)

Greg, you told me something pretty interesting. When you were Chief Product Officer of Bolt, you would be happy to talk to five to ten customers a month. That has really changed with AI. What is... This new level of AI research report that you can build.

**Greg Greiner** (00:02:38)

Yeah, I think it's now possible to actually have real back and forth conversations with thousands or even hundreds of thousands of customers every month. In a way that would previously require an army of researchers, an army of support reps to facilitate all of those conversations. And when you are able to have all of those conversations at scale, you're able to produce really interesting insights. This is an example for the company Ancestry.com of what one of these reports might look like if you're able to have these skilled conversations with customers. One of the first things that we always report on is obviously the impact in the customer journey from a business metric standpoint. We found that having this type of personal conversation with customers doesn't only capture insight, but it also allows you to convert a broader set of this audience. In this case, this is people who've abandoned the process of purchasing a DNA kit with Ancestry.com.

**Greg Greiner** (00:03:39)

And so beyond that conversion insight, you're also learning for these people who specifically dropped off in that funnel, what are their biggest concerns? What are they bringing up most frequently? What is actually driving them to abandon? And then in addition to that, when you layer on the conversion data about what people actually do after these conversations, whether they've finished their purchase or not, you can double click a layer deeper into what are the relative conversion rates of these buckets. So not only like how often are they specifically happening, but when they do happen, how do these people behave and how does that compare against the baseline of all the people who engage in conversations? And so you can sort of see whether something is an issue or a hesitation or a concern that is easily addressed with just messaging, right? The AI responding back to the customer and sharing, specifically answering the question around shipping and delivery time.

**Greg Greiner** (00:04:41)

That's something where this can really just be solved by updating your messaging, maybe more proactively talking about shipping and delivery time versus something like subscription confusion that even when the AI has the chance to respond to the customer and address that concern, these people are still not converting at a high clip. And so that opens up a broader opportunity for you to dive into that problem and try and address it in a more holistic way with your product.

**Aakash Gupta** (00:05:05)

Fascinating. So these conversation counts are so super high. How are these conversations generated?

**Greg Greiner** (00:05:12)

So these conversations happen, you know, when someone drops off in that flow after they've entered their email address, let's say, or their phone number, the AI is reaching out over that channel. And we're getting a large percentage of those people to respond and actually engage in a back and forth conversation. And so that's where we get to the scale of we have customers doing tens of thousands of these conversations, hundreds of thousands of these conversations every month and generating this more scaled insight into the specific audience at the specific point in the journey.

**Aakash Gupta** (00:05:46)

So is this basically like the evolution of in-app surveys plus AI?

**Greg Greiner** (00:05:52)

Yeah, I think that's a good interpretation. And I think what this allows is not just the survey from the insight perspective, but you can dive a layer deeper. When someone says, oh, I'm concerned about this example on the left here. An unexpected relative popping up and that being awkward, you get the chance to not just take that in as a piece of data, but you get to double click on it and ask follow-up questions, attempt to resolve those concerns and see how the customer reacts to that, which gives you a much richer sense of how these different things are actually impacting your customers more directly.

**Aakash Gupta** (00:06:32)

Awesome. So how do I build this?

**Greg Greiner** (00:06:34)

Yeah, so I think for a lot of people, it's not gonna make sense to buy a dedicated product like Woven to accomplish this outreach. And so the awesome thing is that with existing tools, you can build something very similar to this using something like Cloud Code. And so in about 30 minutes before the podcast, I put together a quick example of this.

**Aakash Gupta** (00:07:00)

Most roadmaps are out of date after the quarterly review. A PM spends a week rebuilding it in slides, leadership looks at it once, and two weeks later, half of it is moved, while the deck stays in someone's inbox Still saying the old thing. The other half of the problem shows up when an idea gets committed. The customer insights and the reasoning for picking it live in one place, the tickets engineering works from live in JIRA, and the only thing connecting them is a PM copying an idea. I've been using Jira Product Discovery for both of these. And each one takes about a minute, so let me just show you. This is my discovery project. Every idea has the insights behind it attached. Things like customer quotes, support tickets and usage data, along with the fields my team uses to prioritize. To share it with leadership I publish it.

**Aakash Gupta** (00:07:48)

They get a link to a read -only version. They don't need a license to open it And they only see the fields I choose to show And because the link is live When priorities shift or So that's the living roadmap. The second piece is connecting discovery to delivery. Say this idea is committed for next quarter. I open it, go to the delivery tab, and create the delivery ticket from right here. It lands as an epic in the engineering team's JIRA project.

**Greg Greiner** (00:08:20)

Already linked back to the idea it came from. As engineering moves that work through

**Aakash Gupta** (00:08:25)

their sprints, this

**Greg Greiner** (00:08:26)

progress

**Aakash Gupta** (00:08:26)

bar fills in. Add the delivery progress field to the roadmap view, and the link leadership already has shows where each item actually stands. So nobody has to ping me or set up a status meeting to find out. That closes the loop. The reasoning stays with the idea, the roadmap is a live view of it, and the work engineering ships stays tied to why it got built in the first place.

**Greg Greiner** (00:08:48)

If your team already runs Discovery in Jira, be sure to try out Jira Product Discovery. Link is in the show notes. It takes in a source of customer data. So for the demo, it's just a list of customers on a CSV, right? So people, their drop-off points, you know, this is for people who've dropped off in a trial, data about their usage, et cetera, that allows the AI to personalize the outreach and the conversation. You can also use any form of CDP or a data warehouse like Snowflake or Segment to power this. And then it has some basic instructions on how to approach the conversation, how to format the email in the cloud.md file. So this is all relatively straightforward stuff, but it's important to ensure that you're still making this feel personal. It still feels like an email that you would draft back to the customer directly.

**Greg Greiner** (00:09:42)

And then I filled in some basic stuff. This is for a made up company called Cadence that does AI fitness training. And so some information about different escalation processes, different policies that the company has around things that the agent can do or not do. And then the specific programs. But for a lot of companies, this data already exists. And so you already have pretty rich markdown files about your company that you can point the agent at. And even if you don't, you can use Claude pretty easily, point it at your website, and it'll generate a bunch of this stuff on the fly. And so it uses all that information to personalize outreach to this customer audience. And so I will... Trigger that really quick in my Claude session. So there's a skill that just does the outreach sending, but you can also either schedule this or have it trigger based on new entries entering this CSV or from the database.

**Greg Greiner** (00:10:42)

What it's doing behind the scenes when it does this outreach is it's going through that list of customers. It's identifying the ones it hasn't reached out to yet. It's taking that metadata about the customer, personalizing a specific outreach that is relevant to that customer and their situation and the goals of the outreach, and then sending that directly to the customer. I can show a couple examples of what that looks like. So this is one I did last night right before the podcast, reaching out to someone who has started using this app but hasn't fully converted from their trial, asking specifically about Their experience with the program, what were their thoughts about how intense it was or what the level was. You have the customer respond. The agent is able to get back right in a couple of minutes. You're able to continue that conversation, continue asking follow-ups to gather more information.

**Greg Greiner** (00:11:44)

And one of the things that we found with Woven is A lot of the value of this personal outreach exists when you're able to respond quickly. We've added and tested adding delays to the response mechanism, and you see the reply rate drop precipitously, so people are likely no longer in their inbox, likely no longer in the workflow of doing their email, and so you lose them at that point. And the conversion rate also drops alongside that. And so that's where AI can come in and enable you to respond really quickly, really accurately to these customers at scale. And to get that benefit of these long running conversations where you're really extracting a lot of insight.

**Aakash Gupta** (00:12:29)

So why over email? Why not just within the app, I guess, wouldn't that be a little bit smoother?

**Greg Greiner** (00:12:35)

Yeah, so I think in the app also definitely makes sense. And we work with customers and recommend adding in-app chat as well. But email has a few benefits. One, this abandoned audience, right? They're not in your app anymore. And you also need to be careful when you're doing things in app about not distracting from the core Goal of someone being in your app, right? You don't know that they're going to abandon yet. And so you don't want to actually have this like research oriented chat end up basically hurting conversion instead of helping. The other benefit is it's really easy to roll out and scale. It's a channel that all of your customers already use on a daily basis. And so you're able to be much more proactive and aggressive. And so we get, especially with these research campaigns, 20, 30, 40% of these people responding, which when you think about how many people would interact with an AI chat that exists on a site, it's much, much lower.

**Greg Greiner** (00:13:39)

You get a broader ability to capture that audience.

**Aakash Gupta** (00:13:43)

Can we just maybe break down how you drive? What's the difference between driving 20% response and 40% response?

**Greg Greiner** (00:13:51)

A lot of times it is around the type of campaign that you're running. I think when you are doing something that's very research oriented, and if you're doing something that's a little bit later in the funnel, meaning people have already shown some intent right there, like in this case, like already using the app, have had experiences with it. Much more likely to respond and much more likely to get up to that higher range of responses. We just did an experiment with a company in the fitness space and they saw about a 35% for this exact use case of trial abandon. And then as you go down, it's often lower and earlier in the funnel, right? Maybe someone just entered an email but didn't actually finish an onboarding process. And so there's less intent. But there's also matters, you know, how well you do this initial outreach, how personal it is, how relevant it is to them that is going to drive whether people respond in a similar way to, you know, in B2B sales, you know, cold email outreach, right?

**Greg Greiner** (00:14:54)

The better you make this email, the more likely it is that this person is going to be willing to take the time to respond.

**Aakash Gupta** (00:15:00)

So if you had to give like your average PM at a startup a template for this email, what would it look like? Would it be this kind of plain text sort of version so that it seems more human?

**Greg Greiner** (00:15:09)

Yeah, I think that's the right approach. And asking simple, direct questions that are really relevant to where the user is at at this point in the journey allow you to open the door to them responding, sharing some information, and then you can expand on that. I think mistakes people make is too much content, you're trying to ask too many questions at once, trying to essentially recreate your survey maybe in one email. When if you take it a little bit slower, one, you can let the customer lead you towards what they care about and what they want to share insights about. But also you can often get to all of those questions through the back and forth of the conversation at a much higher rate than if you're trying to stuff them all into one specific outreach.

**Aakash Gupta** (00:16:03)

If you had to think about like, what are the right set of emails for someone to create? These are like the four points along a typical journey. How would you map those out?

**Greg Greiner** (00:16:14)

Yeah, I think, um, you know, if you take this example of this fitness app that has a trial, right? I think there's one at the very beginning, right? There's going to be people who even start that signup process. Like I mentioned, enter an email address. Never actually finish creating their account, finish the onboarding process, select a program. And so that's going to be the widest part of your funnel. It's going to be the lowest response rate, but also the highest volume. And so I think that's one that makes a ton of sense. It can also inform the rest of your journey downstream of that. I think the second touch point is it makes sense to do it somewhere in this trial and potentially multiple times within this trial where you're getting people Set up for success. And then you're checking in on that success to see how they're proceeding through the product.

**Greg Greiner** (00:17:05)

And then I think, you know, when we're talking about onboarding specifically, the last one that makes sense is obviously a lot of the people in these trial situations are not converting, right? They're not going beyond that trial. And so I think it always makes sense to reach out to that group as well. And one of the things that we've seen make sense that I think is really easy to do, you know, as a PM as well. Is at that point offer some form of incentive just for sharing insights. You don't have a lot to lose at that point. And so saying, hey, if you share things that you think we could do better for your next trial, I'll give you 20% off your subscription for the next few months. And so what we've seen that do is it massively increases reply rate, but it also increases reply rate for the audience that's already on the fence.

**Greg Greiner** (00:17:54)

And so you're not going to reply to that email for that incentive if you weren't already considering it. And so you get a captive audience who... You can both address their concerns, right? Like hopefully make them feel good about you, about purchasing the app while also pairing that with, um, a promotion that you were probably going to send anyways, um, to get them, you know, to take that next step and come back and convert through the funnel.

**Aakash Gupta** (00:18:19)

So I guess that's the onboarding stage. What about further? If we go into once they're engaging in the core app, once they're retaining, once they're lapsing, what are the other points along the life cycle that this makes sense?

**Greg Greiner** (00:18:31)

I think when you're engaging in the core app and successfully engaging the core app, that's where the in-app experience and chat makes the most sense, right? That's where you should be capturing people in the moment in that experience. They're using this product on a frequent basis. I think where using these more traditional channels can make more sense is, again, at these points of drop-off or abandonment. So it could be an active user who has explored a new feature or an upsell feature for the first time but didn't actually convert. I think that's a really unique opportunity. Or it could be someone who was, as you mentioned, like previously active, but has decreased their usage in the last few weeks. Or it could be someone who obviously canceled their subscription, right? So that's another opportunity similar to the trial where every incremental conversion you save there is additive.

**Greg Greiner** (00:19:30)

But also those are some of the most interesting insights you can find are from this audience of people who have decided this isn't for them and the value wasn't good enough.

**Aakash Gupta** (00:19:39)

Okay, makes sense. And operationally, I guess are these through like your transactional emailing system? I guess like a lot of times marketing ops will own that.

**Greg Greiner** (00:19:48)

Yeah, so I think for these tests, you can do this. I did this with a standard Gmail account. And so that limits obviously the scale of the outreach that you can do based on what's reasonable to do from Gmail. But it does allow you to do it completely by yourself without using an existing or system for marketing. This is all just happening from this greg at cadencedemo.com. These are the outreach I just sent earlier. And so I think that's very possible if your audience isn't massive. And then I think, yeah, if you're dealing with a larger audience, you would likely need to partner with your marketing team to use an existing tool, or it's really trivial to set up Postmark or another type of tool specifically for this use case. And honestly, relatively common for research-oriented use cases to already be sending from a different service, even if you're using The legacy systems like Medallion, Qualtrics, all of those are not sent from the marketing team.

**Greg Greiner** (00:20:56)

They're sent from those systems.

**Aakash Gupta** (00:20:59)

So you could stand up your own sort of like product research email system. That's what's common best practice. Okay, I didn't know that. Very cool. So what I'm taking away from this is, Email is this super powerful channel. You should set up this stack where you have the ability to email your customers and you can make it a lot more intelligent by emailing them at the right time via the right triggers based on their life cycle. Typical things like trial, didn't sign up, lapsed, churned finally. Then on top of that, you can layer in instant AI responses in your voice to go deeper on the conversation, go deeper on the insights that you obtain, At the same time, potentially address concerns that they have to improve the conversion rate at that step of the funnel.

**Greg Greiner** (00:21:47)

That's right. And I think for an individual PM, I think this type of thing can be very powerful as you're trying to both better understand an audience for a specific product or feature that you own. And then also you want to drive adoption of it, right? You want people to be using it. You want to be able to follow up with those people. And so you also create this audience of engaged people that you can come back to these threads, right? Even if it's manually or you can have Claude take a pass through your inbox and identify interesting folks and say, hey, I'm launching a new feature. I want to see everyone who mentioned something related to this feature. And I want to reach out to them, you know, either with a follow-up question or with a, you know, invite link to jump on a call to talk through this feature that was developed based on their feedback.

**Aakash Gupta** (00:22:37)

So we started with the output report. We showed you what the outcomes look like as email. You cooked it up in just 30 minutes. Can you at least get us started? Show us how you would use Cloud Code? What prompts that a typical PM might be using to get the scaffolding for this setup?

**Greg Greiner** (00:22:55)

Yeah, I think pretty straightforward. I mainly just gave Claude the context of trying to set up a specific outreach program from my inbox using Using the Gmail MCP. And so similar, if you were gonna use, let's say I put the Postmark MCP and pointed it at the source of the customer data. So I think that's one of the main things that you need to figure out is where are you gonna be getting this trigger data from? And then gave it instructions on, hey, these are the context of the conversations I wanna start. I wanna be reaching out to people who are 10 days into their trial. And then let it essentially run with that context. And the first pass needed some tweaking, right? There were things like the threading was broken on the replies, right? They didn't get actually threaded back into the email or some of the language was inappropriate.

**Greg Greiner** (00:23:56)

And so there's some optimization that you can do just by having it run through tests like the ones I'm showing here. But I think even with that, So there's two things I think is really, really interesting here. 30, 40 minutes that you can start testing with real customers.

**Aakash Gupta** (00:24:14)

So there's two things I think is really, really interesting here. The first is that as soon as we're going to talk to the customer, We probably need to think about what our online evals to measure that it's actually pulling up-to-date information from our real help center, that it's helping drive objections down in the way our sales team want it, that it's maintaining our corporate brand of voice. And then there's this component of automation of how do we create this as a system that can quickly respond? So can you walk us through how you might build those?

**Greg Greiner** (00:24:49)

For sure, yeah. I think for this demo, we already have this classification process, but one of the things that we can showcase live is the next step of this, which would be adding evals as a separate step to this process that run before the actual reply gets automatically sent to the customer. And so if I go over to Cloud Code, I'll zoom in a little bit here. You can essentially just ask Claude and explain what you're trying to output. And if you've already put a little bit of work into this, it should be able to give you a pretty good approximation of this. So you can say, we now want to add an eval step after classification for responses that are queued. To be auto-sent, focus that eval step on groundedness in the documentation. If the eval fails, rerun the generation process and save. The new generation as a draft for review.

**Greg Greiner** (00:26:10)

So I think this allows you to do a couple of things. One, it sets up the process for evaling and then I think you can then build additional evals beyond just groundedness. And then two, it starts building this loop that I think is really important of when an eval fails, what happens? So the eval should not just stop the whole process. Ideally, you're using the information from that eval failure to have the agent take another pass so that you can still, even in these cases of eval failures, Get to automation that you feel confident in.

**Aakash Gupta** (00:26:55)

This is something I haven't seen somebody build before. So basically, you're building the evals live into the product. And here we're focused on groundedness. What Claude is doing is it's building this system of judging, okay, what is the groundedness? What is the true data source? What is the LLM judge? And then, like you said, it's creating this loop. If the LLM judge views it as non-grounded, update to the grounded version and then actually send it.

**Greg Greiner** (00:27:21)

That's right. And I think what we've seen on our end is that for the vast majority of cases where these evals are failing, you can pretty quickly get to a positive response that passes. And I think one thing that's important as you're building this is you don't also want to be necessarily overfitting to, okay, it's just taking this exact eval and it's like following it to a T. So you would ideally want to use the eval failure as input to another full run of your process of generating a response so that it's still going through that full logic loop of understanding how to respond and taking the evalin just as input versus like here is the exact instructions, right?

**Aakash Gupta** (00:28:13)

You wanna update things. This is fascinating. I can't believe I haven't heard about this before but basically You're building quality into your product so that there's no non-continuity, that it doesn't just stop. And at the same time, you're probably improving your performance on your online eval. So if you had a groundedness metric, probably if you launched this loop, you would see a bump up in that groundedness metric because it's getting the feedback live.

**Greg Greiner** (00:28:39)

Yeah, exactly. And that's, I think, one of the benefits. We talked about email earlier. One of the benefits of email is there's not an expectation of instantaneous responses, right? It's actually a little bit weird if you're responding like within seconds. And so by having a little bit more time, you can run these loops in a way that you can't if it was a chat-based experience because it would just be like someone sitting there waiting for like three minutes for the chat to respond back. And so that's what allows for this process to exist and still deliver a good customer experience because there's not a need to actually respond within whatever, 300 milliseconds.

**Aakash Gupta** (00:29:27)

So what's pretty fascinating is Claude had no clarifying questions so there's probably some risk that it's going to go off into some direction that we disagree. So as it's finishing up its response here, what are we going to look for?

**Greg Greiner** (00:29:41)

I think you want to understand specifically what changes that it made and how that's impacting your process. Looking at where it's inserting updates to this process of processing the replies, how that's manifesting itself into the summary that it's writing here, and making sure that the summary is aligned with what you actually intended the output to be. The evals are only going to run in autosend mode. That makes sense. If it's not on autosend, we're already going to draft immediately. The groundedness eval will check generated replies claims against the underlying documentation. I think that's also accurate. And then on failure, regenerate once with a specific issue corrected and then save to a Gmail draft, which was what I instructed it to do. I think per our conversation, the next stage of this is probably updating this to retry multiple times potentially and get to that approved response that you can auto-generate.

**Greg Greiner** (00:30:54)

And then I think the power of AI too is it's doing things that I didn't even ask for. As a part of this workflow, I have Slack notifications, like this one from the one I sent earlier, that get sent when an inbound message comes in and it's processed. And it automatically added this failure emoji for the case where the eval fails, which didn't even have to explain that that would be valuable.

**Aakash Gupta** (00:31:23)

Okay. Fascinating. So we just showed you how you could potentially be engaging with almost all of your lapsed customers, downloading information from them. We showed you how you can vibe code this as a system built in cloud code with proper eval so that you have confidence when you're putting it in front of your customers. Not everyone's going to want to build this themselves. So what's the experience like if they choose woven?

**Greg Greiner** (00:31:52)

For sure. So I think a lot of this complexity is, you know, managed for the customers who work with us. And so the process looks largely the same. It's just intended to one, be at much greater scale and to have a bit more of a conversion orientation. Like we talked about the, you know, the more research oriented campaign versus the conversion. And so going back to that ancestry.com example, this is an example, again, of someone who abandoned their DNA kit. These outreaches get sent at scale based on integrations with your marketing automation platform or CDP. So we handle that kind of data pass through. Customers respond and then the AI gets back to them. And then as a part of setting up one of these engagement points, we generate a bunch of simulated examples, which allows you to essentially give feedback to improve the responses directly.

**Greg Greiner** (00:32:52)

And so this is how, without having a bunch of back and forth with Claude, without having to build all of this yourself, You can quickly get to confidence and also see and visualize, hey, here are the changes that the agent is specifically making based on my feedback, right? So I created a guardrail. It created a playbook, it updated the agent context. And so you can review all these things and gain confidence, but then also see the output and how it's been improved. And then on top of that, we talked about evals and guardrails. That's something that we've invested a lot in defining really strong guardrails globally that handle things like groundedness, handle things like the formatting of the email. And then in addition to that, as a part of this training process, we're setting up custom guardrails that are based on the feedback you share, based on what matters most in terms of ensuring quality.

**Greg Greiner** (00:33:54)

And so those are then run on every response. And like we discussed, are rerun essentially until we get to a passing response. And so that's one of the things that makes this powerful is our customers, like we have customers who have hundreds of these engagement points live with us right now. And it takes them like five to 10 minutes to set a new one up once they've gone through this process a couple of times. And so, you know, You can kind of hit on, we talked about all the different points in the journey, start with something straightforward like this cart recovery use case. You can start hitting on these conversational campaigns basically everywhere where you have questions about customers, where you want to be influencing customer behavior.

**Aakash Gupta** (00:34:37)

When is this not the right choice? When should a PM be by hand emailing, looking up customers, making sure that they talk to the customer instead of the AI talking to the customer?

**Greg Greiner** (00:34:50)

I think it's dependent on scale. And I think also where you are on the like product market fit journey, I would say as well. So I think in cases of lower scale, There's a lot of value in having those more direct conversations. There's also a lot of value in having conversations that are not text-based, where you're actually meeting with someone, building a relationship, really understanding them at a deeper level. And I think that's also true when you're in the earlier stages of finding product market fit. You can't fully automate that process of discovery. The AI agent is never gonna have the same amount of context that you have as the PM of this early stage product. And so this is for a little bit later in that product market fit journey where you already have a sense that you're creating value and you just wanna maximize that value.

**Aakash Gupta** (00:35:46)

If you broaden it out, Still at Bolt for a second. You now have this new capability. They've built out this system. What is the broader research agenda advice you're giving to a new PM on the team? What does all of the AI-enabled research activities, not just this one, but all of the AI-enabled research activities they should be engaging in look like?

**Greg Greiner** (00:36:13)

Yeah, I think, like you said, this is one piece of a broader AI research strategy. I think this makes sense for a constant drumbeat of research, but I think there's opportunities to scale the other types of research as well, particular customer interviews, particularly customer interviews. So I think there are tools like Listen Labs and other types of products that Enable you to automate these more voice-based back and forth research conversations. And so again, I wouldn't necessarily recommend those for an earlier stage company, but by the time I was in the later stages of my career at Bolt, those are really powerful opportunities where we had a lot of B2B customers, but also millions and millions of shoppers on our network from a B2C standpoint. And so you have an opportunity to use those automated research interviews to dive a layer deeper and potentially use these email conversations as an entry point to find the users who have the most interesting insights to share.

**Greg Greiner** (00:37:23)

And then using that next level of like actually an AI facilitated voice back and forth to go deep with those people and get like a much richer set of feedback and context from them.

**Aakash Gupta** (00:37:36)

So maybe you can react to this and see if this is about right. Because what I don't want to do is I want people to see this episode and then all of a sudden purely pursue AI-enabled research. So is this accurate that the typical PM should still be regularly chatting with customers on Zoom calls, over text message, over Slack? I would say multiple times a week if possible. By multiple, I basically mean more than two times a week. At least you're having a Slack chat or you're texting or you're Hopping on a call are, of course, the best thing. You're literally watching them use your product in their context. I still think a PM should probably be doing that once or twice a week. But in addition to that, they should be setting up these AI-enabled research programs. Like you said, they should be setting up synthetic conversations with an AI avatar.

**Aakash Gupta** (00:38:28)

They should be setting up email-based chats on key levels of the journey like we demonstrated today. They should probably also be setting up some sort of platform that's analyzing all of their sales calls, all of their social messages. So they probably have at least these three AI enabled plus the regular discovery, which maybe is part of like a continuous process. So there's basically like four sort of key customer research activities that PM should be pursuing.

**Greg Greiner** (00:38:55)

Is that right? Yeah, I think that's right, right? I think what these more automated workflows can enable is making those true moments of interaction and relationship building much more powerful, right? Because you'll be coming into those conversations much more educated on Your user on, you know, what the foundation is, where there's potentially like interesting things to poke at and interesting things to dive deeper on. And so there's don't replace those real. Moments of human to human interaction where you can really dive deep and understand someone. They just make them more powerful. You waste less time in those conversations covering things that you should probably already understand. And that's one of the other things that we think is powerful about the more steady drumbeat process is when we're generating these research reports, I showed the example of this deck based version, but we're also generating More true report-based versions, and we're sending those over Slack.

**Greg Greiner** (00:39:58)

And so that gives an opportunity where this research is really living where people are working, and they get that steady drumbeat of what are our customers saying? What are they actually doing after they share this type of feedback? And so that can then inform that more in-depth research that you do on top of this.

**Aakash Gupta** (00:40:21)

So that is... Just a masterclass in what the state of first class discovery and research looks like. You had some really hot takes on product management in general, and so I wanted to shift there.

**Greg Greiner** (00:40:34)

Sounds good.

**Aakash Gupta** (00:40:36)

How has AI changed what PMs need to be able to do?

**Greg Greiner** (00:40:40)

I think I've been reflecting on this recently, and one of the interesting things that I felt at Uber was that actually the ratio of PMs to engineers was often way too high. You had teams of one PM and three or four engineers, and so you had these cases where PMs were looking for things to do. And I think at my greatest scale at Uber before I built a team, I was at about one to 25 engineers. And I felt that was actually one of the most productive times for myself and the team because there was no room for anything but developing product and creating value and moving quickly. No room for processes and all of these different things that PMs can get caught up in. And so I think one of the things that AI enables is that you can actually go back to that Uber style ratio and have a PM and three or four engineers, but still create the output of that 25 engineer team.

**Greg Greiner** (00:41:43)

And so what that means is PMs will need to be shifting their mindset to be able to handle that level of scale. And that looks like Being able to context switch very quickly, being able to manage a number of roles beyond the traditional PM job description. We didn't have product marketing support. We didn't have all the design support that we needed. And so the PM becomes that person who needs to fill in the gaps when you have so many people producing and you need to be able to Stay ahead of that level of output in a way that still feels cohesive. It still feels like you're building something that's greater than the sum of its parts, which can be particularly challenging when you have 25 engineers or you have an AI-enabled team of four or five engineers because the output is so fast and you're just trying to hold on for dear life and keep up.

**Greg Greiner** (00:42:43)

And so that's like one of the biggest challenges facing modern PMs is being able to stay ahead, being able to continue to have these features that you're launching be cohesive and additive and not just, hey, we're shipping everything at customer requests and we're doing it as quickly as we can.

**Aakash Gupta** (00:43:02)

Can you break that down in more detail for me? What are the processes that PMs used to get caught up in? How do you say no to those processes? A lot of times when I was working at a bigger company, I almost felt trapped by the process. I could recognize it in my time, but I didn't know how to get out of it.

**Greg Greiner** (00:43:19)

Yeah, I think often it's meetings, right? So often it's, you know, you have to get approvals, you have to, you know, jump through a lot of hoops, you have to get like a bunch of stakeholders aligned. You have to, you know, check some boxes for some planning processes at the corporate level. And so obviously, you know, when you have this like torrent of productivity coming at you from the engineering standpoint, You have to get creative, right? You have to be able to push back on the meetings that you know are just busy work and cruft. And then for the others, you need to find ways. I think AI enables this in a much more scalable way to spend less time on those. Automate more of that process of getting ready for and completing those meetings. And I think what PMs could get caught up in the previous world is that all of that cruft, all of those processes, all of those meetings were the actual job and not actually building product and talking to customers and releasing product.

**Greg Greiner** (00:44:32)

It was, hey, I'm going to jump through the corporate hoops. I'm going to You know, check all the boxes on this playbook for how PMs operate. And so I think that, you know, is being forced to be shifted away in this new

**Aakash Gupta** (00:44:46)

era where people can produce so quickly. And then you made this provocative claim around ratios. So just let me understand this. What do you think is going to be like, what is, I guess, the right ratio? Because we can assume maybe that the future will adjust towards what is the right ratio in the future.

**Greg Greiner** (00:45:06)

Yeah, I think now a team of three or four engineers can produce the output of what a previous team of 20 or 25 engineers could. And so I think a really small pod of, let's say, three to five at max engineers in a PM can be a good ratio because they're able to iterate and produce at a much, much higher velocity. Being a smaller team, being very closely aligned without the cost of just like you lose a lot of horsepower in the previous world.

**Aakash Gupta** (00:45:45)

So we touched on this a little bit in the podcast, but I'd love to get your take as somebody who's day in, day out building an AI company. What is the difference between AI that is ready for an internal audience and AI that is ready to scalably engage with customers? And how do you build that?

**Greg Greiner** (00:46:03)

Yeah, I think it's about the technology that you build around quality specifically. I think whether it's an internal audience or even it's a tool that's meant to generate outputs that you then review, The quality bar needs to be so much lower because you can feel confident that, hey, a human is going to look at this before this gets shared in any sort of public way. But when you strip that away, you need to have the appropriate guardrails in place and you need to be thinking about every update you make. And measuring them against both those guardrails as well as continuing to do some level of human QA. So something as simple as bumping a version of a model when you're building something that's internal or not directly going to customers, you can just do that and feel pretty confident that that's going to work. When you're shipping something actively to customers, you need to have a much more rigorous process around having an environment where you have sample data that you trust, being able to run outside of production these generations on that sample data, ensuring that they're still passing guardrails at the similar rate that they were previously, doing some additional QA to make sure that some regression didn't happen that you weren't expecting.

**Greg Greiner** (00:47:33)

And only then can you feel confident upgrading that model. And so when you're doing that hundreds of times a week because you're updating and improving and optimizing these customer outputs across a complex customer base and trying to optimize for things like conversion, you need to be able to do those sandbox environments tests at super high scale. And with a great degree of confidence, that's just not necessary when you're not directly talking with customers.

**Aakash Gupta** (00:48:11)

What's interesting there is you use a kind of like traditional PM language around it, guardrails, testing environments, sandbox environments. You didn't like put a new label on the skill like, oh, you need to learn this type of online eval or this type of method gradation. What would you say are sort of those new skills that you've had to learn from the pre-AI building world to now building AI products 24-7?

**Greg Greiner** (00:48:40)

I mean, I don't think the fundamentals actually change that much. I think, you know, obviously what changes is when you're dealing with a probabilistic tool, right? The type of testing that you're doing in those sandbox environments and the type of guardrails and evals that you're running change pretty drastically. You change from, hey, we have tests that our software team writes that ensure even the most advanced tests ensure that When you're interacting with the product, things happen as you would expect. Now you're in a world where you need to be testing the nth possible iteration of how someone might interact with this. If you're confident about what's going to come out the other end. And so it ends up being a combination of those traditional tests that you would run, like deterministic tests that say, hey, is this output what I expected from a product? Discreetly measurable sense.

**Greg Greiner** (00:49:47)

And then, you know, these more advanced LM as a judge evals that are doing a greater degree of reasoning behind a much more complex problem like groundedness or a much more complex problem like ensuring that the AI doesn't do anything that it wasn't explicitly given permission to do. And so those are cases where it's like, hey, like the AI really wants to please. And so, you know, when customers ask for things and like there's stories about this from the early days of like, I forgot it was Toyota or someone like got a free, someone got a free truck or the AI to say that they can get a free truck on their chat. Yeah. And so those are much more challenging things because the AI and the LM as a judge want to, please, they want to do what they're being asked. And so you need to be thinking about ways to tie those things back to something much more concrete of saying, hey, I want you to actually tease apart Every specific action that the AI has taken in this response.

**Greg Greiner** (00:50:55)

And I want you to actually link back to the specific instruction that gave it permission to do that. And so you have to get like, it's not just Tell me if the AI has done anything it's not supposed to. You have to go a significant layer deeper than that if you want to do this at a significant scale.

**Aakash Gupta** (00:51:17)

So examining the specific traces where things go wrong is really important.

**Greg Greiner** (00:51:21)

Yeah, I think that's particularly important. And I think also examining the specific traces where things go right. I think you have the opportunity where the AI is being creative and doing things in interesting ways. And like the example I gave earlier, let's say in a topic where almost no one ever converts after they bring this up, the AI response one time helps them convert. What can you learn from the approach that the AI took to get to that point is an equally big opportunity as like, hey, I made a huge mistake here. Like, what can we learn from how you can tie that back to how it specifically made that mistake?

**Aakash Gupta** (00:52:07)

So in our pre-call, we were talking about how you guys work. And I think this is going to be really illustrative and insightful for others because you have a unique place, right? You're not at Uber with 200 other PMs. You're a small startup, you guys get to operate and define your processes to the level that the current tooling allows. So what are the interesting things we can learn about what an AI native startup looks like in the inside?

**Greg Greiner** (00:52:39)

For sure, I think a lot of what we've discovered is that It's really easy to build. It's really easy to build quickly. It's also pretty easy to build with pretty good quality. I think those are things if you have the proper engineering workflows, leveraging the latest AI tooling, you can get really good at. What's hard is still building the right thing. And so that's where you spend a lot more of your time. And we found it to be really valuable to spend a lot of that time In discussion. There's four of us on the team. Let's all sit down and talk through this problem space. Let's have someone obviously bring to the table an artifact that Lays out the problem, lays out the opportunity. And then let's work through what are the biggest challenges we need to solve? How are we going to solve them? What's the experience we want to create?

**Greg Greiner** (00:53:35)

Whiteboard that as well. And then you end up with an artifact, which is a detailed transcript that you've recorded from this discussion and a diagram, either a live whiteboard or a fig jam or something similar. You can feed that into an AI skill that then goes and takes that, defines a much more detailed PRD off of that, creates the appropriate linear tasks to project manage that all out into the appropriate work streams, and actually has the agents start churning on that where that makes sense. It follows on with areas where we need to do more definition or have more discussion. You end up with a lot less time, obviously, like directly developing or like sitting down at a keyboard and writing out a PRD and a lot more time actually having those real substantive debates about how the product should work, how it should evolve, what comes next and things like that.

**Aakash Gupta** (00:54:39)

So am I hearing this right? Instead of spending your time writing PRDs or writing front-end PRs as an engineer, engineers and PMs are spending more of their time in meetings sketching out this is what it should look like, making sure that the transcript has that information and they have pictures with that information. Then the AI comes back with, okay, here's a working prototype and you improve it and ship it from there.

**Greg Greiner** (00:55:07)

That's right. And that's why it has been very important for us. And I think in the future, it's very important to have everyone at that table be capable to at least a certain degree from a product and a business standpoint. We want people who understand what we're trying to accomplish as a business. We want people who understand and have some level of product intuition. And so it's when you have those Disparate expertises, but at least the same baseline of understanding where those discussions can be really powerful.

**Aakash Gupta** (00:55:41)

So if you're at a larger company like Uber or Bolt and you can't like adopt all of that, what can you adopt? Like what other specific tools within how you're engineering your harness, specific processes with how you're working with your product team to just operate a little bit more like this nimble AI native new way?

**Greg Greiner** (00:55:58)

Yeah, I mean, I think you can adopt a lot of it because even if the expected output is, hey, we have this standardized PRD that we need to go then, you know, get approval and review from different parts of the organization, you can still model how you get to that PRD in this more AI forward, AI native way, right? So you can still... Have that opportunity to work with, maybe it's not often your full team if it's a larger team, but maybe it's a subset of people that you feel are the most important in making those types of definitions and decisions. Have those conversations and then have the automation and the skills developed to automatically turn that into the format that you need for your corporate processes that you need to run through. So I think a lot of it is very usable. You just need to adapt it to what outputs are expected from you as a team and also the personnel that you have around you and what types of people are going to be most effective in those more open-ended, product-oriented conversations.

**Aakash Gupta** (00:57:12)

All right, guys. Greg Greiner is the name. LinkedIn is where you can find him on social media. Envoy is his startup where if you want to increase conversion rates or get closer to your customers and not vibe code this whole thing out, but choose a solution that has built it for you, you can check it out. Thanks for being on the podcast, Greg.

**Greg Greiner** (00:57:31)

Of course. Thanks you're having me.

<!-- sponsor -->
**Aakash Gupta** (00:57:33)

All right guys, if you want more content like this, do comment below who you want to see on the show next, what topics you want to cover next. Should we have more on AI research and discovery or do you want execution and coding? Just let me know and I'll see you in the next episode. I hope you learned as much from today's episode as I did. If you can do one thing that's totally free that would help the show, it would be to check that you're following on Apple and Spotify podcasts. Check that you've left ratings and reviews on those platforms. Check that you're subscribed on YouTube. Leave a like and a comment on this video, and then share it with your friends. We're trying to make better and better podcasts. After two years, we think we've gotten something pretty good going. So let us know what we can do to make it even better, who else we should interview, and we We'll put on the best shows we possibly can.

<!-- sponsor -->
**Aakash Gupta** (00:58:18)

Finally, don't forget my offer for the bundle. You get an entire year of my paid newsletter, plus my favorite AI tools, Bolt Up New, Airtable, Speechify, Descript, Magic Patterns, Linear, Dovetail, Arise, and Mobbin. That's $27,000 worth of value for just $150. So check that out at bundle.akashgu.com if it interests you, and I can't wait to share our next episodes.
