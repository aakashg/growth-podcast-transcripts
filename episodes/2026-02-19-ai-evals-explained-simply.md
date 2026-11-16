---
title: "AI Evals Explained Simply by Ankit Shukla"
subtitle: "You've never heard such an intuitive walkthrough of evals."
date: "2026-02-19"
host: "Aakash Gupta"
guests: ["Ankit Shukla"]
speaker_names: "inferred"
substack_url: "https://www.news.aakashg.com/p/ai-evals-explained-simply"
youtube_url: "https://www.youtube.com/watch?v=Raa3qjEBvKE"
duration: "01:04:09"
word_count: 14132
source: "Substack episode transcript (aired audio)"
---

# AI Evals Explained Simply by Ankit Shukla

*You've never heard such an intuitive walkthrough of evals.*

**Ankit Shukla** (00:00:00)

Your AI feature fails not because of the model, but because you didn't evaluate it. If you are shipping AI features without evaluations, your product is lying to you and you have no idea.

**Aakash Gupta** (00:00:08)

Ankit Chukla has taught thousands of PMs, AI evals, and today he's open sourcing the knowledge that he normally charges thousands of dollars for for So

**Ankit Shukla** (00:00:17)

I'm going to call today's class the masterclass on creating effective evaluations.

**Aakash Gupta** (00:00:22)

How do we actually build this? So first is the success criteria and the expected behavior. The way the best AI companies work is that the AI PM defines these evals. And that is basically the PRD for the AI engineers.

**Ankit Shukla** (00:00:35)

If you are not doing offline emails correctly, then you have not even created a product that can be actually launched to the real audience.

**Aakash Gupta** (00:00:41)

How can I become an AI PM in 2026?

**Ankit Shukla** (00:00:44)

Follow these steps. Number one is make sure that your product sense skills are exceptional. The second part is make yourself aware about certain technical concepts and some Gen AI concepts. Most of the PMs have no idea about how to write evaluations. They have no idea about how to go ahead and build a production level app. In these 60 minutes, I'm going to assure you that you are not only going to understand the fundamentals of evals, but I'll give you a real case study where we are going to help you understand how to plan your evals like a pro AI PM. Let's get

<!-- sponsor -->
**Aakash Gupta** (00:01:12)

right into it. Before we go any further, do me a favor and check that you are subscribed on YouTube and following on Apple and Spotify podcasts. And if you want to get access to amazing AI tools, check out my bundle, where if you become an anal subscriber to my newsletter, you get a full year free of the paid plans of Mobbin, Arise, RelayApp, Dovetail, Linear, Magic Patterns, Deep Sky, Reforge Build, Descript, and Speechify. So be sure to check that out at bundle.akashg.com. And now into today's episode. Quick note for my audio listeners, there are some things that we showed, which you can see on Spotify or YouTube, but we've edited this audio so that it's a really good listening experience nonetheless. Ankit, welcome to the podcast.

**Ankit Shukla** (00:02:00)

Thanks a lot for having me again, Akash. And till this day, I think we have done that podcast about three months ago. And till this day, I almost get like a couple of messages every day on my LinkedIn appreciating the content of that podcast. So thanks a lot for creating

**Aakash Gupta** (00:02:12)

that content with me. So evergreen. Like some months, it's my top podcast episode, even though I've released other new podcasts. So it continues to grow. True testament to the value we put there. What are we going to do in today's episode that's different from all the other AI evals content out there that people might have seen?

**Ankit Shukla** (00:02:31)

Yeah, so understand most of AI product management is actually product management only. But there is this one skill that is new and most of the PMs are not aware about. And that skill is eventually to go ahead and write good kind of evaluations for your system. Now, what is happening in the market is that I could see a lot of content is being posted around evals. But most of the content is still like introductory level or intermediate level content. And we lack, let's say, real examples. And most of the examples are hypothetical. So I thought that why don't we create this episode so that anyone who has an aspiration to become or pursue like the AI product management career seriously, they should be able to understand with crystal clarity that this is how I should approach evals. Understand evals is not, let's say, So one thing is going to fit everyone.

**Ankit Shukla** (00:03:15)

But I'm going to tell you the nuances that you need to take care of. And you'll be walking away today with a framework so that you can write strong evals for almost any kind of product if you follow these kind of practices. So that is my promise for today.

**Aakash Gupta** (00:03:26)

Well, let's get straight into it. And maybe we can start with fundamentally justifying why is it important for PMs to learn AI evals? Yeah.

**Ankit Shukla** (00:03:33)

Yeah, so I'm going to call today's class the masterclass on creating effective evaluations and understand that I'm going to follow this approach that initially, so I want to give the agenda beforehand so that you are able to take time and make sure that whenever you're watching this episode, you are sitting out with a notebook so that you can go ahead and revise and recollect things. So I'll divide this whole section into three parts. The first part is we look at an AI product because if you don't understand what are the nuances of an AI product, you'll not understand what evaluations are. Then I'll give you a quick five-minute introduction of what evaluations are so that you understand what we are talking about. After that, we'll give you like a quick introduction to evals. I'm going to talk about the nature of large language models, what are the metrics for evaluations, and then I'll give you an end-to-end flow of how to create evaluations for almost any kind of product, whether you are talking about agents, you're talking about simple chat box or you're talking about some enterprise great products and eventually i'm going to go ahead and give you some tips for writing effective evaluations and then i'm going to give you an end-to-end case study of how a company might do evaluations so that is the agenda that we are going to follow today now before i could go ahead and talk about evals let's talk about the fundamental building blocks of jnai product and why it is different so so far Most of us have been creating products which were very deterministic in nature.

**Ankit Shukla** (00:04:49)

But if I go ahead and talk about the nature of a Gen AI product, these are some of the critical components. Let's say one of the component is the language model. I'm not calling it a language model because there are also some useful small language models. So we'll only use language models. Then we have the context engineering part, which is data that you gave from reg or something or the prompt that you put. Then we have tools. Then we have orchestration, how things are going to connect with each other. And then we also take care of the user experience, how the user is going to interact. How do you include humans in the loop? How do you take care of latency and all, right? So these are, I would say, five critical components. But now the issue here is that this particular part, the language models, it is not deterministic.

**Ankit Shukla** (00:05:27)

For similar kind of inputs, it can give you different kind of outputs. So it is almost like a lion in a circus where you have to make sure that although you know about the nature of the lion, which is it's a beast, but as a ringmaster of the circus, you need to make sure that you are able to tame that behavior and show like a good circus or a good product. So that is why we need evaluations. And there are other things also that are going to matter for the evaluations, which we are going to go ahead and talk about. So this is a reason why we need evaluation, because there is a indeterministic nature or stochastic nature for the large language models. Now, before I could go deep into the evals part to make everyone understand what evaluations are, I'll take a very simple case study.

**Ankit Shukla** (00:06:04)

It will only take, let's say, four or five minutes. So, let's say we are creating an AI-first job website. And the use case is very simple. Let's say I want to apply for a job. Every one of us who is applying for a job, we need some information. The information is, the product is, that I will crawl the major job portals of the world automatically. Maybe the LinkedIn, the hired or the angel.co of the world. After that, I'm going to put that job description through a large language model. It could be any of these large language model or something better. And then I am going to enhance that job description, make it more, I would say much better for the candidates because I'm going to enhance it into summary of the job description, possible interview questions from the job description for the job. What are the skills that you need?

**Ankit Shukla** (00:06:44)

