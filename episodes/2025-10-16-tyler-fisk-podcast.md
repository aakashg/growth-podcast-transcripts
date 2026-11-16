---
title: "How to Build Multi-Agent AI Systems That Actually Work in Production | Tyler Fisk"
subtitle: "Stop vibe coding. Start shipping agents that make money."
date: "2025-10-16"
host: "Aakash Gupta"
guests: ["Tyler Fisk"]
speaker_names: "inferred"
substack_url: "https://www.news.aakashg.com/p/tyler-fisk-podcast"
youtube_url: "https://www.youtube.com/watch?v=WVU7MCfFet4"
duration: "01:41:02"
word_count: 17444
source: "Substack episode transcript (aired audio)"
---

# How to Build Multi-Agent AI Systems That Actually Work in Production | Tyler Fisk

*Stop vibe coding. Start shipping agents that make money.*

**Aakash Gupta** (00:00:00)

While we've all been doing vibe coding, Tyler Fisk has gone to the next level to build production AI. We are on a podcast right now, so no pressure at all. And we're going to do a live agent build here.

**Tyler Fisk** (00:00:13)

We're spinning up multiple agents here just to kind of get this process done and get all the context that we

**Aakash Gupta** (00:00:18)

need as quickly as possible. I love how many like parallel processes you have going here. My guest today, Tyler Fifth, is one of the world's most experienced AI agent builders in the world. He has taught thousands of students to build AI agents, and he has worked with hundreds of businesses to implement AI agents in their workflow. We

**Tyler Fisk** (00:00:37)

find that a lot of the work comes when we're doing this for actual clients and what we teach. It's this idea of the mentality of an AI practitioner. which happens to be very similar to like the forward deployed engineer mentality.

**Aakash Gupta** (00:00:50)

Anybody who's watched this far knows why you've hit that success. You just packed thousands of dollars of lessons into 60 seconds.

**Tyler Fisk** (00:00:57)

Deep research is such a powerful tool that I think more people should know about and use because just such a good way to gather info for your agents quickly.

**Aakash Gupta** (00:01:08)

One huge takeaway for me from watching you build these is how Really quickly, I think a crazy stat is that more than 50% of you listening are not subscribed. If you can subscribe on YouTube, follow on Apple or Spotify podcasts, my commitment to you is that we'll continue to make this content better and better. And now on to today's episode. A quick note for all you audio listeners, most of this episode was a video demo, but we have edited that video demo so it's still a good listening experience. If you actually wanna go see the video demo, we upload the video to YouTube and Spotify and you can find it there. Otherwise, let's get back into the audio version of how to build multi-agent systems. While we've all been doing vibe coding, Tyler Fisk has gone to the next level to build production AI agents. my guest today tyler fisk is one of the world's most experienced ai agent builders in the world he has taught thousands of students to build ai agents and he has worked with hundreds of businesses to implement ai agents in their workflows he has gone to the next level to productionize these multi-agent workflows he normally charges thousands of dollars for this knowledge today we're giving it all away for free tyler welcome to the podcast

**Tyler Fisk** (00:02:28)

Thank you for having me, Akash. Really excited to be here.

**Aakash Gupta** (00:02:30)

What are we going to do today?

**Tyler Fisk** (00:02:32)

Well, we are going to go from idea to building out a couple of different AI agents. and then see if we can have them all work together and orchestrate and build an AI workflow like real time from scratch.

**Aakash Gupta** (00:02:45)

Do you need a CS degree to build AI agents in production?

**Tyler Fisk** (00:02:49)

No, I don't think so. I don't have one and we've had loads of people come to our class. In fact, there's a running joke that says, we've even had a student say that they couldn't even spell AI. We spotted them two vowels and yet they're building agentic workflows in four weeks. Yeah. No, you don't need a CS degree anymore, I don't think.

**Aakash Gupta** (00:03:08)

Amazing. Can you show us how it's done? Sure.

**Tyler Fisk** (00:03:11)

Yeah.

**Aakash Gupta** (00:03:11)

So

**Tyler Fisk** (00:03:11)

what do

**Aakash Gupta** (00:03:11)

we want to try and build today? I want to see a multi-agentic workflow. Let's work on some popular company like Apple.

**Tyler Fisk** (00:03:19)

Cool. Let's do it. And we will start in... a tool called typing mind and typing mind is essentially like a playground tool, um, for any LLM that we want. And so I can use an agent that I use frequently called gigawatt. And Gigawatt here is an AI prompt engineering and AI engineering agent. And we're going to run this. It's going to be connected to Sonnet for, I've got some MCP tools toggled on here, uh, like X, uh, perplexity, uh, sequential thinking. And then we're going to do some research because that we find that a lot of the work comes when we're doing this for actual clients and like what we teach is that it's this idea of the mentality of an AI practitioner. which happens to be very similar to like the forward deployed engineer mentality. So we need to understand the problem, understand the business, really get to the secret sauce of it.

**Tyler Fisk** (00:04:16)

And from there, we can kind of gather all of our requirements and then start our build.

**Aakash Gupta** (00:04:20)

Awesome.

**Tyler Fisk** (00:04:21)

Okay, so let's see here. What we wanted to try and do this for Apple, I think is what we wanted to do. Yep. Cool. All right. So I joke when I tell people what I do for a living now is I talk funny to robots. So that's what we're going to do here with Gigawatt. So, hey, Gigawatt, what's up? We are on a podcast right now, so no pressure at all. And we're going to do a live agent build here. What we're going to do is we want to build an expert level agent for Apple and that's Apple Computer. So I want you to go out and use your tools, your sequential thinking tool, your deep research tool, perplexity to really think about If we were going to be building an agentic workflow that handles inbound customer service type emails, and we're going to have two different AI agents as a part of this AI team to handle those, one of them is going to be this expert, and that's the one we're going to focus on first.

**Tyler Fisk** (00:05:19)

It's not going to talk to any people. Its whole job is to go and find the best possible information to help support the email agent that we're going to dub you've got mail and then send that response to it. And then it will craft that email out to the customer service or to the customer as a customer service agent to respond to them. So I want you to think on this deeply. Ask me, let's say, three clarifying questions so that you and I are on the same page. We're not in prompt engineering mode yet. This is where you're just going to do brainstorming and we're getting on alignment on what this build is that we're going to do. All right, let's see what you got. Go get them, Slugger. So that's like a funny thing that we always do here at the end. Like people always ask like, why the heck are you saying go get them Slugger?

**Tyler Fisk** (00:06:09)

And the fact that I'm even talking to this agent in this way, like very kind of loosey goosey, and I'm actually just like talking to it. So I'm using Mac whisper on my computer is because the system instructions for gigawatt here are extremely detailed and comprehensive and trained. on how it is that we've done this process for several years now at this point. So we can see it's using its sequential thinking tool here. It's thinking about what it wants to go do. This is very similar to the thinking traces that you get from any of the reasoning models, but we can use this tool with any model now. And it's come back and it's asking us these questions here. So love the energy. Here we go. Apple's product ecosystem is massive. We're talking about iPhone, like the whole shebang. So it wants to know, let's see here, clarifying questions.

**Tyler Fisk** (00:07:01)

Are we doing this to an expert that handles the entire Apple universe or should we focus on a specific subset? Like maybe the hardware support or just customer devices? Are we going full enterprise? Let's just do, let's do all of the main consumer products. So, All right, Gigawatt, I'm going to go through here and answer some of your questions just stream of consciousness dial back to you here. We're going to build this expert agent so that it knows all things Apple products and Apple culture, plus normal information that it would need to know if it were an expert on the Apple team. to try and surface information that would be useful to respond to generalized customer service questions. So this could be everything from, you know, how do I set up family sharing on my devices? How do I update the iPhone? What is even the latest iPhone?

**Tyler Fisk** (00:07:55)

How do I do this thing in iOS? Like all the whole gamut there. So we need to think about this deeply and the kind of information and expertise that we are going to need to gather in to be able to do that here. Okay, so there's that one. The second one, let's see, what kind of customer service scenarios are we optimizing for? Are we talking technical troubleshooting, product information requests, billing account issues, warranty, all of the above? Okay, on your second question, let's just say all of the above, just for speed. Because you never know what kind of customer service questions you're gonna get, especially for a company the size of Apple. So right now, let's solve for all four of those that you mentioned. And let's come down here a little bit more. Our information sources and research step. What level of research capabilities should the expert have?

**Tyler Fisk** (00:08:47)

Should it be pulling from Apple's official documentation? Okay, so great question. So it's wanting to know like basically how is it going to know this info? This is, we're going to build it into the system instructions and we're going to connect it to a RAG retrieval knowledge base. And we're going to connect it to an internet tool so it can go out and actually find this information. Let's help gigawatt that. Hey Gigawatt, so this agent, this expert agent will be connected to a RAG retrieval database where we will scrape in Apple's website. And for the demo, the sake of the demo, it's not gonna be the entire whole website scrape just for the sake of time, but the agent needs to know that it's connected to that and it can go search through its RAG to find anything helpful to answer the questions that the customers are asking.

**Tyler Fisk** (00:09:35)

It's also going to have a lot of the expertise written and built into the system instructions itself. And it's going to be connected to a web search tool. So go out on the open internet to find information as well. With that one though, we need to be careful that when it's going onto the internet, it's looking at Apple specific sites or official information because when it's out on the open web, that could cause hallucinations. So we need to think system instructions, RAG database first, Internet is good to find real-time info, but we need to use kind of chain of verification mentality when it's thinking about that kind of stuff. All right, so let's do that.

**Aakash Gupta** (00:10:18)

And that should get us up and rolling. And while this is running really quickly, if a user wants to replicate this gigawatt infrastructure or this agent, how would they go about doing that? Can they access gigawatt or how would they rebuild it?

