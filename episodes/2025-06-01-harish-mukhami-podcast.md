---
title: "We Built an AI Employee in 62 mins (Cursor, ChatGPT, Gibson, Crew AI)"
subtitle: "Harish Mukhami demoes how to build a production-ready AI CS agent that analyzes data, recommends actions, and executes tasks in less time than a typical product review takes"
date: "2025-06-01"
host: "Aakash Gupta"
guests: ["Harish Mukhami"]
speaker_names: "substack"
substack_url: "https://www.news.aakashg.com/p/harish-mukhami-podcast"
youtube_url: "https://www.youtube.com/watch?v=Uhs_p-Is0lo"
duration: "01:02:03"
word_count: 9194
source: "Substack episode transcript (aired audio)"
sponsors:
  - name: "Linear"
    url: "https://linear.app/partners/aakash"
  - name: "Maven"
    url: "http://maven.com/x/aakash"
---

**Sponsors:** This episode is brought to you by [Linear](https://linear.app/partners/aakash) and [Maven](http://maven.com/x/aakash).

# We Built an AI Employee in 62 mins (Cursor, ChatGPT, Gibson, Crew AI)

*Harish Mukhami demoes how to build a production-ready AI CS agent that analyzes data, recommends actions, and executes tasks in less time than a typical product review takes*

**Harish Mukhami** (00:00:00)

Today, we'll be building an AI customer success agent, which is going to solve problems for you without any humans involved. We're going to be using Gibson AI database for database backend. We'll be using Cursor on Cloud Sonnet 3.7 for coding. And finally, we'll be using Crew AI framework for AI agents. We're building this in three parts. So part one, we'll build a SaaS-style dashboard app to provide insights and recommend actions. Part two, we'll add AI agents to analyze these insights and recommend actions. Part three, we'll actually make this agent autonomous and take actions on users' behalf. This is the dashboard. This is a result of part one. This is the customer success AI agent dashboard only. So we're focusing on all the way from design, development, deployment, management, and scaling of databases, So when we started building in Gibson, we used a web interface. Now we're actually building tables right from cursor ID and deploying the database.

**Harish Mukhami** (00:00:54)

You're not building a prototype anymore. So you are backed by a very significant production grade database. It's already deployed in the crowd. So you publish this and you get 10,000 users tomorrow. What other AI employees could people create? sdrs are a very popular use case there is also meeting preparation agent executive assistant you can chain together all of these agents to to create a specific role that is tailored for you

**Aakash Gupta** (00:01:22)

Really quickly, I think a crazy stat is that more than 50% of you listening are not subscribed. If you can subscribe on YouTube, follow on Apple or Spotify podcasts, my commitment to you is that we'll continue to make this content better and better. And now on to today's episode. All right, Harish, welcome to the podcast. What are we going to be doing today?

**Harish Mukhami** (00:01:46)

Yeah, today we'll be building an AI customer success agent, which is going to solve problems for you without any humans involved. All right, let's just get into it. Yeah. Let me share my screen. So we're going to be using four tools today. We're going to be using OpenAI 03 mini for planning. We're going to be using Gibson AI database for database backend. I can do a quick intro of what Gibson is. Gibson is a AI powered cloud database. You can build, deploy, and manage your database at lightning speed. So it forms the database backend. And we'll be using cursor on Cloud Sonnet 3.7 for coding. And finally, we'll be using crew AI framework for AI agents. So that's the tech stack that we'll be using today. So we can go on and start building.

**Aakash Gupta** (00:02:37)

Let's

**Harish Mukhami** (00:02:37)

do it. So how are we building this? We're building this in three parts. So part one, we'll build a SaaS-style dashboard app to provide insights and recommend actions. So this is something that most of us are really familiar with, which is a dashboard with metrics and insights, which we have been using for a while now. Part two, we'll add AI agents to analyze these insights and recommend actions. essentially automating out the first part. So now AI agents will be looking at the dashboard, looking at the data and analyzing the data, identifying churn and mitigation reasons and providing actions to users who can approve or take those actions. So this is like a part two is the human in the loop with an AI agent. Part three, we'll actually make this agent autonomous and take actions on users' behalf. So at the end of it, we'll have a fully functional AI agent for customer success.

**Harish Mukhami** (00:03:36)

So let's dive into part one. So for part one, we'll start with planning phase. So we know that we want to build a dashboard for AI customer success agent. how exactly dashboards should be, what metrics should we focus on. So we're going to ask ChatGPT, in this case, O3 Mini, to provide us some guidance here. So I have a quick prompt ready to go. So I'm going to copy-paste this here. Fairly straightforward prompt. Act as a business intelligent expert to design a comprehensive dashboard for bulk trade. That is the company that we're focusing on. A B2B e-commerce platform. You can imagine this could be for any other business, but today we're going to focus on the B2B e-commerce. As a customer success manager, I need dashboard that integrates data from our CRM. In this case, we're using HubSpot. Google Analytics are an application database. The goal is to empower a customer success team with actionable insights that will optimize customer funnel, improve engagement, retention, reduce churn.

**Harish Mukhami** (00:04:37)

Please provide a dashboard with four tabs, sidebar needed to ensure that we achieve goals. I'm spelling this out because this is the one that kicks off everything in motion.

**Aakash Gupta** (00:04:47)

Okay.

**Harish Mukhami** (00:04:49)

I'm going to ask this and wait for using it in reasoning mode. So it came back with pretty quickly came back with a few recommendations here. So funnel performance, engagement and usage, customer health risk, retention insurance. So four tabs like we asked based on what the goals are here.

**Aakash Gupta** (00:05:14)

So why did we use O3 Mini Reasoning mode?

**Harish Mukhami** (00:05:18)

So of all the models that I've used, I found O3 Mini is great for planning, especially it's much faster. So it has worked out well for me so far. For coding, I use Claude Sonnet. That has been the king, I guess, for the past year or so. So those are the two models that we're going to be using today.

**Aakash Gupta** (00:05:39)

Sounds good.

**Harish Mukhami** (00:05:41)

So now we have the dashboard design. The second and even more important thing to focus on is what is the makeup of your database that is powering your dashboard? So I'm going to just ask O3 to tell us what data should we use? What are some of the components here? So what data powers this dashboards?

**Aakash Gupta** (00:06:09)

So now it's thinking about it and helping us plan what data inputs we'll need to create.

**Harish Mukhami** (00:06:15)

Exactly. So it is funnel performance, engagement and usage. So one of the things it just did was it did exactly like the dashboard organization. So it gave for each dashboard, these are all the data fields that you need. What I do want to ask is like organize this by data source instead of tabs.

**Aakash Gupta** (00:06:43)

Makes sense.

**Harish Mukhami** (00:06:50)

So now we have a much more specific response around like, hey, from HubSpot, these are the fields that you need. I'm going to copy paste this whole thing.

**Aakash Gupta** (00:07:02)

It's very much like a data definition.

**Harish Mukhami** (00:07:06)

Exactly. I guess you don't even have to have this specificity from a database perspective. You got a bunch of these. So I'm going to copy this, and then we'll go to Gibson and model this database.

**Aakash Gupta** (00:07:27)

Okay. And so what role is Gibson playing here?

**Harish Mukhami** (00:07:32)

So Gibson is the database that is powering this entire application. So first step when we're building the dashboard, the front end is actually looking into the Gibson AI database to show that data in the front of the dashboard. One of the cool things about Gibson is it's an AI-powered cloud database. So you could imagine if you want to build this analytical backend for like a customer success dashboard, you need to have a database that is easily scalable, can ingest data from multiple sources and handle like hundreds of thousands of transactions, if not millions. Gibson can autoscale with that. So that's why I picked this.

**Aakash Gupta** (00:08:14)

Okay.

**Harish Mukhami** (00:08:16)

So let's go to Gibson. So Gibson is available on the web or it's also available in your favorite tools via NCP server. So we're going to see both. So I'm going to start off with the web version of the Gibson AI platform. So I'm just going to sign in. It's free to get started. Anybody can join. You can use your Google Auth or log in with your email. I'm just going to use my email to join in. And then this is the Gibson AI workspace. The first thing I'm going to do is type in build me a database for B2B e-commerce customer success agent. So I'm just going to type and provide a simple prompt. This is not the actual prompt that is going to build the database, but initializes the project and sets the context on what the user wants to build.

**Aakash Gupta** (00:09:19)

That's our high-level goal. And then we're going to come in with the data definition later, I assume, from O3 Mini?

**Harish Mukhami** (00:09:24)

Yep, absolutely. So the one we copy-pasted, I massage this a little bit to make sure that it's a little bit more cleaner. We're still going to have those three components to it. Here is your project window. So these are all the projects that you're working on. They show up on the left side. So the first step is it initialized your B2B e-commerce customer success agent, and it gives you two options. I can either design and generate the entire data model for you at once, or you can build a data model step by step. So you would choose an option one. If you weren't using O3 Mini, you're just asking it to like, and you can work with it to design and brainstorm. Since we have already planned in O3 Mini, so I'm going to go choose the option two here.

<!-- sponsor -->
**Aakash Gupta** (00:10:13)

Today's episode is brought to you by Amplitude. Building great digital products is hard. You know that better than anyone. Getting teams aligned, measuring what matters, and scaling your product strategy isn't easy. But what if you had a clear framework to guide your next steps? That's exactly what Amplitude built. They studied the best product teams to understand what really drives impact. And turned those insights into the Digital Experience Maturity Assessment. in two minutes you'll be able to see where your team stands and what you can improve to build better products faster click the link in the caption to take the free assessment and get a clear path to product growth hey let me take a quick break to talk about something that's completely changed my product management workflow linear as a pm i was drowning in tools one for planning another for issue tracking roadmaps and sheets and jumping between slack intercom and app reviews just to piece together customer feedback sound familiar I was spending more time So option two says we can build the data model step-by-step as we see fit.

**Harish Mukhami** (00:11:45)

Exactly. And here, the goal is we're more directional and targeted about what we want Gibson to build. It does give you some options, but since we already have it, I'm just going to copy-paste that. So...

**Aakash Gupta** (00:12:03)

And do you have several models working in the back end here? What is powering this experience? Yep.

**Harish Mukhami** (00:12:10)

We use both Anthropic as well as OpenAI. So we actually use Anthropic for writing the code and OpenAI for actually planning and infrastructure management. So both of those are available. This is the crux of what Gibson does since we're building data model from scratch. So this takes about a minute or so because it's a pretty significant prompt. So while it is building, I actually want to walk through pretty quickly what are all are there on the workspace. Sounds good. So while it is doing the data model and schema design, when Gibson is done, you'll get a complete data model schema back, and then it is represented in an ER diagram here. That's the first thing. The second would be a schema. So schema would be your Python code in a schema format. And then if you like that data model that you have designed with Gibson, and then if you want to deploy it, you just hit deploy.

**Harish Mukhami** (00:13:14)

So when you hit deploy, we're going to take this schema and data model and deploy it in our AWS instance. It's a secure, scalable cloud infrastructure that we have made it available for users to use. So at the end of it, so it's done. It built out what you asked, and then it comes back with like a pretty specific response around like, hey, I built this following three modules, CRM, analytics, transactional data module. So let's go quickly look into, this is the ER diagram. So on the CRM side, contact information, feedback, profile. So very cleanly written out with the data types. ID is your key. And then it has some annotations around what the data model is and what are some of the constraints here. Very cool. Second is the schema. So like I mentioned, schema is actually the code representation of what the data model is.

**Harish Mukhami** (00:14:14)

From here on out, you can actually ask Gibson to do anything. It can explain you anything. It can be your pair data model or database agent. So one of the things that we're going to be doing is we're going to be ingesting some test data into it. So what I'm going to ask Gibson to do is to remove all the enums because it becomes challenging to insert test data. So please remove enums. from all the tables. And for people who don't know, what are enums? Enums are enumeration. So when you are defining fields on a table, there comes many different data types. Enums is one of the data types and which locks in very specific values like 0, 1, 2, 3. For example, if a customer is... a lead, a customer or churned or any of those, those becomes like 0, 1, 2, 3. So, oh, there are no enums data available.

**Harish Mukhami** (00:15:16)

So all of them are text. So we don't have to worry about that. So typically I just run that, but we don't have any enums in this data model. So we're good.

**Aakash Gupta** (00:15:24)

Okay.

**Harish Mukhami** (00:15:27)

A couple other things. So once we deploy, I'm just going to hit deploy here. It's going to go take this data model and deploy it in the cloud. And then as soon as it is done, it's going to give you two environments. One is development environment. Another is production environment. So automatically provisions two environments for you to develop, test, and then if you like your data model, then you can promote it to production. So Click on View API, so it's going to show you your entire APIs that are backed by this database. So within under three minutes, you have this entire CRUD layer available for you. So you got the entire database accessed through this CRUD layer. So this is your API. And

**Aakash Gupta** (00:16:19)

a CRUD

**Harish Mukhami** (00:16:20)

layer is... create, read, update, delete. So those are the operations that you can perform in the database via the... Get,

**Aakash Gupta** (00:16:30)

post, delete type commands. Exactly.

**Harish Mukhami** (00:16:36)

I'm going to quickly show you the settings. In settings, you have both the dev and production, and these are the API keys. I'm going to delete this later, so it's okay.

**Aakash Gupta** (00:16:47)

Who's

**Harish Mukhami** (00:16:48)

watching? And then if you want to direct access this, so if you don't want to use the database and you don't want to use the APIs, you also have the opportunity to directly take this connection string, copy-paste it, and then access the database here. Okay. we have the data model built out. So what we can do now, now that we have the data model, let me see if there's anything else I want to show. I think we're good. We can go to cursor and then we can ask cursor to build a dashboard based on this data model. Exciting. So let me share my cursor window here. So here we are in cursor. So the first thing you see is how we have connected Gibson to cursor. Gibson connects to cursor or any other dev tool via MCP. What is MCP real quick? MCP stands for model context protocol.

**Harish Mukhami** (00:17:47)

It's an open standard designed to connect AI models to your tools, your data sources. MCP makes it easy for tools to integrate with LLNs and vice versa. So this has been like a really game changer for us. Like even while we're doing this evolution with Gibson, now with MCP, it's so seamless. Everything is so seamless on how we interact. How do you integrate Gibson with cursor? It's a very simple command. So just four lines, Gibson is in cursor now. What I'm going to do is I'm going to just go and show you... I'm wondering, like, what can I do in Gibson from Cursor? What are some of the tools available? So I'm just going to ask, like, what tools are available via Gibson MCP server? So it's going to tell us, like, what are all the capabilities that we have available in the IDE. The cool thing about this is developers don't have to leave their environment.

**Harish Mukhami** (00:18:46)

And without leaving, they can actually do project management, create, get, update project, schema management. get all the schemas, do the data modeling, deploy the databases. And one, this is my personal favorite, you can actually run natural language queries on your database from here and it can return the results. So literally text to SQL with like curated results back to you. So those are all the tools that are available here. First thing we're going to do since our database doesn't have data yet is I'm going to ask cursor to generate test data. Please generate test data. Oh, I need to do one quick thing. So I need to rename the database so that it's not confusing because since we have many projects here. Okay. I'll just do it in the Gibson end. So I've just renamed the project here to CSA DB1 so that it's, since I have plenty of projects here.

**Harish Mukhami** (00:19:55)

So let me quickly make sure that took into effect. And then I will ask cursor to generate test data. There are a couple of things I said. I'm very specific about using API calls and then also honor relationships between the underlying tables because we have a bunch of tables here. So yeah. I'm just going to say use APIs and specifically create a Python script for this.

**Aakash Gupta** (00:20:20)

Okay.

**Harish Mukhami** (00:20:23)

So if you see here, so it's actually going to Gibson and then getting the project information. So this is how cursor has the context of whatever we have built in some third-party infrastructure.

**Aakash Gupta** (00:20:36)

Got it. And as far as the MCP connection that we were covering, what was the steps involved to do that?

**Harish Mukhami** (00:20:43)

So first step is actually you need to authenticate that you're an authenticated user of Gibson. So we have a blog post out there on our website that shows like it's what first step. The second would be just taking those four lines, going to cursor settings, clicking here, and then this opens up this tab, and then you go to MCP, and then you just add a new MCP server. Okay. So if you see on the conversation window, cursor is actually getting all the API information. So now it knows the context. Now it can go create a Python script for us. So it's going to go generate some test data for the dashboard.

**Aakash Gupta** (00:21:27)

Oh, God. And behind the scenes, Cursor is probably thinking about what might be good test data to make this dashboard look good. Then it's going to be adding that into the databases that were provisioned by Gibson.

**Harish Mukhami** (00:21:42)

Absolutely, yeah. Okay. I think one of the key things we should probably make sure that when we do test data insertion is make sure that we've mentioned realistic. Otherwise, it just pushes in some data that is not necessarily doesn't make sense.

**Aakash Gupta** (00:22:01)

Okay.

**Harish Mukhami** (00:22:04)

It does take a couple seconds to do this.

**Aakash Gupta** (00:22:08)

Okay. Okay. So here at the moment, cursor is building the test data?

**Harish Mukhami** (00:22:15)

Yeah, building the script for the test data. So we're going to run that script. Gibson also has the ability to generate test data. So we can just ask the query tool. I'm like, hey, go generate test data. But I wanted to create a Python script because it's repeatable and then we can execute it pretty quickly. Okay, got it. While it's doing that, I also want to show you a couple of things. One is the model selection. So I'm using the Cloud Son at 3.7. And then the second is I'm also using thinking mode. So for some reason, I found the thinking mode delivers better results. So a couple of things I found while working with cursor.

**Aakash Gupta** (00:22:56)

OK. And is that probably the most expensive model you can use? I think the

**Harish Mukhami** (00:23:04)

3.7 max is, and it's actually an extra cost to it. I know, I mean, nowadays I think it was 4.1, GPT 4.1, OpenAI 4.1. Sounds like that seems to be pretty good at coding as well. So the foundational model coding race is on.

**Aakash Gupta** (00:23:26)

Yeah. By the time this episode airs, I'm sure somebody will have released another one.

**Harish Mukhami** (00:23:33)

I think there's new models coming out today. Anyway, so we're done. Competence of Python script that generates realistic text data, so data is ready. So in the interest of time, let's go ahead, accept it, and then look at the readme. What does it say? Okay, we have to install Faker. So let me do that quickly. And how did you know we needed to install something? I went to the readme. So cursor generated a readme. I clicked on the readme file, and then it says these are the couple of steps that you have to use to run this.

**Aakash Gupta** (00:24:22)

And cursor, unlike the AI prototyping tools that a lot of people are probably used to, this isn't happening on a virtual machine. This is happening on your machine. So you installed that thing on your machine.

**Harish Mukhami** (00:24:31)

Absolutely. Though there's an option for you to create a virtual environment. So UV, V, and V. And we're going to do that too today when we're running the AI agents. And it's going to go. So now it's using that gives an API to generate this data as you see it go through the terminal. But you're right. I think Cursor does that. I definitely prefer Cursor because it gives me more control over what I'm building. Though you are responsible for infrastructure, that's why Gibson takes care of the back end here. Okay. So it'll go through and insert that data. What we're going to do next is now that cursor has inserted test data, I'm going to go ahead and I'm going to say, now that we have the data, let's go build a dashboard. And I'll walk through the prompt here. I'm being very specific on what packages to use.

**Harish Mukhami** (00:25:37)

So build a modern, sleek, and interactive dashboard based on the Gibson AI project. Use the APIs to power the dashboard. Don't use mock data. So sometimes cursor ends up showing a dashboard, but there's mock data behind it. So get API information. And then I'm being very specific about use Next.js and chat scene for UI components for dashboarding. So that's the instruction. What to build, I'm going to go to the chat GPT and what it has given us from a guidance perspective for the dashboard and just copy paste it just to keep things simple here. So I copy this and then I'm going to go copy-paste this from GPT. So this is, hang on, this is exactly what we got. And then, so if you look at this, it's essentially Let me actually share the screen as well so that you can see where I'm copying this from.

**Harish Mukhami** (00:26:42)

So I just took and copied this whole thing. We asked a question, and then we got the dashboard, and then we're just going to copy-paste this into cursor here. Okay, still, it's definitely creating a pretty hefty data set for us.

**Aakash Gupta** (00:26:56)

So at the moment, the Python script is inserting the data?

**Harish Mukhami** (00:27:00)

Yep. Okay. We can open a new, actually we can open a new cursor window while it is doing it so that we can do this in parallel. Okay. So let me open up a new window here. Let's start a fresh project here. And then I'm just going to do this. So I'm going to, it's more clear to read. So what we talked about below is overview of the dashboard in this four primary site tab. So I'm just going to do a send. So since it's a pretty significant prompt, there are a few things that Cursor is going to do. Since we are using Cloud 3.7 in a thinking mode, it reasons pretty good. So while we're wipe coding, we can actually watch how it's thinking. I like to do that and maybe learn a thing or two while it's doing it. Yeah. Yeah. One of the things that it asks here is installation of some packages here.

**Harish Mukhami** (00:28:05)

So would you like your code inside a source directory? Yes. Yes. Would you like a TurboPack? Yes. Customize the import alias, no. And then it goes, the first step is installing the dependencies for Next.js. I'm using Next.js with ChatZen because it looks nice. We can just use Python. It's much faster, but it may not be visually appealing.

**Aakash Gupta** (00:28:28)

Okay.

**Harish Mukhami** (00:28:29)

This whole thing takes about 10, 15 minutes. I obviously have a completed project that we can show because it does take a bit to completely do this. Okay. We'll go through a few steps, and once it's running, we can go and look at the first step finished product.

**Aakash Gupta** (00:28:48)

Sounds good.

**Harish Mukhami** (00:28:50)

We're still at the installation phase, package installation phase.

**Aakash Gupta** (00:28:55)

Getting set up. So it's

**Harish Mukhami** (00:28:56)

done now. Now it's creating the project structure.

**Aakash Gupta** (00:28:59)

Okay.

**Harish Mukhami** (00:29:00)

So this is the step where it's creating the sidebar components. By the way, we're using the agent mode here. Cursor has a few multiple modes. So ASCII is more, acts as a co-pilot. Agent is agentic workflows where it goes through and then builds this, builds a product to the final prompt and then automatically resolves those errors and issues as they come up.

**Aakash Gupta** (00:29:24)

Do you normally spend most of your time in agent mode?

**Harish Mukhami** (00:29:29)

I use Ask Mode quite a bit for the purpose of one-shotting quick apps. Like Vibe Coding is Agent Mode is pretty well. So I've used all the other tools too, like Replit and Bolt and Lovable and all of that. Cursor is the thing that I like the most so far.

**Aakash Gupta** (00:29:52)

It's the most powerful and

**Harish Mukhami** (00:29:54)

Yeah, it is the most powerful. So let's go look at once it executes, I can actually show the end state in the interest of time. We got a few other things to show through. So it does take a while to go through this.

**Aakash Gupta** (00:30:11)

Oh, God. To help you out, I've put together a collection of courses I recommend at maven.com slash x slash Akash. This includes courses like AI prototyping for PMs, product sense for PMs, and getting an AI PM certification. Visit it now at maven.com slash x slash A-A-K-A-S-H. We're putting it in the oven and magically it's going to come out of the oven baked.

**Harish Mukhami** (00:31:07)

Yeah. Let's do this. Let me share. So this is what we get once that session is done. This is the dashboard. This is a result of part one. This is the customer success AI agent dashboard only. We have the four tabs that we asked for. So customer analytics. It talks about your overall customer view, how they're doing from a revenue perspective over time, customer segments, top 10 customers. Click on customer funnel. It's more fancy charts around conversion rates through the funnel. engagement and retention, user engagement metrics, NPS, active users, retention rate, average users, feature adoption. Again, all of this is coming from test data. You can obviously have your live data connected to it. Last piece is a churn risk. So we do have a table that defines what is a churn risk, how many customers are at high churn risk. Now, all these we're pretty familiar with.

**Harish Mukhami** (00:32:20)

What is the next step in terms of looking at this dashboard if you're a customer success agent? Now you have to interpret this data and then understand, analyze, gain insights, and then take actions. That's the key part of this. So for that, the onus is on customer success agent to do that. So in this case, what we want to do is we want to write an agent that is going to actually do that for you. So at the end of it, if you come back to the dashboard, there are actions available for you that you can take as a human in the loop. Yeah. this is the conclusion of part one of dashboard. And then we can go on to building actually the first set of agents, which are going to analyze the data and then take actions for you.

**Aakash Gupta** (00:33:10)

So what we've built so far is, It has built all of these charts via code. So it's not using a BI tool or anything like that. And it's created as a live website that you could theoretically hook up into your database so that you would already have these dashboards. So that's step one, the insights that a customer success agent might develop. Now we're going to take action on those? Yep, absolutely. All right.

**Harish Mukhami** (00:33:35)

I mean, the barrier to build is so low that I feel like, how did we not have this two, three years ago? I wish I had this a few years ago. So let's move on to building the AI agents that analyze the data and recommend actions. So in this case, a human either approves or takes actions based on agent recommendations. This is like the human in the loop use case. So First thing we're going to do is we're going to go back to cursor and ask Gibson via MCP to add an agent action table to the schema. So what we did was we built this dashboard. Now we need to store those agents. So whatever the agents are doing, we need to store that. So we're going to ask Gibson. cursor to do that. And this is where you have the MCP integration with cursor using Gibson.

**Harish Mukhami** (00:34:26)

And then we're going to do that right from the cursor workflows. So let me share my cursor screen here. So here, what I'm going to tell the agent to do here, create a table in this database called agent actions with the following fields, customer account name, contact email, contact person, industry, churn risk, churn reason, action message. So essentially, this is where the agent can write those actions for users to take and approve from the dashboard. Okay. So when we started building in Gibson, we used a web interface. Now we're actually building tables right from cursor ID and deploying the database.

**Aakash Gupta** (00:35:09)

So you can interact with Gibson either way?

**Harish Mukhami** (00:35:12)

Absolutely, yeah.

**Aakash Gupta** (00:35:14)

And what would Gibson be replacing here if we weren't using Gibson?

**Harish Mukhami** (00:35:18)

You would be using your traditional database, whether it is like the Postgres, MySQL, SQL Server, if it's relational, non-relational MongoDB. But the onus is on you to take your data model, deploy it in the database, manage the database infrastructure, ensure that it's scaling, it's optimized, any sort of changes, you got to do migration, and Gibson can do all of that automatically for you. Got it. So it's getting schema and then it's going to go. Oh, it's actually adding a function to the test data to populate. So instead of actually creating the table. So I can ask it to make sure do this. Don't do this way a Python script. Don't create a Python script. Oh, it's actually doing the population. So let me say, did you deploy, redeploy the table? Again, it's checking the status with Gibson AI. And if it is deployed, if the latest schema is deployed, it's going to redeploy it.

**Aakash Gupta** (00:36:49)

Got it.

**Harish Mukhami** (00:36:50)

Okay. It looks like it redeployed it. Awesome. So one quick thing I'm going to do is go to Gibson and show you quickly that agent actions table. We just asked it in cursor. I have created a new agent action table here in Gibson. So let's see where it is. which is right here. So we just ask through cursor, it's available, redeploy. Got it. So now what we're going to do is we're actually going to go back to cursor, but we're going to use the crew AI framework. So that's the framework that we're using. Crew AI is an AI agent framework like LangChain, if folks are familiar with LangChain. So let me... I have pre-written this AI agent because it takes a bit to do it. It takes a few hours. It doesn't take days or months to do this. I'll talk about how the overall setup is.

**Harish Mukhami** (00:37:51)

There are two concepts here. One is agents. These are the agents that you're writing. If you look at this file, there are four agents. First, it's a database query agent. The job of this agent is to query the database, the database that we have, which is a CSADB1, and then extract data and analyze information here. So your expertise includes identifying high-risk customers through, let's see, what does it say? Running sophisticated high-risk customers... There you go. High-risk customers through multiple indicators that might signal churn risks. So low activity levels, declining usage patterns over time, numerous unresolved support tickets, low satisfaction scores, decreased purchase frequency, long periods of inactivity, failed payments or billing issues. So you have the opportunity to actually pinpoint exactly what you're looking for. And then once it's done, it surfaces the data to the churn analysis agent that's going to analyze the churn. And then a mitigation agent that is going to provide mitigation strategies.

**Harish Mukhami** (00:38:58)

And finally, a data ingestion agent that is going to take these actions and put it back in the table that we just created. So there are four agents that are doing the job of what a customer success agent would do typically. And then agents have tasks. So agents call the tasks. So these going to detail around what exactly you're supposed to do. And then all of these are put together as a crew of agents to finish the task. There's a bit of a setup involved here, so which I have done this. So what I'm going to do is I'm going to just run this agent now. So actually before that, one thing that I want to show you is So now we pointed this to our database, right? And then how does a crew agent knows the database context? If you have a different data model, how is it going to work?

**Harish Mukhami** (00:39:48)

So what we have done is it's pretty dynamic. So you can go look at, let me see where the schema tab is. So there's a thing called schema here. This is a schema that you can copy-paste of your analytics database. So crew knows the context of it. So what I can do here is like, can you update the schema with the schema of CSA DB1? Use the Gibson AMCP server. So if you want this to run on a different database, you just say that, and then it's going to go update that for you.

**Aakash Gupta** (00:40:26)

Okay.

**Harish Mukhami** (00:40:27)

And then I'm going to kick this off. So it's going to retrieve the project. It's interacting with Gibson via NCP tool, getting the schema definition and automatically updating it. So you don't even have to copy paste that here. That's done. So what I'm going to do now is run the main agent file here. So I'm just going to kick this off. And it's going to go execute the set of agents to do the job that we have indicated here. So now the agent is in motion. It takes about three to five minutes to execute. While it's executing, one of the things I want to show you is, so if you look at the customer success actions, I click on agent actions, this is empty. There are no actions here. The customer success agent that is running is going to populate that. So let's go back to the crew.

**Harish Mukhami** (00:41:30)

It's pretty interesting to watch and follow that run in sequence and understand how the agent is actually working. So now it is kicking off the churn reasons agent, so churn mitigation agent.

**Aakash Gupta** (00:41:46)

Which is one of the most important things our customer success agents are doing.

**Harish Mukhami** (00:41:50)

Absolutely. Yeah. Um, one of the cool thing is obviously these agents are running all the time. So these are agents that are running 24 seven, uh, They never take day off or time off. They're always on top of it, very consistent. So one of the challenges that we face is even though you provide dashboards and those are all handy, I think the onus is on the individual to actually take those actions and be on top of things. Some are really good, some are not. So we typically don't have a problem with agents running this way, especially if we have strong evals backing those as well.

**Aakash Gupta** (00:42:31)

Yep. And have we created those evals or is that a next step?

**Harish Mukhami** (00:42:35)

No, that's not part of this demo, but we should definitely do that. If you're running AI agents, you should definitely have evals to make sure that your agent is doing as it's intended and then any sort of feedback that you want to give the agent. It's just like your traditional end-to-end test cases that you would have for your typical SaaS software as well. So it's done. So let's go back to the dashboard. So it populated a bunch of actions here. So let's look at these. For this customer, specific customer, the risk level is nine. The action crew is recommending, actually, let me click on that. So action it is recommending is the potential reason could be product usage difficulties, send email to customers, schedule training session, provide product usage guidance. So that's the first one. So let's pick something else. Okay. Second one is product team for escalation.

**Harish Mukhami** (00:43:36)

So unaddressed customer issues, Send email to customer and send email to product team for escalation. So here it's recommending the CS agent like, hey, send an email to customers as well as like, hey, reach out to product team and make sure that we fix those issues. And similar, like schedule, some of these as like send email to customers, schedule training session, provide product usage. So all of these, it has even composed the emails for you. All you have to do here is you can either copy, paste, and then just send that email to that specific customer or product team. Or you can connect your tools to take actions right off from here. That is a step two where the agents are providing recommendations for actions here. Let me see. Now, the last step is the part three. So we evolved from building dashboard in part one where humans use the dashboard as a tool to analyze data to building an agent that does the data analysis and recommends actions.

**Harish Mukhami** (00:44:43)

Now for part three, we'll go a step further and add two more agents to execute those actions. So we've seen sending emails and sending emails to product teams. So we'll do one better and say like, send emails and actually go create JIRA tickets. So why send emails? Like put a ticket in the JIRA board. So we'll do that. For that, what we're going to do is we're going to go back to the crew agent and add those two new agents. Let me, so here's where the agent just ran. What I'm going to ask it to do here is Now for the case where it's product issue is the churn reason, create a ticket in Jira. So write a crew AI Jira tool. This will be a new task and agent combo and a tool. Use a crew AI documentation. I like to specify documentation, especially if it is like an up-and-coming tool so that we get more context.

**Harish Mukhami** (00:45:46)

to cursor. Please add an email agent as a final agent without changing the existing agent tools. Email agents should send emails based on the churn mitigation agent results. Write a create AI email tool. You send grid for emails. Otherwise, it's going to spin up an SMTP server and you don't want to do that. And then finally, like, again, documentation is here. And then I will add the context of the entire project here. So I'm going to give it the whole folder and then I'll just let it run. As you can imagine, there's a bit of a setup involved. So you need to have SendGrid account. Then you have to go copy-paste that into your ENV and then also set up your Jira board and then also create an app in Jira and then provide that app ID as well as, I believe, API token for agent to actually create those.

**Harish Mukhami** (00:46:47)

So it's going to go write those agents. In the meantime, what I want to show you is my email and the JIRA board so that we can see what the state is right now and what it will be once we write the agent and run it. All right. So this is my email. I have... While we're using customers' emails from the database, I want to default it to using my email so that we're not sending emails to random people. So we're just going to use my email as default. And then, let me see. And then here's my Jira board. So I created a CSA demo. There are no tickets created right now. And then now I'm going to go go to the cursor and show you the completely done customer success agent, which is autonomous. So let's go look at the agents here. These are the ones that we're familiar with, like database query agent, churn analysis agent, churn mitigation agent, data ingestion agent.

**Harish Mukhami** (00:47:57)

So these are the four agents that we saw and we ran. Now we have the email delivery agent, which is even communication specialists and personalized emails to high risk customers based on the mitigation strategies. So there's a backstory to it. And then you have a bunch of things that you want to ensure that agent does. Preparing emails for bad sending, knowing when to use test mode versus production sending, ensuring compliance with email communication best practices, a bunch of things. And then the Jira ticket agent. So Roll is a product issue manager. Create Jira tickets for customers experiencing product-related issues. So essentially, this is going to create a summarized Jira ticket for you. Okay. In this case, what I'm going to do here, I think we may have to set up the environment. Let me try this. It would read me. So here is where we're going to be installing virtual environment.

**Harish Mukhami** (00:49:10)

And then activate it. And then we'll do install the dependencies. Oh, I need to go to the right folder. It's going to install the dependencies and then can do a Python main dot PI, which is going to be, which is going to kick off the agent here. This again will take a couple minutes to run. At the end of it, we should see Jira tickets created in the Jira board, and then we should see the email sent out on behalf of the agent. So this completes the loop around like, hey, automatically analyzing, identifying actions, and actually taking those actions. You could imagine we can very easily add a lot more agents that are very specific to your workflow. If you think that agents are finding your product expensive, and if the reason is like, hey, we found some other place that is cheaper, there's an opportunity for you to send some discounts and coupons if you have a bunch of people in there.

**Harish Mukhami** (00:50:19)

If there are concerns around competition, you can definitely send the material around like this is why we're better than others if people are looking to switch to others. And the cool thing about it is we're not doing this after people have churned and trying to identify things and trying to get them back. We're doing this much before when they're churning. So that is the key part here. And it's always hard for CS agents to be proactive because there are so many things that they could look at. So running a customer success agent like this is going to catch customers before they churn.

**Aakash Gupta** (00:50:51)

Yeah, and I see this as the way we've created it, especially with the human loop check on some of these things as a way to make your CS agents that you have now like 10x more effective. Absolutely.

**Harish Mukhami** (00:51:02)

Absolutely. I feel like customer success is a function that you do need human in the loop. That's why I broke it down into a dashboard and an agent with a human in the loop and then autonomous so that you're not sending some random emails and that is only going to make problem worse. So we want to make sure that somebody is actually taking a look at these.

**Aakash Gupta** (00:51:24)

Yep. But you could theoretically, if you wanted, like we're talking about, write some evals where an LLM is evaluating what this one is doing and okay it too, if you wanted to go the other step.

**Harish Mukhami** (00:51:34)

Yep, absolutely.

**Aakash Gupta** (00:51:36)

And you could just use cursor like we have been with what seems like text language prompts to get there.

**Harish Mukhami** (00:51:42)

Yeah. Nowadays, pretty much a lot of tools have MCP servers, so you can definitely connect them and then execute your workflow. Not just cursor, any agent with an MCP client that can support that would do it.

**Aakash Gupta** (00:52:01)

And we talked a little bit about Crew AI. What was the role here of that tool?

**Harish Mukhami** (00:52:07)

So Crew AI is the AI agent framework that abstracts away a lot of things that you would have to do from a memory management, from a tool definition perspective, from chaining of those, debugging. All of that is done by Crew. It's a... I feel like it's more relevant for maybe semi-technical folks as well, because it's fairly straightforward in terms of how it is set up. And once you know it, you can tweak the backstory, you can tweak what you want to write from a prompting perspective on the agent's side to get the crew to do what you want to do. There's also other frameworks called Lanching. Lanching I think is a bit deeper but I felt like this is more targeted towards maybe semi-technical folks. Definitely technical too. So this is done. So the execution is done. So It took maybe like three minutes. So you're free to choose whatever framework you want for this demo.

**Harish Mukhami** (00:53:09)

I felt that this made a lot of sense, especially since I have a PM background as well. So while I'm technical, but I'm not like a pure developer.

**Aakash Gupta** (00:53:20)

Yeah. So let's go check those Jira boards in email.

**Harish Mukhami** (00:53:24)

Yeah, absolutely. So this is the Jira board. It created three tickets. One, two, three. Let's click on this. Customer is facing unaddressed customer issues with the product usage is currently unresolved. Eight tickets is critical to their continued engagement with the product. If we had very specific ticket information, we could have gotten this, but this is essentially created as a bug. I think one of the things that was cool about this is It put in labels saying is churn risk customer reported. So you can obviously make a very significant prioritization decision here. So as a product team, we just created this. Emails could sometimes take a bit, but actually they showed up too. So for emails, let's look at this. I hope you're well. I want to sincerely apologize for the unresolved issue. I would like to offer you a discount. Wow, okay. This went a step further.

**Harish Mukhami** (00:54:26)

Obviously, we didn't put in a specific customer success agent that we could easily configure to have this coming from them versus me. And then let's resolve issues together, improving your experience with our product. We're here to assist you. So it sent out four emails and then at the same time created three JIRA tickets here on the JIRA board.

**Aakash Gupta** (00:54:46)

Amazing. And that covers our live cooking session. So today we created an AI customer success agent. Using the concepts we went over today, what other AI employees could people create?

**Harish Mukhami** (00:55:02)

I think... I think pretty much all of the information work is up for automation. So I think you covered product manager before. SDRs are a very popular use case. Financial

**Aakash Gupta** (00:55:18)

and development representative.

**Harish Mukhami** (00:55:20)

Exactly. Sorry, say that again?

**Aakash Gupta** (00:55:23)

SDR, sales development representative, the person who goes out and gets the initial lead.

**Harish Mukhami** (00:55:29)

Absolutely. There is also meeting preparation agent, executive assistant. You can chain together all of these agents to create a specific role that is tailored for you. Absolutely. We also have AI agents that are acting as recruiters. So they do a lot of upfront work around analyzing resumes and picking those based on the JDs. So these are all very popular use cases. Anything that involves putting together, whether it is structured or unstructured data, to take action, they're all up for automation.

**Aakash Gupta** (00:56:08)

Wow. So basically, the criteria here is you can build an AI employee for any task in your business that involves ingesting information and then sending out information. So all of those tasks, those human connector tasks, we saw it create JIRA tickets, we saw it send emails, we can now do. That was an awesome demo. I want to spend just a few minutes here at the end learning a little bit more about you. So you worked head of product at Siri. You were CPO at LeafLink. Talk to us a little bit about how you came into this process of creating Gibson.

**Harish Mukhami** (00:56:47)

Yeah, absolutely. So before Apple, I spent almost a decade at Microsoft. And And one of the core focus for me was building dev tools and developer frameworks. Primarily worked as a developer on Microsoft Dynamics and then was a PM on the same product. I saw firsthand some of the biggest challenges, especially around building software, building infrastructure around databases, and a lot of those are still not solved. And then those problems continued. onto my next roles at Apple or at LeafLink. So the biggest impediment to delivering software quickly, solving customers' problems quickly is delivering software. And that is relying on engineering teams to develop that. While we are not at a place we can say that engineers are, we don't need engineers and AI can write code for you. I don't think we're there yet. But we have enough tools to make engineers like a junior engineer, a senior engineer, and in general, any person like you said before, a 10x version of themselves.

**Harish Mukhami** (00:58:03)

So that's the impetus behind building Gibson. We are focusing on the database layer of the dev stack. So we're focusing on all the way from design, development, deployment, management, and scaling of databases, which coding tools don't do today. Maybe coding tools can write data models and schemas, but there's a lot more involved in database management than just writing schemas and data models. So there's a big component around schema migration, data migration, query optimization, impact of any schema changes you do, and we're handling all of that via Gibson. We currently solve, from a PLG perspective, zero-to-one use case for enterprise customers we can solve for existing databases as well.

**Aakash Gupta** (00:58:49)

What's your grand vision? If everything works out for Gibson over the next three to four years, what will people be building on Gibson?

**Harish Mukhami** (00:58:57)

Yeah, my vision is that every single business, individual building technology products, AI agents, data-powered products are using Gibson as a backend to manage databases, scale infrastructure, and be on their journey from going from 0 to 1 to 1 to 100. So whether you are serving 10 users to 100 users to tens of millions of users, Gibson is there with you on your journey, and it makes it very easy for you to scale. One of my favorite use cases with Gibson, Akash, that you have just seen, is you plug Gibson into Vibe Coding Tools, and you're not building a prototype anymore. So you are backed by a very significant production-grade database. it's already deployed in the cloud. So you publish this and you get 10,000 users tomorrow, we can handle that. So you don't have to scrap this and rewrite it. So, and it's very quick, right?

**Harish Mukhami** (00:59:57)

We provision database and deployed it in a matter of seconds. So these are the things that take a lot of work. And one of the, one of the key things also is it's not enjoyable. Not every developer enjoys managing infrastructure and databases. They just want to write code. So we handle the grunt work.

**Aakash Gupta** (01:00:15)

So is it fair to say that with the tools that we've showed you today, you can go from beyond just prototyping to vibe coding with a production-grade database to actually put something out there that acts as an employee for your company?

**Harish Mukhami** (01:00:29)

Absolutely. The one thing I would say, whether you're vibe coding or whether you are using databases as a co-pilot, we haven't done that today in the interest of time, but any code that AI generates, please read. Make sure that you don't just blindly accept, like make sure that it is the code that you want. I typically don't code in the agentic mode. I know a lot of developers on my team, they definitely use AI, but they use it in a copilot mode to complete the sentences versus like actually writing code for them. So make sure you're reading what you're actually accepting.

**Aakash Gupta** (01:01:09)

All right. Harish, if we had another hour, we could do another hour. Thank you so much for helping us build an AI employee today. Thank you for having me out, gosh. It's been a pleasure. I really hope you guys enjoyed that episode. It would mean a ton to me and the team if you could please subscribe on YouTube, follow on Apple and Spotify podcasts and leave a rating and review. Those ratings and reviews really help grow the show and help other people discover the show. And they help fund the production so that we can do bigger and better productions. Can't wait to share the next episode with you. Until then, see you later.
