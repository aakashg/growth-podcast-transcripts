---
title: "The PM’s Role in AI Evals: Step-by-Step "
subtitle: "AI Evals are not just a technical task for engineers, but the most critical tool for Product Managers to build high-quality, trustworthy AI products."
date: "2025-07-11"
host: "Aakash Gupta"
guests: ["Hamel Husain", "Shreya Shankar"]
speaker_names: "substack"
substack_url: "https://www.news.aakashg.com/p/hamel-shreya-podcast"
youtube_url: "https://www.youtube.com/watch?v=g_3LJ2QBOQE"
duration: "01:34:32"
word_count: 15216
source: "Substack episode transcript (aired audio)"
---

# The PM’s Role in AI Evals: Step-by-Step 

*AI Evals are not just a technical task for engineers, but the most critical tool for Product Managers to build high-quality, trustworthy AI products.*

**Aakash Gupta** (00:00:00)

Why do PMs need to be good at AI evals?

**Hamel Husain** (00:00:02)

Okay, so there's three things that are really important. One, evals give you a way as a PM to inject your taste and your judgment directly into the critical path of the AI product being developed. Second thing is like evals are really important in helping you iterate. The most effective way to do that is using evals, specifically looking at data in a very structured way. And then the third thing is scale. By mastering evals, what you can do is you can make sure that you can scale your case, judgment, so on and so forth, user requirements across all the AI workloads that are running.

**Aakash Gupta** (00:00:37)

What is the most critical skill for PMs who want to build AI features to develop?

**Shreya Shankar** (00:00:57)

Hands down, error analysis. The ability to look at your outputs and systematically figure out what makes for a bad output, quantify how many of these failure modes you see in a big batch of traces for your system, and then figure out how to turn that measurement into a continuous flywheel of improving your product.

**Aakash Gupta** (00:01:18)

If you guys had to build a roadmap for people who wanted to get really deep on AI evals, what topics should they learn? Really quickly, I think a crazy stat is that more than 50% of you listening are not subscribed. If you can subscribe on YouTube, follow on Apple or Spotify podcasts, my commitment to you is that we'll continue to make this content better and better. And now on to today's episode. Hamal Hussain and Shreya Shankar are the people who the experts go to for evals. OpenAI, Arise AI, those people are going to them for evals and we have them on the podcast today. Welcome Shreya and Hamal.

<!-- sponsor -->
**Narrator** (00:02:02)

Hey.

**Aakash Gupta** (00:02:03)

Thank you, nice to be here. Why do PMs need to be good at AI evals?

**Hamel Husain** (00:02:10)

Okay, so there's three things that are really important. One, evals give you a way as a PM to, you know, inject your taste and your judgment directly into the critical path of the AI product being developed. So like, you know, As we all know, like PMs, they spend a lot of time gaining context from customers, user feedback, so on and so forth, writing PRDs. They're, you know, trying to give context to engineers. And, you know, they're hoping like kind of engineers are faithfully carrying out their vision. Now, what evals give you is, you know, you can directly make sure that your taste and all of that context, if done correctly, is now on the critical path when your engineering team is developing those AI products. The second thing is like evals are really important in helping you iterate. So nothing is set in stone. You have to constantly change your requirements.

**Hamel Husain** (00:03:21)

You're learning more about your customers, so on and so forth. The most effective way to do that is using evals, specifically looking at data in a very structured way. And this is one of the things that Shreya and I teach. You know, that allows you to refine and have really fast feedback loops and really fast cycles of feedback. And then the third thing is scale. So, you know, by mastering evals, what you can do is you can make sure that you can scale your taste, judgment, so on and so forth, user requirements across... you know, all the AI workloads that are running in a way that you just couldn't before. Because ultimately there's a lot of, you know, you can bake a lot of these evals. They're using AI themselves. You just have to make sure that you do it correctly. So you have to make sure that you...

**Hamel Husain** (00:04:19)

align the AI with yourself as a PM in a very kind of process that we teach. And as long as you do that correctly and you do it in such a way that you develop trust in the AI that is doing the eval and there's a way to do that alignment, then you can really scale yourself. So a lot of times PMs or not just PMs, but people at large, they kind of view evals as a very monotonous task that, you know, you just want someone else to do it. It's like, oh, like I have to look at data, I have to annotate data. You know, who's going to do this? You don't want to give up that leverage because when you build that foundation of evals, you develop, you have immense leverage and you can, you know, it's a really quick way to kind of exert lots of influence over the process and in a good way.

**Hamel Husain** (00:05:18)

And so this is why I would encourage PMs to really pay attention to this.

**Aakash Gupta** (00:05:25)

Can you guys precisely define evals? Yeah.

**Shreya Shankar** (00:05:29)

Yeah, I can take this one. An eval is some systematic measurement of some aspect of quality. So what varies in an eval is what that criterion is. For example, maybe it's conciseness of a response. And then how you want to measure it. So maybe that is, I'm going to define it by word length. I'm going to find it by sentence length. Maybe it is some very, very complex bespoke human judgment or something that's more subjective. But those two things make up an eval. And oftentimes products actually have a suite of evals. I've never seen just one eval doing the job. I see three to five, sometimes even up to 10 evals that are really important for a product.

**Aakash Gupta** (00:06:23)

People say that if you get evals right, you've gotten the hardest part of the AI product solved. Is that accurate?

**Shreya Shankar** (00:06:32)

I think it's accurate now. What do you think?

**Hamel Husain** (00:06:35)

I think it's totally accurate. Just like anything else, it's the process of creating the evals that provides all the value. It's not necessarily the eval itself is the journey that creates all the value. And so once you've done all of that work, you've looked at all of your data, you've iterated on your system, you've thought very carefully and oftentimes scientifically about how to improve your system, you've already got 99% of the way there.

**Shreya Shankar** (00:07:02)

The way that I like to think about it is if you ever want your product to make it past one iteration, you need evals. I've never seen somebody make it through multiple iterations of their product without any evals. But once you have good evals in place, then evals are not necessarily the bottleneck for you. But that's a good thing. That's how it should be. You should be able to focus on building out other aspects of the product, making things faster, making things feel better, more intuitive, everything beyond that.

**Aakash Gupta** (00:07:37)

Why can't you just rely on human evals? The PM looks at the feature, the engineers look at the feature, and they feel like those outputs are good enough.

**Shreya Shankar** (00:07:47)

Oh, I love this question on the vibe checks and why. So Hamel and I teach our course and pitch it in a way that we are helping you codify, operationalize and scale up your vibe checks. Your vibe checks are very important, but they don't scale because they involve you, the human. It's very hard to onboard other people to do the vibe checks in the same way as you are. So like, I would have to observe you do this thousands of times, look at outputs, try to build my own rubric or mental model of what you're doing. And then I have no good way of teaching other people of how to do this. So being able to do evals just means taking your vibe checks and translating them to something concrete. In our course, we define that as a rubric of binary criteria. Every criteria could be complex.

**Shreya Shankar** (00:08:36)

That's fine. It can be subjective. That's fine. But you better have a very precise definition for pass, fail, have some examples of pass, have some examples of fail. And we also teach people ways to measure alignment on those results. That's really what this whole process is about.

**Aakash Gupta** (00:08:53)

I think the critical phrase there is binary criteria. Why binary?

**Hamel Husain** (00:09:00)

Yeah. So binary really is a kind of a heuristic, you know, in a sense, like that is like a simplification for that works for most people. And the thing is like, you know, a lot of people try to like assign scores and let's say on a rating scale, one to five, that's usually a really bad idea because no one knows what that means. If you have a average score of 3.2 versus average score of 3.7, what does that really mean? And, you know, that can be very hard to calibrate and you have to work incredibly hard to, you know, make sense of that. So binary judgments force you to kind of make a pass fail decision. And that tends to also correlate with the fact that you are going to have to ship this product. do you want to ship it or not? And it really distills that decision-making down into the annotation.

**Hamel Husain** (00:09:54)

And for the vast majority of people, that's the right choice.

**Shreya Shankar** (00:09:59)

Yeah, and to provide a little bit extra context on the background of LLM as judge and why people have a lot of variance in whether they want it to be binary or rating-based scale, LLM as judge has been around before these foundation models even, just regular language models, fine-tuning models to serve as judges. And in those cases, people, A, had a lot of preference data. of what is good and bad, and maybe even a fine-grained scale, and B, could fine-tune models to be aligned with that preference data. Today's world of LLM judge is very different. We don't see people fine-tuning judge models as much. We see people trying to use off-the-shelf models, still want to align with their complex subjective criteria. And now the alignment problem is much harder. You can't steer the LLM in a way that you could before. And for that reason, we say limit yourself to binary, because that is what the LLM can do very well.