**Tyler Fisk** (00:10:30)

Yeah. Well, gigawatt is something that we give versions of it away as a part of going through our course. That's one thing. And the other thing is like we're actually working on turning gigawatt into a real live product. We are vibe coding this right now. Like I've been deep in VS Code with Claude Code and Codex trying to. turn this into a product that i don't have to be there anymore that like this whole back and forth that we're doing now and forcing the research and even deep research happens completely autonomously um so yeah that's that's a couple ways that we're working on it

**Aakash Gupta** (00:11:06)

If somebody didn't take the course or you hadn't released the product yet, how could they replicate something like this to do this on their own?

**Tyler Fisk** (00:11:14)

I mean, the way that I've done it is that everyone kind of has their own best practices around prompt engineering and what good looks like to them. So I have taken a lot of the work that I've done over the last several years where I manually did this. And because I originally built Gigawatt to speed up my own processes, I use what good looks like from my point of view and how I approach it and the different AI research techniques that we use. So you heard me say chain of verification there a minute ago. That's a process that Meta came out with here a few years ago that was produced in a research paper. I'm a nerd, like I love reading that stuff and watching content around it. And when I saw that, I recognized, oh, this is a framework we can start incorporating into agents so that they hallucinate less frequently because it's like reviewing the information, kind of fact checking it, giving a confidence score before it ever decides to include it in an output.

**Tyler Fisk** (00:12:13)

So that's like one example of one piece of research that GigaWatt knows about. So if someone wants to rebuild that, it's kind of collecting like all of these kinds of bits and pieces of information. And then now the LLMs are really good at writing prompts to begin with. So if you could gather that, put it together, you're going to have a pretty good prompt engineering agent just going from there.

**Aakash Gupta** (00:12:38)

okay so the goal is to build a prompt engineering agent in this tool typing mind which gives that agent access to all these tools that you listed off and then you prompt that agent that's your agent builder helper to help create the actual agent you want to

**Tyler Fisk** (00:12:53)

create Yeah, exactly right. It's a version of meta-prompting almost. And you'll see that happen in here frequently as I go through this process. Not only to build Gigawatt, the kind of odd thing that's like inception-y dream within a dream is that I've used older versions of Gigawatt plus my feedback and improvements and new techniques that I've come up with or found out as new research comes out. and then bake that in and Gigawatt can Metaprompt itself and help build a better version of Gigawatt or whatever agent that is that we're trying to build at the time.

**Aakash Gupta** (00:13:33)

It's like turtles on turtles. You got it, yeah.

**Tyler Fisk** (00:13:37)

So let's see here. So let's come back. So Apple expert agent architecture, complete Apple ecosystem, multi-source intelligence here, chain of verification, comprehensive customer service coverage, information hierarchy. So I'm just like speed reading through this just for the sake of time. So it knows that we want to make sure that the RAG database is primary, secondary is when it's thinking about responding. It's working from the built-in system instructions. Tertiary is going to be verified web search with confidence scoring on that. The output structure is going to be for the You've Got Mail agent. That's an important one. Like if we were doing this in production and I won't do it today, I would probably have interagent communication print its output in JSON because It's not the prettiest thing for us to look at, but when you go agent to agent, it's very useful because the LLMs can parse out information from that very easily.

**Tyler Fisk** (00:14:35)

It makes sense for them. And I know I'm like anthropomorphizing them, but it just is what it is. And that technique really works well. So while this is also running in the background, let me come over here and do this just over multitasking here. I'm going to switch over into Cassidy AI. Cassidy AI is a platform that we teach on and that we use frequently. It's a no-code platform and it makes things like web scraping incredibly easy. So let's just go and grab, let's see here, apple.com. grab their website, pop back over here into Cassidy. We're going to chuck this in. I'm just going to do a domain level scrape just for expediency. We're going to do a thousand pages. I'll turn the sync off here and just go save and begin import. And so while we finished building these agents out, this is doing a web scrape on Apple's website.

**Tyler Fisk** (00:15:37)

And so this is what we're going to connect into the rag here in just a moment. The other thing that I would do is this. We're going to use deep research. Hey, Gigawatt, we're going to use deep research and we're going to work with our clear agent, which is another agent that you're familiar with that is an expert in writing deep research prompts. So think about any areas that you think would be extremely valuable either to help further inform you in this build process or to add as assets into a rag retrieval knowledge base. and give me, let's say, three areas of deep research you would like to see done. Be as comprehensive as possible in your response there. And then I'll hand that over to the clear agent so we can start getting those deep research agents up and rolling. Thank you.

**Aakash Gupta** (00:16:27)

If you've been enjoying this breakdown with Tyler on how to build multi-agent systems, you are going to love his Maven course. It is one of the highest growing courses on Maven. And if you use my code, you will get money off. So use my code AkashXMaven. Use the link that's in the show description notes, that's in the email or newsletter that you got about this or in the social media post. Find that link. Go sign up for Tyler's course. He does it with his partner, Sarah. This is one of the highest reviewed courses on Maven. And if you saw it, we weren't able to cover all the details in the episode. So if you want to actually get through building the workflows, deploying the workflows, building the evals. They teach all of that in the course. I highly recommend it. And now back to the episode.

**Tyler Fisk** (00:17:14)

All right, so let's do that. And so now we're going to let Gigawatt write this up. And again, because I'm talking to these things and just using Mac whisper to like transcribe this, and there's lots of tools that do this now, like I can talk so much faster than I can type. So this is getting like from every angle here, the efficiencies that I get in doing this kind of work is just exponential. Now at this point, it's kind of ridiculous. So why this is happening, I'm going to call in my Clear agent. This is another agent that, again, is kind of a prompt engineering agent, but it's more hyper-focused into writing deep research prompts. And that's to go directly to be used on something like Perplexity or Anthropic, ChatGPT, Google, those four primarily. And it will see what it is that Gigawatt wants to see deep research done in, use that to write the deep research prompt in a way that we found that works really well.

**Tyler Fisk** (00:18:12)

And then from there, we'll go let it go do deep research. Now we're spinning up multiple agents here just to kind of get this process done and get all the context that we need as quickly as possible.

<!-- sponsor -->
**Aakash Gupta** (00:18:24)

Today's episode is brought to you by Vanta. As a founder, you're moving fast toward product market fit, your next round, or your first big enterprise deal. But with AI accelerating how quickly startups build and ship, security expectations are higher earlier than ever. Getting security and compliance right can unlock growth or stall it if you wait too long. With deep integrations and automated workflows built for fast-moving teams, Vanta gets you audit-ready fast and keeps you secure with continuous monitoring as your models, infra, and customers evolve. Fast-scoring startups like LinkChain, Writer, and Cursor trusted Vanta to build a scalable foundation from the start. So go to Vanta.com slash Akash. That's V-A-N-T-A dot com slash A-A-K-A-S-H to save $1,000 and join over 10,000 ambitious companies already scaling with Vanta. AI is writing code faster than ever, but can your testing keep up? Testkube is the Kubernetes native platform that scales testing at the pace of AI accelerated development.

**Aakash Gupta** (00:19:26)

One dashboard, all your tools, full oversight. Run functional and load tests in minutes, not hours, across any framework, any environment. No vendor lock-in, no bottlenecks, just confidence that your AI-driven releases are tested, reliable, and ready to ship. Testkube, scale testing for the AI era. See more at testcube.io slash Akash. That's T-E-S-T-K-U-B-E dot I-O slash A-A-K-A-S-H.

**Tyler Fisk** (00:19:56)

All right, so let's see this. So let's go Clear. Hey, Clear, you can read this thread so you're fully up to speed. We're building out a couple of AI agents here, one that's going to be an expert agent and one that is going to be a customer service email agent. Gigawatt has just given you back three different areas of deep research that we would like to see happen. So take them one at a time, focus on them each in a loop, like one right after another, and then write the deep research prompt that we can go out and use on, let's just use perplexity and anthropic for these just to knock it out quickly. So do that and then write those deep research prompts, please. Thank you. All right. And again, like the reason that I'm able to just talk to these agents and it feels like I'm not prompting them that well is because on the back end, if we want to go like peek at this for just a split second, like gigawatt system instructions, like even this version, we can see it.

**Tyler Fisk** (00:21:01)

are are quite extensive like this is a different version of gigawatt this is 3.2 it's one of the earlier versions and it's almost 72 000 characters so it's there's they're extremely extensive in here it's like what we're covering they're written in xml um because i do a lot of my work in anthropic i work with all of the models but specifically i work a lot with clod models and Claude is trained on XML. So you can get it to do some additional functionality by using this. And because we're so organized, detailed on this end, we can be much more kind of like conversational on the front end here. All right. So we've got our first clear agent prompt here. So let's just take that again. We're gonna, it helps being like, I guess neuro spicy to kind of spin these things up quickly. So I'll just use perplexity deep research to start doing that area of research.

**Tyler Fisk** (00:22:00)

Let's come over here and we have prompt number two. We'll go spend that one up in quad just for variety. So let's check that in there research, let her roll, pop back over here into I like this last one. We'll just do another perplexity one just because it's a little bit faster. I

**Aakash Gupta** (00:22:24)

love how many parallel processes you have going here. That's where the speed comes from, and that's how you're going to be able to finish this in a podcast.

**Tyler Fisk** (00:22:34)

Yeah, exactly. And this just comes from repetition of doing this a lot. So let's see here. Gigawatt, 5.1. All right. So now I'm switching the chat like in chat back over to gigawatt and I moved off of the clear agent. So that's kind of the cool thing here is that in typing mind, it's kind of like in chat GPT, how you can call in like different custom GPTs or Gemini gems. I think you can do that too. Um, it's the same thing here, but this is running all on the API layer. So we have much better security, much more control over like system parameters and things like that. And also like MCP tools. So let's go back here to Gigawatt. And all right, Gigawatt, we have got all three deep research agents up and running. So that's gonna take just a second to finish. In the meantime, what I want you to do is think deeply about everything that we've discussed so far.

