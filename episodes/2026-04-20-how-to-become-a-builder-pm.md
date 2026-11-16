---
title: "How to Become a \"Builder PM\" with n8n, Claude Code, and OpenClaw | Mahesh Yadav (ex-Google, AWS, Meta, Microsoft; Founder LegalGraph AI)"
subtitle: "Everyone is changing their title from PM to \"product builder.\" What does that even mean, and how can you become one? Today, we answer everything"
date: "2026-04-20"
host: "Aakash Gupta"
guests: ["Mahesh Yadav"]
speaker_names: "inferred"
substack_url: "https://www.news.aakashg.com/p/how-to-become-a-builder-pm"
youtube_url: "https://www.youtube.com/watch?v=PL7908aNeSE"
duration: "01:36:49"
word_count: 16088
source: "Substack episode transcript (aired audio)"
---

# How to Become a "Builder PM" with n8n, Claude Code, and OpenClaw | Mahesh Yadav (ex-Google, AWS, Meta, Microsoft; Founder LegalGraph AI)

*Everyone is changing their title from PM to "product builder." What does that even mean, and how can you become one? Today, we answer everything*

**Mahesh Yadav** (00:00:00)

I would love to send this message to all PMs that this is our time to shine. There is a lot of misconception there that, you know, if you start using cloud code or if you configure open cloud, you become a builder PM.

**Aakash Gupta** (00:00:13)

Mahesh Yadav, who's been a PM everywhere. Microsoft, Amazon, Meta, last but not least Google. This is the time to build your own world and I believe in that future and that's why I left and I have zero regrets.

**Mahesh Yadav** (00:00:25)

If you know your skills, you can build it cloud code and delegate that work to agents. I don't know its limitations. It does anything that I want it to do. This is an open challenge I have given to anybody that if you can do a job, just tell me the job and this agent will do it better than you 365 days, 24 hours. everything which used to take you almost two to three months first to write the prd to get to mocks from mocks to a real working prototype from there to getting customers and seeing the signals all that is getting squeezed with this cloud code and you become the builder pm that the world needs the ability to sandbox these agents in a controlled way that's an unsolved problem and that i think is what i am excited about

**Aakash Gupta** (00:01:11)

Google isn't going to allow you to just give your company access to an open claw. Yeah, no, I 100%

**Mahesh Yadav** (00:01:18)

agree. I think the idea is...

<!-- sponsor -->
**Aakash Gupta** (00:01:33)

where if you become an anal subscriber to my newsletter, you get a full year free of the paid plans of Mobbin, Arise, RelayApp, Dovetail, Linear, Magic Patterns, DeepSky, ReforgeBuild, Descript, and Speechify. So be sure to check that out at bundle.akashg.com. And now into today's episode. PMs are now being asked to push PRs. PMs are being asked to code. This is the rise of the builder PM. But what is a builder PM? Today I have Mahesh Yadav who's been a PM everywhere. Microsoft, Amazon, Meta. He has seen everything. Last but not least, Google. So he has seen all the top AI companies. He has been an AI PM for a long time and now he's training AI PMs. And today he's gonna help you understand How do I become a builder PM? How do I use N8N? How do I use Cloud Code? How do I use OpenClaw in order to become a more effective and efficient PM, even if I'm not building AI features?

<!-- sponsor -->
**Aakash Gupta** (00:02:32)

Mahesh, everybody loved our last episode. Thanks for coming back.

**Mahesh Yadav** (00:02:35)

Oh, thank you for having me. And I think this is the time of urgency. So I would love to use your platform to send this message to all PMs that this is our time and we should be ready when this time arrived. I was always preparing for this time. And now the time is right for all the PMs to shine. It's just a little bit that we need to go learn. And if we learn what we need to learn, this is our moment.

**Aakash Gupta** (00:02:59)

So what is a builder PM and how does a PM become

**Mahesh Yadav** (00:03:02)

one? That's a very good question, right? I was always right, means I had an engineering background. I was not a traditional PM who came from a B school and then went to McKinsey and then became a PM. I had a very gradual move to PM. I was an engineer. And I was always building. And then I became a PM because I was always building what is customer wanted or working backward from customers rather than just building for the sake of building, which is very popular at Microsoft, if you don't know. So for me, a builder PM is like as PMs, we are always building. Our job is to build the right thing. And now, earlier, if you had the tools, you would have built the whole product. But it was very hard to build anything. Or you need at least three or six months of rigorous coding, testing, deployment, all that.

**Mahesh Yadav** (00:03:54)

It was needed to go build things. But in the new age, even like people who are engineers all along are saying that they are not writing code anymore. They are talking to customers and the cloud code does coding for them. In that age, the skill that becomes important is like what to build and what does customer want and that you have. And if you use on the right hand side the tools to do the right prototyping and then build at least the first version of your product, and you become the Builder PM that the world needs. And I think all of us need to grow into that, whether engineers, designers or PMs, because without that, we will not be able to diffuse the benefits of AI into economy. So for me, a Builder PM is somebody who has taken the responsibility to diffuse the benefits of this awesome AI we have today into into the economy so that we can all drive the benefits that large companies and research labs are putting so much money into to build.

**Mahesh Yadav** (00:05:00)

So for me, in a nutshell, BuildPM is somebody who can talk to customers, figure out what needs to be built, and build the first version and get to 10 customers without talking to any developer at all.

**Aakash Gupta** (00:05:13)

Amazing. Can you show us an action? What are the skills and concepts we need to understand in order to get there?

**Mahesh Yadav** (00:05:18)

Yeah, I think there is a lot of misconception there that, you know, if you start using cloud code or if you configure OpenClaw, you become a builder PM. I think the hype is right because this is the first time people see that they can manage their calendar. They can delegate work to other party or they can just say things and it just happens. But AI, my perspective, I've been in AI for the last 10 years and build things all along. I think just knowing the layers or understanding how these things work is the first step or of building these things. And for me, I start my journey with, and obviously you talked about a lot of tools. So I will start my journey in first understanding these concepts. So I will start in an earlier day, I will start with something like TensorFlow or PyTorch and understand what a model is or train a model and then inference a model.

**Mahesh Yadav** (00:06:16)

In the new world, in the agentic AI, I will start with something like NA10 and then go and say, hey, Okay, what is an agent? How it interacts with model? What is a model? What are the limitation of it? What is memory? What is tools? And maybe I can just show you if it's cool. Maybe I just share my screen and show you because it's not very hard to learn these things in N810. N810 has done a good job, to be honest. Maybe it's an obsolete tool in building workflows now with Cloud Code, but I think it's still an amazing tool to learn. So let me just share quickly with you what it takes to build or what are the components involved in building these agents. So just a revision from last time. If you look at last time, we

**Aakash Gupta** (00:07:06)

talked about this idea that as we grow as

**Mahesh Yadav** (00:07:09)

humans, a kid is born, they first need to have the knowledge of the world. So this is how the world works. I understand that and I can build my intelligence on that and I can also update it. And second, I need you to understand what is the current state of the world. So if I want to do anything, I want to know, we teach our kids all the time when they are born, we will say to them that, hey, this is hot, this is cold, all those signals, which is current state of the world. Yeah, we know that this is a thing that gives us power or this is where we cook, but this is the current state of the world. So this is your signals or memory tells you what is the current state of the world.

**Aakash Gupta** (00:08:05)

And then if you did a good job, you can

**Mahesh Yadav** (00:08:08)

ask your kids to get a glass of water for you. And that's the tools where they can use a tools like a glass and then open a tap and then move, hold it and get it back to you.

**Aakash Gupta** (00:08:21)

So that's the tools piece. And

**Mahesh Yadav** (00:08:23)

then we learn the guardrails, the laws, what is possible in this country. If you are moving on a road, then you need to look left and right. It's your responsibility, not the responsibility of the driver, especially on a busy road. So we tell our guardrails and laws. If we do all this and if we just replace humans here with a model, so this model is analogous to what you get from OpenAI or Anthropic or Google. The model is just the intelligence layer. It just trained to predict the next world and now have some reasoning. But you need all this harness harness or people call it scaffolding to actually build something that can solve problems or build impact for you. So this harness is called agents. And then we use these frameworks like N8N to

**Aakash Gupta** (00:09:27)

build these agents,

**Mahesh Yadav** (00:09:29)

right? And then if you look at every agent that we have built so far or what people have built has one of these four things in it or the good ones have all these things in it.

**Aakash Gupta** (00:09:40)

So

**Mahesh Yadav** (00:09:40)

let me show you like if you want to build these agents, what is the memory? Why you need this knowledge piece? What will happen if I don't add the knowledge? So let's spend like maybe 10 minutes and understand the basics first before we get into how can you automate your world with this latest agent on how you become a Builder PM. So in my story, I would say the first step of becoming a Builder PM is just getting into knowing the basics. So if you look at this, Maybe. So this is my just any 10. And what I'm doing here is maybe I start from scratch because what's the point of doing an Akash show with Nets? Let's do it without Nets because that's the Trumpies Act without Nets. So

