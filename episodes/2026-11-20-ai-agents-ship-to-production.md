---
title: "How to Ship to Production with AI Agents"
subtitle: "I got the CPO of a $47M AI company to open his GitHub and show me the AI reviewer and the ops agent behind it."
date: "2026-11-20"
host: "Aakash Gupta"
guests: ["Shuhao Zhang"]
speaker_names: "substack"
substack_url: "https://www.news.aakashg.com/p/ai-agents-ship-to-production"
youtube_url: "https://www.youtube.com/watch?v=-xQPRlk7VRE"
duration: "01:02:44"
word_count: 9966
source: "Substack episode transcript (aired audio)"
---

# How to Ship to Production with AI Agents

*I got the CPO of a $47M AI company to open his GitHub and show me the AI reviewer and the ops agent behind it.*

**Shuhao Zhang** (00:00:00)

When agents can generate tens of

**Aakash Gupta** (00:00:02)

thousands of miles of code

**Shuhao Zhang** (00:00:03)

in the blink, the human reviewer becomes the bottleneck.

**Aakash Gupta** (00:00:06)

Tinyfish AI is a startup that has been on a hockey stick growth path. They raised $47 million from Iconic. They went from 100 ,000 to 200 ,000 users in 18 days. They went From 200 ,00 to 300 ,000 users in just 10 days.

**Shuhao Zhang** (00:00:20)

This system will allow anyone to ship to production, not just engineers. Why wouldn't you use like Cloud Code Web? I noticed that Cloud Code web now has more features that I need but This is something I built last year when the features are not available out of the box from cloud. We continuously to improve our service, especially when we build search. It's a web info company that will help agents to work with the web. There's a search fetch and then there's a web agent. We really should consider agents as the new type of users and there will be trillions of them.

<!-- sponsor -->
**Aakash Gupta** (00:00:53)

What are the mistakes you faced along the way building towards this? Before we get into today's show, please take a second to check that you're subscribed on YouTube and following on Apple and Spotify podcasts. If you want access to all of my favorite AI tools, I've gotten them to give you an entire year of their paid plans. Check out bundle.akashg.com for an entire year of Bolt.new, Airtable, Speechify, Descript, Magic Patterns, Linear, Dovetail, Arise, and Mobbin. And now into today's show. Tinyfish AI is a startup that has been on a hockey stick growth path. They raised $47 million from Iconic. They went from 100,000 to 200,000 users in 18 days. They went from 200,000 to 300,000 users in just 10 days. A big part of the reason, after I talked to Xu Hao Zhao, their co-founder and chief product officer, is the way they build. They allow anyone to ship to production in the company.

<!-- sponsor -->
**Aakash Gupta** (00:01:57)

That's because they hired a bunch of amazing former meta-engineers. Xu Hao himself was a former VP of engineering. And they built the system... That allows you to ship features. And so they've invested in the coding agents, the coding review, the CAD system, everything that you can think of from how you started Purity all the way to how you measure the results. Of a feature that allows you to do it on via agents. And so this is the next -gen way of building products. And in today's episode, Shuhao is going to walk you through all the steps of that lifecycle. He's going to actually pull up his real GitHub and show you actually how he uses Cloud Code so that you too can allow anyone at your company to ship features for production. Shuhaou, thanks for being on the podcast. What do people really need to know about this system and how they can build it themselves?

<!-- sponsor -->
**Aakash Gupta** (00:02:51)

Let me show you.

**Shuhao Zhang** (00:02:52)

Yeah, so Akash, today I'm going to show you the whole setup, like what I use on a day-to-day basis from building to shaping into production. And then now I'm actually building the part that let agent to operate and maintain as we just talked about. So this is my CloudCube setup. I have a dev server, and this is a TMUX session so that I can open it up in my mobile phone or my browser. When I close everything, it still runs in Cloud. And it's a full EC2 server, so it can install the tools and the whole stack as needed. So you can see we have multiple projects going on here, and each of them could be a feature or a new product that I'm building. And in this one, you see it's still live, it's working. And this is an AI gateway product, we call it Tiny Router, that will put our models behind one gateway with a discount.

**Shuhao Zhang** (00:03:54)

What it does is this is already, the first part is already built. I'm trying to land it into our sandbox environment. And I can talk about the whole setup.

**Aakash Gupta** (00:04:05)

So maybe you can break down for those of us who aren't as technical or don't have as much of a technical background, some of the things that you just said in the sort of quote unquote four dummies version. Dev server, what are we looking at there? Sandbox, what does that mean there? And then what is this software as well? If you can break down those basics for us, that'd be great.

**Shuhao Zhang** (00:04:28)

Yeah, sure. Let me talk about it. So a dev server is essentially a remote server running in the cloud. It can be an EC2 instance in AWS or any server that you host or your own MacBook that has external connectivity. The goal for that is really that you can run your job, your workloads without you keep your laptop running, which is a local environment. And the sandbox is an environment pre-production. The setup is very close to production, but you don't have real user data. You have canned data for you to test your software before it goes live. The software I'm using is, actually this is built by Cloud Code itself. It's called T -Mux where you can stream a terminal session through the network and it's secured protected by encryption So yeah This is my primary way of working with MyClouds

**Aakash Gupta** (00:05:29)

Why wouldn't you use like CloudCode Web?

**Shuhao Zhang** (00:05:31)

Yeah, I noticed that Cloud Code Web now has more features that I need, but this is something I built last year when the features are not available out of the box from Cloud. But I definitely see a future where It's just out of the box. I can just use it. But I also like the flexibility of owning my entire instance that I can install. For example, if I need my VPN access, I can install my VPN profile here. So there are still things that Cloud Web are not flexible enough that I'd love to have the full control

**Aakash Gupta** (00:06:10)

on it.

**Shuhao Zhang** (00:06:10)