**Shreya Shankar** (00:11:03)

All you have to do is provide examples of pass, provide examples of fail, and have very simple or good rubrics. And people find that much easier to do than, say, rating on a scale of 1 to 5. OK, now you need to provide examples for 1, for 2, for 3, for 4, for 5. You need to have descriptions of what makes a 1 different from a 2. All of these things, the pairwise interactions between all these ratings just explode in complexity. And we never see people successfully able to operationalize that at the rate at which they can do binary evals.

**Hamel Husain** (00:11:37)

And a lot of times, non-binary evals, like ratings of one to five, that is a smell of intellectual laziness. The work hasn't been

**Aakash Gupta** (00:11:48)

done

**Hamel Husain** (00:11:48)

to actually, you know, to make a call of what is good enough and what's not good enough. And it's kind of like, oh, we don't really know. Let's just capture these like rough things, you know, in this like score because we're going to lose something. And it doesn't, you know, like the binary scale like really forces you to be very clear about what you want.

<!-- sponsor -->
**Aakash Gupta** (00:12:11)

AI evals are one of the most important skills for PMs, and I know you know they matter. The question is, are you doing them right? Most teams are winging it with basic metrics and hoping for the best. Meanwhile, the teams that actually ship reliable AI, they've cracked the code on systematic evaluation. Today's episode is brought to you by the AI evals for Engineers and PM's course by Hamal Hussain and Shreya Shankar. This live Maven course will teach you the battle-tested frameworks from Hamal and Shreya, who are the engineers behind GitHub Copilot's evaluation system and 25-plus production AI implementations. Four weeks, live instruction, next cohort starts July 21st. Start shipping AI that actually works. Today's episode is brought to you by Jira Product Discovery. If you're like most product managers, you're probably in Jira, tracking tickets and managing the backlog. But what about everything that happens before delivery?

**Aakash Gupta** (00:13:21)

Jira product discovery helps you move your discovery, prioritization, and even road mapping work out of spreadsheets and into a purpose built tool designed for product teams, capture insights, prioritize what matters and create roadmaps. You can easily tailor for any audience. And because it's built to work with Jira, everything stays connected from idea to delivery. Used by product teams at Canva, Deliveroo, and even The Economist. Check out why and try it for free today at Atlassian.com slash product dash discovery. That's A-T-L-A-S-S-I-A-N dot com slash product dash discovery. Jira product discovery. Build the right thing. I've heard that LLMs are also not very good at one to five ratings. Is that true?

**Shreya Shankar** (00:14:14)

They're good at what they're trained on. Somewhere out there in the world, I am sure there is a task with very clear or simple one to five ratings, and the LLM is good for that. But to make such a blanket statement for all products and all use cases is very hard to do. That's the message we want to hammer home to every single product manager who takes the course. Look, you think the LLM might be able to do something. You saw an instance of an LLM being able to do the task for some other domain. That doesn't mean it's going to translate to your domain or your use case. You still have to put in this work and just don't trust any. Hamill is a great way of saying this. Maybe he should talk about it. But he always tells people, never trust it. Always put on your detective hat.

**Shreya Shankar** (00:14:58)

Hamill, you want to talk about that?

**Hamel Husain** (00:15:00)

Yeah, what underlines the entire process of evals is the scientific method, something that we've all learned in high school education. But it's really applied in this context. And what you have to do is be very skeptical of everything. and do lots of experiments and prove to yourself that the the thing that you're trying to achieve or some new complexity you want to add whatever it is that is actually working and try to do it in the simplest way and build intuition doing by doing lots of experiments but the point is to like measure those and Like, you know, record those and go through it in a structured way rather than those vibe checks. You asked about vibe checks earlier. The analogy that I like to use, and I can give this to you if you ask me later, there's a little video of my friend Greg Seccarelli playing whack-a-mole.

**Hamel Husain** (00:15:59)

And it's my favorite meme to use when telling people about the need for evals. It's like you're playing whack-a-mole without evals. So you see a problem, okay, hammer it over with some tool or a prompt change. Then another problem comes up, you hammer that. And you keep going, you don't really make any progress. It's really with evals that you can systematically try to solve the problem without going in circles.

**Aakash Gupta** (00:16:26)

I want to talk about some stories. So one of the features I implemented in my last job, I was VP of product at Apollo.io. It's a unicorn startup that does sales technology. So what do salespeople need to do, right? They need to write emails. So as soon as I think it was Chad GPT 3.5 came out, we're like, okay, we're going to use GPT 3.5 to write people's emails. But the very first thing we found was that it was hallucinating all sorts of crazy details. And ultimately we had to set up a bunch of evals instead of vibe checks. Can you guys give a little bit more context into why evals help solve that hallucination problem for us?

**Hamel Husain** (00:17:07)

Yeah. So with any kind of problem that you see, you know, hallucination or whatever it is. So the first thing to know about evals where people go off the rails is do not reach for generic metrics. So the industry is full of tools and vendors wanting to sell you things. like a magic pill to solve your evals problem. Like, hey, don't worry. Just buy your tool, plug it in. We'll show you a dashboard of all of these metrics and things like that. The problem is it doesn't work because those off-the-shelf evals hallucination score is not going to work. What you need to do is take a look at, in your case, those emails and understand what exactly is the failure mode. And if you do observe a hallucination, what is the hallucination? And kind of give more life to the domain specificity of the hallucination so that you can then start crafting an LLM as a judge that is prompted in such a way that is very specific to the types of hallucination that you are seeing.

**Hamel Husain** (00:18:20)

And then you go through an iterative process. So you kind of hand label when hallucinations happen, you know, how they're happening. You're building an LLM as a judge and you're measuring that judge. You're being skeptical again through the scientific process. And you're saying, okay, I have this judge. Can I get it to agree with me? Can I have it be, let's say, if it's you, Akash, making this judge, this email hallucination thing, you know, how do I make this judge a proxy of me? And how do I trust it? Almost like an employee. And so the only way to do that is to check it. And you can do that iteratively through this process. And when you do that, then not only do you have something that scales, it's an automated way of checking that problem, but it's also something that you trust. And that second part, that something that you trust is key because the last thing you want is the whole bunch of evals that you put up on a dashboard.

**Hamel Husain** (00:19:16)

And then people stop looking at them because they're like, oh, we have these evals, but you know what? The product doesn't really work. No, that's the death of your AI product because then no one's gonna ever look at evals again. And then you don't have any leverage.

**Aakash Gupta** (00:19:34)

That's exactly what we experienced and you weren't even there. I wanna talk a little bit about your experiences. I know you worked at Airbnb on these products. Can you tell us a little bit more about that and what was the most difficult part of building evals there?

**Hamel Husain** (00:19:50)

So I didn't work on LLMs at Airbnb because it was prior to, you know, way before ChatGPT. But what I did work on my entire career is machine learning and, you know, building predictive models. And a lot of the same... machinery of evals comes directly from machine learning. The reason that is, is because machine learning systems are systems that produce stochastic outputs. You know, they'll give you predictions of various kinds or like classified things and they're non-deterministic and you have to evaluate them. And like, you know, they're giving you different outputs every time and they have noise. And so how do you do that? that's something that's very well established in machine learning that a lot of people haven't been exposed to. So when it comes to like AI more generally, now you have really very similar thing. It's like, hey, you have like a stochastic system, it's non-deterministic, it can output anything like these emails.

**Hamel Husain** (00:20:56)

It's like, how do you go about measuring that? And yeah, and so basically you can kind of bring that over. And so what we teach is instead of going through the entire data science machine learning curriculum, how do you have a very focused way of learning that that is contextualized to LLMs?

**Aakash Gupta** (00:21:20)

That's actually fascinating. How was Airbnb using machine learning models? I'm sure people want to know under the hood.

**Hamel Husain** (00:21:27)

Yeah, Airbnb was using it for a lot of things, such as detecting fraud in payments. Also, the biggest use case at Airbnb was search ranking. So if you're searching for a listing, let me show you other listings that you might be interested in based upon what you've been looking at and what you're searching for. So basic recommendation systems, search ranking, things like that. A lot of like growth marketing marketing. initiatives like trying to figure out the lifetime value of a specific guest so you can allocate marketing to them appropriately that's what i worked on um you know and there's many other use cases but those are the ones that sort of one of like they're bigger ones and now they have you know now airbnb's doing generative ai stuff as well just like any other company

**Aakash Gupta** (00:22:19)

Search ranking is something that probably we've been dealing with for like 30 plus years, I guess, ever since these search engines ever came out. So what can we learn from how people are evaluating search and apply into how we're evaluating our LLMs?

**Shreya Shankar** (00:22:36)