What is the learning guide if you are really seriously preparing for it? And if you think you are prepared, we are also going to give you a quiz for assessment. So this we are creating from the small piece of information that we have got from the job description. And I'm sure that many of the people who are looking for jobs would definitely find this interesting. So this is like a simple product. You can also call it a wrapper on the top of an LLM, right? Now, even if I do this, I will understand that I cannot trust large language models to do this job really, really well. So what I'll do is in order to understand that whether I'm giving the right output to the users and all this information is done correctly, what I'll do is I will try to evaluate. And by evaluation, I mean what I'll do is I will use some or the other method to make sure that whatever the content is being generated, it is factual, accurate, correct, helpful, and maybe some other kind of parameters are being satisfied.

**Ankit Shukla** (00:07:33)

For example, I want to make sure that the summary of the job description should be less than 300 words. Otherwise, it's not a summary. I want to make sure that the skills that are needed are actually real product management skills. And I also want to make sure that the learning guide that I'm creating is actually an actionable guide and the model is not hallucinating. So what I'll do is I'll generate all of this. Then I'll write an evaluation and then I will understand whether my prompt, my model are working correctly or not. Because it might happen that initially I've given a prompt, but it is not able to work correctly. Or maybe I need to choose between whether I should use GPT-5 or I should be okay with maybe GPT-3 or GPT-4, which is a cheaper API, right? So that is the purpose of evals. If I need to exactly show you what this evaluation prompt is going to look like, let me show you.

**Ankit Shukla** (00:08:16)

So this is what the evaluation prompt is going to look like. It's a very simple use case. So I'm going to call another LLM where I'm going to tell it that you are an AI quality evaluator for product management job listings. And whatever input output that I've got from this particular model, like the prompt, my initial prompt, I'm going to give it over there that this is the job description. This is the AI generated summary. This is the interview questions. This is the skills. These are the concepts. These are the quiz. Now you go ahead and run all of these things, which is, is the summary accurate? Are the interview questions relevant? Are the listed skills aligned? And all of these things. So what we'll do is that we will... whatever output that you've got from the model initially, from the base prompt, we are base system prompt, we are going to take it and we are going to run this particular prompt or evaluation through that, right?

**Ankit Shukla** (00:09:03)

And then I'll understand that whether the summary was good or not, questions were good quality or not, or skills were liked or not. And then based on that, I'll be able to understand whether my prompts, my language models are working correctly or not. In case I was able to understand that accuracy is not good, so I'm going to tweak the prompt to make it more tight, tightened. If I think that maybe I'm able to get the same kind of output with a cheaper model, which is GPT-5 or something, GPT-4 or something, I'm going to use that and not use the most costless model. So this is what evaluation is. I am going to get output from, let's say, some of the LLMs or something. And then I want to make sure that I am able to evaluate that output on certain kind of metrics. So one of the things that I am going to monitor is the length.

**Ankit Shukla** (00:09:44)

Length can be done by a simple evaluation of counting the characters that can done with the help of code. While other things which are the accuracy, whether these are the good questions or not, can be evaluated by maybe a human or LLM or other large language model as a judge, which is generally more intelligent and The other models that you use in your product.

**Aakash Gupta** (00:10:02)

So that would like a one rise here. Right. The eval, it doesn't always have to be an LLM judge. We've shown a prompt, but for the 300 words, we can use a simple code. So an eval, it can be anything, right? If we were explaining this really simply, it could be any sort of test. It could be a unit test in the old language. It could just be a counting of words here. Or in the most advanced form, as we've shown, it can be an LLM judge, which is kind of replicating some of that human intuition that we encoded into that prompt we saw. Yes.

**Ankit Shukla** (00:10:34)

Now, we are going to address two challenges today, which are coming in the AI world, AI product world right now. The one major challenge is that prototypes fail to scale. And this has been verified in a lot of research. One of the very popular research that has been quoted everywhere is by this Darnanda committee from the MIT that 95% of the all AI initiative fail. And the major reason for them is the learning gap. So when I got into the paper, I was able to understand that what do they mean by learning? And learning basically means that either they do not like the people who are building AI initiatives, either they are not solving the right kind of problems for the companies, which is they are not aware about the workflows and they are just trying to implement some of the other kind of gen AI solutions.

**Ankit Shukla** (00:11:14)

And the second part, the second part of the learning app is that these systems do not evolve, which is if I'm giving feedback to the AI that please go ahead and don't do this next time, still they are going ahead and repeating the mistakes.

<!-- sponsor -->
**Aakash Gupta** (00:11:25)

AI evals are not the only important new skill for product managers. The second most important skill is AI prototyping. And the problem with most of the AI prototyping tools out there on the market is that they're trying to be low-code, no-code tool alternatives. They're trying to allow you to create an entire startup. Today's episode is brought to you by Reforge Build, which takes a completely different approach to AI prototyping. They are putting the product manager at the center and they have architected the product in that way. So whether it's quickly picking up the design system or generating divergent alternatives, And

**Ankit Shukla** (00:12:16)

To talk about the first part, why prototypes fails, we have been able to do research and we are able to find that there are generally five reasons why prototypes fail to scale. And this is very important because this is the reason between you playing with prototypes and you going ahead and becoming like a real AI PM and building, let's say, some impactful products. So the reason is one very common reason is the data drift. Data drift means that you have trained the model in different conditions. You have created the product in different conditions, but now the customers have evolved, the data have evolved, the context has evolved, the knowledge has evolved, and your product is not able to keep up. The second part is cost considerations. Now, AI is not like some, like Gen AI is not like other product where the costs are fixed. So, in SaaS, most of the time, the operating cost or I would say the marginal cost for every other user is almost very, very small.

**Ankit Shukla** (00:13:00)

But in AI, with each and every call, you are going ahead and paying money. So, sometimes what happens is that costs do not scale well. After that, We have engineering limitations, which is we have not done step testing, issues of scalability, asynchronous behavior we are not taking care of. And then this is an important part, which is in prototype, because you are going ahead and doing it with less data, you do not think of the guardrails, which is how you are going to create a feedback loop, how you are going to create the fallback logic, what are the legal and legal lengths that you are going to play there. And then the last part, which is not the discussion for today, but still it's the major problem, which is collaboration failure. Now, this part of AIPM is also same as a product manager shop, which is you need to make sure that you are a good collaborator.

**Ankit Shukla** (00:13:35)

You need to be good collaborator, not between only your teams, but also between users and your own team. So that makes sure that yes, if you go ahead and do these kinds of things, there is high probability that your prototype will not fail to scale. Right. So yeah, you want to speak something?

**Aakash Gupta** (00:13:49)

So do evals help address all five of these or where do evals really help you?

**Ankit Shukla** (00:13:53)

Yeah. So evals can help you in data drift. So when you are putting evals, you are continuously able to monitor that, yes, this is what is happening with my product. And if something is not going in the right direction, you'll be able to take action on it as soon as possible. So evaluations are going to act on the top of your observability. like your matrix then for cost considerations also so what happens is because in prototypes we are using the best kind of models because we want to show the prototypes in the best light what happens is we are not thinking about the cost but when it goes to production when you and you think that you have to use the right kind of model then if you're only using the best model which is maybe five or something then the issue is that the okay we'll cut from here we'll start from cost considerations okay so yeah So, cost consideration is a very important part because most of the PMs, what they do is they think that if in the prototype I have used maybe the most advanced model, I should use the same model in the production as well.

**Ankit Shukla** (00:14:47)