Yeah, so this is, you can imagine this is the interface where I talk to the agents, but as you can see, everybody use cloud, you can see the UI is a lot of their own work log, but the valuable communication, clarifying product requirements, giving feedback needs to happen in a different place. And what I do is cloud artifact is a great way of communicating. So cloud can generate its plan for me to review and I can type my response in the artifact. I can show one of those artifacts to you. All right.

**Aakash Gupta** (00:06:52)

If you've worked at any company bigger than 30 people, you know this one. The CEO sets strategy. By the time it reaches the people actually doing the work, it goes through three or four layers of translation. That's the problem Ariso is built for. It's an AI operating partner for every manager and team. It connects to where work actually happens, the meetings, the messages, the docs, and it turns

**Shuhao Zhang** (00:07:15)

all that fragmented activity into a clear picture of execution.

**Aakash Gupta** (00:07:19)

Teachers get real coaching grounded in their team's actual work, not generic advice. Teams stay aligned with strategy as it changes, not as it was last quarter. And leaders see where execution is drifting in weeks, not in the postmortem. One shared memory for the whole org. Everyone finally working from the same picture. If you lead a team, check out ariso.ai.akash. That's A-R-I-S-O dot A-I slash A-A-K-A-S-A. Every growth team has a funnel they should be watching more closely. Usually it's checkout. Amplitude custom agents will watch that funnel for you on the schedule you set. Let me show you. You start by describing the job. Watch my checkout drop off. The agent builder will ask a few questions to shape it and then the agent connectors plug it into your stack. That part matters. The agent reads the PRD, the tickets, the team conversations, so its analysis actually carries the full context of what's happened.

**Aakash Gupta** (00:08:14)

From there, it monitors the funnel on a schedule, and when it spots a problem, it acts. Right here, It files the linear ticket itself. The loop between knowing and doing closes on its own. That's the shift. Set up the agent once and it runs the work. Custom agents are free for all Amplitude customers in open beta right now. There's a library of pre-built agents too, including the exact checkout drop-off investigator. Start at amplitude.com slash ai-agents.

**Shuhao Zhang** (00:08:42)

The agent library is linked right there. Let me show one of the artifacts. So when this is, I usually ask my clock kid to, for any like bigger designs decisions to generate a plan and give me some recommendations. And also give me status update. So this is where I review the plan. I won't show the entire thing, but you get the idea where I can actually respond in line. And it's going to pick up my response and then carry on. So that's kind of pretty much the basic setup where you can talk to your cloud. You can review and clarify the designs. And I think this pretty much everybody has their own setup and it worked pretty well. What I'm going to talk about more is how to push your product into production and then how to possibly operate it in production environments. And by the way, this is something that I'm also actively building and experimenting.

**Shuhao Zhang** (00:09:43)

So I'd love to hear your thoughts in the comments. And if I can update in another episode how things are working, I'd love to do it as well.

**Aakash Gupta** (00:09:53)

Aren't we off?

**Shuhao Zhang** (00:09:55)

So first of all, to get into our production environment, again, we start with the sandbox, is to go through the code review process. And as a company, Tinyfish, we have quite a few entities. We are engineers from Meta, so the code review culture is really strong. We hold every line of code very seriously. However, when agents can generate thousands of lines of code, tens of thousands of lines of code in the blink, Common reviewer becomes the bottleneck. But how to solve that? We don't want to let go the quality control. We don't want to let go the second opinion, third opinion. So what we do is we onboard CodeRabbit. A lot of users love them. But how to let CodeRabbit auto-approve your PR and you still stay compliant. You still get the back and the forth as you usually get with your engineers. So what we do is we let CodeRabbit to approve the PR, but also just like a human reviewer, it can reject a PR request for action, and then the agent will pick it up automatically, go back in the form.

**Shuhao Zhang** (00:11:10)

But if coderabit detects a high risk and requires human judgment, it's going to loop in. The agent will attack the right engineers to do a human review. But if coderabit is happy about it, it's a lower risk. PR will be auto-approved and auto-merged. So I'm going to show you, see this is quite extensive PR about a UI change, which there are a lot of changes, a lot of files touched. However, it's considered a lower risk in general, but still you can see There are quite a bit of responses from Colour Rabbit. And let me show you a couple examples here. So it requests for change, meaning that there are things that it's not happy about. And this is where you're going to pay attention to. Then you can see this is where the AI reviewer considers things are not optimized or correct. And then this is actually my agent picking up the response, the feedback, and then make a correction.

**Shuhao Zhang** (00:12:17)

Finally, the AI reviewer approved it. So you can see there are multiple ones until... Both are happy with the results. The PR is merged in the end. So this is one of the examples where when you produce a ton of pull requests and what's the fast and safe way to get them merged and reveal them merged.

**Aakash Gupta** (00:12:41)

So basically you have an independent tool. In this case, you guys are using a third-party CodeRabbit. And CodeRabbit, what it's really doing is it has some context around your code base, your coding standards, what your engineering team likes things to be like. And it is acting as them and working with the Claude agent that initially submitted the pull request back and forth, back and forth until it's happy.

**Shuhao Zhang** (00:13:04)

Yeah. So we have the concept of constitution, which is installed our convention, our standard, and then how strict it should be. So yeah, as you said, CodeRabbits knows the context. And knows how far it goes, how deep it goes in the review. Because you do get into this infinite spiral where it's going to be too picky and the agent is trying to please the reviewer. And you just go into an infinite loop of picking all the problems, which is not necessary. You really want to catch the ones that matters.

**Aakash Gupta** (00:13:40)

Yeah, you don't want to just burn a bunch of tokens on this kind of back and forth.

**Shuhao Zhang** (00:13:44)

