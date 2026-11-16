---
title: "FAANG PM Reveals How to Build AI Agents (and Get Paid $750K+)"
subtitle: "Free masterclass in Agent AI PM from a PM at Microsoft, Amazon, Google, and Meta"
date: "2025-09-13"
host: "Aakash Gupta"
guests: ["Mahesh Yadav"]
speaker_names: "substack"
substack_url: "https://www.news.aakashg.com/p/mahesh-yadav-podcast"
youtube_url: "https://www.youtube.com/watch?v=cddB0JA5kAg"
duration: "01:12:22"
word_count: 12378
source: "Substack episode transcript (aired audio)"
---

# FAANG PM Reveals How to Build AI Agents (and Get Paid $750K+)

*Free masterclass in Agent AI PM from a PM at Microsoft, Amazon, Google, and Meta*

**Aakash Gupta** (00:00:00)

The future of product management and building products is building AI agents. But most people are gatekeeping the knowledge.

**Mahesh Yadav** (00:00:07)

In past, a developer need to read 20 API documents, but now all you are doing is...

**Aakash Gupta** (00:00:12)

And then after that, you worked at so many of the other paying places.

**Mahesh Yadav** (00:00:16)

That's the old world. The new world

**Aakash Gupta** (00:00:17)

is Mahesh Yadav has been a product manager at Meta, Amazon, Microsoft, and Google. In today's episode, he's going to break down exactly how to build AI agents.

**Mahesh Yadav** (00:00:26)

So Microsoft is a dreamland for people who want to go build without caring how it will make business. That's the opposite of that, Amazon.

**Aakash Gupta** (00:00:34)

How did you get so good at the PM interview?

**Mahesh Yadav** (00:00:36)

These three skills were essential for being a successful PM.

**Aakash Gupta** (00:00:39)

The future of product development is agentic. You need to be able to build AI agents into your products. The AI agent PM role is one of the fastest growing and highest paying roles out there. These roles pay $750,000 plus. Today we're breaking down the exact 18 month roadmap you need

**Mahesh Yadav** (00:00:58)

Nobody can stop you. Next iteration, you are even doing better than their PMs. Google will hire you, right?

**Aakash Gupta** (00:01:02)

What do fang companies like Google look for in these interviews?

**Mahesh Yadav** (00:01:06)

All of us should build a reviewer. People who are new in AI lose a lot of their brand in the beginning. A

**Aakash Gupta** (00:01:11)

lot of people, they want to break into these companies. They want to get this 300,000 plus PM AI agent's job. So let's start with your own story. What is the salary and compensation for these AI agent PM roles? Mahesh Yadav is one of the most seasoned product leaders when it comes to AI agents, and so this episode is a masterclass. Without further ado, let's get right into it. Mahesh, what are we going to cover today?

**Mahesh Yadav** (00:01:40)

Today, I'm going to show you how you build agents, not only a fancy front-end in LoveAble, but also a back-end that you can scale with multi-agents. Also, I will talk about how to get 300K plus jobs in AI and especially agentic AI and share any secrets that I have learned throughout the years.

**Aakash Gupta** (00:01:59)

Amazing. What does it take to become an AI agent PM?

**Mahesh Yadav** (00:02:03)

Oh, I know it sounds hard, but it's three simple things. One, we are looking for people who have built in AI. Second, we are looking for people who have done AI PM transactions, which includes like how you dealt with data, how you dealt with models, evaluations, and scaling by iteration. And last is just generic skills around scale, ambiguity, and experimentation. Because this is new, and these three are becoming essential or table

**Aakash Gupta** (00:02:35)

stakes now. So I don't want people to have to wait too long. Let's get right into how to build these AI agents, both backend and frontend.

**Mahesh Yadav** (00:02:42)

Sounds like a plan. So I will be using two major tools. We do this with new people that we show them how can they build their AI agents. So for backend, I will be using this tool called Langflow. Langflow is a tool which allows you to build no code, highly complex or simple agents. So let's start building our backend first. And I will be building a simple tool which you can use for competitive analysis. So as a PM or as anybody who's trying to build or analyze markets, you need to analyze competition. So we'll be building a tool which allows you to do competitive analysis.

**Aakash Gupta** (00:03:19)

So to go through all this content, let's get started with building an AI agent, shall we? Yeah,

**Mahesh Yadav** (00:03:24)

that sounds amazing. So let me just tell you how we're going to build it. We're going to use Landflow, which is a no code tool. It allows you to build highly complex or simple agents without writing a single line of code. And for the front end, we will be using V0. This is like Lovieber or Bolt. You just write prompts and it creates an awesome web app or front end for you. Then I will show you how can you combine a very powerful backend in Langflow to a frontend in V0. So that's our

**Aakash Gupta** (00:03:53)

plan today. Perfect. And I'm just curious, before we even dive into that, how did you choose Langflow in V0?

**Mahesh Yadav** (00:04:01)

Yeah, that's a good question, right? So I think when I was starting, I was looking for no code tools because once you start writing code, you need to learn editor, you need to learn coding skills. And suddenly the barrier to entry is so large that most of the people doesn't cross that barrier. That's why I was looking for tools which are easy. So one is ease. Second is capability. So Landflow was quite capable. It had integration with all model providers. So I can choose Azure, AWS or Gemini, Google models. And third is this ability to get access to the code if we want to go to production. And that also was there. I also look at any 10 and there was one cool thing was that it was completely free and any 10 was charging like after two weeks and I didn't have a free subscription.

**Mahesh Yadav** (00:04:52)

So landed on land flow. Okay, then let's get started. So the first thing first, what you do is you can go to land flow dot debt. Land flow is this tool and data stacks is the company which bought land flow. And now IBM bought them. So it's a journey. You will see this happen again and again in AI. So what we will be building is a competitive analysis tool. You can get to Langflow. The first time you go, you might need to create an account or log in with your Google credentials. Then you will land here. You can just click new flow and choose simple agent. With this agent, you can actually build an end-to-end agent. So let me just get you started there. So this is a simple agent. You can use this. Or let's use this to create our own agent. So this one takes a URL input, a calculator input.

**Mahesh Yadav** (00:05:42)

And we are building a competitive analysis tool. So what we need as an input. And I think that's the first thing we all need to learn. If we can start talking in terms of input-output and what process or what things we need to process, that would be a good product requirements or an interview or a good way to handle an interview is, first up, anybody ask a question, see what are the inputs, what are the outputs. Yeah. And I jot it down for you guys. If you're building your agent, first step you need is you need which competitors you're going to compare. So you need an input as a name of your competitors. What tools your agent will be using. It needs at least a search tool so that it can do all the search on internet and find that information that you're looking for. And then obviously you need agent to process and which requires you to have a prompt with special instructions, which I will show you a little bit tips and tricks on writing these prompts.

**Mahesh Yadav** (00:06:38)

And then what is the output? So input is name of competitors and output hopefully would be a table format and tool is a search tool. Okay, great. If we need to build this, then let's go back to our Lang flow. And our input is basically twofold. So this agent, you can also drag and drop. So that was the cool thing I was talking about. So two inputs. So let's get those two inputs in. Text input. I will edit it. I will say competitor one, competitor A. And in the text input, I can just say open AI. Great. And then I can delete this. I'm not looking for chat input. And I can just control C, control V. And I can just say comp P. And let's compare that with Google. Because that's what it was created, hopefully. So in this case, we're a hypothetical PM where?

