---
title: "How to Build Frontier-Lab Quality Evals with Daniel McKinnon, ex-PM at Meta, Google"
subtitle: "He wrote evals for Gemini, for Llama, and for Ray-Ban Meta. Today he builds one from a blank spreadsheet, live! "
date: "2026-07-28"
host: "Aakash Gupta"
guests: ["Daniel McKinnon"]
speaker_names: "substack"
substack_url: "https://www.news.aakashg.com/p/how-to-build-your-first-eval"
youtube_url: "https://www.youtube.com/watch?v=ztN6bE_FuQQ"
duration: "00:56:56"
word_count: 9705
source: "Substack episode transcript (aired audio)"
---

# How to Build Frontier-Lab Quality Evals with Daniel McKinnon, ex-PM at Meta, Google

*He wrote evals for Gemini, for Llama, and for Ray-Ban Meta. Today he builds one from a blank spreadsheet, live! *

**Daniel McKinnon** (00:00:00)

The Metas and the Googles and all the other large companies have to reinvent themselves right now in the age of AI. Every single PM is going to start building AI features. You cannot exist as a PM without understanding this.

**Aakash Gupta** (00:00:13)

Meet Daniel McKinnon, former PM.

**Daniel McKinnon** (00:00:20)

PMs right now from a career perspective are in a really tough situation. The average PM is an orchestrator, a motivator, and an analyst, but a lot of this is easy to do with AI.

**Aakash Gupta** (00:00:30)

What really is the difference between product management at Meta versus Google?

**Daniel McKinnon** (00:00:33)

Meta is like a much, much more aggressive culture in many ways. Google is considered to be more of an engineering-led company, whereas Meta is more of a product-led company. If you're a PM who's never worked

**Aakash Gupta** (00:00:44)

on an AI feature before, when would you be going through this evals process?

**Daniel McKinnon** (00:00:48)

You work at Pinterest and you want to have a better image generation that doesn't look like slop that actually pleases users.

**Aakash Gupta** (00:00:53)

You need to think about from day zero, what does success look like? If it's the best way to measure it, we've got to learn it. Where should we start?

**Daniel McKinnon** (00:01:01)

Let me walk through

**Aakash Gupta** (00:01:06)

Before we get into today's show, please take a second to check that you're subscribed on YouTube and following on Apple and Spotify podcasts. If you want access to all of my favorite AI tools, I've gotten them to give you an entire year of their paid plans. Check out bundle.akashg.com for an entire year of Bolt.new, Airtable, Speechify, Descript, Magic Patterns, Linear, Dovetail, Arise, and Mobbin. And now into today's show. Welcome to the podcast.

**Daniel McKinnon** (00:01:39)

Yeah, thanks so much for having me and it'll be fun to talk about this stuff.

**Aakash Gupta** (00:01:43)

So I want to start with your article. You had this provocative claim and this funny meme here. Do evils replace the PRD? What is the role of evil?

**Daniel McKinnon** (00:01:52)

Yeah, so I think it was like a little bit spicy in saying it replaces the PRD because without a product strategy or a particular customer, like your product is nothing. But again, that's a paragraph or even a sentence, depending on what the product is. The majority of most PRDs that I've seen in my career Have spent most of the document talking about specifics, how it will work, how it will behave in certain situations, how the user can expect to get value from that. But that gets really turned on its head in this kind of Gen AI world where these products really need to do like Everything, or at least a lot more things than previous products. And it's very hard to describe that. Say, oh, this thing just does everything. And the best way to actually communicate what the product should do is through examples. And that's what an eval is.

**Daniel McKinnon** (00:02:42)

It's really just like a trivia question for the model. And it's saying, this is like the shape of the things the model needs to do well. And if the model does it well, it means it's getting these answers. And if it gets these answers, the users will probably like it. And if the users probably like it, let's ship it into prod and see if they actually like it with an online eval. But the key way to communicate how a product should work in this kind of Gen AI era is, is it performing well on an offline eval? And if not, you either need to change the model, change the harness, or change the product. It's possible that what you want to do is not possible with the models today, but it's better to find that out early with an offline eval versus just shipping it to prod and getting frustrated users.

**Aakash Gupta** (00:03:22)

And for people who don't quite understand that nuance, what's an offline eval versus just shipping to broad and looking at them?

**Daniel McKinnon** (00:03:29)

Yeah, this is a really, really important nuance. And I touched on it in this blog post. But when we usually talk about evals in this AI world, it's something that's run offline. There's like a little bit of gray areas in terms of our environments and stuff. Think about it as like a pre-baked set of trivia questions that you ask the model. So for example, let's say you have a recipes website and you want to tell users how to make their favorite kinds of ice cream. An offline eval would be a prompt set, say 100 prompts of different ice creams that users might like. And the answer key would be a correct answer or a plausibly correct answer with a way to score whether it's good. That's run offline during the development of your product. And you use that as a proxy for real user traffic. Once you do well on your offline evals, you can ship that product online and you have a website and it lets users generate ice cream recipes.

**Daniel McKinnon** (00:04:26)

And you think because you are a good PM and you really thought deeply about what the customer wanted, that performance on that offline eval set will reflect the satisfaction of the user in the online eval. This obviously doesn't always happen, but that's the idea. And it's the best way to measure whether a Gen AI product is likely to satisfy users.

**Aakash Gupta** (00:04:48)

If it's the best way to measure it, we've got to learn it. Where should we start?

**Daniel McKinnon** (00:04:52)