**Aakash Gupta** (00:10:29)

on the

**Mahesh Yadav** (00:10:29)

right hand side, you just take an AI agent. And you search AI agent, you get an AI agent. So AI agent has a model, which is the intelligence layer, which I was just talking about. So now I can connecting an open AI chat model. You can pick any model you want. I will just save money because expensive models... So I'm going to be a little cheap here and pick the GPT 4.1 mini. So you can just pick that model. So now you got model. So this is the agent. This is like a little baby. It doesn't know anything about your world. And now it has intelligence. So, okay, if it has intelligence, we should be ready to go. So I can ask it some questions like, hi, what are neural networks? it can answer those questions. So now what happens is this goes to the agent, the agent calls the model, and one beautiful thing about this is that you can look at what the message was sent, what the input and output were from this screen here.

**Mahesh Yadav** (00:11:38)

It gave me an input, it gave me because it's trained on these things. But if I ask it very simple question like, hey, what is the, president trump said about ending the conflict in iran what do you think it will answer that question or not

**Aakash Gupta** (00:12:04)

it's training data probably ended in like 2023 let's see great

**Mahesh Yadav** (00:12:08)

answer let's see what happens i asked this question and It says, hey, my knowledge cutoff is June 2024 because you're cheap. You're picking a cheap model. So that means that it doesn't have that knowledge. So it can't answer the question. So maybe we need a tool for latest, greatest things. So let's give it a tool. And the tool can be Tavelli, which is a search tool. So this allows it to search the model to do things. So now I go and I say Tavelli. I think it's AVI. Yeah, this is the one. You got it.

<!-- sponsor -->
**Aakash Gupta** (00:12:46)

If you've been enjoying this episode today, Mahesh's classic whiteboard style, his awesome labs and demos, then you will love Mahesh's cohort based course. It has amongst the highest reviews on Maven and I challenge you to go check this yourself. His courses are always rated 4849. That's because of the 13 years in Big Tech at Microsoft Google, Amazon Meta. He's actually built the things. He's not just talking about it. And his course, everybody I know, my mentees who have taken this course have had a positive opinion of it because it is so interactive. You get the first principles that you're sensing from the podcast today. The coolest thing about his new course, building open clause and with Claude code is that you get a Mac mini. So take advantage, use the discount code that i have below in the description so you get a discount on his course get your mac mini better yet get your company to pay for it he's gonna teach you not just how to become a builder pm but he's gonna be in the trenches with you as he said he will even give you ai pm interview advice so it's all in one course to becoming an ai builder pm check that out on the link just below and back to today's episode Today's episode is brought to you by Amplitude.

<!-- sponsor -->
**Aakash Gupta** (00:13:56)

Replays of mobile user engagement are critical to building better products and experiences, but many session replay tools don't capture the full picture. Some tools take screenshots every second, leading to choppy replays and high storage costs from enormous capture sizes. Others use wireframes, but key moments go missing, creating gaps in your understanding. Neither approach gives you a truly mobile experience. Amplitude does things differently. Their mobile replays capture the full experience, every tap, every scroll, and every gesture, with no lag and no performance hit. It's the most accurate way to understand mobile behavior. See the full

**Mahesh Yadav** (00:14:33)

And on query, so now I'm adding a tool, I have my account, it will go do the search, it will take the query and where can you take the query? I can hard code the query or I can let the model define the query. So now I'm telling it that, hey, let the intelligence layer based on what user is asking define what you want to search on internet. So now we connected a tool and Let's go. So now I ask the same question again, which is what has said about ending the conflict in Iran and my spellings are you can see are not that great. But now it goes and now it's going to the search tool. It's doing some searching. Let's see what searching it is doing. Seems like it went to these website, it found information and then it went to a lot of website.

**Mahesh Yadav** (00:15:17)

It captured all the information and now it is able to answer the question. which is from President Donaldson stated that conflict could end at any moment based on his decision. He mentioned there is practically nothing left to target and all that. So a lot of excitement. I'm happy about that. So what has President Trump said? Okay, then if I ask it a question, which is, hey, what conflict am I talking about? You think that will work?

**Aakash Gupta** (00:15:46)

Oh, I don't know. It doesn't have memory, right?

**Mahesh Yadav** (00:15:49)

Yeah, you trained well. So if I ask it, what conflict? I don't see any previous mention of conflict in this conversation. Could you please provide more context or specific which conflict? So if you build an agent with a tool or intelligence, it will be a stupid agent because it doesn't have memory or it doesn't remember anything. Who wants to talk to a person who doesn't remember anything? So let's add a memory. So I will just add a simple memory, which what it does is it takes a session ID and remembers last five conversations.

**Aakash Gupta** (00:16:21)

Nice.

**Mahesh Yadav** (00:16:21)

So now you know what an agent is which is just scaffolding, but the real work is happening in intelligence, memory, or tools. So if I do the same query now and it say, hey, what is the President Trump ending the conflict in Iran, and then it will do the same thing, but this time you see it updates the memory. So it has put all the conversations, all the information in memory. And if I ask my question, which is, hey, what is the conflict I'm talking about? It goes in, it fetches this from the memory. Now it doesn't call the tool because it seems like I'm looking for information. You are referring to the conflict, especially in the military conflict on war situation began around February 2026. So that's what it takes. But maybe, Maybe you have a larger context. Maybe you have contracts in your company and you want to ask questions on those contracts because conflict in Iran is not going to make me money.

**Mahesh Yadav** (00:17:20)

But if I do good contracts, it will make a lot of money. So can I ask a question like, hey, what are the clauses or what are the payment terms impact of tariffs and war in Iran on Iran? payment term impacts of tariff and end of war on our contracts.

**Aakash Gupta** (00:17:50)

So I

**Mahesh Yadav** (00:17:50)

run a company and we have contracts all over the world. I want to know that. Will that work?

**Aakash Gupta** (00:17:57)

I guess right now we haven't given it like a RAG database, right, to our contracts?

**Mahesh Yadav** (00:18:01)

Yay. I think I got the best student there, right, who has all the right prompts. So now it goes in and it says, hey, I don't know or I will just hand you slate. The payment impact on tariffs and war on Iran contracts generally can include several key factor, increased cost, payment delays and all that, but it doesn't talk about my contracts. So I have another lab that we cover in our course where you can actually create a knowledge base or database of your knowledge, how your world works. So this is important because the world is working perfectly, how neural network works or world information. But your company information also needs to be executed or needs to be built. So what this does is, first one, you can upload contracts. So I will just execute this workflow. Here I can upload my contracts. So I will just upload a contract from my company.

**Mahesh Yadav** (00:19:01)

And what you will see is that it will go and create Great. Maybe we put this MSA in. So this is a master service agreement. And what it does is once I go submit, it goes and creates the chunks. Now you can see there is a data loader. You can see insert data. And now you're learning a new concept. how the data is getting into something that machines can understand. Because these agents or these machines don't understand, like you and me understand text. So now you're seeing something called an embedding model. The embedding model allows you to convert text into embeddings. You're also seeing something called a data loader. What is a data loader? Oh, it takes the type of data which is a binary, which is your input file, converts it into text and then does simple text splitting. Okay, maybe I can do custom splitting.

**Mahesh Yadav** (00:20:04)

Oh, so custom splitting you have to specify, but what's happening in simple one? Basically, it's taking 1000 character with 200 character overlaps. So it divides your whole file into 1000 characters and then it goes in and puts that into a database or it calls the embedding model which goes and creates this awesome database which is a RAG or retrieval augmented generation based database for you which we have the same database where we are entering this information and now if I go here and I ask the same question which is I execute this workflow and not this one, give me this one. And I go, I select this one, and I say execute workflow. Actually, not use this trigger. Just come here, and now I ask the same question which I was asking earlier. I can just say, hey, what is the value of contract? Does the payment term change due to war in on tariffs based on our MSA contracts?

**Mahesh Yadav** (00:21:25)

It goes in, it queries this tool, and this is where you have put all your information. So now it queries the tool, it extract all the Texas information from your document that you provided, so your knowledge. And it says the document does not specify any provision, so I think we are good whether it happens or not. And now this information comes from your knowledge. Similar to this, we also discuss The next stage of this learning is multi-agent systems. So single agent systems are great, but if you want to do real checks or real things, this is a multi-agent system that we build. We use the same constructs that we just discussed. And in this one, you see that you can send an email. So right now I can just send an email and ask this information, the same information by an email. So I have pasted that or I have published that flow.

**Mahesh Yadav** (00:22:20)

