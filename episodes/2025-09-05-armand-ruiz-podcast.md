---
title: "AI Agents for PMs in 69 Minutes — Masterclass with IBM VP"
subtitle: "How companies are moving beyond chatbots to systems that actually complete work"
date: "2025-09-05"
host: "Aakash Gupta"
guests: ["Armand Ruiz"]
speaker_names: "substack"
substack_url: "https://www.news.aakashg.com/p/armand-ruiz-podcast"
youtube_url: "https://www.youtube.com/watch?v=g-Yb7CFWItk"
duration: "01:09:20"
word_count: 11047
source: "Substack episode transcript (aired audio)"
---

# AI Agents for PMs in 69 Minutes — Masterclass with IBM VP

*How companies are moving beyond chatbots to systems that actually complete work*

**Armand Ruiz** (00:00:00)

Can you break down for us, what is an AI agent? Because we've all experienced

**Aakash Gupta** (00:00:03)

ChatGPT, but what makes an agent so special? Well, for me, agents is really delivering on the promise of AI. Now we got into this chatbot era, but agents do really deliver the world of automation. You have this tremendous handwritten drawing demonstrating what are agents. So can you walk us through the steps? Yeah, four simple steps. The first one is thinking. Second step, the planning. And then the third component is action. Fourth step is reflection. Simon Ruiz is the VP

**Armand Ruiz** (00:00:29)

of AI Platform at IBM, and he has amassed over 200,000 LinkedIn followers in just two years for his takes on AI. So you've been in AI for 16 years. What have been the biggest open source

**Aakash Gupta** (00:00:39)

releases over time? LLMs. I think Mistral did massive things when they came into the market. They were also, I think, the first to provide a mixture of experts. There are hundreds of thousands of open source models. So let's get to IBM. How is IBM going to make big waves in the AI space? One of the things I'm very bullish is about providing customers flexibility to deploy AI anywhere and to tap into any AI engine they want.

**Armand Ruiz** (00:01:02)

It's about jumping in, using the tools. What's like a good roadmap if you had to give somebody, if they're going from zero to one to ramp up on all these tools, like which tools should they try first and what order? I think first. Really quickly, I think a crazy stat is that more than 50% of you listening are not subscribed. If you can subscribe on YouTube, follow on Apple or Spotify podcasts, my commitment to you is that we'll continue to make this content better and better. And now on to today's episode. Arman Ruiz is the VP of AI Platform at IBM and has amassed over 200,000 followers on LinkedIn in less than two years for his takes on AI. In today's episode, we're going to break down everything you need to know about AI agents and open source AI. We also cover his path from intern to VP in less than 14 years and his takes on the future of the product management role.

**Armand Ruiz** (00:02:03)

Armand, welcome to the podcast. So happy to be here. Finally, we make it. Yeah, I think we both were talking off air that we mutually have been reading each other's work on LinkedIn. So it's really exciting to chat. I think it has this cool effect, which I can see as a reader, which is I almost feel like I understand how you think.

**Aakash Gupta** (00:02:22)

same same here i've been following your journey your newsletter listening to your podcast so yeah very impressive work thank you

**Armand Ruiz** (00:02:28)

likewise daily linkedin posting

**Aakash Gupta** (00:02:30)

for

**Armand Ruiz** (00:02:31)

you for two years and i think this thread you've been on probably for almost the last year so a lot earlier than other people is ai agents so can you break down for us what is an ai agent because we've all experienced chat gpt but what makes an agent so special

**Aakash Gupta** (00:02:46)

Well, for me, agents is really delivering on the promise of AI. So we've been through this journey where I've been working in AI for 14 years now. And at first, it was just predictive analytics, doing predictions, giving just rough numbers for forecasting and things like that. Now we got into this chatbot era. But agents, they really deliver the world of automation that is going to unlock everyone and people and businesses to generate way more output so that's why i'm extremely bullish i'm very excited about it and yeah i've been talking about agents from the very very beginning and there were already some early projects showing the the the potential baby agi or auto gpt those were amazing and and then yeah the whole world now is prioritizing agents

**Armand Ruiz** (00:03:39)

Yeah, those are, I think, almost 2023 news. It took two years for the world to really catch up.

**Aakash Gupta** (00:03:45)

Yeah, absolutely, absolutely. So part of my job right now at IBM is to lead AI platform, so really building blocks for enterprises to build securely AI agents and embed them into different business functions. I just came yesterday night from meeting a CIO. I had met another CIO last week. So I'm meeting some of the biggest customers from the biggest brands. They all have AI as the number one priority in their agenda. And an agency is one of the core components. So there are a lot of different factors on how they empower employees to experiment with the technology. But then at the same time, how they are. can take it into production in a very safe and secure way and there are everything in between in different levels of risk and innovation appetite that they have

**Armand Ruiz** (00:04:35)

so as someone who's educating people about ai agents when i saw your handwritten drawing i was just like that is a piece of art that is something that really helps people understand ai agents so can you walk us through this like what are the building blocks of an ai agent

**Aakash Gupta** (00:04:49)

Yeah, so the first phase is thinking. We've been in this world of LLMs. We've seen LLMs at first that were just spitting text. And now we see that step of thinking. Thinking is number one step. That's where we hear about LLMs being very good at reasoning. And also, we hear Jensen saying, hey, with agentic systems and new LLMs, we're going to use more tokens, more inference, because that reasoning step takes extra compute, but gives you the kind of chain of thought process that we used to do manually, and now it's built into the LLM. And to go to step two, which is planning. So you ask for a task. And the LLM is going to break down that task into subtasks. And for each of them, we'll go and execute. And in some cases, we'll challenge the output from the previous step. But it's going to be able to create multiple subtasks and goals.

**Aakash Gupta** (00:05:55)

And then it's going to go into ACT, which is step number three. And ACT is maybe one of the most fascinating steps because it's going to allow you to tap into execution of actions. So if you need to input something to a CRM or send an email all the way to sending, not just to write the copy, or whatever action it can be, for example, in a system like Workday can go and interact with information for a specific employee. There are so many different things that you can do in the act phase that is being opened up by protocols like MCP. And then reflection. uh that's step number four reflection is really uh what is going to make agents really good because maybe at first a little bit raw but then with human input they will iterate and become better and better and better over time so that reflect step comes with like some technical implementations that you need to do that but you will be able to tap into the all the past history of interactions and learn from it from it and feed it back into the agent so next time it executes it does it better