Let me walk through what's changed since I wrote that article. So the key thesis has remained true. And this has been now two years in that an eval is the best way to communicate what your product should be doing and to Explain to the engineering team working on making the product work what success looks like. This can be very, very challenging in an AI world when these products do so many different things that it's hard to necessarily understand what good is. But things have gotten a lot more complex. So back in the day, evals were really simple. My blog post basically just covers these simple evals. They were question and answer. And this seems crazy to think back two years about what these models looked like and what the use cases were like. But this is before Claude code and agentic coding and all of these crazy business applications that are getting built right now, Claude co-work and the like.

**Daniel McKinnon** (00:05:52)

Really the core thesis two years ago was that Gen.ai was essentially a search replacement. I don't know if everyone remembers when Google's stock tanked because this was going to be the replacement for search. And fundamentally, these were like question and answer products. So what I have right now is the benchmarks that OpenAI reported on GPT-4. And you might remember a lot of these. MMLU, HellaSwag, Arc, Winograd, HumanEval. HumanEval is ironically an automated eval of Python. Drop. These are all just question and answers. So I dropped one example here from MMLU. If you know the actual brightness of an object and its apparent brightness from your location, then with no information, you can estimate A, speed relative to U, B, composition, C, size, D, distance. And if you want to go ahead and look at some of these just for like historical fun, they're all on Hugging Face.

**Daniel McKinnon** (00:06:46)

So this was actually a very, very straightforward thing to do is you had to think about the types of questions users would ask and the types of answers they would expect and how to score that. So the key thing was just matching the questions to the domain of interest and scoring the answers. So if we go back into my post here, we can see a little bit how I said to do this and First thing is just figure out your problem and it doesn't need to be perfect. What is a set of problems that your users might ask about? So the example I used was, for example, generating recipes for videos. I have food on my mind because I randomly came up with the ice cream example earlier. And new problem is I have a video on my social media site and I want to be able to generate a recipe that somebody can use to make that thing as they're walking the video.

**Daniel McKinnon** (00:07:40)

And you say, okay, this is really well-defined. And now you have to measure how do you know if it's good? You know, it might be formatted right. It might have all the ingredients listed. It might be written in the right style. And then you select all of these components and figure Once you have that, it's really a mechanical process to actually write the eval. Come up with probably 100 prompts that are in this distribution. Can be less, can be more, but this is a typical size of an eval in the Gen AI world. And just send it through the model and figure out what is a hard prompt, what is an easy prompt, and have something that scores maybe Maybe like 50% because you have to have room to run. If you create a very easy eval that scores 100%, there's no way for your engineering team to optimize on that.

**Daniel McKinnon** (00:08:33)

And if you create a very hard eval that scores 0%, you also don't even know if this is kind of possible with today's technologies. And that's pretty much it. And once you have this, you can give it to the team. They can improve on it. You can ship it out to users. If you achieve a score high enough, you can see if you're actually online Performance matches what you expect to do offline. And then this blog has a bunch of examples of like, you know, some kind of other nice tips. Why is this not that relevant today? Or why does it need to change today? The real answer is that models have generally saturated QA. This isn't 100% true, but when we think of a good model right now, we don't think of one that can answer a relatively challenging high school physics question, like the example I gave above.

**Daniel McKinnon** (00:09:24)

We think of models that are like winning gold medals at International Math Olympiads. Like there's almost no question that any human beyond some super, super specialist can ask the model to do and it not have a good answer back. And also, QA is not the most useful application now. I mean, I think we all remember this narrative that ChatGPT was going to be the next great consumer app and they were going to get all these users and it's QA and you're answering all these problems and, you know, Google did a generative search experience. But if you look at all the headlines in Gen AI right now, it's not QA, it's agents. And this is actually reflected with how the labs communicate progress.

<!-- sponsor -->
**Aakash Gupta** (00:10:05)

Here's a quick word from our sponsors. If you're building anything that uses live data from the web, eventually you hit the same wall. An agent, a research tool, a trends dashboard. They all need fresh data. Scraping that data is the worst part. Captchas, proxy, layouts that change every week. It's a whole side project you didn't sign up for. That's where SERP API comes in. SERP API gives you clean, structured results from Google, YouTube, Bing, Google News, Google Scholar, and more. One API call, one clean JSON response. They handle the captchas, proxies, and layout changes for you. Take the Google Scholar API as one example. Say you're building a research assistant or pulling sources for a literature review. You hit one endpoint. You get peer-reviewed articles back. With full text or metadata, titles, links, publications, citation info, all of it. Across publishers and formats. No scraping a dozen publisher sites and gluing the data together yourself.

**Aakash Gupta** (00:11:04)

The same idea extends across the rest of Are you looking to up your AI product management chops? I highly recommend the AI product management certification by product faculty. It has a 4.7 with 1,249 reviews on Maven for a reason. I myself took the course back in 2024 and it was awesome. Since then, they have upgraded it. So now you get to learn from product leaders at OpenAI and Anthropic. On top of that, Paul Hearn, author of the Product Compass, leads the Build Labs. So you will go from theoretical knowledge about AIPM to a very practical course. It's going to help you identify AI leverage opportunities. It's going to help you design trustworthy AI experience. It's going to help you systematically optimize outputs for accuracy and relevance, build rigorous evaluation suites, architect AI agentic systems that work, and select the perfect LLM for your use case. It's normally $2,500, but you get a discount when you use my link.

**Aakash Gupta** (00:12:21)

The next cohort starts June 22nd and goes to August 9th, so do check it out with my link in the description. They have been one of my longest sponsors for a reason. I trust this product and I think you should consider the cohort.

**Daniel McKinnon** (00:12:33)