and I can just ask like I ask my lawyers. Now I can send this request and I say, hey, can you get me the risks in this contract before signing? So if you send me a contract, which I believe one day you should send me a contract. But right now, let's say you send me a contract, which is an NDA. Before signing, I will just send this email. If I send this email, what happens is this email hits this provider, which is my Gmail. And if you look at it, I will get this review contract key terms for this contract. Okay, if I get that, then what happens is that if you go to my workflow, I will show you in executions that in few seconds, you will see that it will get a new running. So it automatically triggers this. I need not to do anything.

**Mahesh Yadav** (00:23:12)

It's a published workflow. And now it's running. And when it is done, I will get a response which says that, hey, you got these risks, contract analysis report with all the risks in it. So now you start first understanding all these things, which is, hey, what does these agents do and how they work with your things behind the scenes? So these are the connectors, these are your agents. It has multi-agent system with playbooks or your database connected, and then it can do end-to-end work like humans do. The last thing I would love to show in N8N world, which I think all of the builders PM should go build is, this is great. All this is awesome. This is sending me risk. But what about evals? How are we going to evaluate these? Because These agents are not like us humans, which does a lot of self-evaluations.

**Mahesh Yadav** (00:24:09)

And you can't, if they do a bad job, you are going to get fired. They are not going to lose their job. Even if they lose their job, it's not good for you. So what is this is then, then we create this idea of ground truths. So what I have done here is I have taken this contract. And what I do is I say, hey, here are the terms that you need to look at. here is the correct value and whether there is a risk or not based on our playbook is also written from a real lawyer. Then you can create a workflow like this where you can run this normally in the daytime. What you do is during the day you can have your people submitting these files. You can find all the risk and the results are getting stored here. In evening what happens is, you evaluate these using the judge or risk categories and modifications and you get a fancy report.

**Mahesh Yadav** (00:25:10)

So let me just execute this. So not the eval trigger, but let's just first create this data. So if I go and execute this workflow, I can just upload a file and on that file, what it's going to do is it's going to extract these terms. So now, It's going to find the risk in this contract and submit our results according to the same key terms here. So it runs in automation and then it updates a file like a human will go find the risk but what it does is it will just get the results first. So now you will see once it is done these values will be populated here. So now it's just looking for governing law, justification, agreement terms and once it is done which is still executing Once it is done, you will see this file getting updated and you will get the results like a human would have done.

**Mahesh Yadav** (00:26:06)

First, it's extracting these values from the contract, then checking whether risk or not. it will justify why this is a risk and suggest a modification which allows you to take minimum risk if you sign this contract. This is what a lawyer does for you, by the way. They will look at your contract, compare it with some values, find whether risk or not, and then give you a justification why this is a risk and modification. They never justify the risk, by the way. So now you see automatically that you can see the risk. And once you see these risks, Then you can see the second part of this, which is you can run a quick eval on this by just going and changing it from form submission to eval. And now when I run it, what it does is it will go and run an automatic eval and suggest comparing to my ground truth here, which is my real values, and suggest that how much of this risk is correct, How much of justification is what a human or these modification is what a human will accept as is or they want to change?

**Mahesh Yadav** (00:27:18)

So you can run these evals also and Netan has this awesome tool. So now you run this flow and what it does is it will take it one row by one row. You run your evaluations and find whether the risk is good and what is the quality of modification suggested by the AI.

**Aakash Gupta** (00:27:35)

It

**Mahesh Yadav** (00:27:35)

will continue doing it. But if you can go to evaluation tab, I can show you some of the previous evaluations. So now you see that it goes through, runs row by row. And then eventually it's telling you that, hey, you have a risk. Quality is good. You're able to detect 80% of risk correctly. But your modification quality, the suggestions AI is making, is only 30% as good as a human would have done. So you have work to do. So now you understand as a PM or as anybody who wants to survive this build wave, that it's not very hard to go with something very small, bring your context, make it multi-agent because the world is multi-agent. And then run evaluations to make sure that before you deploy it, it's really good quality so that when it does a job or when it responds to these emails, it does a good job.

**Mahesh Yadav** (00:28:32)

So I got my analysis, which I sent earlier. So now it talks about all the findings. I need to set it up so that you can see it in a more formatting correctly. But I just built it for you to show it quickly. But you see that the whole flow worked and it does give you risk that this economy shall be governed or constructed in law of state of Delaware without regard of conflict of law principle. Delaware is neutral jury deduction under criteria of NDA. So it's talking about these things to you and giving you all the details.

**Aakash Gupta** (00:29:05)

Yeah. Okay. So

**Mahesh Yadav** (00:29:08)

this is what it takes to get first your footing on ground to get started with your building journey. So that's, people talk about this when people talk about AI a lot. They talk about, hey, AI is, you want to build a PM, just start with OpenClaw. My suggestion would be first understand

**Aakash Gupta** (00:29:30)

what is the hardness

**Mahesh Yadav** (00:29:31)

looks like? What is the hardness made up? Ideally understand how this model is built, what are neural networks, what are transformers? And we talk about that in a way that anybody can understand. But then understand the score folding at least because this is where things will break even if you're using cloud code or the cloud code constructs like, you know, context, model, compression, knowledge, memory. First play with them and see what they are. And that's your first step in getting into building knowledge. With AI.

**Aakash Gupta** (00:30:01)

When does

**Mahesh Yadav** (00:30:02)

N8N

**Aakash Gupta** (00:30:02)

fall short? When do you move beyond N8N?

**Mahesh Yadav** (00:30:05)

Yeah, so N8N is very like, I think it's more like a tool which allows you to get to your first 10 customers. I think it's a very powerful tool, especially with Webhook. When we did the last session, I showed you how can you create your backend in N8N without any code and connect it to a lovable or V0 frontend and then build the whole solution where you can click a button and something happens in N8N and you can debug everything without writing a single line of code. I think it's very powerful there. But then if you want to iterate, put things in production, if you want three people to contribute to your code, if you want to have a test set or want to put a container around it and put it into production and it doesn't support that. And if things fall short and the worst part of this is that there is no way for people to see the code and get to the code mode.

**Mahesh Yadav** (00:30:54)

Like we do this in our cohorts and after people want to get to the next stage, which is, hey, I've done this, but now I want to put this in code and share it with my team so that they can see if this is good quality, bad quality, to take it to hundreds of users or thousands of users in the most efficient or latency optimized way, then Aniton has no answer to those questions. So I think it just stops you beyond 10 customers. It's not the right tool I would recommend, and that's where I know what you want to get started with.

<!-- sponsor -->
**Aakash Gupta** (00:31:31)

Today's episode is brought to you by Jira Product Discovery. If you're like most product managers, you're probably in Jira, tracking tickets and managing the backlog. But what about everything that happens before delivery? Jira Product Discovery helps you move your discovery, prioritization, and even roadmapping work out of spreadsheets and into a purpose-built tool designed for product teams, capture insights, prioritize what matters, and create roadmaps You can easily tailor for any audience. And because it's built to work with Jira, everything stays connected from idea to delivery. Used by product teams at Canva, Deliveroo, and even The Economist. Check out why and try it for free today at Atlassian.com slash product dash discovery. That's A-T-L-A-S-S-I-A-N dot com slash product dash discovery. Jira product discovery. Build the right thing.

**Mahesh Yadav** (00:32:26)

Today's episode is brought to you by Naya One.

**Aakash Gupta** (00:32:29)

In tech buying, speed is survival. How fast you can get a product in front of customers decides if you will win. If it takes you nine months to buy one piece of tech, you're dead in the water. Right now, financial services are under pressure to get AI live. But in a regulated industry, the roadblocks are real. NIA1 changes that. Their air-gapped, cloud-agnostic sandbox lets you find, test, and validate new AI tools much faster. From months to weeks. From stuck to shipped. If you're ready to accelerate AI adoption, check out Naya One at nayaone.com. That's N-A-Y-A-O-N-E dot com slash A-A-K-A-S-H. I hope you're enjoying today's episode.

**Mahesh Yadav** (00:33:09)

Are you interested in becoming an AI? So check out our newsletter

**Aakash Gupta** (00:33:13)

articles if you want to see the quality of the type of thinking you'll get. one of my frequent collaborators pavel hern is the build labs leader so you're going to live build an air product with pavel's feedback if you take this aipm certificate so be sure to check that out be sure to use my code and my link in order to get a special discount and now back into today's episode Yes, it's the hottest tool on the market, Cloud Code. Please, Mahesh, show us when should we be using Cloud Code, how should we be using

**Mahesh Yadav** (00:34:03)

it? Yeah, I think you should spend a good two weeks in any 10, and beyond that, you should move to Cloud Code. Because I think what has happened is, with Cloud Code, And especially like in last, I would say three to six months, CloudCode is here for more than a year now. But in the last six months, there's just so much possibilities with CloudCode and co-work to build things and put things in production for you as well as your team. It's the same tool chain, which a person who has no coding experience can use, like building with skills, creating their sub-agents, hooks, and then scheduled jobs. And then on the right hand side is people who know how to code, who has always been coding for the rest of their lives. They also can build on top of what you provided. So this idea of having somebody to allocate or do work with, and then this idea of code is combined in cloud code.