The number one difference now is we definitely search systems to try to get context to improve our LLMs, sure. But the consumer of the search results is now the LLM. In the past, the consumer of search has been the human. And humans and LLMs are good at different things. LLMs are good at finding needle in a haystack in very, very long, complex windows. Humans have very short... attention spans they'll read through things but after a few paragraphs they're done so some of the metrics like how high up a relevant result was ranked are much more important for humans than they are for LLMs. You could try to retrieve like 500 results. And as long as it's, even if it's like 150, 200, the LLM will pick it out and figure out how to give that result to the user. So I think the bottom line differences are we still want to use the same metrics.

**Shreya Shankar** (00:23:34)

but our tolerance has changed slightly. We still want to prioritize recalling the right information, but now that we have long context windows, it's okay for it to kind of be at the end, as long as we carefully leverage LLMs to go and iteratively refine those search results, pick out the bottom results, and then go and show that back to the human.

**Hamel Husain** (00:23:56)

One thing I'll add on to this is people often... wonder, okay, how do I evaluate RAG systems? So RAG is a big thing. And so what is RAG? You know, retrieval, augmented generation. There's the retrieval part, and then there's the generation part. And so the retrieval part, you evaluate that pretty much the exact same way that you would evaluate any search system. So all those classic search systems and informational retrieval, like that entire scientific discipline, can be applied onto the retrieval part. So like optimizing that, making sure you're getting the right documents, the right context, so on and so forth. And a lot of it applies. And Shreya's right, there's some nuance in terms of different tolerances and things like that.

**Shreya Shankar** (00:24:47)

Yeah, the number one thing I see that's different is instead of measuring like recall at 10, like we can measure recall at 500 and have a long context model like Gemini be able to consume those results. At the end of the day, maybe you want to measure precision for the result of the LLM call that feeds in the result to the human. Sure, whatever humans consume, they should all be measured the same way. But if LLMs are there refining search results, then we can use that to our advantage to be able to re-rank outputs from a search engine.

**Aakash Gupta** (00:25:22)

So that search, one of the other sort of really big things in the AI space that I think, Hamil, you worked on a little bit was the precursor to GitHub Copilot, right? LLMs for code generation. What was the biggest problem you guys faced with evals for that? So

**Hamel Husain** (00:25:41)

with, okay, things like code generation are actually really interesting. So in evals, there's more generally, in AI products, more generally is, You want your domain expert inside the inner loop. So what you don't want to do is give your developer the task of annotating your data and, you know, writing evals necessarily because they don't know enough. They don't have enough context. And that... really bottlenecks a lot of teams because they don't get that right. But there's an exception. The exception is developer tools. That is one case where the domain expert is the developer. And so that's why we saw developer tools as the first AI products. because that was the sweet spot. That was like where it was easiest to develop. That's one property of developer tools. The second property is a highly verifiable domain. So there's some structure to code and it turns out like on GitHub, you know, you have all this code and you also have lots of tests defined against that code.

**Hamel Husain** (00:26:54)

So a lot of time was spent in that verifiable domain and it's excellent when you have a verifiable domain is to develop kind of a test harness and the test harness was very impressive. Basically, what it did is it took all of the code at scale, not all of it, but a select like filtered quantity of it and basically recreated the environment that code is going to run in and ran the test at scale. And basically, you know, things like asking the LLM to fix certain things or complete certain code, and it would run all the tests. It's kind of a very impressive engineering effort. Cause you're talking about running all of this random software from everywhere with all kinds of dependencies at scale all the time. Um, so the, the, the details don't matter. What I want to say is like the evals really mattered because a lot of upfront work went into constructing the eval system and it's really after that, that the team was able to iterate really fast.

**Hamel Husain** (00:28:02)

Like when GitHub co-pilot was first released internally, it didn't really work. You know, it was something like, you know, 20% or so of, you know, like acceptance rates of like suggestions, things like that. And then after the evals, the team was able to like iterate really fast and like climb that, you know, to where it did work. And so, you know, it was really like, or let me step back. It was, yeah, it was, it was really like the key that unlocked, you know, progress on that. I didn't work directly on the GitHub Copilot in that phase. I was working on some research before that. I was actually working on some research that led to some of the benchmarks. So basically, one thing I did at GitHub is I worked on this project called CodeSearchNet, which is a semantic search of code. And basically, like, you type in, like, what code you're looking for and, like, semantically try to find it.

**Hamel Husain** (00:29:13)

And it leveraged a lot of the... So a lot of code has comments in it, in the documentation embedded in that code. So it was just a really large data set. We opened a large data set with benchmarks of, you know, code retrieval. And so that was, like, used by OpenAI in their very first iteration of Codex, which is, like, a very... It's not the current codex. It's like a different, same name, but different thing. But it was an eval. It was an eval that was used back in the day. So you can say I've been working on LLM evals for a real long time.

<!-- sponsor -->
**Aakash Gupta** (00:29:52)

Trust isn't just earned, it's demanded. Whether you're a startup founder navigating your first audit or a seasoned professional scaling your GRC program, proving your commitment to security has never been more critical or more complex. That's where Vanta comes in. Businesses use Vanta to establish trust by automating compliance needs across over 35 frameworks like SOC 2 and ISO 27001, centralized security workflows, complete questionnaires up to five times faster, and proactively manage vendor risk. For a limited time, my listeners get $1,000 off Vanta at vanta.com slash Akash. That's V-A-N-T-A dot com slash A-A-K-A-S-H for $1,000 off. Today's episode is brought to you by the AIPM certification on Maven. Run by Mikdad Jaffer, who is a product leader at OpenAI, this is not your typical course. It's eight weeks of live cohort-based learning with a leader at one of the top companies in tech. OpenAI just doesn't stop shipping, and this is your chance to learn how.

**Aakash Gupta** (00:31:14)

Run along with product faculty and Mo Ali, the course has a 4.9 rating with 133 reviews. Former students come from companies like OpenAI, Shopify, Stripe, Google, and Meta. The best part? Your company can probably cover the cost. So if you want to get $500 off, use my code AAKASH25. And head to maven.com slash product dash faculty. That's M-A-V-E-N dot com slash P-R-O-D-U-C-T dash F-A-C-U-L-T-Y. You mentioned hill climbing, and I think that's a really interesting concept because I was reading Daniel McKinnon's piece on evals. He is a PM on Meta's Lama team, and he talked about how it's so important for the PM to define the evals so that then the AI engineers and research teams that he works with can hill climb. Can you guys explain that?

**Shreya Shankar** (00:32:03)

Engineers are really good at hill climbing, especially ML, AI, data science, stats people, people who are trained to go and look at ML metrics, figure out why they're bad and how to improve them. They were good at that in structured data and traditional machine learning because those metrics are very well defined. Accuracy is well defined, loss is well defined. If you're doing a binary classifier and you already have labeled data, it's all there for you. You're just doing your job and trying to improve on those metrics. Now we're in a role in which none of the metrics are defined. And so there's no way to go and exercise all the skills that the AI engineers have to improve those metrics. I think it is so spot on that This article talks about PMs need to set these metrics because they have the best context to set them.

**Shreya Shankar** (00:32:57)

And once you set them, once you provide the definition or examples of good and bad, then engineers will figure out a way to encode this into the product and even get to self-improving products. That is exactly what I see also in my experience.

**Hamel Husain** (00:33:14)

One thing you have to be careful with hill climbing, and when that term is said, it does tickle my brain, is to make sure that people don't overfit. Because engineers, sometimes they use that term, and they are overfitting in some sense. Machine learning people know, data science people know, but it is a thing.

**Aakash Gupta** (00:33:37)

And what does overfitting look like in practice?

**Hamel Husain** (00:33:42)

Yeah, overfitting means that you have hill climbed against some data or something that doesn't generalize. So the key phrase is does not generalize. And maybe you have some evals. So one very trivial way to mess this up, and this is from a real client, is you have a test data set of cases that you want to do well on in your evals and you use the same data as few shot examples in your prompt. So that is a hilariously kind of straightforward way of overfitting because you have given the LLM the answer directly in the prompt. And there's, you know, we can relax that a little bit. There's more subtle ways that you might do that. But essentially, you know, you might over-engineer your prompt with those specific cases in mind with the details of those cases that are a little bit too specific, you know, even though you don't have the exact like information there, you know, that might lead to overfitting.

**Hamel Husain** (00:34:52)

Um, and there's many ways you can overfit. And what we, Shreya and I teach is, well, how do you know that you overfit? How can you guard against it? It turns out you can use a lot of the same techniques from machine learning to kind of give yourself a early warning system to say, Hey, like you overfit.

**Aakash Gupta** (00:35:11)

What are some of those techniques?

**Shreya Shankar** (00:35:15)