**Armand Ruiz** (00:07:08)

so there's so many different terms and frameworks out there that people have heard about ai agents what are the frameworks they should understand and how do they fit into these steps

**Aakash Gupta** (00:07:18)

frameworks uh you mean developing development frameworks yeah i think i would like to um classify them into two categories there is like the coding frameworks. And these coding frameworks are becoming simpler and simpler, but still you need to know, in most of the cases, Python. But you have frameworks like LandGraph or CrewAI or LlamaIndex or Autogen. Those are excellent frameworks, open source, widely popular, and with a lot of information, documentation, and courses online, you can go and try them out. but then you have on the flip side you have like uh low code no code tools one we we have at ibm that is very popular it's called lang flow um i saw the new announcement from lindy there is um there is na8 and yeah which is also getting uh very popular uh stack ai uh from a fellow spaniard here in in san francisco as well also taking off Flow-wise, there are a lot of tools that help you build these agents in a very simple way.

**Aakash Gupta** (00:08:26)

Still, you need to understand the concepts, but it helps a lot with the development.

**Armand Ruiz** (00:08:31)

okay so if you're not a very technical person you can use some of these no code tools lindy n8n make.com zapier you name it they're all becoming huge or if you're trying to develop a more robust internal system you're going to work with developers to build on top of a crew ai or a lane graph is that right

**Aakash Gupta** (00:08:50)

that's that's right i think those programming frameworks give you needed control and flexibility that for very complex and genetic implementations, you still need. And those are evolving quickly. And I think also the exciting piece of that, those are open source projects. You can go to the GitHub. Something I do sometimes is I go to the repos, I see the PRs and the issues and the conversation in the repo itself and what people are asking and And anyone can contribute to those frameworks and make them even better. So there is a lot of fast innovation happening at that space because of the power of the community and the ecosystem.

**Armand Ruiz** (00:09:35)

JOSHUA SHARFSTEIN- You just mentioned building things. And that's when I've really figured out what is RAG versus what is fine tuning versus what is the other elements of context engineering. But for someone who hasn't gone through that, what is RAG useful for? FRANCESC

**Aakash Gupta** (00:09:49)

CAMPOYO- So RAG is useful to give additional context to an LLM. So if we step back for a second, LLMs are trained with data at a point in time. And obviously, for most use cases, you need to inject new updated data in order to get the output you're looking for. In order to do that, the most popular technique is called RAC. You can use fine tuning, but fine tuning is not really to inject new updated data that is changing all the time. It's fine tuning. Actually, one of my most viral posts is a guide on when you should be doing fine tuning versus RAC. But Rack is basically great in order to connect directly to a knowledge base, to a database, and it's a space that is evolving extremely quickly. My first year... After the release of ChatGPT, 90% of the use cases we were doing for enterprises were RAC use cases, because it's one of the most powerful methodologies.

**Aakash Gupta** (00:10:56)

You can tap into all this structured data, but also unstructured data, and just feed it directly into an LLM. So I think it's a goldmine for most traditional companies that are sitting on a lot of valuable data.

**Armand Ruiz** (00:11:09)

Wow, 90%. So tell me a little bit more. How are enterprises using RAG systems? What are employees using RAG for? How does that help them build a better agent?

**Aakash Gupta** (00:11:18)

Yeah, think of Rack as one of the core components of an agentic system. You can use Rack just simply on a chatbot. But if you're taking it into an agentic application, Rack is basically the component that is going to, let's say, just stepping back, we have think, we have planning. And most likely, in the planning phase, you will have a step of fetching some data from somewhere. So that's a Rack pipeline right there. So users and my customers are just looking at ways to tap into massive amounts of data instantly. We've been very big on enterprise search, but most of that enterprise search has always been at the metadata level. and this is taking it to a whole new level this is allowing us to tap directly into the information on on those documents and structured data so you can go tap give me like the the top use cases for for a specific uh for my top 10 customers and and then you can export directly from whatever reports or documents you have and get that directly into for example a product manager and then they can start making some assumptions on which feature they should be developing for example to go and accelerate development in certain areas so um yeah there is Some say we're in the age of ideas.

**Aakash Gupta** (00:12:44)

So with these new tools and new access to intelligence tab to enterprise data, my area is really on the enterprise side. That's where we see an explosion of new use cases.

**Armand Ruiz** (00:12:58)

Are there particular technical frameworks or things people should know about when it comes to RAG, like different options to implement it?

**Aakash Gupta** (00:13:05)

Many, many different options and many different building blocks and ways you can do that. At the end of the day, we are... We are building these pipelines that they do a lot of different things. So it seems like all the hype is on the LLMs. But then you need good embeddings models. Embedding models are those that are going to convert text into tokens. And those need to be really good. And those need to be, they can be good in different languages. They can be faster. They can be slower. It depends on your application. You need vector databases. You need ways to do filtering, search, ranking. So all that. And we have folks killing it out there with data engineering education, like Zach, for example. Because a lot of the problems in AI are data engineering problems. They are connecting the LLMs to all these very complex data systems.

**Aakash Gupta** (00:14:08)

And in order to do that, that scale is very, very complex. And for that, you have a lot of different technologies. If you are more on the AI application layer, we have frameworks like LimeChain that we mentioned and so on, Lama Index. And if you are more on the heavy data side, then you have things like Spark or Airflow or things like that.

**Armand Ruiz** (00:14:29)

Okay. So that's where all those terms fit in. And then there's this concept of vision rag. What does that help you do?

**Aakash Gupta** (00:14:37)

Yeah, so as we mentioned, Rack extracts information, adds context into the LLMs, right? And a lot of that information, it's in the structured documents. So very rich PDFs with very complex tables or charts with a lot of valuable information. So Vision Rack is taking the classic Rack that is more just based on text, And it's opening up to more multimodal scenarios. And it's adding that component. There are some LLMs that are great for multimodality nowadays. But then also, you have open source projects. One from my colleagues from IBM called DocLink, which is available on GitHub. It's a free framework that you can go grab. And it's going to be really good at getting info from, like, Word documents, PDFs, PowerPoint, a set of different file formats and extract all that information visually. And then you can fit it into a RAC pipeline. So that's what we call Vision RAC.

**Aakash Gupta** (00:15:44)

It's also very popular and is opening up new use cases.