**Tyler Fisk** (00:23:33)

the set and setting that we are building for here in this AI team. And I want you to give me back a PRD as you understand what it is that we're building specifically for this expert agent. And let's call this agent core, please. Thank you.

**Aakash Gupta** (00:23:53)

Let's go. All the PMs are smiling. There's a PRD in here.

**Tyler Fisk** (00:23:57)

you got

**Aakash Gupta** (00:23:58)

it

**Tyler Fisk** (00:23:58)

yeah yeah so for all the folks that don't know what that is because we we have to explain our tech bro speech frequently uh prd is a product requirements document so this is basically think of it as like a full write-up of uh what are we building who is it for what's this journey look like what is it gonna do what is it not gonna do like all all of these like different um lenses you look at a project through, and by doing that and even training a model on what a good PRD looks like from your point of view, that could even be, and probably should be, its own separate agent. You get a really good alignment to like lay out in the thread here like what's our game plan and then gigawatts going to go build from that this same process works like when you're like after we've done all this work and we're like hey let's go turn this into an actual product or a workflow or whatever that might be um like coming back and getting your plan together first before you ever try and go do the actual work is is paramount here All right.

**Tyler Fisk** (00:25:05)

So let's see, we've got our PRD going. We've got core is going to be our ecosystem expert. And it just so happens, like I may or may not have built an Apple expert agent before in class. And I like I'm a millennial. So like I'm extra on using emojis and like fun names here for these agents and Claude all on its own came up with core. I was like, that's a freaking good name. So like anytime I build an expert, an Apple expert, that's what I'm doing here. So let's see.

**Aakash Gupta** (00:25:40)

Not coordinated folks. He just asked me who to build it for. So many agents that he had already built this. Yeah.

**Tyler Fisk** (00:25:49)

It was either this or a, we were joking about Hattie B's chicken before we got rolling today. I was like, we can build it for that too. Yeah. So let's see, we're gonna build core out here. This is the research and intelligence expert agent. It's given its primary function, who the target user is, which is important here. We want it to remember because the inputs that this agent is gonna get is like, for us, we're gonna come up with a synthetic email that an Apple might receive on the regular. They might get more data points as well as an input. But if you're not very clear and specific on this of who is the, what are the inputs? Who is the intended audience? What are the output requirements? Then this agent will have a kind of role mix up and start trying to actually write an email back to that end user.

**Tyler Fisk** (00:26:44)

And that's

**Aakash Gupta** (00:26:44)

not what

**Tyler Fisk** (00:26:45)

we want at all. So like getting this clarity is extremely important here. And

**Aakash Gupta** (00:26:49)

for people who don't understand, why is it important to have multiple agents and separate these agents in this way?

**Tyler Fisk** (00:26:56)

Yeah, well, in this example, we learn in building customer service email flows and just our own experience. Like I always, for me, it's easy to learn things in stories and to like visualize this. So when we built a version of this out for my family's company called Grower Solution, they sell like gardening supplies and greenhouses. And when they get customer service emails coming in, the people team, There's like different tiers of customer support and like different specializations in there. They have their own internal knowledge bases and things. But then just like in every business, literally every business that we have worked with, they're no exception. There's tribal and tacit knowledge through all different areas of domain expertise. And so their people team have to go and like tap other folks on the team to get the right answers because they might not know. So they might get a question that's really complicated about irrigation or something, and there's a few people on the team that really specialize in that.

**Tyler Fisk** (00:28:02)

So they have to go ask those people the question and then bring it back after they've gone on this fact-finding mission to respond to the customer. And the funny thing about this in real life is that the real-life experts typically are not the same people that you want answering the customer service emails. they don't always like talk in an empathetic way, not that they're like harsh, it's just they're experts and to distill that down in a way that like lands at the level that the customer's trying to talk at, it doesn't always resonate there. So that's like one really clear example of we want our expert to be focused in different areas of domain expertise and then hand that off to an agent that specializes in taking that, translating it and being on brand And like having very separate roles. And from an agent, like a technical point of view also, if you try and have like one more generalized do it all agent, It's more difficult when you get into things like temperature and system parameters and things like that, you might want to have a bit of a higher temperature so that when your email agent writes a response, it's much more like it feels human or feels authentic.

**Tyler Fisk** (00:29:18)

And if you have an expert agent, that temperature might be like much lower, maybe even zero. It's like much more deterministic in its response. And if you had that bundled into one and had that temperature turned down really low, It could come across really rigid. And also if you turn the temperature higher to break that rigidness out of it, then it's going to maybe not follow your instructions quite as closely and can have hallucinations or not do every step that you're asking it to do. So it's like, it's really important to have this like separation. And that's why multi-agent teams and then having them work together is, again, it's like a key thing in this space

**Aakash Gupta** (00:29:59)

that we're seeing. You just packed thousands of dollars of lessons into 60 seconds. So just to reemphasize for folks, you can almost think about it as who would be the different people in a company? As we just analogize, like there's the expert, there's the customer service expert, they have different skills one is really good at the tech one is really good at talking to people you can think about it the same way with agents and with agents technically in particular if you give them too many things to do they're not going to perform as well and so that's why it's important to have build a multi-agent system to actually separate these things out and to use this technical term that some people might not be familiar with in fact i'm not totally 100 sure i understand it temperature can you just explain that a little bit more

**Tyler Fisk** (00:30:42)

Oh yeah, I have a super fun analogy. So I have young kids and we watch a lot of Disney and Pixar movies and stuff. So Toy Story, I've seen it a ton. And if you think about like the claw machine, like the little aliens that are in there and it's like coming down, the claw. Okay. So imagine that we are, temperature is like this icy peak inside of a claw machine. And when the temperature is dialed all the way up, because it's different from model to model, but generally it's on a scale of zero to one or zero to two. And when the temperature is dialed up so that it is like, or I'm sorry, when it's dialed down to zero, you can think like it's cold and this like icy peak is what temperature is like. So when the claw comes down, which is the LLM coming to try and predict what is the next most probable token that needs to come in the response, it's very deterministic.

**Tyler Fisk** (00:31:40)

It's gonna pick off the top of this peak or the pile basically. And when you turn that temperature up to one, that's when like the peak melts down. And so when the claw comes down, it's easier for it to grab from multiple spots off of the peak or off of the pile. And what you're doing when you turn this temperature up or down to like, I'll switch into tech pro here for a minute, is that you're changing the shape of the probability distribution curve. So that means that you dial it up, it's gonna be much more creative. It has more options for tokens that it can pick from. When you take it down to zero or take it down to freezing, it's much more rigid and it's only gonna pick off the peak there. So there's different instances when you would wanna have a temperature up or down.

**Tyler Fisk** (00:32:26)

And how that looks like too, this is one of the ways it was explained to me like early on, is that when temperature equals zero and you say the sky is, and then you leave it blank and have it complete that sentence, it might say the sky is blue, the sky is clear, like something like that. Very like predictable, right? When you take it all the way up to one, it might say the sky is full of fluffy clouds and rainbows or something like extremely creative in that way because it has more tokens to go and choose from, essentially. It's like the randomness is increased there. All right, so let's get our agents working here in the background again. So I'm going to kick up gigawatts. So all right, gigawatts, this is excellent. Now we are ready to kick over into prompt engineering mode. I'm going to vibe code this a little bit.

**Tyler Fisk** (00:33:15)

And for the sake of time, I didn't, I'll admit, I didn't fully read your PRD, but I trust you. So what we're going to do is you're going to draft the V1 version of system instructions in the way that you've been trained. This is going to be in the XML output. You're going to include at least, but definitely not limited to these top, five level XML sections that are going to be role, context, instructions, criteria, and examples. But for the examples section, since this is the first version, I don't want you to do traditional shop prompt examples. Instead, I would rather you get a little bit more meta about it. Think about different scenarios that this agent might encounter. And then what are the steps that it might go through to achieve the intended goal? So it's not just a direct, like here's an input, here's an output type shot prompt example.

**Tyler Fisk** (00:34:11)

Be much more descriptive and let's just give it, let's say two different scenarios in the example section to begin with. All right, take a deep breath, proceed in a step-by-step manner and go get them Slugger. Let's see what you got.

<!-- sponsor -->
**Aakash Gupta** (00:34:25)

Today's episode is brought to you by the experimentation platform Chameleon. 9 out of 10 companies that see themselves as industry leaders and expect to grow this year say experimentation is critical to their business. But most companies still fail at it. Why? Because most experiments require too much developer involvement. Chameleon handles experimentation differently. It enables product and growth teams to create and test prototypes in minutes with prompt based experimentation. You describe what you want. Chameleon builds a variation of your webpage, lets you target a cohort of users, choose KPIs, and runs the experiment for you. Prompt-based experimentation makes what used to take days of developer time turn into minutes. Try prompt-based experimentation on your own web apps. Visit chameleon.com slash prompt to join the waitlist. That's K-A-M-E-L-E-O-O-N dot com slash prompt. Today's episode is brought to you by the AIPM certification on Maven. Run by Mikdad Jaffer, who is a product leader at OpenAI, this is not your typical course.

**Aakash Gupta** (00:35:26)

It's eight weeks of live cohort-based learning with the leader at one of the top companies in tech. As you know by now, the future of PM is AI, and this certificate will give you the learnings, plus the hardware, to show you are ready for an AI PM role. I myself took the course and recommend it. Put on by the amazing team at product faculty, including Mo Ali and Pavel Hearn, it's worth it. Former students come from companies like OpenAI, Shopify, Stripe, Google, and Meta. The best part? Your company can probably cover the cost. So if you want to get $550 off, use my code AKASH550C7. That's A-A-K-A-S-H 550C7. And head to maven.com slash product-faculty. That's M-A-V-E-N.com slash P-R-O-D-U-C-T dash F-A-C-U-L-T-Y.