Uh, number one thing is collect label data, reserve some of it for testing as Hamill kind of alluded to, you know, you want to have some test cases that you want to try out your product to see if it performs well on, you know, reserve that set and never, never look at it. Never look at it when you're developing your product, when you're developing your prompts, even when you're kind of trying to test out your prompts to figure out how to improve it. Just make sure that the test data is like in the sandbox that you never, never see. That's the number one strategy that I tell people. Another thing that I tell people, and PMs should also know this, is anytime you see a metric that is suspiciously too high, like I achieved 99% alignment or 95% or 100% or whatever, Immediate smell warning flags that something is off.

**Shreya Shankar** (00:36:09)

We're leaking some data into our prompts from the test set, maybe. Maybe our test set doesn't have enough examples. So go back and question the process if you see any numbers that are too high.

**Hamel Husain** (00:36:21)

That's absolutely true. One of my favorite examples is there's There is an interview that's been going around for a while now. It's from a company called Case Text, who's bought by, I believe, Thomson Reuters, or maybe LexisNexis, one of the two big ones, legal companies. And the CEO said, hey, you need to keep iterating on your evals until you get to 100% accuracy. And so, you know, if you're iterating, if you're getting 100% accuracy in your evals, it's likely your evals are worthless because they are providing you with no signal. Just think about anything else. If every student in your class is getting a perfect score, is it a good test? You know, any kind of test, if everybody is passing it and everything is passing, should you be celebrating? No. It means the test doesn't have, is not differentiating good and bad and probably is not really worth it.

**Hamel Husain** (00:37:26)

And so it's really good, you know, you have to keep that in mind. You want your test to be hard. A

**Shreya Shankar** (00:37:33)

bit of nuance to it. You want some tests that are, you know, basic regression tests or functionality tests that absolutely you want to pass them because otherwise you're shipping a broken product. But I think the broader point Hamill and I want to make is you also should have some aspirational. evals um and those you know it doesn't need to be zero percent or like designed adversarially but some benchmark that helps you know whether you know the general ai or intelligence in your system is getting better

**Aakash Gupta** (00:38:08)

in talking to so many ai companies about evals what's one ai company that sticks out to you as doing it particularly well and why

**Shreya Shankar** (00:38:22)

Everyone's struggling. Okay, I'll talk about some design principles that I see people converging on that are solving parts of their problem. So I don't think anybody is doing it perfectly. I mean, otherwise you would have like a rocket ship AI startup that's like already perfect and like gone public and everything works. We just don't have that, right? It's not there. So like, let's be honest. Some of the things that I've been seeing teams that really seem to give them leverage are, one, building custom data labeling and annotation interfaces, or providing ways for domain experts or other people that they trust to be able to get feedback on traces. A lot of the observability tools for LLMs have started to build in these features. They didn't have them even in the last two months, three months. So it's going to take some time until we can really see the effect of that.

**Shreya Shankar** (00:39:28)

Another thing that I've been seeing is these really well-scoped LLM judges. that are being deployed as part of products. Claude Anthropic just had a new post on their research agent about how they really break down the complex task into a multi-agent system. And then, critically, they have a bunch of LLM judges that are very, very well scoped to each task, much like we teach in our course. And I'm sure they're making a bunch of revenue off of this product. Yeah. And then, of course, I think there's a lot around Cursor, famously, very dutifully measures your next token prediction. They have their own models for this. I think next token prediction for coding is interesting because that metric is very well defined. People know that it's useful. It directly correlates with product success. Not all products have such a metric like that. PMs need to really go figure that out.

**Shreya Shankar** (00:40:22)

But these kinds of things, I think, are broadly helpful across the board that I've been seeing. But I think we're pretty far out from the product that's perfect right now.

**Aakash Gupta** (00:40:31)

What is next token prediction?

**Shreya Shankar** (00:40:35)

When you're writing code, the next snippet that you're going to write in your code, if the AI model predicted that correctly, then the metric goes up. If not, metric goes down.

**Aakash Gupta** (00:40:46)

Kind of like an advanced autocomplete. Why haven't we seen better autocomplete in like regular products, like email and text message and things like that?

**Hamel Husain** (00:40:58)

It's incredibly frustrating. Um, if, especially if you're writing code, if you're a programmer using cursor phrase using cursor, I know like six hours a day. Um, And, you know, the developer tools are very far ahead of the other tools. And it's incredibly frustrating if you try to use AI in Gmail or in Google Docs or in PowerPoint or anything. And it's, like, even more frustrating because then you open LinkedIn or whatever and it's like, do we have AI in everything? And we're like, no, you don't. Like, you barely do. And, yeah, I'm not really sure why...

**Shreya Shankar** (00:41:37)

I have some hypotheses. Yeah, so it goes back to Hamill's comment on verifiable domains. Code is a verifiable domain to some extent. You can just make sure the code runs. That's already great. The other thing is there's a bunch of data of how people write code that's already there and available on the internet in ways that we don't have that for emails. Emails are not very verifiable. Nobody is telling you this is ground true, this is correct. or this is not correct. PMs have to do this job of figuring out how to design a system around good and bad emails. And that's where it becomes really, really bespoke. And I think that it goes also back to Hamel's comment around code, where it's like developers knew what the evals were, so they were able to implement that. But this is why we need AI PMs. We need people to be able to help developers craft these verifiable or even loosely verifiable signals.

**Aakash Gupta** (00:42:42)

I know you guys have spent some time with OpenAI. How is OpenAI approaching evals and what can we learn from them?

**Hamel Husain** (00:42:51)

So one thing I'll say is, um, you know, there's a really big difference between foundation model benchmarks. So MMLU score, human eval score, these are like general purpose benchmarks, which tried to assess the general capability of models. And then there's another kind of eval, which is your domain specific eval evals for your business. And they're very, very different. And it's important that people know that. Now, rightfully so, the foundation model labs like OpenAI, they very much focus on the former, the general purpose benchmarks, because that is, you know, relevant to their product. But I think, you know, they're kind of at the same level of playing field as everybody else. when it comes to domain specific evals and like how the companies should be defining their evals.

**Shreya Shankar** (00:43:51)

The other thing is they're not going to do it. Because your definition of a good email is different from my definition of a good email. And we're both building email assistant companies. They're going to be different products than they should be because they should reflect our taste and our company's vision. OpenAI just cannot solve both of them with one model. That doesn't make sense. And they're not in that business. They're trying to make the model that you want to hire, for lack of a better term, to do the job. But you need to train, not really train in terms of model parameters, but you need to figure out how to make an environment, how to elicit the right signals, how to reject emails that are bad according to your definitions. That's all the stuff that you've got to build that's domain specific that no foundation model company is going to do for you.

**Hamel Husain** (00:44:38)

Definitely. One example that is top of mind right now is Shreya just wrote this excellent blog post writing in the age of LLMs. And, you know, if I was the, so the problem is, is like foundation models, you know, they're trained, they have like sets of labelers. And basically it's the, it's by definition trained on the average taste of some people. And, you know, if you're, if for, so if you're writing a lot, you know, like I know you are Akash, you know, as well is the, you know, what comes out of the LLM, like almost everybody I know that writes a lot kind of hates it. Like, why can't it be better? Like, why is it giving me like the same, like, why is it like using so many words? And why is it like doing this? Why does it keep using M dash everywhere?

**Hamel Husain** (00:45:30)

Why is it using so many emojis? Like, stop it. It's because like, you know, whoever's labeling the data, you know, they kind of bias towards like longer explanations and like overusing bullet points and all this stuff. And so like, you know, if you want to have like a thing that writers love, you know, then you have to get someone, you know, you have to get like perspective like Shreya has and like iterate on your product like over time and make it do those things that incorporate the taste that you have, you know? And so that's kind of where it diverges from the foundation models.

**Aakash Gupta** (00:46:11)

So do those wrappers where you're putting in your own taste into the evals, do they actually have some sort of moat where people should consider building those startups? Yeah.

**Shreya Shankar** (00:46:21)

Oh, absolutely. I think maybe I'm crazy. I think evals are the moat for AI products and truly nothing else. Tomorrow you can use a different model. You can have a different stack for surfing, whatever it is. The secret sauce is your evals. And how you're able to operationalize or scale that out as quickly as possible. So that means having good LLM judges, for example, that are very well aligned with your preferences that you can just automatically run on everything and build that flywheel for yourself to go then look at what failed and improve your product and so forth.

**Hamel Husain** (00:46:59)

And it's not just the eval itself. It's the whole system, like Shreya is saying, around the eval, the entire eval pipeline. It basically should be portable. You should be able to switch models or switch components and see what the effect of that is. And the key thing is evals open up a whole lot of doors. So it opens up the door for easy fine-tuning. Once you've done an eval, you've already done 99% of the work of fine-tuning. fine tuning is just a kind of a formality that you can go through after that almost to an extent because you've already done you already have all the tools for data curation you know how to measure things you know how to like see measure the effects of the fine tuning so on and so forth you know and I suspect that that will become that just accelerates your advantage like that much more