**Armand Ruiz** (00:15:52)

And I think Vision Rag is really important for charts, right? Because there's so much rich data that lives a chart.

**Aakash Gupta** (00:15:57)

Yeah, yeah. If you're in some industries, like, for example, in health care, you need to read charts that come from very advanced equipment. Or you're in finance, and you have a lot of charts for the markets, right? Or tables as well. Tables many times come, they're exported from a spreadsheet and put together in a nice report on a PDF. There is so much you need to do in order to understand what the chart is saying, what the table is saying, what are the conclusions. So yeah, that's why vision rack is becoming super critical and there are a lot of different ways to to build that i think the right combination here is to again build the right pipeline so with the right components like dock link that i mentioned and then have very good multi-model models that are able to also understand like image as input for for the prompt

**Armand Ruiz** (00:16:55)

Today's episode is brought to you by the experimentation platform Chameleon. Nine out of ten companies that see themselves as industry leaders and expect to grow this year say experimentation is critical to their business. But most companies still fail at it. Why? Because most experiments require too much developer involvement. Chameleon handles experimentation differently. It enables product and growth teams to create and test prototypes in minutes with prompt based experimentation. You describe what you want. Chameleon builds a variation of your webpage, lets you target a cohort of users, choose KPIs, and runs the experiment for you. Prompt-based experimentation makes what used to take days of developer time turn into minutes. Try prompt-based experimentation on your own web apps. Visit chameleon.com slash prompt to join the waitlist. That's K-A-M-E-L-E-O-O-N dot com slash prompt. AI evals are one of the most important skills for PMs, and I know you know they matter.

**Armand Ruiz** (00:17:52)

The question is, are you doing them right? Most teams are winging it with basic metrics and hoping for the best. Meanwhile, the teams that actually ship reliable AI, they've cracked the code on systematic evaluation. Today's episode is brought to you by the AI evals for engineers and PMs course, by Hamal Hussain and Shreya Shankar. This live Maven course will teach you the battle-tested frameworks from Hamal and Shreya, who are the engineers behind GitHub Copilot's evaluation system and 25-plus production AI implementations. Four weeks, live instruction, next cohort starts July 21st. Start shipping AI that actually works. What do most teams get wrong implementing RAG Systems?

**Aakash Gupta** (00:18:52)

I think at the end of the day, a lot of the conversations that I have with customers are frustrations on accuracy. I think in the consumer space, a little bit of lack of accuracy is acceptable. You can keep iterating and it's not like a big system is going to go down and affect millions of customers. But when we are talking about, for example, putting a customer service chatbot that needs to connect to Rack, it needs to be very, very accurate. Like 70% accuracy is not acceptable. Or we have used cases where the human is not interacting with the system. It's like machine to machine. And then you need to have the right humans in the middle. So you need to build very trustworthy systems. And what many people are getting frustrated is about the accuracy of the rack because they are just applying some vanilla, out-of-the-shelf templates and implementations.

**Aakash Gupta** (00:19:52)

So you need to really build a strong practice to properly evaluate the outputs. And at the end of the day, it's really a data problem. So, yeah, you need to build that practice to properly evaluate and understand what is an acceptable business accuracy for the use case, and then just keep iterating in the architecture in the different configurations that you need to do in your pipeline in order to build that accurately. So that's one. I think they are also underestimating the power of Rack, because Rack is providing... Like, if Google was unbelievable to provide access to information for everyone, at the end of the day, they are providing, like... set of links, and then you need to go and find the information. Rack is giving that superpower to every single company to build that at scale, to tap into all the company's information for every single employee.

**Aakash Gupta** (00:20:54)

And there is so much that can be done in that space. But in order to do it right, it needs very heavy engineering at this point.

**Armand Ruiz** (00:21:05)

Hmm. So if you're thinking about evals, that's usually an area that people talk about just in the context of the final output. But it sounds like you're saying evals are really important in the RAG system itself.

**Aakash Gupta** (00:21:21)

Yeah. And yeah, I mean, the evals, the RAG space and the eval space, keeps evolving super, super fast. And there are new techniques, new companies innovating in that space. I think evals in agentic workflows should be almost put at like every single step if you're really serious about developing something, a critical system. And then you need to evaluate at different points before you put something into production. At the end of the day, evals is basically adding that human expertise to validate the output of what the AI system is giving you. So if you have a system that has a lot of multiple steps and you are only checking the output at the end of the spectrum, I think you are missing. I think in classic software development, you will have evaluation in different points. So it doesn't change that much in that front. It's just more about the methodology on how you do it.

**Armand Ruiz** (00:22:27)

OK. And how do you do good evals for a RAG system?

**Aakash Gupta** (00:22:31)

There are, again, this is an area where there are a lot of papers talking about good techniques. And then it's pretty cool that the frameworks and the open source community is coming with projects to help to help customers or users to do that at ibm we have something called the evil studio that basically allows allows the either the developer or the business user to do like proper evaluation of the outputs and and there are different ways there are ways that makes um um They mix synthetic data with human check-ins, with having a data set that has the ground truth. There are different tools. We've been pushing one that is called Evaluation Studio, which is GUI-based. Because we also understand a lot of the use cases, the knowledge and the expertise is in the SMEs and the business users. And they know very well what is good and bad.

**Aakash Gupta** (00:23:35)

And they need to be able to assess the outputs of an AI system. And this needs also, it's not a one-off. That is just you do it once and then to the next agent. These systems need to continuously be checked and improved. And that's really the power.

**Armand Ruiz** (00:23:53)

Yeah. It's like any internal tool you're going to build. There's going to be ongoing maintenance. Absolutely. With an AI agent, a lot of it is in the evals phase.

**Aakash Gupta** (00:23:59)

Yeah.

**Armand Ruiz** (00:23:59)

I think that's a really interesting insight that you want to equip your SMEs to be able to help you with those evals. You don't want to just be doing those in some engineering silo.

**Aakash Gupta** (00:24:09)

Yeah, that said, there needs to be some framework on how you do that. When we're talking to companies like my set of customers that are like hundreds of thousands of employees, you need to put some best practices and frameworks on how you do that at scale in a company. So I think that's a little bit the challenge in a lot of these companies. Everyone has a lot of ideas, and it's how they can experiment in a safe way. And then also, a customer told me recently, they don't want to spend like $20,000 in compute to get a benefit of like $100, you know? So this false illusion of, like, I'm using AI, I'm being more productive. But what's happening underneath is, like, you're spending a lot on execution, either on the pipelines or on the AI compute. So there needs to be, like, frameworks. Some are talking about, like, AI hubs or an AI office that tracks all those projects.