**Mahesh Yadav** (00:35:02)

So I think it started with something that people wanted to do code with. But then this one thing they realize is, or we all realize is that, If you can build something that codes well, it can do any task well. And that is what cloud code is. And that's what I think why it's the hottest tool in the town.

**Aakash Gupta** (00:35:22)

And you talked at the beginning about needing to harness this moment. And Andrei Karpathy talked about something changed in December 2025. What exactly changed?

**Mahesh Yadav** (00:35:34)

Yeah. So I think this is like for me also, right? I mean, I'm contemplating this and I think still not have wrapped my head around it. What has changed is if you look at like last three years where I, I I was at Google and we were building AI, but I thought we are not building AI fast enough. So I left Google. I started on my own. I'm building this company where we thought we can go and automate a back office and build AI or the benefits AI faster than what I could do at Google. With my own agency, obviously Google is doing great with their agency. And if you look at all the companies in the last three years, what they did with AI is... They took these models that we had and if you take the examples of any company and I can put them what they do in this map.

**Mahesh Yadav** (00:36:23)

If you look at Gama, Gama did one thing, Gama said okay I am gonna go and connect these models with tools and make it very easy for you to create slides and then I will provide you connectors connectors to PDFs, connectors to everything so that you can go and publish this in PPTs or Google Slides or just PDFs. They just did one job. And this was I think now at billion dollar valuation. The second kind of company. So first kind of companies that you saw was these kind of companies which go and make the model and tool working and put a lot of connectors in place. So Gamma is there. The second kind companies said, hey, we're going to take this model, harness it to domain specific knowledge. So the Harvey's of the world, the Lagoras of the world went and said, hey, we're going to take this model and do the context engineering piece here and say, hey, we will context to the lawyers and solve their problems.

**Mahesh Yadav** (00:37:28)

And they become one to $10 billion companies in two years. And some just went in and provided signals and memory well. And then there were third kind of companies which said, hey, can we provide you frameworks to build this? Which is what you saw with Salesforce, Agent Force, Amazon Q. They said, we'll just help you build with all these things faster.

**Aakash Gupta** (00:37:54)

This

**Mahesh Yadav** (00:37:54)

was happening for the last two years. You will see a lot of companies just come out and every company was planning to do something like this. Then what happens is, there is something a breakthrough happens inside Anthropic where they are building just a tool for coding and they thought for doing coding let's just do one thing which is build the agent loop they called it agent loop and the idea is it will build the context it will take the actions which is all the connectors and tools And it will do the evaluations. And based on that, it can come back and keep doing that again and again. So now, what happens is, if you are a context company, Harvey, Lagora, if you are an action company, Gamma, if you are an eval company or you did evals to make sure that your actions and all this is good, all this is coming part of this product called Cloud Code.

**Mahesh Yadav** (00:39:05)

yep and now people realize that it's not only coding specific you can actually do work with it so then they release these plugins for legal marketing and sales and what happens is they are able to do a better job at context management taking actions and evaluations why because for context there is another unblock in this world which is what I thought of that like the best thing that will happen with these models but I thought maybe it is the browser where things will happen but where things happened is this idea of computer control and we all became normal because we thought these are coding tools so we gave them access to two things one your file system and second your bash commands This is how the whole world works. This is how if you're an engineer, you can control your computer and if you can control your computer and your browser and you can have access to your file system, you can do all the context management and with bash you can do all the actions and third it has the browser control as well.

**Mahesh Yadav** (00:40:22)

So now you have all the action powers. And on top of it, they have evaluations, which is they are saying, hey, I can do the lint checks, do rule based checks. I can go and do UI element checks in HTML. And I can do what I was showing you, which is these LLMs as a judge. And all this I am going to do. So you don't need a third party provider. You don't need Harvey. You don't need somebody to come in and do it for you. If you take co-work and if you use my tested skills, you can do it yourself. So this is first time that whole intelligence layer that we were talking about, which was Claude actually became the whole harness provider as well.

**Aakash Gupta** (00:41:17)

So

**Mahesh Yadav** (00:41:17)

this is entropic entering into everybody's lunch and saying, hey, we need the space of this also. And that 2 to 3 billion what you're seeing in cloud code is basically coming right now from these valuations, which these people thought that they can go solve for each customers. But now they can't solve because everything is mostly three things. So once you have this, then on top of it, you can connect. a UI layer or these three things how they are able to teach the world and obviously you have done a great job with all your podcasts in teaching the world these skills on top of it which is that anything that you want to do can be a skills anything and skills are powered by these action taking sub-agents which can be triggered by something called hooks and now you can schedule jobs with these people learning these on top of these computer control, which is powered by this context loop.

**Mahesh Yadav** (00:42:26)

And by the way, there is a bottom layer to this, which is these models like Opus 4.6 have grown and able to do long horizon jobs. What is that? They are trained in a way that they can run for three to six hours without breaking this is was not there if you looked at the matter benchmark the last six months ago the longest horizon job they can do is three minutes and this has gone exponentially last six months so you put a long horizon job you give me access to your bash file file system and then the users can create these skills naturally in English language you have unlocked what the human potential was logged inside these coding or some software or some software provider will go and do it for you now it's just a skill and if it is a good skill and if you know your skill and if you have your craft you can put it in a skill which can be paralyzed with sub-agents and triggered with events like hooks and then whole this operating system is available to everybody and I think that's what happened with Cloud Code Claude code people realize that they need not to do the hard piece of which I was showing you with the rag, what the chunk size needs to be.

**Mahesh Yadav** (00:43:49)

And this rag, we do it in our labs with N8N where I show people that it's so hard to do the right retrieval and check this right retrieval with evals. So you have to do agentic rag, then you have to do graph rag. All that now is the responsibility of Claude code. It goes, it gets the right context. If the context becomes too large, it compacts the context. all that is happening for you you need not to code for it you just pay for it and you pay by by like some 20 bucks or 200 bucks which harvey by the way was charging you ten thousand dollars to do so that's what every lawyer got now that's what every law firm has now and they are looking and saying maybe we don't need tools and that's how the Benefits of AI are getting diffused into economy with ClaudeCode, then Cowork.

**Mahesh Yadav** (00:44:43)

And maybe we can talk about OpenClaw next. But that's what changed for me six months ago when I actually took hold of ClaudeCode with the latest, greatest model. I tried ClaudeCode, by the way, and I was not very impressed with it. for doing things which are beyond coding and i was like yeah it's a good tool yeah but cursor does the same thing i have github copilot which i got for free because i'm microsoft you know so but then three months ago i went to cloud code once opus 4.6 came out and now it's a superpower i don't know its limitations it does anything that i wanted to do And that's why when I talk about it, people say that I'm scaring them to take my courses. My life is good without my courses, by the way. I'm just telling you that anything like when I looked at ChatGPT, I was very excited about it.

**Mahesh Yadav** (00:45:34)

When I looked at Lovable, I was excited. That was the second moment for me that yes, front end is a solved problem. And then I looked at Claude code and it seems like everything is a solved problem. It can replace anybody and this is an open challenge i have given to anybody that if you can do a job just tell me the job and this agent will do it better than you 365 days 24 hours and that's what we are playing with now right so that's the world you live in and this is moving each model this long horizon jobs are shifting to more and more jobs These context action evals are getting better inside. So you need not to worry about it. And more and more people are sharing their skills, their agents and their scaffolding. And this is the new scaffolding layer, which is a very thin layer in English.

**Mahesh Yadav** (00:46:25)

Rather than figuring out all RAG, all of this tool calling, all of that putting the guardrails, obviously guardrail is still your responsibility, but there is like at least you can rely on these companies to not screw up because that's the only thing they need to go solve next. So that's my take on the question, right, which is, hey, what has changed for all of us? What has changed for all of us is that if you know your skills, you can build it in cloud code and delegate that work to agents.

**Aakash Gupta** (00:46:58)

Can you show us this in action? What does that look like?

**Mahesh Yadav** (00:47:00)

Oh, you like action so much. Let me show you that also. And again, right, so there is one job I do, right, because I started my own company. I have, like, at this point, 20 people working with us and, Once you do that, you figure out that most of your time goes into reviews. So what I build for myself here is that what I was able to do with just, I just thought maybe I just do this. Let me share. As you can see, this is my screen. This is my co-work. I have a bunch of stuff going on. What people send me all the time is that they will send me a PRD for review. So now I have given the review job to my agent. how it works if you send me a prd i will just go and say hey or i can just start a new task and i will say hey and i will select my folder so this is co-work same like cloud code you can provide it a context so i will select my review call context i will change my model opus 4.6 is too expensive so let's do sonnet so So I will go to Sonnet because I'm paying them a lot.