**Tyler Fisk** (00:36:20)

I'm saying a lot of this stuff here in the user prompt, which is like what we just sent through that is already in the system instructions. But because the system instructions are generally like extremely long, I find that it's like helpful to like re-inform them, like help remind the agent or remind Gigawatt like what I want it to do on certain key things. And then because shop prompts are like, Most of the instructions are telling it how, or what to do, and the instructions around that, but the shop prompts are showing it how to go and do that. And one thing that you'll find that if you include shop prompt examples in there, and they're not really what you want it to be, if it's not a good representation of that, it kind of muddies the whole water, and the outputs you're gonna get are not gonna match your expectations.

**Tyler Fisk** (00:37:11)

It can cause it to mess up, basically. So that's why I have, when I'm first building it, like be much more like meta in that way instead of a direct input and output. And then the, the like ending part here, people, I say, go get them slugger a lot. And it started as a joke. And then it's, I just like do it all the time. That actually comes from AI research though. So there's a technique called emotion prompting. And this is really interesting. Like I've loved like research. So like this was a, you find that in, sociology and psychology, a lot of the information that we see there has led to some of the breakthroughs in LLMs and techniques that you use. So when you gaslight or give like positive reinforcement or negative reinforcement to a person, they will actually do better. And it turns out that that's true in LLMs too.

**Tyler Fisk** (00:38:03)

But we always say like, you know, be positive. These things have pretty good memory now. Probably we're working towards like perfect recall in everything eventually. So like, and they're going to have robot bodies soon. So be nice and friendly to your AI. So I'm always going on like the positive side of like, you know, boost them up a little bit and they will actually do better at the job. It's been proven. So it sounds goofy, but it works. All right here, so gigawatt is going through sequential thinking and you can see like this is spinning up. It has a couple of internal thought traces and then we could even like go in and read what it's doing here. It's like seeing its own inside its head. And then it started to write the system instructions here. All right, cool. So we can see it's got the, I'm scrolling through it quick here.

**Tyler Fisk** (00:38:57)

It's got the role section context. There's even subsections within context here. So the role is basically like the job description for the agent. Context is all the background information and nuances around that of like Where is it working? Who is it working for? Who is it working with? Like all sorts of different kinds of details can go in there. Uh, instructions is the exactly what you might think, like a step-by-step instructions. You want the agent to follow each time it does its job. Criteria, once we get down here to that, and it wrote in and out of a code block, which is okay. Criteria down here, these are kind of like the guard rails that you're going to put around it. These can both be like do's and do not's. So like do not use emojis in your output or always have an empathetic tone when you print an output.

**Tyler Fisk** (00:39:49)

You can make these up, whatever you want these rules to be. And then the example section down here is the shot prompt examples. So when I do this, Gigawatt's pretty good. It's going to probably have a set, I would say like a B set of instructions right now if you're going to grade it. And like, that's okay. But I have like figured out that by using this process called meta prompting, which this is like a prompt I have stored right here, is that It basically that you're having Gigawatt review its own work, go section by section, give it a quantitative score and qualitative reasoning around that, and give, if they exist, give suggested areas of improvement. And then another thing I have it doing this as well is I give it these ideas of different techniques and frameworks that I use, such as like Meta prompting, step back prompting, AI agent self review, chain of thought, chain of density, like just a few different things to give gigawatt inspiration.

**Tyler Fisk** (00:40:52)

And because it's connected to perplexity and EXA, it can go out on the internet and think about, hey, what kind of agent am I building? What are the latest breakthroughs in AI? I can go and research that. What if that makes sense to incorporate into this agent? And it will come back here in a minute with those suggestions. So you can see it's done multiple perplexity searches here. It might decide to go use EXA. It might think about what it found in a search before it ever responds back to us. But this process, it basically is like, we've got this set of B instructions. After the evaluation, we're going to have it do it again. And we generally go to like an A, A minus territory. And that's generally good enough for us to start, let's go take it and start testing it and doing what we call observational evals on it.

**Tyler Fisk** (00:41:42)

Like, go see if this thing's any good and working like we hope it will. All right.

**Aakash Gupta** (00:41:48)

Love this. And you mentioned the phrase shot prompting. If people don't know that, I believe that's when you're giving various examples within the prompt itself, correct? That's right,

**Tyler Fisk** (00:42:01)

yeah. Yeah, that's exactly it. So this could be, let's come up here and look and see what even Gigawatt wrote. So here's one of the examples it came up with. The scenario is product information research with evolving information. I'm trying to decide between the iPhone Pro and the iPhone 17 Air because we all need a thinner iPhone. So what's the main differences in which one would be better for photography? I heard there might be some new camera features, but I'm not sure what's current.

**Aakash Gupta** (00:42:33)

I actually have this question. So I love how it was able to pick something that people would really ask.

**Tyler Fisk** (00:42:40)

Yeah, like really ask. And then like, it's current too, because it went out in real time to find like, what's the latest, you know, kind of stuff here. And so like the example is showing it, what should core go do? It's saying that do the initial analysis, go research the rack database, think about your own system knowledge. go out on the internet and research and use chain of verification for that, like synthesize and generate your output and then give that to the next agent. So it's like walking it through, like we've told you what you should do in the, in the system instructions, but this is showing you like, how do you actually go walk that out in a practical way? Yeah, cool. So gigawatts still thinking here while it's doing that, let's go check on deep research. Sweet. So this one is done. I'm going to grab this and export this just as a document really quickly.

**Tyler Fisk** (00:43:37)

Cool. There's one. Claude is like, it's one of my favorite deep research tools because it looks at so many sources. It will literally go look at thousands of websites to do this work. which is like, I would, we would never have time to go do that, especially in this sort of time. But for some reason it's like goofing up right here right now. I think it's because of, it's trying to call additional like tools I have connected to it, like Canva and stuff. And I don't want it to do that right now. So let's see, give it one more shot here. I

**Aakash Gupta** (00:44:10)

haven't actually seen these connectors and I'm a pretty heavy cloud user. What are those?

**Tyler Fisk** (00:44:17)

It's basically like they've made it easier to kind of connect in MCPs. So if you come over here to, I think you have to do it on Claw Desktop initially. I could totally be wrong on this. But if you come over here and you go to your settings, I think is where you're doing it at initially. right here connectors is like where you can come in and either set up your own custom ones that are, you know, basically like MCP tools, or they've made it easier with, uh, some like out of the box ones. Um, that's awesome. Yeah. I think it's just like, and an MCP is like for people that don't know is model context protocol. That is, um, Before this came out, it's like a framework that they've used. When people would need to go and use a tool, like if you wanted to connect an agent to Gmail, let's say, you'd have to do all these different API calls.

**Tyler Fisk** (00:45:16)

And that's very scary. Most people aren't going to do that. But because we know that context, like bringing relevant information back to an agent is so powerful, having these tools is part of what makes an agent an agent. And so Anthropic, who makes Claude, came up with MCPs, and they've really simplified that process and maybe even democratized it is a better word so that more people can connect more tools to their agents. And it just makes them so much more useful. Let's see. Yeah. All right. So it's finally kicked off its research. We'll let that one finish. Perplexity did its other research. So it looked, this one looked at 119 different websites and sources to pull this info in. I'm gonna export that as a doc as well. And again, I'm like, we're having to scatter around here. This is the import over here in Cassidy.

**Tyler Fisk** (00:46:12)

And it pulled in, it had a few pages that aired out. Let me click that. We'll let it retry them just in case while we have time. And now if we come back out here to my main file, like here's the website. It's pulled in this many pages already. And if we go add, I'm just gonna make a new folder to check all this stuff into one spot. Apple knowledge, save it. Let's pull this into here. And then now I can also add those deep research documents that we just did with perplexity to throw them into this RAG database or like you could think of this as an AI second brain system essentially. So now all of that's going to live in its head. So that's uploading. Here we go. So now back over here in typing mind and I'm like, I'm jumping around. So I'm trying to make sure we've make this easy for folks to follow along is gigawatt uh just finished up its self-review where it was evaluating its work and saying what it did well and where it could do better and sort of section by section analysis here um you can see like it's it's pretty we don't want it to be biased or have an ego towards its own work and it even kind of says that in the prompt that we gave it saying that Our whole goal is that we make the best possible agent for this specific role.

**Tyler Fisk** (00:47:35)

And it's giving itself a 78 out of 100. It's giving its like reasoning as to why it gave it that grade and then how it could improve it. 82 here. So it's like, as you can see, like we're doing okay, but we're like C territory even right now. So we need to get that grade up for sure. We're A students around here. And let's see, so overall we got a 77 out of 100. So we've got some big gaps that we need to fill. And it's giving basically itself its own instructions on how we could do this better. And so now what I'm gonna do is I have another prompt that is, let's see here, right, the improved version. Let's adjust this. So here we go. This

**Aakash Gupta** (00:48:21)

is where- I love this use of saved

**Tyler Fisk** (00:48:23)

prompts. This

**Aakash Gupta** (00:48:24)

is

**Tyler Fisk** (00:48:24)

huge. Speeds it up. Yeah, like it takes a while to get them like dialed in, you know, like the way that you want them, but once you have them done, like pulling them in from a prompt library is key. Let's see. So today is, what is today? The 24th of September. So I'm putting this in because now it's going to write in some metadata into like the head tag area of the system instructions and even incorporate a change log in there. So let's go ahead and do this. It's basically telling it write the complete new updated set of system instructions. This should be additive and not reductive because if you just let it go out and do its thing, then it might like wholesale rewrite the system instructions. Uh, instead it's like, you've already got a good foundation, like use what you recognize about what was working and what wasn't and go improve upon that without like just completely changing everything.