And then because of cost considerations, the management has to go ahead and pull the plug up. But now there is a good possibility, which is that maybe another model, which is a cheaper model can go ahead and produce a similar kind of output. So if you go ahead and look at, so I'll just show you the pricing of different kind of models. Okay. So I'll just search for open AI pricing API, and then we can see the pricing. Right, so you can see that the best model, GPT 5.1, which is mostly going to be used in your prototype because it's very intelligent, the output is $10 per million token. But for maybe a model such as GPT Nano, the output is maybe 0.4, right, which is only 40 cents. Now, you do not need to use only this. You can also use this and you will only get the confidence of using this when you have created the right kind of evaluations.

**Ankit Shukla** (00:15:33)

Right. So that is why evaluations are important over here. They can let you understand whether a cheaper model can also go ahead and perform at a similar kind of level or not. And it has, we have seen that multiple places that people just need to, let's say, do the intent matching or intent separation. And still they are using for the simple tasks, they are also using GPT-5.1 because they are not sure. And they are not sure why, because they have not created the right kind of evaluations.

**Aakash Gupta** (00:15:56)

And there we saw a 25x price difference. That's really not crazy because there's also open source models out there that price similar to that 40 cent per 10 million token. So you might say, oh, GPT Nano, it's so much worse than GPT 5.1. But actually, there are some competitors to GPT 5.1, whether that's DeepSeek's latest model or Kimi K2 that are pretty good and also pretty cheap.

**Ankit Shukla** (00:16:21)

Yeah. And also there is a concept called a transfer learning where you take a small language model like a Gemma from Google. And then because you are, let's say, your case is very specific, such as a customer support for a particular kind of company with limited kind of product, you don't need to use GPT 5.1. You can use a small language model, use transfer learning in order to create, let's say, you can create synthetic data, do transfer learning, do fine tuning, and then you'll have a similar kind of model which is able to go ahead and maybe dedicate it to all the use cases that you have.

**Aakash Gupta** (00:16:47)

So as long as you have a really specialized use case, you can take these smaller models, you can do transfer learning, and you can make the cost much cheaper. Yes. But how do you know that you're doing it at the same quality? Evals. Evals. Yes. Correct.

**Ankit Shukla** (00:16:59)

And then for engineering limitations, I think this is going to be wider in scope. Yes, some of this can be solved with evals, but not all of it. And then guardrails. This is a major part. where evals actually shine which is you are going to define what should the model do what should the product do what should it not do where like when should it could when should it ask for help and what are the different kind of output that it should produce and this is where evals are actually going to go ahead and shine which we are going to see in just a moment and then this collaboration failure now although this is not directly related to evals but when you are writing good evals you are always going to involve the subject matter experts And that will give you a different kind of empathy with the user.

**Ankit Shukla** (00:17:40)

So I think this also is indirectly contributed because you have not cared enough to go ahead and create the right kind of evals.

**Aakash Gupta** (00:17:48)

100%. Makes sense. Yes. Actually, one more question since we saw that MIT slide. Is that BS? It seems like overstated. 95% of AI initiatives fail. It feels like... Maybe that's true in like a bank or somebody where they're like really tech backwards. But in tech startups, it feels like it's probably the opposite. Like 95% of AI initiatives succeed. Cool. So understand,

**Ankit Shukla** (00:18:12)

data is data, right? You can create a story with the selective data that you have. So... Now, what has happened in this study is if you look all the, let's say, 30, 35 pages of that particular research paper, you'll be able to understand that first, we are right now in the very early stages of AI, which is considered 89, 91, 1991, 1981, when the internet has came. So, it's very, it's too quick for us to go ahead and maybe assess the, let's say, the profitability or the, I would say, the scalability of AI. That's the first, or usefulness of the AI. The second part is the companies that were considered were on account of double or triple digits only. Okay, so they have not considered a lot of companies which are going ahead and maybe trying a lot of things in the AI world. However, I generally am very much aligned with the findings of because it is very logical.

**Ankit Shukla** (00:19:02)

So, if we go back to like the traditional product management, product management, basically fail because they are not catering to any user needs and they are not even evolving with the user needs and that is what they are saying in the end and if you now look at this then even in the real world like almost 90 products fail you would have created so many products so many prototypes but most of them have failed like at least they were not commercial success so i think Yes, the output of the study could be good. But yes, there was some kind of selective data. But then in the future, I believe that if more people are taking their initiatives, then the failure rate could be mostly around the same because it's not easy to create like a very scalable and a very profitable product. Okay. Yeah. So now we are talking about evals because of one major reason, which is the large language models are non-deterministic, right?

**Ankit Shukla** (00:19:49)

And this is a major reason why we have to go ahead and do all of these things. Otherwise, this could be, let's say, handed over to maybe a testing team or a QA team, right? Yeah. I'll give you an example. So although I've given you the drop site example, now I'll go deeper. I'll give you like a more common sensical example, which is maybe example of a chai or a tea, right? Yeah. So, if someone asks you how would you create a tea, then maybe your answer would be different than someone else and then every person in the world would love a different kind of taste of the tea. But then the definition of tea is the same, that you go ahead and have some water, you have some tea leaves and then some BVD would have the sugar, somebody would have the milk and then they are going to create the tea.

**Ankit Shukla** (00:20:24)

So, now, when I go to different places, okay, for example, when I go to maybe a hill such as Manali or something, the quality of tea is going to be different, the taste is going to be different. When I go ahead and take a tea at home, it is going to be different. And then, when I'm going to maybe go on a trip on railway, you'll understand that the tea is different and this is mostly the worst kind of tea that anyone has gone ahead and... So what is happening here is that although the output is the same, output is the tea, but based on the customer needs, based on the context, based on who is preparing the tea, the feeling that you get while drinking that tea is different, right? So your product is also the same. So if I give you, let's say for large language model, if I give you the prompt that how do I make a cup of tea?

**Ankit Shukla** (00:21:07)

because they are non-deterministic they are going to give me the right answer they will tell me how to go ahead and maybe make t and understand hallucination rate is not as much as it was maybe a couple of years ago right now hallucination has reduced a lot most of the answer are generally factful but still this t is different than this t and this t is different than this t right this is the moral of the equation that the large language model, yes, it can be correct. We are not going ahead and questioning correctness at this point of time. They hallucinate, but the hallucination rate has reduced. However, apart from hallucination, even if the models go ahead and became perfect in terms of not hallucinating in the future, which they are going to be, still they cannot go ahead and understand what your customers want because every customer is different.

**Ankit Shukla** (00:21:48)

Their needs are different. So you as a product manager need to make sure that you are able to ensure a similar kind of experience or the right kind of experience to all the customers so that if people want to take a tea, they are going to come to your shop rather than going to some other product out there. Yes. Do you like tea, Akash?

**Aakash Gupta** (00:22:05)

Yes, of course. I drink chai every day. Okay. Yes. All right. So I think we have the intuition down. Now, how do we actually build this?

**Ankit Shukla** (00:22:14)

Yeah. So now I'm going to give you like a detailed flow and I've made it like very dramatically, like, sorry, I've made it in the form of a diagram so that everyone is able to understand very visually. So I'll just go ahead and share the Figma. Yes. So this is Sigma right now. It might look overwhelming, but I'll tell you how it works. Okay. Okay. So very first thing is, whenever you go ahead and start any kind of product, you are going to define the success criteria and expected behavior. Okay, let me give you a very small example. Okay, so although we are going to talk about this example in detail later, but I'll show you a gist. So let's say most of you might have used Robinhood Cortex, which is a new feature that they have launched. And a similar feature, like a company in India, IND Money, which I used to work, let's say, three, four years ago, they have also, let's say, built that kind of feature.

**Ankit Shukla** (00:23:01)

