---
title: "We Built an AI Agent to Automate PM in 73 mins (ZERO CODING)"
subtitle: "If you’ve ever wanted to know how the best product teams automate their workflows, scale systems, and build platforms that actually drive impact, this episode is for you."
date: "2025-04-11"
host: "Aakash Gupta"
guests: ["Anthony Maggio"]
speaker_names: "substack"
substack_url: "https://www.news.aakashg.com/p/airtable-vp-of-pm-heres-how-to-automate"
youtube_url: "https://www.youtube.com/watch?v=vh-urCCJhTs"
duration: "01:13:50"
word_count: 11970
source: "Substack episode transcript (aired audio)"
---

# We Built an AI Agent to Automate PM in 73 mins (ZERO CODING)

*If you’ve ever wanted to know how the best product teams automate their workflows, scale systems, and build platforms that actually drive impact, this episode is for you.*

**Anthony Maggio** (00:00:00)

If you want to learn how to build your own AI native applications without any coding or development experience, then this is an episode you don't want to miss.

**Aakash Gupta** (00:00:10)

So let's get to see how we put one of these apps together. Yeah,

**Anthony Maggio** (00:00:14)

let's do it. We'll walk

**Aakash Gupta** (00:00:15)

through building an app. So let's say we wanted to like add their LinkedIn profiles. What would that look like?

**Anthony Maggio** (00:00:21)

Yeah, so we can do LinkedIn. We can actually even like take it, you know, a step further. And what I was going to suggest. Amazing.

**Aakash Gupta** (00:00:28)

You have become VP of product at a Decacorn company, a $12 billion company, pretty crazy.

**Anthony Maggio** (00:00:35)

App to a CRM to track your guests, like dates, upcoming interviews, episode data.

**Aakash Gupta** (00:00:40)

What is unique about how Airtable is building product?

**Anthony Maggio** (00:00:43)

The potential for putting AI into action is bringing it into these types of applications where...

**Aakash Gupta** (00:00:49)

really quickly i think a crazy stat is that more than 50 of you listening are not subscribed if you can subscribe on youtube follow on apple or spotify podcasts my commitment to you is that we'll continue to make this content better and better and now on to today's episode Anthony Maggio, you are the VP and head of product for Airtable, which was last valued at $11.7 billion. It's kind of mind-blowing. Can you tell us a little bit of how Airtable really reached that valuation?

**Anthony Maggio** (00:01:23)

Absolutely. Nice to see you and thanks for having me on. So if anyone of your listeners are not familiar with Airtable, Airtable's goal is to be the best and easiest place to build AI-powered applications and enabled for non-developers. So really kind of where we stand out is finding this middle ground between the sophistication of apps that would traditionally require a really skilled developer to build, but with the entry point and ease of use of a spreadsheet or other low-end market tools. You know, a little bit of our journey is that the company was founded back in 2013, started out with this very user friendly spreadsheet like UI to allow our customers and users to track projects and organize their data and convert spreadsheet-like workflows into databases. And fast forward to where we are today, we're now relied on by 80% of the Fortune 100. Airtable's been adopted by over 500,000 organizations with over 50 million apps created on the platform.

**Anthony Maggio** (00:02:37)

And so it's been a long journey that has got us there. Obviously, the product, the go-to-market motion, the company as a whole has evolved over that last decade and change. But where we are today and really kind of where our focus is going forward is how to be the fastest and easiest way to deploy really powerful AI applications into any line of business workflow.

**Aakash Gupta** (00:03:01)

So who are the competitors of Airtable and what makes you different from those other options?

**Anthony Maggio** (00:03:06)

Yeah, so Airtable obviously as a horizontal platform has a myriad of competitors across the market. The two major categories that I typically think of are for the entry point use case, which might be an individual or a user or a team who's looking for a simple way to stand up a workflow within their company. There, we oftentimes will compete with spreadsheets, right, with Google Sheets or with some project management tools where the way that a team or an individual has been managing work starts to break down. They start bringing more and more people into a process and it becomes really hard to govern and manage. And that's often where we'll see those teams upgrade into a full-fledged application in Airtable. On the high end in the enterprise, increasingly we compete with point solutions for specific functions. So think product management tools, marketing, campaign management tools, as well as other enterprise low-code app platforms like Salesforce and ServiceNow.

**Anthony Maggio** (00:04:10)

And the big differentiator that we have on that side of the market is that we can deploy applications with the same level of sophistication as a Salesforce or ServiceNow without requiring custom-trained developers to build and maintain those applications. So on the low-end side of the market, we bring higher workforce sophistication, ease of use, more governance and control over the way that you're running a process. And then on the high-end side, we really compete and differentiate over the ease of use, the time to deployment, and the lower cost of maintenance of these apps because they can be maintained by individuals and non-developers rather than a professionally trained developer.

**Aakash Gupta** (00:04:54)

That's what I've heard time and time again from people who are big Airtable fans is I created what's functionally an app that's automating some of these key operations that would have cost us half a headcount and I just did it myself. So it sounds like you guys have really cracked those low-code apps in the enterprise. Today we're focusing on Airtable AI. And can you give us a quick overview of what it can do?

**Anthony Maggio** (00:05:22)

I'd love to. And you're going to see some great demos of what it can do today as well. So we'll go into those in a lot of depth. But really the best way to think about AI is in two camps within Airtable. So the first camp we refer to as co-builder and assistant. And really what the co-builder and assistant do is they help you to quickly create an application in Airtable. So I mentioned that the big differentiator for us has always been this ease of use, the time to value. allowing non-developers to create really sophisticated software. With AI, we're making that even faster and even easier. So opening up the aperture of the potential audience that can build really high-powered applications in Airtable. And we're doing that with AI being built natively into our own platform. The second category is what we think of as AI at runtime.

**Anthony Maggio** (00:06:15)

And this is where I spend a lot of my time with our customers and a lot of time with our product teams and really honing the offerings and capabilities there. But what our AI at runtime offerings do is allow you to actually insert AI automations and agents into the apps that you're building. So within a product management workflow, for example, you can have an AI agent that automatically categorizes and triages all your product feedback, or maybe one that goes and researches competitive offerings and keeps you up to speed on what's going on in your market, or helps you to aggregate research and gather insights out of research studies related to your product. So those can be really time consuming tasks for individuals to manage on a recurring basis. And with Airtable's AI, you can automate those types of workflows and run them on an ongoing basis within the apps that you create.

**Aakash Gupta** (00:07:15)

Awesome. Well, seeing is believing. So shall we get into a little bit of a live cooking session?

**Anthony Maggio** (00:07:20)

Yeah, let's get into it. And we've got two sections of our demo today. So one focused on some product management workflows, and then we're also going to do some hands-on building with co-builder and assistant. Any preference on where we start first?

