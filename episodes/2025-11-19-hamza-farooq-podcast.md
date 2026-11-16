---
title: "How to Land an AI PM Job: Complete Roadmap from Hamza Farooq"
subtitle: "The exact roadmap and the technical skills you actually need."
date: "2025-11-19"
host: "Aakash Gupta"
guests: ["Hamza Farooq"]
speaker_names: "substack"
substack_url: "https://www.news.aakashg.com/p/hamza-farooq-podcast"
youtube_url: "https://www.youtube.com/watch?v=Pg9M-2bpOXA"
duration: "00:28:43"
word_count: 5234
source: "Substack episode transcript (aired audio)"
---

# How to Land an AI PM Job: Complete Roadmap from Hamza Farooq

*The exact roadmap and the technical skills you actually need.*

**Aakash Gupta** (00:00:00)

There's a lot of hype on AI, but it's actually the opposite when it comes to AI PM roles. Look at the median total comp that is available for them. The median salary for AI PM is skyrocketing. Hamza Farooq,

**Hamza Farooq** (00:00:11)

an expert who has worked with companies like Home Depot, TripAdvisor, and Jack in the Box on their AI and is going to give you all of the sauce for free.

**Aakash Gupta** (00:00:19)

You have to be a jack of all trades. You need to know exactly what AI can do. You don't need to know what drive is. You don't need to know what fine-tuning is. You don't need to know how context engineering works.

**Hamza Farooq** (00:00:30)

If they want to go from here, what else is there in the six-month roadmap to go from no experience to PM at OpenAI or Anthropics?

**Aakash Gupta** (00:00:37)

And within 30 minutes, we were able to build Lovable, connect it to NITN, and have RAG working right in front of us. In today's episode, we're going to teach you everything from prototyping, RAGs, and agents all how to become an AIPM. They don't even know the problem they are solving for.

**Hamza Farooq** (00:00:53)

Can somebody without experience become an AIPM? Really quickly, I think a crazy stat is that more than 50% of you listening are not subscribed. If you can subscribe on YouTube, follow on Apple or Spotify podcasts, my commitment to you is that we'll continue to make this content better and better. And now on to today's episode. Hamza, welcome to the podcast.

**Aakash Gupta** (00:01:20)

It's a pleasure to be here, Akash. Thank you for having me.

**Hamza Farooq** (00:01:22)

So the topic today is AI product management. And where I want to start is AI product management all hype. A lot of people have been telling me this role doesn't even exist. A lot of product managers have been saying people are talking too much about AI PM. Is it real?

**Aakash Gupta** (00:01:34)

Well, I'll tell you one thing. There's a lot of hype on AI, but it's actually the opposite when it comes to AI PM roles. Because who's going to make them into real products, into real systems so that users can associate with that? And I just want to show you one screen, just one detail to show you the growth that we have seen for the requirement of AIPMs across the board. And it's just because these things are a need for today. You need to learn all these things so that you can build products so users can go beyond using ChatGPT. And if there is one more, you know, sort of marker for it, look at the median total comp that is available for them. You know, look at the 25th prompt. I mean, I really hope that people land at the 90th percentile, but just the median salary for AIPM is skyrocketing.

**Aakash Gupta** (00:02:22)

This is only second to software engineers or even exactly where the software engineers are right now in the Bay Area. Why do you think the AIPMs are paid so well? Well, it's basically not just a PM role anymore. That's the reason behind it. You have to be a jack of all trades. You need to know exactly what AI can do. Previously, you didn't need to know the technical details. You don't need to know what drag is. You don't need to know what fine tuning is. You don't need to know, hey, this is how context engineering works. Here, what we're seeing is that the AI PM is needed to understand, to build the next generation of tools that did not even exist a year ago. For example, Lovable. Lovable is a product that we didn't even imagine about. like a year ago or maybe a little more than a year ago, who would have thought that you could just build websites just like that?

**Aakash Gupta** (00:03:12)

Your AI PM role is paramount to make this available for the next billion users.

**Hamza Farooq** (00:03:18)

It's really thinking ahead about what are going to be the next generation of products. These are going to be AI enabled products. Therefore, we need PMs who deeply understand AI to build them.