**Aakash Gupta** (00:25:14)

And you want to encourage innovation and use case creation. But then at the same time, you need to have a way to assess those projects.

**Armand Ruiz** (00:25:23)

Yeah. So you've said most employees should be getting to the stage where they're managing 10 to 20 agents. How do you think through what agents you should be building?

**Aakash Gupta** (00:25:32)

It depends on the business practice. Let's take, for example, you are sitting in marketing. If you see all the things that I'm sure you want to do, you have bottlenecks in different areas, right? Maybe you have a bottleneck in terms of like You cannot iterate fast enough on the copy because you are relying on some third-party agency, and then the turnaround maybe is one week. So using agents, maybe you can, what takes a week and a set of maybe meetings, you can do it in one or two days or even faster. Then maybe you have challenges as well creating advanced... um just creative material videos images charts that are impactful again you can use ai for that or or you wanna uh in in experiment with a b testing on the website you can have ai to create different iterations of your website of your copy So at the end of the day, I think everyone, depending on their function, will have different specialized agents that can give either recommendations or full automation on execution of certain tasks.

**Aakash Gupta** (00:26:43)

And then you will be able to generate more output.

**Armand Ruiz** (00:26:47)

So it's almost like managing a team under you and you need to figure out what are the right stages of human in the loop or human approval so that it doesn't just go out and misrepresent our brand or something when marketing, but at the same time, it is reducing the work we have to do it.

**Aakash Gupta** (00:27:03)

yeah there is this concept of orchestration that everyone has been talking a lot about this year which is this need of orchestrating agents and a lot of our our job is going to be on the judgment of the output of some of those agents again i think we're far from that reality three to five years not because of the state of technology we are here in silicon valley and we see this ai first ai native companies that are built from day zero with this agentic mindset. But then when you talk to more traditional companies, there is a long journey in order to get there. But orchestration of agents and being able to quickly iterate on them and orchestrate them and check the outputs that they are generating are good. Because ultimately, it's going to be the responsibility of the humans. That's a new skill we all need to go and get used and learn.

**Aakash Gupta** (00:28:07)

How do people get better at orchestration? I think, honestly, I don't have a very clear answer. A lot of companies, they are working on AI literacy, so learning. So I think getting hands-on with the technology is really important. um if you use the early days on the internet you were on a on a console and then we moved into easier and easier interfaces right so um i'm sure the technology it's being already democratized so it's going to be accessible for everyone but then at the end of the day it's good good education content like the one you're creating and and good courses and then um yeah target targeted for specific functions is going to be very critical

**Armand Ruiz** (00:28:53)

So if you're a product manager, what AI agents should you build first?

**Aakash Gupta** (00:28:59)

I think, well, first of all, product management I think is also one of those functions that is changing. I lead a team of product managers, and I think usually the ratio, the standard ratio that I've seen in the industry, which we don't always follow, is like a product manager for six to 10 developers. So you tend to have product managers that are really focused on one specific area of your product. So for example, in my AI platform, I have a PM that is really focused on tuning techniques, another PM that is really focused on inference and serving models. And you have these PMs that are really focused on certain areas. I think with AI agents, we can get into a different ratio. Instead of one to six to 10, maybe we can get one every 20 or 30 developers. And these PMs, they might be able to cover multiple areas all at once, because they have agents that can do competitive.

**Aakash Gupta** (00:30:05)

You can have an agent that is doing competitive analysis. It's a crazy market. I mean, the AI space is a crazy market. Every big vendor, small startup, YC, there is so much action. You cannot keep up. So you can have an agent that is doing research, another one that is building up reports for competitive. Those competitive analyses then need to be polished, and the salespeople need to be equipped in order to have a good conversation in front of a customer defending your product versus the competition. then you have a lot of, you need to prioritize all the user feedback. So with very powerful AI agents, you can match, you can have agents that can check your usage data from SAS metrics directly with maybe user feedback that comes from social media, from other systems that you have to collect feedback, NPS systems. And then you can start gathering more inputs to prioritize better your roadmap.

**Aakash Gupta** (00:31:08)

And then when you prioritize the roadmap and you come with a new feature, you need to write the PRD. AI can do like 80, 90% of the work. And then before even you validate and you prioritize the feature, that's where we can get into more details, but you can even prototype it, you know, and then work with a select of users to get some feedback. So that's, I think, where we are going with product management. And I

**Armand Ruiz** (00:31:36)

think the final step too, right? today's episode is brought to you by vanta as a founder you're moving fast toward product market fit your next round or your first big enterprise deal but with ai accelerating how quickly startups build and ship security expectations are higher earlier than ever getting security and compliance right can unlock growth or stall it if you wait too long With deep integrations and automated workflows built for fast moving teams, Vanta gets you audit ready fast and keeps you secure with continuous monitoring as your models, infra and customers evolve. Fast scoring startups like LinkChain, Writer and Cursor trusted Vanta to build a scalable foundation from the start. So go to Vanta.com slash Akash. That's V-A-N-T-A dot com slash A-A-K-A-S-H to save $1,000 and join over 10,000 ambitious companies already scaling with Vanta. Today's episode is brought to you by Amplitude. Replays of mobile user engagement are critical to building better products and experiences, but many session replay tools don't capture the full picture.

**Armand Ruiz** (00:32:42)

Some tools take screenshots every second, leading to choppy replays and high storage costs from enormous capture sizes. Others use wireframes, but key moments go missing, creating gaps in your understanding. Neither approach gives you a truly mobile experience. Amplitude does things differently. Their mobile replays capture the full experience, every tap, every scroll, and every gesture, with no lag and no performance hit. It's the most accurate way to understand mobile behavior. See the full story with Amplitude. Today's episode is brought to you by the AIPM certification on Maven. Run by Mikdad Jaffer, who is a product leader at OpenAI, this is not your typical course. It's eight weeks of live, cohort-based learning with a leader at one of the top companies in tech. OpenAI just doesn't stop shipping, and this is your chance to learn how. Run along with product faculty and Mo Ali, the course has a 4.9 rating with 133 reviews.

**Armand Ruiz** (00:33:34)