Yeah, they can really keep going if you don't have. So that's why we build a knowledge base or repository of what type of reviews, the review style, the coding style is quite extensive. But this is where I think modern engineering teams should invest in that you build this. It's kind of your organization's playbook for both your coding agent and the review agent.

**Aakash Gupta** (00:14:06)

And who's the right person to own this? How do they really execute on this project? How much ongoing effort is required? Is it like one of your most senior tech leads who's super AI-pilled and loves this stuff? They get a project for some amount of time where they're working on the code reviewer agent and then they have to maintain that every couple weeks for a couple hours? Or how does that process look?

**Shuhao Zhang** (00:14:29)

Yeah, exactly. So we have our head of engineering, Pasha, to personally look into AI productivity. We have a channel, all the engineers can chime in but we have one senior engineer to look into this and experiment with multiple projects. And, you know, it can be in production, in staging, to repetitively and iteratively validate this approach.

**Aakash Gupta** (00:14:54)

So how can people replicate this on their own? What are the elements they need to do to build this up from the ground up where they feel like they're actually shipping production quality features?

**Shuhao Zhang** (00:15:04)

Okay, so yeah, the best place to start is a template. So this is easy for your team to replicate. Your lead engineer can work on this template. This is ours. So you can see we use Terraform for For every infrastructure process and CI, CD. So in this template, you have, what's really important is actually this infra folder where you have, say, sandbox environment, production environment. And, you know, you have these, like, templates, Terraform files, which, you know, talk about the how do I do... The requirements, you can configure your network in production, you can configure the access, the whole, how do you do ECS, how do you do Kubernetes, and this will have a Let your coding agent know how your clouds, how your ops are set up. And they will use the same setup across different projects. And then how the DB should be set up.

**Shuhao Zhang** (00:16:10)

Docker, Containers, and then your app logic leaves in this app folder. And how you test it set up, all the scripts. So with this template, a lot of the scaffolding is already in, especially the deployment CICD part, which is usually where the agent can be very opinionated and you don't want your ton of projects have different ways. So this is usually a good starting point. To make sure your project is deployable to your environment.

**Aakash Gupta** (00:16:43)

And you had mentioned Terraform. If people don't know that, what is that and what does it do?

**Shuhao Zhang** (00:16:46)

Yeah, Terraform is a configuration language done by HashiCorp. Essentially, your infrastructure is code. If you want to land a new instance, if you want to configure a domain point So if you're joining to a certain service, instead of going to AWS console, you're actually making changes in the Terraform file. And the benefit of that is you can have your team review this like a code, right? To double check. And then once it's merged, it's going to propagate the change all the way to AWS.

**Aakash Gupta** (00:17:22)

Very cool. Okay. Yeah. So it's basically all the instructions from what I'm guessing inside this dot cloud folder is like your cloud MD, your different coding skills, your different architecture of your database, like you had already mentioned in Docker. What all goes in this?

**Shuhao Zhang** (00:17:39)

Yeah, so in Cloud, yeah, you can see from the folder name their best practices. That's for the entire organization. The rules is this with the guardrails that agent must follow. Yeah, so this is another like what we want to share across and let everyone to have the same coding agent style. And it's proven to be very effective. And we're kind of sharing the organizational knowledge together and put the best practice all in one place.

**Aakash Gupta** (00:18:09)

Does everyone use like the same coding agents or is this kind of built in a coding and agent agnostic way? So if somebody prefers Codex or Claude, it can work in either.

**Shuhao Zhang** (00:18:18)

Yeah, it's quite easy to migrate the cloud skills and plugins. Yeah, we do have engineers prefer different coding agents, and we also have a tool that can transform the skills across.

**Aakash Gupta** (00:18:33)

And you use cloud code, though, mainly. So what goes from here? So you've got a GitHub project. Maybe actually let's start at the feature level. How are you initially prompting the feature, creating the prototype? How does all of that work?

**Shuhao Zhang** (00:18:46)

Yeah, so probably a new feature, depending on how big it is, but I think today you also have like an agreement with your agent what kind of language you're going to use. Like I prefer using very simple language and then it talks back to me in a simple language. Andrew Kaposi talked about the IC standard, which used in aerospace, that there's no immigration. You only have a certain vocabulary that you can use. I really like that. But my workspace is actually this. I have a text editor. The voice mode, you can see from here that I can talk to it even while I'm driving and they will talk back. So there's this back and forth brainstorm with the agent and kind of get the context of what want to build. I can kind of type in through here, the voice will also end up here. I led the agent to design this from the top level, the product design documents as an artifact.

**Shuhao Zhang** (00:19:43)

So that's where I go from there. I also wanted to do enough research on the markets, the competition. What's the best product out there? What is missing? So there are a significant amount of time spent on just idea-ating and making sure that agent knows exactly what I'm trying to build. And along the process, I I encourage agents to challenge my idea to propose alternatives and have a small-scale experiment to fail fast, to see some early flags. But the end product is a bunch of documents. You can see how many documents it produces. Let me show one of those. Now, this is kind of a scratchpad, which is a repository just for remembering all the designs. So you can see there is the API design, the cloud architecture. And I'm just going through, you can see there are a whole bunch of documents. And this is like really, it's the PRD, the engineering plan, the implementation plan.

**Shuhao Zhang** (00:20:57)

I won't click through it, but... You know, each plan is sophisticated enough and they can see the V2s. So I do go back and forth with my agent. And so I know almost exactly what it's going to do. What is the design decisions? And I always ask it to list the 10, 15 decisions needs my attention. And I also encourage it to make decisions on the low risk ones. That will kick off a fairly lengthy coding session.

**Aakash Gupta** (00:21:31)

So you go from idea that you bat around with the agent and you ask it to push holes in your thinking to eventually a PRD to eventually an engineering specification. And then it sounds like sometimes a prototype and then you go to code. Is that the life cycle?

**Shuhao Zhang** (00:21:47)