**Aakash Gupta** (00:47:54)

It's kind of funny because I see people tend to focus on fine-tuning a lot more, and there's a lot more attention given to that. I think it's because in the open AI and anthropic developer docs for when they give you a model, they're like, yeah, this is how you can fine-tune it and things like that. How does fine-tuning really fit in with the overall lifecycle? When should you be putting attention into fine-tuning?

**Hamel Husain** (00:48:19)

We should put it in last. So you should do evals first because what are you... You have to know what you're finding.

**Shreya Shankar** (00:48:29)

Sorry,

**Hamel Husain** (00:48:29)

maybe my connection is

**Shreya Shankar** (00:48:30)

bad. There's like lag here. Yeah, you need to know. This goes back to you want to iterate on your product. You want to know, OK, my product is not good, so I'm going to improve it. You don't have any way of knowing if your product is not good unless you have evals. So evals are step zero. Quantify your performance. Then step one is, OK, how am I going to improve its weak points? Some low-hanging fruit ways of improving are just use a more powerful model. Switch from GPT-40 mini to GPT-40. See if that works. Because you have good evals, you can just make that switch, run it, see if your numbers go up. There are other more complicated strategies you can do, like take a complex LLM call, a complex task described in them, and break them down into multiple LLM calls. So instead of having an LLM extracting 10 things from this document, I'm going to have one LLM call each extracting one of those 10 things.

**Shreya Shankar** (00:49:30)

So like that, you can kind of do task. That's what we call task decomposition. When you exhaust these strategies, then it makes sense to move into fine tuning where it's like, I have no other way of solving my problem. The model's just not there yet. I'm gonna collect a bunch of data or use the data I've already labeled and fine tune a model. Fine tuning has cons because now you have to make sure that you're continually fine tuning that model As you get new data, you learn something new about your preferences of your customers. They don't just automatically update if the base model updates. GPT 4.0 or 5.0 or whatever comes out. Now you have to redo your all fine tuning all over again. And then if you don't use a model provider's fine-tuning service, like you're fine-tuning an open-source model, you need to deal with the MLOps complexity of serving that, making sure it has good uptime, latency is low.

**Shreya Shankar** (00:50:28)

This is all actually pretty complicated. It costs a lot to maintain this infrastructure, both in human personnel as well as in money. And using an off-the-shelf LLM is pretty much the right way to go in most people's use cases. So for those reasons, we really try to not encourage people to do fine-tuning unless you really, really have a good reason for doing your own fine-tuning.

**Hamel Husain** (00:50:55)

One example where I might go to fine tuning hilariously is this writing thing. Because like Shreya, we talk about it a lot, like writing, writing, bash your head against the wall. Even right before this call, it's like, oh, like, do you try 4.1? And Shreya made good comments. Like, no, like, you know, you can't prompt it with all of these rules. It's not going to follow these rules. So I'm like, okay, there's no, this really feels like there's only one avenue left here. You know, we have to put a lot of work into it. But it's like, if you wanted Shreya GPT, that feels like the only way to get it.

**Aakash Gupta** (00:51:27)

Fine tuning is always talked in the same conversation as prompt engineering and rag. So when do you really think about using each of those three techniques?

**Hamel Husain** (00:51:39)

Um, okay. So like, yeah, prompt engineering is basically, you know, everybody that's this basic, you know, you're using the LLM. You have to communicate what you want to it. You have to specify what you want in whatever way. So you should always be writing prompts. You don't even need to worry, put the word engineering at the end. We are kind of, you know, adding a lot of ceremony. You know, we're just, you're writing, you know, write English or, you know, in some cases you might, you can write other languages too, but it is mostly English, you know, and refine your thinking and refine your instructions. RAG is, you know, anytime you're, you need external context to, Um, which there's a very narrow set of use cases where you don't need external context. Most of the time you do need in many applications, you need some external context.

**Hamel Husain** (00:52:30)

Um, you know, that's not some general knowledge of the world. Like, and so, um, that's when you need rag, you know, and you're not trying to bake all that external context into your prompt. Um, um, And then, yeah, fine-tuning is sort of, hey, like, if you can't prompt this behavior, if the model is not doing what you want, Shreya has created this, like, very powerful model called the three gulfs. Maybe we should bring it up on the screen, actually.

**Shreya Shankar** (00:53:07)

Yeah, this is the three gulfs question.

**Hamel Husain** (00:53:11)

Yeah, we should dive into the three gulfs.

**Shreya Shankar** (00:53:17)

I think they're in lesson one.

**Aakash Gupta** (00:53:19)

Okay.

**Shreya Shankar** (00:53:20)

Or, great, you have them. Oh, you made your own gulfs. Nice. Yeah, I can take

<!-- sponsor -->
**Narrator** (00:53:32)

this

**Shreya Shankar** (00:53:32)

out. So your question was, you know, you have all these tools available to you for improving AI products. You have prompt engineering, you have rag, you have fine tuning. Are they the same? Are they the different? When do I use them? Blah, blah, blah. This is a good question that trips people up a lot because people are just thinking of them all equally as ways to improve their product. They're all complementary strategies. You can do multiple of them. You can do none of them. You can do one of them, whatever it is. Prompting is very good when you have specific requirements that your task follows, and you need to communicate that to the LLM. So say you were to hire some human to do some job or contract some job for your company. You might give them a task specification. Say, do this, then do step A, then step B, then step C.

**Shreya Shankar** (00:54:22)

Make sure your output follows these requirements. That's prompting. It almost feels like there's no ceiling sometimes to how much value you can get from good prompting. And this is the first thing that you should be doing. And this solves this gulf of specification problem that Hamill and I see a lot. in how people build LLM products, which is they have some latent, this hidden criteria, this hidden task that they want the LLM to do, but they just don't know how to specify it well in a clear way and completely so that LLM fully understands all of those hidden preferences. Now, fine-tuning RAG strategies are for this gulf of generalization, which targets this problem of, I have a very good specification, but the model is simply not good enough for some reason. Maybe the model is not powerful enough, so I should do fine-tuning. Maybe the model just doesn't have all of the context that it needs to make the decision, that's where RAG comes in.

**Shreya Shankar** (00:55:30)

I need to pull in external data sources to improve my product. But, yeah.

**Hamel Husain** (00:55:37)

Very helpful. And I will submit to you, I know that you ask this question a lot in your podcast, because I think it's confusing, rightfully so, you ask this question. I would say this might be a good framework for answering that question, you know, since it comes up a lot.

**Aakash Gupta** (00:55:56)

Yeah, I try to play the role of the watcher, right? And they keep asking me that question, so I got to ask the experts. Makes sense. If you guys have to build a roadmap for people who wanted to get really deep on AI evals, what topics should they learn?

**Hamel Husain** (00:56:12)

Great question. So Shreya and I have developed this course reader. It's actually a very extensive set of notes. One might even call it a book. It probably will become a book. It's 150 pages. This is the detail that we go through in our course. We arm our students with a lot of information to make sure that they get materials in many different ways, including, you know, live instruction, office hours, but also this very detailed sort of treatise on like how you go through eval step-by-step process. So we start off with, you know, like what is evaluation? We go through the three gulfs framework that we just described. You know, we talk about why you need evals. We motivate that. Then we kind of do a little bit of overview of like, okay, the strengths and weaknesses of LLMs, you know, what kinds of things you need to intuitively understand when you're doing evals before you even get to evals.

**Hamel Husain** (00:57:10)

The third chapter is very important. It's probably where we spend a lot of our time in practice. And a lot of people, we don't know about this step. It's called error analysis. So what is error analysis? So you might hear Shreya and I talk a lot about looking at your data. We keep beating people over the head with this phrase, look at your data, look at your data. What does that mean? Look at my data. What data do you look at? Do you look at all your data? Do you just quit your job and look at your data and do nothing else because you don't have time? How do you look at your data? And what do you do when you look at the data? How do you make sense of it? How does it make it tractable and learn something from your data? What if you don't have any data?

**Hamel Husain** (00:57:59)

What data am I talking about? What if you haven't built anything yet? The key thing is like you need to look at some sort of data, go through a structured process. It's not as painful as it sounds looking at data. It's actually really beneficial. A lot of my clients, you know, we have a plan to go through this whole process and they get so much value just out of error analysis that they just... They're like, this is amazing. I'm done. I'm like, wait, what do you mean you're done? Like, I can do all this other stuff for you. Like, no, no, this is great. Like, this is like, I'm busy for a while. Error analysis has taught me so much. And, you know, error analysis is, you know, to go to error analysis. We can scroll through... Let me see if I can... There's a diagram here.