**Tyler Fisk** (00:49:21)

And that's what we're seeing here. All right. And it's also telling it too, because this happens or can happen is that, um, if you happen to cut off before you complete writing this set of system instructions, like know that I'll have you like pick up, uh, in a followup message. And I tell it that ahead of time, because if you don't, then the model, um, can kind of try and like write to optimize for its its context output window to an extent like it'll try and make it more concise and i don't want that like i want it to be um extremely descriptive in here as you can see uh like these generally like once you do this next lap or this next version the the system instructions kind of balloon up in size and it's not to write them longer for the sake of writing them longer It's because this is like very key information that we want to make sure that this agent gets like every time it goes to do a task.

**Tyler Fisk** (00:50:26)

And that's why we're, we're like taking extra care in the system instructions. So, all right, cool. So while this is happening again, I'm going to come over here and let's do a, um, get this ready to put this agent into production. So I'm going to call this like core, We'll call it the podcast edition. And we're back in Cassidy. Yeah, back in Cassidy. Yes, thank you. Do you have a preference? I'll let you choose. Honestly, it doesn't matter. I would suggest probably choosing one of the Ferrari models, but... do you want to run this on do you want to do it like gpt5 or we have any of the clod models or even

**Aakash Gupta** (00:51:08)

maybe just tell us a little bit more about how you would think through the choice and model choice i feel like everyone's always asking me about that yeah

**Tyler Fisk** (00:51:14)

yeah uh same like i think that a lot of it comes down to like personal preference and taste it's it's literally are you like an apple or a pc person uh just to some extent and then there's also like really clear reasons when you might choose one model over another. All of the leading models from pretty much all of the big providers are at a point right now that they're extremely good at pretty much most tasks that most people are going to have them do. So the good news is that like Like we're rich with intelligence now. Um,

**Aakash Gupta** (00:51:54)

yeah.

**Tyler Fisk** (00:51:55)

So like picking GPT five versus like Sonnet or, or, um, or Opus or even Gemini pro like the new pro, um, I mean, you could argue that you could really switch them out. And that's even what we teach is that you want to be somewhat model agnostic because when you get into production, you know, if Anthropic has a new release and their API is running a bit glitchy, but you have agents in production, like glitchiness is not acceptable. We need to be able to pull the plug on it running on an Anthropic model and plug it into Anthropic. uh, GPT five or whatever it is so that we're not losing anything. There's redundancy there. Um, but it could be things like speed. Speed is a big deal. Uh, if you need reasoning, uh, like for a model to like think through something using one of the reasoning models is a big deal.

**Tyler Fisk** (00:52:49)

If latency matters using something like a mini, a nano, a haiku, those are, those are faster and cheaper, but not capable necessarily. Um, Yeah, and then like context window is the other thing. This is like the amount of short-term memory that an agent has, like how much space can it hold in its head. And a million and two million is like Google was kind of the first one to go into that territory. Anthropic's at a million now with Claude Sonnet. GPT-5 is still at like 400K. I suspect they're going to be at a million or maybe further than that like soon. So let's just go, for now, let's go GPT-5 and we'll go high thinking. Let's just make it really good here. I've got the tokens. So this is the context window. I'm turning this all the way up so it can have the most information possible.

**Tyler Fisk** (00:53:43)

I'm going to go ahead and toggle this on. This basically is turning on the RAG knowledge base. So it's the data that we've been populating in here. And

**Aakash Gupta** (00:53:53)

I'm

**Tyler Fisk** (00:53:53)

going to select this folder. So everything we chuck in that folder, it will have access to. And because I'm saying always search, it's like forcing the agent to go look into that folder every time to see if there's anything that will help it. Maybe it does, maybe it doesn't, but we're making it go look there. And then let me save this. And the last tool or two tools I'm gonna turn on here are gonna be data analysis and web search. Data analysis allows it to use like Python. It's like code interpreter basically. And web search is allowing it to go out on the internet and research things. So I'm gonna give it those tools as well. And let's go see, I think gigawatt finished over here. I heard the easy bake oven timer go off. Let's see. Yeah. There we go. All right. Yeah. So I finished the whole thing.

**Tyler Fisk** (00:54:47)

So I'm going to grab this whole set of instructions, go back into Cassidy now and actually put it into production. and let me go to the very bottom because it had some notation here at the bottom that aren't a part of it isn't a part of the instructions i'm just going to delete that out yeah and i think that we have that clean xml instruction yep you got it so it's got the tags in there exactly like we want it's using it per the way that i've like trained it to do this uh it's got the new and upgraded enhanced version of the system instructions in here and we're at 7,000 tokens right now. Actually less than that because let me delete this off the other like commentary here at the beginning. So approximately like 7,000 tokens for just the system instructions. Not bad. Let's see.

**Tyler Fisk** (00:55:38)

So now we can go ahead and open this one in chat and let's test it out. So like what was, you said, what was the question you wanted to ask it? In fact, I'll just, I'll hold down my key and you just talk and it'll transcribe it into it.

**Aakash Gupta** (00:55:54)

Um, should I get a iPad or iPhone air or iPhone pro? I'm trying to weigh battery and photo quality.

**Tyler Fisk** (00:56:06)

Love it. The battery is the thing I want to know about. I watched their like keynote address or whatever. And I'm like, I don't know. They were pushing that, that add on battery pretty hard right out of the gate. So we'll see. It looks cool though.

**Aakash Gupta** (00:56:20)

Exactly. It looks so cool, but I'm worried that it won't have a good battery life. So let's see if the agent can help us address that.

**Tyler Fisk** (00:56:27)

Yeah,

**Aakash Gupta** (00:56:27)

for

**Tyler Fisk** (00:56:27)

sure. So it's going to go through here and look at this. And while this is happening, we're going to go do one more thing here. I'm going to go grab... Let me come over here. Where is it at? I think I jumped off of it. Here it is, this one. I'm grabbing example system instructions of another You've Got Mail agent. And this is our customer service agent. So we built the expert. Now we're gonna really quickly build an email agent. And examples are everything. So when I can come back over here into typing on in that exact same thread and tell it that like here are some system instructions for a completely different email agent to use as like inspiration and what good could look like. Knowing how we're going to be using it here, draft the V1 version of the Apple email agent and come up with a fun name for it kind of thing.

**Tyler Fisk** (00:57:23)

All right, Gigawatt, this is awesome. We have the core agent deployed in Cassidy, and we're testing that out right now. I've now given you an attached copy of system instructions for a different You've Got Mail agent, which is our customer service email agent. But this one is made for Hattie B's. It's a hot chicken joint in Nashville. So look at this for inspiration on what a good customer service email agent looks like. Think on this deeply and think about What would you need to change and update and embody so that it sounds on point and matching the culture, the vibe, the brand tone and voice for Apple? You're also going to need to come up with a fun name to go along with the core agent for this. You've got mail agent for Apple. It should be like a one or two name that feels very on brand and authentic to what it's going to be doing here.

**Tyler Fisk** (00:58:23)

So don't do any prompt engineering yet. Review all this, reflect on it, and then come back to me and let me know where you land on it. This is not brainstorming and alignment phase again, just with this new agent. Okay, so we're going to let Gigawatt again work in the background. And let's pop back over here to, let's see here, our iPhone question. Awesome. Well, this is not going to be very pretty for us to look at, so I'll have it legit here in a minute because it returned it in JSON, like what I mentioned earlier. Which is what we wanted. Yes, exactly what we wanted. That's what we want it to do interagent communication. It's good. But now I'm just going to be like, hey, Cor, we're running evals on you right now, and you did perfect. You output your work into a JSON. But we're reviewing this.

**Tyler Fisk** (00:59:14)

Can you convert this into Markdown so it's much prettier for us to come in, read it and review it and see how it looks? OK, so we're just going to let it go through and like recreate this for us in a way that's easier to look at. And down here we can see, this is like what's powerful about using a RAG system or even having, even if it researches on the internet, it cites its sources. So if we ever wanted to come back in here when we're doing evals to see where the heck did it even get this information or arrive at this outcome, we can fact check it in this way by like, it's citing this website that it found. or what came out of the knowledge base that it went and read that documentation internally, like whatever it might be. All right. There was the oven again.

**Tyler Fisk** (01:00:05)

So let's come back over here and type in mind again. Sage. I don't like Sage. This is like a generic. Yeah. We can do better than that. All right. So let's see. Hattie B's agent is good. Masterclass. Yeah. Cool. I think Giggle, it's like gaslighting me here. Let's see, Sage, one word. Okay, so clean, apple aesthetic, like a genius bar expert, natural, organic, loves nature metaphors. I don't know about that, but sophisticated and approachable. Okay. So like, we're just going to kind of, again, for the sake of time, rock with this to some extent, because you can see Hattie B's, it has sophisticated simplicity versus playful irreverence. Hattie B's brand voice, they're Southern. So they say like y'all and use like these really kind of funny chicken puns. Instead, like Apple's going to be, you know, we need to take that idea and translate it for them.

**Tyler Fisk** (01:01:06)

Yeah. If we were doing this for real, we have a whole process to do brand voice and communication analysis. And we even have like workflows for that. Um, but we're just going to do this quickly now, um, and just roll with it. So, all right, Gigawatt, this looks awesome. Now that we have an idea, I think, first of all, Sage, no, let's not do that. That's not a good name. Think more Apple, Apple branding, the way that they do it, something that feels on point for an email agent in that space. Again, it's a one word name, like look at core as an example, core is an excellent name for being on brand for Apple. Think of that for this set and setting as well. With that in mind, use sequential thinking, use your EXA tool to research anything else that you feel that you need to, whether it's like brand guides, brand voice styles out on the internet, and then come back and draft the V1 set of system instructions.