Former students come from companies like OpenAI, Shopify, Stripe, Google, and Meta. The best part? Your company can probably cover the cost. So if you want to get $500 off, use my code AAKASH25. And head to maven.com slash product dash faculty. That's M-A-V-E-N dot com slash P-R-O-D-U-C-T dash F-A-C-U-L-T-Y. Once you release it into production, it can monitor if all of the sudden users are getting some corner case you didn't realize. And then two or three weeks later, it can tell you, hey, here's what the statistically significant results were. So it's like across every step of the PM life cycle.

**Aakash Gupta** (00:34:12)

Absolutely. Absolutely. It's one of the most exciting functions because, as I mentioned before, we are in this world of ideas. And I think PMs have, as part of the job description, is to bring some of these ideas to life. Yeah. You know, and if you you work in product management, you know, like it's been always kind of like a frustration to turn ideas into not features, but sometimes even validating the idea. Right. You need to work with design, maybe get the mock up. have user feedback and work with engineering and engineering is overwhelmed with production tickets on support and things that need to be fixed and new feature development so yeah it's it's that's why I think also PMs all the PMs that I usually hire are really good technically and now with AI they will be able to take it to like three four steps further by themselves

**Armand Ruiz** (00:35:16)

So you recently commented on this idea of writing first versus prototype first cultures. Talk to me a little bit more about what the future of the role looks like, the future of the PRD in this world.

**Aakash Gupta** (00:35:28)

Yeah, I'll tell you a story, a personal story about that. And I think that that built a lot of success in my career. That's more than 10 years ago. But I'm from Spain. I moved to the US. My English was very, very rough. And we had this big meeting with a lot of big executives, how to reimagine how the next machine learning platform is going to be. And at that time, I still remember I had the meeting in two days. And I was really struggling to articulate all the ideas that I have. So I said to myself, I'm going to build a prototype. And to my surprise, in that meeting, everyone was just talking and showing slides. And I was the only one that was showing. I was showing the product. You can touch it. You could see it. It was nothing close to production. It was all kind of like fake, but giving the ideas and the art of the possible.

**Aakash Gupta** (00:36:22)

And guess what? I got to lead the project. That became kind of like the default and the path forward. So I think that's what is happening right now. Before, I had to just get hands-on, start coding, and do a lot of the work I could have done. that now in maybe like three or four hours. So now with all the tools, I think every single PM should have access to by coding tools, different options out there in the market. And to just kind of like skip ahead and show some of those ideas directly into working prototypes. And that also helps a lot with communication. The teams I work as well, they are worldwide. So there's also language barriers. A lot of the work in big corporations is all about communication. And that communication is either in meetings or written or in GitHub repos. So a lot of things are missed in translation.

**Aakash Gupta** (00:37:24)

So I'm a big fan of showing and skipping a lot. And even if you write the most beautiful detailed PRD, still a lot of information is lost in translation. And just there is nothing that speaks better than just a working prototype.

**Armand Ruiz** (00:37:43)

There is some worry out there that we're going to start to get into a more feature factory solutions focused world. We're not going to heavily investigate the problem space if we just jump into AI prototypes. What's the right... step the right life cycles to make sure that you are investigating the problem space, but you're also taking advantage of this new prototyping technology.

**Aakash Gupta** (00:38:04)

Yeah, that's a very valid concern. I spend a lot of time with customers. I think that's, and again, that's also part of how I build my career. Like my first two years, I was traveling every single week to visit customers. I spent two years traveling. I had no wife, no kids, so I was free to meet a lot of customers all over the world. And it was unbelievable, not only network, but just going deep into what they were doing, trying to figure out the problems. And I didn't have LLMs, but I started framing my own ideas, hypotheses, and checking what was going on in the market to build solutions. So I think you always need to start customer first. And PMs, in my opinion, they need to spend a lot of time talking to customers and going deep, not at a high level, but just really trying to understand what are their challenges and then figure out how your product can solve.

**Armand Ruiz** (00:39:04)

All right, so let's zoom back out of product management for a second and just talk about general tech workers. You've encouraged people to learn Python, get technical, even you've asked leadership to get more technical in the AI era. Why is that so important?

**Aakash Gupta** (00:39:19)

Yeah, and I think everyone should have technical literacy in this day and age. Otherwise, I think you are completely going to miss out on the opportunities of AI. One that articulates this very well is Aaron Levy, the Vox founder and CEO. He says, you have two ways to approach AI, either as a cost savings tool, that's completely fine. Or you can just go do way more with AI. So in order to do way more, and I think that's the right approach. I think that's how companies will grow, will expand. Work is going to be more fun because we're going to be able to accomplish new use cases and new work. In order to do that, you need to understand the art of the possible AI. And there is no document, white paper, LinkedIn post, video that is going to teach you the art of the possible unless you actually try the technology.

**Aakash Gupta** (00:40:21)

So luckily, I mean, if you learn how to code in Python or do the basics in Python, that's completely cool. Luckily, the technology is getting democratized, so you can still touch the technology and not code at all. But you need to understand the concepts. And a lot of the leaders in the space, they have a lot of ideas on things they should be doing and they can do. And they need to understand how the technology bridges that gap. So yeah, I'm spending a lot of time learning myself. Many people ask me how I'm so up to date or I write about this content so often. I mean, number one is I'm obsessed with it. So it comes to me naturally. So every time there is something new, I just jump and I try it out in the evenings usually. And then I start to form my own opinions based on my professional experience.

**Armand Ruiz** (00:41:23)

So it's about jumping in, using the tools. What's like a good... if you had to give somebody, if they're going from zero to one to ramp up on all these tools, like which tools should they try first in what order?

**Aakash Gupta** (00:41:36)

Yeah, I think first just understanding the concepts and then tools. I think everyone should just develop one AI agent. And there are a lot of different tools. You can do that with no code flow builder. There are many out there. I was actually trying yesterday the new Lindy. Yeah. AI. Very, very, very impressive. At IBM, we have a tool called Lang Flow as well, which is a low code flow builder experience as well. At the end of the day, if you see each of those tools, they still require you to understand the concept of AI. So I always recommend start with the concepts and understand what is an LLM, understand what is reasoning, understand what is RAC, and some of those things. And then use any of those tools that give you like the building blocks and just think about one use case that you have in your own personal job or life and then try to solve it, you know, and try any of those tools.

**Aakash Gupta** (00:42:40)