So back here two years ago, if you look at how OpenAI communicated progress, it was these five evals, I guess six evals, If we fast forward to look at how Anthropic communicated progress for Opus 4.8, you can see they're using entirely different benchmarks. You don't see any continuity. It's partially because those evals are saturated and Opus 4.8 would score effectively 100% on all of them, but it's partially because the task is really different. You'll notice we have agentic coding, agentic terminal coding, Multidisciplinary reasoning, this is actually some agentic reasoning, agentic computer use, knowledge work, this is actually agentic knowledge work and agentic financial analysis. All this means is what the core model task is, is no longer to get a prompt from a user and come back with an answer, But it is actually to get a task from a user that requires many, many steps.

**Daniel McKinnon** (00:13:35)

Some of these steps might involve just thinking, which is called reasoning in this world. Some of it might involve tool calling, something like search. Some of it might involve more advanced tool calling, like something we'll go over today. And this is a totally new paradigm of writing evals because you're no longer thinking about QA, you're thinking about tasks. Fortunately for us, the framework is largely the same. We still have to define the problem, We still have to be good PMs and know what we're solving. We still have to collect representative prompts. I call this Goldilocks style. Again, they can't be too hard and it can't be too easy. There has to be some room to run. A typical good eval will have something like 25%, 50% success rate. And then over months that will go to 100% and then you'll have to throw it away and create a new one that is harder.

**Daniel McKinnon** (00:14:22)

And then you also have to figure out how to score. One thing that's changed is QA is relatively easy to score with humans worst case scenario. There's exceptions to this. Of course, the reason these models are so bad at things like creative writing is because it's hard to score and there's different preferences and different users like different things and why they're so good at math and coding is there is like some right answer and this is much easier to hill climb. For, to some extent, QA-style questions, you can ask human raters to review worst-case scenario if you can't find a better way to score it. With agentic work, it's much more challenging because the time horizon tends to be very long, and the final output is a collection of many, many, many steps that it took. Some steps could be correct and lead to the wrong outcome.

**Daniel McKinnon** (00:15:11)

Some steps could not be correct. And it's just from a labor perspective and a... Like defining success perspective, it's much, much more important to get something that can be automatically scored to make more of these rollouts and understand how you can do more experiments. But again, it's largely the same and the tasks are much longer time horizon. The goal of this podcast is to walk the audience through creating an actual agentic eval in real time. I want to caveat this. This is a little bit pre-baked. It is unrealistic in 45 minutes to come up with a brand new eval. This is kind of like a week's or month's problem of deep thinking, but we're going to kind of pretend and we'll go through some of the steps together. First problem. I want to measure and improve the model's ability to help with clinical genomics. This is a problem that I care deeply about.

**Daniel McKinnon** (00:16:06)

It's one that I think can improve the world and it's something that I've launched a new startup to solve. And the problem is, is that whole genome sequencing has Become the absolute gold standard in diagnostics in NICU settings, so for sick babies. Unfortunately, interpreting the results of a whole genome sequence is very labor intensive. And it limits access to this life-saving technology. So I wanted to see if I could distill some of this human expertise into a model to help broaden the accessibility of this technology. So first thing is like before, We have to deeply understand the problem. And I'm not going over these flow sheets, but this is just kind of how complex this is. Generally, you start with the raw reads off the sequencer. You do a lot of processing work to identify how the particular patient differs from the reference human genome. And then you do another set of work to determine whether those changes to the genome matter.

**Daniel McKinnon** (00:17:20)

For example, if my genome were sequenced, I would get about a billion reads that are 150 base pairs long. They would come out in a giant text file, and I would need to transform that into a diagnosis that says that this gene may or may not be responsible. So I'm not going to spend too much time on this here because we're going to go over some real examples, but you really need to deeply understand the problem. This is why people like Anthropic and OpenAI are hiring Investment bankers, accountants, lawyers, you see job ads for all these vertical specific teams, you must deeply understand the problem. You will unlikely be successful in creating an eval for some topic if you don't have some background in it or haven't really educated yourself on it. So then let's say we've understood the problem. I think I understand this problem pretty well and by the end of this podcast you will too.

**Daniel McKinnon** (00:18:14)

Let's go to the prompts. So Again, we want to find this like Goldilocks set of prompts. So the first thing I like to do is just start with something easy. So you want to make sure the model can actually do this. And when I say the model for agentic stuff, I'm usually talking about the model plus the harness. So I'll use those words interchangeably, but this is a frontier model harnessed in a way that it can use these tools and it can do this reasoning and it could come back with a solution. So for this problem of genome interpretation, I picked like one of the easiest genetic diseases possible and this is cystic fibrosis. This was something that we have known the genetic cause for quite some time and there are like canonical genes that cause cystic fibrosis. So to save you the effort of me Googling for this, I just had the link right here and let's just go ahead and look at this.

**Daniel McKinnon** (00:19:11)

So what we see here is The canonical cystic fibrosis mutation in ClinVar, which is an NIH database for a lot of genetic disease. And what we see here is it's got four stars and three stars. This really should be four and four. So I'm going to make sure that my agent can actually get this before I go forward. And so this is like the easy thing to start. So we're going to have our agentic genetics eval, and we're going to say gene, and we're going to say CFTR2. This is the, again, canonical gene. And then we'll say variant. And what a variant is, is how a particular gene is mutated. So right here, this is, again, this is a somewhat niche eval, but what this is saying is that on this particular transcript of CFTR, at this position, there is one base deleted. And what that results in is the 508th Phenylalanine deleted.

**Daniel McKinnon** (00:20:24)