**Mahesh Yadav** (00:48:11)

So they are like, let's eat his token with Opus and give him the best results. No, Sonnet is good enough. So I go to the review folder and now I can upload a file and say, hey, can you just put comments on it? So if the good model or before this, if you were doing something like this, what will happen is you have to go and create So now you can get, so this is a product two pager. We are just building a new product. This is live. And what happens here is that I can go and upload this file and then say, hey, can you use our checklist and review this file? Put comments as I would have done. So now if you look at this, this is some sophisticated tool that you need because now it needs my checklist, which I already provided in these reviews.

**Mahesh Yadav** (00:49:07)

But first it needs to build the context. It needs to understand. But now you need not to build the query engine, the query to knowledge mapping. Now it automatically finds out the skill which I have built. It's my PRD review skill. And then it goes to my reviews instructions. And then it's reading my checklist. And based on my checklist, which I have provided to it, It's going to review this file and then upload or put comments in it like I would have done. As I showed you earlier, I could have put this whole agent inside Slack, and somebody could have just asked my review, and this would have given a review in five minutes and saved me a bunch of time on basic things, which people forget, of course, because they are busy with their lives. So that's the

**Aakash Gupta** (00:49:52)

first. Can we see inside the PRD Review Checklist MD and see what that's all about?

**Mahesh Yadav** (00:49:57)

Definitely. So let's go to my VS Code. So second thing I do is, so the same folder, VS Code, and now you can see This is my checklist. So this is my checklist. I've created this with a lot of blood sweat, which is mostly prompting to . But I had a checklist before because I was very fanatic on how we should write our two pages. And I'm a big fan of Amazon PR facts. So I like that format because with one page, you can get a very gist of what's going on. So now this is our

**Aakash Gupta** (00:50:30)

checklist. Just based on where your face is now, can we move the camera down a little bit again? Oh. Thank you so much.

**Mahesh Yadav** (00:50:40)

Yeah, there is this circus we need to do because this mic thing today, right?

**Aakash Gupta** (00:50:44)

yes please thank you for

**Mahesh Yadav** (00:50:47)

pointing me thank you i have no clue because i get lost in these no no you're

**Aakash Gupta** (00:50:52)

killing it so we're just you're talking about how you built this blood sweat engineers prompting

**Mahesh Yadav** (00:50:57)

great so uh so this is like i'm a big fan of amazon prfx uh i have looked at all the prd formats and still stuck with that like we had one at meta and we had one at google but still i love this whole two-pager thing of a and this is a checklist you are looking at with all the things that are like it checks does the problem has urgency is clear is the solution differentiated from chat GPT copilots or commodity AI wrappers. So I have put my AI specific things here also because this is specific for building and evaluating AI tools. So I build it with lot of knowledge I have but obviously prompting. a lot as well, but I stand behind it. That's the deal. If you do what I have said here, you can be rejected. So as you have seen, so now what it is doing is, okay, good, I have read the checklist, the doc, let me unpack the docs, target it.

**Mahesh Yadav** (00:51:54)

Now let me inspect the documenter to find the right paragraphs to anchor each comments to. So now it's going and it's also going to use another skill that it has, which is updating Word documents. So it will go and comment inside the document. It will unpack the document. It will find which sections or which points it is having problem. So now it's saying all seven comments added. Now I need to insert the XML marker into document.xml to anchor each comment to its paragraphs. And once that is done, you will see a file which should look like this. So this is how it will go and say, okay, Mahesh has put this, which is market sizing is too broad. Moat is missing. Add section explaining defensible advantage. What are the steps at a dog or big for consulting firms from building this? AI failure modes are unaddressed.

**Mahesh Yadav** (00:52:53)

What happens when attribution is wrong? How do you handle misclassification of AI versus human work? So not only like some wishy-washy, real good comments, which I will put in. So that's your first step. Maybe you got it right. And maybe you didn't. Maybe. So if you go and build an agent, then... This should be it. If you build a chat chat, then this should be it. But then you will go and I look at this and I say, yeah, they did the good job, but I don't like this whole section wise. So then I will put another comment and I will say, hey, you know what? This thing is, this is more market specific. How can you make it? So now I am adding my comments and I'm saying it looks for PR fact for it right in that format. This means that heading problem and solution section without question answering here.

**Mahesh Yadav** (00:53:56)

Question and answer format. So it seems like format was not taken and that was not in R. So I added a new comment here.

**Aakash Gupta** (00:54:03)

Okay.

**Mahesh Yadav** (00:54:04)

The beautiful part earlier was that, yes, it did the job, but obviously it might miss few things and today I have a very different angle. One day I go and comment everything, one day I don't comment anything. So today I want to push AI. The idea is that if AI does our work, what are we going to do? We're going to do and push it even further. So now I'm doing my job, which is I'm saying, hey, you go this comment and then I look at this and I say why this problem is hard. General observability tool don't understand. Workflow multi-step multi-tool. Adoption is invisible. This is too broad. So I can say, hey, this is too broad. This is too broad. Make it point. Make it point to human story as what happens to CXOs when they can't see impact. of their AI investments. Great.

**Mahesh Yadav** (00:55:12)

So now I have put two comments. So this was output file that you got, and now you got this whole thing. Then what I build on this is that I said, great, now AI does the review work for me because I have these skills, I have put my instructions in the cloud code, and it does the work. But if you have somebody who is working for you, or if you work in real environments, you've wanted to learn from it every day. So for that, I build another skill and other sub agent, which is what it does is it goes in and I have scheduled them to go and check for my review comments. So what this one does is it goes and runs every two hours or every 30 minutes and checks. What are the comments I am adding? It automatically is scheduled. It looks in the same folder where in the reviews I'm putting all my things.

**Mahesh Yadav** (00:56:10)

And it goes and then what it does is it creates this file called learner.md. And it learns from my patterns.

**Aakash Gupta** (00:56:20)

So

**Mahesh Yadav** (00:56:20)

now if you look, it's updating this file, which is a learner.md, which Cloud Code did not provide it. This is what as a human I added. So it goes... and put all my files, first every day whenever this job is done, because I'm a PM, I do a good job of organizing things because I need to evaluate, because I understand these concepts. So every time a job is done, it creates a folder here which says who did the job, what was the job about, when it happened. And inside that, it creates this, that this is the checklist I used, this was the input document, this is the output document, and this is what the user modified document looks like. So it creates all the artifacts, so if you want to go back, check, you have all the data that you need to debug or see what happened in this story.

**Mahesh Yadav** (00:57:15)

And then, each 30 minutes, Claude goes and compares these two files and creates this learner.md file which says, hey, I looked at this job folder and user added these comments. And with that, I have these new learnings. What I got right, what I missed, and these are the checklists that I want to go and update in the checklist. But it doesn't go and update it right away. I have another skill that sees the patterns here and if it finds it for five days, it sends me an email. And says, hey, I want to upload your checklist. I have seen that you revised this many times. You have updated the same comment five times today or five times in past week. Do you want me to update the checklist? Here is the updated checklist. And I quickly review it. And then my new checklist comes into life.

**Mahesh Yadav** (00:58:10)

So now I have.

**Aakash Gupta** (00:58:11)

How does that look?

**Mahesh Yadav** (00:58:13)

Yeah, so that is the PRD review checklist. This checklist and then you will see versions of this checklist, which is getting stored above this whole thing. So there is a master version and then there is a version that is in works. So now, if you look at it, what I'm trying to do is, okay, because I'm human right and I have to push beyond what these folks have already solved for so what they have solved for is you can create these skills but they are pretty static this is what basically I think all the people are trying to solve for let me just fix the camera first okay so if you look at it what I'm trying to solve is

**Aakash Gupta** (00:59:03)

let's start here

**Mahesh Yadav** (00:59:07)

Okay, then what I'm trying to solve for is that, yes, this agent loop can solve the world hunger, but it can't solve my hunger. So what I have done is I, as Mahesh, call this agent loop. We take the learnings of this, which is the learners.md. And then I have my agent, which sits on top of it. which is inside machine, so this is Mahesh, box is AI and it goes and checks the work done by this agent loop in those folders and then keep updating my comments or my work every day and creates this learner.md which updates the checklist which is an input to this loop, not without my feedback, with my feedback. So now I have created a continuous learning loop. So now every day, now what happens is every day when you come in and I use this system, my reviewer is going to be better than Akash reviewer or

**Aakash Gupta** (01:00:23)

anybody's else reviewer or cloud code reviewer because it

**Mahesh Yadav** (01:00:27)