**Aakash Gupta** (00:03:27)

Exactly. Because If you don't know what AI can do for you, you are stuck in going all about what GPT is doing, what OpenAI is coming up with. You have to think about, I'm an e-commerce company. How can I use AI to get what's best for my customers? That's what you need to know what AI can do for you.

**Hamza Farooq** (00:03:45)

This is some fascinating data. OpenAI and Google obviously playing at those 90th percentile that we saw, Oracle paying at that 10th percentile. Overall, AIPM, highly lucrative field.

**Aakash Gupta** (00:03:55)

Absolutely. Absolutely. Like this is the best time I think ever it has been to become an AI PM and actually lead from the front so that you can build products for your users.

**Hamza Farooq** (00:04:05)

Does any of the content around AI PM really matter if you don't have AI experience? Can somebody without experience become an AI PM?

**Aakash Gupta** (00:04:13)

Well, that's what people have done in the past couple of years. Like, let's say if you want to become a doctor, you have to go through school, you have to have learning, you have training. Well, you know, to be honest, OpenAI just dropped GPT to us, you know, in 2023. And we had to all, we all had to scramble and learn. And that's the biggest thing that, you know, that we tell people is don't live in FOMO. There is a roadmap, there is stuff, there is training that you can achieve, assimilate and actually become an AI PM in like six months or

**Hamza Farooq** (00:04:42)

less. Amazing. So what are the key skills? What's the six month roadmap to become an AI PM?

**Aakash Gupta** (00:04:48)

Well, I think the most important thing is to first identify the tools that you sort of need to learn to get started. And, you know, if you look at the slides, this slide seems a little daunting. Like, oh my God, I have to learn so many things. But honestly, it's how you use them and you don't have to use every single one of them. For example, and I'm going to start using the whiteboard. So the first thing you need to know is what kind of tools do you need and how do you want to use them? And I'm going to draw a very basic architecture design for you. The most simplest, you know, that I have. that should get you started. You need to know how to use an LLM as an API endpoint. So you have a GPT available to you, you have the chat GPT available to you as an application.

**Aakash Gupta** (00:05:36)

They all have API endpoint. So you need to have an API connection or be able to understand how to use an API, which is almost literally getting a key and you're ready to go. From that, you need a back end ecosystem, for example, NITM. N at N is this magical ecosystem, which is completely no code. You don't need to write a single line of code. And this amazing tool gets you up and running with the backend of what the engine that becomes your AI backend. and then like any other tool you need to build you need to have a front end or the main landing screen where your users will sort of uh communicate with you so if you go here you basically what you want is a front end and we use something like a lovable to build a front end right and again this is a no code tool.

**Hamza Farooq** (00:06:27)

LLM back end, front end, pretty simple architecture.

**Aakash Gupta** (00:06:30)

So I want to take you through an example, you know, this, I've written three, three, three different architecture components. Now, let me show you a simple example. So Akash, I want to ask you, do you use Airbnb? Of course. Right. I am the biggest fan of Airbnb, but like I'm their you know platinum level if they had a tier i'm the platinum tier now the one thing that i hate about airbnb is actually i cannot search anything up beyond the dates and a city i literally cannot do anything beyond that so i built this unofficial version of airbnb and you know i really want to show you guys an example of this so for instance i want to stay in a modern apartment in tokyo near the train station and Looking into today's let's just say that I want to go from 25th of November to 2020 let's just say 29th of November and That's all.

**Aakash Gupta** (00:07:28)

All I need to do is just enter my name and my email. And what this tool will do now is it will connect. So this is the front end, which is built on Lovable. This is the backend. This is the backend, which has been built on N8N. It will receive the request from the user and using the request from the user, it will call something which is called MCP. And before you worry about what is MCP and what are these things, all I want you to worry about is Everything over here is built with a no code. Like all you need to do is build things in the simplest form. And once you have this thing ready, this workflow gets activated. And once this workflow is activated for you, it will generate a response. It will run behind the scenes and then it will generate the listings for you that you can find in Tokyo.

**Aakash Gupta** (00:08:17)