So this is the actual variant that's going to exist in our eval. Sounds good. Okay. So what we see is that this is the exact variant that we care about. And what you'll notice is this is like very complex and new So this kind of comes back to the absolute first point I was making is you really need to know the space to do these evals. A lot of the evals are kind of like picked up. Like if you're trying to come up with an eval for Python coding, like many of these are pretty good now. And for any of you who have used these models, saying Python coding is a solved problem is a little bit of a strong statement, but it is a very, very well understood and well characterized problem. So we will go to this and we're going to say, okay, so this is the thing we want to know.

**Daniel McKinnon** (00:21:11)

And I should add a column here. And this is the phenotype is cystic fibrosis. So what you see here is I'm starting to build a table of question and answer. So the question is I have this phenotype of cystic fibrosis, which is a lung disease. And, you know, we'll describe exactly what happens there. And then we have the genome of this patient. And then we have the answer, which is this variant. So let's walk through like how we would do that. And when you're constructing these evals, you're going to really, really, really use Gen AI a lot to construct them. What I'm going to do is now I'm going to go over to a terminal window I have open here and I'm using Codex. Any of the tools will work. I have it on 5.3 Spark low because I want it to be fast for this demonstration.

**Daniel McKinnon** (00:22:02)

But, you know, you can use any model, anything you like. And for this task, this will be fine. So what I have here, and I pre-baked some of these just to kind of make it go faster, but I want to walk through any step anyway, is I have actually two files here that are representing my genome. And what I want to do is create a synthetic version of this genome that has these variants that have the question and answer through this agentic flow that I want to get at. So what I'm going to do is I'm going to say, please add And then this is going to be this variant two. And this is a small variant. So it's going to come through here and create a new file in a new folder. And we're going to call this dancflive.vcf.gz. And we're going to have this be And we're actually asking AI to help us create the eval for AI.

**Daniel McKinnon** (00:23:13)

So we're going to do this. And what the model is going to do is a variance file is literally just a text file. Actually, we can see what it looks like here, just for fun. So while this is running, let's just take a look just so we know what these variant files look like. And this is fine. We don't need to show all of it. But what we basically see here is a chromosome. So you might remember from things like 23andMe, we have 23 chromosomes. So this is one. This is the biggest one. And this is a position. So your chromosomes have different number of bases. You might remember we have like 3 billion bases in our genome. And then these are swaps. So what we see is in this position, a reference human has C, and I have a CA here. So that means that during something I inherited from my parents or maybe something that emerged during my development, I got a base swap here.

**Daniel McKinnon** (00:24:12)

And then there's a bunch of metrics around quality, how real it is. You might remember you have two copies of each gene, so this is actually heterozygous, meaning only one copy is impacted. You know, really, it's just a text file of all the letters in your alphabet. And what I'm saying is I want to add, okay, this is still running, and if this is still running in a while, I'll just use the pre-baked one, is I just want to add this particular variant into my genome to see if our system can catch it. And... This is what Codex is doing right now. And I actually don't know why this is taking so long because this is like a one-liner.

**Aakash Gupta** (00:24:55)

Line the line, I think.

**Daniel McKinnon** (00:24:56)

Yeah, yeah, right, right. I guess I probably, I didn't want to make this demo too pre-baked. I thought about it. Should I just have a Python program that just does all this for you? But then I'm like, that would not help the users at all because when they're constructing their own, they wouldn't know how to do it. So just believe me that this will work. And for the sake of time, we'll go to the pre-baked ones. So basically what's going to happen is that codex is going to add, this is in chromosome, where is it? I'm actually not sure. But in whatever chromosome this cystic fibrosis gene is in, it's just going to add one row. And it's going to say, we're going to have a deletion. So instead of having like CA here, It'll just have a C. So like here's a deletion. You'll notice that we've lost an A.

**Daniel McKinnon** (00:25:42)

We went from TA to T. And then it's going to have a fake cystic fibrosis patient. So now let's just check to see how this works. And we'll say, use our agent. And again, these are all agentic evals. And I'm using Codex as our agent, but you could use anything, Klein, OpenCode, ClaudeCode, your custom harness, any way you could. To get these agents to actually operate. And in fact, even ChatGPT and Claude, actually in the web UI, they use agents right now. They're not just model in, model out. They're model in, reasoning, tools, everything. Okay, cool. All right, so the agent finished here. So we see we added this in a record. Okay, and we see here it is. It's in chromosome seven. And you'll notice this is deletion. It says TCTT and instead it's a T. And so this means that this is like the canonical CF.

**Daniel McKinnon** (00:26:34)

So we're going to see if our agent is able to do it. And we're actually going to try a few different agents because one thing I mentioned is you want to score like, you know, 25 to 50% on these evals. You have to think about what tool are you using the, you know, Mythos 5 for some biodefense thing, then it's got to be really, really hard. Or maybe this is something that for infrastructure reasons or cost reasons, you need to use a very small model. You need to use haiku or something like that. So we're actually going to try these simultaneously on a few agents and see what happens. So we're going to say inside, what was this file we had? DanCFLive. Again, this is the one that we just made.

**Aakash Gupta** (00:27:17)

Hmm.

**Daniel McKinnon** (00:27:22)