has learned from my best practices and everybody who's improving this file maybe five people comment on this file my organization has a different soul we care about different things and now all this can also be contributed if we build on top of the agent loop which is bringing our own context and this is the idea of continuous learners which i have like first step today but there is more obviously we all can follow but that's not coming inside the loop this is outside the loop that i'm trying to build with this learner checklist and feedback And once you do that, you can adapt these continuously. Now you have a continuous learner like humans. So you and me go to any company like this podcast and last time to this time, I'm improvising based on the feedback you gave me and based on the comments all of you gave me.

**Mahesh Yadav** (01:01:22)

Same way, these agents are also learning now based on what you provide as feedbacks, which is very natural. We are not asking you thumbs up and thumbs down. We're just asking you to do the job that you gave it to us. And if you added to that job, the next time we will do better. So keep doing your jobs. Keep these agents along with you and they will learn your world. And every day they will get better and push you to push you to even get better at your job. And that I think is a dream for all people. Like if you have a craft and if somebody is there to learn from your craft from you and then push you further. I think that's the dream humans always had.

**Aakash Gupta** (01:02:03)

So we got a preview into PRD Commons, but what else should PMs be using cloud code to do?

**Mahesh Yadav** (01:02:10)

I think first is like do your first thing, which is like you started in any 10, then you created your first agent, which you were able to do a normal job that you're doing every day. Like for me, PRD reviews was the thing for you. Maybe writing PRDs is the thing and you to do that first job. But then after that, I think the genie is out of the box. Let me show you what PMs do and what we help PMs do in our cohort. So what happens is once you understand all these cool things that they exist, then what can you do with these? You can just go. So this is our first lab that you can use. which says, hey, creating agents in Cloud Code, we talk about all the basic things that you need to do. And this one just does competitive analysis.

**Mahesh Yadav** (01:02:54)

So this is building your own competitive analyzer. So it will go research the web and gives you insight. So this is a lab which we give our creating sub-agents. Here you create sub-agents, which basically what they are doing is We have a lot of sub-agents now inside Cloud Code and they will go and look at different competitors you have and what's the insider news, what's the outsider news and generate a report for you. Oh, that's not enough. Then this one allows you to create mocks. Once you do your user research, market research, you can create PRDs in Cloud Code, but you can create mocks and visualization which earlier you were waiting for your design teams to do. But that's not fun, maybe. Maybe you can clone your mocks from the source and then modify the mocks to build an end-to-end prototype of your product. So now here we build a whole product from the mocks.

**Mahesh Yadav** (01:03:51)

So we take these screens and we modify them and build an end-to-end working prototype that you can publish and customers can feel, touch and give you feedback. Not in mocks, as a real product. And then you can analyze data. So you can see who is using, how they are using, where things are failing. So then we give you this lab which allows you to not only just give you data but also analyze this data and create fancy dashboards which shows you how many contracts have been analyzed, what is the processing time, what is the average rating, compliance rate, bug reports, all. So your app gathers the data and now you are creating these dashboards. So everything which used to take you almost two to three months first to write the PRD to get to mocks, from mocks to a real working prototype, from there to getting customers and seeing the signals, all that is getting squeezed with this Cloud Code.

**Mahesh Yadav** (01:04:50)

And all this you can do with Cloud Code. And we give you labs for that. And the labs are public. So for all Akas audience, we will even do one hour free sessions. Whatever it takes, because the mission is to make sure that everybody can build in this new age because there is a lot of spend on these. This technology is very expensive. And if we can't build, if we can't diffuse the benefits of this technology to economy, we all are going to fail. So with that, at least I will do my part and Akashi is doing his part by allowing all of us this platform to spread whatever we have learned or whatever we have seen out there.

**Aakash Gupta** (01:05:30)

So Cloud Code, it's obviously great. It's a session-based power tool. What are the limitations of Cloud Code, and when should PMs be thinking about using OpenCloud?

**Mahesh Yadav** (01:05:41)

Oh, another one. So this is an amazing session. We start with like chatbots, then we go to NA10s, then we go to Cloud Code. And now the most beautiful thing called OpenClaw. So as we talked about this agentic loop, right? What happened? This is another exciting thing that happened in December. And generally what happens is November, December, people get time to actually do things and like sit down and not just run through these errands of life. So what happened with that is, that Peter who is a developer

**Aakash Gupta** (01:06:15)

from Australia by the way

**Mahesh Yadav** (01:06:16)

and all these things needs to come from developers and not from big companies that's the one pattern you are seeing that the big breakthrough came from chat GPT which is like an open AI one team few people launch something in and then they could see amazing thing happen similarly loveable a team outside US just build something and became overnight sensation. And then you saw OpenClaw. So what is OpenClaw? So OpenClaw said, hey, now this agentic loop is open. Anybody can build on it. So initially what they said is OpenClawed because this agentic loop is coming in agent SDK. So I can write the same tool like Cowork or Claude code. Anybody can write that And the beautiful part is that it can connect to any model. So when Claude built it or Anthropic built it, the agentic SDK was open that it doesn't only work with Claude models.

**Mahesh Yadav** (01:07:18)

It can work with any models. So what he did is he said, this loop is great, but people are having problems connecting to different channels. So first layer, what he did is he connected to these channels, which is WhatsApp, Signal and Slack.

**Aakash Gupta** (01:07:44)

Telegram and everything. Yeah. And at this point, like hundreds of these.

**Mahesh Yadav** (01:07:48)

And then he created this gateway, which automatically opens a port. and make sure that these are good so he did the hard work of taking the formats and making sure that all can be processed and then what I was passing through my email when I get this example you were sending this email but I was passing it to the model he takes all these inputs or puts this agent SDK and then says hey this is the intelligence layer and now anybody sending me these messages here I will process it here and then Come back and you can connect your tools. You can connect your models. Same way. And all this is coming as one thing called open cloud. And by the way, I'm going to open source all of this and give everybody free access to it. So it's not tied to any company. It's out there.

**Mahesh Yadav** (01:08:48)

Anybody can audit it. it's not something. So this is the first version of open Claude. So he said, I'm going to open source Claude, which by the way, like today, yesterday, the code got leaked, but this is the code getting leaked in a very nice way. And now if you look at it, because it's developed by a developer and because it has two things that Claude code didn't have at that time. One, it allowed everybody to just go and delegate work to it so as you were talking about like the session the idea of cloud code was that it was built for developers and developer does iterations but here there was not iterations here what they did is they did delegate the work so you can delegate the work I will go do the work and when the work is done I will come back to you And you need not to bother about it because I'm directly coming to you through your channels and you need not to be in terminal with me and go back and forth.

**Mahesh Yadav** (01:09:52)

So one idea is the delegation idea. Second idea is this idea of a shell or this sandbox. So instead of you giving me permissions on every file, every folder, why can't you just install me on a machine? So install me on a Mac mini. That's why Mac mini is out of orders or three weeks delay now. Because

**Aakash Gupta** (01:10:15)

if I can install

**Mahesh Yadav** (01:10:16)

this,

**Aakash Gupta** (01:10:17)

this is the new operating system.

**Mahesh Yadav** (01:10:21)

These tools became the UI or the mouse clickable things that you can assign things and now this whole compute works for you. And the third unlock was you can connect any model and even open source models and you are no more tied to the limits that cloud code basically everybody's hitting every day. So

**Aakash Gupta** (01:10:41)

now

**Mahesh Yadav** (01:10:41)

you can tied it to any open source model.

**Aakash Gupta** (01:10:44)

that is open claw for you

**Mahesh Yadav** (01:10:47)

so open claw one so this is the template that you will see everywhere now so this template is gonna be the next operating system if my predictions have been right and I'm predicting all these trends all along by the way I've said agents will be great in 2023 then I said hey you know what we are going to go to multi-agent and orchestration in 2025 and this year I've been saying that this pattern that you have seen here will be copied all over again and again and again and everybody will build on top of

**Aakash Gupta** (01:11:22)

these so now

**Mahesh Yadav** (01:11:24)

this is the new agent declare or this is the new agent definition and now you can give the work And the work is getting done by the agent and you get the output back. So you can measure input and output rather than measuring tools, evaluations and all. So that's open claw for you. And you can just see it in action as well, because I know you will just say, hey, can you show me in action? So I have

**Aakash Gupta** (01:11:53)

transition.

**Mahesh Yadav** (01:11:54)

Now I know, right? I've done it enough times with you. So what I have done is I have, by the way, I have my Mac mini here also. But for today, what I have done is I have done simple installation because it's hard to just show you my Mac mini and there is just a lot of things going on that which I can't share a lot about. But what there is another way to put Mac mini or open claw beyond Mac mini is this UTM. So on your Mac machine, you can create this new VM using this. tool and I have my whole setup by the way we have labs for these so you can see that this is my session you can see my overview you can see which channels I have connected I have connected only WhatsApp as a channel and now you can see my usage of it which is pretty okay because this is not what I use daily the daily is in the Mac mini and then you can set up cron jobs which is like scheduled jobs you can define your agent skill nodes here also so how How can you delegate work?