once it has discovered all of them, it will send you an email saying, hey, I have found the, you know, the Airbnbs that are most relevant to what you are looking for, right? So imagine we identify a customer need. We said this customer, we as customers would like better search capability and we are able to get that search available to us. And, you know, as part of a magician, the last thing is to show the result so when i open my email over here i have the day it picked up the dates it picked up locations it tells you why it's a good location for you

**Hamza Farooq** (00:08:56)

and just it's like that it's like chad gpt natural language concierge for airbnb right

**Aakash Gupta** (00:09:03)

and then if you click on a link it's actually the like it's not hallucinated for you it's actually the right it's a live link yeah it's a live link right so

**Hamza Farooq** (00:09:12)

Okay, so we've seen the end product. Can you walk us step-by-step how we would build this ourselves?

**Aakash Gupta** (00:09:17)

Absolutely. So there are, as I said, the three major component with this LLM API, there's a backend where you build end at end, and there is a lovable front end, which you have to work on, right? So in order to get started, let's just say we want to start with building the backend API. So, you know, the best thing over here is that I have, you know, finally got into writing comments and everything is available for you. So this is what NNN looks like over here. You have NNN set up. You're like... how do I know I need all these components? Well, it's actually pretty easy. Once you start designing the ecosystem, you're like, okay, there's an Airbnb, I need to build an MCP connector. The job of the MCP connector over here is to take your request and be able to connect to Airbnb app and pull information from there.

**Hamza Farooq** (00:10:05)

Awesome. Today's episode is brought to you by Amplitude. Replays of mobile user engagement are critical to building better products and experiences. But many session replay tools don't capture the full picture. Some tools take screenshots every second, leading to choppy replays and high storage costs from enormous capture sizes. Others use wireframes, but key moments go missing, creating gaps in your understanding. Neither approach gives you a truly mobile experience. Amplitude does things differently. Their mobile replays capture the full experience. Every tap, every scroll, and every gesture with no lag and no performance hit. It's the most accurate way to understand mobile behavior. See the full story with Amplitude. Really quickly, if you've been enjoying this episode so far, Humza teaches two Maven courses that I highly recommend. The first is the Agent Engineering Bootcamp. This has 4.8 stars with over 78 reviews. It's a seven-week live cohort-based course.

**Hamza Farooq** (00:11:02)

People at Google, Walmart, and other places are taking this course and learning a lot. The second course he does is agentic AI system design for PMs. If you wanna go to that next layer technically on agents, even further than what we're doing in this episode, you should check out that course. Use code AKASHXMAVEN for a discount and use my URL in the description to get that discount automatically applied. Now back to today's episode. Can we build this from scratch?

**Aakash Gupta** (00:11:26)

Well, yes you can, but in order for you to make a lasagna, you should know how to bake something simple. And in order to get us started and not get overwhelmed, let's start with the most basic building steps of anything. All right. The first basic step of using lovable and anything together is a webhook. Webhook is this magical thing that allows you to communicate across different tools. And that's what we're going to do right now. So for instance, The first thing you want to do is if you go to our GitHub, I've created a roadmap on how to get started with NITN. You can start, the most basic one is start here, which is literally just a couple of nodes. But here, what I want to do is I'm going to build something a little smarter for us, which is able to connect to Lovable and it's able to run on NITN at the same time.

**Aakash Gupta** (00:12:17)

And the basic version of this is that there is a webhook, which is your front end. You have an AI, a webhook, which communicates with end at end and is able to respond back and forth in real time for you. So the first thing we'll do is what you want to do is if you click on the web hook over here, and this is the best thing. There's so many examples that are already created that we don't have to worry about. Hey, how do I do everything from scratch? This is the most basic way to get started. There's a JSON file. You copy the JSON file and you come to edit and you can paste the whole thing and it's ready to go.

**Hamza Farooq** (00:12:52)