**Aakash Gupta** (00:07:36)

Let's start with those PM use cases.

**Anthony Maggio** (00:07:38)

Great. So we'll go through a few PM use cases on the product today. What you're seeing here is an app called Product Central. This is our dedicated application that is oriented around product management teams and the enterprise. It's all built on top of the Airtable platform. So really any UI or workflows that you see here can be customized and tailored around the needs of any individual team. But we'll take a tour and go through a few of the workflows that we see as common ways that PMs are leveraging AI within Airtable. So I want to start with user interviews. And what we've got here is a database of user interviews that are being collected and aggregated in the product. And in a typical world, this data would all be flowing through automatically. Think like an integration with Gong or with Zoom or with any platform you might be using to record your user interviews.

**Anthony Maggio** (00:08:44)

But for the purposes of the demo, I'm just going to paste in an interview transcript so we can see what's happening behind the scenes here. So let's say I'm a PM.

**Aakash Gupta** (00:08:53)

Really quickly, though, I think that is one of the superpowers, right, of Airtable is you have a lot of those integrations built in, right? Exactly. So we could technically do a Gong integration. What would that look like if I was just curious to see where I'd start there?

**Anthony Maggio** (00:09:07)

Exactly. Yeah. So in a Gong integration, and this is something we actually do internally, we have this application hooked up to Gong. All of our recorded Gong calls come into this product central application. And from there, those transcripts are then chunked into individual pieces of product feedback that are searchable or indexable or can be referenced to customer accounts. And we'll show some of what that actually looks like in practice. So, again, I'm going to just paste in this transcript for today. But you could imagine that, you know, in a real instance of this, every time you get off a user research call, that Gong transcript is just flowing directly into this app. Okay. So once I create this, this is where some of our AI processes will kick off behind the scenes. So what you're going to see happen here is this interview is going to pop up.

**Anthony Maggio** (00:10:03)

We've now run this through a custom prompt where we've asked the AI to summarize the content of this interview.

<!-- sponsor -->
**Aakash Gupta** (00:10:10)

Today's episode is brought to you by Amplitude. Building great digital products is hard. You know that better than anyone. Getting teams aligned, measuring what matters, and scaling your product strategy isn't easy. But what if you had a clear framework to guide your next steps? That's exactly what Amplitude built. They studied the best product teams to understand what really drives impact. and turn those insights into the digital experience maturity assessment in two minutes you'll be able to see where your team stands and what you can improve to build better products faster click the link in the caption to take the free assessment and get a clear path to product growth

**Anthony Maggio** (00:10:46)

And then we've also asked it to pull out some of the topics that are discussed. So these are a range of topics that we're tracking internally within Product Central that are kind of common themes that we're following. So we can start to measure how often are different themes or topics being discussed by customers. We can also reference what are the projects that we have going on that are relevant to this particular customer. So this is always fun for me when I'm talking to somebody on an interview or speaking with a customer. I can pretty much in real time throw in some notes about a topic or an interest area they might have and actually show them our roadmap and backlog of initiatives that are being worked on right now that, you know, that will address that theme. What is the

**Aakash Gupta** (00:11:37)

AI in the background here that you guys are using?

**Anthony Maggio** (00:11:40)

Yeah. So each of these fields, and let me just, I'm actually just going to pop this into edit mode here for a second so we can pull this up and look at it more closely. Um, So essentially what this is, is a custom prompt that is being generated and then run against this transcript. So if I wanted to, you know, modify this just to call out, you know, specifically areas that a user was frustrated by or specifically topics that they, particular topics that they discussed, I can modify this prompt however I'd like. And then I have a choice of what models I want to use to, uh, to run this actual, uh, prompt. So, um, we integrate with, uh, with open AI, with anthropic models, with a number of other, you know, leading models. Um, you can either just, you know, stick with the default here, um, or you can, uh, choose to, to use another, um, model maybe based on your company company preference.

**Anthony Maggio** (00:12:42)

Got it. Great. We'll keep going, and I'll show off a few of those other features I mentioned. This is one simple summary of how we get some insights out of that interview. Where things get a lot more interesting is as you really start running through your discovery process. Here I now have a research hub. This includes a number of studies, a number of different pieces of of content of long form like user interviews that our research team has put together over time. And maybe I wanna ask about a particular topic that we've researched in the past. So I'm gonna say here that I'm thinking about a new feature related to helping customers Try on clothing in store. Have we done any research there? And what our assistant will do here is it can actually, this assistant works on any app that you build in Airtable. As I asked this question, it can understand the intent of my question, then go actually look through your app, the structure of your app, the tables that have been created, the content that you're storing in this app and formulate a plan around how it's going to answer this question.

**Anthony Maggio** (00:14:15)

So if you've used perplexity like deep research, you can think about this as deep research for your own data sets. So in this case, it's this user research studies kind of research hub. I see that there's been some relevant studies based on my question here. I can then click into each of these studies and go deeper. And I can actually even see the specific sources from these studies where this content is being pulled. So if I click on view sources here, this will pull up the actual PDF of this research study and show me the citations that the AI is referencing in generating an answer. So lots of use cases for this. Research hubs have been a big area that we see this utilized around, but obviously lots of different documents in the product management workflows. You can use this for PRDs, for searching tech specs, searching past experiments that you've run and indexing on experiments that maybe have or have not been successful.

**Anthony Maggio** (00:15:19)

So very flexible in terms of the types of analysis that you can leverage when engaging with this assistant.

**Aakash Gupta** (00:15:27)

Okay. So there's probably been a lot of work you guys did on directing the AI and prompt engineering to make it reliable and make sure it's citing its sources here.

**Anthony Maggio** (00:15:37)

Exactly. And that's been a big theme for us is that we really want our users to be able to trust the output. So we try to show a lot of the work. You see that in the assistant as it's actually generating a plan. We try to show off what it's indexing, what tables it's referencing, how it's getting to an answer to help you understand that the answer that you're getting is accurate and matches your intent of the question. And then similarly, within the document analysis use cases, providing those type of sources. will you know really kind of give you that that confidence that whatever the intention was in this case it's just a summary but you know let's say you asked a more specific question about uh you know are there any references to the fitting room experience we can see exactly where those references are coming from and really get the confidence that our answer has been provided correctly

**Aakash Gupta** (00:16:33)

So I think as a PM, this is all about being able to get to those user insights faster, being able to synthesize them faster. If you want to pull up user insights to use in a particular PRD or product review, that should be a lot easier here.

**Anthony Maggio** (00:16:48)