**Mahesh Yadav** (00:07:40)

You're a PM, which is trying to do a competitive analysis. across this company and let's say you're trying to see which APIs to use or which to invest in or you're looking at this company that you're starting a new model company and you're trying to see who out there in creating these models. Yeah. So maybe we need a new model which helps us because none of them are good enough anyways. Yep. So then you need a prompt. So you can put a prompt one. And now it requires you to copy, paste or get to your what message you want to write in your prompt. And prompt writing is the art, I think, these days.

**Aakash Gupta** (00:08:21)

Yeah, the system prompts in particular for your AI agent are everything.

**Mahesh Yadav** (00:08:27)

Let me just copy paste the prompt because I'm not going to type, but let me talk about what it does and how you can write a good prompt, a good prompt structure. The first thing you talk to your agent is your role. So you're saying, hey, you're a professional business analyst with expertise in corporate research and competitive benchmarking. Now your instructions compare the two companies given company A company B. These brackets are telling it that this information is coming from outside. Once you put it in bracket the prompt structure will change and it will open up two ports so that you can pass this information from outside. And taking help from Tavelli. Oh, what is Tavelli? I think it's a tool for doing AI's research or search. I will attach that in our flow in a second. And then put the structure in a markdown format that includes the following attributes.

**Mahesh Yadav** (00:09:16)

And then you're specifying exactly what you need in your world. These models don't know how your formats are, what your company needs, what your report needs. So give them very detailed instructions. And then this part, which is guardrails. So if I'm talking to you, or if I'm interviewing you, or if I'm seeing how good you know, if you have a good structure in your prompt, like role, instructions, guardrails, or even you can say tool sections specifically, I know that you have learned AI well. So these are the ones. So let's say that's our role, goal, and tools. Did I give company A, company B? And that automatically opened me these ports. These ports were not there earlier. And if you edit this and say company three, you will have another one.

**Mahesh Yadav** (00:10:06)

Now

**Mahesh Yadav** (00:10:07)

this input I can get from here. I connect this. I connect this. Great. And this

**Aakash Gupta** (00:10:15)

input as my friend. So the purpose of the text fields and making it company A, company B is so that you can change out what companies are there?

**Mahesh Yadav** (00:10:22)

Correct. And I will show you that you can take this from a front end as

**Aakash Gupta** (00:10:27)

well.

**Mahesh Yadav** (00:10:28)

Like the user can pass these. So you need not to show the user this whole back end thing or playground or this fancy thing. They will see a fancy website. They can put out two companies and they can get their analysis done.

**Aakash Gupta** (00:10:39)

Nice.

**Mahesh Yadav** (00:10:40)

And that's why this needs to be a separate input because this you are going to take from outside.

**Aakash Gupta** (00:10:45)

Yeah.

**Mahesh Yadav** (00:10:45)

Okay. Seems like we need a tool. And as I gave you a tip earlier, we are looking for a search tool. And Tavelli is an awesome tool because this is the search written for agents. What it does is it also takes out the URLs from the search, put the text out and then give it to the agent. So the agent can process a lot of text or that it got from the urls rather than just the urls because the urls are not very helpful okay so taveli is their third party tool which need an api key you can go to their website it's very simple so you can go to their website and say obviously everybody requires you to have a login but once you log in you can just click a button and they give you an api for free i hope this whole thing continues like this forever So you can just take the API.

**Mahesh Yadav** (00:11:37)

So now you can come and you can paste your API because your code needs that access to their API and change the mode to tool mode. You need not to pass the query and then you can connect the tool to the tool section. And now you have a fully capable agent which takes two inputs, which is competitor names. It has its instructions that goes to agent instructions. It uses this tool to do the search and gives you an awesome output. Ready to test? Maybe one last thing. It also needs an open API key. How you get an open API key? You can go to platforms. OpenAI. You can go to platform.openai.

**Aakash Gupta** (00:12:20)

I think I've exposed those before of my own. Oh, great.

**Mahesh Yadav** (00:12:25)

I think then I'm not the only one.

**Aakash Gupta** (00:12:27)

Then you

**Mahesh Yadav** (00:12:27)

go to billing. Make sure you have some money left. $6 is enough. $5 is generally enough. Then go to API keys. Create a new secret key. Put your test key name, say podcast and select a default project and create secret key. Once you have the key, you can copy it and come back to your flow, replace this one with your key. And that is all. This is what it takes to create an awesome agent, which is using tool, which is using prompts and giving you output.

**Aakash Gupta** (00:13:03)

Can we try a different model though, maybe instead of GPT-40? What if we try something else? Oh, it sounds like a plan.

**Mahesh Yadav** (00:13:10)

Maybe you want to change the model here. So, they're a model and it supports all OpenAI models. And by the way, it can also take Amazon, Anthropic and other models. But I just got the keys for OpenAI.

**Aakash Gupta** (00:13:21)

So, I'm

**Mahesh Yadav** (00:13:22)

just going to use OpenAI. But let's change this model name.

**Aakash Gupta** (00:13:25)

Maybe

**Mahesh Yadav** (00:13:25)

you want to change the model name from... GPT-40 to mini because you're doing experimentation and you don't want to be bankrupt trying a lot of things. So let's just, this is the smallest model with the smallest cost and the fastest results. So let's experiment with this one. If we don't get the highest quality.

**Aakash Gupta** (00:13:41)

Can we use

**Mahesh Yadav** (00:13:42)

GPT-5 over there? No, they don't support that yet. They don't support GPT-5 yet. Oh, that's sad. Okay. Awesome. So now I have changed it to GPT-40 mini.

**Aakash Gupta** (00:13:54)

And the limitation here is on lane flow side.

**Mahesh Yadav** (00:13:57)

Yeah, they have to expose it, right? So that's the problem.

**Aakash Gupta** (00:14:01)

That's what

**Mahesh Yadav** (00:14:01)

happens once you take abstractions, you lose something.

**Aakash Gupta** (00:14:04)

Yeah.

**Mahesh Yadav** (00:14:06)

So that's

**Aakash Gupta** (00:14:07)

maybe the one

**Mahesh Yadav** (00:14:07)

downside

**Aakash Gupta** (00:14:08)

here.

**Mahesh Yadav** (00:14:09)

Yep. That you need to rely on these things to do the same-day integrations. I think N8N... Okay. N8N has five... Yeah, I use it on five. Yeah, yeah. So I think it's like they have to get early access, right? Yeah. So they gave it to N8N. They didn't give it to this guy. So these guys are just like...

**Aakash Gupta** (00:14:29)

But that actually looked pretty good, that output, even though it was 4.0 Mini. Yeah.

**Mahesh Yadav** (00:14:33)

Yeah, yeah. Five doesn't change these basic things. To really evaluate the quality, you need very different things. I will stick to photo mini any day.

<!-- sponsor -->
**Aakash Gupta** (00:14:45)