Trust isn't just earned, it's demanded. Whether you're a startup founder navigating your first audit, or a seasoned professional scaling your GRC program, proving your commitment to security has never been more critical or more complex. That's where Vanta comes in. Businesses use Vanta to establish trust by automating compliance needs across over 35 frameworks like SOC 2 and ISO 27001. centralized security workflows, complete questionnaires up to five times faster, and proactively manage vendor risk. Vanta can help you start or scale your security program by connecting you with auditors and experts to conduct your audit and set up your security program quickly. Plus, with automation and AI throughout the platform, Vanta gives you time back so you can focus on building your company. Join over 9,000 global companies like Atlassian, Quora, and Factory who use Vanta to manage risk and prove security in real time. For a limited time, my listeners get $1,000 off Vanta at Vanta.com slash Akash.

**Hamza Farooq** (00:13:50)

That's V-A-N-T-A dot com slash A-A-K-A-S-H for $1,000 off. Today's episode is brought to you by Naya One. In tech buying, speed is survival. How fast you can get a product in front of customers decides if you will win. If it takes you nine months to buy one piece of tech, you're dead in the water. Right now, financial services are under pressure to get AI live. But in a regulated industry, the roadblocks are real. Naya One changes that. Their air-gapped, cloud-agnostic sandbox lets you find, test, and validate new AI tools much faster. From months to weeks. From stuck to shipped. If you're ready to accelerate AI adoption, check out Naya One at nayaone.com slash akash. That's N-A-Y-A-O-N-E dot com slash A-A-K-A-S-H. Today's episode is brought to you by the experimentation platform Chameleon. Nine out of 10 companies that see themselves as industry leaders and expect to grow this year say experimentation is critical to their business.

**Hamza Farooq** (00:14:49)

But most companies still fail at it. Why? Because most experiments require too much developer involvement. Chameleon handles experimentation differently. It enables product and growth teams to create and test prototypes in minutes with prompt based experimentation. You describe what you want, Chameleon builds a variation of your webpage, lets you target a cohort of users, choose KPIs, and runs the experiment for you. Prompt-based experimentation makes what used to take days of developer time turn into minutes. Try prompt-based experimentation on your own web apps. Visit chameleon.com slash prompt to join the waitlist. That's K-A-M-E-L-E-O-O-N dot com slash prompt. So RAG is a many tens of billions of dollar industry. People are also talking a lot about fine tuning and context engineering. What do AI PMs need to know about those?

**Aakash Gupta** (00:15:39)

Awesome. Well, I'm going to talk about context engineering. All right. And context engineering for me is the most important thing that an AI PM should know. Usually what we do is that, you know, when you're trying to talk to an LLM, we have a system prompt and we have a user prompt. Correct? These are the two things that we have available to us or we basically use them for our LLM to respond to us in the way we would like it to, you know, sort of respond. However, let's just say Akash, I want to make it personalized to you and personalized to me. So let's say we have a finance agent which is listening to your conversation And you're like, you know what? I only want to invest in S&P 500. I want to do safe trading. I want to do things, you know, which have historically, you know, they have gone up and they are safe bets.

**Aakash Gupta** (00:16:37)

So we want to say Akash wants to go after S&P 500. Right. And now let's just say I'm another person. I'm like, I'm very frivolous. And I'm like, I'm going to go into crypto. Right. I'm like, you know what? I don't make any money. You know, ever since I quit Google, you realize how less money you make. Right. So I'm going to, you know, do or die or like all in. So how do we make sure that you are getting the right information? Like you are getting the right information and I'm getting the right information that is relevant to me. And that's where context engineering plays a role. So here, what we do is that we do, we have a system use prompt and a user prompt. Then what we can do is we add memory, which are your past interactions and things that the LLM has learned about you and stored.

**Aakash Gupta** (00:17:36)

So we call this the long-term memory. This is also a prompt. And then we get information, relevant information from the rag. So you just saw the rag, right? You just saw that the rag was able to pull context and you were able to get an answer. That's your rag connector right there. So when you combine all these things, That's your context engineering. So prompt engineering is what you tell an LLM. Context engineering is how you design the instructions for your LLM. And that's the beauty of having the knowledge of context engineering because it then makes your entire ecosystem dance. You can get personalization, you can get, uh specific answers to what you are you're looking for and it understands each users based on on that information right so context engineering is extremely important more important than prompt engineering now because you have to combine multiple levels of things at the same time get to to that answer in today's world right so that's what we have context engineering for the second thing that you have mentioned is fine tuning yep So you see fine tuning is all about task adaptation.