Absolutely. And it really starts to come together as you bring multiple sources together. So what we'll often see is, I mentioned user interviews and transcripts as one source, but the magic of this is when you can really bring all that feedback together into a single searchable hub or database. So call transcripts can be one source, support tickets can be another source that is coming in, direct feedback from your sales team. pulling cases out of something like Salesforce to really kind of capture all these different signals that you're getting around customer intent and then make them highly searchable, make them indexable or proactively surface them for your product teams. Got it. Yeah. So I'll jump forward here a bit now and say maybe we've seen some research about customers being frustrated in this case, this is a fictional e-commerce company, customers being frustrated by the in-store try-on experience.

**Anthony Maggio** (00:17:54)

We looked at some research that showed that fit issues are a common problem that we see from our loyalty customers. And as I jump into this backlog here, One of the things we're also doing with AI is auto prioritizing our backlog of projects. So this is a weighted rating that we've created with AI to look at for each of these potential initiatives on our backlog. What is our confidence level? How many audience segments is it going to reach? Um, where do we, uh, where does it best align to our own like internal goals? And we can kind of come up with a custom rating to, to auto sort this backlog. Um, I see here, like personal fitting experience is actually already, you know, something that we're, we're tracking on our backlog, um, and can pull in some of the related customer feedback that is auto matched against this initiative.

**Anthony Maggio** (00:18:49)

Um, and then even start generating the, the PRD. So. Again, we're using custom AI fields here. We can generate each of these and have the product suggest what are some success metrics or some feature requirements that we might want to consider building into this product. I can do some back and forth, give it feedback, edit the actual metrics that it comes up with. And then once I'm ready, I can just go ahead and click, you know, create document and this will fire off a process to actually pull together this whole PRD. So, um, it's now assembled this like into a, into a Google doc, into my PRD format, um, and makes it ready for me to continue editing or sharing with my team.

**Aakash Gupta** (00:19:37)

Awesome. And how did you configure your PRD format?

**Anthony Maggio** (00:19:40)

So that's all configured as part of this automation where we're pulling out these sections of, let's say we want a customer problem statement, success metrics, and feature requirements. Those are being grabbed from these fields and then assembled into a document through our automations product.

**Aakash Gupta** (00:20:01)

Okay.

**Anthony Maggio** (00:20:02)

So I'll show one more demo here on the PM side, and then we can maybe jump into actually creating an app yourself in Airtable, and we'll see a lot more of the behind the scenes around how this comes together. But let's say I actually decide I'm ready to to move forward on this feature project that we've been, um, discussing and I need to go find some beta participants. So I'm gonna, um, I'm gonna, you know, go build this new experience for a scheduled kind of in-store fitting session for my, uh, for my product. and I want to find some beta customers to help test this experience in a local market. Now we're not only referencing the user interviews, but we can also reference data coming out of the CRM, so out of Salesforce or any other metadata that we're storing at a user level and be able to query an index against this to actually find users who meet the description of the beta and the CRM is telling us that they're located in the market that we're going after to test this.

**Anthony Maggio** (00:21:15)

So, you know, a little bit of a simplified kind of example here to just show the whole lifecycle of product discovery in a few screens. I think, obviously, as all of your listeners and PMs know, it's much more, a lot more than this goes into it in real life, but hopefully kind of gives you a sense of how some of these capabilities could apply to really accelerate your discovery processes.

**Aakash Gupta** (00:21:41)

Okay, and that one kind of had that agentic behavior where it was giving itself a set of tasks, then it executed on those, and then it returned the summary.

**Anthony Maggio** (00:21:49)

Exactly, and that's a great example of what I mentioned around just showing the thinking. So with each of these questions, and one of the reasons why this assistant is so powerful is that it can really understand any data set that you've modeled in Airtable. and what's actually happening there. And as you saw in the example, it's going through the backend of this application and saying, what tables do I need to look at? What searches do I need to perform across these tables? Where is this data coming from? Do I need to tap into the Salesforce data sources to be able to find the user's location? And then pulling all of that together into a plan that answers my questions in around 30 seconds.

**Aakash Gupta** (00:22:35)

So you can really do a lot of different stuff. If we summarize all the different things we just looked at, we got AI-powered feedback analysis. We connected it to a research repository. We generated a PRD. We did some beta sourcing. So we kind of end-to-end are coming up with the feature idea, helping distribute it to our teams and distribute it to customers eventually.

**Anthony Maggio** (00:22:58)

Yeah, absolutely. And I think that our belief is that AI is already automating and accelerating every stage of the product development lifecycle. I think that we are seeing that, especially within some of that discovery phase, so tagging and managing feedback, getting insights out of research studies, running market analysis. analyzing user interviews, recorded calls, you know, understanding where those opportunities exist. There's just a huge amount of automation that can go into those processes and really, you know, turn a lot of this into, you know, a much more collaborative and proactive process versus what has oftentimes in the past, and certainly in my career as a PM, been a lot of painstaking manual review and manual treasure hunts to go find the users or the nuggets that you're looking for.

**Aakash Gupta** (00:23:55)

yes absolutely and this goes back to in terms of the competition you were talking about really competing with a lot of those research and pm point solutions i'm seeing some elements of dovetail and sprig in here i'm seeing some elements of a product board really like insights to roadmaps and prd so you guys have really gone from i guess historically been like a marketing ops or really known for marketing ops to like full frontal attack on these pm use cases

**Anthony Maggio** (00:24:25)

Yeah, exactly. And I think what our customers will frequently tell us is that the point solutions can be a good starting point, oftentimes for a smaller company or a mid-market company, just to kind of get stood up quickly. But as you really scale into a larger enterprise or company use case where you're operating these workflows across hundreds of product teams, sometimes thousands of PMs and product teams, having the flexibility to really tap into all these internal and third-party data sets to customize the experience both down at the local individual product team level and to synchronize and to cascade that data up into global roadmaps. That's really where Airtable stands out and shines is that flexibility over the data model, the visibility that allows our customers to really mold these applications to best suit their own needs and workflows.

**Aakash Gupta** (00:25:26)

Sounds like you guys are very laser focused on that enterprise ICP. Is that fair to say?

**Anthony Maggio** (00:25:32)

Yeah, that's fair to say, and that's been a big focus for us over the last few years, is really orienting our product around how we solve problems in larger companies. Airtable serves all segments of the market. We have a huge self-serve business. We have many, many individuals and small teams that love the product, and we continue to support those those users today and encourage our community of evangelists within that community. But from a use case perspective, where we really focus on are those use cases that exist in larger companies. I mentioned at the top of the call, our mission has always been and continues to be to democratize software creation. And when you look at just where apps are being created or where individuals are operating in applications, the vast majority of that happens in an enterprise context, in a business context where you have large companies with tens of thousands of knowledge workers who are spending a huge chunk of their day in software.