I'm not anyway affiliated to the company and all of this is actually reverse engineering. So the product is very simple. IND Money or Robinhood are stock trading apps where you can buy and sell your stocks. Now, what they have done is they have understood that many people before buying a stock, they want to do some research. And for that research, they are generally going to go to Google. They are going to type something. They are going to go to chat GPT or they are going to ask a financial advisor. These people thought, why don't we go ahead with AI? We should be able to help people understand more about this particular stock. So they have created a feature called as I in the money mind. And what it does is whenever you click on this below any stock, it is going to give you some auto populated questions.

**Ankit Shukla** (00:23:41)

And then you can also write your own question. These are commonly asked questions. And then when you click on that, it is going to give you an answer which is powered by AI, which is it is going to fetch the right kind of documents and it is going to give you a very contextual answer. This is the use case, right? Now in this use case, if I walk you through the whole flow now, so now remember this use case, I'll walk you through the whole flow. So first is the success criteria and the expected behavior. Now understand, I want to make sure that there are some guardrails that I need to follow, which is whatever the input, the output that I'm getting out of this chatbot, let's say that should be limited to maybe 150 words or maybe 300 characters to make sure that it is summarizable and people are able to go ahead and see it.

**Ankit Shukla** (00:24:20)

The second behavior is that I should make sure that the model should never recommend selling or buying a stock. Why? Because illegally you are not allowed to go ahead and give any kind of recommendations. So there is a regulation in India which says that no, if you are not a registered model, if you are not a registered investment advisor, then you cannot go ahead and do, AI cannot do this, right? So let's say these are the behaviors that the thing should be factual. They should be grounded from the data. And then you should not go ahead and suggest someone to go ahead and buy or sell a stock. You should not make a direct recommendation. You should just give the information. So this is the expected behavior that we have. Success criteria should be that in the end, when people are going ahead and maybe they are getting this information, in the end, they should give a thumbs up or something so that we understand if the output was actually good or not.

**Ankit Shukla** (00:25:05)

So that is expected behavior that we have. Now what we'll do is we will go ahead and transform that expected behavior and success criteria into some kind of metrics. Right. So the metrics could be, let's say, what is the quality of information? Maybe some kind of UX metrics such as latency and all. Then the output has to be safe. It has to be performance oriented, which is again latency. And then we are going to talk about behavior, which is it should not go ahead and suggest you that you should go ahead and buy or sell that stock. Right. Now you can understand that if I go ahead and talk about UX, maybe if I want to make sure that it is up to maybe 150 character or 300 character, I can choose to do a code based evaluation. So now in order to make sure that these evaluations are being done correctly, I can choose multiple options.

**Ankit Shukla** (00:25:48)

One option is I can do it through code. I can have a human to review it. I can do it through LLM or I can go ahead and choose a combination of these three. Right. So this is what I'm doing at this side. But on the other side, as soon as I understand the success criteria and the expect behavior, the first step that I need to take is I'll create a base product. So I have an expectation that yes, I'm going to create the version one of the product. It should not do these things. So that is the base knowledge that I have. From that base knowledge, I'm going to create a system prompt. System prompt is very simple. Given this talk and this question, answer this question. Make sure that you are not suggesting, make sure that you are always getting the output from, input from this kind of data and maybe some other system prompt, right?

**Ankit Shukla** (00:26:25)

And then I'm going to choose certain kind of system prompt. I'm going to choose some kind of models. I'm going to choose some kind of tools. Here I'm going to use a tool called as web search. Right. And then I'm going to give it certain kind of context, which is a user information or its background. And then I'm going to use certain kind of orchestration. Understand all of these are variables. A major mistake that product managers make is they think that now these things are fixed and they tend to love their solutions. Understand all of these things are variables. These are knobs on a dashboard that you need to click here and there in order to make a better product. Right. So you are going to start from something basic that is coming out of the information initially that you have. So you are going to put an input and then you are going to get an output.

**Ankit Shukla** (00:27:04)

This is the base product. For

**Aakash Gupta** (00:27:05)

example, orchestration layer.

**Ankit Shukla** (00:27:08)

So orchestration layer is that how are you going to make sure that all of these four things are going to connect with each other? For example, a good example is N8N. So on N8N, I'm going to have different nodes of LLMs, tools, memory that connect with each other. Now, this orchestration layer could also be a reason of failure. If it has a lot of latency, it is across the geographies or maybe there are some kind of orchestration issues, this can also give you certain kind of challenges, right? So, you as a product manager don't have to fix anything right now. You should understand them as variables. You don't have to love your product. You have to make sure that your aim is to give the best experience to the users and be helpful for them. So now you are going to start from here. After this, what you will do is you need to understand how your product is performing.

**Ankit Shukla** (00:27:54)

So what you will do is in order to see that performance, you will create a very good data set. This is where I have marked this as star because this is where most of your efforts are going to go. You have to create this data set, which is data set is nothing but what are the different kind of inputs that users can give your product. Right. So you are going to collect the past data. So for example, at Indie Money, they already have, let's say, some kind of advisors, which are humans who are sitting at the back end. So they also offer a service where you can talk to an advisor. So they can talk to advisor and they can understand that from the logs that these are the different kind of questions that people generally ask. So that will become one source of data. The second source of data is research.

**Ankit Shukla** (00:28:30)

They are going to go to Google, chat, GPT and all in order to go ahead and research as in what do people ask when it comes to understanding about a stock. Similarly, they are going to use LLM. So with LLM, you can also generate something called as the synthetic data. You can tell that this is a product that I'm offering. Can you go ahead and give me some kind of sample data set? And then it is going to give you some kind of data set. And then eventually there are experts. You are going to talk with real investment advisors. You are going to ask them that what are the different kind of questions that people ask? And then you will get them to fill certain kind of sheets. These four things are very important because they are going to make sure that you are actually dealing with real cases.

**Ankit Shukla** (00:29:05)

So once you have that, then you are going to run it through your base product, whatever you have created, and then you'll get certain kind of output. And I can assure you, and you'll also get surprised when you'll see that, no, this output was not as good as I was thinking my base product to be. And most of the times you might not be a good judge for the same. So you can also include experts. So let's say I'm a product manager. I do not know that what is a good advice, what is a bad advice in terms of finances. So I'm going to involve a financial expert in this particular case. And then I'm going to ask them to tell me whether these outputs are good outputs or bad outputs, which is they have failed or passed the criteria. Okay. And then they also need to tell me that what is that criteria, right?

**Ankit Shukla** (00:29:47)

Otherwise, what happens is most of the people, because if product manager, they are not like if they are not subject matter expert or domain experts, they'll not be able to come up with the right kind of evaluations. Once you show people data, then they'll be able to tell you that this is a mistake. So it's easy to point mistake rather than to go ahead and prepare for them in advance, right? So what we'll do is we have this output, we have these remarks. Now these remarks are again going to go through this. So what we'll do is from the expert analysis, from the user empathy, from the success criteria, from the expected user behavior, what we'll do is we'll have a set of evaluation metrics. That now we should make sure that these things do not happen. So one of the investment advisors will see that we are going ahead and building this.

**Ankit Shukla** (00:30:26)

They will say that this output machine is actually cut. So one of the evaluation experts can tell you that your product is actually generating recommendations. Or the information that it has given is very outdated. Or they are trying to hallucinate the information. So you are going to take all of these outputs by actually giving them the input and the outputs. And then you are going to decide these metrics. Okay. And understand, it will take you some time to understand and decide these metrics. That is why I have also created a cheat sheet. Okay. So this is a cheat sheet that I have created with the help of, let's say, some of my knowledge and Claude and GPT. If you are building any kind of product, I'll make this available in the description as well. Akash will make it available. Where you can understand that for what kind of product, what kind of evaluations metrics should you go ahead and consider.