**Aakash Gupta** (00:18:45)

So usually when you have a LLM, the LLM can produce, you know, you give it a prompt and for every prompt, there's a response. However, you want to say, hey, you know what? I just, I don't want this prompt or this LLM to produce general responses. I want the LLM to only produce Python code and the best practice Python code. So that's when you fine tune an LLM. on best practices of coding. So it becomes a coding agent or a coding LLM, right? So fine tuning, again, I want to say is task adaptation in which you are basically telling the LLM, this is how I want you to respond. And this is the context behind it. These are 10,000 examples or 100,000 examples of what greatness looks like over there.

**Hamza Farooq** (00:19:31)

And once you give it all those examples, it can really customize to that specific use case and become that specified LLM.

**Aakash Gupta** (00:19:38)

Yeah. Another example is that you work, let's say you work for a pharma company and you want the LLM to remember the vocabulary about your things, about the different acronyms you have and different products that you have built. That's where you fine tune for understand, for vocabulary. I want to say vocabulary and not knowledge. Vocabulary refers to adding new words to the LLM. For knowledge, what you want to do is you want to connect to a rack. Amazing.

**Hamza Farooq** (00:20:08)

So we've given people a preview of the knowledge. We've given them the demo. If they want to go from here, what else is there in the six month roadmap to go from no experience to PM at OpenAI or Anthropic?

**Aakash Gupta** (00:20:19)

So I'm going to share sort of like a very basic architecture that, you know, I tell people, you have to learn by doing things. The best way is to keep building things. This is a sort of a basic roadmap. You need to know what LLMs are. You know, in this conversation, we looked into how we can build applications. We discussed prompt engineering. Then we looked into, you know, some kind of rags. Now, you just have to follow this roadmap in order to build better products. And you have to do it or, you know, you have to follow this theme over and over again till you get to a point where you have identified this is the roadmap or you've started to feel that I am making sense. And this is... how you do it you know one of the most important questions I get from people is what should I build why do I need to what how do I go and I tell them think of three wave approach the first wave is you want to build something that saves you time efficiency gain productivity gains I'm not doing anything else I'm just saving time to do something exact same thing the second wave is you want to build better quality better output And the third is that you are building something which is completely new.

**Aakash Gupta** (00:21:29)

So for instance, you have, let's say Akash, you meet a lot of people, you need maybe a summarizer which says, this is the conversation you had with all the people today. And these are the action steps that you need to do. That's your time, cost and efficiency. The second part is quality, better output. Hey, AI agent, can you take my video, slice and dice into different parts and make a trailer out of it? The third part is, Hey, AI, can you actually build an AI recording of as if this is the prototype of the script? I want you to build a script. I want you to have, you know, AI agents which act like human and do the recording for me and then publish it on my YouTube channel.

**Hamza Farooq** (00:22:11)

Very cool. Yes. I should build that.

**Aakash Gupta** (00:22:15)

Right. So, and we, now it just makes sense. So instead of just following the roadmap or I need to learn tools, you saw in within 30 minutes, we were able to build lovable connected to anything and have rag working right in front of us.

**Hamza Farooq** (00:22:28)

Yep.

**Aakash Gupta** (00:22:29)

Right? That's what you need to do. You need to keep building things and see where your products fit in the business problem that you're trying to solve for your customers. That, does it solve a user problem? Does it solve an organization problem? Does it align with your business model?

**Hamza Farooq** (00:22:45)

Three awesome questions to ask yourself as you guys go on this AIPM learning journey. So I want to talk to you a little bit here at the end of the episode about you. What is the business of Hamza? How big is the business of Hamza? You were formerly Google. We talked about poking fun about those are some serious golden handcuffs. What does the pie chart of your revenue look like today?

**Aakash Gupta** (00:23:06)