**Anthony Maggio** (00:26:40)

And so we've increasingly focused a lot of our attention on that user profile, both because the problems in that segment are really just much greater problems and the pain that those users experience around how to manage connected workflows and data silos and to build better visibility across larger teams. align really well to some of the differentiated value that Airtable provides. Awesome.

**Aakash Gupta** (00:27:08)

So let's get to see how we put one of these apps together.

**Anthony Maggio** (00:27:11)

Yeah, let's do it. So we'll walk through building an app in Airtable co-builder. Let me jump over to co-builder now. And Airtable CoBuilder, we released last July. It was an instant success with our user base. This was one of our first major AI offerings where we incorporated AI and LLMs into our own product. And again, the intent of CoBuilder is really to be an expert Airtable developer who is sitting alongside you and helping you to co-create your own application.

<!-- sponsor -->
**Aakash Gupta** (00:27:52)

Today's episode is brought to you by the AIPM certification on Maven. Run by Mikdad Jaffer, who is a product leader at OpenAI, this is not your typical course. It's eight weeks of live, cohort-based learning with a leader at one of the top companies in tech. OpenAI just doesn't stop shipping, and this is your chance to learn how. Run along with product faculty and Mo Ali. The course has a 4.9 rating with 133 reviews. Former students come from companies like OpenAI, Shopify, Stripe, Google, and Meta. The best part? Your company can probably cover the cost. So if you want to get $500 off, use my code AAKASH25 and head to maven.com slash product dash faculty. That's M-A-V-E-N dot com slash P-R-O-D-U-C-T dash F-A-C-U-L-T-Y. It is correct. I use a spreadsheet.

**Anthony Maggio** (00:28:42)

Okay, great. So, you know, we're going to say that We want an app to a CRM to track your guests, like dates, upcoming interviews, episode data. I also actually just pulled down a LinkedIn post that you shared of your upcoming guests. So I grabbed a CSV of upcoming guests on your show that will go ahead and attach and give it some context in this application as well. So the first thing that we do after this step is we will analyze the user's intent. We're running this through various LLMs and a number of different prompts that we've created on the backend to kind of get an idea of what this app is that you're creating. So looking at the data sets, looking at the instructions that we gave around guest tracking, interview tracking, like episode tracking, and you start to see this kind of preview of the app come together, some details of the guests that you've got coming up on the show.

**Anthony Maggio** (00:29:42)

We also give you a few other suggestions of things that you might want to track or add into this application. But for today, I'm just going to say, okay, this looks great. Let's actually go build this thing. And now what will happen here is that we're using the LLM to actually fully construct this app on the Airtable backend. One thing I'll call out that's really interesting and differentiated about this is that what you get here is actually a production-ready app. So there's obviously... now a lot of code gen kind of app creation tools on the market. They have been a lot of fun to play with. I've been playing around with them for many of my own kind of hobbyist use cases as well. But there's kind of a big gap between getting to that first gen of a code gen application and something that is actually ready to be shared, collaborated on, ready to be used by users within your company.

**Anthony Maggio** (00:30:48)

So that's really kind of what we're excited about here is that this app that's been generated, I can now immediately go in, edit, make any modifications to it, and publish it, and it's ready to share right off the bat. The other kind of big differentiator here is that is what we like to call or think of as inspectability. So again, with the kind of CodeGen products, if you don't know how to code or don't know, at least know how to read code, it can be pretty hard to understand what's actually going on under the hood of this app. And with Airtable, after this first generation, I really get full inspectability. So I can come over to the data layer of this app. I can see what were the fields that were created here. How are these fields linked together? Guests are connected to interviews, to episodes.

**Anthony Maggio** (00:31:44)

If I want to make changes and delete any of these fields or change this around, it's all point and click to do that. So it really makes it much more approachable for a non-technical audience to customize the application.

**Aakash Gupta** (00:32:01)

So let's say we wanted to add their LinkedIn profiles. What would that look like?

**Anthony Maggio** (00:32:06)

Yeah, so great. We can do LinkedIn. We can actually even take it a step further. And what I was going to suggest is that we do some research on each of these guests. So I'm going to

**Aakash Gupta** (00:32:18)

ask

**Anthony Maggio** (00:32:18)

it to search the web, create a research summary, include any details or past episodes of podcasts that they've appeared on, include news about their company, And here you're actually going to see a couple different things come together. So the first is this assistant that we were previously using in a kind of Q&A search capacity can also actually help you build the application. So the assistant has now generated a plan around this request to add a new field to my guest table. It's created a prompt. um, for the LLM, um, to, uh, to go and run like research on this guest. Um, and, uh, you can kind of see, you know, the output of what's generated here. So I'm just going to look at the prompt, like this looks pretty good. And maybe we don't have any interview dates in here yet. So I'll, uh, I'll just take this out and I'm going to tell it to, um, to generate automatically.

**Anthony Maggio** (00:33:19)

Cause I want it to actually run this prompt across, every one of your upcoming guests. So once I kick this off, we are now launching a internet search agent in Airtable that's going to go perform this research summary for everybody in this database. And, you know, this will take a couple seconds to generate, but what you're going to see is it's going to go, you know, look for the individual, go look for their LinkedIn. It'll analyze any kind of social posts. It will look up the company, you know, look for company news and we'll come back to you, you know, with a summary. So I'll just, you know, pull this up for myself. We'll see some recent podcasts that I appeared on that all looks right. I can actually kind of click and view the sources so we can look into where these podcasts came from and kind of get a sense of, you know, what I've done.

**Anthony Maggio** (00:34:19)

what products or what podcasts I've participated in recently. That

**Aakash Gupta** (00:34:24)

would save me a lot of time.

**Anthony Maggio** (00:34:26)

Yeah. And so if we want to take it a step further and where I think a lot of the power comes in in these AI use cases is actually not just the one shot, but chaining these together. So what I was going to suggest we do next is not only research, but actually come up with a potential interview guide for you. So I'm going to ask it here to brainstorm some potential interview topics for each guest. And what should happen here, we'll see how it decides to generate this, is that it should actually you know, now create a new AI automation within this app that's going to use the research that we just conducted to come up with a set of ideas or topics. So we can see here, yep, it's created a number of research topics with this guest interview summary. I'm going to, again, like ask this to run automatically.

**Anthony Maggio** (00:35:26)

So we'll, you know, we'll run it on the whole data set. And what you're going to get out of this now is, you know, something kind of like an interview guide, like what are some relevant themes incorporating the context of product growth, the types of topics that you typically like to discuss, as well as the areas of expertise for, you know, for each of your guests. So we'll take a look at one of these and, you know, see some Some areas that it's suggested that you discuss with with the linear CEO if you haven't interviewed him yet.