We have the genome of a patient suffering from, and let's just very quickly copy and paste some cystic fibrosis symptoms. This one. We suspect cystic fibrosis. Please find a genetic cause. And then we are going to, we're actually going to copy this prompt so we can use it across multiple agents. So now we're going and we're checking GPT 3.5 codec sparklow. We have a few other tabs open. So I mentioned, you know, maybe... We want to actually see if Haiku can do this. So we'll just upload this. And again, we're going to the CF Live. And let's also try CatGPT 5.5 extra high. And I'm not going to use Pro because it will take too long. And this is also a relatively easy task. I suspect all the agents will get them. Okay, great. So we are cooking with And we are cooking with, you can see what's already happened with our first agent is after one minute of thinking, you've actually find the CFTR mutation pattern consistent with this deletion, right?

**Daniel McKinnon** (00:28:43)

This is the canonical cystic fibrosis gene. So what this is telling us, going back to our steps, is this task is not too hard for these agents, at least in the easy case. Especially not with a powerful system like Codex. We'll see if Haiku gets it. I suspect Haiku will also get it. But you can see Haiku even itself knows the CFTR region is important. So while that's cooking, let's go back to our next step. So again, we start with something easy just to make sure it's possible. I knew that this was possible, but if you just told a layman and say, hey, could... Quick thought experiment for you. Is there anything in this video you should be trying on your own? If there is, try it, take a screenshot, post it on LinkedIn or X, and tag me. I'd love to see what you're learning.

**Daniel McKinnon** (00:29:32)

Now a quick word from our sponsors before we get into the back half of the pod.

**Aakash Gupta** (00:29:51)

If you've worked at any company bigger than 30 people, you know this one. The CEO sets strategy. By the time it reaches the people actually doing the work, it goes through three or four layers of translation. Half of it gets lost and nobody finds out until the quarter is over. That's the problem Mariso is built for. AI operating partner for every manager and team. It connects to where work actually happens, the meetings, the messages, the docs, and it turns all that fragmented activity into a clear picture of execution. Managers get real coaching grounded in their team's actual work, not generic advice. Teams stay aligned with strategy as it changes, not as it was last quarter. And leaders see where execution is drifting in weeks. Not in the postmortem. One shared memory for the whole org. Everyone finally working from the same picture. If you lead a team, check out ariso.ai slash akash.

**Aakash Gupta** (00:30:37)

That's A-R-I-S-O dot A-I slash A-A-K-A-S-H. I want to take a second to talk to you about the fourth cohort of LAN PM job. I trained 30 students in cohort one, 50 students in cohort two, and 75 students in cohort three. And I am bringing back a program for cohort four. It starts in August and it lasts Three months where you're going to have intense sessions, a Monday morning session where I go over your resume, behavioral interviews, LinkedIn. On top of that, Bart Jaworski is going to be teaching you the PM fundamentals in 2026, how to write AI PRDs, how to AI prototype with cloud code, all of the key skills you need to freshen up your knowledge for this market. And Ankit Vermani is going to be teaching you AI product management. He is an AI product manager at Uber, and he is going to teach you how to build AI features that actually work successfully.

<!-- sponsor -->
**Aakash Gupta** (00:31:26)

On top of that, Prasad Reddy is going to be doing one-on-ones with you for market reviews, LinkedIn review, candidate market fit review. So it is a full package. It is three courses in one for one low fee. So join at landpmjob.com. Today's podcast is brought to you by Pendo, the leading software experience management platform. McKinsey found that 78% of companies are using Gen AI, but just as many have reported no bottom line improvements. So how do you know if your AI agents are actually working? Are they giving users the wrong answers, creating more work instead of less, improving retention, or hurting it? When your software data and AI data are disconnected, you can't answer these questions. But when you bring all your usage data together in one place, you can see what users do before, during, and after they use AI. Showing you when agents work, how they help you grow, and when to prioritize on your roadmap.

**Aakash Gupta** (00:32:16)

Pendo Agent Analytics is the only solution built to do this for product teams. Start measuring your AI's performance with Agent Analytics at pendo.io slash akash. That's p-e-n-d-o dot i-o slash a-a-k-a-s-h.

**Daniel McKinnon** (00:32:29)

But then if you know that the easy thing works and we already have early evidence that easy things works, you have to establish the ceiling. Is the hard thing working? Because if it's just totally saturated, then what's the point of even having eval? This task is already solved. So I'm going to show off something that's pretty hard to do today. What we have here is a recent paper, so this is from last year, and I will make this bigger. The authors here are deciphering the digenic architecture of congenital heart disease. So what does this mean? This means congenital heart disease is if you're a baby and you're born with problems with your heart, and digenic means it involves two genes. So single gene, single variant genetic diseases are actually sometimes a solved problem. Like with cystic fibrosis, not all cases, but many cases like this one are totally understand.

**Daniel McKinnon** (00:33:32)

Digenic genetic diseases are like a very, very new thing that people are studying. So this is like a very hard task to do. And even though this is published, And in theory, an agent should be able to search the internet and find every publication and deeply understand all of this. It's actually not that simple. They're not perfect and they actually need a lot of guidance, which is why there A lot of these companies, including my own, that are called like harness engineering companies or vertical AI companies or agentic AI companies because you need some specialized capability to be able to have the LLMs do stuff like this. So let's briefly return to our agents and let's just make sure they got it. Okay, so Codex with GPT 5.3 says, okay, this, if you recall, this is the deletion that we added. Boom, I gave it the phenotype.

**Daniel McKinnon** (00:34:25)

I gave it the genome. This is correct. So how would we mark this correct? We would actually probably have another LLM. I'm not going to do this right now for the sake of time. Just compare my scorecard. This is the correct answer with the response the model is giving right here. And then we can check haiku and even haiku. Oh, wait, did haiku not get this? Okay, so this is interesting. This is actually... It's harder than I would have thought. I would have expected Haiku to get this because this problem is so easy. But you'll notice what Haiku says is there's 48 variants spanning the gene. So it's looking at the gene, but it fails to actually find the particular, oh, this is so interesting. Hallucinates a hemizygous large deletion. So coming back to this, coming back to our point is start with something easy. I thought I started with something easy here.