today's episode is brought to you by maven the sponsor of this podcast and also the place where maven hosts his ai agent mastery course this course has been taken by hundreds of pms at some of the top companies in the world like google amazon meta netflix stripe and many others and it has amazing reviews in fact it has some of the best reviews of any maven course i've seen and people who in my community have taken the course have had great things to say so If you want to get $100 off of Mahesh's course, use code AkashXMaven. That's A-A-K-A-S-H XMaven. And if you're looking for a quick place to click into that where you don't even have to use that, go to maven.com slash X slash Akash. That's M-A-V-E-N dot com slash X slash A-A-K-A-S-H. Today's episode is brought to you by Miro. Let me ask you something.

**Aakash Gupta** (00:15:40)

How many tools are you juggling just to get a single project across the finish line? One for brainstorming, another for planning, something else for tracking tickets. That's where Miro comes in. It becomes an all-in-one collaboration workspace. Whether you're consolidating user research from several interviews, developing and synthesizing product briefs or a wireframe, or project managing development. Miro brings everyone into the same space. It's fast, intuitive, and fully loaded with features like project templates, two-way Jira Sync, and integration with software like Draw.io and PlantUML. Miro's AI features can be used to synthesize elements in a board to develop a ready-to-review product requirements document in seconds. If you're tired of tab overload and scattered workflows, try Miro. Head to Miro.com and see why over 90 million users choose Miro to guide from idea to outcome.

**Mahesh Yadav** (00:16:32)

Okay. Okay. Let's go back to the model changing piece, right? So, okay, then I just changed the model to GPT Forum Mini. This seems like it's ready. Let's test it out. So to test your agent on the backend, you can just click playground and you just click this button called run flow. And you see that it's processing the input. You can see what step it is taking, how much time it is taking. By the way, when it is doing that, you can see that where it is and you can see how much time it took across these things. And finally, when it is done, you can just see the results are here. I'm finished. And

**Mahesh Yadav** (00:17:11)

here is

**Mahesh Yadav** (00:17:11)

across these eight verticals your results. That's pretty cool. But maybe you want to launch this as a website in your team and don't want the world to know your secrets that you build it in like five minutes and the whole world is building it. So maybe... What you want to do is you want to create a fancy website which sends these two things. And now anybody in the world can use your tool to do this. So let me show you how you do that. So this is your backend. You can make it as complex as possible. This allows you to do RAG, multi-agents with crew AI. or we have labs where we have gone ahead and even put agentic rag with graph or did some fine-tuning also. For that, some other day. But today, let me just show you how can you take this and connect a lovable or V0-like agent with Landflow so that you can do all a fancy work on the front-end, but your back-end is where your AI is and that can remain separate.

**Mahesh Yadav** (00:18:16)

So for that, you need to do couple of things. So just follow along. If you click publish, you click API access. So they allow you to access this as an API, the whole flow. I'm ready to test this from outside. And to build this end-to-end, you will need the response also. For that, you can use this tool called Postman. Anybody I know, Postman is a tool which you can use to test back-end APIs. You go to Postman, first time maybe you need to log in. So once you know what command to send and what the response is, you can go to a tool like v0. And then... I'm going to give you a prompt. Build me a modern responsive landing page for a competitor comparison tool using provided APIs. It takes two inputs, company A and B and compare button. It calls APIs resolves Some issues like cores, which is cross-resource resolution.

**Mahesh Yadav** (00:19:14)

If one party calls the other party, there is a normal error you get. I put it as an error handling. I also tell it to do error handling. And that's pretty much it. And here, you need to response your command that you send. Okay?

**Mahesh Yadav** (00:19:29)

Yeah.

**Mahesh Yadav** (00:19:29)

It now can automatically figure out how to send this request automatically. And once it gets the response, it will show you in a very nice format, but it need to know how the server is going to respond. In past, a developer need to read maybe 20 API documents to get here. But now all you are doing is copy pasting the response. And that is it. You can send this request right now. And hopefully in two minutes, your front end will be ready and you will be ready to publish your app. So that's pretty much all it takes these days to build end-to-end apps with a solid back end with AI and a front end, which is a website which I will publish on my site, say Mahesh Yadav slash competitor analysis. And then as you guys respond, you say, I want this step. I want that step.

**Mahesh Yadav** (00:20:24)

I can keep it reading and keep building and eventually build the best competitive analysis tool the world has ever seen.

**Aakash Gupta** (00:20:31)

We have armed v0 with a really good prompt. And so we'll include that prompt for folks in the newsletter article so that you can just copy paste exactly what Mahesh used. But I think that what's probably most important there is it wasn't just a simple one line prompt, right? You had a lot of specific points you included. While we're waiting for this to outline, can we just cover what were those like four or five key points in that prompt again?

**Mahesh Yadav** (00:20:56)

Sure. So that prompt, by the way, I went ahead and did something more for Akash

**Mahesh Yadav** (00:21:02)

and

**Mahesh Yadav** (00:21:03)

his listeners. So what I did is, because it could be audio, I have created this whole lab with screenshots and everything. And we are open sourcing this. So you will get this link. This allows you to step by step follow what I am doing.

**Aakash Gupta** (00:21:15)

I

**Mahesh Yadav** (00:21:16)

like V0, by the way, you were asking earlier, they give you a lot more credits. because i've tried the same thing with lovable and the credits were going over very quickly so if you want to do just free stuff or do prototyping try v0 if lovable you don't want to pay them their credits are really good i could build like two apps and everything remains here awesome i got my compare companies with intelligent insights And give me an example of meta or anthropic. Maybe I can try something. So let's try. And you will see, like, it may not work out of the box. And there is a debugging experience in Vype coding, which you can do now. So what you can say is, OK, company A can be, let's say, Google. And let's say, Microsoft.

**Aakash Gupta** (00:22:07)

Or what if we give it a harder one? Let's do Mistral, M-I-S-T-R-A-L.

**Aakash Gupta** (00:22:11)

sure i wish

**Mahesh Yadav** (00:22:15)

like this is like if you would have written the code or if you are supposed to write the code you worry about these things a lot but now who cares all we have to do is just modify the prompt so

**Mahesh Yadav** (00:22:24)

try

**Mahesh Yadav** (00:22:25)

everything now you have full control right and at this point it's sending that request out and it might take couple of iterations iterations for us to get it working it might fail it's like

**Aakash Gupta** (00:22:35)

stop showing the load No,

**Mahesh Yadav** (00:22:36)

no, it came like

**Aakash Gupta** (00:22:37)

Google

**Mahesh Yadav** (00:22:38)

versus Mistral. Google started in 2023. Arthur Manich is the emerging player in AI. Venture back, privately held. Makes sense.

<!-- sponsor -->
**Aakash Gupta** (00:22:48)

Today's episode is brought to you by the experimentation platform Chameleon. 9 out of 10 companies that see themselves as industry leaders and expect to grow this year say experimentation is critical to their business. But most companies still fail at it. Why? Because most experiments require too much developer involvement. Chameleon handles experimentation differently. It enables product and growth teams to create and test prototypes in minutes with prompt based experimentation. You describe what you want. Chameleon builds a variation of your webpage, lets you target a cohort of users, choose KPIs, and runs the experiment for you. Prompt-based experimentation makes what used to take days of developer time turn into minutes. Try prompt-based experimentation on your own web apps. Visit chameleon.com slash prompt to join the waitlist. That's K-A-M-E-L-E-O-O-N dot com slash prompt. AI evals are one of the most important skills for PMs. And I know you know they matter.