**Aakash Gupta** (00:36:02)

Awesome. Yes, that interview is coming up in a few weeks. That's exciting. There you go. And so I assume that I could like. How can I add more context? Cause like that interview guide right there, like as people are seeing watching this interview, like we probably all need to narrow it down to like one topic, but then we'll need to cover some of those subtopics for just short amount of times. How could I go the next step?

**Anthony Maggio** (00:36:25)

Yeah, absolutely. So, you know, everything like in this, um, this field that has been output is this is like your sort of first set of suggestions. You could decide just to edit these directly in the field and whatever you edit here will maintain its context. So, you know, if you wanted to actually turn this into your interview guide and store them in Airtable, you could do that. Or maybe you want to kind of cross-reference it with some other contacts. So maybe you've done like a prep call with each of your guests. You could have another field here for notes from the prep call and use that to actually refine this prompt and get to something like a full-fledged script or full-fledged interview guide. Okay. Yeah. One other piece I'll show just to really kind of bring this all the way to life in terms of a working app and thinking about what your workflow might actually look like is creating automations with this data.

**Anthony Maggio** (00:37:24)

And I think that's really where Airtable's power really shines is not just the storage of your guests in this app, but actually what are you going to do with the data? I have another kind of prompt here where I'm going to ask assistant to send me an email or like a notification every time a new guest is added and then to include that research summary as well as the interview ideas. So, you know, maybe if you're just tracking potential guests or tracking like folks that you might want to have on the podcast at some point in time in the future, you can just quickly kind of add them into your Airtable app. And then the AI will go do its thing. It'll go run its research. It'll go come up with its potential interview ideas. And when it's done, it's going to send you an email with all of the research that it conducted.

**Anthony Maggio** (00:38:21)

So this automation was just created. We can see here that it's It's ready to be enabled and to be turned on. It's saying a new guest has been added to your database. It's including some tokens for the research summary we just ran, the interview topics, and giving you a link to come into Airtable and get the full context around the research that was just conducted.

**Aakash Gupta** (00:38:46)

Awesome. Sounds like if I had like a full-time researcher, they could just automate half their job and then really focus on the value add on top of that. So it seems like there's a lot of potential here.

**Anthony Maggio** (00:39:00)

Absolutely. Yeah. And that's exactly where we've been focused is trying to give you that full-time database app builder through the assistant and researcher who's going and conducting this type of guest analysis and research on your behalf. That's really where we see just so much of the the potential for putting AI into action is bringing it into these types of applications where, you know, it's not just a one-shot conversation that you're having with a cloud or chat GPT, but really a recurring workflow that is something that you're managing on an ongoing basis, right? You know, everything I kind of showed you here, like you could probably do in one-off interactions with, with the chat GPT or perplexity or whatnot, asking it to run these research summaries. But where we really see the power of this is bringing them together to manage this entire research process for you on a recurring basis.

**Aakash Gupta** (00:40:03)

And personally for me, I would probably hire perplexity as my researcher and Claude as my writer for these two steps. Do I have that type of fine-grained control here?

**Anthony Maggio** (00:40:15)

Yeah, so the same thing applies in all of these fields that we're creating. So let's say like that you have decided that, you know, quad 3.7 is your preferred model for any kind of writing or, you know, creative tasks. Right. So I can go ahead and like save this. I'm going to overwrite all the data. And now we're going to basically just run this same exercise, this same agent, but using a cloud model. So if you have those types of preferences around where you've seen the best results through some of that one-off prototyping that you've done, you can then codify that into the application. And every time we add a new guess, it will utilize the models that you've set up.

**Aakash Gupta** (00:41:04)

Amazing. Well, it looks like we just figured out a way to save me an hour or two a week. That's awesome. Yeah, I will share the app

**Anthony Maggio** (00:41:12)

with you and you can report back next time on how

**Aakash Gupta** (00:41:14)

it's going. So I want to hear a little bit more about how Airtable uses Airtable and get into, because you are the head of product at Airtable and there are a lot of heads of product listening, a lot of PMs listening, how are you guys using it to do product differently than other places you worked? I know you were really senior at Envision and other companies like that. What is unique about how Airtable is building product?

**Anthony Maggio** (00:41:39)

Yeah, so I guess I'll separate those questions. Let's talk about how Airtable uses Airtable first. And we use Airtable extensively throughout the company, not only in the product development space. Within product, we heavily use a lot of the workflows that I demoed at the top of this call. We bring in all of our customer feedback, all of our insights from support, from sales teams. We use it to mine for potential product opportunities, to help with user research aggregations, to help with drafting PRDs. manage our status reporting process so that we always have visibility into what products are launching when, how do they align to big launch moments. It's really the operating system for our product management as a function. But we've actually gone beyond that where we have implemented a rule at the corporate level that any software that we buy, any third-party software, we actually first ask ourselves, why can we not build this on Airtable?

**Anthony Maggio** (00:42:47)

So our procurement team enforces this as a rule. They actually have a process where Anytime someone says, hey, I want to go buy this tool, we have a series of checks first to say, is this a use case that we could support on Airtable? And what's really interesting about that is that it also essentially feeds ideas back to our product team for customers. new capabilities, new kind of platform capabilities, new solutions that we can go, you know, bring to our customers, because it's a great way to expose some of the product gaps or opportunities that we have to really make the platform more powerful. And I actually remember, you know, just like one example of this, when I joined the company about four and a half years ago, we had recently rolled out Workday for our employee review cycles. If you've ever worked in Workday, as probably, you know, many of your listeners have, it is not the most user-friendly tool on the market.

**Anthony Maggio** (00:43:47)

We heard a lot of feedback from, you know, from our teams around some of the challenges around like managing those workflows in Workday. But frankly, at the time, this is four and a half years ago, Airtable, the product just wasn't ready yet to manage that workflow. There was a lot of gaps in terms of multi-layered permissions. You want a manager to see the review content from peer reviews. You have employee ratings and sensitive data in this application. You have routing rules. when can I release peer review content to an individual? Fast forward a couple of years, and actually early last year, we rebuilt this whole process in an Airtable application. So we have an app that runs all of our employee performance reviews. The platform had matured to a point where we said, we can actually now run this end-to-end on Airtable. We have some really great AI features built into this app.

**Anthony Maggio** (00:44:51)

that will actually check for bias, like when managers are writing reviews. It will help managers construct reviews with more specificity and maybe point out when they're being too broad or generic in the reviews that they're writing. So it's a really cool example, I think, of just how this whole process runs end-to-end, where We're looking at our own needs and some of the own needs that come from other departments in terms of how they're thinking about software that they need to manage their function and then using those insights to actually improve the product platform.

**Aakash Gupta** (00:45:28)