So there are essentially two different things which I'm doing right now. I run a startup with the name of traversal.ai. We experimented with a lot of different tools. We had initial traction on them also, and we kept building. But where we have sort of found a PMF, is we have become this company that you can connect that we sort of our tagline is intelligence that runs your data. So imagine manufacturers across US, you have, for instance, you have PNGs of the world, you have the Unilever, but then they are small and medium businesses also. We worked with, so imagine we work with a manufacturer who builds all the boxes for Amazon. They're no way small and medium, but they're just like a mom and pop manufacturing that basically is producing cardboard boxes for Amazon. They had zero data scientists. They had zero insights on what and how much should they produce.

**Aakash Gupta** (00:24:05)

They were reactive. which meant that, hey, we're gonna get a response from, a request from a customer, we're gonna scramble and we're gonna, so they were always like just in time building. What we did is that we built an army of agents for them that can process that information and give 20,000 SKU at a daily level that this is the demand, expected demand for them for the next one week, for the next 14 days, for the next three weeks, right? And it saves money for inventory optimization. It gives them better planning. It gives them saving money on raw material because they know what they're going to demand be so they can purchase it beforehand. So we call this product as Olive. And we're working with Jack in the Box. We're working with Home Depot for similar use cases. So that's the company that we have. The second part of my life in ecosystem is teaching across various, you know, um various industries maven is a huge part of that my ecosystem in fact one of the major reasons that i was able to quit google was i started maven i started teaching on maven and maven gave me enough money or like i made enough money on maven to get started with that right so I would, I like to say 10, 15% of my entire year revenue comes from Maven and, you know, teaching different courses apart from Maven.

**Aakash Gupta** (00:25:24)

And the remaining comes from, you know, working in my organization, you know, working with our customers, subscription services for our products, so on and so forth. And that's how we have been building slowly our company and learning about, you know, actually becoming an AI PM myself.

**Hamza Farooq** (00:25:43)

Yes. So you're practicing these skill sets day in, day out. That's so cool. Why keep the Maven course around if you have a successful software startup? It feels like most people would just do one or the other.

**Aakash Gupta** (00:25:56)

You see, I'm going to let you into a secret. I teach, yes, because I make the money, but I teach because I grow. So I teach two courses. I teach a foundation course, which is an AIPM grow course, because that's my learning on how I have learned to build empathy towards users and customers. And the crowd that we get over there are folks who really want to build something, but they do not have the tools to build them. So I learn from their ideas. I learn from their thought process. The second group is a developer course, which I teach on what we are building in our company. We build an open space. So our entire product is in public. So they're almost like an extension. So we give them, we work with them in problems that we are facing and how we solve them. So working with those developers or, you know, those engineering managers, senior engineering managers, they uplift my technical skill set.

**Aakash Gupta** (00:26:49)

So, you know, there was once, you know, we were sitting with friends and, you know, somebody asked me that, Hamza, if money was not a problem, what would you do in your life? And my wife said, he will still teach. Uh-huh. Right? I mean, I also teach at Stanford SPD. I also teach at UCLA. I also have a book. They are also, you know, rewarding in terms of the experiences that I gain, because otherwise you will not, like, yes, you will talk to customers, but you will not talk to so many people. Like, I met somebody from Airbnb, and he was one of my students in the course, and he was like, I think we should take what you have built for Airbnb. Do Airbnb and tell them do this now.

**Hamza Farooq** (00:27:35)

Love it. Amazing. Hamza, thank you so much for coming. If you guys want to check out his Maven courses, you can use code AkashXMaven to get a discount. He has two courses, as he said, Agentic Engineering Bootcamp and Agentic AI System Design for PMs. I recommend them both. Hamza, thank you so much for being on the podcast. Absolutely, Akash. It's a pleasure. So if you want to learn more about how to shift to this way of working, check out our full conversation on Apple or Spotify podcasts. And if you want the actual documents that we showed, the tools and frameworks and public links, be sure to check out my newsletter post with all of the details. Finally, thank you so much for watching. It would really mean a lot if you could make sure you are subscribed on YouTube, following on Apple or Spotify podcasts, and leave us a review on those platforms.

**Hamza Farooq** (00:28:25)

That really helps grow the podcast and support our work so that we can do bigger and better productions. I'll see you in the next

**Aakash Gupta** (00:28:34)

one.