<!-- sponsor -->
**Aakash Gupta** (00:23:45)

The question is, are you doing them right? Most teams are winging it with basic metrics and hoping for the best. Meanwhile, the teams that actually ship reliable AI, they've cracked the code on systematic evaluation. Today's episode is brought to you by the AI evals for engineers and PMs course by Hamil Hussain and Shreya Shankar. This live Maven course will teach you the battle-tested frameworks from Hamil and Shreya, who are the engineers behind GitHub Copilot's evaluation system and 25-plus production AI implementations. Four weeks, live instruction, next cohort starts July 21st. Today's episode is brought to you by Amplitude. Replays of mobile user engagement are critical to building better products and experiences. but many session replay tools don't capture the full picture. Some tools take screenshots every second, leading to choppy replays and high storage costs from enormous capture sizes. Others use wireframes, but key moments go missing, creating gaps in your understanding.

**Aakash Gupta** (00:25:02)

Neither approach gives you a truly mobile experience. Amplitude does things differently. Their mobile replays capture the full experience, every tap, every scroll, and every gesture, with no lag and no performance hit. It's the most accurate way to understand mobile behavior. See the full story with amplitude. So now we've got it. So I guess let's publish this, right? How do we go to the final step?

**Mahesh Yadav** (00:25:24)

Yeah. So you can go and say publish to production.

**Aakash Gupta** (00:25:27)

So what makes what we just built an AI agent versus a regular AI product?

**Mahesh Yadav** (00:25:32)

Yeah, I think that's a good question. What makes it an AI agent is three things. One is that it uses tools. Second, if you look at the instructions, it is taking a role and a goal. And unless that goal is achieved, it will keep on trying things and it won't fail. And third, which we have not done is connecting knowledge. And just, I said three, but one more is the guardrails. It can put its checks. So it can assign things and it can have like feeling and it can also have memory. So it can do many interactions, learn from each iteration. And then keep on improving until you achieve your goal. And that's an agentic capability, which is not an AI capability. AI services are more of you give me speech and I give you a text back. It is only single purpose. Here it's doing competitive analysis and you can keep sending different companies, different verticals, and it will continue to do that thing.

**Mahesh Yadav** (00:26:36)

And it can fail, but it will recover and you need not to worry about it. So that's how you build an AI, end-to-end AI agent. You go, you build your back-end where you have full control in things like Langflow, NITN, where you can drag and drop, but you can build complex things like tools calling, prompt engineering, or knowledge. or putting your guardrails and making it multi-agents and then coming and showing, connecting them to a fancy or full control web app, which sends these requests, analyzes and gives you a result in your format. And anybody can try it over internet. So this is how you build and explore with AI agentic first prototypes.

**Aakash Gupta** (00:27:21)

So we helped people build an AI agent. How did we come to this place? What's the architecture of an AI agent?

**Mahesh Yadav** (00:27:27)

a short history of agentic AI. Let's talk about that because I was lucky enough to start or been working in agentic AI for a while and this is the first time. You see that everybody can remember that moment when you first time heard about ChatGPT. It was such a compelling proposition that you took your data to the product. That has never happened in AI before. By the way, I was trying to sell AI based products. seven or six years before ChatGPT and we have to sign hundreds of NDAs, go through corporate loops to get people data. But this was one product where people actually took their data and copy-pasted in ChatGPT and said, analyze it for me. So that was the moment where we started seeing success in chatbots. This is where we solved the Q&A problem. And in 2023, what happened is we said, okay, you need not to take your data to chat GPT.

**Mahesh Yadav** (00:28:21)

The big giants woke up like Amazon, Google, or Microsoft, and they launched some version of Copilot in their products. So now you can have the product, you can write, swipe and ask questions or do things which were not possible before. And then 2024, we made reintroduce agents. I was lucky enough to work on the first framework to build agents at AWS. And there we said, okay, Q&A is cool, but what about I let you connect tools or make changes in the world or change the state of the world by calling APIs, doing search, writing code, all these tools, if you connect to these Q&A machines, can they start doing things? And that's agents. And then in 2025, we are making them multi-agent and multi-modal. What does that mean? That it only not take text, but can take images, which I was showing you on V0, that how can I just paste a picture and say, hey, make it look like Gartner's website.

**Mahesh Yadav** (00:29:26)

Or I can just send my save through audio also. So we are making it multimodal. Also, we are saying not a single agent is enough. Maybe connect many agents to do complex things. One good example of multi-agent is the AI coding agents. This is not a single agent. One agent is thinking, the other agent is writing the code, other agent is testing, and all that combined are able to do complex things. That's what is so exciting. So we have gone from simple chatbots, which were amazing, can summarize, can generate poems and all, to fully blown multi-agents which can write code like all of us do, create web apps, or do PhD level research for us. So that's our journey so far.

**Aakash Gupta** (00:30:15)

So that covers the history of agentic AI. Now let's talk about these vibe coding interviews, these AI coding interviews. We just demoed an end-to-end workflow for people. A lot of people are going to need to execute these in interviews because places like Google are bringing on these interviews. You worked at Google. You helped them write some of their first AI guidelines. What do fame companies like Google look for in these interviews?

**Mahesh Yadav** (00:30:37)

That's a great question. And AI is new, right? So what we are looking for people is that have actually built in AI. Because what we want to avoid is people who are setting the expectation too high or setting them too low. And we don't really care. We understand that you have not worked in production. But have you actually built an end-to-end workflow and maybe 10 people tried it? How many iterations of that? So we are looking for builders and not people who know just frameworks and emotion. So that's the most exciting part for people like me. Second thing we're looking for people who have done interactions in AI specific world. Let me explain. What that world looks for is, do you have sense of how to interact or get your data or handle data responsibly? Can you understand how these models are designed and which models are good at what?

**Mahesh Yadav** (00:31:28)

Can you evaluate an agent or AI or can you work in iterations? And third, I earlier talked about, which is how much things have you achieved at scale? Not in AI, maybe with some other example, you can bring your cloud scale or if you pivoted in mobile. But we're looking for people who have seen one technology transaction going from one change, which is big enough, and how they handled it. And if you have two of these, I think you're a really good chance to get into any of the bank companies because they are desperate to, to be honest.

**Aakash Gupta** (00:32:05)

So this PM interview type that is spotted up, this vibe coding interview, they often ask you to vibe code live in the interview. What's the right way to handle this interview type? What's the right framework and structure to ace it?

**Mahesh Yadav** (00:32:17)

Yeah, I think that's a very good question. And I think it's being perceived differently. So let me tell you my take on this. So I think when we are asking you to vibe code or when anybody asks you to do vibe coding, the requirements has not changed. We are not looking for your technical skills of how good you write code or do you understand what is written. What we are looking for is what are you adding in your code? It's just an easy way for us to create something together and help me judge how you think as a product manager. So when you're vibe coding, do not forget your product principle. That's my lesson number one. Second thing, please play with these tools. They're not very hard. So what I'm looking for there is like the prompt I showed. Do you structure your prompt? And that tells me that, yes, you have done some interactions with AI.