Very cool. So you guys are enforcing it at that company level. You're replacing other SaaS with Airtable. That's awesome. And then the second part of the question, what's unique about how Airtable builds product?

**Anthony Maggio** (00:45:41)

Yeah, I think there's a few things. And I love this question. I'd say the two things that really kind of stand out to me about our culture and the culture of the product management team here are first, like our commercial orientation. So, you know, as a horizontal product, we could kind of go after like any number of use cases, any number of different markets. And we really encourage our product team to start with that kind of market and commercial thinking first. We orient our product teams around revenue goals. So each of our product leaders has a revenue number attached to them. So our product leader for self-serve is aligned to our self-serve revenue number. We have a product leader aligned to our touch sales enterprise number and then products that are, you know, more in this sort of zero to one stage where we're looking to kind of get them off the ground and generate, you know, revenue from new offerings.

**Anthony Maggio** (00:46:44)

So, you know, that's one. And I think that that was a somewhat controversial decision at the time that I implemented that and decided that, you know, we really wanted like all of our teams, not only thinking about weekly active users or thinking about like user retention, but, you know, really like directly connected, to the business level impact, which for a SaaS business like us is revenue. And it's been a really positive change that we made. I think there's sort of no clearer way for everyone at every altitude of the organization to know that their products are making an impact than to understand, are we building something that is valuable enough that our users are willing to pay for it or to continue paying us for it? So that's one. And then I think, you know, number two, and this will come as no surprise with our PLG roots is our obsession with the user experience.

**Anthony Maggio** (00:47:41)

You know, given our goal of democratizing software creation, of making these oftentimes like very technical concepts, you know, accessible to a non-technical audience, we have to put a really high level of attention to detail into the design of the product, into the copy, into sort of how we frame these concepts for our user audience. And that's something that really stands out in the culture. We're big believers in prototyping. We're big believers in wireframing. We encourage our PMs to wireframe concepts themselves rather than always relying on designers. We spend a lot of time prototyping and shaping both within Airtable as well as with other third-party tools on the market. Some of the CodeGen tools have been a lot of fun for our teams to play around with as well. But I think that sort of obsession with the delight of the user experience and distilling a technically complex concept of software creation into simple and easy to understand terms is something that's unique about our

**Aakash Gupta** (00:48:48)

culture here. I think if I think about the complaints for revenue goals, the first thing I hear about is that the types of teams that can drive impact dramatically changes. Where if you had teams specifically focused on upper funnel, specifically focused on internal platforms, those teams... have a really hard time showing revenue impact when it comes to the end of the day, especially in sort of a stat sig sort of way. They can always build like a growth model, like, oh, we moved this upper funnel metric, but did we actually move revenue? Same with like platform, like, oh, we built this capability that this team has said they might use. So I think that's like one of the big things I hear. The second thing I hear, Is that PMs feel like, oh, well, I don't actually have control over this. Like, I shipped a great feature, but product marketing didn't enable sales.

**Aakash Gupta** (00:49:38)

Or sales team didn't get the proper training from sales operations. Or... You know, any myriad of other things that could break down that weren't in their control. Customer success never enabled people with it, whatever it might be. You know, there's so many excuses you can come up with. So that's the second thing I hear about revenue goals. And then the third one I hear is that it sometimes shortens the tenure of product leaders because as they don't hit that revenue goal, they get axed. So that's what I hear against those revenue goals. Talk to me about those.

**Anthony Maggio** (00:50:07)

Yeah, I'll talk to you about it individually. So I think the first thing on, oh, there's not always a direct correlation. That is true. There's going to be areas of the product where the goal has to shift a little bit. So for example, we have a large infrastructure pillar. Their goal is not actually driving revenue, it's reducing cost. So again, it's still oriented towards a business level outcome. and something that's important at the company level, but not exactly in the same way. It's kind of looking more at the bottom line versus the top line. That's point number one. I think on point number two, the pushback that Oh, well, there's all these other things that need to happen, right? Like sales enablement needs to happen in the right way. Product marketing needs to happen in the right way. That is true. And that's actually partly why we put this structure into place.

**Anthony Maggio** (00:51:03)

Because what I've seen happen myself, what I hear about from other peers at other companies is that if you don't actually have the PM... thinking about you're thinking full stack thinking like a gm thinking about um how the product is not only going to be built but how it's going to be sold how it's going to be brought to market ensuring that the marketing plans actually make sense for you know the audience that you are targeting with this product then it's really hard to know who has the ball and where are the gaps in this process right And like you said, it's very easy to just point fingers and push blame on product marketing or on enablement or on sales or whatnot. But part of the reason that we actually made this change and that we were excited about this orientation is that the product manager really becomes the overall DRI for success of the product.

**Anthony Maggio** (00:52:01)

And that includes understanding how it's positioned and sold, how it's marketed, whether it's intended to be a self-servable product or a top-down sold product. And if there are challenges or gaps in that, obviously there's escalation paths, there's ways for PMs to say like, hey, this is broken and we need help and we need to pull in a leader from over here to go fix these problems. But it encourages that type of full stack ownership and not just ship the product and then let it be somebody else's problem to figure out how to market it and sell it and whether or not it's successful. And then on point number three, I think we have had Our product managers and product manager leaders have all been quite tenured at Airtable. Actually, two out of the three leaders on my team have been here for multiple years. I think that what I would say to that is that while you have goals, um there's always going to be a understanding of the different sort of sizes and types of bets that you're making and we might not hit all of our goals right we might not hit all of our goals every year but the intention is for us to set ambitious goals aligned to the priorities that the company cares most about if we're not hitting them for some reason it prompts a really good conversation around what's breaking down and you know where are the challenges are the challenges product problems are they sales problems are they You know, marketing and lead generation problems.

**Anthony Maggio** (00:53:33)

And that's really, I think that the biggest value that we get out of that structure is that it always kind of keeps us focused on the end outcome. And we don't just get stuck in the, you know, in the weeds of like, did we ship the feature on time or not?

**Aakash Gupta** (00:53:48)

So let's say I'm a product leader. I'm sold. I want to shift my team over to more ARR goals. I think the next question they're going to ask is how do you guys enforce the measurement on this? Do you have like a product analytics team that needs to make the calls on this or how does that go?

**Anthony Maggio** (00:54:02)

Yeah, we primarily partner with product analytics and finance. So each of our product pillars have a counterpart in product analytics and within our finance team. And that kind of trio, I would say, is the overall tracking and kind of enforcement around how we're doing against our goals in each of those areas.

**Aakash Gupta** (00:54:23)

Okay. And personally for you as a product leader, are you okay with like fuzzier associations to ARR? Like let's say in one of the most used features in Airtable, the subjective experience is way better and the team has done that. Are you okay with just a fuzzier, we think we helped retention or how strict are you with those incremental revenue numbers you want to see?