Yes, exactly. And I tend to front load a lot of the designs and considerations and have an entire engineering plan and implementation plans to kind of go off on. Only 20 plus hours or multi-day of implementation and go as far as it can. And then I can go start another iteration of testing. So I do want to kind of play with the service myself, give some feedback. But the idea is really I want to run multiple agents, building multiple products and features in parallel so that while one agent is running for Hours and tens of hours, I can focus on brainstorming for another different feature. The pattern of having an agent ask you a question every half an hour, what I found is you're going to easily have this AI fatigue and you find yourself kind of drawn in multiple agent sessions and be in the bottleneck of answering questions and approving the next action.

**Aakash Gupta** (00:22:53)

Yeah, that happens to me all the time. It's like I put box out like two hours to do this thing and then all of a sudden I just find that I spent the last two hours looping through my 12 different agents and giving them prompts. How do you make sure that you stay productive in those sessions and you eventually accomplish what you were there to do?

**Shuhao Zhang** (00:23:10)

Yeah, so I really want to find a way that agents can continuously work for much longer hours, but not drifting. And that's why I front load with a lot of documentation process where, you know, from ideas. So it's almost like you focus on design with your agent where you can have a lot of your own human time. And once you reach agreement, this agent, this particular feature is ready to go so that you're spending continuous time designing and getting feedback and agent will spend continuous time building.

**Aakash Gupta** (00:23:52)

All right. Where should we go from here? What else should people know in order to be able to build like this?

**Shuhao Zhang** (00:23:56)

Yeah. So now we have seen how, you know, kick off a building session and having the code reviewed and then pushing to get the PRs approved. And then eventually you're going to use the Terraform, use whatever CICD that you can Have your service built by agent running in some environments. Let's say it's in a sandbox. And eventually this will run in production. So this is where I see the next frontier will be, where you let your agent, So what we just talked about is going to be fairly today's commodity. I think everyone has their own favorite way of doing things and set up, but to have the agent operate in production is really something that I believe will differentiate how fast companies can build their products.

**Aakash Gupta** (00:24:46)

Are you looking to up your AI product management chops? I highly recommend the AI product management certification by product faculty. It has a 4.7 with 1,249 reviews on Maven for a reason. I myself took the course back in 2024 and it was awesome. Since then, they have upgraded it. So now you get to learn from product leaders at OpenAI and Anthropic. On top of that, Powell Hearn, author of the Product Compass, leads the Build Labs. It's going to go from theoretical knowledge about AI PM to a very practical course. It's going to help you identify AI leverage opportunities. It's going to help you design trustworthy AI experiences. It's going to help you systematically optimize outputs for accuracy Build rigorous evaluation suites, architect AI agentic systems that work, and select the perfect LLM for your use case. It's normally $2,500, but you get a discount when you use my link.

**Aakash Gupta** (00:25:41)

The next cohort starts June 22nd and goes to August 9th, so do check it out with my link in the description. They have been one of my longest sponsors for a reason. I trust this product, and I think you should consider the cohort. I want to take a second to talk to you about the fourth cohort of LAN PM Job. I trained 30 students in cohort one, 50 students in cohort two, and 75 students in cohort three. And I am bringing back the program for cohort four. It starts in August and it lasts The next three months where you're going to have intense sessions, a Monday morning session where I go over your resume, behavioral interviews, LinkedIn. On top of that, Bart Jaworski is going to be teaching you the PM fundamentals in 2026, how to write AI PRDs, how to AI prototype with clients. So it is a full package.

**Aakash Gupta** (00:26:24)

It is three courses in one for one low fee. So join at landpmjob.com. Virmani is going to be teaching you AI product management. He is an AI product manager at Uber, and he's going to teach you how to build AI features that actually work successfully. On top of that, Prasad Reddy is going gonna be doing one -on -ones with you for market reviews, LinkedIn review, candidate market fit review. So it is a full package. It has three courses in one for one low fee. So join at landpmjob .com. I used to think I had a retention problem. Turns out I had a messaging problem. I was sending the same onboarding emails to every new user, whether they activated on day one or never logged in again. I had no idea who was slipping or why. Customer.io changed that. And what users actually do in the product.

**Aakash Gupta** (00:27:09)

Someone hits a key activation moment, they get nudged to the next one. Someone goes quiet, they get a different path entirely. Their AI agent makes it fast. I describe the campaign I want and it builds the full journey form. Triggers, timing, copy. Even branching logic. And when I want to know how something is performing, I just ask the agent directly and it tells me what to do next. They also have an MCP server, which means AI tools like Claude can see directly what's happening in your customer data or workspace. Your segments, your customer data, Your attribution, all of it. So instead of explaining your business context every time you need help, Claude already knows it. Notion used Customer.io to personalize their onboarding and hit nearly 50% open rate, improved conversion by 6% to 7% with localized campaigns, and pushed open rates up another 20% through A-B testing.

**Aakash Gupta** (00:27:56)

The idea is simple. Customer.io helps you deliver more impact from every message you send. If you're a PM or founder and your onboarding is still one-size-fits-all, try Customer.io at Customer.io.

**Shuhao Zhang** (00:28:06)

I believe it's going to be data backed. And agents need to have access to the production matrix, traces, and logs. Well, where we start first is to build a system. I can show you this. Observability, right? So every company has their own stack. I'm not opinionated on any of those, but we decided to build our own observability stack because of the load we're having. And the traffic, but also the control, right? So we use a combination of open source and also self-built solutions. And this is a diagram you can see where applications will have a, it's really easy to plug in, it's a couple of lines, then your application will have the entire observability stack for Tinyfish. So you can have the logs, matrix, and the traces. The three critical information you want to gather from a production. And then you're going to find out into the backend.

**Shuhao Zhang** (00:29:13)