**Mahesh Yadav** (00:33:05)

And second, you understand the limitations of these models that they can't take humbo-jumbo instructions correctly. So this is the second thing I think people are looking for vibe coding. And third is, more than you just show me how cool this thing is, you show me these iterations. That tells me what is your taste. So I'm looking for two things, to be honest. I'm looking for taste. And can you improve with iterations? Can you evaluate? and then improve it so show me maybe three things one show me how how you think and show me in your prompt how you think second once you build it show me what kind of user insights you are bringing in your second iteration and hopefully third iteration show me some feedback loops that i will make for this which shows me that you have a sense of data and ai in you And I think that could be a very good interview or three-step framework that people are looking for when we ask you to vibe code.

**Mahesh Yadav** (00:34:03)

So just take it like a canvas, I would say. to show your PM skills.

**Aakash Gupta** (00:34:08)

One of the things that we talked about in the pre-show conversations we were having for folks was this idea of cart before the horse development. I loved your take on this. What is cart before the horse development?

**Mahesh Yadav** (00:34:19)

I think now all of the PMs can hate me after this. But the idea is this, right? The idea is that PMs, just every room they go to, they stop engineers saying that, hey, this is us and we will tell you don't put cart before the horse. But in AI, that's changing because that's the whole idea of having a PM because they decide like where the horse goes and then build the cart. But to be honest, I think this is the first time we are actually in a position to change that idea a little bit. Because what's happening is three things. One is the cost of prototyping has gone 100x lower in last two years itself. So building something as you saw is very cheap and anybody can do that. That's number one. Second, the customers really don't know what to expect out of AI. And third is, there's this idea that so many possibilities, so many ideas, so many things are possible.

**Mahesh Yadav** (00:35:15)

And if you're going to do six months of research to figure out which problem to solve, maybe somebody who did something else will solve it before then. So this FOMO factor. So these are the three changes. And what it is doing to our industry or what is, it's changing the expectation from PM from saying, hey, I will take this. So old method is, I take this problem. I do a research three months. I write this awesome piece called PRD. In another two months, I get these approvals in two months and then I hand it over to engineering and hopefully I will show up when business needs me or when it is done in another six months and we launch one product or one feature every year and I get promoted. That's the old world. The new world is the PM actually talks to customer two weeks, three weeks, creates a prototype.

**Mahesh Yadav** (00:36:07)

Show them what's possible. And then iterate on the prototype maybe for two or three weeks. Then write a very small PRD with detailed user experience that this is what happens on this click. This is what we should show. This is what we should show. A clear user experience with ideally some prompts. And then evaluations, which is how we're going to evaluate what is the quality expectation. And with these three things, they can hand it over to engineering. Engineer makes it possible and make it production ready. And then you iterate every three months and in a year, you have built a product and actually made it make money and made it what exactly you could never think or nobody will ever tell if you have not done that. And that's the new way of doing AI PMing or PMing. And in this case, you're building the cart first and then working with the customers to figure out where the horses will go.

**Mahesh Yadav** (00:37:09)

And that's the idea of cart first AI product development.

**Aakash Gupta** (00:37:15)

Love that. So I want to shift a little bit into how you broke into Fang because a lot of people, they want to break into these companies. They want to get this 300,000 plus PM AI agents job. So let's start with your own story. How did you break into AI at Microsoft? I believe this was back in 2016.

**Mahesh Yadav** (00:37:33)

Yeah, no, I think very good question, right? So I think first is having an intuition for a new technology. I had that. I was working in Azure IoT, and I thought maybe this idea that you can, instead of hard coding or doing logic-based programming, this whole ML thing will be a cool thing. But as you may all be feeling, there is not easy to enter. There are barriers of... terms like you know gradient descent local minima math you need to be this research scientist it was even worse in 2016 and for me i just wanted it so desperately that i started hanging out around microsoft research campus i offered my services on friday saturday for free and then i came up with one idea of building a vision ai dev kit which was a camera that can inference on edge, but train in cloud. And I offered that to our Azure machine learning team.

**Mahesh Yadav** (00:38:34)

And I was a dev then. And they said, you need to test. And in Microsoft, if they tell you to test, it's not a good deal. But I took anything. I said, yeah, I will test it. And in three months, some people dropped something. I took on that code, then code. And eventually I became the TL for that. I shipped that product end to end. And that was my story. I was the guy who actually built Vision AI DevKit and shipped it end to end to production. Satya took it in our 2017 or 2018 build on stage. And after that, it's just a story from there. I knew a lot of things like I knew how chips acceleration work. I knew different architectures. I knew how to train them in cloud. I knew how to optimize them to run on small hardware. and after that it just iterations and I think after that it just becomes like once it's like a marathon where a lot of people run with you and if you get to do the first good project you get a good lead and from there you can run the marathon correctly or without like running into people or getting stopped every five minutes because nobody's moving in front of you So my two tips out of my own experience is be ruthless and passionate.

**Mahesh Yadav** (00:39:52)

Take anything that's coming in ML and AI your way or create your own paths. And once you have them, don't take them for granted. Work twice or three times harder once you have those opportunities. And I'm pretty sure it will change your life. It has changed mine since I was able to double my salary every other year after that.

**Aakash Gupta** (00:40:12)

Wow, that's insane. Talk us through how you made it from dev to PM.

**Mahesh Yadav** (00:40:17)

You have really good questions for me. So when I was doing this Vision AI, I also realized this another insight, which was in AI, I believe that building things will get easier and easier. But what to build and how to work closely with customers to build the right thing. would be a skill or would be a thing that will save a lot of time for organizations or developer time and to be honest I hated like what PMs did because they could just tell me and then I have to spend six months and I couldn't like question a lot so but I found them like little vague so I never wanted to get into PMs But the stakes were so high for me that I did like two iterations and things didn't work out. And I don't want to blame anyone. So I said, okay, let me figure out.

**Mahesh Yadav** (00:41:10)

And my God, it's so hard to figure out what's the right thing to build. It's super easy when somebody tells you what to build to build it. But figuring out what is the right thing to build, especially for a large company when the stakes are higher and your role is little, like you get into L7 levels. you're playing with at least 300 to 400 people's life and you're almost playing with 50 to $60 million worth of decisions you are making. So why I started? I started out because I wanted to make sure that we are building the right things. And I think what I loved about it is learning how to build the right things, which I'm still trying to figure out.

**Aakash Gupta** (00:41:51)

How do you architect that internal transfer though? Some people, they just get stuck in the engineering ladder. They can't make it into the product management ladder.

**Mahesh Yadav** (00:41:58)

Oh, yeah, I think that's a very good question. And I've seen that. I've seen a lot of my friends who actually wanted to become PMs, but nobody made it. And I was trying to stay back. And the PM manager actually said, Mahesh, I want you in my team. Can you join my team? And I said, no, I can't join your team because my visa has this, you know, pram, all the thing that happened in US. But he kept pushing, insisting on me. And why? To answer your question, because I was super passionate about customers. I was working backward from there. I was there to solve the problems. I could prototype real quickly. And I cared about business. I cared about making money for the company. I cared about what will matter when all AI dust will settle. And that was 2018. This is not like, now it's just a store, not dust.