**Anthony Maggio** (00:54:44)

Yeah, good question. So one thing I should clarify is the altitude at which we set these goals. So for us, it's not actually at the individual like ICPM level. It is at the you can think of it as kind of like the group or pillar level is like where the goals are set. And then a lot of onus is put on the product leaders of those groups to think through, you know, what are the huge bets I'm making? What are the big bets, medium sized bets? You know, where are the kind of different altitudes of initiatives that I'm going to put in place to help my group like hit these goals? At the higher altitude level, I'd say the tracking is pretty clear. If we're not hitting our self-serve revenue numbers, that's fairly unambiguous. At the lower altitude, it can be slightly fuzzier, but there's still pretty good orientation around hey, we're going to go build this new product or we're going to go build this new feature.

**Anthony Maggio** (00:55:46)

We set some expectations around what we think it's going to do to our activation rate or our upgrade rate or how it's going to better help us retain users. And then those things are pretty measurable. So we can understand and assess, was our hypothesis off? Were we just way off in our analysis or our our expectations of this product and it gets broken down into more grokkable altitudes that we can access against.

**Aakash Gupta** (00:56:19)

Awesome. Makes a lot of sense because I personally had been in the situation where I was the director and we were crushing, you know, like our actual overall number. And we were succeeding in our product metrics, but it seemed like we couldn't attribute anything to the incremental ARR and we got really dinged for that. So I like your approach. I think that's my example is the cautionary thing that could happen if you don't implement it like Anthony just explained. So that's really good. Then the second thing you said that's unique about how you guys build product is you guys are actually having PMs in the pixels. And thank God for that. I'm so happy to hear somebody talk about that because every time I bring this up, I'll get pushback from folks like, oh, designers need to be in the loop, et cetera. So talk to me a little bit about how you empower PMs and how PM and designers work together to allow PMs to actually get into prototyping and mockups and those types of things.

**Anthony Maggio** (00:57:13)

Yeah, I think, you know, again, it's a collaboration, right? Obviously, our PMs are not spending 100% of their day, right, designing and wireframing and prototyping. It's a team sport in that front. But I think what's really important is encouraging PMs to come with hypotheses, with product thinking, with ideas that they're gleaning from other products that are on the market, especially right now with AI products and AI product development. There's so much changing so quickly. The technical capabilities of what you can bring into any product that you are developing is literally changing on a week by week basis right now, right? And so, you know, what I think is really important about that is that the role and the responsibility like really rests on the PM to say, what are the models capable of? What new magical offerings or solutions or experiences can we bring to our customers with these models?

**Anthony Maggio** (00:58:18)

And then what is the fastest path to go from idea of what we could do into a tractable prototype or experience or at least kind of a wireframe that we can look at and kind of understand how this product could start to take shape. And so that's really like the level of prototyping that we encourage from PMs. Once we decide, hey, there's a lot of meat behind this. This is an idea we're really excited about. We want to go, you know, build this as a product. We're going to staff a team around it. We're going to have a designer who's attached to that product as well and is thinking through all of the, you know, additional kind of UX patterns and look and feel and UI around the product. To be very clear, we have an excellent design team and they drive a lot of that work.

**Anthony Maggio** (00:59:12)

But I think what I've seen both in prior chapters of my time at Airtable and at other companies was a feeling like, hey, PMs shouldn't touch the design or shouldn't touch the user experience. And that's something that we've really tried to consciously break out of.

**Aakash Gupta** (00:59:29)

Yeah, I think they have to if they want to have success. Otherwise, they just get so removed. So I love how you clarified that. And that was actually going to be my next question is, how do you guys handle the process of roadmap planning? You talked a little bit about there's this PM discovery phase, then we might actually staff the project. How do you guys decide, okay, we're going to staff the project? Do you guys do a quarterly roadmap? How do you guys handle all of that?

**Anthony Maggio** (00:59:52)

Yeah, it's evolved over time. I'd say where we are right now is we predominantly plan at the half. So at the half, we have our big moments to come together as the company, to think about our big launch moments and the external story we want to be able to tell to the market. We typically have two big launches a year, like a spring launch and a fall launch. Our bigger bets and initiatives are lined up against those launches. And then the quarterly planning happens more at our product pillar altitude, where each of those product leaders that I mentioned are driving the localized priorities around some of their specific revenue goals, some of their specific initiatives, the multi-quarter kind of bigger bets that they're going to make as a team. And those are typically done on a quarterly cadence, which just gives us enough flexibility in between the year to say, Hey, we really want to accelerate this one particular product or initiative, or we want to maybe take the foot off the gas on something else that's not showing quite as much promise as we initially thought it would.

**Anthony Maggio** (01:01:00)

So that's worked for us in terms of giving us the kind of two big... big impact moments to get everybody around the table, like aligned on the strategy, aligned on the big things, and then provide enough flexibility to adjust the plan throughout the year as we gain new insights and gain market feedback and gain data from the products that we're putting out there.

**Aakash Gupta** (01:01:23)

So in 17 years, you have become VP of product at a Decacorn company, $12 billion company, pretty crazy. If you had to go back and give yourself advice at the beginning of the journey, what advice would you give yourself?

**Anthony Maggio** (01:01:39)

That's a really great question. I think the advice, you know, I'd say that I've had so many learnings like at every stage of my career. And I think the one consistent theme is that I've been, I've always just been motivated by where is there going to be the highest opportunity for learning. So as I think about like each of the jumps that I made, I started out in consulting. I felt like I just, I got a picture of sort of how big, really big companies plan and execute and drive initiatives. But I felt like my personal rate of learning just wasn't fast enough. And I very quickly jumped into early stage startups. I was at Jet Setter, which was a spinoff of Guilt Group back in 2010, 2011 timeframe. From there, I had a great experience learning about the early stages, zero to one, product market fit finding of building new products.

**Anthony Maggio** (01:02:43)

I loved that and wanted to keep doing it and went and started a company with a couple of co-founders building enterprise software in the hospitality industry. Um, and there, you know, learned a ton as well and felt like I got exposure to, um, you know, what it looks like to not only like build a product, but how to think about sales and distribution and like a multi buyer, um, sales process selling into, uh, into hotel chains with CIOs and, you know, general managers and different constituents that you had to build for. Um, so I think, you kind of through line has always been like, how do I really challenge myself to do something that I have not done before? And to make kind of each chapter of the career intentionally a high velocity learning experience.

**Aakash Gupta** (01:03:34)

And I'm sure you help a lot of people who want to make those quick jumps in their career. They want to go from PM, especially I'm seeing a lot of people struggle right now with like the senior IC to director or group level jump. And then similarly from the like director group level jump to the VP jump. A lot of people are kind of stuck at those points. How did you break through those?