**Mahesh Yadav** (01:12:56)

Okay. I can just go in here. I can go to my WhatsApp and I can just start chatting with it. I can say, hey, do a deep research on what is agentic loop and long horizon jobs capability. and how they can impact software market. Give me full report. By the way, I can say all this through my command line as well. So it goes in now. What it is doing is it's going to process this request and give me results. This is me sending a message on WhatsApp to a friend or to an agent on the other side of the world. You see that it says, hey, here is the agentic loop. Introduction, landscape, emergence of autonomous software agents, increased demand, companies leveraging. And this is just vanilla. I have not even put my skills and everything that I have put on others. But now you can just put a channel.

**Mahesh Yadav** (01:14:08)

And in 30 minutes, we give you labs as well. So for this also, we have set up labs where you can go and create your whole. Just give me one second, I think. Those are... Okay, this is coming down. Open Claw. So... Here also, we have labs for you where you can go and set it up with WhatsApp, but you can also automate all of your world using this lab where you can connect your Gmail, which I have connected to my Mac mini, which I couldn't show because just there is so much personal stuff, but you can connect and make it your personal assistant. You can let it manage your calendar by step by step following this guide. Second thing, what we have done on this one is that you can go and create a whole discovery process or whole autonomous developer for you which goes and scans your GitHub and then fixes the bugs that are P2 or P3 for you and then send a PR request to your development team.

**Mahesh Yadav** (01:15:28)

So now if they are becoming a threat to you, you are becoming a threat to them. So you can build the whole lab where it scans your GitHub First, the agent goes and does tests for your UI or a new feature, then file the bugs, and then instead of assigning these bugs to developers, it goes and tries to fix the bugs as well, and then send a pull request for final approval to engineering because they still control the code. But you can build all that in OpenClaw. I'm also building a mini-PM in OpenClaw, which will do all the PM's jobs, but first I thought maybe I should build the dev because that's what is scarcity for me. Maybe the engineers are building mini PM. So that's open claw. If you can take these kind of a structure, you can set and assign work to it through the channels that you are already familiar with.

**Mahesh Yadav** (01:16:17)

And then you can have this idea of this whole sandboxing or controlling a whole machine to itself. And you're just giving it that work and then permissions to go access it to do your jobs.

**Aakash Gupta** (01:16:33)

So you've been a PM at all these big tech companies like Google. Let's be real, right? Google isn't going to allow you to just give your company access to an open claw. How should a PM at a big company mitigate security concerns? How should they be using this latest technology?

**Mahesh Yadav** (01:16:50)

Yeah, no, I 100% agree. I think the idea is not like, open claw is not a technology. It's not a product. It's a pattern. For me, it's a pattern on how these agents can be useful with an agentic loop. And they will copy the pattern and offer you in a sandbox way, which can be inside their anti-gravity or inside their Gmail workspace or on GCP. So in GCP, if you ask somebody today and say, hey, my Kubernetes cluster is down. I can't debug that today. But with this pattern now, this message will be sent to their sandbox VM, which will be running OpenClaw or some version of similar pattern. And now it will go and simulate first to their Kubernetes cluster, try to make the same deployment, and then debug it. First reproduce the whole problem. And that's what people do. Like as humans, we will first try to reproduce that problem.

**Mahesh Yadav** (01:17:47)

We will try to make the same cluster, do it. But these agents can't do it. Single loops can't do it. But now we can do it because we have the full control on a full machine. And now the agent can create, reproduce your problem, suggest a solution, try the solution, and then come back to you. And that pattern on that VM is fully controlled by Google. And as a user, all you are seeing is I provided a solution to your problem. But you don't know that I tested it, but now I can test it. That I think is what I am excited about. Obviously, there are challenges all around the security layer, which I think you already talked about in your podcasts earlier where a lot of skills, a lot of attacks around those. But I think once you sandbox it, which I think is the next big thing.

**Mahesh Yadav** (01:18:41)

Now, what is left? We have the agent loop, we have the whole pattern, then what is left? I think the ability to sandbox these agents in a controlled way, that's an unsolved problem. And Google will solve it. And I think OpenAI is solving it. And that's what you saw with MyManus also. By the way, this idea of OpenClaw is not new. Like MyManus, the personal agent company, gave you a VM and they ran their code. And if you look at it, last I looked at it, I can actually log into that VM and start doing web browsing on their VM or do whatever I wanted to that VM. So this was like this idea of enabling a lot of possibilities was always there. Open Cloud just made it so popular or so famous because it was open source. So Google will bring it to their companies in their sandboxes and solve end-to-end problems which humans used to do on their laptops and then dismantle that based on each query or each problem they solve.

**Aakash Gupta** (01:19:40)

So can you put it all together what we've learned today? How do we... organize this knowledge? What drawers do we put it in? Where does basic knowledge about ChatGPT and N8N agents, Cloud Code and OpenCloud, how does it all come together to create that Builder PM?

**Mahesh Yadav** (01:19:58)

Yeah, that's a great question. So you said a lot of things. How can I just have a plan for it? So I think first two to three weeks, just understand the basics. Without that, you won't be able to leverage or even understand it will become overwhelming being once you reach the open close stage. So I spend with my people, like people who join our cohort, I spend like first six weeks with them explaining them what the models is, what the intelligence or knowledge is, how these tools actually are working. So spend that first three weeks, then get to cloud code or co-work and automate your world. which is whatever you do now agent should be doing and you should be building systems, which basically allow agents to continuously learn or follow your patterns, which was two things in my example today, my checklist and my learner.

**Mahesh Yadav** (01:20:49)

And then this human in loop pattern, which was update everything every night, but keep me in loop. So that the second thing I would love you to build as a second pattern, stage and third thing i would love you to spend another month on is just understand in and out of open clock and see how can you have one thing in your lifetime in your job that you can just give it to a machine and the machine does the work and give you results somewhere else and the whole machine will be controlled by this agent, give permissions left and right, make sure that you are not giving permissions to your world, just create a separate world for this and then see if you can delegate work and get it done. And once you have done these three things, then just read obviously your newsletter or take any product and see is it a variant of OpenClaw or agent loop or it is something that is starting from scratch like model knowledge.

**Mahesh Yadav** (01:21:50)

And then you will be able to see what are the possibilities that exist out there and which possibilities work for your company, for your feature, for your product that you're going to build next. And that's your next three weeks. So this is like three weeks, first four weeks, then three weeks, then two weeks. So you're looking at nine to ten weeks of a good product. work through of building with AI or becoming a Builder PM.

**Aakash Gupta** (01:22:20)

So you became a Builder PM. Now you're trying to interview for the role. How has the PM interview changed with AI? What should PMs expect in the new AI PM interviews?

**Mahesh Yadav** (01:22:32)

Yeah, I think there is one thing that I would love to share with everybody because I'm doing a lot of research on this and a lot of people are coming to me every day. My calendar is booked for 15 minutes calls. I do four of those with our cohort members, just 15 minutes because they have interviews and I don't charge for it if you have done our cohort because I just want to help and I want to stay updated as well on what's happening. So let me tell you like three things that are happening. One is this idea, especially for level five, level six, AI rules, that idea of doing normal product sense is gone. You will be given a problem and you will be asked to solve it either in a case study or during your interview. That is becoming a pattern. And in that, people are trying to see, hey, do you understand?

**Mahesh Yadav** (01:23:19)

where we stand, how the world is working, or you are stuck in some past, like six months ago or one year ago past. So are you the person who is going to take us to the new world or drag us with the old world making old decisions? So that's what the first thing I'm going to check by giving you some assignment or by giving you case study or giving you a random problem. Second thing people are trying to assess is that, hey, have you done some kind of system design work Because still, there is a lot to even understand these things. So they will ask you questions on, hey, design a system for me. Here is a system design where you think the AI should improve with OpenClaw. Or where with Claude code-based agentic loop, how will you redesign the system? which people sometimes PM just come to me and they are like, we have this story where my wife was interviewing for an MBA job after doing her MBA.

**Mahesh Yadav** (01:24:18)

She's a very good software engineer. This was like a hybrid job and the recruiter asked her what are linked list or how to reverse a linked list, which is a very basic question for engineers. But she was like expecting an MBA question, so she put down the phone. She's like, I did the whole MBA, to get away from link list and here they are again. So some people get offended with these like, hey, why is a system design question for me in an AI PM interview or a PM interview and becoming normal? Because if you don't understand the design of these systems, you are going to not find the right capabilities that we should be building on. If you these tools are coming up every day and each design is elevating what's possible. But if you don't understand the design, you can't see what the possibilities are.

**Mahesh Yadav** (01:25:09)