**Mahesh Yadav** (00:42:53)

But I cared about these three things, which is, hey, are we building the right thing for our customers? Is it going to make money for us? And how can we bring people together to build it? And I think these three skills were essential for being a successful PM. And if you show that to people, if you do that without giving that, it does require time, effort and energy, to be honest, because I need to still code. But I went ahead and did that anyways, because I wanted to code what will matter, not code what things won't matter. So I think those three things, and if you are struggling, start doing these three things, which means writing a lot about what is the problem, how many, just don't write PRDs because your PM friends will get offended. But write your customer insight. So I had this customer insight newsletter I started.

**Mahesh Yadav** (00:43:46)

And

**Mahesh Yadav** (00:43:47)

because I was debugging each customer problem with Vision AI DevKit, I will write as if like I talk to them, this is their problem. This is the model they are using. This is why this fails. This is what our system have gaps. This is what AI as a whole has gaps. And that's why I just patched it right now. But this could be the next thing for us. One example of that is Onyx. Like we build it out means, you know, you don't know what to build because you're cool, you're new PM. So we said, you know what, we're going to kill NVIDIA and we're going to build it on Intel chips. So when I went to Azure Stack, which is this idea that you can run AI on premise rather than sending everything to cloud. That time we were dealing with government contracts. And we took Intel FPGA chips for that design, not NVIDIA.

**Mahesh Yadav** (00:44:44)

And then I learned quickly that these architectures, like that time we were doing vision models, so MobileNet, YOLO, and each time there was a new architecture comes, Intel can't catch up and it works out of box in NVIDIA. So I wrote these and then we came up with this idea of ONIX, which is Open Neural Network Exchange. And the idea is that Microsoft built a layer which allowed any architecture to automatically done accelerated computing across any chips. So you can train a model in TensorFlow or PyTorch. You can convert it into ONIX that Microsoft provides you with open source framework. And then this model can run on any hardware accelerated and you or the cloud provider need not to do any specific thing. So once you start making these kind of contributions, you can actually, nobody will like stop you. Either you're going to become a PM or you're going to become a GM through engineering ladder because people want people who are taking broader impact and broader challenges than what is given to them.

**Mahesh Yadav** (00:46:03)

Small prompt, long response.

**Aakash Gupta** (00:46:05)

And then after that, you worked at so many of the other FAANG responses, FAANG places, Meta, Amazon, Google. How are you cracking all of these FAANG interviews in

**Mahesh Yadav** (00:46:16)

piano? I think once it was very hard, to be honest, right? I was born in Microsoft. I was supposed to die in Microsoft. Microsoft is such a family, right? Because it's especially on this side of the Lake Washington. It's on this side, Seattle on the other side in Seattle. So in Redmond, if you live, you live in Microsoft bubble. which is you go to restaurants where all Microsoft people, you go to the gym with Microsoft people, all your friends and all your kids' friends are Microsoft. And it's just hard to leave that place. So first time when Facebook reached out for me, I thought at that time I was working on inference, which is like, how can you run these models? But I wanted to go into training and they had an awesome opportunity for me. So that time it took a lot of time. But after that, I think, to be honest, AI has done a great deal for me.

**Mahesh Yadav** (00:47:16)

I had this, except a different skill set, which was in demand across these like four or five years where I've done these transitions. So I would say that played one role. Second role is that I was able to just articulate well my stories, show scale, show how I handle ambiguity and third this never giving up attitude which I think these companies are hungry for. Because once you enter these companies, the people there are just too hard to work with and things don't move fast. And if you can say that I'm going to come and make things go fast, these PM managers are hungry for you, especially in AI because everybody had that FOMO pressure. And this guy knows what we can build. And he has done an iteration outside. And... He's hungry. He is impatient. These three, I think, just made it so easy for me.

**Aakash Gupta** (00:48:16)

Okay. And how did you get so good at the PM interview though? Like the PM interview, case interviews, what was your approach to that?

**Aakash Gupta** (00:48:22)

I think I watched all your series, all your, read all your blogs.

**Aakash Gupta** (00:48:28)

Awesome. That's amazing. Yeah, I think

**Mahesh Yadav** (00:48:31)

I think just I know I truly I followed you and others and I was able to like at least keep like what's out there. There is a lot of good content or summary, but I did. I generally I don't stop in LinkedIn. I take what you guys post and then I look at the links and I read them. Like I was reading, there's another guy named Lenny, I think. And he posted this AI jobs and that I was trying to figure out, okay, what's the trends look like? Is this going to be the right thing for us, for the economy? And then I read more like five reports. So I think staying on top of this, that's one thing I would suggest. And don't do your own research. Let people like Akash, Lenny work for you so that you can get from an abstract form and then scale it to your own world.

**Mahesh Yadav** (00:49:20)

So that's one thing I would suggest. Second, I think... Just having stories where you show these three things, which is scale, ambiguity, and what is your impact on business. And show it, say it succinctly, and let the interviewer run your interview, but land these ideas. And third is just having an opinionated view on things, I think was helpful for me. like don't be a pushover if they push you just say I mean I'm very respectful and I'm very like I listen to them but I try to say why I thought and you can go with me like three levels down and I will be able to tell you that my fundamentals my model of the world is not very bad and then you can say okay maybe in this case he might be right

**Aakash Gupta** (00:50:15)

And going back to your very first, at the very beginning of the conversation, you've developed, I can build AI, I can build it at scale. And so that's, those foundational experiences allow you when they're pushing you in the interviews to just go three levels deep where other people might not be able to. So you worked at all these companies. How would you compare them? How would you compare Microsoft, Amazon, Meta, and Google? Which one is best for which people?

**Mahesh Yadav** (00:50:40)

I think that's a great question. It's hard, but let me give it a shot. So what happens is, I will tell you what I loved about each company. So let's start with Microsoft. So Microsoft is a dreamland for people who want to go build without caring how it will make business. I don't know. It's just ingrained in Microsoft to just innovate without figuring out how will we make money. The opposite of that is Amazon. If you are working in AWS specifically, you have to be very clear how you're going to make money because if you want to be a PM, if you want to build a lot and try taking a lot of shots, then go to Microsoft. If you want to be a PM who owns profit and loss statements, who actually cares a lot about business and ready to die for that $1 thing and execute at speed of light, go to Amazon or AWS specifically.

**Mahesh Yadav** (00:51:42)

Specifically, AWS AI teams. So much fun there for that one aspect. But they won't let you innovate a lot. That's the downside. That brings you to meta. Menda is a company where you will go if you want to innovate a lot with the right amount of people. Here, one thing that I still remember is that PLs there are world class. And they will come to you and say, tell me what you want me to build. And you say, dude, I'm not sure. I have these like three ideas and all are like 20%. I'm sure that they are successful. They will be successful based on interactions I had. He said, can you give me one? And I will build it. And then you can launch it. And then if it doesn't succeed, I won't even tell my manager. And they will take on these experiments. They will build it over the weekend.

**Mahesh Yadav** (00:52:35)