And this is a very efficient, high throughput system. What's critical is usually it's the human that consume the observability output. And whenever there's an alarm, whenever there's errors, or you just want to look at the metrics and performance logs and find where to optimize. We really believe AI agents are better ones to consume this huge amount of data in production continuously, meaning that you watch this 24-7, and you can know where your memory has a bottleneck and what the reason before it even sends you an alarm and your service is down. So within the logs, you can watch for business logic problems, errors, and opportunity to improve your system. So this is the system I really want to build well and make it work in Tinyfish.

**Aakash Gupta** (00:30:13)

Can you say more about the difference between logs, metrics, traces, what exactly those are for people who don't know?

**Shuhao Zhang** (00:30:18)

For logs, logs are, you want to keep it more of a verbal, verbose version of what happened in your service. And developers can inject certain, well, this is logs, right? You can print out what exactly happens for, say, a user lifecycle. When users start to use this feature, the service, say, we start a database connection, and this is the connection I got. Send a particular request. You can log the request. And then what your system does across this whole time per step, you can be as granular as you want. You have the full control. And the log is a huge amount of data you can imagine. This is the replay, if you will. If anything goes wrong, you want to see the logs. So Matrix is really where you want to see the performance of all numbers. The number of requests you can serve, the CPU loads, how memory is doing, all the latencies.

**Shuhao Zhang** (00:31:21)

And TreeSees is how your systems connect together, how one user's behavior will go through your multiple services. When you have a ton of microservices, how do you trace the entire activity across them and trace is usually done automatically through injection. So all three are important, and you should look at them all together.

**Aakash Gupta** (00:31:51)

Got it. Okay. And basically what you're showing here is a system that is the point here that it's figuring out the errors or the mistakes or what is this accomplishing for us?

**Shuhao Zhang** (00:32:04)

Anything that is a surprise or a potential improvement potential. So if there's anything that's wrong, you usually have an alarm system that certain run, certain execution does not complete successfully. And they usually will go back to the logs to see where things fail. And that can point you at potentially the part of the code that you need to fix. And metrics that will tell you the performance problems, how well your systems scale, and how reliable they are. The traces really tells you that if all the systems are connected together, when you are identifying bottlenecks in certain microservices, if the overall latency is high, but where? Is it the login? Is it the database? Looking to this, it's a massive amount of data. We're talking about terabytes of data, petabytes of data. That is like you can mine opportunities to improve your software and service.

**Aakash Gupta** (00:33:10)

Where do we go from here?

**Shuhao Zhang** (00:33:11)

What we go from here is really to have the agent to look into this matrix and logs and traces continuously. And these are usually behind firewalls, behind authentication. So having your agent authenticated to have access, you can have, if it's all behind firewall, then you can have the VPN installed on your dev server. So they'd have the access and then build a skill for them to know how your observability system works, where things are, the formats and all the mechanisms for them to access. And then they will start to detect problems. So this is an example of, I'm looking at a linear project and it's brand new. It's actually running today. You have this AIOps that's detecting issues from the observability system. For example, this is a real issue where it finds out when an LLM call reached MAX tokens, it returns a server error. It's actually not a server error.

**Shuhao Zhang** (00:34:20)

The server is functional. But this is like the client sending too many tokens. It should be a con-error. And it only detects this because it finds out this behavior from the logs, from the traces. And then, hey, this is What agent does is, I'm calling it is ops agent. It's going to first open a linear, kind of mimicking our engineer's behavior. Engineers would open a linear ticket first, and then it's going to go ahead and then try to fix it. So this is documenting what it finds and the potential fixes. And then it starts to making the fixes. So far, so good, right?

**Aakash Gupta** (00:35:07)

OK. Makes sense.

**Shuhao Zhang** (00:35:09)

And after it makes the fix, it's going to push a pull request. It's going to push the code into our GitHub and ask for review. And you can see for this particular fix, it's considered a lower risk and code Automatically approve it. And what happens is the agent will know, okay, my change is good. The test, everything is okay. I'm going to merge it. Merge here means it's going to be automatically picked up. And deployed to staging environment through our CI CD. So you see the entire thing is running continuously, watching the production traces and logs, detecting errors, and make a fix, get an AI reviewer to review, and automatically deploy to the environment.

**Aakash Gupta** (00:35:59)

And how does it know the Nordstar of what's true that it should give a cut answer?

**Shuhao Zhang** (00:36:03)

Yeah. So usually when you look into the observity, the whole mining part, quite a bit of those are pretty obvious. Like you have this exception, you have the error log, you have this super long latent And what happens in the past decades is it's going to either be an alarm sent to your on-call engineer, or it's going to kind of backlog in your You use Sentry, you use other systems, and engineers will try to kind of crunch through this backlog. But a ton of those are never fixed because they are very low percentage and The system over time will degrade because of this. And the user has to wait for a much longer time for things to be fixed if they're not that highest priority. But having the ops agent We're talking about you can have multiple sessions and make a fix and test it properly, deploy to production automatically when the engineers are sleeping.

**Shuhao Zhang** (00:37:14)

You can also have gated rollout. You can roll out to 1 % of the users in production and make sure there's no regression. You have multiple flags on A -B test. So this is the whole new paradigm I'm looking into, and really I want to install this to tiny fish and prove it works.

**Aakash Gupta** (00:37:34)

Okay, and those things you just mentioned are pretty interesting sort of safety mechanisms. How often should you be doing it in like the 1 % rollout? Or should you always be doing it in like a phase rollout, always either have a rollout or an A-B test? How do you think about shipping these things that were essentially after the engineering spec, it was just done by agents, right? Just clock and code draft.

**Shuhao Zhang** (00:37:58)