And then if you want to go deeper and deeper. I think it depends on the role. If you are into leadership, I think there is a lot of education about how you inject AI into an organization and change management and so on. If you are more on a practitioner practice in different domains, I think you will have a lot of authentic solutions that can help you speed up your work. So there are a lot of different options.

**Armand Ruiz** (00:43:10)

OK, so build with a no code tool. Then what's the next step? Do you go into like a cursor or something like that? Do you learn to program? Where should people go after?

**Aakash Gupta** (00:43:19)

Yeah, like programming. I think also by coding is a big one because I think you need to understand the different levels. I don't expect everyone right now to just create something and put it into production in an enterprise setup. I think that needs to be a little bit somehow controlled, depending on data access and tool access. But yeah, start with developing some agents. Try bi-coding. If you are curious, try different things that are more advanced using Python, depending on your level of expertise there. I mentioned earlier, deep learning AI, amazing short courses. And yeah, it's interesting because you can, if you want to, for example, hey, I heard about Rack every day. I see it on my timeline every single time. I log into LinkedIn or X. Just do a quick course on Rack. You will really understand that it takes like three, four hours. And then you can understand, hey, basically my entire organization can access all the information if we build these Rack pipelines really good.

**Aakash Gupta** (00:44:34)

So maybe something we should invest. And you can do it in-house. You can... do it through a vendor you can have like a third party help you build those but you need to understand those concepts because again people in the business need how they have the ideas and the use cases and in in their heads you

**Armand Ruiz** (00:44:52)

know let's shift focus to open source ai ibm and you in particular have had a lot of focus on open source ai can open source really win it feels like it's always a cycle behind closed source

**Aakash Gupta** (00:45:05)

Yeah, I think we need to understand in the enterprise context that I'm coming from. And I think in that enterprise context, open source, I would say, always wins. Oh. Yeah. Like, let's take the latest OpenAI model, right? Why everyone is so excited, especially in the enterprise. First, the license is unbelievable. It's an Apache 2 license, which is really good. Then it's a very good reasoning model. Like, I think we've been lacking some very good reasoning models in the open source space. And then you can just take them and deploy them anywhere. So you don't have to rely on a third party API call where you most likely, for most of my customers, they cannot just send a lot of confidential information there or they cannot connect it with their own tools. So right now you can take that model, make it your own, deploy it anywhere in your own infrastructure.

**Aakash Gupta** (00:46:05)

A lot of customers are still running on their own infrastructure. They are creating their own AI factories with different AI accelerator providers like NVIDIA, AMD. So you can deploy it on your own machine. So open source provides a lot of control for enterprises, which is a great thing. Then I think the pace of innovation of the community, even though sometimes it's a little bit slow at the beginning, at the end of the day in the long term it shows up and i i think we've been a little bit through a cycle i think last year on we were we could see open source models getting closer and closer to closed source and then i think this year it's been a little bit different and tropic google with gemini and open ai with gpt5 they they showed that they are still ahead

**Armand Ruiz** (00:46:52)

yeah

**Aakash Gupta** (00:46:53)

but you will see again the open source community running behind and and and pushing that forward and lastly is developer ecosystems What we were talking at the beginning on all these different frameworks that actually enable companies to develop applications, they are built on open source as well. And they are deployed on open source systems like Kubernetes and VLLM. VLLM is basically the engine to run models, you know. So, yeah, I think it's not just the LLMs itself, it's the entire AI ecosystem. PyTorch is another great example. Everyone is building on PyTorch, which is also open source. So I'm very passionate about open source, and I think in the long term it always wins.

**Armand Ruiz** (00:47:40)

What's PyTorch for people who don't know?

**Aakash Gupta** (00:47:42)

Pytorch is basically the framework that allows you to create very complex deep learning algorithms and run them.

**Armand Ruiz** (00:47:52)

And just about all of the closed and open source foundation companies are building with Pytorch, right?

**Aakash Gupta** (00:47:58)

Pretty much all of them. And that's a project that came out of Meta. And yeah, it's open governance and everyone is contributing to it. And it's been used by every single major AI lab in the market. So you've been in AI for 16 years. What have been the biggest open source releases over time? It's been a wild journey because when we talk about open source, a lot of the conversation right now is with LLMs. So I think if we just focus for open source LLMs for a moment, I think Mistral did massive things when they came into the market. They were also, I think, the first to provide a mixture of experts, open source model. Also, they did it in a very funny way with a torrent link. You have to get a little bit your way to go download. And then we had Lama building a fantastic ecosystem around open source models.

**Aakash Gupta** (00:49:01)

IBM, we open source our models. I can speak to that. And then now OpenAI and others. So there is innovation in the model space. If you go check Hugging Face, which is kind of like the repository of all these open source models that Clem and the team is building, there are hundreds of thousands of open source models. Then there is data as well. also available on HuggingFace. There are a lot of data sets, data sets for many different things, for pre-training, for post-training, for alignment. So these are also components. Major PyTorch, massive. TensorFlow looked promising. Finally, PyTorch took over. There is always kind of like at the beginning, you don't know which one is going to win. And then you let the community and the ecosystem move that forward. And in most of the cases, there are very technical decisions that are very critical or user simplicity.

**Aakash Gupta** (00:49:57)

And then a lot of the conversation as well is happening on potential alternatives to CUDA that provides a lot of control for NVIDIA. So it's a very exciting ecosystem and yeah, it is not stopping.

**Armand Ruiz** (00:50:12)

And it's operating at every layer,

**Aakash Gupta** (00:50:14)

really. Every layer. In every layer of the AI stack, you have three or four projects and new incumbents coming with new alternatives. And I think the beautiful thing about open source is let the best one win.

**Armand Ruiz** (00:50:28)

Yeah. You briefly mentioned pre-training, post-training, and alignment. For people who don't understand that, those are the steps in model building. What's one layer deeper? What's happening in each of those?

**Aakash Gupta** (00:50:39)

Yeah. And for 99.999% of the people, they don't really have to touch that. This is really done by the Frontier AI labs that they train the models. and basically in pre-training is when you basically gather all that clean data set and you and you train this is what you use to train your your model and then you have the post-training phase and alignment to to make sure it performs properly so these are different data sets that you use for that obviously we are running out of data so then you have new methods to create synthetic data, high-quality synthetic data, which synthetic data is data generated by AI algorithms, and then supervised by humans to make sure there is high quality. And all that process is what is used by all these frontier labs to train all these magic LLMs that we're using.