I will be able to launch it on some sample set. And if it works, all they want from you is create a post and publish it. And then they will keep coming to you. But if you can't give them good ideas, if you feel three times back to back, they're going to the other PM and they never come back to you. And that's your death in AI world if you're working for Meta. So Meta is a place where you want to have good iterations and working with great people to do the next level thing. And also never worry about money inside Meta. They have a lot of like, I felt at least I was there before like this whole, you know, squeeze and everything. So it's a very rich company. And it's an awesome company inside, outside people think badly about, you know, whatever they do.

**Mahesh Yadav** (00:53:21)

But inside, it's a very homely and awesome company. And you go there to build latest technology, whatever it could be. If metaverse, if tomorrow quantum becomes a thing, they will be able to catch up. So if you want to stay on the edge of things, go to meta. And last one, I will give you Google. Google is an awesome company for user experience. They just are obsessed on user experience. If you want to learn how you serve anything on user experience, there's so many experts there, like what a copy should look like, where a button should go, what happens from this screen to this screen, and how can we create magic between this experience, even if there is a five second delay. They are obsessed on that. And second is, they give you a lot of time. So it's like Microsoft, but they care about money and user experience.

**Mahesh Yadav** (00:54:14)

So if you add a little bit of money, less money, not like crazy like Amazon.

**Mahesh Yadav** (00:54:20)

So a

**Mahesh Yadav** (00:54:20)

little bit of money, but a lot about user experience. So I think you want to go work for Google.

**Aakash Gupta** (00:54:28)

Okay. I

**Mahesh Yadav** (00:54:28)

hope that helps.

**Aakash Gupta** (00:54:29)

So we have been talking so much about how to break into these thing companies. And we started with these agent PM jobs. How many AI agent PM jobs are there really out there?

**Mahesh Yadav** (00:54:41)

That's a great question. Let me just show you. I got this data from this site called Trueop. They did this analysis and they show you all the data that, hey, how these jobs are. By the way, they were also cool to show you who's getting paid the most. So I felt a little bit FOMO that why I'm not there yet. But let me quickly show you what this data looks like. So this is the data on jobs in agentic AI or AI specifically. So these are all the jobs postings that are open and don't look at the numbers because you know all these people who scrape these jobs have some problems but look at the trend right you're looking at a lot of jobs in pm then dropped and these are all the pm jobs if you go to the next slides you are looking at all the ai jobs And now you see like where the growth is going or coming from.

**Mahesh Yadav** (00:55:36)

So this is Trueop and you're looking at 25k AI jobs. And then this is the last one where Lenny did this analysis, working with again Trueop. And here it shows that if there are new jobs, The likelihood of that job in AI is double than the likelihood of that job in PM space. So this

**Aakash Gupta** (00:55:58)

is

**Mahesh Yadav** (00:55:58)

like all PM is down here. And I'm just looking at delta because these numbers are not like proportional. But if you look at this, that just the comparison on that scale, this is growing two to three X more than what your traditional PM jobs are growing.

**Aakash Gupta** (00:56:15)

What is the salary and compensation for these AI agent PM roles?

**Mahesh Yadav** (00:56:21)

That's a really good question. I think easily like you're looking at level six or level seven roles at man companies, you can expect anything from 750 and above. I think that's a normal pace these days. And if you are looking for level eight and above, you're looking at 1.2 to 1.5 million. That could be easy. And I'm saying total comp. Like your joining bonus plus your stock. And even if the stock remains same, that's the comp these days across these companies. And most of the startups are trying to give even better. So if you're going to open AI, you can just at level six, level seven, you can even expect 900K. Netflix recently posted a job. I think they posted some 790 or 950. across these jobs and that's normal for top 10 ai companies and i think that's why people are excited about or people spend so much time and years preparing for that so i think that's a good number

**Aakash Gupta** (00:57:21)

insane numbers okay and can anyone become an aipm

**Mahesh Yadav** (00:57:26)

I think so. I think don't expect to become an AI PM if you have never worked in AI before in six months or six weeks, to be honest. It might take you an year to get to this level where you can start interviewing at like top companies and get to 700 plus salary. But if you want to get to like 300 plus, I think you can crack something in six months. And I think 18 months is a really good time to get mang if you're starting from zero. And I think it's a great time to do that because there is a level playing field. There's a lot of AIPMs needed and whether you were at Google before or not doesn't matter or whether you were at Meta before or not doesn't matter because we need that talent. And if you are outside and have been iterating, solving ambiguous problems and building product with iterations and not by research, then I think this talent the world is looking for and if it's not happening just hold on to it by the way it took me like AWS told me no like when Meta took me Google also said no so just a secret for you that it doesn't always work and then you just get double salaries and all it takes time but if you're working on something that you're passionate about and you believe in the tech stack and you are working as fast as anything you can afford to 18 months is a really good time for anybody to just get in and get to the top 1% of HNTK IPMs.

**Mahesh Yadav** (00:59:01)

And you can just join our community, listen to me every Friday. And if you're building what I'm telling you or using our learnings, I promise you 18 months, I've seen nobody fail so far.

**Aakash Gupta** (00:59:14)

What is that 18-month roadmap to becoming a PM IT thing?

**Mahesh Yadav** (00:59:20)

So let's divide it into your six milestones. Your first milestone is understanding and building your first good prototype. So what does that involve? That involves, do you understand what goes behind the model, this intelligence piece in this diagram? So this intelligence piece is your LLNs. You can call this GPT-5 or this. How this piece is built, Then how you connect it with your own knowledge of the company, your own databases. So this is the thing that we all have intelligence and this is coming in machines these days. This is how the world works. Knowledge that is not in the model, which is, hey, what's the vocations in your company? What you like, where you have visited in last one year if you're building a travel agent. Then your memory or signals. Then your tools, which can change the state of the world. So this is how the world works.

**Mahesh Yadav** (01:00:18)

Current state of the world. And then your tools, which is how can you change the state of the world. And then guardrails, which is what you should do and what you can't do. Or putting all the checks and laws. Or even checking by feedback, did we achieve the goal or not. And then bringing this all together to build a real working agent That should be your goal in first three months. That you understand these concepts in and out. And you have built your first agent with all of these ingredients in it. That should be your goal for first three months. After that, what you're looking for is either starting your own thing on side, which is a real good problem you have, which can be any problem under the sun. I don't care. Do you have PhD level expertise in that thing? Does it have unstructured data and complex decision making?

**Mahesh Yadav** (01:01:15)

And if it has all these three, just start solving that problem. That's your next three months. And you should have at least 10 to 20 free users on that. That will teach you how to evaluate these things. So next what we are learning is first three months you learn concepts, then you go and say build and evaluate. Once you reach that, that's your six months. That's your first iteration. And after that, next six months, I really want you to get it into production. Whether you are hiring your own team of five engineers, maybe somewhere in India, or somewhere it doesn't cost that much. And you are actually making it production and going from 10 customers to 100 customers. Another idea there is work for a startup for free. People will love to take that. And everybody wants people who have this much done and help them give them free hands so that's your next six months build and give people the right thing this will teach you how actually this build and evaluate iterations will work and bring the ambiguity and scale factor on your world once you have that you have hit an ear then you start actually doing a lot of After this, you're trying to decouple any companies that you want to target their products and seeing what feature you will build.