**Hamel Husain** (00:58:54)

But, you know, this is like one way to generate synthetic queries, for example. It's hard to dive into the details just without the context. But we go through the process of like how to generate, you know, synthetic data, you know... And then also we go through like how to look at your data. And, you know, so we describe it in a lot of detail. A lot of it is supplemented with videos. Let me see if I can scroll up. Maybe Shrey, you can.

**Shreya Shankar** (00:59:28)

Yeah, that diagram is pretty good.

**Hamel Husain** (00:59:30)

Yeah, this

**Shreya Shankar** (00:59:30)

one.

**Hamel Husain** (00:59:31)

So there's a concept called axial coding or open coding and axial coding. Shrey, you want to tell us everyone where that comes from and the history behind it?

**Shreya Shankar** (00:59:41)

Yeah, definitely. So in creating this curriculum, we took a lot of inspiration from social science research, actually, because we were thinking, OK, in what field and domain do people need to look at vast amount of unstructured freeform text and labels and come up with meaningful, actionable insights out of it? Well, it turns out social science researchers have done this for a very long time. There's this process called grounded theory. that gives this systematic structure to the process. And first, what people do is go through their open-ended data outputs or whatever it is. They read them, and they write freeform open codes is what they call it. Freeform notes on what's good, what's bad, any themes that emerge, whatnot, on a trace-by-trace basis. Then after going through about 100 of those, they will try to merge similar notes together into clusters. And this determines your failure modes.

**Shreya Shankar** (01:00:42)

If you find that a bunch of notes around a specific type of hallucination get merged together, well, looks like that's a huge problem that you need to solve in your product. And this kind of loop keeps going until what we call theoretical saturation in qualitative research, which means I've not learned any new failure modes. That's all. I keep looking at data and I just keep adding to my existing failure modes. At that point, you can kind of stop. And then you can move on to, OK, how am I going to turn those into automated evaluators so I don't have to do it all the time? Maybe I'll build LLM as judges based on my labeled failure modes. Maybe I'll write some code-based evaluators for things that code can check. And then we find that we teach people this diagram, error analysis. And then suddenly, they're like, oh, this is great.

**Shreya Shankar** (01:01:36)

OK, bye. And it's like, I mean, I guess, right? It makes sense. This is where most people are actually bottlenecked, right? ML, traditional machine learning people, didn't have to do this. When they looked at their data, they would just look at all these tables of features, which are all numbers, and the outputs are also numbers. And so there are ways to kind of debug those. LLMs are different because now the inputs are freeform text and the outputs are freeform text. And people are like, I don't know how to. It's new skills that you need to be able to make sense of that. But fortunately, once you do this, then you can go and implement automated evaluators as you might with traditional machine learning. And then you can do improvement strategies. You can do fine tuning, all of these things like a traditional machine learning person would.

**Hamel Husain** (01:02:27)

One thing I want to share that might be useful here or interesting perhaps for a product manager, we have Teresa taking our class. And just today she was discussing, okay, I love the class too. When open and axial coding, are we analyzing opportunities towards an outcome? And she responds, I've been thinking about this a lot. you know, and then she has some comments about generating synthetic data, you know, but she also recognizes, and this is really fun. This is why we have product managers in our class, because, you know, these kind of like tying together of things like, okay, identifying opportunities from interviews is based on grounded theory also, you know, and then she's experimenting with methods for capturing annotations directly from the customer. And she also kind of points out that, okay, these are the scientific method applied, look at the data. So I think project managers have a lot to offer here, bringing their customer and user research into the whole process.

**Hamel Husain** (01:03:35)

That's why we think it's really important that they are in the driver's seat of these evals.

**Shreya Shankar** (01:03:42)

I will go even further to say that I think that PMs are vital. in building AI products. We're not going to have successful AI products across different domains unless we have good AI PMs. I cannot emphasize that enough. Without good AI PMs, we're just going to have failed AI products. So I hope this is a call to action for PMs. This is a skill that you absolutely need to develop. It's going to set you apart, obviously, of course, from a career perspective. But also, we need this in order to really realize this vision of AI products changing people's lives.

**Hamel Husain** (01:04:24)

Okay, so to get back on the things to know. So once you do error analysis, now you have a grounded way of knowing what to focus on. Because the question is, what do you even evaluate? Right. You can come up with like millions of metrics like hallucination score, toxicity score, conciseness score. You can name these scores all day long and you can get really confused and overwhelmed and say, oh my goodness, like I can't do it. So error analysis is very important. You know, you would be surprised in our Discord channel, almost every other question is answered with the phrase error analysis because, you know, One of the main trouble people have with evals is what do you eval? You can, you know, you can eval anything. There's an infinite number of things, ideas of things that can go wrong. You know, instead of just being paranoid and sort of, you know, working yourself up about like what can go wrong, you should be grounding it in things that are going wrong or the things that will probably go wrong.

**Hamel Husain** (01:05:28)

And that's what error analysis helps you with. It helps you focus on high value things because evals are not free. it takes a little bit of effort. And so this entire time that you're doing evals, there has to be a cost-benefit analysis around like, what do you even eval? Should you be evaling? What do you eval? Whatever. And so error analysis is the answer to all those questions. And error analysis is so valuable that a sizable portion of my clients, they sign up with me to go through this whole evaluation process. And they do the error analysis part. And they're like, great, Hamill. We love it. We're done. I'm like, no, wait, I have all this other stuff, all this other stuff in this table contest I can take you through. They're like, no, this is so much value. We're so happy. And it's true because error analysis is this thing about looking at your data.

**Hamel Husain** (01:06:30)

It actually drives you to develop a very deep intuition about your system and what's going wrong with it. And it makes you develop a nose for everything and kind of gives you a sixth sense of like what is even going to break if you're doing it enough. And so it's extremely powerful, probably the most powerful technique in evals. So, you know, I can't highlight it more than that. But, okay, once you move past error analysis, now you know what is wrong and where to focus and what to prioritize. Now, how do you actually go about the process of writing the evals? And so that's where these other chapters come in around, okay, who writes the evals? Who does the annotations? So we have some strong guidance in here. We're not afraid to cut right to the chase and have opinions. And so one opinion that we have, for example, of the many opinions, but I'll just highlight it here, is benevolent dictators.

**Hamel Husain** (01:07:38)

So we say, okay, people always ask, well, who is going to make the final call of whether or not this is a pass or fail? Or who is going to be the one writing the email? Who's in charge? Okay. I have a whole team. Do I just involve the whole team? The answer is no. You need to have a benevolent dictator in most situations. And there's some, you know, there's some reasoning behind that. It's just, you know, it's like the binary classification thing. It forces you to kind of make a decision and it makes the whole process tractable because it can quickly become intractable if you add various complexity. So going back to the table of context, let me get a context. Let me just roll back up. Feel free to interrupt me for any time. So we talked through implementing, you know, making this a process automated with LLM as a judge.

**Hamel Husain** (01:08:29)

Now with LLM as a judge, you're writing prompts and you're asking an LLM to grade something. Now, almost everybody... I would say 80% of people who are using LLM as a judge are just writing a prompt and just praying that is doing the right thing. But that's not what you should do. The right way to use an LLM as a judge is to get your label data, which you already done in a previous step, that's what we're teaching, and measure the LLM as a judge against your label data to understand... is the judge any good number one but number two more importantly you have to iterate on your lm as a judge you have to see like where is it wrong and you're like oh it's always the case that not only do you adjust the lm as a judge but shreya has a lot of research that shows that the annotator also adjusts their requirements seeing the lm output i'm sure you want to talk a little bit about that

**Shreya Shankar** (01:09:34)

Yeah, I have a paper called Who Validates the Validators with 2024, if people are interested in the venue. But yeah, one of the things we did was we built an interface for people to go and annotate outputs to train LLM judge evaluators. And then we found that people will keep changing the rubric as they encounter new failure modes when looking at the data. And this underscores how tricky it is. to figure out what the rubric is, how you need to go through this iterative process, how sometimes when the criteria is a little bit too subjective, maybe you want to have multiple people weigh in on what correctness means. And there are ways to do this, like the inner annotator agreement metric that we talk about, Cohen's Kappa in this course reader, a lot of stuff. The point is that we just provide a lot of frameworks to really systematically solve the problems when you encounter challenges in coming up with good labels and ground truth.

**Hamel Husain** (01:10:37)