**Armand Ruiz** (00:51:39)

So let's get to IBM. How is IBM going to make big waves in the IEI space?

**Aakash Gupta** (00:51:44)

Yeah, so I joined IBM when we announced IBM Watson. And it's been a while decade with a lot of lessons learned and also things that we got right and things that we got wrong. One of the things I'm very bullish is about providing customers flexibility to deploy AI anywhere and to tap into any AI engine they want. So what does that mean? That means our customers, they sit on a lot of data, as I mentioned before. It's a gold mine of data. They need to execute that AI close to that data. Cost per token is extremely important. So I think we are one of the only providers that provide all this flexibility to deploy the AI very close to in the infrastructure they want, whether it's a hyperscaler, whether it's on-prem, on a private cloud setup, or a combination of all of those. So that's number one.

**Aakash Gupta** (00:52:47)

Then we've been developing also our own AI models. It's a family of models called Granite. But our customers, they want everything. The customer I was yesterday, and it's a trend I see with every single customer, they have all the options. So how you provide and govern access to all these AI engines, no matter where they run. So you make sure you have some way to understand the overall course, the access control, and things like that. And then we provide a lot of tooling on top to make sure we give productivity to developers. And at the end of the day, these systems are built for scale, massive scale. So we are working on different projects to help scale inference throughout multiple clusters in different environments. And then an area that I've been responsible as well is the governance piece. One that many people are thinking after the fact, and it should be thought before, especially in an enterprise setup.

**Aakash Gupta** (00:53:57)

So I'm sure you heard about a lot of the AI regulation that is coming to the market. And that regulation is being updated and is different sometimes by industry, by state, by country. And so you need to have an inventory of use cases. at different stages. And for those that are in production, they need to be compliant to a certain regulation. So we have very good tools in order to do that at scale.

**Armand Ruiz** (00:54:24)

Why is the Granite model important?

**Aakash Gupta** (00:54:26)

I think the Granite model has two, I would say. Maybe the research team will disagree with me. There are more. But I think we have two major components. One is cost per token. So these are very small models. One of the most popular ones is a $2 billion model that performs really, really well. So if you see what OpenAI released last week, the smallest one is $20 billion.

**Armand Ruiz** (00:54:53)

Okay.

**Aakash Gupta** (00:54:54)

These are different kinds of models. OpenAI model is very good at reasoning. But for certain use cases, what we see is cost per token is extremely critical. And for some use cases, you don't need generic models that know how to do everything. In enterprise setups, you need models that do one thing and do it really, really well. So these very small models are extremely good. They are very cheap and they run in hardware that in some cases is even commodity hardware. And then the second thing, I will add two more. The second thing is easy to customize. So we're talking about tuning or drag or things like that. The larger the model, the more complex every single thing you're trying to do is. So if it's a very small model, it's easier to tweak it, to tune it, to change the weights, and to embed it into different customization setups.

**Aakash Gupta** (00:55:52)

And then the last one, which is it was stock. a lot at the beginning of this AI craziness that we have going on. It was about the copyright of the data. For most of the models that we use today, we have no idea which data was used to train. All our data is actually is even disclosed on the white paper. Our legal teams, they went through it, has the proper copyrights and so on. And we provide that information very transparently to our customers. So that built a level of comfort for some specific use cases in certain industries that has been really good.

**Armand Ruiz** (00:56:33)

so the ai talent wars have gotten insane people have heard about one billion dollars for four years at meta for some of the highest paid ai researchers yet you're still saying that ai talent may still be underpaid what's your take on this like what's going on with these ai talent wars why is ai talent underpaid

**Aakash Gupta** (00:56:52)

i i got in trouble for that that post But I think I think there are two things here. One is like kind of like the ethical piece. It seems completely unethical that someone is making that absurd amount of money. But then you need to put things also into context. Right. We're in a capital allocation market and we're talking about talent that is very unique. I would say maybe there are like 200 of those folks worldwide. And those folks are the ones that are actually using all these capex being spent by the biggest and strongest companies in the world. So when you have one of those companies spending billions on AI clusters, And they are even talking about building nuclear plants to power those AI clusters. And those clusters, they are for training new models, tuning new models, serving new models. So you need the right talent to leverage that.

**Aakash Gupta** (00:57:57)

And literally, one architecture decision can use capacity on those clusters for weeks and months. So if you put the numbers into context, that's massive. That's number one. Those folks are really capital allocators right now, not only just employees. yeah and and second one is i mean you need to see the state of the market like a lot of these people they are either in their founders or or first employees of very well-funded companies so they have like very sweet equities uh at extremely high valuations right so if you see what they are what what is their opportunity Maybe they have two or 300 million on equity in some company. So if you want to hire them, you need to put a very sweet package. So I think that those are the two motions, like the capital allocation motion and like the state of the market. And where these technical folks that they are like founders of some of the most promising companies in the world.

**Armand Ruiz** (00:59:07)

Well, I just love to see the nerds get paid like athletes.

**Aakash Gupta** (00:59:10)

I mean, I heard there are AI agents, but not agents, like NBA agents for players that are helping you negotiate those contracts and things like that. It's wild. It's the nerds are taking over. Revenge of the nerds.

**Armand Ruiz** (00:59:29)

Amazing. So you have an amazing career story. You rose from intern to VP of AI. A lot of people would want to follow your trajectory. Of course, you know, you did good work, you made good connections, but are there things about the way you work or the way you manage your career that really helped you propel so quickly?

**Aakash Gupta** (00:59:50)

Yeah, I think this is one of those that would be careful what you dream because it might become true. I was a kid and I was just obsessed with being here in Silicon Valley, watching all the keynotes, the action happening with Apple and Oracle and all these companies. And I really, really, really wanted to be here. so every single thing i did either very intentionally or unintentionally took me here um and for some things i was like very very aggressive trying to get there i when i was in europe i wanted to be in a u.s company to get the visas to to get here and get sponsored and and so on um so that was one factor i think the other factor is is there is a component of luck. I joined IBM when IBM Watson was announced. And then I've been very consistent on that AI path.

**Aakash Gupta** (01:00:45)