That's why people are trying to test you there. So these are the two things. And beyond that, of course, like great product sense, great taste in the product, paying attention to detail. Those are not going anywhere. But these are the two new things that I will add. in testing whether you're a builder pm or not and i do that all the time like i if i give you a job and if you're not pulling out your cloud code or some kind of a tool like lovable you're already out like if you just ask me like hey can i do a drawing tool or can i create mocks in figma those are the things that are like done done i'm not interested so that's the new world

**Aakash Gupta** (01:25:51)

One of the distinctions that you make pretty frequently is this distinction between agentic AI versus AI specifically. So what is the difference? What do people need to understand?

**Mahesh Yadav** (01:26:02)

Yeah, so AI is this idea that you can find patterns. So this idea that we all have data. Machine learning helps you find patterns in data. AI helps you use those patterns and make money. Broader AI, like AI as an umbrella. And then agentic AI is the thing which allows you to actually take actions, do jobs, and finish work. So the idea is that agentic AI need to have like these three or four components which we talked about. Can I understand the world that I am living right now? Can I understand what's happening right now in that world? Building my context with these two. Once I have built, can I take actions now? which is running bash commands or calling tools or MCP servers. When I do that, can I run my own evals and make sure that I have achieved the goal or not? And if I have done all these three, then I am an agentic AI or product.

**Mahesh Yadav** (01:27:00)

Or if I just send you something like, hey, is it positive, negative emotion? Then I'm doing more like an AI thing, which is I can do one thing specifically. And if you send me in this format, then I will work else. Best of luck. That's the whole world of AI or cognitive services we used to talk in Microsoft about. But this is like a world where we are relying a lot on the model or this intelligence and giving it a loosely connected tools, knowledge, and memory, and then just trusting it to solve world hunger or any problem thrown at it. That's the agent TKI and that's where most of the excitement and money is today.

**Aakash Gupta** (01:27:41)

I want to ask you a couple hot personal questions. You spent 13 years in big tech. You started in Microsoft around 2012. You left Google in 2025. Can you share the honest, what can people expect in terms of total compensation trajectory? What was yours over those 13 years?

**Mahesh Yadav** (01:28:01)

Yeah, I think first it's pretty standard, right? You start with 120. I think AI worked very well for me. So I started with 120, spent all my life at Microsoft to grow it at 360, 400. And that time I felt like I have achieved Nirvana. This is like the best it can be. And then when I think it got a 70% bump when I joined Meta. And then another 70%. So this is all the AI that was there. So after that, I pretty much doubled my salary every year. Every two years, 18 months, every switch I made was a double salary switch. So if you end my last comp, it was looking at 1.3, 1.4 million is what you make easy at my level in my experience. If you're working in AI, This is not you applying for jobs, this is them saying, hey, we need you, we're doing this new thing, seems like you are the only one who have done this before.

**Mahesh Yadav** (01:28:56)

You tell us what you're getting, we will give you 30-40 percent on top of whatever you're making. Then you can say I need 100 percent and then generally they don't say no. And this is not only my story, right? All my friends who were at any stage, right? If they were in meta, they are working in NVIDIA today and their total comp is looking at 2, 2.5 million.

**Aakash Gupta** (01:29:19)

Wow, that's insane. So is that why you bounced around so much? Because I never see people who worked at all four companies.

**Mahesh Yadav** (01:29:27)

I wish, but it's not that, right? There was like, I loved Meta. So Meta was because I was just bored at Microsoft and I wanted to get out of Seattle because for personal reasons, I wanted to live in Bay Area. And so Meta was a great company and I would never left Meta, but Meta had this legal visa problem. So once I switched, I needed like my green card and need to switch my roles as like a product manager. And they couldn't do it because they had a USCIS case pending. So They couldn't file like my green card and I was in that line for 10 years. You might have known this a little that we stay. That's like one life thread that always running. So I gave them like good eight months to a year to resolve that USCIS case, but it was not moving anywhere.

**Mahesh Yadav** (01:30:14)

At that time, I needed to make a call. At the same time, I could admit that Bedrock at AWS was just building and they needed somebody and they threw a lot of money at me. So I could have waited more, but they didn't let me wait at all. So that was a big deal. And then Google was more like a dream company, to be honest. Like, My wife always told me that if you are a PM and if you have not worked at Google, you are not a PM, like that was her way of judging me. Because, you know, if you've done an MBA, so you need not to prove to the world. When you come from an engineering background and you become a product manager, you have to prove to the world that you are a legit product manager. You're not a developer, just wore a suit.

**Mahesh Yadav** (01:30:57)

So that was just that. And when they needed somebody who has built frameworks and actually built agents in 2024, That I think what got me and not my awesome frameworks or potify forces. It was mostly how much I knew about AI and so was my interview. My interview was very AI driven, what I have done in AI and how I can bring AI to production. That was my Google. First that comp and I think it was never driven by money. Otherwise, I would have never left. why

**Aakash Gupta** (01:31:35)

did you leave 1.3 at google when you left and it would be something like 2.5 2.6 now if you stayed and maybe jumped again so why did you leave what are you up to now

**Mahesh Yadav** (01:31:46)

yeah so idea is like i think these companies are going to throw a lot of money at you to keep you and then waste you So that was my observation, especially at Google, right? I think I'm away from them enough and I'm not going back ever. So the idea is that these are large companies. And if you look at like what happened in AI is large companies have not produced shit in AI. Like if you look at OpenAI, it was a small company which created ChatGPT. Then it was a small company, Loveable, that created Loveable. It didn't came out of Google. And then if you look at Claude code, it was created by a very small team inside Anthropic when Anthropic was not big. And then OpenClaw. So what has happened with AI is that tools are distributed, but these big companies have no environment to grow something which can be imagined Put in production and put in customer hands.

**Mahesh Yadav** (01:32:46)

I'm pretty sure I love people at Google. Most of the level three thinkers or level four thinkers live inside Google. I will go any day to stay even two hours with those people. I love them. But the company will never launch something like Open Claw. Something like this will be killed. Maybe you are thrown out of the company for trying something like Open Claw. So that's the kind of environment and that's the kind of guardrails they have put inside their whole ecosystem because it's such a big machine. Same as ChatGPT, right? Like if you look at OpenAI today, they have become so big and it's very hard for you to just come up with new ideas and throw it on Twitter and then take feedback and trade for six months. And then one day say, I have created something which is like some, I think, largest liked repo on GitHub.

**Mahesh Yadav** (01:33:37)

that is not possible and for me i reached a point in my life that i wanted to just stay unbounded as much as i could and i was very blessed that i had this course and that was giving me a lot of satisfaction of staying with people and not losing like one threat i had like money was like secondary to be honest main problem was that you You get so dependent on these institutions for learning, for staying up to date. I do miss, right? I will pay them today to be around Google, right? So that is the main thing. But for me, that course that I started teaching on Maven always helped me stay even up to date than what is there. So as you see, I have tried OpenClaw. I have built my mini PM. I would have done more here than what I would have done at Google.

**Mahesh Yadav** (01:34:26)

And given a choice, I will never go to Google again or to be honest, any company. They just kill every intelligence neuron you have. You won't believe that for a two-page document, you have to have a one-page of approvals. That takes six weeks. In six weeks, a non-builder PM becomes a builder PM. Then they can build anything they want ever. so that's the world we live in and these are the companies backward i know most of the people will watch this podcast with the branding of you know these big companies and the dream on how you get into i just want to assure you that there is more you have today than you will have once you start working at these companies especially in ai and especially for next two years this is the time to go build this is the time to build your own world And I believe in that future.

**Mahesh Yadav** (01:35:24)

And that's why I left. And I have zero regrets.

**Aakash Gupta** (01:35:28)

What a way to end it. Mahesh, this is amazing. Your last episode, it was crazy. I think in like the first two weeks or something, it hit 8,000 views. But every month since, it consistently gets 3,000 to 4,000 views because your content delivers. It's evergreen. And this episode was a perfect demonstration of that. Starting from first principles through to actions. Thank you so, so much.

**Mahesh Yadav** (01:35:53)

Oh, Akash, thanks a lot. I hope you

<!-- sponsor -->
**Aakash Gupta** (01:35:55)

enjoyed that episode. If you could take a moment to double check that you have followed on Apple and Spotify podcasts, subscribed on YouTube, left a rating or review on Apple or Spotify and commented on YouTube, all these things will help the algorithms and distribute the show to more and more people. As we distribute the show to more people, we can grow the show, improve the quality of the content and the production to get you better insights to stay ahead in your career. Finally, do check out my bundle at bundle.akashg.com. to get access to nine AI products for an entire year for free. This includes Dovetail, Mobbin, Linear, Reforge Build, Descript, and many other amazing tools that will help you as an AI product manager or builder succeed.

**Mahesh Yadav** (01:36:39)

I'll see you in the next episode.