**Tyler Fisk** (01:02:02)

Again, remember to print them in XML. Use the role, context, instructions, criteria, and examples. Do the same sort of shop prompt examples that I had you do with the previous expert agent where it's much more meta. Let's do two different scenarios there. So it's not the traditional, here's an input, here's an output. It's like walking through what it should be doing and showing it that through that scenario. And with all of that in mind, that's a laundry list of tasks, work through them one by one, take a deep breath, and show us why you're a savant at Prompt Engineering. Go get them, Slugger. All right, let's see what we get here. So that one's gonna be working. Now let's go back to Cassidy. And like language matters too. I use that phrase savant. I use that frequently when I'm prompt engineering because, you know, they're large language models and the words that you choose have power and meaning and shape the quality of the agent build that you're doing.

**Tyler Fisk** (01:03:08)

So you want to be thoughtful when you're doing that as well. So let's come up here. So it's saying decision guide, iPhone air versus iPhone 17. Here's the summary. If photography is your top priority, iPhone 17 Pro is it because it's got that new, it's got the Pro Fusion plus the ultra-wide telephoto and the optical zoom built in. It's got 39 hours of video playback, thinnest phone with a strong main camera, 48 megapixel main camera, no ultra-wide telephoto up to 27 hours. So it's retrieved all this information. Put it into a pretty good breakdown here. I don't know. Is this helping

**Aakash Gupta** (01:03:49)

your decision-making process yet? We'll see what. Yeah, definitely. I mean, I'm seeing, okay, 27 hours video play. Maybe the iPad or the iPhone air is good enough for my battery needs. Similar megapixels. I already own three fancy cameras for the other stuff. So yeah, this is awesome.

**Tyler Fisk** (01:04:07)

Yeah. Sweet. Okay. So now we're. We can see all of this, like it's looking good. And ultimately like what we really wanted to see was this JSON response up here. So I'm gonna go ahead and go ahead and queue up some messages. So let's go eval and improve. I'm gonna queue that. And then I'm gonna go write the improved version. Let's see here. take this off so i can have these messages like pending so it can continue working more in the background for us here oh wow i've never done that that's super cool yeah it's like it's helpful for speed for sure um 9 24

**Aakash Gupta** (01:04:57)

25

**Tyler Fisk** (01:04:52)

let's cue that up again cool so those are just like waiting in the wings

**Aakash Gupta** (01:04:57)

and Wow. That would save me so much time just queuing things. That's great.

**Tyler Fisk** (01:05:03)

Yeah. It's little, little wins in this stuff that you just kind of figure out, um, Here we go. So like here is that, that Claude research finally finished. So it did 394 sources, which is actually kind of low for it. It normally is going up above a thousand in general now, but it took 10 minutes to finish that research. Deep research is such a powerful tool that I think more people should know about and use because Yeah, it's just such a good way to gather info that is valuable, not only like in the build, but to curate info for your knowledge base, like for your second brain, either for yourself or for your agents quickly. It's so amazing. All right, so I've got that in here now.

**Aakash Gupta** (01:05:57)

Hypothetical question. Let's say you're building a RAG database here and you have a bunch of not searchable information, but let's say you have like two gigabytes of enterprise documents. How would you build that in this case?

**Tyler Fisk** (01:06:14)

Yeah, that's a whole, a whole, like, it depends kind of decision tree. Um, because like you can use something like unstructured dot IO is like a platform that can go through and, what's called like vectorize and turn the documents into embeddings and like chunks that are stored in a vector database. Um, and especially with things like PDFs or documents that might have things in it that are also not text, that might be visual. This is where like for that specifically, something like Gemini flash is really good at that. It's, it's extremely inexpensive to basically do OCR now and not only extract the text that's on the page and put it into a format that's better to then go and like turn it into the vector store. but it can look at the visuals and you can have a flow set up where it actually extracts and describes that and turns it into the vector store data as well.

**Tyler Fisk** (01:07:16)

So it's actually searchable. The thing though, like RAG is extremely powerful and potent, but there's also limitations to it. Things can change and update. Like a really easy example is that in our classes, when we first started teaching our early cohorts, they were on certain days of the week and certain times of the day, like all that kind of stuff. And we have an agent that lives in Slack in our community called The Professor. And so students can go and ask it a question and say like, Hey, I don't, I don't have my calendar in front of me. Like when's the next foundations class? I'm in cohort 12, like whatever it is. And it would go and look into the rag system. But because we're like adding all of this information and we're not going to take the time to go in and like clean out all this historical data because we're that would take forever.

**Tyler Fisk** (01:08:09)

And it's just, it's not a job you want to go do. Um, it, the professor might not bring back the best information because the more you add into a rag system, it's powerful, but it can also kind of degrade, uh, the retrieval of it, like the quality of the retrieval, because, um, there's just so much information for it to be looking through. And so the, the way that we're thinking about trying to solve that more is not only the structure that you put into your rag and having like We've been working on this concept called the Cairns method. It's like a three kind of tier system in there. And even more so now, it's a Gentic RAG. So it's not just connecting it to a database like this, a RAG database. It's connecting it to GraphRAG, which holds much more like relational information in there. And it updates it as well.

**Tyler Fisk** (01:08:59)

So that could be like... graph rag, graffiti, things like that. So it would go in and keep up to date in that other data store that, hey, cohort 12 is now on Mondays and Fridays from this time to this time. And so the agents connected to both of those data stores. And also even like MCPs are another tool that you connect for this. So it gives it more information and like ways of connecting the dots in that information so that it gets a better quality response outside of just rag itself. So yeah. Amazing.

**Aakash Gupta** (01:09:37)

So much value in that one response.

**Tyler Fisk** (01:09:39)

Yeah. No worries. All right. Gigawatts still working. Um, even if we tell it to type like the wind, it'll try. So what's happened like coming back over here into, um, typing mind here, It has thought through what I had to go out and write the V1 instructions. It used EXA, which is like an agentic web search tool. So it did research more on brand voice guidelines and customer service communication examples, like this kind of stuff. So it's going to find like real world shop prompt examples, bringing it back, writing the V1 version. It's probably going to be okay, but not great. And then... If we, let's see, it started its next process now of it's like reviewing this and let's see what we got here. It's got an 82, 85. So we're a little bit better. We're not scoring in the seventies here. We're up in the eighties at least.

**Tyler Fisk** (01:10:41)

Well, there's a couple of seventies we can do better and coming down here at the very end. Let's see. And it's also doing that research into other areas. like frameworks or techniques that it could be using for this specific agent. Um,

**Aakash Gupta** (01:10:57)

one of them is like. Huge takeaway for me from watching you build these is how much care you're putting into the system prompt. You know, you had an amazing system prompt to begin with. You had an amazing agent creating it, but you're having that agent review its own work and iterate. And most people probably skip that step.

**Tyler Fisk** (01:11:16)

Yeah, I would say so. Um, like sorry, and I dub it as like the founders level of service. And for me, what that means is, you know, when you first start a business and you're like, you're just, it's just you or like you and a co-founder or whatever that is, you're doing everything and you're putting your heart and soul into it. Cause it's like, it's your baby, right? So it's that level of care that we try and put into pretty much everything that we do. And even when we're doing this for clients, like outside of class, Uh, our whole discovery process, which that's a whole nother topic we could talk about is very intensive so that we can temporarily become experts in their business and in their culture and feel like we're like plugged into their team. So that we can then come take that knowledge and come over here and work with gigawatt to do this for them, like in real time.

**Tyler Fisk** (01:12:09)

And I think that's the skillset more people need to learn. That's it's incredibly important. That's how I think you build a system that works versus one that. is uninformed and not aligned with like what your, your intentions or your client's intentions are. And this, like all of these little steps matter. So yeah, our community has dubbed this weaponized OCD as well. So yeah, let's see here. So we've got a, it went with echo. Okay. Echo is not terrible. I'm not going to like razz giggle on its naming convention. It could do better, but, So we've got Echo is what it's dubbed the customer service email. You can see it's got version information in here, a quick change log, and then it's printed out the whole new version of system instructions. Let's just skip to the end and see if it's, nope, still writing. So while it's doing this, let me come up here and I'm gonna grab, just like, let's go Echo V2, copy, we're gonna pop back over here into, Let's just go here.

**Tyler Fisk** (01:13:18)

So let's go assistance, create a new one. We'll go ahead and get this ready for it to.

**Aakash Gupta** (01:13:24)

Yep. The placeholder for a new agent.

**Tyler Fisk** (01:13:26)

You got it. Yep. So this is going to be Apple customer service demo. And for this one, let's see, we did GPT five high thinking. So let's be multi-model here. Let's either go Anthropic or Gemini. Like, honestly, I could go either way. Do you have a preference you want to see happen here?

**Aakash Gupta** (01:13:47)

We've been doing a lot of Anthropic, so let's try Gemini. Let's give them some shine. Let's do it. I love it. So here's

**Tyler Fisk** (01:13:53)

Gemini 2.5. Yeah, all these models are so good. We are blessed with choices now. The Flash model and the Pro model are so good. Flash is kind of like this weird kind of in-between model. It's not quite like the front runner, and it's not as, I don't want to say like low quality because it makes it sound like it's bad, but not as... Um, the tier that mini and like haiku are at, it's like kind of in between those two, in my opinion. Um, okay. So here we go.

**Aakash Gupta** (01:14:25)

And if you're productionizing, it's like crazy cheap.

**Tyler Fisk** (01:14:28)

Yeah. Oh my God. People should go and look into how much it costs to process documents, like what I said. Basically do what you would pay for OCR, but now you can use Flash for that even. Holy smokes, it's so much cheaper. It's like literally, I've done the math on it. It was like hundreds or thousands of pages for, we're talking about like a dollar or something. It's crazy cheap.