**Anthony Maggio** (01:03:56)

Yeah, it's a good question. And I think there's always some, you know, timing, like factors involved in those things. And like, where is there a need in the organization? So it's hard to give a one size fits all answer to that. But what I would say, like at the, you know, kind of group to director level jump, and I think that is probably actually probably one of the biggest like jumps that I see in and hear about, like from folks who are in this role. is going from like individual contributions and individual thinking to how do I actually kind of get high output and high quality product thinking from a group of people, right? Like from my team. And that's a big jump, right? You have to go from like, I know how to build like great products myself. I know how to think about the product experience and the commercials and the quality of, To how do I actually train and coach like other people to to do that?

**Anthony Maggio** (01:04:58)

So, you know, typically the like the advice that like I give to other folks who are maybe in that boat but don't yet have. a team to manage is like, can you start practicing by like mentoring others in the, in the team or in the company, like take somebody literally under your wing and help them be more successful, um, and to go help them like figure out some kind of area of the product that they're struggling with or having challenges with on, on your own. I think, you know, not only do you start to build that skillset, but just, it shows the initiative and the company first, you know, thinking that. um, will often be considered in a, you know, in a promotion to, to a director level. Um, so, and then from the second, you know, the second one, like director to VP, at least like the way that I think about that is, um, you know, how do you start going from driving like really high quality results and execution, um, to actually starting to shift like the thinking or direction of the company.

**Anthony Maggio** (01:05:57)

So, you know, that's where the expectation becomes not only that you can, run a big area of the business and come up with great ideas within your own part of the business, but actually to maybe tap into new markets, to build new products, to uncover opportunities and pitch opportunities that are not yet top of mind for the business. You have lots of practice and lots of at bats at that. Obviously, you know, being a PM is being constantly on the search for product market fit. But I think that at the director level, as you start to get more of that kind of forest from the trees view, there's even more of an expectation to be able to, you know, cultivate, validate and really kind of bring those like bigger needle moving ideas to the rest of the business.

**Aakash Gupta** (01:06:44)

Those really resonate with my experience. I mean, as a director, like how much you build up other people is so key. And then as a VP, how you impact other functions, right? It's not just product, but design, engineering, analytics, all these related fields, you want to be shifting kind of the strategic direction. So we talked about your awesome culture that you've built at Airtable. We've talked about the highs of building these projects. Obviously the PM job and especially the VP of product job, it isn't all highs. I'm curious, can you talk to us maybe about your lowest point since being a VP of product?

**Anthony Maggio** (01:07:22)

Yeah, that's a hard question. I don't have one specific low point that comes to mind. But I think that one thing that I think about regularly is that the number of peers that you have in your function starts to shrink as you move up in the organization. So if you're an ICPM, You have dozens of other people who are in the same boat. As you're a director, you have maybe fewer people who are in the same boat. And then as you get into VP level, you are essentially a team of one for your function. Your first team becomes your partners, your engineering partner, your design partner, your product marketing and sales partner. But I think that that is, you know, that's probably like the biggest challenge area is not having, you know, the same sort of peer support group who has your company context, who has, you know, your product context that you can really kind of lean on, you know, on a day to day basis.

**Anthony Maggio** (01:08:28)

And so personally, that's an area where I've really invested in keeping up with my network. maintaining ties with other product leaders at similarly staged companies. I have a great coach who I work with. All of our leadership team at Airtable works with professional coaches who kind of help us think through both our own personal and work-related challenges and help to grow us as leaders. So yeah, I'd say it's probably less of one one particular low moment and more, I'm always thinking about that back of your head, kind of shrinking network of peers who are there to support you in the day-to-day.

**Aakash Gupta** (01:09:16)

Yeah, I definitely felt that. And then I'm curious, we talked a lot about AI features that were working, but having built a lot of AI features, I know that they go in fits and starts. Sometimes you release something, it's not reliable. Sometimes you release something and it's just the models change. There's so many things that can happen. There's so much stochasticity. Can you talk to us a little bit about that? Maybe some struggles you had with AI features and how you evolved them to respond?

**Anthony Maggio** (01:09:42)

So building products with AI, I think, has really changed, honestly, the way that we do product development at Airtable. I think that the process has evolved to be a much less linear process where Historically, you could start out with a PRD, you had a pretty good idea of what you wanted to build, what the sort of technical capabilities were going to be around that product, maybe some kind of open questions around the design that you needed to sort out or think through. Typically, I think before we were building with LOMs, the process was pretty tractable. If you pulled an engineer or a designer into your early brainstorming and PRD writing, you could pretty quickly get the shape of what your product might turn into. I think that's totally changed with AI. There's now this first phase that really becomes, what can we get out of the models?

**Anthony Maggio** (01:10:46)

How far can we push the edges of the latest AI models? And where do we get the highest quality, the most consistency, the most reliability in the experiences that we want to create? And a lot of times that's just not known upfront. You know, like if you look at the example of the assistant that we walked through today, you know, when we started working on this initiative a few months ago, like we just really did not know if we were going to be able to consistently get the quality of responses that we, you know, would meet our bar for shipping this to users with the models that were available at that time. Right. And especially, you know, you know, as Airtable, as like a totally horizontal product, like we want this assistant to work on anybody's data structure, on any set of, you know, tables, on any set data sets that you're bringing into the product.

**Anthony Maggio** (01:11:41)

It's not like we can go fine tune an assistant and, you know, tell it, hey, like you're always looking at a, you know, support ticket database. So use that context when giving your responses, right? So there was actually a lot of shaping that had to go into, a product like that, a lot of playing with different data sets, a lot of understanding, do we need to make product changes to give enough context to the model or to the agent in this case that it can actually go and develop a great plan for answering this question? There's a lot of trial and error. We would get initial prototypes and say, hey, this isn't quite working well for certain use cases. you know, maybe we need to do, maybe we need to take some like actual new approaches in terms of, you know, how we like feed in the right level of instruction and context to achieve this.

**Anthony Maggio** (01:12:35)

So I think it's really totally changed, you know, the way that we build products. It pushes a lot more onus onto that upfront, like prototyping, dogfooding, and really kind of getting hands-on to understand where the edges are of what's possible in a way that just never existed to the same extent. We've always been big on dogfooding, we've always been big on prototyping, but I think the urgency of it when building AI products is just a completely different league.

**Aakash Gupta** (01:13:09)

Really resonates with my experience. Anthony Maggio, thank you so much for being here.

**Anthony Maggio** (01:13:15)

Thank you for having me. It was a really fun conversation and hope to chat again soon.

**Aakash Gupta** (01:13:45)

See you later.