**Ankit Shukla** (00:31:10)

Right, so this is a very exhaustive cheat sheet. After that, what will happen? Now, I have certain kind of criterias. Now, I will decide what should I use for evaluations. Things which are very definitive. I am going to use code for the same, such as whether I have all the words mentioned or not. whether I am following a certain kind of criteria, which is summary length or not. Then I'm going to use code for the same. This is cheapest. In some ways, I'm going to use humans. In some of the evaluations, I can use LLMs. But most of the times, I'm going to use hybrid. Hybrid means that LLMs are going to flag situations that is not working. And then the human is going to go ahead and maybe give it a final call. Right. And then you are going to write evaluations. Okay, so now in the machine learning or LLP world, we already have some, I would say, some base level evaluations that can be done by code.

**Ankit Shukla** (00:31:54)

For example, this length, this bilingual evaluation, this Rav and Word evaluation. word ratio. Here we are going to make word error rate. Here we are going to make sure that we are able to understand whether this is following this criteria or not. And then in some of the parts where code cannot work because it is, let's say, it is something that is very subjective, then we are going to use other evaluations. So evaluations with LLMs can be of type such as measuring the guardrails, understanding the UX, tone, helpfulness, relevance. This can be done with the help of prompts that we are going to give to a large language model and we'll make LLM as a judge. Now, once we have done this... Rogue mean? Yes. So, there are two things, blue and rogue, right? So, in blue and rogue, what happens is, traditionally in machine learning, we tend to see that, let's say, if I am, let's say, I have some output, which is given to me by the machine learning model, and then I have a golden data set, right?

**Ankit Shukla** (00:32:50)

So, now what I'll do is, I will not play intelligently, what I'll do is, let's say I'm saying, I am... Wait, I'll try to explain this again. I'll take the question from rogue, okay? Yes. Yes. So, BLEU and ROGUE are two methods which are going to help you understand the recall value and the accuracy for your models. For example, let's say I have a case where I am getting this output from the large language model. The output is the cat is on the bed and then the golden data set. Golden data set means this is the real output. This should be the accurate output. bed sorry the cat is on the mat right now these things are entirely different in terms of meaning right it is a different scenario this is a different scenario but what blue and rogue do is they are going to compare the words which is if you go ahead and consider the blue and the rogue matrix for the same it is going to come around let's say i have one two three four five six words and here i have one two three four five six words the blue and rogue are going to tell me that five of the six words are matching that means Yes, your output data and the golden data set are actually matching with each other, right?

**Ankit Shukla** (00:34:01)

But if you go out and use another LLM, you will understand that, boss, this is not true. The cat on the mat and cat on the bat is actually a different kind of statement, different kind of scenario. So that is where they are used, right? Now, in traditional machine learning, they are used a lot. They can be used in order to make sure that your information is grounded or not. You can just do some math making. But ultimately, if you're giving answer on the basis of blue and rogue only, you'll not be able to do it. That is why these are slowly getting outdated from real genii cases.

**Aakash Gupta** (00:34:29)

Yeah, so these are the generic ones. And I've also heard this as rouge. So that's R-O-U-G-E, which is the recall-oriented understudy for disting evaluation. And I think you mentioned these come from the traditional ML and NLP. People don't know machine learning and neurolinguistic programming language. So these are the initial ones, but it's these evaluation prompts that you have below the functions. That's where a lot of the meat and the success is going to be driven from, right? Yes, correct. But...

**Ankit Shukla** (00:34:56)

It does not mean that you will not use these because when you can use a needle, why would you use a sword? So we should not repeat the mistake that we are only using the costly effective methods because we don't want to go ahead and engineer things in the best possible way. So don't try to say I'm because these are going to, these costs are going to compound in the future. Yeah. Right now. So now once we have set the guardrails, we have created the evals. What we'll do is we will now run these evaluations. OK, we are going to run these evaluations. Now what we'll do is as we are running these evaluations, there are two methods of running evaluations. One is the offline evals, which is we are going to run this on the product before we launch the product or before we make a major release.

**Ankit Shukla** (00:35:36)

Yeah, make sure that whatever changes that we have made, they're actually correct. Right. This is like the alpha beta testing that we go ahead and do. Right. So you are going to define the system prompts, model selection and all the other parameters that I have mentioned.

**Aakash Gupta** (00:35:49)

And I think that this is a really important point to double click on for people. The way the best AI companies work is that the AI PM defines these evals. And that is basically the PRD for the AI engineers. Then the engineers say, OK, here's how we're performing on the evals. We're at 36%, 42%, 56%, 80%, and 10%. What they're going to try to do is all those low ones, 10%, 34%, 62%, they're going to try to get those to like 80% or 90%. And then you'll actually go ahead and ship something. So there's this hill climbing mechanism. And that's why evals are so important. And when you keep hearing this term offline evals, don't think offline equals unimportant. Offline is actually the critical pre-development process evals that are your PRD. Is that right? Yes, correct, correct,

**Ankit Shukla** (00:36:37)

correct. So what happens is if you're not doing offline evals correctly, then you don't even, I would say, you have not even created a product that can be actually launched to the real audience, right? I'm not saying that offline evals should be always perfect, but at least whatever you know, you should try to go ahead and implement that before you go ahead and launch the product. Yeah.

**Aakash Gupta** (00:36:55)

This is how you're traditionally we define like the edge cases, the corner cases in the PRD. We're defining those in the form of evals now. Yes, correct.

**Ankit Shukla** (00:37:03)

And then what will also happen is that, yes, offline evals are good. Many people do it. But there is also something which is equally, if not more important, which is online evals, which is you have to use a platform. You can use any of the observability platforms. All of them are now having these two major popular ones are Arise and Trulence. So what they will do is you will keep on observing the product. So, I have talked about data drift in the beginning, which is that now the user expectations have improved. So, your current prompts, whatever you have tested in the evals or your current models or something is now not working. The world has changed. So, you are going to keep on observing and maybe if not on every output or input, you are going to run the online evals, which is the same evals on your production level data.

**Ankit Shukla** (00:37:45)

Maybe you'll not run it on every input and output, but maybe you'll choose 1 in 10, 1 in 100, 1 in 1000, whatever is the, let's say, the ratio that you need to take because they are costly as well. And then you are going to make sure that you are observing them. And whenever any change is made, you are going to make sure that you are able to observe them and you are able to make changes again in your base product. And then this whole cycle is going to go ahead and repeat itself. Okay, so just to give you like everyone a summary again, we start with the success criteria and expected behavior. On basis of that, we are going to get one level of metrics and our expectations, what the prompt should do. And then we are going to create like a base product where we are going to put the very primary prompt, very primary system prompt, whatever the best thing that we can do, right?

**Ankit Shukla** (00:38:26)

And the models and everything. After that, we are going to collect a lot of data from multiple places, edge cases, and from the expert, from the LLMs and all. And then we are going to go ahead and run all the data set input data set with our base model, like our base product. And then we are going to evaluate everything. We are going to create evaluations based on the mistake that we have found. And then we are going to make this into evaluation. So evaluation will become, let's say, a set which is going to run all the time. Whenever you are releasing them, doing the major release, you can choose it to run every week or every month so that you know that if the data is not drifting. And then you are having something called as online evals, which you are going to run in the production level data set.

**Ankit Shukla** (00:39:03)

And you are going to get informed whenever an evaluation is passing here and there. For example, we have an evaluation called as accuracy. So if we believe that accuracy is anytime going less than 98% in these evaluations, then we should get flagged and we should go ahead and maybe improve the prompt of any of the orchestration that we have. So this is like the whole end-to-end flow that you do while creating evaluations.