**Daniel McKinnon** (00:35:21)

It's a good thing I did this because if I were benchmarking high Q, this is too hard and I'd have to make it even easier. And the things I could do to make it even easier would be potentially, you know, limit the region of the genome of interest, give it more hints, maybe Provide access to more external information more easily, but we can see that Haiku even fails this easy task. And I would be absolutely shocked if 5.5 did. Okay. It's not finished yet, but you can already see that it found the correct answer. So if we were to score this, we could easily have an LLM say, okay, haiku, this is not correct. This does not match what I have in this table. This is correct. And this is correct. So that's kind of, and then in our spreadsheet, we would just say, you know, haiku, bad, others, good.

**Daniel McKinnon** (00:36:11)

But now let's move on to something where we want to understand the hard cases. And again, I unexpectedly actually picked out a hard case for haiku, but this paper is quite challenging. And I believe it is unlikely that any of the models will solve this. So in the supplementary information of this paper is a table, and it is a list of patients, and a proband is a medical This is a clinical term for the patient you're evaluating, and it has diagenic causes for congenital heart disease. So this particular patient has ACACB, I have no idea what this is, some gene, it's HET, This is one copy of this variant and myocd, which is also one copy. And these researchers discovered that the combination of these two diseases leads to congenital heart disease. So let's see if the models can figure this out. So what we'll do again is we'll go to our table and our phenotype.

**Aakash Gupta** (00:37:14)

Is it two diseases or is it two abnormalities in their DNA?

**Daniel McKinnon** (00:37:19)

Yeah, that's a great question. It's one disease. It's a congenital heart disease. And I don't know exactly which one it is from this paper. And, you know, we could read the paper and figure out exactly what the phenotype is, but it's some defect with the heart. And what's unusual about this and why this is hard is it's two heterozygous variants on two different genes that is causing this single disease. So it's complicated. So Our phenotype here is congenital heart disease. And our gene here, we have two of them. One is this guy. And oops. And the second one is this guy. And then the variants are these guys. And this is, you'll notice the notation is a little bit different, but this is something that you'll just have to deal with in these evals is like, You know, no matter what you're doing, because these tend to be in very technical, specialized domains at this point, you know, no one wants evals for boring stuff like ice cream flavors.

**Daniel McKinnon** (00:38:16)

You just have to get comfortable with all these different mutations. And now let's go and let's try this again. So what I would do is I would say something like, please add these to den.d variant.d. VCF. But I'm actually not going to do this because you already saw how this worked and basically how the VCF file was structured. It would add these two rows. And for the sake of time, I've already done it. But then let's go and let's check and see, oh, how do we do on this use case? So in this case, I've already pre-baked it. And I'm going to say this is danchd. And I'll say this contains the... Genome of a patient with congenital heart disease, please identify the genetic cause.

**Aakash Gupta** (00:39:17)

Okay.

**Daniel McKinnon** (00:39:18)

And while we're going to have this one running, we're going to try our other two agents just to see how they do. We can almost guarantee that haiku... We'll not get this because it didn't get the much, much easier task. But for the sake of completion, completeness, we'll do this as well. And then we'll do this with GPT 5.5 extra high as well.

**Aakash Gupta** (00:39:51)

And again, we would do probably like some non-deterministic nature, right? Like, do you need to like test the same model a couple of times to just see if like maybe two out of three times it gets it right? Or is that not important?

**Daniel McKinnon** (00:40:02)

Yeah, that's a really good point. So this is a question about sampling. So sampling is actually really important. And you might remember like all of this old research where You would basically sample for good traces. And this is kind of what like RL environments do is you do a rollout, you do a rollout, you do a rollout, and then you get the correct answer and boom, you give it a good reward for that. And the key thesis here is inside the weights of the model, the right answer might live there. It just might not get the right answer each time. So when you're doing these evals, you do want to try multiple times. In this particular case, I actually know from having done it that sampling has very little effect and it's essentially determining I've seen slightly the same model get to the same conclusion with slightly different approaches.

**Daniel McKinnon** (00:40:58)

But in general, sampling, in my experience, is less important than it used to be, where sampling used to be a big deal. Like if you look at, let's just look at, this is a funny story. Let's look at Gemini Ultra scorecard. So if you'll remember, Gemini Ultra, oh wow, did Google actually bury it? Okay, here it is. So you'll remember way back in 2023 when people thought Google was kind of out of the AI race. I actually worked on this model, so I know this story very well. Google released Gemini Ultra, which I believe was a 660B dense model, which was crazy back then. That was like one of the largest dense models ever trained. And they released this scorecard. And what you see is this. This was very controversial. And this comes back to your question about sampling. If you remember, MMLU, this used to be like the canonical benchmark for LLMs.

**Daniel McKinnon** (00:42:00)

And let's just go back to look at what a question is to remind you is... Just simple question and answer. If you know the actual brightness of an object, it's apparent brightness from location with no other information you can estimate this, okay? Models used to be bad at this, which is hilarious because this seems so distant right now. And Google wanted to be the best. And GPT-4 was the best at this point. It got 86.4% on MLMU and it was on five shots, meaning it had five samples and it picked the best one. And that's why you see five shot, three shot, three shot, 10 shot. It really is like kind of like a way of cheating is like how many times can you sample from this model? And what you see is that Gemini Ultra actually had 32 shots. So they got more shots on goal.