Yeah. If you have the bandwidth and capacity, you should always do this partial rollout. Always. Even for a critical fix that, you know, you take an extra hour. It also depends on your production volume, right? You want to take an extra hour to see how this 1 % user behaves on this new change, right? And that always is the last defense against something catastrophic. But it used to be very, very costly. Imagine A company with, a team with dozens of engineers, hundreds of engineers, the changes they make when they roll out to production. It's not realistic to have a partial rollout for every change. And because you need to, someone, some Some human needs to look at the partial rollout stats and then make a judgment. But now you can actually have agent to do this. So the whole thing is actually designed for agent automation.

**Shuhao Zhang** (00:39:01)

And arguably with this approach, it's safer and more efficient than human operation.

**Aakash Gupta** (00:39:10)

Okay. Is there anything else people need to know to replicate this on their own?

**Shuhao Zhang** (00:39:14)

I think there are existing services doing this, right? There's more of a, you know, we kind of came from a vibe coding to more of a coding agent that would remove the vibe part and to be more serious about it in production. And then there's the concept of agentic engineering that we start to kind of look at more that agent can do, not just coding, but, you know, the whole thing we just talked about. But I believe this is going to be what engineering will focus on. As I said in the beginning, that it's no longer a matter of what product you build. It's really, this is the muscle every engineering organization You can still use as many third-party tools just like us using CodeRabbit, but I think the knowledge, the methodology, the framework, and then the opinions you have in the next six months will And maybe in one or two years, this will just become so out of the box.

**Shuhao Zhang** (00:40:27)

Maybe the cloud providers will just have this. But for the time being, when everybody still risks to the market, to their users, this is really a critical and high ROI investment.

**Aakash Gupta** (00:40:41)

What are the mistakes you faced along the way building towards this? And what are kind of that scar tissue that other people can learn from?

**Shuhao Zhang** (00:40:48)

The biggest scar tissue is really thinking too much. And it's kind of a paradox. It's kind of self-conflicting. You want it to be your agent to run as much as possible, but at the same time, you're thinking Thinking of all the things could go wrong and spending a lot of time telling yourself not to begin. But I think it's really going to believe in this future because it's going to be the case. And don't wait for others to hand you this system for yourself. You really need to build it yourself. Just don't spend too much time convincing yourself not to make a move. And I think we spent enough time debating, but now we feel that we could have started this a bit earlier.

**Aakash Gupta** (00:41:34)

People are saying in the back of their mind right now, well, he's at a startup. They've only raised $50 million. So put your Meta hat back on when you're at Meta or at a much bigger company. What are the things that they're saying, hey, we can't adopt this for? And how would you address those one by one?

**Shuhao Zhang** (00:41:52)

Actually, I found the companies with much bigger resource, they actually gone really far. They gone further than startups. Not all the big companies, right? But this is really fit for companies who, let's say meta, they build their own repository infrastructure, monoripple, things that they share externally. So they have the entire organization with hundreds of engineers just working on the infrastructure piece. And what is the best infrastructure to build today is definitely this, right? So large companies with more resources actually went pretty far. And they have the production volume to do this partial rollout to get the feedback. And they have so many products and features that they can experiment on.

**Aakash Gupta** (00:42:37)

But many people are probably watching and they're not at companies that have this at all. Although their engineering org might be accelerated by AI, the product org is not feeling it at all. The product org is not suddenly just submitting PRDs and they're getting billed by agents.

**Shuhao Zhang** (00:42:55)

I think this is, well, with every technological evolution will reset the market, right? I think this time the way to reset it is not only who builds a product that people love, it's going to be who really adopt this new way of building faster. And of course, the one that pretty holding on, holding back is going to see a very tough time in six months where everybody else is on a rocket and you're still walking.

**Aakash Gupta** (00:43:24)

Why is building fast in particular so important? Because I guess in the traditional sort of Marty Kagan sort of school of thought, it was always, well, building the right thing is more important. If you build fast, you could just ship a bunch of slop and then it could become a product experience people don't like.

**Shuhao Zhang** (00:43:39)

So first of all, building fast does not mean shipping slop, right? We're talking about production grade. So that's the tough part. That's where you need a lot of your products and engineering, especially the senior ones to think of. How to ship and operate production grades, the best-in-class services and products using agents. That's always the aura. And why building fastest matters today? If you think of why building the right thing is important in the past, it takes maybe six months to have a PRD. When you have every director's signature, I've gone through that time, right? And then you have the engineering, the ERD, right? That's another three to six months when you have architect design. Because, just because how costly building it is, It was back then. You want to build the right thing, right? But today, building it so fast, you don't want to spend a year just decide what to build.

**Shuhao Zhang** (00:44:42)

You want to spend as fast as possible to put it out. The best way to get the feedback is not a room of a PM's engineer sitting in a room in your own company. It's from the user, right? So things kind of reversed.

**Aakash Gupta** (00:44:55)

Can you show us what the right level and quality of input then from a product engineer, product team needs to be so that an agent can go out and operate correctly, like maybe what a quality PRD looks like?

**Shuhao Zhang** (00:45:10)

So this is a research agent. And I can just quickly scroll through the definition and you can see how sophisticated it is. It's quite in depth.

**Aakash Gupta** (00:45:29)

What I worry about when AI is writing these long documents is adrift. So how did you create that right alignment between what you wanted and what that document said?

**Shuhao Zhang** (00:45:37)

Yeah, so there are definitely multiple. You're going to layer them, right? So I have the PRD, and I also have the engineering plan. And you can see this is actually... Responding to the PRD, and then you have the implementation plan. So what happens is, again, this is something that you want your agent to work for hours and hours on top of, right? It's getting better and better to plan for a large-scale project. And it's going to actually have its own sub-agent planning. Okay, I'm going to build one component, and this is what I'm going to focus on. And you're going to have a bunch A bunch of sub-agents to kind of create these components together and then piece them in the end. So more granular, more detailed planning ahead does help. The reason when drift happens is agents start to make assumptions when things are not discussed, not documented.