And so we teach you a lot of things like also how to correct the LM as a judge error rate based upon your real error rate and all kinds of advanced things. We also teach you how to think about multi-turn evaluations. Like, okay, if you have a long conversation that's like multiple turns between an AI and a human, how do you actually evaluate that? Um, do you evaluate the entire conversation? Um, you know, one piece of advice we have is like, you should, you know, evaluate, you should, when you're doing open coding, for example, you should stop on the first air that you see, because these things have causal relationships. And it's usually the case that the first air is the blocking, uh, is the blocking problem. And so a simplifying heuristic is to anchor on the first error. And there's all kinds of heuristics like this that make the entire process tractable.

**Hamel Husain** (01:11:34)

But also when it comes to evaluating multi-term conversations, how do you actually have test data sets for that? How do you simulate in multi-term conversation? Or do you need to simulate in multi-term conversation? There's a lot of things to dive in there. So we cover that. We also cover how to evaluate retrieval augmented generation. And so we talk about... when to treat certain aspects of the problem, like a search problem, what components of the problem, like the generation problem, how to think about that separately, and all the nuances there. And then we talk about other specific architectures and components. So like how to think about tool calling, what you need to know about agents. So agents are systems that can be very dynamic. They might have trajectories that are unpredictable and do various things that you can anticipate. How do you evaluate that? How do you tame that monster, that spaghetti?

**Hamel Husain** (01:12:40)

It turns out you can use various analytical tools that simplify the problem and allow you to attack it and make sense of agentic systems. And we show you things like how to use transition matrices and other analytical tools to help wrangle that problem. And then we talk about, you know, how to evaluate specific input data modalities, like different types of modalities and like not just text. Then we talk about production, productionizing these things. So like CI, CD, you know, kind of automating these and running these at scale. And then we talk about also kind of probably my second favorite subject in chapter 10 is interfaces. And I'll give it to Shreya to talk about the interfaces, actually.

**Shreya Shankar** (01:13:33)

Yeah. Chapter 10 and 11, they're the last week of the course. And they're kind of like special advanced topics that you will, I think I can guarantee that you won't find them anywhere out there on the internet. So we wanted to do something special for our students. Chapter 10 is about how to build perhaps even vibe code your way to an effective interface that has people really, really labeling things very quickly, maximizing the throughput of how many labels you can get from human reviewers. We talk about principles there to case studies of good, bad interfaces. And then chapter 11, I think, is about improvement. obvious strategies that you might know about, like decomposing tasks, fine tuning models, so forth, but also cost optimization and cost improvement. A lot of people actually say like, oh, my pipeline is working, but it's too expensive, especially if it's working on really long documents.

**Shreya Shankar** (01:14:33)

How do we keep the same quality, but reduce the cost by an order of magnitude or even more? Well, we talk about some cost optimization techniques there. So that's a very long answer, I think, to your question on, you know, what's the roadmap like? Here is a roadmap. We think it's pretty good. A lot of places you can dive in. You can dive into each chapter that you're interested in. And chapters 10 and 11 here, I think, are pretty open territory in research to explore more as well.

**Hamel Husain** (01:15:02)

so upon seeing this book a natural question is where can i get the book are you going to release this book and so the answer to that question is eventually yes maybe early next year however um you know if you want the kind of hands-on approach of you know doing this in in a very guided way then of course take our course

**Aakash Gupta** (01:15:27)

That's actually what I wanted to ask next, Helmel, is you were working at Airbnb and GitHub. Why did you transition into consulting and courses?

**Hamel Husain** (01:15:37)

Good question. It kind of happened somewhat organically. You know, I took a sabbatical after GitHub for a bit. I worked at some startups. And then I, sorry, after GitHub, I worked at a few startups. Then decided to take a sabbatical. Um, and a company decided to contract me. It convinced me kind of to, uh, the name of the company was weights and biases. They convinced me to, uh, do some consulting work for them. And so I, yeah, I always thought that like I would hate consulting cause I did consulting with a large consulting company very early in my career before tech, um, And I realized like, hey, I really like it when you're doing it on your own, becoming like an independent indie kind of entrepreneur. It's very enjoyable. It's a lot of freedom. And I found that a lot of people found it very valuable, like in terms of like helping them sort of navigate things.

**Hamel Husain** (01:16:42)

lms and ai um and then i just yeah i just started really enjoying it and one thing led to another and here i am like uh there's no let's say grand plan as such it's just uh kind of you know Yeah, it just like happened to be in this place. And it happened that everybody building with AI, they're always stuck on evals every single time. In this exact same problem, almost every single time I needed to start with error analysis. And this is like, you know, working with 25, 30 companies. You know, and then I just started writing about it a lot. And it was really apparent to me that there's not that much education on this topic. And it's where everyone's struggling. You know, and consulting is expensive. And so that's why we created this course to make this way more accessible to a larger audience.

**Aakash Gupta** (01:17:36)

And you tell people who want to consult you as a consultant to not reach out if they can't spend $38,000? Yeah. So

**Hamel Husain** (01:17:44)

I think one thing that you have to do as an entrepreneur is to... lot of different things but one is like it's important can be important to have a niche so that you customers know uh what you can help them with so in this case mine is evals and you know just from a practical perspective there's a lot of overhead that comes with being an entrepreneur like you you're in charge of your own sales your own marketing your own, you know, all the administrative overhead of it. And, um, you know, I don't want to be on sales calls all day. You have to qualify people and, you know, the problem has to be painful enough for them to want to solve it. And so that's just a kind of a basic kind of blocking, tackling approach to say, okay, like, how do I not drowned in zoom meetings?

**Aakash Gupta** (01:18:43)

And then the course, it costs roughly $2,000 and you have over 600 people in this cohort that me, Teresa, Pavel, other people are participating in. So does that mean you earned over a million dollars on this cohort of the course?

**Hamel Husain** (01:18:59)

Um, not, no. So we didn't quite cross the million dollar threshold because we gave a lot of stuff away for free. A lot of friends. Uh, we, you know, I let all my friends in basically, uh, Shreyo. We're also

**Shreya Shankar** (01:19:14)

very generous with any discounts for people who have any need. Basically, if your company can't reimburse it and you don't want to pay fully out of pocket, just email us with how much your company can reimburse. And we are super flexible. We want people to join the course. We have a steep price point because we find that we want to attract people who are serious about building AI products and evals. It benefits nobody if our course has 10,000 people and everyone's only mildly interested and serious. We want to focus on the people who are going to go and put these techniques into production. We're going to go build products. And for that, it turns out, you need to have a steep price point.

**Hamel Husain** (01:19:57)

So almost a million. I don't want to dodge the question because I know whatever. It's like almost a million. It's like 800K is what it was, the first cohort.

**Aakash Gupta** (01:20:08)

Which is insane. That's mind blowing, right? Especially for the first cohort of a course. And what's even more insane, I think, is that your next cohort is going to be your last. Why?

**Hamel Husain** (01:20:21)

Yes. So, I don't want it to be... You know how you, like, watch a movie and, like, the first one is good? And usually, like, it's really hard to make a good sequel. But it's, like, really impossible, like, to make it, like, continue to be good. And honestly, like, you know, I don't want to... You know, I have a lot of different interests, but also there's a lot of things that we can do with the course. So we could, for example, you know, you see this like 150 page. This is just a draft, honestly. I mean, we keep iterating on this book that we have open right now. Um, so one, you know, one sort of motion is to like, okay, focus time on writing a book. Then can, you know, it's currently it's a $2,300 course. We're going to actually be increasing the price $2,500 on Friday.

**Hamel Husain** (01:21:18)

Um, you know, can there be a recorded version that doesn't involve us like live that doesn't involve any office hours or anything else? Um, you know, that's like a lower cost. Okay. That's fine. So we think like there's different products out there that we can offer a different ways that we can offer this. Um, but But also like, you know, this course takes an immense amount of time to deliver. And so one of the things that we like to do is actually build these AI projects. Like I like to work with customers and build these things. I know Shreya does too. She likes to do research on this topic. Her research is very applied. She works with companies on this. She builds tools in the space. And it's really, yeah, if we do the course over and over again like this, we wouldn't be able to do that.

**Hamel Husain** (01:22:05)

It would actually dilute the course. So we want to keep it special. We want people to feel like, okay, if they were here for this course, it's something they could remember. You know, last year I had a course like this. It was not on this. It was on fine-tuning. It was... It was provisionally about fine tuning and then became like basically a conference. But it was basically the same scale as this course. It was like also a $900,000 revenue course in one cohort. And yeah, we decided like we don't want to do that again. Because how can we possibly recreate that subject and that feeling of that time? Yeah. You know, we don't want to do the second one and just have it be underwhelming because we try to repeat something. So like, you know, this is different. This is like, that was, you know, kind of a conference in a way.

**Hamel Husain** (01:22:59)