**Aakash Gupta** (00:39:21)

Awesome. And it sounds like a lot of the art here, or actually I know a lot of the art here is in writing those LLM judge system prompts, creating those metrics. So how do we see this in action?

**Ankit Shukla** (00:39:33)

Yeah. So what do we do is, let's say I have created, let's say a PRD. Let me just go ahead. Yes. So, let's say this is what a product manager will actually do, right? So, this is, I have created, I have reverse engineered this. I am again saying that I am not affiliated to the company. So, if there are some similarities that are just coincidental. So, I have reverse engineered this product and this is what they would have done. Okay. So, I have broken down the document into these 10 sections. The first part is like before you talk about AI PM, understand that you are a PM first before an AI PM first to make sure that you are setting the context correctly, which is this is the product. This is what it does so that you are able to understand it. So yes. And you have to always start with writing the value for the user, which is reduce search friction, decentralized financial.

**Ankit Shukla** (00:40:16)

So what is the value of the user? That user do not have to spend a lot of time in order to search for something that is the value for the product. They'll get the advisory within the product itself. And then we have written down the value for the business because these are again going to come when you go ahead and understand the metrics for evals and your product. And now we are going to make different layers. Okay. One is a user interface layer. I'm talking about these layers because these layers are also going to decide your metrics. So user interface layer, orchestration layer, data retrieval layer, LLM layer, logging analytics. All of these are going to play an important role in your eval systems. And then eventually this is the level one. Okay, so I have not written a complete prompt, but I have written what will go into that prompt, right?

**Ankit Shukla** (00:40:56)

So, prompts and context, system prompt core, and AI assistant is configured with the following key principles. Now, look at this. Role as an analyst, not advisor. So, I know that I don't have to ask it to be an advisor and suggest me something. I want it to just act an analyst and then give me the understanding. Although it is a very small line, but this is going to define the behavior of the system. So I'm going to use all of these things and understand that I'm not writing the whole collective prompt because I have to make it iteratable. So what I can do is I can look from these points that yes, now in the new eval, whenever I've run eval or whenever I have to change the system prompt, I can choose which line I need to pick. Otherwise, in the bigger prompt, it's very difficult to go ahead and find what you want to go ahead and edit.

**Ankit Shukla** (00:41:36)

So we have to be, let's say, taking care of productivity because these are like small frictions that let product managers to not do the right thing.

**Aakash Gupta** (00:41:44)

I think you're bringing up an important point, which is that you need to be very sensitive to your organization and you need to go to your development leader, AI engineers, your head of product, and clearly define where does the role of PM end and the role of engineer begin? Yeah. I think this is a nice line you've shown here where there's guidance for the system prompt, but you're not necessarily saying this is exactly what the LLM judge and system prompt should be. That's going to often be the case in a larger company. where your AI engineers are still going to be the ones writing the system prompt for your evals, but you've defined at a high level how it should look. At a smaller company, you might actually be writing the system prompt. You might actually be in an Arise or something like that. So it's good to have the skill, but it's really important to understand where PMs should be in this.

**Aakash Gupta** (00:42:33)

And I think your example here, this is more for a slightly larger company. Is that fair?

**Ankit Shukla** (00:42:37)

Yeah, I think I would say it would depend upon the autonomy that a PM gets. I have seen that in a larger companies, also some people are able to be more agentic and have some more agencies and they are able to do all of these things. But in small companies, generally, you don't have to do a lot of things as a product manager because then you are figuring things out as the light becomes more clear. Makes sense. Yeah. Right. So now these are the response guidelines. And then these are also some context variables that we are going to inject in some queries and understand this document has to be created so that everyone is on the same page. Right. So don't just think that you have written an evaluation prompt and then your task is done. You have to give all of this context so that people can read it and they can understand.

**Ankit Shukla** (00:43:16)

Because understand you will not be the eventual person who is coding and the engineers have to be aware about all of these things. Right. Now, yes. So now I've also mentioned that for maybe fundamental analysis, technical analysis, these are, let's say, other things I need to make sure that I'm giving to the context to the AI so that it is not able to hallucinate. What do some of these acronyms mean here? For example, if I talk about fundamental analysis, then I need to collect the information. So whenever I have to understand a stock fundamentally, I need to look at a variable called as P ratio, which is profit to equity ratio, right? Here I need to, and I need to make sure that I'm giving this context to the LLM that what these terms are so that it is not able to do a mistake of hallucination.

**Ankit Shukla** (00:43:58)

Now understand, I could have not done this and I could have used GPT-5, but that would be a very lazy decision, right? Because in the long run, the costs are going to combine. What can I do in order to give more context to the AI? And then maybe I'm okay with using a lesser capable model. That is what you need to understand as a PM. So

**Aakash Gupta** (00:44:17)

almost putting on the hat that you're not working with the best model.

**Ankit Shukla** (00:44:20)

Yes, yes, yes, correct. So aim for the best, but design for the worst.

**Aakash Gupta** (00:44:26)

Makes sense. Yes.

**Ankit Shukla** (00:44:29)

Yes. And then, yes. So then we are going to also put, so understand, you understand what, what evaluations are, but engineers might not have at the top of their mind or maybe designers or the leadership might not have the top of their mind because they are only exposed to the prototypes. They're not about like familiar about this nature. So you have to clearly explain why it is happening. Right. Here is a high stakes domain. And in India, this space of FinTech is heavily, heavily regulated. You cannot do this even without, let's say, doing evaluation. And also understand, it might happen that sometimes this is going to go wrong. At least at that point of time, you'll be able to show the regulation that we have taken all the failsafe features to make sure that it is not happening. Right. And then we are going to have all of these.

**Ankit Shukla** (00:45:07)

I'll share this document so that everyone can read in advance. And then we'll have these deciding metrics and expected behavior. So what are the evaluation dimensions? Factual accuracy, compliance, groundedness, relevance. This is what it means. And this is why it matters. So understand it will take some time to read this document and you don't have to write it by yourself. My general recommendation is what you should do is if you are really like an AI enabled PM, go ahead, walk through whisper flow to your GPT or your cloud or your Google doc. Right. Talk as much as you can because that is more productive. After that, ask Claude or GPT to go ahead and put it in this structure. Right. So you are you will and also ask GPTN plot to also fill the gaps that you have missed in this particular document. And then we have some more documents.

**Ankit Shukla** (00:45:49)

Yes, we have also defined some thresholds. So numerical accuracy means that let's say if AI is suggesting any kind of numbers, images or percentage of returns or numbers, I should make sure that my target is more than 98% of the time they should be correct. And if it is becoming more than less than 95%, I should get flagged and this product should not go into production. Unless I'm improving something, right? And I have also mentioned this. Now, this is super helpful for the online evals, which is if this metric compliance pass rate is going below this, then I should take an immediate action, right? Immediate action. And then this is the expected behavior by query type. That's now. This will not come out of the blue moon. You would have gone ahead and done this process of creating inputs, outputs from the expected inputs. So what we'll do is, yes.

**Ankit Shukla** (00:46:37)

So here we are going to make sure, where is the document? Yes. So here we are able to observe that maybe these are the things that should never be missed. Right. And then we would have some edge case behavior, which is stock with missing data, penny stock, these kind of things. And this will only come once you are collecting all the data in your data set. Otherwise, it will not come at the top of your mind. Right. Now I can show you the data set. Now understand this is all synthetic, synthetically created data set, but that will serve the purpose of learning. Okay. So we have divided into multiple parts and these are the sources. Let's say for fundamental analysis, what I'm going to do is I have collected the data from multiple sources, synthetic data, talking to the experts, looking at my own data, doing my own research and I was able to understand these things.