Even on these AI winters that we had in between, I've been always working in AI and machine learning. And yeah, we are now in this stage where AI is the biggest thing in the world. So there is that luck factor. But I had a good intuition. I saw the promise of the technology. And I was very connected with all the developments that were happening with, for example, with NVIDIA and AlexNet and the promise of all this technology. But we didn't expect this to happen so quick. and then and then is also more about managing kind of like the corporate ladder right something i always recommend is network is very important and network and add value and just be humble and problem problem solving so yeah i've been always kind of lucky to be in these very hot projects and then part of my nature i'm very impatient i want to build things very quick And that fits the narrative in corporate America that people want to see results quickly and they want to see innovation.

**Aakash Gupta** (01:01:54)

So yeah, I was always with this mindset of building and showing, not telling. And then I've been lucky to surround myself with unbelievable colleagues that made things happen very fast. So that's been kind of like my story. I'm from Spain. I started working at IBM in Belgium, in France. I moved to Chicago. And then I've been here in the Bay Area for 10 years.

**Armand Ruiz** (01:02:19)

Wow. Very intentional journey to get

**Aakash Gupta** (01:02:22)

to

**Armand Ruiz** (01:02:23)

Silicon Valley and then seize the opportunity, stay grinding. A lot of people, they come to Valley, they see the gray weather, they leave after three

**Aakash Gupta** (01:02:30)

years.

**Armand Ruiz** (01:02:31)

You stuck it out. And that's really an incredible story. Another incredible story that you have is I believe June 2023 you shared was when you started your content posting journey. We're talking in August 2025, you have nearly 200,000 followers. I think it's like 194,000 today, right? By the time this episode published, it will be 200,000. How, and you've written about this a little bit, you use AI in your content creation process. How can other people use AI in their content creation process to grow like you did?

**Aakash Gupta** (01:03:02)

yeah um first why i started doing it i i think i always um wanted to be a better communicator and i think if you want to get good at something you just need to flex that muscle

**Armand Ruiz** (01:03:15)

yeah

**Aakash Gupta** (01:03:15)

so um and Because of the work I was doing, every time I was posting something, either at the time on blogs on Medium or sometimes on LinkedIn, I have posts from like five years ago that were getting like thousands of views, which is rare. They were resonating. So then I was like, okay, I'm going to try to put consistency in a framework and it's something I should have been doing before. And then I put a system just to collect ideas. And just write every single day. I have a post every day on LinkedIn at 7 AM Pacific. No, 4 AM Pacific, 7 AM Eastern. So kind of like when the US is waking up and it's still working day in Europe, you get an update from me. I will say, though, that I was using AI a lot more before. I barely use it these days.

**Aakash Gupta** (01:04:12)

Oh. And I think that's also part of the differentiation on good content. And I have posts where I had like two years ago, I had agents build with baby AGI and things like that. And I think at that time, I was always kind of like concerned that I didn't have enough information. So I had agents to do research, and they will just scroll YouTube, X, or different sources and give me what is the content that is getting more engagement. And then my content was really optimized to go viral. um which was good that that helped grow a lot um right now my content is more targeted to the people i want to talk to and the audience i'm going after and and that's helping as well with my my connections and professional experience so when i sit in front of a customer most of like 90 of the time they already follow me they know my content They have questions about it.

**Aakash Gupta** (01:05:16)

And that helped also inspire other people at IBM to help promote IBM technology. So I was very heavy on AI. I use it a little bit less these days just because I think just trying to spend more time thinking, that's a way to differentiate. Otherwise, the content is also getting democratized these days.

**Armand Ruiz** (01:05:42)

Yeah, it is, right? I also had a phase like two years ago when I was using AI and I felt like it was giving me an edge. Now I don't use it at all because it ends up leading you down the path of creating content like everybody else and that's the content that doesn't work.

**Aakash Gupta** (01:05:57)

Yeah. And I think maybe where I use it is more on the ideation. OK. So many people ask me, how do you have time to write so much? And I think if I didn't write, my thoughts wouldn't be structured and in order. And I need that for my job. So I was flying yesterday back from a customer visit. It was like a 24-hour visit to a customer. In the flight back, I just had so much information that I was kind of like structuring it and writing my thoughts, kind of like old school and pen and paper and a notebook. And I will use AI to kind of expand on those ideas, help me structure them, but then write something. And I usually have my own routine every day after kids go to sleep, just spend some time writing. And then the more you do it, the faster you do it as well yeah um at first maybe it will take you like 45 minutes to write something now it takes me maybe like five seven minutes you know wow because i i i don't have like these uh paralysis when i have to write i already know what i'm going to be talking about and more or less um i learned about formatting content and so on so Yeah, it's one of those things that you just need to do it regularly.

**Aakash Gupta** (01:07:20)

And then also track metrics as well if you really care about growth, what works and what doesn't.

**Armand Ruiz** (01:07:25)

Oh, yeah. I actually look back at the days you got more followers, the

**Aakash Gupta** (01:07:28)

posts

**Armand Ruiz** (01:07:29)

that got more likes.

**Aakash Gupta** (01:07:30)

Yeah. Yeah. but i'm also not super obsessed with that because um a lot of the content that gets a lot of likes and stuff is just reporting the news yeah and i think i can bring additional value on top just be just reporting what's happening in the market there are many people that are doing that very well so it's more about okay i'm i'm in this spot where i'm developing enterprise ai software and i talk to ai implementation in in enterprises so that's where i'm trying to spend more time so i I'd rather get maybe like 200 or 300 likes, but the people that are engaging are like executives in some of the most important companies in the world or aspiring executives than just reporting about the latest model in the market and getting like 3,000 likes. That's more valuable.

**Armand Ruiz** (01:08:19)

What an ending to the podcast. Armand, thank you. This was, I think, your first deep, long-form podcast. Cannot wait to share this with the world. Really enjoyed it. Thank

**Aakash Gupta** (01:08:29)

you for inviting me and looking forward for more. Thank you.

**Armand Ruiz** (01:08:31)

All right. So if you want to learn more about how to shift to this way of working, check out our full conversation on Apple or Spotify podcasts. And if you want the actual documents that we showed, the tools and frameworks and public links, be sure to check out my newsletter post with all of the details. Finally, thank you so much for watching. It would really mean a lot if you can make sure you are subscribed on YouTube, following on Apple or Spotify podcasts, and leave us a review on those platforms. That really helps grow the podcast and support our work so that we can do bigger and better productions. I'll see you in the next

**Aakash Gupta** (01:09:10)

one.