**Shuhao Zhang** (00:46:46)

But when you have enough, large context is no longer a problem. And it really knows to read a certain part of the document and go back to work and come back to another part of the document.

**Aakash Gupta** (00:46:57)

Okay. And then to complete the teaching you were kind of doing for us earlier, the initial feature you were doing, you were going to push to staging. So what happens next? Like where are basically all the steps where human is in the loop?

**Shuhao Zhang** (00:47:10)

So after you push this to staging, again, staging is an environment almost identical with production. And usually, companies invest in building their staging environments to simulate the production environment, right? Just that you never school up the user's data and experience. Pushing from staging to production is actually a lot faster and easier after you have done enough tests because the environment is identical, you need to flip a certain flex, and again, the gradual rollout, partial rollouts, and that's it. So I spent more time in staging. And, you know, you have a dog footing if you have a UI components in your products, or you have load testing if it's a backend service. And again, AI is very good at that. Then when things look okay, you'll consider rolling out to production. And that's only beginning of the journey, you know, when then agents start to watch the observability and, you know, Start to make improvements again.

**Aakash Gupta** (00:48:16)

And what about the part where a human would typically look at the results of the future and say, do we really want to keep this in the product even? Do we want to do more here? How much have you brought agents into that part of the process?

**Shuhao Zhang** (00:48:29)

Yeah, you definitely want to, as a human, you want to experience the product no matter what it is. So I can show this is This is our product. So one of the products, this is the model router I talked about. And initially this is, the color scheme is not this, right? It's green. And Tinyfish color scheme is already So this is the miss in the initial design with the agents. And this is the part where you really want to kind of go in play and see if the playground works when it shows different models. And then you can see how this works. Latency feels like it's a human. Definitely the latency is all captured in the traces and the matrix, but you still want to kind of get a human touch. You want to try different things. We also have a type We have a test automation agent that can open a browser and click around because Tinyfish is a web agent.

**Shuhao Zhang** (00:49:29)

So we can use our own products to do test automation for UI. Yeah, but a human has to experience and dog food. And then all of the findings can be collected and sent back to the coding agent again.

**Aakash Gupta** (00:49:45)

So what we've done so far in this episode is we've really helped those non-technical PM backgrounds get into all these technical concepts. So can you also explain for those who don't know the test automation and how that all works?

**Shuhao Zhang** (00:49:57)

Yeah, so test automation is really, you know, for all the code that either engineers or AI agents created, you need a way to test. And you don't want to test everything manually. It's just not scalable. You have anywhere between unit test to end-to-end integration test and then load test. Unit test will cover more smaller features, whether you can do one plus one correctly. And then you just have a ton of these unit tests Carving the low-level logic, the end-to-end test is more of how the user experience will be as a user. And that will not capture all the problems, but you kind of have a good idea of, as a user, will they easily run into problems or it's going to be okay. And load test, of course, is when you have a large volume in production, can your system hold? So AI agent is actually pretty good at creating all of these tests.

**Shuhao Zhang** (00:50:56)

You just need different set of infrastructure. And unit test is the most straightforward. It's just another set of coding. Load test is to kind of bring in simulation of traffic. And end-to-end test, you need some sort of agentic solution to be able to open a browser and then navigate.

**Aakash Gupta** (00:51:14)

Wow. Okay. So how technical do people need to be getting in order to use a system like this? Like there's probably some component where you have this really deep engineering background so you can go this technical, but how technical does one need to get to? I imagine they can partner with an engineer who is handling a lot of this and where do they need to get?

**Shuhao Zhang** (00:51:36)

Yeah, I think I really, if there's one takeaway from Disciples, I really want all the product builders, PMs, or, you know, you're interested in becoming one in this area, is don't be intimidated by... The amount of technologies and engineering requirements that pushing things into production sounds very scary when you have a large user base. It's a large user base, it's really...it's a reset. But you do need a good engineering partner, like you said. If you don't want to drive, you're going to have a friend who can drive. So it's really kind of knowing what's the high-level risks, what good looks like, what are the common practices. The unknown unknowns are usually very difficult, but if you have an engineering partner, they will kind of easily tell, okay, this is someone who does not have a technical background. What are the areas they may miss? And then let me fill that in.

**Shuhao Zhang** (00:52:39)

And when you have the right setup, hopefully your engineers are very supportive in the system. The ideal case is really the PM will spend a lot of time talking to the agents back and forth, define the requirements, and then give feedback in the lab test. The rest will be taken care of and supposed to be taken care of by your company's machinery.

**Aakash Gupta** (00:53:06)

So we started at the beginning with this idea of when you typically ship to feature, you'd leave an engineer hostile. You'd have to be holding them hostage because they would have to maintain that and know that and have the accountability around it. Is that now shifting to the PM? Is it the system? How do you make sure that that accountability still exists somewhere?

**Shuhao Zhang** (00:53:28)

Yeah, well, it's a spectrum, right? So traditionally, when you build something, you're responsible for it forever. And no matter if you have a dedicated support team, when it comes to tricky ones, it always comes to And then you have a limit, right? Then you start realizing someone spent half of their time maintaining and supporting what they built and eventually they may just be You can be able to run two services, two features at most, which is what I mean by holding someone hostage. It's not supposed to be that way. You always want to create, improve, innovate. So agents really going to play that role, holding the lights and keep improving. So I don't think it's also PM's job to do this either. PM's going to watch the market reaction and watching the top lines and see how we can enrich, improve the products and service, but not spending a lot of time on the low-level stuff.

**Aakash Gupta** (00:54:40)