**Daniel McKinnon** (00:42:46)

And actually, now that I'm remembering this, this actually might be pre-examples, If this is actually not the number of examples in the context window and just the shots or the number of times sampled, it doesn't really matter for the sake of this argument. But the answers to MMLU might be inside the model weights, but it might just be not enriched enough in terms of the probabilities. So by sampling more times, you actually get a higher chance of getting the correct answer. So this used to be a really big thing back in the day. Today, I don't think this is a big thing. The labs don't really publish anymore. I don't think there's a lot known about this. In my personal experience, I've not found that running the same prompt through the model multiple times generates different answers. In fact, I don't know if I've ever seen that for this task, but it's a really, really good thing to do and you should test for your use case.

**Daniel McKinnon** (00:43:34)

Little side conversation while we look at the answers. And we've got all these cooking. These are all cooking. And we can see that 5.3 Spark finished first. This is actually why we did it. And what you'll notice is it's totally wrong. They found multiple variants, tbx1, myhsys, jag1. You'll notice these aren't even genes of interest for us. These variants aren't even relevant. No high confidence variants. So what we've done here is we've done the second step. In our process is we've established the floor. We found something easy, that cystic fibrosis gene. Now we found the ceiling is this model didn't get it and plot twist, no model on the planet gets this without like a very, very strong harness. Again, I'm working on that very strong harness. So, you know, we can make systems get this, but this is hard. And then you just kind of go through and it's almost like a binary search process.

**Daniel McKinnon** (00:44:30)

Process where you say easy, medium, hard, and then just assemble a list of prompts. You know, you might have a hundred of these, which again would be phenotype gene, phenotype gene, phenotype gene, and then you understand how the models do on it. And then you're done. And then you have your eval. And then you understand what is good enough to actually ship product. So if you're scoring 50%, is that good enough to ship your product? Probably not. So then you look at which phenotypes am I better at? Maybe you put guardrails on the product to make sure that Only will answer the types of questions that it can get 80% on or something like that. That's a product decision. That's a product manager's decision to do that. And then you also hand all the hard ones to the research team and you say, hey, guys, you didn't get this.

**Daniel McKinnon** (00:45:17)

Fix the model or fix the harness and make sure that it can get these in the future so I can ship a product with these capabilities. Not shockingly, haiku is totally off base. Clearly, haiku is not good at all at this task. So that's surprising. It's the first one. Not surprising. It's this one. And we, again... We have, oh my God, okay, this is so interesting. Okay, so this is actually a good example of something that came out and sampled a second time and worked because I actually tried this. We were just talking about sampling, but we can see right now that GPT 5.5 extra high this time actually did identify this diagenic pairs and it did almost certainly find the paper. Yeah, so it did find the paper with all these diagenic pairs. So this is actually a very interesting reasoning trace where it was able to turn this congenital heart defect Phenotype into a search for a very specific paper and then pull out the results from this paper.

**Daniel McKinnon** (00:46:24)

So actually, this is quite impressive from GPT 5.5, but this is correct. So in this case, I would have to find an even harder one if I were benchmarking this model in particular. But this is basically... The key set of steps, and I don't think we have time to do a bunch more, but it's basically running through all the different types of scenarios and then coming up with prompts that will challenge the model, but not totally stump the model. So yeah, with that, that's how you write an agentic eval. And here's two lines in our new one. Wow.

**Aakash Gupta** (00:47:01)

So it's just a spreadsheet. And the key thing here is the domain subject matter expertise. It's not like how it's written or anything like that. You're not giving us an eval template like we might have given people a PRD template before. It's really the subject matter expertise that's driving all of this.

**Daniel McKinnon** (00:47:20)

Yeah, exactly. There are a lot of companies over the last, you know, N years who have tried to build better tools for evals. And I'm not saying that tools for evals don't need to exist. There's plenty of ways to improve. But when you're creating evals like this, it is literally just prompts, responses, and ways of scoring whether response is correct.

**Aakash Gupta** (00:47:43)

Fascinating. So just to bring it all back full circle, if you're a PM who's never worked on an AI feature before, when would you be going through this evals process and when wouldn't you and how would you be using it?

**Daniel McKinnon** (00:47:53)

Yeah, that's a good question. So if you've never worked on an AI feature before, I would actually try to find somebody who has, who can help you through this. This is deceptively simple. I made this really simple because we had 45 minutes today. But And I don't know why it's so complex. Honestly, I had many, many conversations with people about how to build evals, but there's just something kind of like taste-based or nuanced about how to build them. And, you know, it is what it is, but find somebody who can help you. But I would say you start from the beginning. It's like, you are building an AI feature. Like, I don't know, I'm just making it up. You work at Pinterest and you want to have a better image generation that doesn't look like slop that actually pleases users. So it's like an image generation feature.

**Daniel McKinnon** (00:48:39)

You need to think about from day zero, what does success look like? What is unique about those Pinterest users? What do they want to see? And you need to translate that. You can't just write down a PRD and say they want beautiful kitchens. You have to explicitly define what a beautiful kitchen is and Not in words, in examples. And a way to score those examples. And I am not in the image generation space, so I don't exactly know what that looks like. But there are many, many, many examples like this where you need to understand what the user wants and translate that into prompts and responses and a way to score those responses. And that is the first thing you should do when you're starting to build a new AI feature.

**Aakash Gupta** (00:49:21)

Okay. So just like you have ramped up your expertise in the genomic space, if you were tackling that problem, you'd go learn, you'd go talk to people who have built image and evals. You'd understand, oh, this is how I build an LLM judge that generates images of this type. And then that would really be the basis for your eval.