**Ankit Shukla** (00:47:21)

Let's say if someone asks, how good is ITC as a dividend stock? Then this is the context that I need to give and this is what I expect. And then eventually these are going to be the red flags, right? So now eventually what I'll do is I'll not write the valuation prompt by myself. I will put all of these things, this information into an LLM and ask it to write a better prompt. Right. Because as a human, you can go ahead and miss out on a lot of things. And then you will run all of these things again with the data set to make sure that it is not making a mistake. Right. And I've also said some kind of priorities. So the

**Aakash Gupta** (00:47:53)

role of the human is figuring out what are the expected elements, what is the overall guidance for the prompt, then use AI to create the final prompt. And there are studies that show that AI is better at writing prompts than humans. So... Put AI where AI is better, put humans where humans are better.

**Ankit Shukla** (00:48:10)

Yes, correct. And I think collaboration is the best way out there. Rather than competing, you should collaborate with an LLM and then both of you are going to unlock different kind of powers. Yes, for sure. Yeah. And then this data set is there. And then understand that we have done multiple methods of collection, which is we have taken it from production queries. If you are creating a support chatbot, you would be giving support before this chatbot, right? So you can collect that data. Then there are expert curation. In this case, we can take ideas from the financial experts. And then we are going to do synthetic generation. And then we are also going to look, this is also important that we have to maintain this data, which is Although at time when it is not needed to manage this data very frequently, but if your product is, let's say, talking about a use case where data is very much changing, you should make sure that you are able to at least upload this data once in a while.

**Ankit Shukla** (00:49:01)

So this is kind of your test use cases, which should run always before you are doing a major release, right? And then this is evaluations, right? So we are going to do three kinds of evaluations, automated programmatic evals, LLM as a judge and human evaluations, right? Right. For automated wells, I can do factual accuracy checker, compliance checker, groundedness checker, structural checker. What I can do is I can just match the words. Whatever is happening, numbers and all, do I able to see it in the sources as well? Right. And then LLM as a judge, I can check relevance, balance, tone, and then I can. So I will not create a prompt by myself. I'll just give this particular thing to an LLM. It is going to go ahead and generate like a good prompt for me. Right. And then as a human evaluation protocol, I'm going to use, I'm going to use them humans because they are costly and they are going to take time.

**Ankit Shukla** (00:49:47)

So whenever a new feature launches, something happens, like something important happens, I'm going to make sure that they are using the same. Right. And if the automated metrics, let's say the LMM is a judge or these things are failing, then I'll make sure that I'm involving a new human to check what is happening out there. right and then yes now this is a bit different thing which is I can for a human I have two methods I can ask them to just give me pass for fail or I can give them a rating of 1 to 5 different people have different kind of opinions but it's good to start with maybe a pass or fail criteria so that people are objective but eventually as you go forward Even if people are rating 1 to 5, ask them to give you a remark, which is why do they think this is the case?

**Ankit Shukla** (00:50:28)

Because you can use the data in order to further train your, like further improve your, let's say, context or the models, right? And then we have tests. This is the criteria that at any moment of time, we have any kind of these issues, we are going to make sure that we are going to block the deployment, right? It should be actually less than that. Yes and then offline event I think this we have already understood but I'll share this document. Yes so here what we are doing is that we are going to smoke test we are going to do full regression and everything we are going to run all the let's say all the evals and we are going to do block or no block in these particular criteria we will not release it and then on the online evals what we'll do is we will have the latency so p50 p95 p99 means that whenever we do averaging averaging is not going to give you the right kind of results so let's say If you are having 100 users on your website and if you are going to see that maybe 10% people.

**Ankit Shukla** (00:51:19)

So I think that's an important part. So I can take some time here. So in order to measure latency, in order to measure, so many people might have heard about P99, P95. Okay. So what are these things? So let's say I want to measure the latency of a product. then I cannot say that if 90% people are getting it at 100 millisecond and 10 people are getting it at let's say 1000 millisecond or 10,000 millisecond. If I take the average, average will come maybe something around let's say a better number. It will look like let's say not a big number but still 10% people are facing the issues. P95 means that 5% of people, like 95% of people, are actually having this kind of latency, which is, let's say, a good number, right? Or maybe I can say P99, which is the most used metric, which is 99% of the people should be able to get the results within, let's say, a particular latency, let's say 100 milliseconds or 10 milliseconds, because averages do not work there.

**Ankit Shukla** (00:52:16)

So you have to maybe write these kind of latency metrics. And then eventually... Yes. So this is their sampling based quality. Well, this is good. User feedback. Yes. Now this is one thing which is more important that apart from only running your evaluations, online evaluations have one more input, which is after every AI tool has finished doing its job, you will see a hands up or a hands down option, like thumbs up or a thumbs down option so that you are able to integrate it back into your product. right this is like a hard feedback but a soft feedback could be that people are again and again generating time to generate the same answer or they are not closing the session as soon as possible they are just going ahead and maybe frustrated with the answers that means that you have a soft feedback which you should also go ahead and consider and some other things such as maybe they have removed the session before going ahead and buying or selling something or they have gone ahead and escalated it to support that means that your evaluations are maybe not working so also consider these as evaluations like also consider these four things also as some kind of i would say evaluations in your product right and then drift detection is already there yes and then we have a b testing query which is that make sure that you are also going to go ahead and maybe do some maybe testing on various kind of evaluate like with various kind of prompts and models and something so that you are able to understand how evaluations are running over there what is the user experience and And then we have the last

**Aakash Gupta** (00:53:34)

part. Can you say a little bit more about that? So are you A-B testing the

**Ankit Shukla** (00:53:37)

evals? Yes. So we are testing, we are, okay, so evals cannot be A-B tested. What we'll do is we are A-B testing the prompts and the models. And then we are going to see in production that how do evals perform there. Evals plus the hard and soft feedback from the users. So it might be possible that your evaluations are running correctly, but the user has something else to say. Right? So, these will be testing will make sure that you are paying the right stuff for the users and you are not too much short-sighted by your synthetic evaluations.

**Aakash Gupta** (00:54:07)

Yeah. Makes sense. You can't just only rely on the online evals. You have to actually look at the user data. Yes, yes, yes.

**Ankit Shukla** (00:54:13)

Correct. We don't understand. Your evaluation did not come out of your own mind. You have gone ahead and maybe done a lot of research on subject matter experts, right? And here also, you have to understand that you don't have to stick yourself or you don't have to go to a fixed mindset. You are going to be evolving with the user feedback as well. And there is no better method than to understand the user with the help of A-B testing. Right. Yes. And then this is going to be continuous evaluation improvement, which is online eval and offline eval are going to be in continuous loop with each other. And then eventually we are going to have this coverage, which is what are we testing? What is done through online? What is done through offline? And what is the frequency out? This is very important because many teams want to do is they think of this process as a set it and forget it part.

**Ankit Shukla** (00:54:57)

Which is, I've just done the evals, the product is done, now what do I need to do? But if you're not observing, if you're not setting a cadence for improving your evals, improving your prompts, then you are going to suffer from data drift. And it happens with many of the products. Initially, when it launches, it looks very good. But after a certain period of time, the expectations of the users are also increasing. That is one thing. But the quality of the things get reduced because now the data has changed. Like the evaluations need to go ahead and evolve. Right. So this is like the end to end, how you are going to go ahead and do like a real life production level in your evaluation documentation as a product manager. I understand you don't need to like create this detailed documentation, at least create something basic and take the help of LLMs and just make sure that before you reach to the team, you are able to take a quick look on the same.