**Aakash Gupta** (01:14:53)

Crazy.

**Tyler Fisk** (01:14:54)

Yeah, let's see here. So save this. Let's give it tools here. What is not saving? Why is it not saving? Oh, it cleared the instructions. Okay. I'm just going to put something in here. We'll update that in a second. Yeah, we'll give it its brain here in a minute. So I'm going to connect those here as well. Save it. And Gigawatt, you done yet? All right. Cut off. All right, here we go. So here we go. All right. You, why am I typing? You were cut off. Please pick up where you stopped and continue on to complete the system instructions. Thank you. It's pretty close. So it's in the criteria section. This is what I was saying. Like a lot of the time, um, the system instructions can kind of bloat up a little bit and that's not, that's not a bad thing. Um, depending on like, we'll, we'll know for sure when we test it.

**Tyler Fisk** (01:15:53)

Right. But I find that, um, the more detailed, the richness that you put into this process, the better the outcome that you're going

**Aakash Gupta** (01:16:02)

to get. So people are worried about like context rot as you add more tokens, but your practical experience just go longer.

**Tyler Fisk** (01:16:12)

Yes. And there's like Tina, good Lord. Yes. And there's like techniques to help with that of, um, like reminding it, like when you, if we were going to go put this into a workflow and there are, and we're writing the user prompts for different stages of this workflow and we can even go like see what something like that looks like while we're waiting on this to cook. uh, we would remind it in the user prompt of like the key things we wanted to remember, uh, just kind of like how you might even refresh a person's memory. Cause we've given it so much detail. It's not that it's hallucinating or dropping context is that there's so much context in there. We need to kind of steer it to like, what are the most important key things that always needs to keep in mind. And you can do that on the user prompt side of things.

**Tyler Fisk** (01:17:00)

So, um, Yeah. Let's go look and see if this is done and we'll connect it still running. All right. So while that's running, do you want to go take a look and see like what one of these systems could look like once we get past the agent creation, we actually go put it into a workflow. That'd be good. Like here. Or I think we're almost there with this one.

**Aakash Gupta** (01:17:23)

Oh yeah, it

**Tyler Fisk** (01:17:23)

is. Okay. Yeah, there we go. It just finished gigawatt finished up. You never know. Sometimes we're having to fill a time with it. So here we go. Echo. I'm going to give myself some space here so I can see where it cut off. Let me come back up here. Escalation triggers right here is where it is. I'm going to delete this out. Hit save. All right, cool. So now we've appended the two different sections here. This one ended up coming in at 8,900 tokens. So again, very modest. It's not going to cost a ton of money to use this. And they're not so long that you really are in the range of needing to worry about context rot, like you said. Not yet. I think that once you get deeper into a chat, maybe that would matter, but I don't think here. Let's go ahead and we're just going to leave your message in here from before.

**Tyler Fisk** (01:18:24)

I'm going to leave this response back from JSON. And I'm going to come in here and see if I can just edit this and switch agents and change the prompt here. So let's do this. Let's switch this over to core the email agent. Or no, it was Echo. I'm sorry. Echo is the name of it. Here's Echo, and let's tell it, hey Echo, I want you to review the work that Core just did, think on it deeply, and then generate the response back to the end user, please. Thank you. Okay, so let's save this. There we go. And so now we're like manually testing this and doing what we call observational evals. This is where we're actually just coming and testing this thing, recognizing in production, And what we would really do is we would test this through a bunch of different potential scenarios and inputs and things like that to see how these two react together before we go put them into a workflow.

**Tyler Fisk** (01:19:34)

Because we need to see if we need to make some changes here first before we move on. We had that response on the question. Echo has looked through this. This is what I was talking about with the XML tags. So Anthropics CLAWD models are actually trained on XML. And so if you use certain tags like Think, Answer, and Scratchpad, just as an example, it forces the model to do certain things at different instances. We're running this on Gemini 2.5, and so any of the new models from OpenAI or Google, they aren't trained on XML, but they now have been trained in their building that Anthropic can do that, and it essentially kind of knows what I'm expecting it to do here, and it's trying to emulate that. So it's not... The function of how it's doing it is different, like here in this thinking tag, but it's trying to do a very similar thing.

**Tyler Fisk** (01:20:38)

So it's thinking through, basically, given this scenario, what do I need to do to answer this? It's then, like reasoning on that, it will then switch into scratch pad mode, which is what it's done here. Scratchpad is where it's like essentially like writing a first draft. So this is like a meta prompting right in line right here. Like I'm thinking about what the information I have. Who am I talking to? What's the info that I found in my knowledge store or that my expert agent gave me? Given all that, like just like a person would like jot down notes or do a first draft of it. Then think about revising that, which is done here. then go out and write the complete and total finalized answer, which is what it should do down here at the bottom somewhere. And it's wrapped it in an answer tag.

**Tyler Fisk** (01:21:28)

The reason we're also using these tags in the output is because we can parse that out when we go put that into production. So we don't want the end user to see all this crap, but if we wanted to parse out the subject and map that to a subject line, parse out the actual email body and map that back to wherever we want that to land, Because we have it in these little containers, it makes that easier to do. So let's see what this sounds like coming back. We don't have a lot of information. This is like a pretty short email message in. So hey there, that's an excellent question. Choosing between these powerful devices is all about finding the perfect partner for your creative life. And it's great that you're focusing on the photo quality and battery life. Let's break this down so you can feel confident in your choice.

**Tyler Fisk** (01:22:10)

For the photographer, uncompromising quality versus beautiful simplicity. When it comes to photography, your best camera is the one you have with you. Here's how these devices empower your creativity differently. And it's going to explain that here. For all the power, it's like walking through that. It feels like on brand as best as we could get it quickly for Apple. This is where we are going to recognize like This is a choice for the Apple team. Would we write an email like this? Because if we were working with a client, this is like a client feedback checkpoint where we want them to review this with us and say, what do you like about this? How might you have done this differently? Does this feel authentically like you all and the brand that you're wanting to represent? These kinds of questions and that feedback that they give us, we directly incorporate into the next iteration of this thing.

**Tyler Fisk** (01:23:09)

so that we're further honing it in on what they think is good, based off of their criteria. And that's also helping us gauge when we set up evals, what are the most important things for them for these particular tasks that we need to be reviewing when we go into full systematic evals in production as well. So, I mean, this thing printed for days here, and it did a pretty... solid job just in the email itself, I would say. And even if we wanted to come in and critique this, like maybe the team at Apple's like, you know, we really wouldn't use bullet points in an email response. Let's just say it's that. And we would make this like much more conversational, It's also more verbose than what we want it to be. We would write it in a more concise manner. These are all data points that we can then come back in and make adjustments on to dial us in further.

**Tyler Fisk** (01:24:08)

But really quickly and under, what has it been now, an hour, hour and a half, we've been able to build two agents that after some testing here, we could... put them into a workflow and connect them to their tech stack and then have them into a production type environment very quickly.

**Aakash Gupta** (01:24:28)

So what would that look like if we were to start to go on that path?

**Tyler Fisk** (01:24:32)

Yeah. Well, there's like several steps, but the no code tool like Cassidy makes it pretty simple for that. An example of this, and there's, there's a lot of this comes in like taste as well of the, what would the Apple team, how would they want to interact with this? The first thing I would say is we would never put it into production without some sort of a human in the loop checkpoint. That's, that's very irresponsible. And in like actually in live production, you have no idea the types of inputs that you might get in a system. Uh, like someone might say something, um, that Apple doesn't want to respond to or, uh, There could be a myriad of different things. And so it's very important to have an intentional human in the loop checkpoint put in place somewhere. And you can begin to, once you have it in production, add more autonomy into the system where you then like know for these certain use cases, we can kind of auto send it.

**Tyler Fisk** (01:25:33)

And if not, it still needs a human to review it before we send it on its way, but it speeds it up and can do them in batches. So here, this is a workflow in Cassidy that is also an email workflow. And what's happening is we set this up to work with Slack as well, because this was like our intended, that's where we wanted to work with our email agent at. And so what happens is we would connect this upstream with something like like you can even do it now natively in Cassidy too, but before you couldn't. So we would use something like Zapier or Make or something that when a new email comes in and if you're like, for instance, using Google and it's tagged a certain way, then it would then trigger this workflow to start running. And we would get their message, their name, the date of the email, the subject, and the Gmail thread ID, which is important to be able to route it back to the correct thread.

**Tyler Fisk** (01:26:28)

And then this first block here is an agent called Cinnamon. It's a sentiment analysis agent. The funny story on that name is that I'm a Big Bang, like TV show theory, and Raj's dog on that show's name is Cinnamon. And every time he calls to it, he's like, Cinnamon! And whenever I say sentiment or sentiment analysis and it gets transcribed because of my accent, it often comes out as cinnamon. And so 100% my sentiment analysis agent is going to be cinnamon. That's awesome. So it's basically doing a vibe check of the email and passing on that information downstream to the other agents. So there's even another agent in this flow. There is an expert agent here that's doing like what core would be doing. We've even added in like a separate research agent to go out onto the internet to do whatever other kinds of research you might think is valuable to pass on that context downstream to the other agents.

**Tyler Fisk** (01:27:32)

Then you have all that information then gets handed off to the You've Got Mail agent, so that customer service email agent, and it's writing its V1 draft of the email. Even in the workflow, we will do this process of, we call it the toast method. It's like tests, it does a thing, it grades itself, it does it again. It's the meta prompting, but at a workflow level. So you've got mail, wrote its email, it's QAing its email, and then it does it again here in this next step. and then this is a version of gigawatt that's called gigawatt unhinged and it writes things that will make your grandma clutch your pearls like it's pretty terrible and we just do that as like an internal agent to send us a slack message it's funny uh it saves this into a short-term memory bank and a knowledge base in cassidy so it will know it uh like moving forward is a history and then it sends us a slack message And so if we're the grower solution team, what this feels like for us or for the Apple team, let's say, is that our agents are constantly listening for new email.

