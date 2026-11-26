---
title: "OpenAI Head of Product (Integrity) on the Future of AI Agents, PM, and AI threats"
subtitle: "What it's really like building products at the hottest AI company in the world."
date: "2025-08-24"
host: "Aakash Gupta"
guests: ["Jake Brill"]
speaker_names: "substack"
substack_url: "https://www.news.aakashg.com/p/jake-brill-podcast"
youtube_url: "https://www.youtube.com/watch?v=j4gdMHYfHaE"
duration: "01:21:05"
word_count: 15089
source: "Substack episode transcript (aired audio)"
sponsors:
  - name: "Jira Product Discovery"
    url: "https://www.atlassian.com/software/jira/product-discovery"
  - name: "AI PM Certification"
    url: "https://maven.com/product-faculty/ai-product-management-certification?promoCode=AAKASH550C7"
  - name: "The AI Evals Course for PMs & Engineers"
    url: "https://maven.com/parlance-labs/evals?promoCode=ag-product-growth"
  - name: "Maven"
    url: "http://maven.com/x/aakash"
---

**Sponsors:** This episode is brought to you by [Jira Product Discovery](https://www.atlassian.com/software/jira/product-discovery), [AI PM Certification](https://maven.com/product-faculty/ai-product-management-certification?promoCode=AAKASH550C7), [The AI Evals Course for PMs & Engineers](https://maven.com/parlance-labs/evals?promoCode=ag-product-growth) and [Maven](http://maven.com/x/aakash).

# OpenAI Head of Product (Integrity) on the Future of AI Agents, PM, and AI threats

*What it's really like building products at the hottest AI company in the world.*

**Aakash Gupta** (00:00:00)

In the future, are PMs going to have to learn how to manage not just humans, but agents?

**Jake Brill** (00:00:03)

Absolutely. You're going to be interacting with, managing, collaborating with other people. I think that's very much the case with agents. And so there's going to be a new skill set that people need to develop.

**Aakash Gupta** (00:00:12)

Jake Brill is the head of integrity product at the hottest AI company in the world right now. He works at OpenAI. Before that, he was a director of product at Instacart and a product manager at Meta. So you guys just released GPT-5. It was a whirlwind launch. What did it feel like inside? Truly energizing. What do PMs need to know

**Jake Brill** (00:00:32)

about agents? If you look at your average product manager and you said, what's your AI strategy or how are you building an AI first product? A lot of people wouldn't necessarily have an answer for that. And over the past couple of years, it's like if you're not building a product that has AI fundamentally in its DNA, you're not really keeping up with the future of digital technology.

**Aakash Gupta** (00:00:51)

One of the craziest things I heard about agents recently was that agent internally was manipulating performance data.

**Jake Brill** (00:00:58)

How do you deal with a world where agents learn to cheat? It's a hard problem, a very big research problem we're going to keep working on.

**Aakash Gupta** (00:01:04)

You mentioned Slack. I think that was one of the coolest insights that came out about OpenAI in the last few weeks that the company almost entirely runs on Slack.

**Jake Brill** (00:01:12)

Yeah, almost entirely. I would say conservatively like 90% of my written communication is in Slack.

**Aakash Gupta** (00:01:17)

If you're a company who's maybe not a model company, but you're trying to create an eval system as robust as OpenAI, what would be your lessons for them? Well, in a lot of cases, you don't have to build these evals from scratch. There are industry standard evals that you can use. What does the PM role look like in five years? Really quickly, I think a crazy stat is that more than 50% of you listening are not subscribed. If you can subscribe on YouTube, follow on Apple or Spotify podcasts, my commitment to you is that we'll continue to make this content better and better. And now onto today's episode. Jake Brill is the head of Integrity Product at the hottest AI company in the world right now. He works at OpenAI. Before that, he was a director of product at Instacart and a product manager at Meta.

**Aakash Gupta** (00:02:10)

We have a ton to talk about, especially as it relates to how does OpenAI handle negative scenarios within AI? How does OpenAI build product? Jake, welcome to the podcast. Thank you so much for having me. It's a real thrill to be here. So you guys just released GPT-5. It was a whirlwind launch. You guys were actually everywhere. I think this was the most marketed launch I saw from you guys. What did it feel like inside?

**Jake Brill** (00:02:40)

truly energizing you know we've been working on gpt5 for a very long time and in the days weeks months leading up to the launch the energy was just palpable we knew how incredible of a model we had we knew how much of a game changer it would be for people to experience a reasoning model because most people haven't and so bringing that power to people um it just felt like we're just one step further in our quest towards AGI and fulfilling our mission. The energy was great. The day of the launch, you know, it was a really well done launch event. And just seeing people's reaction in Slack, starting to see the graphs, like watching people use this product, it just, it felt incredibly fulfilling because this was a lot of really smart people working really hard for a long time and seeing it come to the world, it was just like, okay, we're here.

**Jake Brill** (00:03:33)

Very exciting.

**Aakash Gupta** (00:03:34)

You mentioned Slack. I think that was one of the coolest insights that came out about OpenAI in the last few weeks that the company almost entirely runs on Slack.

**Jake Brill** (00:03:42)

Yeah, almost entirely. I would say conservatively, like 90% of my written communication is in Slack.

**Aakash Gupta** (00:03:50)

wow and what does it look like like is there any special things about your guys's slack setup do you guys have a lot of ai agents in there keeping things updated

**Jake Brill** (00:03:58)

yeah you know it's funny because at instacart we were really slack heavy as well and instacart was fully remote for my last several years at the company and so we relied a ton on slack there so when i joined open ai i had something that could fall back on and so i was used to a company that ran heavily on slack In terms of what makes our usage of Slack special and more unique for us, yes, absolutely, we have AI agents in the channels. They can serve any number of purposes. There's one that we have that's like a general purpose answer agent, which is really helpful. So if you have a general Q&A in the channels where that agent exists, you can get questions without one of your coworkers having to see the post and respond to it manually. We very much believe OpenAI and in using AI in all parts of our user and enterprise experience.

**Jake Brill** (00:04:45)

So, yeah, it's no different in Slack.

**Aakash Gupta** (00:04:47)

very interesting now you head up integrity product what is integrity products role in a big launch like

**Jake Brill** (00:04:55)

gpt5 sure so there are a couple big areas that were involved in this launch the first is what you might classically think of when it comes to integrity you know preventing bad things from happening people from doing bad things with our models and our products and we certainly did a lot of work in the lead up to and following the launch in that space for gpt5 In addition to our work on preventing bad things from happening, one thing that often happens when we have new launches is we see a lot of people try ChatGPT for the first time or try our new models via the API for the first time. And another area that integrity is responsible for is our identity system. So when we release new models, like this happened with our image gen model, as well as GPT-5, you see an increase in traffic, people wanting to sign up for the first time, people logging into their accounts.

**Jake Brill** (00:05:46)

You wanna make sure those systems don't fall over and that your systems are able to take meaningful increases in volume so that they maintain their world-class uptime and latency because it would be a really bad user experience if people try to go use GPT-5 for the first time and they just get an error message. Similarly, our team is responsible for our financial systems. when we launch new models is often the case that will lead to people converting to paid subscriptions or more people using prepaid API credits to use the model. And so similarly, we want to make sure that our payment systems are up, they're running, they're seamless. good authorization rates, but also that you don't see an influx of people with stolen credit cards fraudulently using our models and our products. So a lot of work behind the scenes to make sure that GPT-5 shines in all of our different products.

**Aakash Gupta** (00:06:43)

Fun fact, Amazon put two holds on my account as I ordered the equipment for this in-person podcast today. So it's not just on the credit card side. Even the person who's making a purchase, an OpenAI or an Amazon, is monitoring those accounts to see are these suspicious transactions and flagging those appropriately. Exactly. Very interesting. So if we break down, let's say, let's stick to GPT-5 for a second. What are the big streams of work that a company like OpenAI is doing to make sure that it meets your integrity standards? Is there red teaming? Are there certain evals? How would I put it into buckets?

**Jake Brill** (00:07:22)

Yeah, absolutely. We do red teaming not just for new launches, but for our products all across the board. And red teaming happens at all stages of product development. When you're training the model, when you're training your production systems to mitigate... uh harms from happening we have both manual red teaming as well as automated red teaming uh we'll do that at different checkpoints while the model is being trained we do it with the final version of the model before it goes live and then we also do red teaming after models go live just to make sure it's like okay well we prevented the known jailbreaks are there new jailbreaks that are out in the wild that that are automated systems or or uh penetration testers are trying to to find ways to to get around the protections in our model other sorts of work that we do there's a lot of work to make sure that our automated systems have high precision and high recall you know we want to make sure that if we're taking some sort of automated action that we're really accurate with that because we take it very seriously if we block a generation or warn someone's account or even at the extreme ban someone like those are very serious interventions And we want to make sure that we hold ourselves to a really high standard that when we take those actions, we have really high confidence that we're getting it right.

**Jake Brill** (00:08:37)

Similarly, we want to make sure that our recall is high so that we're just not blind to false negatives and there's all sorts of bad stuff going out there that we're not aware of. We also do a lot of making sure that we have robust operational tooling and capacity to make sure that we project forward. We think X number of things will require manual review. We want to make sure our tools are sufficient so that people have extremely efficient workflows and that we have enough human power and bandwidth so that we can get to things in a very timely fashion.

**Aakash Gupta** (00:09:14)

And I think some people might be kind of rolling their eyes at this moment, like, is all this stuff important? But I think it's actually goes to the core of why even OpenAI was created at the beginning and a lot of the values that you guys have from the beginning of creating this safe AI. Talk to me a little bit about that. How is that interwoven into OpenAI's philosophy and how does that manifest?

**Jake Brill** (00:09:35)

Yeah, I mean, if you read OpenAI's charter, safety is one of the things we talk about very publicly. It is part of the reason why I even wanted to join OpenAI in the first place was when I had my first conversations with them, it was very clear that safety was really important to the company at all stages of model and product development. And I figured if I was going to leave a job that I really loved with people I really cared about, I wanted to do it not just to jump on a hot AI train. I wanted to do it because I really believed that the company... was responsible and took that responsibility seriously. So safety and integrity, it's something we talk about throughout the entire development process. And we do also believe in iterative deployment. So it's not like we're launching models and there's absolutely zero possible way that something could happen that could have a bad outcome.

**Jake Brill** (00:10:25)

We talk a lot about what risks are non-negotiable that we have to mitigate before launch, which are the other ones that we want to have systems in place, and which are the other ones that's like, hey, actually, we could sit in the room stroking our chins thinking like, oh, how might someone do something bad? But actually, at the end of the day, it's really helpful to... to follow OpenAI's approach of iterative deployment, because once you start rolling things out, you can actually see in the real world how people accidentally might misuse your products or professional bad actors might misuse it. And then you can very quickly respond and build sophisticated solutions.

**Aakash Gupta** (00:11:00)

one of the areas that i imagine this is really important is the recent open source weighted model that you guys released and i know you guys even delayed that launch a little bit because you said it wasn't ready how do you really determine like okay this model is safe enough and ready to put out there

**Jake Brill** (00:11:17)

yeah well a lot so much of that is evals you know we try to Make sure we're holding ourselves accountable to objective sources of truth on the relative safety of our models. And there are a number of public evals that companies talk about to ensure that their models are safe. This could be safe in terms of, like, is the model deceptive? Is it safe in terms of is it appropriately refusing some of those high-risk bioprompts, for example? Yeah. You can make vibes-based decisions on this sort of stuff, but ultimately evals are really what's going to guide the day in helping you objectively and with data determine if your model is safe enough to release.

**Aakash Gupta** (00:11:57)

If you're a company who's maybe not a model company, but you're trying to create an eval system as robust as OpenAI for whatever product you've created on top of the OpenAI API, what would be your lessons for them? How can they build evals that they can trust? Well, in a

**Jake Brill** (00:12:14)

lot of cases, you don't have to build these evals from scratch. They're industry-based. standard evals that you can use and we've published a bunch of them but there are many other excellent frontier labs creating safety related evals and so what i would ultimately say is if you're if you're an earlier stage company you don't have to reinvent the wheel here i would really encourage you to just You could even use AI to go do a search on what are the best safety evals. Simultaneously, there are a lot of open source, open standard safety models that you can layer in on top of your model or your product. At OpenAI, we've built a moderation API, and there are plenty of other great options out there. And so I'd say you're not starting from scratch, and I would really encourage people to make use of the great open technology that exists out there.

**Aakash Gupta** (00:12:59)

got it cool so we're walking back in time through all of your amazing launches the one before that you mentioned it earlier agents yeah feels like i can't go on social media without seeing some post about ai agents why is everyone making such a big deal out of agents

**Jake Brill** (00:13:18)

because they're the bee's knees. The way I think about this, you rewind three years ago, ChatGPT launched, people started having their first sort of broad scale consumer experience with AI. And for those first couple of years, it's really been what we call assistance. You know, you asked a model a question, you give it a prompt and you get a response. And that's been incredibly powerful. I mean, the growth of ChatGPT and many other great AI products sort of speaks to the power of AI assistance. But Where we foresee this technology going is not just question and answer, but rather, here's a task. Can you please complete it for me? And that's really where agentic product experiences come in. It's, hey, there's something more complex than just, like, what's the weather today? Can you go and take an action on my behalf? And that action could be synchronous or it could be asynchronous and you come back because it's a rather complex workflow.

**Jake Brill** (00:14:14)

And I think what's been so great about the progress that's been made in the field of AI is... We've been talking about agentic product experiences for several years, but we're now really starting to bring to bear across ChatGPT agent and also agentic products that other companies are building a real way to put tools in people's hands. They can't just answer their questions. They can also do things on those people's behalf.

**Aakash Gupta** (00:14:37)

Yeah, I personally am using a lot of those no-code agent builders like Lindy, Relay, Make, Zapier. You can chain together like crazy workflows. So what do PMs need to know about agents?

**Jake Brill** (00:14:52)

The thing I would say is I'm going to go back again to 2022. If you look at your average product manager and you said, what's your AI strategy or how are you building an AI first product? A lot of people wouldn't necessarily have an answer for that. And over the past couple of years, it's like you're. if you're not building a product that has AI fundamentally in its DNA, you're not really keeping up with the future of digital technology. And I think we're sort of at that space again with agentic products. It's, you know, that classic Wayne Gretzky quote, you skate to where the puck is going, not to where the puck is. The puck has been at assistance. The puck is going to agents. And so what I would say is if you're not thinking about how to build products that are agentic in their fundamental nature, You're probably A, not maximizing the power of this technology and B, you're probably building a product that's going to be obsolete in a shorter time horizon because your competitors are going to be thinking about building products that solve people's problems in an agent first fashion.

<!-- sponsor -->
**Aakash Gupta** (00:15:57)

Today's episode is brought to you by Jira Product Discovery. If you're like most product managers, you're probably in Jira, tracking tickets and managing the backlog. But what about everything that happens before delivery? Jira Product Discovery helps you move your discovery, prioritization, and even road mapping work out of spreadsheets and into a purpose-built tool I'll see you next time. That's A-T-L-A-S-S-I-A-N.com slash product dash discovery. Jira Product Discovery. Build the right thing. Today's episode is brought to you by the AIPM certification on Maven. Run by Mikdad Jaffer, who is a product leader at OpenAI, this is not your typical course. It's eight weeks of live cohort-based learning with a leader at one of the top companies in tech. OpenAI just doesn't stop shipping, and this is your chance to learn how. Run along with Product Faculty and Mo Ali, the course has a 4.9 rating with 133 reviews.

<!-- sponsor -->
**Aakash Gupta** (00:17:16)

Former students come from companies like OpenAI, Shopify, Stripe, Google, and Meta. The best part? Your company can probably cover the cost. So if you want to get $500 off, use my code AAKASH25 and head to maven.com slash product dash faculty. That's M-A-V-E-N dot com slash P-R-O-D-U-C-T dash F-A-C-U-L-T-Y. And what does it mean to build in an agent-first fashion? Because people are talking about, you know, user experience is going to turn into agentic experience. You need to figure out how your product will be open to AI agents. Like, what are the elements that a PM should be thinking through for making their product agent-friendly and usable?

**Jake Brill** (00:18:01)

Yeah. One of the first things I would say is so many digital products are synchronous in their nature. Like I take an action and a response or something else happens immediately. And if you start thinking, hey, what if I could enable a product experience that is far more complex? and it doesn't have to happen immediately i think that's one of the biggest changes that's happening right now is is a stop boxing yourself in and thinking like someone clicks button and action happens immediately rather it's someone clicks button and something far more complex can happen behind the scenes and you don't have to sit there waiting for response uh the product can come and let you know in the future when that very complex task has happened

**Aakash Gupta** (00:18:45)

So what are some real life use cases that you're using agents for? Yeah.

**Jake Brill** (00:18:51)

Well, we're growing a lot at OpenAI. And so I spend a lot of my time hiring and interviewing candidates. And I find it's been deeply meaningful and helpful. to use agentic products to help with the recruiting process. I'll say like, hey, we need to bring in a designer. Here's sort of the properties. Ideally, they have X years of design experience or they've worked in this size company and they're located in the Bay Area. Please go help and source some candidates. really really strong for that sort of use case in my personal life i've been using agentic products a lot to do longer horizon uh research um i got this like super gnarly uh respiratory virus in december and i have been seeing a bunch of of doctors about it and like i'm not Varying levels of usefulness from those doctor's visits. And I've actually found that using agents to go do some of the research and suggest alternative methodologies for helping my lungs get back to 100% has been really helpful for me personally.

**Aakash Gupta** (00:20:03)

Okay. And on the product management side, if I'm just a product manager, what agents should I think about building or using? Yeah.

**Jake Brill** (00:20:11)

So for building, I think agents are really helpful for running market analysis, understanding if you're a PM in a given area, like What sort of products exist in that area? What is the general sentiment towards them? What are the needs of people who are looking at products in that area? I think agents can be really helpful in helping you pull together collateral. I am not the best at visual... I'm not a great PowerPoint PM. I can tell the story, but... I don't have a background in consulting. I was never the best at making beautiful slides. There are now some really excellent agentic products that can help you visually tell your story in a way to supplement all of your written communication skills. I also think agentic products... can help you prototyping a lot. That's one of the things we've been starting to do internally is rather than just writing a proposal for how something works, just build a prototype of how something could work and you put that in people's hands and it's a great way of illustrating how your product might work without having to go in, make mocks, start building an initial prototype on the software side.

**Jake Brill** (00:21:39)

It's like a very inexpensive way of bringing your ideas to life.

**Aakash Gupta** (00:21:44)

Yeah, I ask a lot of heads of product on the podcast, like, what are the big ways your PM team is using AI tools? And AI prototyping is always the number one thing they talk about. What do you see as the future for PRDs in a world of AI prototyping? Yeah,

**Jake Brill** (00:22:02)

that's a great question. So I still think there's a world for PRDs because in some of the, like, AI technology is making PRD writing so much better you know if I these days I'm more in a support role so I'm not writing as many PRDs but if I rewind like a year and a half when I was in my earlier days at OpenAI and spending more time writing PRDs and I I kept trying to use AI for writing the PRDs and it just like came up short. The product form factor wasn't right. It didn't sound like my voice, the like amount of context that was necessary. Like the PRDs, like I ended up just writing a bunch of them and you fast forward to where we are now. And I think AI has made PRD development much better. You know, at least within OpenAI, I think Canvas is a much better form factor for collaboratively putting together a longer documentation.

**Jake Brill** (00:22:53)

I think our models are better at creative writing. With connectors, you can connect to external data sources to help bring these documents to life. And then lastly, with memory, these models learn a little bit more about what your writing style is, what other things that you've worked on. They can bring that to bear. So I think there definitely is a future for PRDs. I think they're going to be AI first. And the value of PRDs is you can do a prototype, but you may be missing a bunch of things in that prototype. Like, how do I handle, you know, like... How do I handle this failure case or how do I? You know, what is it? What is our marketing strategy that we're gonna bring with the product when we bring it to market? So I think there's I think they're gonna go hand in hand the prototypes and the PRDs I do think PRDs will be less wordy Because you won't have to spend as much time describing oh you click on this button and this thing happens you can just show people but I think even a world where people are prototyping more with our models and our products, I still think there's a place for PRDs.

**Jake Brill** (00:23:57)

One of the

**Aakash Gupta** (00:23:58)

coolest things that you guys open sourced, I believe it's called your model spec, which had like a ton of examples. I think probably that your team was responsible for of like when user has request this, don't provide that information when they say this, do that. Is that more the direction your PRD needs to go in a world of AI products where you are giving the specific examples of what not to cover and how to respond? I think

**Jake Brill** (00:24:23)

that's a good example. I think part of what you are talking about is also covered by evals, which right now we sort of view that as complementary to the PRD or spec. But I do believe increasingly in the future, yes, it's going to be describing not just the way the product work, but the way the model that's powering the product should work.

**Aakash Gupta** (00:24:43)

Mm hmm. yeah okay actually can you clear that up for me what should go in the eval and what should go in the prd

**Jake Brill** (00:24:50)

i think a lot of the prd is like classically it looks a lot like what we have today like here's the problem that we're solving here is the way a product would work here's our definitions of success here's our target user and evals are really fundamentally like here are the use cases this product should be good at and here are ways that we can We can test the model to evaluate. Is it successful at these specific use cases?

**Aakash Gupta** (00:25:16)

Okay. So PMs, they typically own the PRD, even though they're jointly creating it with the research engineering and design teams. When it comes to evals, you know, who owns that and how do PMs plug into

**Jake Brill** (00:25:29)

those? Well, increasingly, we're asking PMs to take a really active role in developing evals. And I think as the role of PM changes over time, that's going to be of increasing importance. Anyone can write an eval. It doesn't have to be a researcher. It doesn't have to be a software engineer. It doesn't have to be a PM. But we're finding that because the PMs oftentimes are the ones with the clearest vision of how the product should work in their head, they're very well positioned to write evals because they have a very strong opinion on here's what the product should be good at and here's what the product should not attempt to do.

**Aakash Gupta** (00:26:03)

I always love to get sidetracked on the tangents about PMs. I want to return back to agents for

**Jake Brill** (00:26:07)

a second. Yeah,

**Aakash Gupta** (00:26:08)

sure. How

**Jake Brill** (00:26:10)

do AI agents talk to each other? Yeah, this is a good question, and I don't think it's a solved question. I really enjoyed your podcast about MCP, and the power of something like MCP is it is a common protocol that multiple... companies AI developers can use that standardize how agents talk to tools. I think if you project out in the future, we're going to need something like that for agents to talk to agents. There's not going to be just one company building agentic products. There's going to be the frontier model labs building their models that can power agents. Those model labs are going to build agentic products. And then there are going to be tens, hundreds of thousands, millions of developers building agentic products on top of those models. And the failure state would be if... there's not a standard language for all of them to talk together.

**Jake Brill** (00:27:02)

Agent A talks to Agent B, but they're speaking different languages, and so it just falls apart. So I think the answer here is going to be that we need something in the vein of MCP, which is an open standard that companies can use so that whoever's making the agents, they can talk to each other. But it's something we're talking about internally, but I think there's more work that we need to do to have a consistent answer that can work broadly.

**Aakash Gupta** (00:27:24)

Okay. And MCP is, it's developing. I guess people are trying to call it the USBC. What are the limitations of MCP that people should know about? Is

**Jake Brill** (00:27:38)

it? Ultimately, the limitations are going to be that it's just really early stage, and there's a bunch of key functionality that needs to get figured out. So if you'd asked me a couple months ago, MCP hadn't quite figured out auth, and that was something that standardizing how authentication would work was a big open opportunity. I think that's going to be the case for a while, that there are key things that's good at tool calling, but... I think it's just like, it's early. It hasn't even been around for a year. So I think fundamentally MCP is just like, The way it's going to get better is more time, more people developing on it, and frankly, more companies contributing to it so it becomes more fully functional.

**Aakash Gupta** (00:28:19)

So you don't need to evaluate the state of it as it is. Sometimes people are worried about the security and these things. It's still an open standard. It can still be improved and developed. Correct. Yeah. Okay. So one of the craziest things I heard about agents recently was that an agent internally was manipulating performance data. How do you deal with a world where agents learn to cheat like humans

**Jake Brill** (00:28:41)

do? Yeah. It's a hard problem and a very big research problem we're going to keep working on. And to me, a lot of that fundamentally gets down to the question of alignment. Like, are the agents, is AI acting in a way that is aligned with the values that you're trying to install in it? So at the core of it, it's a lot of training the model, making sure that it's robust, making sure that it isn't deceptive. And one of the things we're really excited about for GPT-5 is... you know in our evals um measuring deception uh this model is is so this is where you want the score to be the lowest not the highest so it scores the lowest but you know it's greater than zero and you want that number to be zero so um a lot of it has to do with alignment and then a lot of it has to do with you having systems to detect when when uh the agents go rogue it they could be going rogue because you know a person asked the agent to do something bad um And the way you solve for that is, you know, multi layers of defense.

**Jake Brill** (00:29:44)

You know, again, like I said, you train the model not to do bad things. Then you have model level classifiers looking at the inputs going into the model and the outputs coming out of the model. And then you layer on top of that a lot of account and behavioral signals about the individual. Is that individual trying to do something sketchy with the model? Yeah. And then there's also is the model doing something because it got tricked into it. And that could be cheating, like you said, but it could also be data exfiltration. And so there's a lot of work to make sure that even if the model is perfectly aligned, even if the person who's acting in a very benign fashion. the agent may still interact with some external resource that tricks into doing something bad. That resource could be a code repository, could be a website.

**Jake Brill** (00:30:31)

And so there's a lot of work that we do to mitigate prompt injection, to make sure that the agents are acting in a reliable fashion. Similarly, model training, model level classifiers, actor level classifiers, production monitoring, and then just like constant red teaming. So the answer is we haven't, We don't have a silver bullet here because there's never going to be a silver bullet. The answer is you need to have multiple layers of defense against agents acting in deceptive fashions, agents cheating, or people using agents for nefarious purposes.

**Aakash Gupta** (00:31:01)

AI evals are one of the most important skills for PMs. And

**Jake Brill** (00:31:05)

I

<!-- sponsor -->
**Aakash Gupta** (00:31:05)

know you know they matter. The question is, are you doing them right? Most teams are winging it with basic metrics and hoping for the best. Meanwhile, the teams that actually ship reliable AI, they've cracked the code on systematic evaluation. Today's episode is brought to you by the AI evals for engineers and PMs course by Hamal Hussain and Shreya Shankar. This live Maven course will teach you the battle-tested frameworks from Hamal and Shreya, who are the engineers behind GitHub Copilot's evaluation system and 25-plus production AI implementations. Four weeks, live instruction, next cohort starts July 21st. start shipping ai that actually works enroll at maven.com with my code ag-product-growth for over 800 off that's ag-p-r-o-d-u-c-t-g-r-o-w-t-h Today's episode is brought to you by Maven. The problem with most courses online like Udemy is there's no live component and the instructors aren't experts in their fields, they're professors. At Maven, you get direct live access to experts and operators from the world's best tech companies.

<!-- sponsor -->
**Aakash Gupta** (00:32:15)

You can't get that access anywhere else, in any university, and you usually can't find them on YouTube either. I featured so many of Maven's experts in the newsletter and podcast for that reason. To help you out, I've put together a collection of courses I recommend at maven.com slash X slash Akash. This includes courses like AI prototyping for PMs, product sense for PMs, and getting an AI PM certification. Visit it now at maven.com slash X slash A-A-K-A-S-H. So agents is one topic that everybody, when I asked, what should I ask Jake? They were like, ask him all about agents. We covered that. The next second most voted topic was all about what does the product team culture look like inside of OpenAI? So if we start with the context, right? How does integrity product fit in more broadly within the product teams at OpenAI? Sure. So I'm going

**Jake Brill** (00:33:13)

to be super reductive. OpenAI is a research and a product company. We have a number of PMs on the research side of the company, people who are focused on things like model behavior, like what is the personality of the model, what are the vibes of the model, people who are focused on safety, things I was saying before, how do you do research on frontier safety risks, train the model to be safe and not take harmful actions. And then there's the product side of the company. And that's really focused on how do you take these frontier safe models and bring them to humanity. And you've probably interacted with many of the products we built. You know, there's PMs working on the consumer version of ChatGPT, the enterprise version of ChatGPT. got a team of pms focused on third-party developers and the way i talk about integrity is we are a platform team that builds shared technology that helps those product teams bring our ai models to humanity we are we are fundamentally we we build systems products and tools that are focused on minimizing risk and maximizing trust and control

**Aakash Gupta** (00:34:19)

So platform teams, I've PMed a couple of them, managed a couple of PMs on platform teams. I feel like more than any other team for them, like the traditional corporate planning process was really helpful because

**Jake Brill** (00:34:31)

they

**Aakash Gupta** (00:34:31)

could get buy-in from teams who would build on their platform that they were going to actually use it so that they could actually figure out if they were building it. Does OpenAI have a planning process like that? How do you guys get the buy-in you need to understand what

**Jake Brill** (00:34:44)

platforms to build? Yeah, yeah. So we do have a planning process. We deliberately try to keep it pretty light because it's a very dynamic environment and a very fast-moving industry. And, you know, Kevin Weil, my manager, our chief product officer, often repeats the Eisenhower quote. Yeah. Plans are useless, but planning is everything. It's a really helpful exercise for people to talk about what they think is most important, where they're going to be spending their time. And even if you diverge from your plans, it's good to go in being mindful about what you think is most important over those next three months, even though something's inevitably going to change. So our planning process only lasts a couple of weeks. We plan over every three-month quarter. And often the guidance I give to the integrity team is, Assume you're only going to accomplish something like 60 to 70% of your plan.

**Jake Brill** (00:35:35)

If you do anything more than that, it probably means you weren't being flexible enough to the needs of the business. If you do anything less than that, probably didn't do a great job forecasting what was going to be most important over the quarter. But we very much write our plans in pencil, not in pen.

**Aakash Gupta** (00:35:49)

So you guys still do the three-month planning process. And how does that couple-week sprint look like? So

**Jake Brill** (00:35:54)

it's very bottoms up. There's some amount of the teams, you know, for integrity, we've got in the other, like, product verticals within the team, within OpenAI, you've got your own like individual swim lanes within there. And so we asked the teams to sort of come up with bottoms up plan for what they think is gonna be most important over the next three months. Simultaneously, we run like an internal dependency intake process where people say, hey, I want to do X, can you help support X with this version of technology. Being a platform team, we get a large amount of inbound requests, probably multiple times more than the other average team within OpenAI, both because we're building shared technology for the other product teams, but also because we have really close partners on our user operations, product policy, intel investigations teams, and we build tooling and data systems for them as well.

**Jake Brill** (00:36:54)

So the process only takes a couple of weeks. We put together pretty lightweight documents that follow a template of like, You know, reflections on the prior quarter. Here's what we're, you know, here's the big themes running after this quarter. Here's how we're going to measure success. And then we'll either review those documents synchronously or asynchronously. We aim for async, again, because those meetings can be expensive. So we try to see how much we can get through in comment form. And if there's still some meaty topics that we can't resolve asynchronously, then we'll jump in a room with the relevant folks and just talk through the main outstanding items.

**Aakash Gupta** (00:37:31)

And how important are success metrics as part of that equation? Because some companies I've worked at, that's like the entire currency. I worked at a fintech company. Everything, ultimately, it's boiled down to GMV, right? And I feel like there's so many different goals OpenAI has as a company. You probably aren't just like an OKRs-based company. How do you treat success metrics? So we definitely have

**Jake Brill** (00:37:53)

success metrics. What I'll say is the success metrics for integrity have a different shape from any other teams. You can measure the success for ChatGPT and classic things like how many people are using the product, things of that nature. For integrity, we sort of view our success metrics as are we building systems that enable the success of other products? So there are some standard metrics that many teams use, but for us, we think a lot about latency, uptime, maturity of our systems. And really what those systems are there to do is to make sure the other products can shine. So for example, I mentioned earlier, our team is responsible for our identity system. So we think a lot about like How many nines of reliability do we have? Because if people can't log into their accounts or people can't sign up for their accounts, well, OpenAI just isn't going to accomplish its overall goals.

**Aakash Gupta** (00:38:45)

um okay so sounds like each of the little platform areas might have some product metrics but there isn't like some overall business output metric that an integrity team would be going after um

**Jake Brill** (00:38:57)

the the top metrics for the company we view ourselves in service of them but like we we don't like take goals on on you know number of users of of this product or that product because we're a bit downstream from that and and so the way we think about successes those teams are going on those metrics and what we do is we we ask ourselves are we building systems that make our products enable our products to hit their goals effectively

**Aakash Gupta** (00:39:26)

so you've been a pm at facebook for a really long time you're a director of product at instacart What are the things that are unique about OpenAI's product culture? Oh, man.

**Jake Brill** (00:39:42)

So with the caveat that I left Facebook like nine years ago, which is a very different company now, and I left Instagram about two years ago. One of the things that's classically different about OpenAI is... AI, you know, like we are constantly asking ourselves are we making are we truly dogfooding our technology? Are we using it as powerfully as we can in all parts of our product development process? And I imagine those companies are asking themselves the same questions now. They just weren't at the time when I was working there secondarily is You know, classic product development is, okay, who are my users? What are the problems they have? And what are the products we can build to solve those problems? And to be clear, we absolutely do that at OpenAI. But then there's this other pretty fascinating approach to product development is we've got the best researchers in the world building the most powerful AI capabilities in the world.

**Jake Brill** (00:40:34)

And sometimes it's like, holy moly, we just had this big research breakthrough. How do we bring this capability to humanity, which is quite different than... like going and interviewing someone, because they might not even know that that capability exists and they could solve their problems. So it's a very different environment through that lens and one of the special parts of being at both a research and a product company.

**Aakash Gupta** (00:40:56)

I think just having a research arm probably also makes it different. What is it like? How do you correctly work with the research team? How do you bring them into your overall product trio? Yeah, so

**Jake Brill** (00:41:09)

fundamentally, it... it's all about having shared vision of the model capabilities and the product capabilities we want to bring to humanity. And so a lot of this is understanding the research roadmap, trying to make sure that as we are post-training the models that they're capable of unlocking the capabilities that match the products we're trying to bring to the world. So, you know, I mentioned Canvas earlier, like that doesn't just like come out of the box. There's a lot of collaboration between the product team building Canvas and the research team that's building it so that it can really shine for collaborative editing of a document, for example. So in my experience, the products that are most successful, there's like a really, really close collaboration between the engineering product and research team so that there's extreme clarity on... What are the problems we're trying to solve and what is the product experience we want to enable for the world?

**Aakash Gupta** (00:42:06)

Yeah, because I guess the best products will probably be ones that are using the most recent research breakthroughs, but also kind of sculpted in a way like Canvas for some set of user problems that is new or opening up some new ground for OpenAI. That's exactly right. Yeah. Very interesting. What are the key rituals that you guys have as a product team?

**Jake Brill** (00:42:29)

You know, many of the rituals are similar to rituals you would find elsewhere. We talked about one earlier, which is we are very Slack heavy. And we do a lot of information sharing and collaboration over Slack. We also, you know, we really strive to have everyone in the office three days a week. So there's a lot of product development, which is just like, let's grab a whiteboard and let's work on this together. I really enjoy that. You know, I love my time at Instacart and my last couple of years, we were fully remote and I had a great experience being fully remote, but there is something special about being in person with your collaborators and being able to have that real time conversation. We, you know, there's classic like we do product reviews. We have recurring meetings. The product reviews are interesting because, you know, oftentimes when you see companies really fast one thing that changes is there becomes a lot more process and a lot more polish around product reviews really like expansive product review decks and one of the things I really appreciate about the way that we've been growing is we try to keep our product reviews like they are They're not nearly as fancy as that.

**Jake Brill** (00:43:37)

People come in, it doesn't matter what level you are, you can talk directly with leadership. You don't have to have a fancy slide deck. You bring in the product, you bring in collateral around it, and you have a very high integrity discussion on it. And then I think, as I mentioned before, one of the rituals is just like constantly asking yourself, are you using our technology as much as possible? And that not only means in terms of developing the products, but we do a lot of dogfooding internally. Like as soon as something is ready to be tested internally, we roll it out to employees. We heavily encourage people to test things out because that's one of the best ways you can answer the question of, is this any good?

**Aakash Gupta** (00:44:16)

Mm hmm. and if i think about that product review process being high integrity not requiring a slide deck there must be a certain culture of trust then within the organization trust that hey even if they haven't laid out all the data that they looked at behind this product decision that they did that data work how do you what is how do you create

**Jake Brill** (00:44:39)

that culture of trust Yeah, and maybe I should clarify. We absolutely do include the data in the product reviews. It's just that, you know, it's more of a classic document as opposed to a very pretty slide deck. The way you create trust, however, there's a couple things. One is, you know... One way to get trust is you just hire the best people in the world because you know that people think through things very thoroughly and very intelligently. Two is you sort of communicate transparently both within the review and then afterwards we sort of share here's the discussion we had and here's sort of next steps coming out of it. And then lastly, I think a lot of it comes from leadership. Create a space where you hold people accountable for having... honest and hard discussions but also in a very supporting and humble way so that people feel like hey you know i may have been wrong about something but there's no shame around that like we're trying to solve some pretty gnarly problems for the first time ever it's like we're not going to get it all right the first time and so making sure that people feel comfortable um having conversations and understanding they may get directed to move in a different direction but that that's not something they should be embarrassed about

**Aakash Gupta** (00:45:51)

Hmm. What's OpenAI's take on experimentation? Are you guys experimenting with everything? How do you handle that?

**Jake Brill** (00:45:59)

We experiment a ton. You know, when you have a product that's used by a tenth of humanity every week, a lot of responsibility comes along with that. Because small changes, you know, may have like large downstream impact in how people experience the product or how they... how it fits into their day-to-day life. So I would say over my two years at the company we've become, we've really leaned into experimentation. We've become very rigorous around how we analyze data. And within integrity, our experimentation looks somewhat similar to other classic product teams. And in some ways it's a bit more unique. We do classic A-B tests. We do do long-term holdouts. But one thing that's a bit more unique about this side of the world is we will also, let me give you an example. Let's say we want to roll out logic to mitigate account takeovers or what we call ATOs.

**Jake Brill** (00:46:54)

Rather than just turn on a role live for everyone or turning it on a 50%, one of the things we may do is running it in shadow mode. turn it on and just log what the hits to that rule might be. And then we either through some other automated or manual process sort of validate, hey, did this match our expectations before we then roll it out to production? So across the product org, we do a lot of experimentation.

**Aakash Gupta** (00:47:19)

So we briefly talked about this, but I want to get a little bit deeper on this. What does working an integrity product look like versus a regular product manager? Yeah,

**Jake Brill** (00:47:29)

I mean, being a platform PM is just, you know, it's like a Venn diagram. You know, there's a decent amount that looks the same, but then there's some stuff that's rather unique about being a platform PM in OpenAI. The first thing is that we are building systems that work well. regardless of who the end user or the end product is. So to go back on that example I mentioned earlier, the deploying logic to mitigate account takeovers. We don't just want to build that one ATO model that works on ChatGPT and then one for people when they're logging into the platform dashboard or one for people who are logging into Sora. That would be extraordinarily inefficient and that's not the right way to build leverage systems. So we build product systems and tools and the goal is they work everywhere. And that's a bit different from many other PM roles at the company, which are focused on like, oh, I'm building this thing for Chachy Petit or this thing for developers.

**Jake Brill** (00:48:32)

The second thing I call out that's different about being an integrity PM at OpenAI is we kind of work on every launch, not every launch, but like pretty close to that. And so what that means is we get to like be involved with a lot of cutting edge stuff that In a way that maybe not every PM team does because they're like really focused on their product or their specific product service. And that's challenging because there's a lot of inbound requests to the team. But it's also super exciting because we get to see all the incredibly cutting edge stuff that we're building across OpenAI. And we get to play a role, sometimes very small, sometimes very large, in the vast majority of product launches that we have. And I think the third thing I would say that's different about being an integrity PM at OpenAI is, you know, classically working in the trust and safety platform space.

**Jake Brill** (00:49:29)

It's often compared to being like a soccer goalie or an offensive lineman. It's like if you're doing a really great job, people don't notice. And it's only if like things go sideways that the light shines on you. You know, as I mentioned before, it could be like payments just start failing or people can't log into the account or we mess up and we ban people. We shouldn't. And so what that means is a lot of the work that we do isn't going to be on the front page of the Times or TechCrunch or there's not going to be a ton of threads about it on Twitter unless things go bad. And so it requires a very low ego to work on this team because you know that what you're doing is you're building really important technology, but that technology is setting up the core products. to have those articles written about them on the Times.

**Jake Brill** (00:50:18)

And so you have to accept that you won't get as much shine, but that doesn't mean your work isn't just as important.

**Aakash Gupta** (00:50:24)

um so when i asked pms in my newsletter to rank the dream companies they wanted to work for open ai was way ahead of the rest of the pack like it was like i think it was like 600 first place votes and the next was 200 okay

**Jake Brill** (00:50:41)

so

**Aakash Gupta** (00:50:42)

you guys had a huge delta you guys everybody wants to work in open ai so If somebody were wanting to work on your team, what would be your advice to them? Like outside of, you can't just sculpt your own background, but what are the things you should be doing, you know, side projects, learning, passion to break in?

**Jake Brill** (00:50:59)

Yeah. There's a couple things there that I would call out. One, you know, when I interviewed with OpenAI around two years ago now, consumer AI wasn't what it is now. And so the fact that I hadn't had a ton of experience working with AI-based consumer products outside of Chappie GPT, obviously, that wasn't, You know, that could be explained away. These days, like, you really need to have a facility with AI products and models. And there's no excuse for not. You know, it's so easy to use these products. It's so easy to vibe code. It's so easy to play around with these APIs that I think the first things first would say, like, start playing around with these models and building things. Mm-hmm. Second, I would say is, you know, one of the best ways of joining OpenAI is if there's someone that you know personally who's worked there.

**Jake Brill** (00:51:53)

You know, the bottom line is when we post jobs publicly, a lot of people apply to them. And so you have to really sift through to find out who's going to be the right fit. And there's two things that really help us know if someone's the right fit. One is if someone at the company has worked with you and can speak to your skill and how great a fit you would be. And the second is you have a presence, particularly LinkedIn, but it could be your resume, it could be elsewhere, that sort of speaks to A, Your comfort with AI and be sort of the specific experiences you have that are particularly relevant for any job that's been posted. The like, oh, you know, in integrity, if we've posted a role, you know, fighting fraud. Well, if you fought fraud in your past, then like making that very explicitly clear is really helpful for us to figure out if you're the right fit.

**Aakash Gupta** (00:52:46)

Yeah. I mean, if you're hiring the best in the world, I imagine you guys are very focused on people who have functional and ideally some domain experience within our AI.

**Jake Brill** (00:52:56)

That's correct. You know, what I found is, at least for the folks that I've hired for the integrity team, the best candidates are. have a pretty well-rounded background. They do have familiarity with AI. They have worked in the specialist space, but many of the best folks also have worked in other spaces. And so they've got like a pretty broad horizon. They're not just, oh, to use that same example, I've only ever worked on fraud in my career. I've worked on fraud and I've worked on ads and I worked on... growth, things of that nature. The benefit of that is it means that you can think about problems from a lot of different perspectives, which is really important because we're dealing with a lot of ambiguous problems that have never been solved before. So having a pretty broad perspective is really helpful as you encounter these problems for the first time.

**Aakash Gupta** (00:53:41)

And I often coach people like if you want to make it to your dream company, think about going into the backgrounds that the company is hiring from. And if we look at the product team backgrounds at OpenAI, there's a ton of meta and Facebook presence there. So could an interesting strategy for somebody be to like kind of work their way through a big tech job? Would that help them eventually get a job at OpenAI?

**Jake Brill** (00:54:04)

It could, but it's not a guarantee and it's not a necessity. You know, one of the benefits of a fang type company is you're getting to work at incredible scale. You work with super talented people and you know that like they have a really high hiring bar. But we also find that people who've worked, people who are startup founders or have worked in hyper growth companies that aren't at the scale of fang companies. That's really helpful, too, because like. The pace of development, frankly, the fact that we sort of take pride in the fact that we're not process heavy. That's really important, too, for being successful at OpenAI because, yes, you can develop a lot of skills at these excellent companies. Certainly, I wouldn't be in the job I have now if not for my time at Facebook. But that alone is not going to mean that you're necessarily going to be able to be successful at OpenAI.

**Jake Brill** (00:55:00)

It's a wide range of skills that you will get both at large and smaller scale companies.

**Aakash Gupta** (00:55:04)

Yeah, there's probably thousands of PMs at meta and tens at OpenAI. So just by the math, you know, it's not a guarantee. But it's interesting then that there are certain backgrounds you've identified, though, whether it's hyper growth company or big tech that will help you for OpenAI's scale and culture.

**Jake Brill** (00:55:22)

Yeah, yeah. You know, there's no one size fits all. It is definitely the case that we have a number of Facebook and XFANG PMs at OpenAI, but we also have a ton of people who have not worked at those companies who are absolute rock stars. I mean, like, you know, you look at some of our product leads. Actually, if I think about our product leads off the top of my head, I think I might be the only one who's worked at Facebook. Okay. Yeah. So there's no one size fits all to be a successful PM at the company. For sure. So what was your story for breaking into OpenAI? Oh, man. I certainly wasn't expecting it. Instacart was an incredible experience. I'm so grateful. I got to work on fascinating problems. I got to work with brilliant people. And I have to say, the experience of being there during COVID is super unique.

**Jake Brill** (00:56:18)

And I am forever grateful I got to experience that firsthand, as intense and wild as it was. And so in 2023, you know, I had my like whole next couple of years planned out and it did not involve leaving Instacart. I had qualified for my recharge. My wife was about to qualify for hers at her gig and we were going to like time them up and take it together. And then I went on pat leave. My daughter was born in the spring of 2023 and I was a couple months into pat leave and when i got a message from a former colleague of mine from facebook we hadn't talked in years and he was in a new leadership position at open ai and i when i saw the message i was like oh my goodness what so great to hear from you and also like i'm flattered you you'd even think of me and i went into the call being like it'll be great to catch up with him and i'll sort of like hear what i say and i'll say thanks but no thanks and like great to see you and And I got off the call after 30 minutes.

**Jake Brill** (00:57:14)

I was like, oh, my goodness. This is kind of mind-blowing, the sort of stuff that we were talking about. And I reached out to a buddy of mine who was working in the sort of trust and safety space at the time at the company. We spoke for an hour. And I very vividly remember that night lying in bed. And my mind was racing. And I could not sleep. I had so many thoughts racing from my head. It was like... Wow. The scale of the problems, the sophistication of the problems that this company is trying to solve is mind blowing. The fact that this company is talking about safety so, so regularly in a way that they want it to be part of their brand and their products is really inspiring. Yeah. And like the fact that they even want to talk to me in the first place was like deeply flattering because it's open air.

**Jake Brill** (00:58:04)

They can talk to anyone, you know. And I remember maybe it was because my daughter had just been born. I was being very circumspect to like and thinking about being like this kind of feels like what I've been working towards my whole career. And. Like, what sort of world am I bringing my daughter into? And like, what role am I going to play in that world? And I did a lot of thinking. I was like, I think this is the most meaningful thing I can be doing with my time if I'm lucky enough to even have more conversations with the company. And so I spent a couple months in the summer of 23. You know, the shape of the job changed a couple of times. I think there were like three or four different hiring managers over the course of the process. And when they made the offer, I was like, yeah.

**Jake Brill** (00:58:44)

Yeah. Who am I to turn this down? So it was not something that was on my radar in the slightest. And it just so happened that, you know, someone thought of my name from having worked together years ago. But, you know, it was a very demanding interview process. And I think on some level, the fact that I was on pat leave really helped because I was either like... changing diapers or i was preparing for an interview and i did that for like two months and i i think that was really helpful for it ultimately turned turning out to be a higher decision on the company's behalf

**Aakash Gupta** (00:59:17)

oh wow two months of preparation and it sounds like you took this intensely like seriously i took it

**Jake Brill** (00:59:22)

very seriously because you know um as i said it sort of felt like i've been working my whole career to get to someplace like this dude you know i've I was never hired to be the first trust and safety PM at Facebook or Instacart. It just so happened that I ended up being the first trust and safety PMs of those companies, like opportunities presented themselves, the org changed in such a way that that ended up being the role I felt. And so this was the first time I was talking with a company and they were like, we'd actually explicitly like you to join for this job. And so I figured in joining in that context, I just really wanted to make sure I understood what are the types of problems the company was thinking about. And, you know, I was by no means an expert on this sort of like, what are the safety risks in AI models?

**Jake Brill** (01:00:05)

And so I just wanted to make sure I put my best foot forward for those conversations.

**Aakash Gupta** (01:00:10)

I think that's really important advice, though, for people. When you get those really awesome interview opportunities, really do everything you can. You may not be an exact expert in their industry, but you can be humble and learn also. So that's really, really inspiring. So you spent two months on it. If I were to reverse engineer, though, I think part of it is then that you had positioned yourself really well in your career to be that first Traced in Safety PM at Instacart and Facebook because they want to hire the best in the world. So you had that opportunity to create those career experiences. If you look back, what were the essential ingredients? Maybe we can go story by story that positioned you for those roles.

**Jake Brill** (01:00:49)

You know, I moved to San Francisco almost 20 years ago. It'll be 20 years next week. And if you had told me 20 years ago that this is what I'd be doing, that wouldn't have made any sense to me because I didn't study this stuff. I studied a small liberal arts college in the Northeast. I majored in psychology and Latin American studies. And when I graduated, what I wanted to do was go into the mental health field. And when I moved out here 20 years ago, It was to establish my residency so I could apply to get an advanced degree in psychology at a UC. And so I was like full steam ahead on psychology and mental health when I came out here. And the story of me getting to Facebook was basically I spent a couple of years working in the mental health space and had a quarter life crisis.

**Jake Brill** (01:01:36)

And I was like, I don't think it's the right thing for me. I'm like not super happy. I don't feel fulfilled in the way I thought I would. what am I going to do with myself? And it just so happened, I had some of my really good friends from my first couple of years living in San Francisco were in the customer support team at Facebook and they loved it. And I was a huge fan of the product. I had moved from the East Coast and left a lot of my best friends behind and Facebook was this lifeline to keeping in touch with them. And so when I went through the interview process, it was not because I knew I wanted, I didn't even know what a product manager was, but I thought, you know, Worst comes to worst, I do this for a little while and I realize, oh, actually, I do want to go back into mental health.

**Jake Brill** (01:02:18)

And this was a good way to, you know, just like the grass isn't always greener. And I ended up joining in customer support and it was like, you know, not a super glamorous job. My first year I was doing a lot of really like, you know, it was like changing people's passwords, approving their name changes, stuff like that. And towards the end of my first year, I ended up moving into a role leading our privacy team in support. And when we had our first phishing attacks on the site, our team was sort of at the front of the operational response. And when we created... The site integrity team at Facebook, we should show you a little bit of how long ago it was called site integrity because all Facebook had was a website at that point. And I applied for a role to be a project manager on the team.

**Jake Brill** (01:03:03)

But like, I didn't know what a project manager wasn't. Facebook certainly didn't. I was the first project manager at the company. And if I, you know, ultimately it was like. I worked hard my first year and I put myself in a position to be in a leadership role, but I never would have guessed it was like, oh, because there's going to be a phishing attack. I didn't even know what that was. And so when I moved into project management, I was sort of figuring out on the fly what I was doing. And for my first year, I don't think what I did was actual project management. I think it was like it was like coordinating our response to spam and malware and phishing attacks. And that had a lot of different shapes. And it was like, just do what's necessary. And that could be like training up some of our support counterparts and how to do certain workflows or like making sure like, you know, This engineer is working on this fire and this engineer is working on this fire.

**Jake Brill** (01:03:53)

Sometimes it was just like running command line scripts to clean up a bunch of bad stuff. And after about a year, it became clear that we had to stop being so reactive. We had to start building user facing products to help explain like, hey, your account got hacked. Here's what you do. And now I was like, oh, I think we need to start building products. But that wasn't my job and I didn't know how to do it. And I remember I was chatting with one of my counterparts and he gave me some of the best advice I ever got. and i haven't talked to him for years but dan levy if you're listening if this makes its way to you thank you for the advice i've given it to many other people and it was if there is a job that you're interested in and there is an opportunity to do that job even informally just start doing it and good things will happen and so i kind of in a de facto fashion just started being the product manager for the site integrity team and The products I built were of varying quality.

**Jake Brill** (01:04:50)

Some of them we turned off pretty quickly, and some of them are still there in some form. If you ever log in from somewhere suspicious and you get asked to verify your identity, you can blame me. I sort of built the first version of that for Facebook. Oh, cool. And I remember I'd been doing like de facto product management for a while when like a new lead for the integrity team joined. And I was like, hey, I've been doing this job. Like, can I like formally become a PM? And I remember having some conversations and the answer was like, Jake, we think you're smart, but like, you've never had any formal training or mentorship with this. Like, let's give you some of that before you actually transition to PM. And yeah, my ego was bruised a little bit, but like, boy, howdy, were those people correct?

**Jake Brill** (01:05:34)

And, you know, I learned a lot. I had two really important mentors, these two gentlemen named Dan Rubenstein and Arturo Behar, and they had like really invested in me, helped me learn a lot about product craft, strategic thinking, how to bring teams along with your vision. And, you know, by, you know, maybe like six, seven months later, I went through the interview process. And I think if I had gone through it when I originally wanted to, I would have just fallen flat on my face. But because I, I got more hands-on mentorship that set me up to be successful when I interviewed. And then when I interviewed and ultimately passed, I think I was the first person to ever transfer internally, interview and move over to PM at Facebook. And at that time, there may be like 30 PMs at the company. And so when I think about what put me in a position to move into PM there, it was a lot of just like rolling up my sleeves and doing what the business needed.

**Jake Brill** (01:06:24)

And then also being... open to coaching um and finding mentors who were really willing to invest in me and then learning from where i did well and where i didn't do well um yeah so that's that's my facebook story it was it was great but like i never would have guessed uh when i started facebook that it would ended up being a pm in the integrity space

**Aakash Gupta** (01:06:46)

Facebook's first internal product management hire. That's amazing. That was probably a lot much harder to do than the average move. So when we think about like taking on additional responsibilities, I think the first thing that probably people is popping into their head is like, but I'm already working 40, 50 hours a week. How do I take on additional responsibilities? What did that look like for you? Um,

**Jake Brill** (01:07:07)

it meant working more hours in some cases, but also like, you know, a huge part of being a PM and being a leader is like, figuring out what is the highest leverage thing for me to spend my time on? What is something that's really important, but you can delegate out to other people? And then what are some of the things that are important, but not urgent? And you sort of just like put them on the back burner. And you know, there's some amount of trial and error, but like, you know, at that point, it was really clear that even though it wasn't my job, we needed to start building user facing products. And so like, that was one of the more leveraged places for me to spend my time on. And so you know, as I mentioned before, it was like part of the way I've been spending my time was interfacing and training up some of my operational counterparts on sort of how to respond to the phishing attacks.

**Jake Brill** (01:07:54)

And then it became the, well, can either someone on the engineering side train them up or can we have a leader on the operational side sort of take over this responsibility?

**Aakash Gupta** (01:08:05)

Okay. So that's the Facebook story. What about Instacart?

**Jake Brill** (01:08:13)

So when I left Facebook, I was there for about 10 years and it was just like an incredible experience. But by the end of my time, you know, I was ready for something new and I left and I had this plan that I was going to take a couple months, plan a wedding. I just got engaged, you know, recharge and then start up working again. And Instacart wasn't on my radar then. But I ended up being out of work for two and a half years because a couple months into my time after Facebook, I suffered a very, very serious brain injury. And it took me about two years to recover from it. And thankfully, I found the right rehab program after a while. And I went through that rehab program. And when I got to the other side of it, I wasn't positive I was healthy enough to work again.

**Jake Brill** (01:08:58)

I hit all these milestones in terms of I can do things. I can read for this long before getting a headache, or I can drive for this long without getting a headache, or I can look at a screen for this long without getting a headache. But I still didn't know that I was ready to work again. But I figured, I think at this point, the best way to find out if... if I'm ready to work, is to get a job. And Instacart really resonated with me because I had had a firsthand experience of what it was like when I couldn't drive because I was part of my concussion recovery is I couldn't drive. And so all of a sudden I'm like, oh, I've taken for granted that you know, up until me having these health issues, I could just drive to the grocery store and drive home and then have everything I wanted.

**Jake Brill** (01:09:39)

And then for two years, I would literally walk to the closest Safeway and walk back with stuff. And I had this whole new empathy for what it was like for people who had mobility issues, either physical issues or they didn't have access to a car or public transportation. And You know, I remember my conversations with Instagram. I went and being like, how hard can this grocery delivery thing be? And I was like, oh, my God, it's so hard. It's like so complicated. And that was fascinating to me. And so when I joined, it was, you know, I was talking with a couple of companies and it was really important to me that I joined a company as an individual contributor because I was like, I don't know if I'm going to be healthy enough to do this job. And I don't feel comfortable. Like I need to.

**Jake Brill** (01:10:21)

be responsible for my own career i don't feel feel comfortable being responsible for supporting someone else's career success i have to really nail my own personal career success first and so when i joined instacart i joined as an ic working on sort of like shopper engagement products um and like very happily it turned out that i was in a good place health-wise and you know experienced some success there and After a period of time, I got offered an opportunity to move into a leadership position to build out a team that was focused on customer support and internal tooling. And I was super excited about that because there was a huge opportunity and because I started my career in support. So I had a particular passion for that. But the job changed a ton over the years. The mandate of the team grew a bunch, which was super exciting, especially during the days of COVID where like some of the things we were responsible for, it was...

**Jake Brill** (01:11:14)

customer support or shopper safety or fraud like those became really important when the company went from like a you know a niche delivery product to an essential service during a black swan pandemic so that was like that was just like such an incredible experience that I know for sure you know I wouldn't have gotten the open AI role and whatever version of success I've had at open AI I learned so much during my time at Instacart that's been really instrumental

**Aakash Gupta** (01:11:43)

Okay, so at Instacart, again, you weren't hired for trust and safety. How did you position yourself to be that first trust and safety PM? So

**Jake Brill** (01:11:54)

this is like, I still vividly remember the conversation where my edge counterpart and I sort of came to this conclusion. As I mentioned, I was moving into this new role where I was going to be building out a team focused on customer support and support tooling. And as we were wrapping up some of the work that our team had been doing in the shopper engagement space, my end counterpart and I took a step back and we were like, huh, we were building this to address some shopper feedback. i think a couple of the products we built were were actually like focused on shopper safety and and uh giving people tools to report fraud and we viewed it through an engagement lens but like that's actually trust and safety work and we looked around and we're like no one on the technical product side here is really like building out scaled systems and user-facing products for this stuff we were particularly operationally heavy and i'd gotten the company to that point in 2019 But we felt like that's probably not going to work long term.

**Jake Brill** (01:12:54)

You need to also have more sophisticated technical solutions. And so we made the case to leadership that like, hey, I know the purpose of the team was to just focus on support and tooling, but what if we expanded the mandate to also be responsible for trust and safety? I think for a number of reasons. People sort of got why it was important, as we made the case. Our operational counterparts were really eager to work. We had a positive experience working with them on those first couple of projects, and they were eager to have dedicated technical counterparts. And, you know, I think the fact that we'd had a couple of wins that we could point to, we had built some sort of confidence with leadership. And so when we made this case, it was actually a pretty straightforward conversation. People were supportive of it. And then it just so happened that that was incredibly fortuitous because fast forward three months, COVID-19 hits.

**Jake Brill** (01:13:45)

And as I mentioned, all of a sudden our customer support times ballooned to three and a half hours. And we had to get that down to minutes in very short order. We were sending shoppers. into public spaces um and we had to figure out ways to you know in product make sure that they were healthy that they were getting them ppe that we were uh helping them understand best practices about how to interact with their customers you know we certainly saw an increase in people stealing groceries during that time you know as often happens you know when a company goes through hyper growth The good usage grows fast and also the bad usage grows fast. And so there's a lot that we had to do to clamp down on that sort of fraudulent usage. And so it was one of those things where I couldn't have guessed it would have become that important that quickly.

**Jake Brill** (01:14:37)

But I do think we were on to something that we're like, well, it's going to become important at some time, so let's get in front of it.

**Aakash Gupta** (01:14:42)

Mm-hmm. And then the key, bringing this all back, right, was you had a former colleague reach out who is now working at OpenAI. And so part of it is that you are also just good at building a good reputation for yourself in your workplace. Are there any things you've learned over the years that help you do that? I

**Jake Brill** (01:15:02)

have to. One, I think one of the best ways you build a good reputation is you do the work. You build great products, you build impact. I think that's like some of the core currency of being a PM. But more so than that, I think people really get it when you care about them as individuals. Like this isn't just like, you're not just like a vehicle to build X, like you are a partner to work with on solving people's problems. And I think when you invest in relationships with people, they appreciate it. And I know I appreciate it when my colleagues really invest in getting to know me and care about me as a person. One, because that just means the vibes are good, but also that means that when we go through tough times, when we disagree or when, you know, like I screw up all the time and when I make a mistake, People don't think, oh, Jake, he's a bad person or Jake, he's incompetent.

**Jake Brill** (01:15:55)

It's like, oh, Jake's human. He's like not going to be perfect 100 percent of the time, but we have some trust. And like, I know that he's got my back and that, you know, he has proven that he's competent in his job. And I think that really lays a strong foundation for, you know, people wanting to work with you again.

**Aakash Gupta** (01:16:13)

Do good work plus build real connections. Yeah. Okay. So as I mentioned, I pulled my followers. I asked them what I should ask you. And we have to end on these topics because they're just so excited to hear your answer. What does the PM role look like in five years?

**Jake Brill** (01:16:33)

Um, I'll start with what I think looks different and then I'll sort of wrap with what I think looks the same. So we've talked about a couple of things that I think are going to be different. One, AI prototyping. Like this is a new world where we as PMs are empowered to not just use words to express the thoughts that we have, but also use code to express the thoughts that we have. And I think increasingly the role of a PM is going to be doing prototyping. You know, we're still going to be very important to have world class designers and engineers actually designing, building those products. But like coming up with a tangible version of like, here's what I think we could build. I think it's going to be a huge part of the job moving forward. Secondarily, I mentioned this before, evals, evals, evals.

**Jake Brill** (01:17:17)

I think that is something that PMs are uniquely well positioned to do because, you know, we, we are most well positioned to say, here's what the product needs to be good at. And here's how we know if the product is good at that. In terms of what I think is going to be the same, it's sort of along the lines of the last question you asked me, which is like the interpersonal part, you know, um, A question I get a lot is like, what do you look for most in PMs or what do you think is most important? And like my answer has been the same for the decade plus that I've been in the role as a PM, which is I think the most important skill that a PM can have and that like is going to be the case in five years is empathy.

**Jake Brill** (01:18:03)

Fundamentally, you are building products for people who are nothing like you. They may live in a different part of the world. They may be a different age, different gender. If you're just trying to build something for yourself and you don't know the people you're building for, you are just going to miss the mark completely. But I also call out empathy because I think it's such a critical part as a leader for a team. You're working with engineers, with designers, with people from comms, marketing, and data scientists, other PMs, and what motivates them, the way that they communicate. It's going to be different for everyone. And having that sort of context in having clarity of leadership and the deep ability to understand who a person is and how to help them do their best work. I think that is going to be even more important in the future as other parts of the job change and maybe go away.

**Aakash Gupta** (01:19:05)

Mm hmm. In the future, are PMs going to have to learn how to manage not just humans, but agents?

**Jake Brill** (01:19:11)

Absolutely. But I don't think that's just PMs. I think that's going to be a lot of the way jobs change in the future, is that absolutely you're going to be interacting with, managing, collaborating with other people. But I think that's very much the case with agents. And so there's going to be a new skill set that people need to develop in terms of how to give the best prompts to get the outcomes you want, what sort of... actions you're comfortable delegating to an agent versus you say, no, I want to be in the loop for this given action or decision. So I think agents, absolutely for PMs, but I think that's kind of where a lot of jobs are going to evolve over time as AI and agentic experiences become more common.

**Aakash Gupta** (01:19:55)

I could do 90 more minutes of questions, but this has been a masterclass. Jake, thank you so much. Thank you so much for having me. This was great. If people want to get in touch or learn more, where should they find you? Best place to find me is on LinkedIn.

**Jake Brill** (01:20:09)

My name is Jake Brill. I'm happy to chat with people. And again, thank you so much. I've really enjoyed our conversation.

**Aakash Gupta** (01:20:16)

All right. See you guys later. So if you want to learn more about how to shift to this way of working, check out our full conversation on Apple or Spotify podcasts. And if you want the actual documents that we showed, the tools and frameworks and public links, be sure to check out my newsletter post with all of the details. Finally, thank you so much for watching. It would really mean a lot if you could make sure you are subscribed on YouTube, following on Apple or Spotify podcasts, and leave us a review on those platforms that really helps grow the podcast and support our work so that we can do bigger and better productions i'll

**Jake Brill** (01:20:55)

see you in the next one