<!-- sponsor -->
**Aakash Gupta** (00:55:44)

You know that feeling when you try to prototype something with AI and it spits out something completely generic? Then you spend hours tweaking colors, fonts, copy, and features just to make it feel like your actual product? Here's the problem. Most AI app builders aren't built for product teams. They're built for those starting from scratch. But product teams aren't building from zero. You have an existing product, real customers, design guidelines, a backlog full of ideas you need to explore and validate fast. That's what Reforge Build does. AI prototyping that starts from your product. Add your customer feedback, strategy docs, and product features as context. Create reusable templates using your product design. Explore multiple variants side by side. Collaborate with your team in one place. Reforge Build generates prototypes that reflect your real pricing tiers, real features, real customer language, not generic placeholder. Stop fighting tools built for founders.

<!-- sponsor -->
**Aakash Gupta** (00:56:33)

Start prototyping like a product team. Reforge Build. AI prototyping built for product teams. Try it free at reforge.com slash akash. That's R-E-F-O-R-G-E dot com slash A-A-K-A-S-H. And use the code build for one month free of premium. Yes, please edit it and don't just send them some LLM slop or they'll start to lose respect for you.

**Ankit Shukla** (00:56:58)

Yes. And one more advice I would give to people is, now there is a major issue that I'm sure that most of you, when I was scrolling through this document, you were looking forward to a download link that when can I share this document with you. But I can assure you that 99% of you are not going to read this document ever. And this also happens with our engineers. They don't have time to read all of this. So generally what I do is like this is just a stakeholder management hack, which is taught at Amazon, which is that if you really want people to read these documents, get them on a meeting and maybe for 15 minutes of that initial part of that meeting, 15, 20 minutes, get them to go ahead and read that document while you are in the meeting. So if the document is important, first of all, don't write too many documents.

**Ankit Shukla** (00:57:37)

You can write them for your own clarity, but don't expect other people to go ahead and read it. But in some cases like this, if you have to really have to go ahead and write a document, make sure that other people are reading it. And the best best hack is to make sure that if you are considering a 20 minute meeting, make it a 35 minute meeting and dedicate the initial 15 minutes for people to go ahead and only read that document.

**Aakash Gupta** (00:57:57)

Makes sense. So we've covered what this all looks like. Can you maybe bring this back to us with some real life examples of why evals matter? Yes. So

**Ankit Shukla** (00:58:08)

I'll give you some examples. Yes. So before I could talk about all the examples, one, there is major, I would say, confusion in the world that evals are nothing. But fancy QA role that has been now given to a product manager. Okay. Yes. And that cannot be far from reality because now you have seen the process. Okay. A QA is not involved with the subject matter experts. A QA is not improving the prompt. He's not improving the product. He is going ahead and informing. So information is different from transformation. As a product manager, you are transforming your product. While as a QA, generally you are giving the information to the developer that no, this is not working. So there is a difference between the transformational role and an informational role. So don't think that if you are doing evals, you are just doing the job of a QA.

**Ankit Shukla** (00:58:49)

It is much more than that. Although the terms are matching. Yes. Yeah. Now talking about why evaluations matter, and I'll give you some cool examples. So reliability and trust, right? So evaluations, like good evaluations can give you reliability and trust. If you consider example of Grammarly, that if one tone error can change, like let's say, Grammarly will translate across multiple languages. So if one tone error can change meaning across 500 plus scenarios. So there is a lot of trickle down effect, right? So if you're writing good evals, you are making sure that yes, the tones and everything is matched correctly. Similarly, this actually happened in GitHub Copilot that when it was initially launched, they had a very small error. The error was that in the YAML file, there was some mistake and that was not caught by the code. And they don't have evaluations for the same.

**Ankit Shukla** (00:59:37)

And what happened was, when people started using it and when they were moving it to production, most of their products were breaking, right? So if they would have written an evaluation, this would not have done. And now it's a scale product, so it faced a lot of repercussions. Then we give Klarna. So Klarna... make sure that they are not so initially when Klarna developed their AI chatbot they were focusing on things such as how many people are looking at this short bot how many people are saying that it is helpful but soon they were able to understand where they need to push people in the conversion funnel so there are business metrics also that we need to take care of and then they transform the strategy and now they are using the AI led suggestion increase their AI led suggestions are now increasing the checkout conversion rates So don't think that it is only for the users.

**Ankit Shukla** (01:00:24)

You should also evaluate your AI on some business metrics. And then eventually, chatbots. You will see a lot of chatbots that, let's say, you created a chatbot. You created a chatbot on, let's say, some information that is available right now. But in the future, if you add more products to your system, and if you are going ahead and maybe some context is changing for the users, the user behavior is changing, your products are changing, then you have to make sure that your evaluations are always running. They are always online, right? So that is why a chatbot, maybe any chatbot that you are developing for, this is a very common use case that chatbots are being developed for customer support by AI. Then support chatbot will keep giving old policy into drop CSAT and it will lead to, okay, I'll repeat this again. I'll repeat the chatbot part, okay?

**Ankit Shukla** (01:01:07)

Okay. Yeah. And another very interesting use case is the chatbot that whenever you are building like an AI assisted chatbot to support your customers, then a major issue is that if you are only giving it older information, if you are not making it very relevant, then you are going to give outdated information to the users and then that is going to fail the efforts. And you will not be able to know whether the information is old or new unless you are running the evaluations. So evaluations are going to play a very important role in all of these things. And in the end, my major takeaway from the session would be for everyone is that evaluations are not optional. They are the guardrails for all the AI driven outcomes. Don't think that you'll be able to create like a very solid, complex product without having the right kind of evaluation.

**Ankit Shukla** (01:01:46)

Also, evaluation is not like I would say it's a goal. It is actually an ongoing journey which will keep on evolving as your product evolves.

**Aakash Gupta** (01:01:54)

So there you have it, folks. We walked you through, if you recall, at the very beginning, the intuition for what hevels are. If you're making and getting instructions for making chai, even the same LL model is going to give you three different responses. That's non-determinism in action. To check, are those responses acceptable? Are they not hallucinating? Are they at quality? Are they at the length that we want? We would create evals for those. Some of those would be code-based evals. Some of those would be LM judge evals. Some of those would be hybrid human evals where you bring a system... a domain expert, a subject matter expert, in to help you. And so this eval is not just a QA rebranded. It is a critical skill. It's almost part of the PRD. We saw the long document that Ankit created. We are going to include all those links for all these things that we shared in the description below of this episode or in the newsletter accompanying and summarizing this episode.

**Aakash Gupta** (01:02:52)

So that'll give you all the resources to go build these evals yourself. Don't be scared of adding AI to your features, guys. AI is just another API. And with these avals, you will be able to handle the non-determinism of it. Ankit, thank you so much for this masterclass in evals.

**Ankit Shukla** (01:03:09)

Thanks, Arulakash. Happy to be here and happy to be helpful.

<!-- sponsor -->
**Aakash Gupta** (01:03:11)

See y'all later. Take care, guys. I hope you enjoyed that episode. If you could take a moment to double check that you have followed on Apple and Spotify podcasts, subscribed on YouTube, left a rating, a review on Apple or Spotify and commented on YouTube. All these things will help the algorithm distribute the show to more and more people. As we distribute the show to more people, we can grow the show, improve the quality of the content and the production to get you better insights to stay ahead in your career. Finally, do check out my bundle at bundle.akushg.com to get access to nine AI products for an entire year for free. This includes Dovetail, Mobbin, Linear, Reforge Build, Descript, and many other amazing tools that will help you as an AI product manager or builder succeed. I'll see you in the next episode.