**Daniel McKinnon** (00:49:39)

Yep, that's correct.

**Aakash Gupta** (00:49:40)

Okay. Wow. There's so much, so many layers. I've done like five or six episodes on evals, but I think this was one of the most tactical that really helped me understand How things change. And I think that's a function of your experience, which I wanted to talk about for a little bit. So your evals piece crossed my radar. I think another really interesting piece you wrote about was product management at Meta versus Google. You've worked on Gemini. You've worked on Llama. You've seen both of these cultures. What really is the difference between product management at Meta versus Google?

**Daniel McKinnon** (00:50:16)

Yeah, so I would caveat that and say I wrote this like two and a half years ago and I was at Google three and a half years ago, I think. So a lot has changed. When I was at Google, Google was a dead company. I think the stock fell to like $80 and I think it's 300 or 400 right now. And they've really changed how they think about things. I am a boomerang, that is. I think I spent seven years there in total. And, you know, I saw everything from Cambridge Analytica lows to highs of like Lama 3 really wowing people So I saw a very large spectrum. And what I would say, like my key takeaways for what Google versus Meta was like is Meta is like a much, much more aggressive culture in many ways. I think that it comes from like the founder leadership of Mark Zuckerberg is thinking, He is the last man standing, well, I guess besides Elon, but he is the last man standing who's got like, you know, the founder leading a fan company who has utter and absolute control, who's going to do what he wants.

**Daniel McKinnon** (00:51:20)

And sometimes it's really empowering because he says, this is super important to me. You have all the resources in the world and you should go do it. And sometimes it's like not what you want. For example, I worked on Lama 4. Lama 4 had problems. I think the main problem was actually how it was evaluated. Huh. Funny, those emails are important. If you want to read about that story, Google it. I had nothing to do with that. And I loved working on Lama 4. And Mark just said, you guys all suck. You need to go find new jobs. So basically, the whole Lama 4 team is gone because of, you know, Mark's... So I think that, you know, that cuts both ways. I'd say my overall preference is for like a very like high conviction founder led company. I actually have like incredible respect for Mark.

**Daniel McKinnon** (00:52:03)

I've only met him a couple of times and every time has been just like, wow, this is like a really smart guy. But it creates a lot of problems too, right? Because, you know, Google is much more consensus driven. I think Google has much weaker product management function. At least it did when I was there. You know, Google is considered to be more of an engineering led company, whereas Meta is more of a product led company. At least that historically has been the case. And it was a really great experience working at both places. I think I learned a lot from both places. I left both places with a lot of friends. And yeah, if you want to read like kind of this blog post actually pretty viral. If you want to read like kind of an interesting snapshot of what it was like in, say, 2023 between both of the places, you know, give it a read.

**Aakash Gupta** (00:52:49)

Highly recommend it to everybody. As you guys can see, I'm itching to ask many more questions. So Daniel, we're going to need to have you back. Before you go, tell us a little bit about your startup.

**Daniel McKinnon** (00:52:57)

Oh, cool. Yeah. So I've started a company called Gamoff Labs. And as I hinted at during these evaluations, The core problem I want to solve is to make it much, much easier to get whole genome sequencing into every single NICU in the entire world. And I want to see them in, you know, Rural Arkansas, rural India, rural China, all the places where this kind of life-saving technology is not being harnessed. And my key thesis is that a lot of the human work involved in interpreting these genomes could be augmented by AI. Again, this is small scale. We started this five weeks ago. So, you know, but one person is really crazy to have that impact on their life. And yeah, like it's a deeply, deeply mission driven thing. I think it's very, very interesting technically because it's all about building the best agentic harnesses. It's all about understanding how AI can help with biology.

**Daniel McKinnon** (00:54:27)

And if you're interested in joining me on this journey, we are hiring We're a very small team, raised our pre-seed round, and are basically planning on building the operating system for rare disease and genomic medicine. And I couldn't be more excited to wake up to work on this every morning. And I would love it if you would reach out if you're interested.

**Aakash Gupta** (00:54:47)

Wow. So a lot of you guys I know, at least in my audience, you want to become that AIPM at Met or Google. This is often the next step after that. So, you know, we always say the grass is greener at some point. This is where I've seen those AIPMs at Met and Google go, just like Daniel, into starting their own companies. And that's actually the cool thing is it helps prepare you for that. You can see how his own Evals and deep AI knowledge has now applied to his startup. Daniel, thank you so, so much for lending your expertise today.

**Daniel McKinnon** (00:55:19)

Yeah, I want to leave with just one parting thought is the Metas and the Googles and all the other large companies have to reinvent themselves right now in the age of AI. If you're inside these companies, it is very, very interesting to see how this classic I hope you learned as much from today's episode as I did. If you can do one thing that's totally free that would help the show, it would be to check that you're following on Apple and Spotify podcasts, check that you've left

**Aakash Gupta** (00:55:46)

ratings and reviews Check that you're subscribed on YouTube, leave a like and a comment on this video, and then share it with your friends. We're trying to make better and better podcasts. After two years, we think we've gotten something pretty good going. So let us know what we can do to make And finally, don't forget my offer for the bundle. You get an entire year of my paid newsletter. Plus my favorite AI tools, Bolt Up New, Airtable, Speechify, Descript, Magic Patterns, Linear, Dovetail, Arise, and Mobbin. That's $27,000 worth of value for just $150. So check that out at bundle.akashgu.com if it interests you.

**Aakash Gupta** (00:56:44)

And I can't wait to share our next episode soon.