It turned into a conference. It was just like everybody about anything about LLMs. It was really fun. You know, this is like really focused on evals. We think that, okay, there's a lot more repeatability to this. But, you know, our goal is not necessarily... you know, trying to milk all the money out of it per se. We're actually like, you know, all this, this money that made, we actually like going to invest it in all these things. So like writing a book, um, you know, doing this additional, like different kinds of courses, like that are, can be delivered in different ways. You know, it's all going to be reinvested into that to make this material like accessible. Um, because we really believe we have a lot of conviction in this message and this topic and the impact of learning this.

**Aakash Gupta** (01:23:45)

I think there's a lot of lessons there for aspiring and current course creators. But I think one of the most interesting ones is how of the time you've made this course, like you're addressing the problems that you're seeing with your consulting clients and with AI engineers and AI PMs that they're facing with evals today. So you're able to write about it that way. You're not trying to just create timeless content. And I think that makes it really effective.

**Hamel Husain** (01:24:12)

Yeah, I hope so. I mean, you know, people message me and they're like, oh, this is a lot of money for like a month or whatever. But then I remind them, like, I've been writing about this for two years. I think Shreya has reviewed all of my blog posts throughout the years. Um, you know, I send it to her and she like reviews it. Uh, you know, I'm really grateful for that. Um, you know, and she's been writing about this for many years as well. Um, and by some stroke of luck, I was able to convince her to nerd sniper also and say like, okay, let's do this course together. Um, and I wouldn't have done it if she said no, it was only like, if she does it, then I will do it kind of situation. Um, Um, you know, because Shreya is, you know, if you look at her writing, it's actually really impressive.

**Hamel Husain** (01:25:01)

Like she, yeah, she like, um, it's a very good compliment cause I'm like really focused on consulting and stuff like that. I don't have time to survey the field, bring in, you know, like this like generalized perspective and theory, but there's a really good compliment there. where Shreya brings to, you know, structuring this material, bringing in, like, you know, a lot of the kind of... I mean, I didn't even know what axial coding... I was just doing axial coding, open coding. I didn't know it had a history in social sciences. So it was really good to know that there's actually some, like, history of this working. So things like that. I mean, I don't even know if I'm answering the question anymore. Yeah.

**Aakash Gupta** (01:25:46)

There was no question. So that was great. If you were to give advice to somebody who wanted to create a $800, $900,000 course, what would be your advice to them?

**Hamel Husain** (01:25:58)

Yeah. So one is, okay. So a lot of people ask me this question. Uh, let me try my best. One is to really find a niche that you are passionate about. I didn't think I was going to create a course around this, honestly. I've been writing about this forever. In fact, emails is one of the most unpopular things you can possibly write about or talk about. It's deeply, deeply unpopular.

**Shreya Shankar** (01:26:27)

yeah i really want to drive that point had we talked about something very cool and sexy like you know i don't even there's so many buzzwords out there like mcp and like agents and stuff right like that is a easy topic to write a course on because everyone wants to learn how to do it evals is something that everybody knows is a problem but doesn't want to go and put in the effort to doing so i think yeah my number one advice would be to find a If you want to do it the easy way, find a problem that people are excited about going and actually doing the work for, because you could probably 10x what we did for evals if you pick an exciting topic. But Hamill, you should continue.

**Hamel Husain** (01:27:09)

Yeah, I mean, I actually went through several nights or weeks or months or whatever of thinking to myself, man, am I swimming upstream? Like, you know, I talk about evals, I build... Sorry, built my consulting around evals. But like, you know, you know, it's like telling people to eat their vegetables. You know, it's not really that popular. And, you know, it's much easier to talk about agents. You know, if you did some like background research, if you try to come out of the perspective, like, hey, I should build a course, I want to like build a course, you would never pick evals, you would pick agents. You'd be like, okay, I'm going to sell an agent course. Everyone wants to learn about that. People are actively Googling. If you do like SEO research, like what are like the keywords people, like almost nobody is like searching for evals.

**Hamel Husain** (01:28:01)

There's very little competition for that keyword actually. Like if you search for evals, like, Shreya, myself, Eugene, basically our friends, like Shreya, me and our friends. And I'm talking about our friends, meaning the friends that Shreya and I have in common. We all are come up on like, you know, at the top of the list. It's pretty insane. It's like, that's how niche or quote niche it is. But, you know, at some point I just didn't care. I was like, we need to create the category. So, you know, it's not popular. You need to make it popular. So I don't know if that's good advice. That was my mindset, but I can tell you the only reason that allowed me to get into the mindset is because Shreya partnered with me. And so one thing I would say is like, find a good partner to partner with you.

**Hamel Husain** (01:28:51)

So like to get into the mechanics, like, You know, a lot of course sales has to, you know, marketing is very important. You need to let people know that the course exists. Otherwise, they can't buy the course. We don't know. And they not only need to know it exists, they need to know, like, what it's about. They need to get excited about it. They need to know, like, it's good. They need to know, like, you know, need to have some social proof or need to have, you know, some idea, like, people like it. Their peers get value out of it, all of these things. And they need to be reminded about it constantly because, you know, I need to be reminded about things constantly for anything. So, you know, all of this is very, very important. And so that's a full time job. You know, and so if you want a course that you want to sell a course like that, like you have to spend a lot of time doing that.

**Hamel Husain** (01:29:50)

And can you outsource that marketing? You can definitely partner with people in marketing, but you kind of have to drive it because you are the subject matter expert. You're the domain expert. You know, you know, you have to build that authority and that connection with your audience because, you know, whatever. You know, just relentless focus on that.

**Shreya Shankar** (01:30:22)

You know, we're talking about X, Y and Z. So and so is like the world's leading expert on X. Like Y has been applied in these three companies. So let's get somebody from there. This the guest speakers are really diverse and I think really distinguish also our course from a lot of other courses out there. It's not just us monotonously lecturing. It's we've got other people coming in, showing you how these things are implemented in practice at big companies, at small companies, at specific domains or whatnot.

**Hamel Husain** (01:30:55)

Another thing is focus. Yeah. This is like, I get up in the morning. All I think about is the course and how can I let more people know about the course or like, you know, make it better for students. Um, how can I bring more perspective into there? So on and so forth. Yes, all that stuff is really important. And just constant experimentation. So kind of going back, it's kind of like a, you know, I'm a data scientist kind of thinking person. I'm just constantly doing experiments and looking at the data. And, you know, I send Shreya like probably the average of 200 text messages a day or something like that with like different experiments. Like, I was like, oh, I'm trying this. I'm doing this thing. Look at these numbers. Okay, like, what do you, like, this marketing copy, this here. Like, we put an ad here.

**Hamel Husain** (01:31:44)

This is what happens. Do you have any ideas for, like, how we can go about this differently? Whatever. You know, hopefully she has do not disturb on, I hope. But, you know, so, yeah. I mean, this is, like, constant experimentation. So, you're kind of treating it like how I treat evals. to be meta is like, you know, this like iterating on, you know, the business of making the core. And the thing that's like really good about making money in a course is like, you can, I've hired a lot of my friends, you know? And so like, you know, a lot of my friends are data scientists, machine learning engineers, and you know, a lot of them are involved in one way or the other, either as affiliates or guest speakers or TAs. And I pay all of them. Uh, and it's great. I love paying them.

**Hamel Husain** (01:32:36)

And yeah, it's like really great. Like all my friends win too. And that's like the good part is, you know, to create that situation where everybody wins.

**Aakash Gupta** (01:32:49)

What a great place to end it. If people want to find you guys online, where should they go?

**Shreya Shankar** (01:32:54)

Yeah, we're both active on X. You can pretty much just search us up. You'll find us. I have a blog. Hemel has a blog. Email us. Yeah, nothing super fancy, I think.

**Aakash Gupta** (01:33:09)

Where do they find your email?

**Shreya Shankar** (01:33:12)

The best way to do it is just to Google us and our email is at the top of the page. But I can also, my email is first name, last name, Shreyashankar at Berkeley.edu.

**Hamel Husain** (01:33:28)

And mine is just get in touch with me at X on X. It's easy. You know, you can send me a DM there. You can message me, whatever, and I'll figure it out.

**Aakash Gupta** (01:33:39)

amazing thank you guys so much for lending your expertise we'll see everybody in the next one so if you want to learn more about how to shift to this way of working check out our full conversation on apple or spotify podcasts and if you want the actual documents that we showed the tools and frameworks and public links be sure to check out my newsletter post with all of the details Finally, thank you so much for watching. It would really mean a lot if you could make sure you are subscribed on YouTube, following on Apple or Spotify podcasts and leave us a review on those platforms. That really helps grow the podcast and support our work so that we can do bigger and better productions. I'll see

<!-- sponsor -->
**Narrator** (01:34:22)

you in the next one.