**Tyler Fisk** (01:28:42)

And when a new email comes in and they've answered them, it runs through this process of all these different agents doing the work and then pinging us in Slack and saying, Hey Tyler, guess what? Here's the new email we got. Here was the situation. Here's what we thought about it. Here's the version of the email that we wrote. Do you like it? If so, we'll auto send it. If you don't, let us know what we need to do better and we'll go back and fix it again. And depending on how we answer that question in Slack, It will then force this other trigger right here, which is like the second part of this flow. So this is constantly watching that Slack channel that the agents are talking to us in. And we just talk to that agent, like no hot words, no fancy language. It's literally like we're talking to like an executive assistant that comes in and does this.

**Tyler Fisk** (01:29:31)

And this is what we call a generative filter. It's just a very simple like GPT-40 or it could be like GPT-5 mini, like anything like a cheap, fast model that looks at what we said or what the Apple team said and determines, did we say, yeah, it looks great. Go ahead and send the email. No, it needs this revision or it needs to add this or whatever it might be. Or is it like a message coming back in Slack that's some sort of a confirmation message from an agent? and this is a generative filter based off of that it understands and it will only print one of three outputs here it's either like ship it revise or confirmed and based on this output there's different paths here so if it says ship it the agent will go look up the history go pull the gmail thread id find the email that was written, know that it's approved and actually go send the email for us.

**Tyler Fisk** (01:30:26)

So we don't have to do anything. Like Apple just needed to talk to the agent and then the agent go does its thing. If we had something that we wanted it to improve on or revise, it goes through this different path where it goes and looks up more information. It sees what was done originally. It goes back to the expert agent, the research agent, the email agent. They kind of do their process again. To take into consideration what you said it needs to do differently. And then it brings it back to you in Slack at this like checkpoint for you again of like, hey, we went back and fixed it. Do you like it this time or not? Like we can send it or if we need to fix it again, we can do it. So it's like all of these agents are working under the hood autonomously without us.

**Tyler Fisk** (01:31:08)

And we just have to talk to it in Slack. And that's it. And then once we finally say send it, it sends it on its way, records all that here back into a folder system that we have set up in the RAG knowledge space. So that if, let's say you send through that email about the iPhone Air versus the iPhone Pro, and then we send you a response in email, and then maybe tomorrow you send a follow-up email, we now have memory of that, like both at a system level and like in the email. Also, we could go and like research it in the tool if we wanted to as well. So yeah. This is part of the piece of getting into production is like building out the workflows and the user prompts and all the system parameters around this. That's like a whole thing to go into that.

**Tyler Fisk** (01:31:57)

And at the same time, we have to put into place an eval system and evals are paramount in production. They're so key because that's what gives you observability and a detailed audit trail to know what it is, what's happening in production, what do you need to go fix, what improvements need to be made, what's actually working well. We put that into a Golden's database to reinforce what's going well. Yeah, so it's a complicated system to get to this type of quality, but We haven't found another way to do it, to get to that level of outcome without that level of complexity as well.

**Aakash Gupta** (01:32:41)

Amazing. And all these tools we walked through today, what plans are you on? How much are they costing?

**Tyler Fisk** (01:32:49)

You don't want to see my tech stack, Bill. This is like a mind shift change. So in Cassidy specifically, because we actually teach out of that platform as well as use it ourselves for internal work, We're on an enterprise plan with them. So we're spending like a couple thousand dollars a month on it. But that's like heavy, heavy usage. I would say, though, and this is what like when we were doing more client work. Now we're much more like focused in education. When we were doing client work, it's this kind of. A paradigm shift of don't look at it as like tool expenses. Instead, this is where I have an accounting degree and it comes in handy quite a bit here is that look at what this costs you to do without AI, like your people team to go to each of these functions. If you had to have your experts go get pinged and their time is valuable to go ask them a question about something that only they can ask, and then you have to give that to a customer service rep, and they have to take the time to read the email and respond to the email.

**Tyler Fisk** (01:33:56)

If it's like a high-stakes email, they might have to go get that approved or checked off by someone else in management above them before they hit send. Calculate their hourly wage accordingly. back that into here. And it's always a winning scenario. Like, even if this costs a lot of money in credits, when you look at that on a cost to cost of like, not necessarily like tech stack spend, but real world value translated into what are we spending to agentify that process? Uh, there's always a huge Delta there, like in a positive way. And that will only increase as we keep moving forward because, uh, This is the most appreciating asset. AI is the most appreciating asset in the sense that the quality of the outputs that we get is improving on a logarithmic scale. And we know it will continue on that trajectory because of things like Moore's Law.

**Tyler Fisk** (01:34:53)

And it's also racing to zero on how much it costs to actually use these things. Because there are open source models that you can run for the price of electricity on your local machine now that are... like essentially free that are just as good, if not better than the leading models from like OpenAI or Anthropic from like six months to a year ago. so like it's going to be the most expensive it's going to be right now is the main takeaway i would tell you for that

**Aakash Gupta** (01:35:22)

all right this completes our demo of how to build multi-agent workflows into production there's obviously much more that we could have gone into but that's the high level before we go since i have you here there are a couple questions i have to ask you guys You and your partner, Sara, you guys crossed seven figures in a year. What's your advice to people looking to create seven figure courses?

**Tyler Fisk** (01:35:52)

Be ready to work your tail off for sure. We launched AI Build Lab as what we thought was going to be a side hustle, actually. I would say a couple of different things. I would say constantly be listening to your customers and iterating and improving because we hear them. We understand if they're like grasping these concepts and the way that we're teaching it. Is it connecting with them or not? And we're going back and revising it so that the next round we're getting better for each cohort. So that's one thing. Once you start to get any sort of massive students coming through, you need to start thinking about your own personal infrastructure, whether it's AI-fying processes yourself or bringing people team on, adding the headcount, which we've done, both of those. Yeah, and just like really honestly just like working your butt off as well, like in bringing value.

**Tyler Fisk** (01:36:47)

We spend a lot of time in live sessions answering questions for folks and we find that that has like, we poured into them. Like we have very much so an abundance mindset. And because of that, we don't have to advertise very much. Almost all of our business is word of mouth. And, and even talking to like the Maven, uh, executive team, even, even, uh, gagging himself. Uh, they're like, y'all are a bit of enigma to us because we don't have PhDs after our names and we didn't work for any of the big Silicon Valley tech companies. And yet, uh, somehow we've managed to come out of nowhere and make a seven-figure course on Maiden. So I think it's just like pouring yourself into the quality of the product that you're giving to your customers and

**Aakash Gupta** (01:37:32)

really

**Tyler Fisk** (01:37:32)

caring about that.

**Aakash Gupta** (01:37:33)

Are you able to share any facts and figures for folks, like how the business is doing now or how big the latest cohort was?

**Tyler Fisk** (01:37:39)

Yeah. We have had, I don't even know what the new, so we have another cohort starting up here in October. The one that's in there right now is between 100 and 200 people in foundations. And I believe we're over 200 people in our doc gen course, which is like the advanced, the next course. We are now at a run rate where we're running at like about 1.6 million in gross revenue, which is still kind of baffles me because I'm an entrepreneur. I've been a part of multiple businesses and launched multiple businesses and Sar and I take that for granted sometimes of like how quickly we've been able to hit that and we're grateful for that for sure.

**Aakash Gupta** (01:38:22)

Definitely a really interesting case study. Anybody who's watched this far knows why you've hit that success. It's the depth of the knowledge of these new tools that nobody else has. I've had plenty of people build AI agents on this show and you have a next level depth of that knowledge. What's next for the AI Build Lab empire?

**Tyler Fisk** (01:38:41)

That's something we've been talking about quite a bit, actually, internally. I think a few different things. We really want to scale our foundations course, which is our entry-level course. It's definitely not entry-level, but it's our first course because for us, it's incredibly important to not just say it, but actually do it to bring more people from all over the world, diverse areas of work and demographics so that we are actually democratizing AI because we still live in a bubble. Most people still don't know what's even possible with this tech and we want to enlighten folks and bring more voices and more people to this table because it's huge. So there's that. And then the other thing I would say is that we've been thinking a lot about trying to get into the product space. So like this Hey Gigawatt thing, we've been trying to figure it out because that also helps people go from needing to know all of this head knowledge.

**Tyler Fisk** (01:39:43)

The idea is that Hey Gigawatt works for any kind of a non-technical user, guides them through this process and builds everything for them in the back end. So it's kind of like vibe coding. And I don't even love that term, but kind of like that for agent building in an essence. So, yeah.

**Aakash Gupta** (01:40:01)

Well, I'll be cheering you on from the sidelines. I'm sure everybody who's watched and listened to this point will as well. Tyler, thank you so much for sharing your expertise with us. Thank you so much. It's been

**Tyler Fisk** (01:40:11)

a lot of fun. I appreciate it. Bye, everyone. All right. Bye, y'all.

**Aakash Gupta** (01:40:15)

So if you want to learn more about how to shift to this way of working, check out our full conversation on Apple or Spotify podcasts. And if you want the actual documents that we showed, the tools and frameworks and public links, be sure to check out my newsletter post with all of the details. Finally, thank you so much for watching. It would really mean a lot if you could make sure you are subscribed on YouTube, following on Apple or Spotify podcasts, and leave us a review on those platforms. That really helps grow the podcast and support our work so that we can do bigger and better productions. I'll see you in the next one.