**Mahesh Yadav** (01:02:47)

And you start working in their open communities. You run evaluations for them free. By this time, you should have your evaluation frameworks. And you're running evaluations and telling them what are their gaps. And you're doing it for top 10 companies that you want to work for, for their top 10 products, which everybody cares about. Whether it is OpenAI, Anthropic, Meta, Lama, start doing that. I've done that and it does wonders. And then you create a small community around it and you are building them and you're saying, hey, You know what? I got these three engineers. I came up with this feature list and I have checked it into your code voice. Like at that point, like, okay, Meta won't hire you, but Google will hire you, right? Nobody can stop you. Next iteration, you are even doing better than their PMs. And the beautiful part is all these companies have open source their model or some version of their model.

**Mahesh Yadav** (01:03:39)

Even GPT has an open source model now. And you can take that and show them how GPT-5 is so bad at instruction following and take the open model and fix it and do a side-by-side eval and publish it as a paper. And you can do that once you reach this one year time frame. After that, Our students, like people who have done, have been in our community, have done the courses, have been done all the paths. They get jobs before this step. But if they don't get it, I know a guy who just hacked the whole website and showed them their prompt and said, hey, maybe you want to do these checks in. Otherwise, people will see your prompts. And he got his first gig like that. And then he worked in, now he works for Carfax, building their AI stack. So it's not like people are desperate for you, but you need to be desperate for learning.

**Mahesh Yadav** (01:04:37)

And that's your 18 months, month on month. And every three months, you should be hacking after this. And I don't, if you reach that stage, just ping me.

**Aakash Gupta** (01:04:49)

This was the clearest, most actionable roadmap I have gotten yet. And I've asked quite a few people this question. So make sure you guys were taking notes on that. I want to talk about this final angle of AI agents, which is if you're just a regular PM, not an AI PM, what AI agents should you be building to improve your efficiency on the job?

**Mahesh Yadav** (01:05:10)

It's a really good question. I think one AI agent which all of us need is the guy who looks at our customer interactions. So we live in a multifacet or multimodal world and we go to a lot of calls where our sales or our friends or things talk about this. So always have a single agent which goes through every channel, every interaction where you can get feedback on your product, processes it and does something. I think that's a missing agent. I have not seen any tool. I've seen some tools here and there. I think you should build it and iterate on it. So that's my number one suggestion. My number two suggestion is build something that you can run A-B tests at scale, which is this idea that Before what you want to run, there's never enough people to run A-B test. And to be honest, when we ran them, it was such an insignificant sample to make any judgment calls.

**Mahesh Yadav** (01:06:05)

But we live in AI now and you can create thousands of different personas with small, small variations, put them into groups and show them your product and maybe run a quick simulations of A-B testing or just simulation of who is going to use their product most or love the product most. So one is, this simulation should teach you how your product fails and for what customers so that's one thing you should get out of that agent and second thing the output of that agent is that it tells you which personas will love your product which which by the way will be the people who have finished the flow faster have stopped at the key points and click the feedback So these two, and I think all of us should build a reviewer. I think people lose a lot, especially people who are new in AI, lose a lot of their brand in the beginning.

**Mahesh Yadav** (01:07:06)

because they have these documents which are immature, they had used terms loosely and not to their fault, they are just new. So I will build a reviewer. I think people who are building like PRD tools or create PRD tools, I think they're really foolish. They don't understand how much is about credibility of the person. And their intuition goes in that PRD. And if AI generates it and you think that can solve or that's how the organization will make decisions, I think we're not there yet. So I don't need that. What I need is I will write the PRD and I will check it with AI. But I want to have a reviewer who has looked at my manager, 20 reviews, how he commented and can automatically comment on my PRD. In his style, what he cares about, what he doesn't care about. And if I build that reviewer, Everybody should be able to use it.

**Mahesh Yadav** (01:08:06)

Just upload whoever you are reviewing with, take their previous 10 reviews, upload them, upload your document, click a button, you got the first review. You address things and then you show up. I think that people will use and will be a great thing. So A-B tool for testing or a scale to run simulations of your customers and get insights. which is based on this thing, which actually watches different channels and give you insights. And third is a reviewer tool. I think these are the dream tools, which I want to build or use, or I think everybody should build and use. And we are working on a couple of them. If you want to help, happy to take that help too.

**Aakash Gupta** (01:08:47)

Love it. So we talked about how well these roles are paying, yet you've chosen not to continue on the path of these roles. I have to ask, this is the hot question now, you're on the hot seat. How big is the business of Mahesh?

**Mahesh Yadav** (01:09:04)

I think that's a good question. So I think I'm very comfortable with the community and things that build. I won't give you my exact numbers, but you can look at how much our course sells for. We have grown 40% cohort by cohort. We started with 40 people and we have grown 40% each cohort. We are on our eighth cohort and we just served, we are serving 180 or so people. And we have divided it into two because I never wanted to have more than 70-80 students in one group. Because I really wanted to have personal interactions and know them by name. So I run two classes now. So that's how we are making money. But I'm also working on building my own thing. And the money that we make here goes into that.

**Aakash Gupta** (01:09:49)

So

**Mahesh Yadav** (01:09:50)

not like business of Mahesh is a lot of transactions. I'm a medium these days. So it comes from here, goes here. And the goal is to bring the best AI capabilities in the hands of people which are least likely to use them without help. And with that goal here, we are trying to bring a lot of people who can't get to AI faster. And then on the other side, we are building tools for people who can bring AI to a lot of other fields, not just tech, so that more people can come in. And if I can be a catalyst in that reaction, that's business of Mahesh. And now you

**Aakash Gupta** (01:10:28)

did some

**Mahesh Yadav** (01:10:29)

math maybe already.

**Aakash Gupta** (01:10:31)

I'm doing the math in my head. I'm trying. Okay. This was amazing, Mahesh. This was a masterclass in AI agents for PMs. Thank you so, so much.

**Mahesh Yadav** (01:10:41)

Thank you for the chance. I always wanted to be here. I always looked up to you from the beginning, even when AI was not cool. I think growth was the thing. Growth was, I think, it was an eye-opener first time for me. It means nobody talked like that. about growth it was more about building especially in the companies i worked for but you brought and i think couple of people at that time brought this idea to life which is it's an essential skill of a pm to grow the business and i think nobody else has contributed more than you on that channel and with ai you are pivoting and you are iterating so fast that i can't catch up so thank you for having me it's just i'm so humbled for giving me this experience thanks akash

**Aakash Gupta** (01:11:25)

I'm the humbled one. Thank you so much. Everyone, check out his course on Maven. Support his startup when that comes out. And we'll see you in the next episode. So if you want to learn more about how to shift to this way of working, check out our full conversation on Apple or Spotify podcasts. And if you want the actual documents that we showed, the tools and frameworks and public links, be sure to check out my newsletter post with all of the details. Finally, thank you so much for watching. It would really mean a lot if you could make sure you are subscribed on YouTube, following on Apple or Spotify podcasts, and leave us a review on those platforms that really helps grow the podcast and support our work so that we can do bigger and better productions. I'll see you in the next

**Mahesh Yadav** (01:12:13)

one.
