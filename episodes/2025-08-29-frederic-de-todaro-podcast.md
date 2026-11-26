---
title: "Complete Course: AI Experimentation"
subtitle: "Every way that AI has changed experimentation"
date: "2025-08-29"
host: "Aakash Gupta"
guests: ["Frederic de Todaro"]
speaker_names: "substack"
substack_url: "https://www.news.aakashg.com/p/frederic-de-todaro-podcast"
youtube_url: "https://www.youtube.com/watch?v=MC1FfWdAyX4"
duration: "01:02:34"
word_count: 9753
source: "Substack episode transcript (aired audio)"
sponsors:
  - name: "Mobbin"
    url: "http://mobbin.com/aakash"
  - name: "Jira Product Discovery"
    url: "https://www.atlassian.com/software/jira/product-discovery"
  - name: "AI Product Strategy Certificate"
    url: "https://maven.com/product-faculty/ai-product-strategy-certificate?promoCode=AAKASH550C1"
  - name: "Maven"
    url: "http://maven.com/x/aakash"
---

**Sponsors:** This episode is brought to you by [Mobbin](http://mobbin.com/aakash), [Jira Product Discovery](https://www.atlassian.com/software/jira/product-discovery), [AI Product Strategy Certificate](https://maven.com/product-faculty/ai-product-strategy-certificate?promoCode=AAKASH550C1) and [Maven](http://maven.com/x/aakash).

# Complete Course: AI Experimentation

*Every way that AI has changed experimentation*

**Aakash Gupta** (00:00:00)

How has AI changed experimentation?

**Frederic de Todaro** (00:00:02)

Fred De Todaro is one of the world's most knowledgeable people on AI and experimentation. What company do you think is doing

**Aakash Gupta** (00:00:09)

experimentation best?

**Frederic de Todaro** (00:00:19)

I'm not going to choose the usual one, like Netflix, Airbnb, Microsoft, and so on. I'm thinking about a

**Aakash Gupta** (00:00:26)

company called Booking.com. What are the biggest mistakes PMs make when it comes to experimentation?

**Frederic de Todaro** (00:00:33)

I think the top three I hear the most about is to slow down.

**Aakash Gupta** (00:00:39)

How would you define the roles of PM, data scientists, and AI analysts?

**Frederic de Todaro** (00:00:44)

The PM, the data scientists, have to work together to make sure that the business context is there, the constraints are known. How has AI changed experimentation over time? If you look at the past, I think there has been two big waves in the end. The machine learning wave, which started around 2016, and then the generative AI wave,

**Aakash Gupta** (00:01:03)

which really kicked off in 2022. What is the precise difference, and what exactly are these banded algorithms? Talk to me a little bit about content generation. Do you have any stories yourself that your team has used? So content generation, so basically

**Frederic de Todaro** (00:01:16)

you take content on your website and then you ask the AI to come up with an alternative version of it, right? So that's the goal of content generation.

**Aakash Gupta** (00:01:23)

This is one of the coolest demos out there. Would you be willing to show us how this all works? Fred, welcome to the podcast. Hi, thanks for having me. So, Fred, has AI really changed experimentation much?

**Frederic de Todaro** (00:01:38)

Yeah, AI has been the biggest driver of changing experimentation I've seen in my career.

**Aakash Gupta** (00:01:43)

How has AI really changed experimentation?

**Frederic de Todaro** (00:01:46)

Yeah, sure. So maybe let's take a step back for a second. So if you look at experimentation, Well, it usually comes down to four simple steps. You have an idea, then you make an assumption. If you release that feature in production, it will increase by X, that metric, because of these reasons and these reasons. And then you build the experiment, the variations, then you set up the targeting, you know, who are you going to target with that experiment? Is it all your users or a segment of users? And then the KPIs, which is an important step as well. How will you measure the success of that experiment? And then you look at your results, right? So it's a simple loop, right? So you iterate as long as you learn something with your experiments.

**Aakash Gupta** (00:02:35)

Okay, so there's four steps, and I imagine you're going to map this against how AI affects each of these four steps?

**Frederic de Todaro** (00:02:41)

Yeah, exactly. If you look at the hardest part of experimentation, it has always been the build phase, right? That's why over the past decade, most of the experimentation tools have been introducing some visual editor to build variations or to let anyone create some variations. Even dedicated feature experimentation vendors have been introducing them very, very recently. But the truth is no one really delivered on that premise today. Most tools still rely a lot on developers. They are already busy building the next features in your roadmap. And so as a result, most teams do not AP test the majority of what they deliver to their users. And they'll run meetings to just prioritize the best experimentation that might be worth building. And then they wait one or two sprints to see anything go

**Aakash Gupta** (00:03:37)

live. Yeah, I think this is an important point, right? If we look at the lifecycle of experimentation between ideate, build, configure, and analyze, build is the bottleneck. That's kind of the... tragedy of the commons that we're all facing where very few teams are actually experimenting a high percentage of their releases. And it seems like that's the area where AI could be the most interesting. Before we get into that build phase, I want to talk a little bit about the idea phase, right? So we have here, you know, it's a three out of five difficulty, perceived difficulty for folks. But how powerful can AI be in ideation?

**Frederic de Todaro** (00:04:17)

Well, it can be, it can be powerful. When you look at the history, I think it has been possible during the generative AI wave. So back in 2022, so you were able to ask an AI to give you some ideas, right? Limited to content generation at the beginning. But then, since the release of the latest model of GPT, for instance, GPT-4, well, things have changed a lot. You can really ask the AI to come up with some ideas. You provide a page and then the AI will try to come up with some ideas. And so this is where it's starting, right? Because the AI, to some extent, has or can assume some context. You know, what's your business about? Who are your users? What is the framework that you use behind your website? And so with all that context, then the ideas generation is possible. And so we'll see some of it later during the demonstration as well.

**Aakash Gupta** (00:05:22)

Okay, so I think that this is a really, really powerful set of techniques. Like the way I personally have been coaching people to deploy this, if they don't have it built into their experimentation tool is, what you want to do is you want to set up the AI with all that context that you mentioned. And you want to take advantage of the latest AI feature. So I'll do something like, Either have a really strong prompt that has context on features we've shipped in the past, the reason we have certain messaging, the metrics that we have seen, or better yet, create something like a cloud or a chat GPT project, depending on whatever AI you have access to at your work, that loads it up with all of this context. so that you can then ask it the right questions and maybe even include a screenshot of the image.

**Aakash Gupta** (00:06:12)

It feels like the better the context you can engineer for the AI, the better the ideas it'll spit out. Yeah, absolutely. Absolutely. So in the build phase, there's obviously a lot that we can build with AI. People are probably familiar with building with AI, AI IDEs like Cursor or Windsurf, prototyping with AI prototyping tools like Lovable, Bolt or Replit. But before we get there, we got to stay on this configure step, right? What is the right way to use AI to configure an experimentation experiment that you're going to do? Where should you, the human, be putting an input and where should you be relying on the AI?

**Frederic de Todaro** (00:06:55)

Yeah, it's a good question. I think the role of a product manager is still, you know, absolutely critical there. And same for the data analyst or the data scientist. You know, they are all working together and better in a way. As a product manager, Well, your role is still to bring the business context that the AI does not have. Sometimes you need to deliver that feature for a customer. The AI does not have that context, right? The PM comes with all the internal constraints that the AI does not have. Why are we working on that idea? What is the assumption in the end? And what success will look like as well when you ship that feature? That's the job of the product manager, right? And then the data scientist is still there as well. And I think it is kind of the essential human in the loop that you need.

**Frederic de Todaro** (00:07:48)

when you need high confidence in the data that you are collecting in your experiments or things like, you know, what is the right model to use? Is it, you know, rag versus fine-tuning model and so on? So the data scientist is still very, very important. And he's also going to challenge basically the AI's output, right? Is the data biased as well to some extent? Are the results, you know, plausible? That's the job of the data scientist. So if I had to sum up, the AI makes, I would say, the whole experimentation process, you know, faster and more accessible to the whole organization. For example, the AI can fully determine or identify patterns, you know, and suggest some recommendations when an experiment is non-inclusive. You would normally do that, you know, by digging into the data manually or, you know, and it's not possible here. Behind human scale, there are so many data points to crunch and so on.

**Frederic de Todaro** (00:08:50)

So the AI is fully capable to do that. But then, you know, the human in the loop is very, very important, both at the product management level and I would say at the data or data scientist level.

**Aakash Gupta** (00:09:02)

I think that really sums up very nicely the profiles that each person needs to take, right? So if I were to repeat it back, the product manager, they're going to be the person who's taking in all the context and helping to come up with the initial idea. where they prove that context into an AI system. That AI system gives you some initial configuration options. The PM might sanity check that. And then the PM needs to bring in or work with the data scientists or have a process where a data scientist comes in and they're further challenging and hardening the assumptions. And so there's kind of two human in the loop steps, but the PM is really using the AI to make sure that that first version is strong.

**Frederic de Todaro** (00:09:42)

Exactly, exactly. And then the AI can really build that variation for you as long as you have very good hypotheses and some metrics on which you will backup your measurement

**Aakash Gupta** (00:09:58)

there. And then analysis of features. How would you define the roles of PM data scientist and AI analyst?

**Frederic de Todaro** (00:10:07)

Yeah. So, I mean, like I said, I think the AI is today fully capable to give you a summary of, you know, what happened when that experiment was running for your users. It is also able to, you know, identify patterns. Like, you know, if your experiment is, you know, not providing what you are expected, sometimes by, you know, drinking down the data, by, you know, breakdown in the data, by, I don't know, device type of users and so on, you will spot out some opportunities to do better. And that AI can do that for you. You don't have to do that anymore. There are some, you know, many experimentation vendors who have released such capabilities as part of their offering because there is nothing very complex there and the human at that stage, you know, does not have to be, basically. Again, the PM, the data scientists have to work together to make sure that the business context is there, the constraints are known.

**Frederic de Todaro** (00:11:11)

And that the metrics on which you will measure the success of that experiment are clearly defined and measurable as well. If you run an experiment that you are not able to measure the success, well, that's the point, right? And the AI will not help you. So again, both the PM and the data scientist and the AI now are working together and better in a way.

**Aakash Gupta** (00:11:39)

So if we had to summarize here, in the ID8 phase, sure, AI is doing some, but it's really just a co-pilot. In the building phase, AI is getting to the phase and we're seeing a future where AI can really dramatically do most of the build for you. And in the configure phase, again, AI can really dramatically do most of it with some human in the loop review. And then in the analysis phase, again, it can do most of the basics as long as you have predefined the right metrics, the right North Star, the right guardrails, the right secondary metrics. It can go ahead and look at those. And so it's really that ID8 phase where humans need to stay super connected. But all these other steps, it feels like AI is going to be taking over most of the workload.

**Frederic de Todaro** (00:12:24)

Yes, yes, exactly, exactly.

**Aakash Gupta** (00:12:26)

So for PMs, product sense here and becoming a great experimenter and coming up with great ideas is really going to be the most important thing to becoming a great experimenter.

**Frederic de Todaro** (00:12:37)

Exactly, exactly. I mean, if you look at what a product manager, you know, does in the end, it identifies, you know, features to improve the user experience, but also, you know, the business, right? And so I don't think that what's preventing today PM to experiment is the lack of ideas. Usually they have already a long backlog of ideas to test there. For sure, AI can come and validate some of these ideas. You know, you provide some context to that, and then the AI can tell you, yes, this idea has a high chance to succeed, especially because when AI is fully connected to your, I call it the experimentation knowledge base, because maybe you have been running, you know, tons of experiments by the past and so on. But AI can tell you, you know, this thing has been tested already by the past. Here are the results.

**Frederic de Todaro** (00:13:30)

And maybe you didn't know it because another team had run that experiment already by the past. And so the AI can also bring some context from history. I like to call it UX memory in a way because you come up with an idea as a product manager and then the AI will pop up there saying this thing has already been tested. And here are the results that were, you know, discovered at that time. Do you want to go and proceed with that idea? Because maybe you can test it again. Your users may have been evolved. You have new behavior. Your website has changed and so on. So that's something really, really important that the AI can come as well with UX memory, which

<!-- sponsor -->
**Aakash Gupta** (00:14:11)

is very, very important. Today's episode is brought to you by Jira Product Discovery. If you're like most product managers, you're probably in Jira, tracking tickets and managing the backlog. But what about everything that happens before delivery? Jira Product Discovery helps you move your discovery, prioritization, and even road mapping work out of spreadsheets and into a purpose-built tool Transcription by CastingWords That's A-T-L-A-S-S-I-A-N dot com slash product dash discovery. Jira Product Discovery. Build the right thing. Today's episode is brought to you by the AIPM certification on Maven. Run by Mikdad Jaffer, who is a product leader at OpenAI, this is not your typical course. It's eight weeks of live cohort-based learning with a leader at one of the top companies in tech. OpenAI just doesn't stop shipping, and this is your chance to learn how. Run along with Product Faculty and Mo Ali, the course has a 4.9 rating with 133 reviews.

<!-- sponsor -->
**Aakash Gupta** (00:15:31)

Former students come from companies like OpenAI, Shopify, Stripe, Google, and Meta. The best part? Your company can probably cover the cost. So if you want to get $500 off, use my code AAKASH25 and head to maven.com slash product dash faculty. That's M-A-V-E-N dot com slash P-R-O-D-U-C-T dash F-A-C-U-L-T-Y. I want to dive into that in a little bit in a second. But before we get there, let's take the historical point of view on this. How would you break this down historically? How has AI changed experimentation over time?

**Frederic de Todaro** (00:16:05)

Yeah, if you look at the past, I think there has been two big waves in the end. The machine learning wave, which started around 2016. So we started to see some machine learning, you know, algorithm coming out. And then the generative AI wave, which really kicked off in 2022. And so if you look at the machine learning phase, I think AI helped, you know, removed some key bottlenecks like, you know, finding the right users to target with AI targeting, for instance, or allocating traffic to the best variant. And we saw multi-arm bandit, you know, contextual bandit. you know, being released there and analyzing results as well. You don't have to use a generative AI to analyze to some extent some results. So machine learning can do that as well for you. And so they have all been designed to some extent to help teams optimize, I would say, faster and, you know, adapt in real time, right?

**Frederic de Todaro** (00:17:11)

And then there has been the generative AI wave and that changed, you know, everything there. with the rise of content generation to quickly create some copy variations. Because at the beginning, I think models were only good at this, to be honest. So many, many vendors outside of the experimentation world started to include content generation. If you go to Notion, you had to generate that content for me. I want something more fun, blah, blah, blah. So you started to see this kind of, you know, features being released in any tool. Then AI assistant as well started to pop up, you know, often RAC based. They help, you know, answer any question, interpret results or support users, you know, inside the platform. So that was, you know, one year later. And more recently, especially at the end of 2023, things are still accelerating so much. I mean, with GPT-4, oh, it was a new parting.

**Frederic de Todaro** (00:18:20)

And new model, you know, like, again, GPT-4 changed what people thought, you know, that was even possible. And suddenly, vibe coding became a mainstream, like nine months ago, vibe coding became mainstream there. And I mean, if you look at experimentation, it changes everything as well, because it means that you can turn any idea into a running experiment just by prompting an AI. And that's why, you know, at Camelot, we released the prompt-based experimentation so that anyone in the organization, you know, HR, finance, product manager could directly come up with an idea. I want to improve that there. You provide that prompt to an AI and then the AI will come up with a variation and an experiment that you can directly test in minutes and not anymore in a sprint or two sprints, depending on your organization velocity.

**Aakash Gupta** (00:19:21)

So let's take a step by step on some of these for people. Now that we got the broad stroke of how things go, right? In the beginning, we use AI to improve targeting. Can you say a little bit more about this? Is this about AI selectively showing which person gets which experience or how do you use AI correctly in targeting?

**Frederic de Todaro** (00:19:44)

The main purpose of AI targeting is to predict what you will do. Let's say you browse a website, the AI is fully capable to give you a score, which is a conversion intent. What is your likelihood to convert? And so with AI targeting, we kind of try to replicate what the sales do, does, you know, when someone enters a shock, good sales will understand if you are in a, you know, about to buy or not. depending on how you're dressed, how you move in the shop, what kind of products you look at, and so on, the sales will score you. And so we tried to reproduce that behavior on the web. So as soon as a visitor lands on a website, and depending on what you do, what you consult, and so on, the AI will score you. And then customers can use that directly to target the right users instead of creating a segment manually, you will just use the score which is provided by the AI.

**Frederic de Todaro** (00:20:47)

So it changes everything in terms of, you know, at the configure stage where you set up the segment, you want to target with that experiment, well, you don't do that anymore. You just use the score from the AI. It's very similar to multi-hand bandit or contextual bandit, but the role of the purpose is a little bit different.

**Aakash Gupta** (00:21:08)

I think this is actually really powerful, and I want people to look at the left side of the screen. I want people to look at these older things because these are actually probably the most mature and, in my opinion, probably really strong to just use in production, right? So if I'm understanding this correctly, right, this is these old-school... machine learning models, which are essentially really strong gradient descent algorithms, really strong regression models, which are looking at the user behavior to say, okay, this is the user that maybe is very high intent to churn off. So maybe we should give them a higher coupon to keep them here or give them something to keep them here. Or maybe they're looking at their beaver and saying, this is a user who is almost ready to purchase. So maybe we should just help them get onto their purchase right away.

**Aakash Gupta** (00:21:53)

So it's really about in sort of real time, based on the user behavior, you can rank your users and you can show them personalized experiences.

**Frederic de Todaro** (00:22:02)

Absolutely.

**Aakash Gupta** (00:22:03)

Absolutely.

**Frederic de Todaro** (00:22:03)

Many customers have been using that for, you know, showing a coupon to the right users. So I'm sure, you know, every time you visit a website, you always have that pop-up. I that comes there providing you 10% straight away. But instead of doing that, maybe you should keep that 10% there and provide it to the users that are in need of that percentage of discount to buy, to go to the next step and buy. So that is the main goal of AI targeting.

**Aakash Gupta** (00:22:36)

Love it. And you said it's adjacent and similar to multi-arm bandit and contextual bandit. I feel like I want to really tease this out for everyone listening. What is the precise difference and what exactly are these bandit algorithms?

**Frederic de Todaro** (00:22:50)

Yeah, sure. So if you look at a standard A-B test, usually your goal is to know if, you know, variant B actually improves a specific metric. And so you split your traffic equally, and when you wait, you know, a sample size, and then you have enough data, you can make your decision, right? With multi-hand mandate, the focus is on performance. So the AI will gradually allocate, you know, more traffic to the, I would say, the best performing variant based on the data you have at that time, right? But there is a trade-off. I mean, I like multi-unbanded there, but there is a trade-off. You lose some accuracy in the data. because the AI starts making some decisions based on a smaller sample, which is fine. I mean, to some extent, in some use cases, it makes a lot of sense, like in the media, where you need usually to know sometimes within a day which article headline drives more, I would say, clicks or engagement.

**Frederic de Todaro** (00:23:59)

So you don't care that much about the accuracy. Your goal is to make sure that you push the best headline to all your users. So that's multi-hand bandit. Contextual bandit on the other hand is a little bit different. You have a bunch of variation, like let's say 10, 100 of variation, and your goal is to push you know, variation one to the group of users that prefer version one. And you push version two to the segment of users that are in love with that variation. So your goal is to learn and adapt. So it's still based on machine learning algorithm. And so the goal is really to push the best variant to each individual user.

**Aakash Gupta** (00:24:44)

So it sounds like if you have something highly time sensitive and you're okay with potentially slightly less confidence in the results, go for one of these multi-armed contextual bandit type things. Yes. And within those, can you just tease out really carefully so that I understand it, what's the difference between multi-armed and contextual? What's the difference, right, you said? between a multi-armed bandit and a contextual bandit?

**Frederic de Todaro** (00:25:09)

Contextual bandit. So multi-armed bandit, your goal is to push the best variant to all users, right? With contextual bandit, you push to each user the variation but, you know, is the most performing for them. So in the end, it's like, you know, having a website which is fully personalized. You know, every user will not see exactly the same offering, the same content. So that's highly advanced. I'd like to say it's more tailored for personalization where your goal again is to adapt to the content. based on each user preference

**Aakash Gupta** (00:25:45)

in the end.

**Frederic de Todaro** (00:25:46)

So when

**Aakash Gupta** (00:25:47)

should you be using which? Which industries, which types of organizations should have the headspace of using one or the other? I

**Frederic de Todaro** (00:25:56)

think media, as I said, for multi-end mandate makes a lot of sense because usually you don't want to run an experiment on the headlines or article titles. Your goal is to go with the best one as soon as possible. Contextual bandwidth appeals to any kind of industry. If you have, you know, let's say a coupon, for instance, you have 10%, 20%, and 30%, well, you let the AI push right percentage depending on each user. So that's one usage of contextual bandwidth as well. Or if you have you know, multiple home pages with different contents and so on. And your goal is not to A-B test or to know which homepage is the best. Your goal is to push the best homepage to each individual user. So you are really, you know, in the hyper-proposalization way of seeing experimentation here.

**Aakash Gupta** (00:26:55)

It sounds like probably Your e-commerce and those types of things are doing a lot more contextual bandit where they have a lot more users, the ability to personalize maybe your social media and probably more your B2B type of things are using more multi-armed where they just have one experience that they can refer to. Is that a high level fair or is there some what is the nuance to that?

**Frederic de Todaro** (00:27:17)

Yeah, well, that's for sure is that you need a lot of traffic for both usually, because again, as you need to make decisions very fast, you need a lot of traffic, right? If you have less than 100k, I would say of visitors, you know, per month, Maybe, you know, that's not the best approach there. But when you look at media, they have millions of, you know, visitors every month. So that's not a problem at all, right? And for Contextual Bandit, as, you know, the goal again is to learn and act based on that learning, well, you need to learn a lot of behaviors before, you know, starting to push, you know, variation one to that user or variation two to that user. So it appeals to customers with some significant amount of traffic in the end.

**Aakash Gupta** (00:28:05)

All right. And then let's marinate a little bit on this opportunity detection. This was happening right at the end of the machine learning wave. What does this enable you to do in your experimentation?

**Frederic de Todaro** (00:28:16)

Yeah, so the reason we've built or we've seen this kind of feature is because if you look at the broad statistics of experimentation, well, less than 20% of them are successful, meaning that when you ship that feature, well, 20% of the time it will increase the metric that you want to improve with that experiment. And so most of the time when that happens, you see a lot of data analysts trying to drill down into the data to understand why it happens and to see there is an opportunity to do better. Because in the end, maybe that variation does not work for all of your users, but maybe if you drill down, you start to understand that maybe that feature works well for mobile devices users. And so, instead of doing that manually, AI opportunity detection does that automatically. as soon as an experiment is non-conclusive, it is showing a downlift on a metric, then that AI will start crunching the data and point out some opportunities to do better.

**Frederic de Todaro** (00:29:30)

Like again, this variation is performing well on mobile devices. Maybe if you personalize the experience for mobile device users and you show that variation, you will increase the performance. of your website and ultimately the revenue of your website. So that's the main goal of AI Opportunity Detection. It's trying to spot out some opportunities to do better.

<!-- sponsor -->
**Aakash Gupta** (00:29:55)

Yeah. If 80% of what you're shipping isn't going to hit your metrics, you want to make sure that you're still learning something from that 80%. And so this is really going to help you in that step. Before we dive deeper, let's talk about something every PM faces, getting alignment on product decisions. You know that feeling when you're trying to explain a user flow to engineering or justify a design choice to leadership and you're just describing it with your hands? That's where Mobbin comes in. Mobbin is the world's largest library of real-world mobile and web app designs from industry-leading apps like Airbnb, Uber, and Pinterest. Instead of spending hours taking screenshots or hunting for inspiration, you can instantly find exactly how successful products handle onboarding, paywalls, checkout flows, whatever you're facing. Over 1.7 million product builders use Mobbin to benchmark against best-in-class products and show their team's proven solutions.

<!-- sponsor -->
**Aakash Gupta** (00:30:47)

Whether you need to convince stakeholders there's a better way to handle user activation or research how top apps approach future discovery, Mobbin gives you the visual proof to back up your product decisions. Check out mobbin.com slash Akash. That's M-O-B-B-I-N dot com slash A-A-K-A-S-H. You can get 20% off your first year. Today's episode is brought to you by Maven. The problem with most courses online, like Udemy, is there's no live component, and the instructors aren't experts in their fields. They're professors. At Maven, you get direct live access to experts and operators from the world's best tech companies. You can't get that access anywhere else, in any university, and you usually can't find them on YouTube either. I've featured so many of Maven's experts in the newsletter and podcast for that reason. To help you out, I've put together a collection of courses I recommend at maven.com slash x slash Akash.

<!-- sponsor -->
**Aakash Gupta** (00:31:38)

This includes courses like AI prototyping for PMs, Product Sense for PMs, and getting an AI PM certification. Visit it now at maven.com slash x slash a-a-k-a-s-h. Talk to me a little bit about content generation. I'm curious, do you have any stories yourself that your team has used where AI content generation has led to a win?

**Frederic de Todaro** (00:32:03)

Yeah, we see that a lot. So content generation, basically, you take content on your website and then you ask the AI to come up with an alternative version of it. So that's the goal of content generation. So we have seen users putting that kind of experiment when they try to create some pop-ups, for instance, or some messaging for banners and so on. They want to make sure that they have the best performing content. And so they use AI for that. They will generate content there to make sure that, again, they increase the engagement. Because sometimes, you know, you come up with a version and you like to, you know, engineer that with a prompt. You're asking, you know, give me a better version for that goal. I'm sure everybody is doing it today. Even myself, I'm doing it every day. I go and I say, okay, I'm doing a podcast with Akash.

**Frederic de Todaro** (00:32:58)

Can you provide me the best thing I should say? And so I provide my content and then I generate something which is appealing for a podcast.

**Aakash Gupta** (00:33:09)

Love it.

**Frederic de Todaro** (00:33:10)

Talk to me

**Aakash Gupta** (00:33:11)

about RagAssist.

**Frederic de Todaro** (00:33:13)

Yeah, RagAssist, so this is the era of chatbot, basically. So we have that in our tool today. So the idea is to, you know, have an AI that, you know, users can interact with to get answers to anything like Git. You know, I have that experiment there. Tell me what is the best, I don't know, stat engine to use for that experiment. We know that it is increasingly complicated. You have, you know, Frequentist, Bayesian, sequential testing, and so on. So users are like, okay, which one should I choose? And so you can go and talk with that AI there. The AI will ask in context, like, okay, what is that experiment about, blah, blah, blah. And then the AI will tell you, for that experiment there, you should use a Cupid, for instance, because I know that you have some history of data on the metric you want to improve.

**Frederic de Todaro** (00:34:05)

If you use that, you can, you know, decrease the duration of your experiment by maybe two weeks. So that's the main goal of AI Assist. We've seen also that kind of feature being very useful for generating some code. For instance, some of our customers do put in place some feature flags. Well, it's very annoying to look at the documentation because you have a lot of methods to look at and so on. So you can go and talk with that AI and say, okay, I have this feature there. I want to release it behind the feature flags. I want to verbalize some behavior of a feature while providing me with a code. And so you can directly go and interact with that AI that will generate, you know, some steps to put in place, you know, by using some SDKs so that you can go with your feature flags as soon as possible.

**Aakash Gupta** (00:35:02)

This is huge. I feel like this is like the co-pilot, right? This is all about, especially if it's built into your experimentation platform, you being able to converse with it. Now you dropped two pieces of experimentation knowledge there that people's ears probably perked up on. And I want to at least give them the quick overview on. So you talked about frequentist and Bayesian statistics. So can you unpack that for us first?

**Frederic de Todaro** (00:35:29)

Yeah, sure. So there are usually two, you know, methods to kind of analyze the experiment. So we look at, you know, the statistical confidence of the results you are looking at, because, you know, an experiment is basically a statistic experiment. You take a decision based on the data that you have at one point of time. And so you can use a frequentist approach, which is usually what most of the users will use. This is a default statistical engine there. Then there is a Bayesian, which gives you a probability. That variation has 80% chance of being better than the original or the control. So, you know, it's like having two schools here. Some will love Bayesian, some will love Frequentist. What we see is that usually 90% of the market, you know, they go with Frequentist there. And then you have Cupid, which is another statistical method, which is very powerful, especially if you have a lot of returning users in the B2B, for instance, industry.

**Frederic de Todaro** (00:36:41)

that's very powerful because it takes some data as an input so that when you start your experiment you actually have two weeks of you know metrics already available and so ultimately it means that you can get some results much faster than if you start you know from scratch. So they are all designed, you know, to answer a specific case. But in the end, your goal is to make sure that you are taking the decision with the best accuracy. And so all these statistical engines are, you know, very powerful and very known by our customers and users in the experimentation industry.

**Aakash Gupta** (00:37:22)

And it's Cupid, C-U-P-E-D, right? Yeah. All right. So one of the coolest things that you talked about as you were previewing the Gen AI wave was how the vibe coding has really changed experimentation. Can you unpack this further? What has vibe coding enabled with experimentation?

**Frederic de Todaro** (00:37:45)

Yes, it's a good question. So what vibe coding really has unlocked is this ability to take a product idea from a concept to a live prototype. And in just a few hours, right? So it helps you build things, you know, faster. And I love it. I mean, we are, I think, all using, you know, vibe coding in the product management ecosystem today, like Lovable or Bolt. You know, you have your idea and you get a prototype that you can then test with your users. But... As a product manager, my goal isn't to just, you know, build and deliver faster. It's to learn faster, right? You want to make sure that when you ship that feature, you are able to learn, you know, some insights so that you are sure that, you know, that feature is actually being used and increases, you know, I would say the user experience, but also the business outcomes, which are also very, very important there.

**Frederic de Todaro** (00:38:46)

And so that's important because that way I can kill features, I can drop the features that don't bring any value to my users or to the business. So that's what ViveCoding unlocked. You go from an idea to a prototype that you can test with all your users. But the real question to me isn't, can you build it? It's really, should you build it, right? And so that's why experimentation is very important because experimentation answers that question there. Should you build that feature or not? And so that vibe coding won't help that much with that. Well, for sure, you can test this prototype very quickly. And again, it's outstanding and so on. So you can test that with a few users and that's very great. But the truth is, you will only really know, and I want to say that loud here, if it works, you will only know if it works when that feature will be going live to all your users.

**Frederic de Todaro** (00:39:52)

Because I've seen it so many times. I mean, users say, They want something, they say they like it when you show a prototype, and then once you launch it to everybody, you launch it broadly, well, nothing happens, right? And I'm sure you've got that as well as

**Aakash Gupta** (00:40:11)

a

**Frederic de Todaro** (00:40:11)

PM by the past. And so, prompt-based experimentation sits right at the crossroad of VIPE coding and experimentation. We actually call it an internative vibe experimenting because you can read the same concept in the end. You can test ideas in minutes just by prompting the AI, and you do it right from your website or your web application. You don't do it from a blank page. You go to a website, you prompt your idea, then the AI will generate that feature or that variation, and then you can test it directly with all your users. So you get basically the best of both worlds here. The speed and creativity that is provided by, I would say, VibeCoding with prototyping, you know, but directly from your web apps. And I would say this... structure or maybe the discipline of real testing to make the right protocols. You are sure that when you get the data about that experiment, you know or you do not know if that feature will improve your metric.

**Frederic de Todaro** (00:41:19)

And so this is very, very important.

**Aakash Gupta** (00:41:22)

All right, so that about covers this amazing change that we've seen in AI affecting experimentation across all features. Now, can you break down for us the second side of this topic? How do we measure and experiment AI features themselves?

**Frederic de Todaro** (00:41:43)

Yeah, I think there are some key indicators that you have to look at. The first one is, you know, the usage or the adoption of people, you know, using your feature. The second one is the outcome, you know, is that feature, you know, fixing the problem, you know, users came for, or is it helping them, you know, complete more tasks faster, you know, activate more experiments and so on. And the last one is the experience. Once the feature is live, well, you want to ask users, you know, the feedback about it. And usually we see, you know, in AI features, you know, the quick thumbs up down that you see everywhere. Because this is one of the only way to get, you know, feedbacks about, you know, is the answer provided by the AI accurate? Or is it missing some context there? So very, very important to include them as well.

**Frederic de Todaro** (00:42:45)

And if we look at what we are following with prompt-based experimentation, it is not just about usage. It's about how quickly our users can go from an idea to a learning. Because in the end, this is ultimately the main goal of experimentation. So we look at things like how many prompts it takes to create an experiment. But if it's too many, something is off. Maybe the AI is not providing the piece of code or the variation that the user wants there. The second thing is, you know, how long it takes from the first prompt to an experiment live. Very important as well. If it is faster than any other methods, that's a big win for us, right? Instead of taking days, maybe you took five minutes to put in a production your experiment. And the last one, which is also very important for us, is how often developers still need to step in.

**Frederic de Todaro** (00:43:54)

If you look at the past, before prompt-based experimentation, I would say that maybe 80% or more of the experiments needed could. That's the true and the reality of our market. If we drop that number to, let's say, 20%, which is our target at Chameleon, well, we know it is, you know, a massive game changer for the industry because we haven't seen that, you know, anywhere else in the last decade. So those are the metrics we do follow. And so again, it's not only about usage, it's about the value that we want to generate to our users. The feature needs to allow them to run experience faster, to get to learning faster, and so on.

**Aakash Gupta** (00:44:44)

I love this. It's almost structured as like the whys, the five whys, right? Are people using it? Is it solving the problem? Was it helpful or reliable? And then translate that to your experiment like you've done with prompt-based experimentation. I'm curious, what was the North Star metric you guys looked at and how did you determine the North Star metric for success?

**Frederic de Todaro** (00:45:05)

Yeah, it's a good question. So at Cameroon, we look at the number of experiments, you know, which run daily on our platform. So we have been following that for, you

**Aakash Gupta** (00:45:15)

know,

**Frederic de Todaro** (00:45:16)

many years. We came up with that North Star metric because it is, you know, simple to follow, to measure. We don't have to ask data scientists to get access to that metric. And the second reason is that it is very easy to anyone in the organization, right? It's not something very complex, very specific to a product team and so on. The number of experiments that run daily. That's the metric we look at. Because we know that, you know, when there is a drop on that metric, it means that there is some churn at Cameroon. It means that we have less customers, you know, creating campaigns every day. And if it goes up, it means that either, you know, we are increasing the business with new customers or we have, you know, more and more users creating experiments. And so this is critical for pump-based experiments because, again, our goal is to have more users, creating experiments so that it is not only limited to a team of users, it is not only limited to product teams or to engineering teams.

**Frederic de Todaro** (00:46:26)

We really want to democratize experiments as part of the organization. And so the more experiments are created, well, the better it is. It means that, you know, prompt-based experimentation is delivering on the promise, which is again, to be able to have an idea to an experiment in minutes and not days or weeks as it is in most organizations today.

**Aakash Gupta** (00:46:50)

So I think there's a lot of hidden takeaways there for people listening. The first is the North Star metric you chose is basically your business's overall North Star metric. You're not just choosing some random North Star metric specifically for this AI feature experiment. If it's a big AI swing, you want to just move the whole business. The second thing is is that you didn't choose a revenue-oriented feature. You actually chose a product input metric that you guys can change, but that you know is highly correlated with impacts on your output metrics like revenue. Are those fair takeaways? Exactly. Exactly.

**Frederic de Todaro** (00:47:26)

Because with that North Star metric, everyone can play the same rules of the game. If you look at product teams, You know, they can improve features that drive it forward. That's why we, you know, introduced point-based experimentation. It's a product initiative as well. And I know that my product, you know, managers can deliver on that and increase that north star metric. Customer success as well. Customer success can, you know, help users get more value out of the product. And their goal is to increase the noftar metric. Because if they have happy customers, if they know how to use the product, you know, well, they will ultimately create more experiments. Marketing can also work, you know, in, you know, publishing some benchmark per industry, per market, so that, you know, our customers can compare with each other. So every, I would say, department, divisions in the organization work towards, you know, improving that North Star metric.

**Frederic de Todaro** (00:48:28)

It's not just revenue because we're revenue. Well, you can't hold up on that metric. It's very hard in the end. But if we, you know, find an off-tar metric which is highly correlated to revenue and that can be, again, actionable by any team, that's something that can change the face of an organization there because everybody is moving to the same direction in

**Aakash Gupta** (00:48:56)

the end. So that's how you measure kind of a game-changer feature like PBX. It's really changing the way people use your platform. Talk to us a little bit about how you measure RAG systems.

**Frederic de Todaro** (00:49:07)

Yeah, so RAG systems, so again, this is what is usually powered behind this, you know, assistant there. Same story, I think it's very important to look at some business-oriented metrics there, you know, adoption, the usage, you know, the outcome, the experience. And then I think there are also some technical metrics to look at. And at Camelot, we have been looking at them before, you know, shipping that feature into production. And, I mean, there are three things we look at at Cameloon, and I think it can be applied to any organization using a RAG system there. The accuracy, you know, is the answer really based on some documentation that, you know, do exist? You know, for instance, if someone asks, how is traffic, you know, split in a ULTI on Bandit? And if the AI answers, while traffic is always split evenly across all variants, well, that's a miss, right?

**Frederic de Todaro** (00:50:21)

So that's a bad answer in terms of accuracy. Relevance is very important as well. So relevance is all about, you know, does it actually answer the user's question? For instance, if I ask something like, you know, what are ways to target feature flags or what are the different options there? And the AI will answer saying you need to create a new experiment. Well, you know, it's a miss as well. It is not answering the targeting logic or the targeting part of the experiment creation. And the last one is the context quality. You know, where are the documents or documentation it used really helpful. You know, if it pulls some outdated documentation or some, you know, or not the most recent, I would say, release notes, well, something is half as well. So these are good signals to me to check if the AI is giving answers you can trust.

**Frederic de Todaro** (00:51:30)

Now, I just wanted to end on something. There are also, you know, if you look at what we've been doing at Chameleon, if I can say something as well there, one method which works well, because I'm sure people will ask, okay, but how do I do that? How do I make sure that, you know, accuracy, relevance, and so on, you know, is good? One method we've seen working at Cameloon is to use, you know, a LLM, so a learning language model, as a judge, right? So you have a judge which will judge the performance of your RAG system. So for instance, here for the response relevance, which is again how well does the chatbot answer, you know, match the user's question. One method is to use an LLM which will generate two, three new questions based on the answer which is provided by the first LLM.

**Frederic de Todaro** (00:52:29)

So for instance, if I say, how do I enable AI targeting in Chameleon? And the chatbot answers me, you need to go to the experiment settings, enable the AI targeting toggle and save. That's a good answer, right? And so the LLM, the alternative LLM, as a judge, you ask him to generate two, three questions based on that answer. Like, where do I find the AI targeting setting? Or how do I activate AI targeting? And so these questions are very similar to the question being asked by the user. So it means that, you know, the relevance is there. And so you can do that, you know, for the matrix and the retrieved context as well. Context relevance, you know, the scoring, the LLN can score the answer as well. You can do that with the accuracy. That's what works well today, I think.

**Aakash Gupta** (00:53:28)

So it's that combination of looking at faithfulness, relevance, context quality, operationalizing those into metrics for you, and then building a good eval suite, potentially using an LLM as judge to look at things like response and relevance, context relevance, faithfulness. That's the overall recipe for measuring an AI feature. Are there any big mistakes you see teams making while measuring these AI features?

**Frederic de Todaro** (00:53:55)

Yeah, I guess one of the biggest mistake is, you know, to stop at usage again, because, you know, most of what we see is when, you know, some users, you know, will complain about, you know, any feature, we'll just stop using it, right? So, I mean, usage is one piece of the cake here that you need to look at the outcome and the user experience. And so some of the insights I've been sharing there are pretty useful for you as well.

**Aakash Gupta** (00:54:29)

Amazing. Before you go, I have an experimentation expert here with us. So I have a couple of questions for you. First, what company do you think is doing experimentation best?

**Frederic de Todaro** (00:54:43)

Yeah, so I'm not going to choose the usual one like Netflix, Airbnb, Microsoft, and so on. I'm thinking about, you know, a company called Booking.com, very known as well. And, you know, they've built such a strong, I would say, culture of experimentation. Nothing goes live into production, whether you are shipping features on your website, on your mobile application. They do everything through experimentation. So I think it's a great model for any company that wants to learn fast and build with confidence.

**Aakash Gupta** (00:55:21)

And I think they test almost everything, right? So they've really built that experimentation culture from the top.

**Frederic de Todaro** (00:55:29)

Yes, exactly, exactly.

**Aakash Gupta** (00:55:31)

And I think that's incredibly rare, but it's incredibly common amongst winning companies.

**Frederic de Todaro** (00:55:37)

Yeah, yeah. And my advice, I think, just to not, you know, scare every people there, I think it's not, don't have, you know, you don't have to go, you know, all in one and test everything from day one. At Cameloon, we have been going step by step on this topic, even at Cameloon. So we are also chipping features, experimenting with them and so on. And I think you have to start simple at the beginning. If you are not doing any experimentation today, well, first use feature flags just to push code safely into production. At least you have a turn on off. You can see how it goes into production. Then you introduce what we call progressive rollouts or targeted delivery where you ship the feature to, let's say, 20% of your users or to a segment of users. And then you learn from that. So you learn from the usage.

**Frederic de Todaro** (00:56:37)

Are they using that feature? Are they complaining about the user experience? And then you improve that feature before releasing it to every single user. And once you're ready, then you start adding some A-B testing there to make data-driven decisions at scale. And I do believe that people have been putting barriers because of the high build cost. So that's why I think with AI, that thing is going to be removed. so that you can hopefully, you know, going to push more things behind experiments as well because you are able to ship them, you know, without having to bother your developer teams.

**Aakash Gupta** (00:57:24)

Yeah, AI is a game changer to becoming a company like Booking. You have no excuse at this point. What are the biggest mistakes PMs make when it comes to experimentation?

**Frederic de Todaro** (00:57:37)

Yeah, I wouldn't say there are mistakes, but there are some common misconceptions there about experimentation. And, you know, I put three of them here, but there are others, of course. And I think, you know, the top three I hear the most about is it will slow down our delivery. The second one is we don't have enough traffic there. Or, you know, because you do product discovery, well, I'm fine. You know, I've learned a lot from product discovery. So why should I bother with experimentation? And so none of these objections for me are perfectly true. I mean, experimentation actually helps team build, you know, better products. There are many studies about it. There is one which I like to talk about, which is one being done by Harvard Business Review. which basically says this, there is a direct correlation between the number of experiments you run annually and your revenue growth.

**Frederic de Todaro** (00:58:39)

That's a fact, right? So the more you experiment, the faster you can go there. So if we look at all of these objections there are, I think the first one actually it speeds things up. It's not slowing, you know, it's not slowing things down there. With experimentation, you can release, as I said, early versions of your feature. You can learn from, you know, real users, you know, using that feature and then you improve as you go, right? That way you get to the right feature faster in the end. So you don't have to work on the best feature before shipping it. You ship the first version of it, you iterate with it, you learn, and then you ship the final version to all your users. Like I always say to my own team, you know, fast gets, you know, good quicker than good gets fast. So the key message here is that you do not wait for the perfect feature.

**Frederic de Todaro** (00:59:37)

You ship early and you iterate until you reach your goal. You will learn so much more in a short period of time than if you don't do experimentation there. The second one, very quickly here, it's always a little bit funny to me because teams often find validating features with just a few users. They have a prototype, they go and show that prototype to 10 users and then they think that all their users will love the feature. So why it is a problem with experimentation there? So it doesn't make any sense to me. And the traffic is one point. The number of conversions is also very important. When you look at, you know, the sample size you need, you need a good number of visitors, but you also need to look at the metric. The more conversions you have, you know, the fastest you will get some insights about your experiments.

**Frederic de Todaro** (01:00:31)

And the last one, product discovery is enough. I would rather say that discovery and experimentation go hand in hand. You know, discovery gives you early signals. That's a fact. That's why it's very, very important to do some product discovery. But experimentation will tell you exactly what users do when they interact with that feature. So product discovery will tell you what users say they want. Experimentation tell you what they actually do. So very important for me to have both so that you get the full picture in production.

**Aakash Gupta** (01:01:14)

Amazing. This episode, our complete course on AI experimentation is coming out an episode after our complete course on AI discovery with Teresa Torres. I think it's the perfect combo of content, perfect ending for episode today. Fred, this has truly been a masterclass. If people want to find more, if they want to connect with you, where should they go?

**Frederic de Todaro** (01:01:35)

Well, directly on LinkedIn. Directly on LinkedIn, I would answer most of the questions I got.

**Aakash Gupta** (01:01:41)

Amazing. Thank you so much for your time today. It has been a pleasure. Thanks for having me. So if you want to learn more about how to shift to this way of working, check out our full conversation on Apple or Spotify podcasts. And if you want the actual documents that we showed, the tools and frameworks and public links, be sure to check out my newsletter post with all of the details. Finally, thank you so much for watching. It would really mean a lot if you could make sure you are subscribed on YouTube, following on Apple or Spotify podcasts, and leave us a review on those platforms. That really helps grow the podcast and support our work so that we can do bigger and better productions. I'll see you in the next one.