So just to put it in concrete terms, what is your thought on where the role of PM begins and ends and developer begins and ends in this future? Because where really, if the engineers are building the system to allow PMs to build a bunch of features, one could forecast a potential future then where engineers more focused on like this infrastructure, the system to build the system. PMs are actually focused on inputting the system. So To build a particular feature, essentially, the amount of engineering you should need would be less. Is that true? Or have I played that out in the incorrect way? How would you react to that?

**Shuhao Zhang** (00:55:19)

Yeah, I think you're correct. But we are also in this amazing world when we don't really know what the models can do in six months. So whatever we say today could be different. But what I'm envisioning is really It's still the best time and it's going to be a better time for both engineers and PMs. What I mean by that is if you think of the amount of work that's really not adding much value done by these two professions in the past, 90% of those will be gone. And today you're seeing PMs or anyone that can build something and it looks amazing to show. But there will be a inflection point where PMs will continue to go back to Focus on the market, focus on the users and creating the right things. And building will just become even invisible. Today, you still need to prompt and do a lot and then work with cloud code.

**Shuhao Zhang** (00:56:21)

But there will be a point, I believe in the near future, you don't really need to see the cloud code session anymore. And PM is really going to use all the tools to know where the market goes. And the engineers will make sure the machinery behind the scene will be very competitive in wherever the landscape you're at. So they're still kind of going back to where they're really good at. But today we're kind of sort of seeing a mix, but I don't really want to mix building prototype, putting it out for a little bit as a real building. And if PM feel great about, okay, I can use Cloud Code to pull something out, I don't need an engineer, I think that needs to kind of change and you still need your engineers to think much bigger and how can you partner together to have this machinery.

**Aakash Gupta** (00:57:14)

One of the most interesting product philosophies you shared, and I would love to hear the next layer of the onion on, is this idea that, okay, the cost of building used to be astronomical. Now the cost of not building is astronomical.

**Shuhao Zhang** (00:57:29)

You know, there are so many reasons why we spend a lot of time finding out what the right things to build. We talked about that just now. But today, because of the cost of building, it's so low and it's going to be lower. And you're not the only one You're not the only one that is racing. So if you look around and people are launching much faster and at a higher quality and they keep the service up, keep improving in production, and you don't Don't build that muscle. So I think that's the real cost. It's not really that you're missing one product opportunity. It's really you're missing the opportunity to build this muscle and not having this capability in six months, I think, or a year. That time when you look back, you realize how much you missed and how hard it is to catch up.

**Aakash Gupta** (00:58:20)

So talk to us about how you embracing this early, how that has helped your growth. Like you guys have seen this basically hockey stick growth where you're going from 100K to 200K fast, but then you're going to 200 to 300 even faster and you continue to see that sort of exponential right now. Yeah. How has this way of building helped drive that?

**Shuhao Zhang** (00:58:40)

Yeah, so we see the hockey stick in, you know, we can correlate to a few events. But first of all, we really should consider agents as the new type of users. And there will be trillions of them. Every human will have a whole A whole bunch of agents. And these agents are going to be the smartest users. They will look for new products. They will have their own way of testing, not listening to the product owner's words. So we have that in mind. They even can check out the price, calculate everything and make decision. So we have that in mind. So it means you have a really picky user, that you have to be the best choice among the competition. So what we did in the beginning that really helped us is we adopt this improving in production, or you can call it the hill climbing in production, that we continuously to improve our service, especially Usually when we build a search, it's a web info company that will help agents to work with the web.

**Shuhao Zhang** (00:59:46)

There's a search, fetch, and then there's a web agent. And if you see the use cases coming from the other agents calling us, It's very diverse and versatile. And we ran into all kinds of edge cases, which is impossible to fix in the traditional way. So having this process running in production allows us to stay ahead of competition and allow the agents to build a reputation of, oh, tiny fish is the best in class for this particular job. And that's why we're seeing a lot of traffic from them.

**Aakash Gupta** (01:00:21)

So you built for AI agents. That sounds like one of the key unlocks here.

**Shuhao Zhang** (01:00:26)

Yeah, exactly. I think the services will become more headless and a few super agents will stay to continue to interact with the humans, the users, and becoming the gateway of all other services. So they are actually the ones that are making choices and decisions.

**Aakash Gupta** (01:00:47)

If people want to learn more, where can they find you online?

**Shuhao Zhang** (01:00:50)

They can go to tinyfish.ai. All right.

**Aakash Gupta** (01:00:53)

This has been a wealth of information. Not too many people are willing to open up their actual system, break it down in so much detail to help the rest of the community.

**Shuhao Zhang** (01:01:04)

Thank you so much. Thank you. This is really fun. And I look forward to comments and I want to exchange notes with the community. All right, guys, so drop it down below.

<!-- sponsor -->
**Aakash Gupta** (01:01:16)

What do you think you're doing that he might want to experiment with? We'll make sure he gets all of that feedback. You can reply to the email if you are just listening to this on Substack. Like something over 10,000 of you regularly every episode, by the way. So appreciate you guys. We will see you in the next one. Have a good one. I hope you learned as much from today's episode as I did. If you can do one thing that's totally free that would help the show, it would be to check that you're following on Apple and Spotify podcasts. Check that you've left ratings and reviews on those platforms. Check that you're subscribed on YouTube. Leave a like and a comment on this video, and then share it with your friends. We're trying to make better and better podcasts. After two years, we think we've gotten something pretty good going.

<!-- sponsor -->
**Aakash Gupta** (01:02:03)

So let us know what we can do to make it even better, who else we should interview, and we We'll put on the best shows we possibly can. Finally, don't forget my offer for the bundle. You get an entire year of my paid newsletter, plus my favorite AI tools, Bolt Up New, Airtable, Speechify, Descript, Magic Patterns, Linear, Dovetail, Arise, and Mobbin. That's $27,000 worth of value for just $150. So check that out at bundle.akashgu.com if it interests you, and I can't wait to share our next episode [music]
