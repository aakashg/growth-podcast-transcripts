---
title: "Complete Course: AI Product Management"
subtitle: "In today's podcast, Pawel Huryn shows you every key skill to become an AI PM. We go from basics to expert mode: starting at AI prompting, then AI PRDs, fine-tuning, RAG, MCP, and finally AI Agents"
date: "2025-04-22"
host: "Aakash Gupta"
guests: ["Pawel Huryn"]
speaker_names: "substack"
substack_url: "https://www.news.aakashg.com/p/complete-course-ai-product-management"
youtube_url: "https://www.youtube.com/watch?v=IfW1FMDkw4k"
duration: "01:36:17"
word_count: 10576
source: "Substack episode transcript (aired audio)"
sponsors:
  - name: "Linear"
    url: "https://linear.app/partners/aakash"
  - name: "Miro"
    url: "http://miro.pxf.io/PO4WZX"
  - name: "Amplitude"
    url: "https://bit.ly/4hl25RG"
---

**Sponsors:** This episode is brought to you by [Linear](https://linear.app/partners/aakash), [Miro](http://miro.pxf.io/PO4WZX) and [Amplitude](https://bit.ly/4hl25RG).

# Complete Course: AI Product Management

*In today's podcast, Pawel Huryn shows you every key skill to become an AI PM. We go from basics to expert mode: starting at AI prompting, then AI PRDs, fine-tuning, RAG, MCP, and finally AI Agents*

**Pawel Huryn** (00:00:00)

In today's episode, we cover everything, prompting, fine-tuning, rack building that you need to know to become an AI product manager.

**Aakash Gupta** (00:00:07)

Are all PMs going to need to become AI PMs?

**Pawel Huryn** (00:00:10)

The AI market is growing so fast that there is a high probability that we will meet more AI product managers in the future.

**Aakash Gupta** (00:00:16)

You can't just prompt like an average person, right? You need to be prompting at a very high level.

**Pawel Huryn** (00:00:22)

And we instruct ChatGPT to think separately from different perspectives. I like adding that you will get $1,000 if you perform this task on a champion level or something like that.

**Aakash Gupta** (00:00:32)

Why are AI PMs paid so much?

**Pawel Huryn** (00:00:35)

One of the reasons is that they need to combine business skills with the technical knowledge. Then based on this generic information, it plans up to 11 separate tasks, and those tasks are distributed to different

**Aakash Gupta** (00:00:47)

agents. It's not that everyone needs to become an AI PM. This market is growing really fast, and we just gave you all the tools to become an AI product manager. Looks like that's ultimate list of product metrics. I'm a dummy, so I'm still trying to understand when do I use fine-tuning or when do I use RAG? Really quickly, I think a crazy stat is that more than 50% of you listening are not subscribed. If you can subscribe on YouTube, follow on Apple or Spotify podcasts, my commitment to you is that we'll continue to make this content better and better. And now on to today's episode. Paul, thank you so much for being here again. It's great to be here. Thank you, Akash. So I want to talk a little bit about AIPM. Why are AIPMs paid so much?

**Pawel Huryn** (00:01:36)

That's a good question. Yeah, they are definitely paid more than an average product manager across different industries and regardless of their experience. One of the reasons is that they need to combine business skills with the technical knowledge. So even though you do not have to... Just like with technical product managers, you do not need to code. And in this case, you will not fine tune or create AR workflows. But you need to understand the technology good enough, well enough to work with engineers. And that might be challenging. This is a new technology.

**Aakash Gupta** (00:02:18)

Yeah, I think that's one thing. And then the other thing is it's just such a hot area, right? So all of the PMs want to go into it. And I think that as a result, what we're seeing is that the best companies, they're trying to pick up the best talent. And to pick up the best talent, you might need to pay a little more. So today I want to break down for everybody how you can become an AI PM. And I want to start at the very basics of AI PMing. You need to be able to prompt well. So can you break this down for us? Yeah, of course. You want me to

**Pawel Huryn** (00:02:51)

demonstrate a prompt, share my screen? Yes, I would love to see how you prompt. So an example prompt from my article where I describe the best practices is like this. So first, this is a prompt about identifying hidden assumptions for the product trio, which performs continuous product discovery. And the first thing we want to do is to explain the context. So just like when we are working with engineers or product teams and we want to communicate the context, so not only what is the task they are supposed to perform, but also why it matters and the how it aligns with a broader organizational context. So in case of working with LLMs or AI in general, we also want to explain this context. So I informed ChatGPT that it is working in a product trio, performing continuous product discovery. I explain what the goal is, what are the team objectives.

**Pawel Huryn** (00:03:52)

The next thing that is in this prompt are identified opportunities related to that objective that might be the result of interviewing customers. And only after providing all that context, we ask about assumptions that needs to be true for those ideas to work. So we have, sorry, we have idea that one of the ideas might be offering automated investment recommendations. And we instruct ChatGPT to think separately from different perspectives. So this is a perspective of a product manager, experienced product designer, and experienced software engineer. And we would like for each of those personas to identify assumptions related to value, usability, viability, and feasibility. And what we have done here is, so the first element is introducing the context and describing the goal, the broader objectives. What happened before performing this task. So we have identified some opportunities. We have came up with an idea. And then we explain the steps that LLM needs to take in order to perform this task well.

**Pawel Huryn** (00:05:14)

So we have iterating four different roles, and for each of those roles, there is a specific task to perform. Let's try and see what will be the result of the section. Okay, so we have different assumptions related to... The four areas that we mentioned for product manager, product designer, and engineer, those will not be the same risk areas because each of those persons brings a different perspective to the table. And when being so specific and defining the steps that LLM needs to take, also providing the broader context, we can get much more reliable, much better results. So in the post about top high ROI use cases for product managers about the prompting, I explained several hacks. So one of the hacks is to ask AI to play a role, like a product manager, product designer, or software engineer. The next hack, the next important thing is to clarify the context.

**Pawel Huryn** (00:06:26)

So not only what is required, but also why we need it. Another one is talking like we talk to humans, even though LLMs do not have emotions. You get better results if you treat them well. Maybe.

**Aakash Gupta** (00:06:46)

Yeah, I feel like it's like a 1% difference, but just being polite, even including a smiley face helps. Yeah. Yeah.

**Pawel Huryn** (00:06:54)

Another one is to set clear expectations. So it's just like when we delegated ask to a human. It's way better when we specify what are the desired outcomes and how the response should be formatted, for example. What are the success criteria? Like those four risk areas for each of the persons that we selected. In other situations, so for example, if the prompt was about generating a user story, it's very helpful to provide a template. So not just inform LLM that we want the user story, but if we have some user stories that we used in the past, we generated in the past, give them as an example so that the answers can be better aligned. Another one is providing step-by-step instructions. So, for example, first iterate for this and this and this role, then identify assumptions related to first value, second usability, and so on. In the reasoning models, so here, this is one-shot prompting, so it doesn't actually do it sequentially.

**Pawel Huryn** (00:08:10)

But in reasoning models, it will actually iterate on those steps. Another one is avoiding leading questions to avoid injecting biases. I have tested several times and I get better results when I say AI that they will get a reward. So for example, if I have a prompt that I cannot get the satisfying answer, I like adding that you will get $1,000 if you perform this task on a champion level or something like that. And it, for some reason, it works. And definitely LLMs tend to provide longer answers, more detailed answers, if you mention the reward. Yeah, and the last two is just to iterate. So there is a high chance that if you try it the first time, the output might not be ideal. So in that case, we just iterate, try to improve and inspect the outcomes. And in some cases, it also helps if you provide an example of the ideal output, like a user story, let's say, or a product requirement document, and you can ask LLM to reverse engineering.

**Pawel Huryn** (00:09:32)

So what should be the prompt, assuming this is the outcome? And that's a very powerful technique.

<!-- sponsor -->
**Aakash Gupta** (00:09:42)

Okay, so that's skill one for AI product managers. You need to be able to prompt well. You can't just prompt like an average person, right? You need to be prompting at a very high level. The way I would think about prompting is try to think about it like chess, right? hey let me take a quick break to talk about something that's completely changed my product management workflow linear as a pm i was drowning in tools one for planning another for issue tracking roadmaps and sheets and jumping between slack intercom and app reviews just to piece together customer feedback sound familiar i was spending more time keeping systems in sync than actually building product every time development kicked off my carefully crafted plans would immediately need updating i was the human api between all our teams constantly chasing updates and translating between tools That's why I love Linear.

<!-- sponsor -->
**Aakash Gupta** (00:10:25)

I can capture customer feedback, shape product ideas collaboratively, quarterback cross-functional teams, and monitor development progress in one place. It cuts through the maze of disconnected systems that are complicating my life. Product teams at OpenAI, Vercel, Brex, and Cash App all use Linear. If you're tired of spending your days keeping different tools and teams in sync, check out Linear at linear.app.com. That's linear.app.com. today's episode is brought to you by miro let me ask you something how many tools are you juggling just to get a single project across the finish line one for brainstorming another for planning something else for tracking tickets that's where miro comes in it becomes an all-in-one collaboration workspace whether you're consolidating user research from several interviews developing and synthesizing product briefs or a wireframe or project managing development Miro brings everyone into the same space. It's fast, intuitive, and fully loaded with features like project templates, two-way Jira Sync, and integration with software like Draw.io and PlantUML.

<!-- sponsor -->
**Aakash Gupta** (00:11:27)

Miro's AI features can be used to synthesize elements in a board to develop a ready-to-review product requirements document in seconds. If you're tired of tab overload and scattered workflows, try Miro. Head to Miro.com and see why over 90 million users choose Miro to guide from idea to outcome. You can get pretty good at chess if you put in a couple hundred hours, but you're not going to suddenly be Magnus Carlsen until you put in 10, 20, 30,000 hours. And so Paul is sharing some of his hard-won tips and tricks after putting in those hundreds and thousands of hours. I want to move to the next area for AIPMs, which I think this is the one where... It's now veering really into the PM skills, which is an AI PRD. How do you write a PRD in an AI context?

**Pawel Huryn** (00:12:15)

For this one, we partnered with Miktat Jeffer, which is product lead at OpenAI. And arguably, PRD for AI features or AI products is not something completely unique. What is unique is a lot of hype around artificial intelligence. And this hype causes that in some cases, product teams... pursue features or products without a justified business case. So what is included? There are two areas that are included in this PRD. One is ensuring that our initiative is aligned with our business strategy in case of AI features with team objectives. And the second one is including AI-specific considerations, like how we will ensure that there are specific guard drives implemented so that the model is aligned with the user. And there are several sections. This post is still free and can be downloaded from my newsletter or together with the template. But before we discuss the template, maybe it's worth mentioning that the first AI PRD is a tool for alignment, building alignment in the organization.

**Pawel Huryn** (00:13:49)

We don't necessarily need, and I actually don't like it, documenting every single detail, like user stories, tasks, very detailed deadlines, roadmaps. We would rather want to use PRD as a tool to highlight our assumptions and provide some evidence and also connect our initiative to the broader organizational context. And the second thing is that it shouldn't be a distinct phase at the beginning of the product or project or initiative. We usually start with a draft and as we build our feature or AI powered product, we iterate on our PRD. And the sections in the PRD. So the first one is executive summary. So just briefly, we'll briefly summarize what this initiative is about and how it will, what are the success criteria, how it will benefit the organization. The second one is about market opportunity and this is about AI specific because we would like to explain why this is something that we should build right now and maybe this is something that has just become possible.

**Pawel Huryn** (00:15:15)

And also what is the potential for the future? So is this market big enough or will it become big enough in the mid or long term? Another one is strategic alignment, and this is also inspired by this AI hype. So we want to ensure that for an AI product, it is aligned with our vision, our strategy. It supports company objectives. And for AI feature, there is additional assumptions related to our team objective.

**Aakash Gupta** (00:15:51)

Yeah, because you don't want to just build AI for AI's sake, even if your board or your investors are asking you.

**Pawel Huryn** (00:16:01)

customer and user needs so this is quite straightforward so what is the problem we are trying to solve at Let's hope there is some problem. And the only problem, because building an AI-powered product cannot be the problem in itself. So we want to identify market segments, which are clusters of customers with similar underserved needs. And for each of those segments, we would like to understand how important those needs are for the customers and how satisfied they are with what they already have. The next one is our value proposition and the value proposition is about how we will address those needs for each of the segments. So what is important here is that we do not want to focus only on features, but also we want to mention capabilities. and benefits. So what is the current state? What is the customer pain? How we will address it?

**Pawel Huryn** (00:17:06)

So for example, we will introduce a specific feature and what will happen after. So what are the benefits for the customers and also how it is different from what our competitors offer. and how we can communicate it. And for this there is a value proposition template, also value curve so that we can easily compare our value proposition to what other companies offer. The next section, competitive advantage, is about not just competitive advantage right now, but how we can sustain competitive advantage in the long term. So what can we do? So our competitors can't or won't copy our strategy. And this is a classical can't want test from Roger Martin work from his

**Aakash Gupta** (00:17:56)

guest.

**Pawel Huryn** (00:17:57)

Whose podcast, I believe, will be right before yours. Oh, yeah, that's nice. And here, yeah, I'm a big fan, so I will watch it for sure. Okay, and product scope, so high-level assumptions, use cases, links to Figma prototypes, non-functional requirements, so general requirements and how we will measure them, and also AI-specific, so what are the key architectural choices, how can we assess our implementation, so for example, AI-specific evaluation metrics or bias and fairness audits. So AI evals, how do you handle those? I will do a simple demonstration when we will be discussing fine-tuning. Okay, perfect. Okay, and the last one is go-to-market approach. So, what are the build and release phases? What market segments we want to focus on first? So, yeah, this is our, perhaps we want to apply the pitch heads strategy and how we will measure our success. There is also a PRD template to download, which is simplified and much shorter.

**Pawel Huryn** (00:19:20)

So even though this article seems long and the actual template is like three, four pages document. And also there is a case study, and here you can read Nick that explained how this AI PRD was applied to Shopify, and he was responsible for releasing a feature called AutoWrite, which was about product descriptions.

**Aakash Gupta** (00:19:51)

Can you walk us through a practical demo of fine-tuning for PMs?

**Pawel Huryn** (00:19:55)

Yeah, sure. Before I demonstrate the fine-tuning, and I have an example for you, let me explain what is wrong with the current, with the popular approach. So just taking off-the-shelf model and instructing it to perform some prompts. So for example, here we can see Delphi AI, which is a common platform for building clones. And in order to get... the right results that resemble your style you need to inject a lot of instructions every time you ask a prompt so for example this is a purpose of the clone here you can see a speaking style and it is all part of the prompt so every time user connects to a chatbot all those instructions are injected and of course this causes that you need to select much more expensive model and even with more expensive more powerful models it might be challenging to adjust, and this is one of the things that is actually difficult with LLMs, to adjust LLM to your style, your unique style, like brand voice.

**Pawel Huryn** (00:21:20)

So what fine tuning allows you to do, is that you can take a smaller model like ChatGPT 4.0 Mini, and you can train it specifically on your training data. And those are the parts like user prompt and model response so that it internalizes this knowledge inside the model parameters. And as a result, you can use much smaller specialized model, And you will use much less tokens because you do not need to include all this context every time you ask a question. So I have prepared two datasets with example prompts and answers to fine-tune ChatGPT so that it can talk like Yoda from Star Wars. And if we open one of the datasets, you can see that It's just a collection of messages. So for example, user asks, can you explain gravity? And the response is something what Yoda could respond. Okay. So to use this to fine-tune a model, the easiest way is to go to platformopenai.com.

**Pawel Huryn** (00:22:46)

And here on the left, we should have a fine-tuning tab. And all we need to do is to click create. The default model is supervised and we don't want to touch it. The base model is the model that we will be adjusting. So for example, chat GPT 4.0 mini. Next, we provide training data and the training data is this data that I presented. And the second data set that I can attach is validation data. So it means that during the training, uh, OpenAI will automatically run tests on this additional dataset to see how well it can predict the answers. And what is important here is that this test data is not present in the training data. So it's like an independent audit of how our training is performing. Okay, number of epochs, so batch size, it's how many examples we will process. If I remember correctly, at once, if I remember correctly, it's just one record after another, and we do not want to touch that.

**Pawel Huryn** (00:24:13)

This setting is also something that we can leave with a default value. And number of epochs is how many times we will iterate over the training data. We will see that in the interface in a moment. So let's say we will do it three times. And after clicking create, it will start iterating on our files. I have done it several, and the process takes like 20, 30 minutes. So it's not very quick, but I have done it several hours ago. So maybe we can see how it went.

**Aakash Gupta** (00:24:53)

This is a cooking show. You put it in the oven and then it comes out ready.

<!-- sponsor -->
**Narrator** (00:24:57)

Okay,

**Pawel Huryn** (00:25:01)

so what we can see, this green line is... how well the model was able to, after training, was able to predict your answers. So training clause, this is the difference, how much generated text was similar to the expected text. And this is not comparing characters, but semantic meaning of the generated answers. Okay. So as you see, after 10 iterations, it was still pretty bad. After 40, it has became pretty good. And after the first epoch, so processing 200 records, we see that answers became almost ideal. Additional epochs were not needed. So this red point is that after each epoch, OpenAI tested the entire test dataset, so the second dataset, and calculated how well the model was trained. So after the first iteration, we check... Probably it was not needed to repeat the process, but either way it was repeated twice. So let's now take one of those fine-tuned models and we can preview it here.

**Pawel Huryn** (00:26:37)

If I copy the name, I will go to the playground probably, I hope. No? Okay, so I can just take it and go to the playground manually. Something didn't work. The model we want to interact with is this one. So it is ChargeGPT 4.0 Mini. Trying to act like Yoda. And let's say, how are you?

**Aakash Gupta** (00:27:21)

Well, it's like Yoda. Do or do not. There is no try. Clear your mind must be to see the truth. And how are you? What

**Pawel Huryn** (00:27:28)

can you tell me about product management? So, yeah, this is, of course, you will not be, you're unlikely to need Yoda in your product, AI-powered product or AI-powered features, but adjusting AI to your unique style, your brand voice, it is something that might be much more needed. And also it allows you to, it allows the model to internalize knowledge inside model weights. So rather than accessing external data sources, which is also fine in many cases, the model can learn and respond immediately without accessing any database like Rack.

**Aakash Gupta** (00:28:20)

So is an AI bot posting all your LinkedIn posts yet? Have you fine-tuned it?

**Pawel Huryn** (00:28:26)

No, I actually plan building, not for posting, but I plan combining fine-tuning with React to build a clone.

**Aakash Gupta** (00:28:33)

That's awesome. I think this is really powerful. So I've been profiling a lot of AI companies, and they almost all use fine-tuning in this way. Because of what you emphasize, number one, you get to use a much cheaper model. And number two, just read this Yoda response, right? Named must be your fear before banish it you can. Understand it you will in time. To get it to speak in a certain way, you can also do that. So you can actually increase the quality of the results by while reducing costs. So fine tuning is just one of the most important concepts out there.

**Pawel Huryn** (00:29:08)

This is probably must have forever any query, any prompt that you are executing repeatedly in your product.

<!-- sponsor -->
**Aakash Gupta** (00:29:16)

Today's episode is brought to you by Amplitude. Building great digital products is hard. You know that better than anyone. Getting teams aligned, measuring what matters, and scaling your product strategy isn't easy. But what if you had a clear framework to guide your next steps? That's exactly what Amplitude built. They studied the best product teams to understand what really drives impact and turn those insights into the digital experience maturity assessment. In two minutes you'll be able to see where your team stands and what you can improve to build better products faster. Click the link in the caption to take the free assessment and get a clear path to product growth. Because we know those expensive models, they're way too expensive if you have somebody paying you $20 a month. So you have to reduce the cost on these things, and this is how you do it. So the other concept that people talk a lot about is rag.

<!-- sponsor -->
**Aakash Gupta** (00:30:07)

Can you explain that to us and show us how that works?

**Pawel Huryn** (00:30:11)

Yeah, sure. So for that, I have... Okay, what we will build first, so I have this Google Drive folder in which I store different documents and those will be my articles. And I would like to build a chatbot that can connect to this, that can use documents that I will be storing here to answer the questions. And of course, someone can say that, yeah, but if you have 10 documents, you can just read all of them and get the entire content and inject it inside the prompt. And the first problem with that approach is that you pay for every input token. So if you have 10 documents, you include all the entire content, it will be expensive. And another reason is that In many products, you do not work with 10 documents, but with millions of documents. For example, when working with Ideas, which is a VDR solution, we've been working with millions of documents.

**Pawel Huryn** (00:31:19)

So it would be impossible to read the entire content and create a big prompt that will include all the information. So we need to use a rack. And in order to do that,

**Aakash Gupta** (00:31:35)

I'm a dummy, or I'm stimulating a dummy. So I'm still trying to understand, when do I use fine-tuning or when do I use rag?

**Pawel Huryn** (00:31:44)

Uh... Those are two different use cases and there is no contradiction between them. So you can combine fine tuning with Rack. If you want the model to, if you want that the model answers will be based on some data, then you use Rack. You can, of course, you can combine it with fine tuning, which will, to some extent, encode this data also in model weights. But if you wanted to quote documents or you have a lot of documents, a much better solution is connecting, the default solution is connecting to a RAC data source. And only later you can fine tune the model so that it also has a general knowledge about your documents.

**Aakash Gupta** (00:32:37)

Yeah.

**Pawel Huryn** (00:32:37)

Thanks for that clarification. Okay, so let's imagine this folder has 100,000 of documents. Okay, so in order to do that, we won't connect with this folder directly, but we want to use a vector database. I will create a new database, and there are many solutions. My favorite is using a pine cone. which is quite easy to use. And what happens inside Pinecon is that documents are not stored in the original form, but they are converted into multidimensional vectors and stored as chunks. I will demonstrate it. We can preview it in a moment. But first, let's create this database. There are different ways to convert a chunk of the document to a vector. different algorithms, let's say, I will use text embeddings by OpenAI, small, which is cost effective. And let's call this index or database demo product growth. And the next thing is to take documents and put them inside this vector store.

**Pawel Huryn** (00:34:08)

And for that we can use n8n. Oh, sorry. This will take a moment. Okay. So NINT, it's a solution that you can host for free on your local environment to create agentic workflows and also agents. It can use MCP servers. Yeah, but today we will focus on simple workflow. Okay. So the first step we would like to perform is that when the new document appears in this folder, we would like to take this document, download it from Google Drive and save it in our vector store. And we can do that by creating something that we call trigger. This is the way how our workflow can start. And we will be reacting to changes in a specific folder. I previously provided my Google Drive credentials. So I will not repeat that process, but you can easily find information how to do that. You need to open Google Cloud Console and create an authentication token.

**Pawel Huryn** (00:35:36)

Okay, and the folder we are going to monitor is Product Compass Demo. So let's find this folder. Okay, and we wait for file created. This will be a simplified example because in real life you also want to react on file updated or file removed so that we sync all those changes with a vector store, but I hope it's enough to understand how we can do that. Okay, and I clicked fetch test events, so it's simulated an event for this one document that we currently have in Google Drive. So every time a new document appears, we will get something like this, so basic information about the document. I will pin this data so I do not have to repeat this process, so that it's used as a mock data when working with the editor in the test environment. what we want to do next is to download this document so Google Drive once again we want to download file also using my Google credentials file by ID and on the left you can preview the data that we previously got this and one of the properties is identifier of the file okay so it can download this file.

**Pawel Huryn** (00:37:25)

I hope. Yeah, it was downloaded. This is live, folks. Yeah, this is live. So the next step, we want to split this file into small chunks and convert each chunk into a vector, multidimensional vector, that can be stored in our Pinecon here, demo product growth. So let's do that. There is a ready-to-use node, Pinecon VectorStore, and we want to add documents to VectorStore, right? Okay, and... Oh, sorry, one more thing. I think I should... No, we don't need it. Okay. Sorry. So we want to insert this document too, and also I have previously generated an API token for Pinecone, but we can see our new index. And then we need to provide a few additional information. So first, how this node can get the document, get chunks of the document, because we cannot just take the entire Google Drive file. And for that we will use default data loader, it will just take data from the previous step.

**Pawel Huryn** (00:39:13)

The type of data is not JSON, it's a binary file. We expect Word documents or PDFs, things like that. And what we want to load is not all the metadata, we don't need it, but specific data, this one, with the file content. And Also, I would like to add some metadata in case in the future we would like to search documents in a vector store by properties. So, for example, by file name, like in a traditional SQL database. And for that, we can just include... Let's see if we can find it something... File name, yeah. We have name. We have ordinary file name. Let's say name... just by dragging and dropping those elements. So it will also be stored in a PineCon store in addition to the chunk of the content. And the text splitter is about how we will split document into different chunks and we will use the default one, default policy.

**Pawel Huryn** (00:40:35)

Let's not dive too deep into this. And then the next thing is that we need to decide how we can generate those vectors. In Pinecon, we have already defined that our embedding model is this model by OpenAI, and so we need to use the same model here. I also previously generated an OpenAI API key, so NAN already knows it, and we will use text embeddings more. Okay. like this and let's see if it works I will disable this unpin the data and let's test the workflow so it gets real document data once again from from Google Drive it generates some vectors and as we can see here it's generated 18 items we can preview those items So what it generated is maybe here. It will be better. So...

<!-- sponsor -->
**Narrator** (00:42:05)

Yep.

**Pawel Huryn** (00:42:09)

So we have the basic metadata for each chunk about the document, including, I hope, including the file name that we ask it to include, and chunk of the text from this document. And this is repeated 18 times. Okay, we can now go to our pinecon, refresh it, and see if those document chunks are inside. uh okay so if we open one of them we should see that there is a chunk of the text and also metadata that we can use for additional filtering to fully test it i will now publish this workflow okay and add more documents to this folder Uh, without this, this document that is already there. I

**Aakash Gupta** (00:43:18)

like it. So we start with one document, we test out the workflow, then we add more. We don't just start with million documents. Yeah.

**Pawel Huryn** (00:43:27)

Uh, this workflow is executed more or less once every minute. So we don't necessarily, it might happen that we will not see it immediately. Okay, it is running. We can preview it. I know what I made a mistake. Okay. I will stop it. We made a mistake because we should repeat this process for every document. Okay. um okay so we want to loop over items

**Aakash Gupta** (00:44:14)

by the way guys this is how the process actually happens right you put something on paper then you iterate and improve and we're actually doing this live for you all yeah

**Pawel Huryn** (00:44:23)

okay so for every new document it will repeat the process that we already demonstrated um just to make sure i will remove everything from this database uh namespaces. I will remove the entire namespace because it already created some records. Okay, and now the database is empty. I can also remove documents from Google Drive. Save this workflow. And

<!-- sponsor -->
**Narrator** (00:44:59)

yeah. Just in case. And let's try again. All

**Aakash Gupta** (00:45:18)

right, so let's upload those documents again. Let's see.

**Pawel Huryn** (00:45:25)

It should detect that there are new documents. And let's see if we will succeed this time. It's cool how it detected it so fast. Okay. It detected only two items. So probably it will detect more items in one minute. Okay. Oh, wait. Maybe detected more.

<!-- sponsor -->
**Narrator** (00:45:59)

Okay.

**Pawel Huryn** (00:46:16)

Yeah, I think we need to wait because it detected only one file. Okay. Yeah. Now it is adding more.

**Aakash Gupta** (00:46:27)

There we go. It's working every minute.

**Pawel Huryn** (00:46:39)

Yeah, maybe it does it in batches. Anyway, it succeeded again. So let's see what is inside this index. Yeah, we have 77 records.

<!-- sponsor -->
**Narrator** (00:47:19)

For some reason I can't see it. I just needed a refresh.

**Pawel Huryn** (00:47:35)

Okay. Yeah, we have 10 documents chunks and it's detected. The first document it detected is objectives and key results, PDF. And let's see if there is any other objectives and key results. Not really.

<!-- sponsor -->
**Narrator** (00:47:59)

But it is, yeah, top five. Let's try again.

**Aakash Gupta** (00:48:14)

Looks like that's the ultimate list of product metrics. So it did find the other documents.

<!-- sponsor -->
**Narrator** (00:48:23)

Well, yeah. Okay, let's...

**Pawel Huryn** (00:48:34)

I think we have two documents. Is that enough?

<!-- sponsor -->
**Narrator** (00:48:37)

Sure.

**Pawel Huryn** (00:48:39)

Yeah. Yep. I do not want to debug it right now. No problem. For some reason, yeah, we have... Okay, so we can see that there are two documents. There are already two documents inside. One is the ultimate list of product metrics. Another one is... objectives and key results, PDF, and over time it will index more files. And I demonstrated it also in my newsletter in the past with detailed recording of indexing all the documents. So the next step is to create an endpoint for our chat that will connect to this rack. So let's try to do this. Because we now want to use those documents inside our chatbot. And in order to do that, we will create something called a webhook. This is like an inbox for your web service where different apps can ask a question and get a response. Okay, let's say other apps will call this webhook.

**Pawel Huryn** (00:50:11)

So our chatbot will call this webhook. And they will provide the question like here. So... Okay, so the question, the user query will be part of the URL. And we can see that we received that query. User message is here. So let's now retrieve documents from our vector store. So the next... The next step is getting ranked documents. As we already explained, in VectorStore, we store document chunks, not the entire documents. So we'll get different chunks from our demo. Let's say we will get 10 most similar chunks. Of course, we compare vectors, not text. And here we could ask OpenAI or another LLM to generate a specific prompt to generate a query to our vector store, like different phrases by which we will search documents. But in this case, to simplify, I will just rewrite the user query from the user message from the URL. So we will use the same query parameter.

**Pawel Huryn** (00:51:52)

And just for the demonstration, there is no authentication. I will disable this webhook after the demonstration. Okay. After we... In order to retrieve document chunks... they are represented as vectors. So we also need to represent our query as vector. And the vectors will be compared across those different dimensions. So user query from the URL becomes a vector, and then we ask Pinecon to retrieve similar vectors. The next step is to combine those responses so that we can use it, do something with them. It will be easier if we just merge them.

<!-- sponsor -->
**Narrator** (00:52:53)

Actually, aggregate will

**Pawel Huryn** (00:52:55)

be better. And what we want to aggregate is this page content, which is document chunk. What we also want to include is the file name. So if the chatbot provides an answer based on based on some document, I would like our chatbot to quote this document. So to do that, we can refer to this metadata that we previously exported to Pinecon.

<!-- sponsor -->
**Narrator** (00:53:40)

Okay.

**Pawel Huryn** (00:53:41)

Let's test. Okay. We have page content and yeah, different names combined. That's okay. And the next step is to call OpenAI. So now we want to call an LLM that will look at the user request, analyze different chunks from the database, and provide an answer. So let's say this will be an OpenAI. We want to message a model. I can also access fine-tuned models. So for example, we could ask this Jedi, but we will not see anything smart. It is not trained to perform those operations. Okay, so I will just ask chat GPT for all. And I have previously prepared a prompt that we can now reuse. So the prompt is as follows. So answer the user request only based on RAC data below. Provide the answer and at the end of your response, quote the sources. the property is not file name but actually it is name so let's rename it and yeah user request was we can take it from the webhook from the url And additional context for our chatbot will be what we have from Pinecon.

**Pawel Huryn** (00:56:12)

Okay, we have our document chunks and document names. And let's keep it simple. Let's try to test it. So the query will be OKR and the assistant replies, what is OKR? And let's see if we will quote the source. Yeah, in the sources we have a specific document name. So the last step will be changing the webhook so it doesn't reply immediately but actually waits for this logic to be executed because we want to process, we want to get chunks from VectorStore and use OpenAI and at the end We want to respond to a webhook with text, and the text will be this content provided by OpenAI. Let's activate our workflow. We can also test it, but I will take the production URL this time. Okay, and let's say that our message is North Star.

<!-- sponsor -->
**Narrator** (00:58:00)

What it is? Huh?

**Aakash Gupta** (00:58:09)

The workflow was started. Yeah. It provided some answer. Oh, nice. And this is based on your article about it. Yeah. That's awesome. The North Star metric is a critical measure that aligns a business or product's focus. For some reason,

**Pawel Huryn** (00:58:29)

it provided several quotes because North Star metric, but those are real documents names. So measuring and maximizing customer value, this is also part of of my folder and there is a PDF. As we see, it started processing more. There are already more documents processed that we initially seen. Okay, now the last step, because this was only debugging, would be going to Lovable and asking it to create a chatbot. Okay. So please create a simple chatbot

<!-- sponsor -->
**Narrator** (00:59:14)

that will call a webhook

**Pawel Huryn** (00:59:22)

like this. message. This is a user input. I hope Lovabor will understand it. Okay. Call a web hook like this to get a response. To complicate it, interpret responses as Mark Downer This is a special type of formatting. And inside the workflow, this was part of the prompt that an agent should reply with using Markdown formatting. So let's see if Lovable will do this.

**Aakash Gupta** (01:00:13)

Such a good tool. So powerful. Yeah. So to summarize so far, we used NAN for our workflows, Pinecone for our database, and Lovable for our frontend. Is that right? Yeah. Yeah.

**Pawel Huryn** (01:00:40)

lovable and previously we have used fine tuning but not in this case here we have pine cone as a vector store for storing those embeddings we also used open ai text embeddings model which was one of the choices because pine cone offers many others What is important is using the same embedding model when we ask a question because we need to compare vectors so that document chunks are represented as vectors and also the query we are asking to pinecon later needs to be encoded in the same way. Okay. Okay. Nothing unexpected. It should resolve this problem in a moment.

**Aakash Gupta** (01:01:34)

Yeah. Typical. Did it all on its own. You didn't even have to prompt it. I'm sorry? You didn't even have to click anything, right? It just fixed the error on its own.

**Pawel Huryn** (01:01:45)

Sometimes it happens.

**Aakash Gupta** (01:01:48)

No, just...

**Pawel Huryn** (01:01:49)

Just... Just fix the error. I have not even... So

**Aakash Gupta** (01:02:00)

we're clicking to fix this too. I

**Pawel Huryn** (01:02:11)

just keep clicking fix. I hope it will figure it out. It's the best sonnet on the market. The best coding model on the market. Okay. Okay. I tested it before.

**Aakash Gupta** (01:02:37)

These things are stochastic, right?

**Pawel Huryn** (01:02:40)

If it doesn't solve the problem, I will just remove this.

<!-- sponsor -->
**Narrator** (01:02:47)

Okay. Okay.

**Aakash Gupta** (01:02:59)

It's like it's rendering something. Here we go. We have a chatbot.

**Pawel Huryn** (01:03:05)

What is the star metric?

**Aakash Gupta** (01:03:09)

Let's see who does it. I

**Pawel Huryn** (01:03:14)

don't know if it will work. It worked. It worked, but this is not fully formatted as Markdown. You

<!-- sponsor -->
**Narrator** (01:03:26)

didn't format.

**Pawel Huryn** (01:03:37)

If we go to executions, we should see that there was a production request. The response was This? The response, it was... Okay. Yeah, maybe it will fix that. If not, maybe it's already enough.

**Aakash Gupta** (01:04:16)

This part's giving its intrapers.

**Pawel Huryn** (01:04:18)

Yeah, it happens more often than usual. Usually when working with Lovable, I don't have those issues, but yeah. Not at this stage. It happens with much larger projects.

**Aakash Gupta** (01:04:38)

It knows that you're recording this, so it's for air. Yeah. All right. Let's see if it's working now. Isoki. Will it be in Markdown? Let's see. Fingers crossed.

**Pawel Huryn** (01:05:01)

Okay. I think I will not fight with because it is like it is independent, I think. Yeah. Just to fix the formatting, we could probably ask it several more times, give examples, and it will figure it out. Yeah. Yeah. Okay. But we have our rack-powered chatbot. And as we can preview in executions, Here it actually gets user requests from the webhook. what is OKR. It gets document chunks from the vector store. It aggregates them. Then we use OpenAI with all this context. And based on the context, we send the response to the webhook. And the response is correctly formatted. So what could be improved here is that instead of just writing user requests, we could use, we could have an AI node here that will decide if it needs to query Rack at all. Perhaps it can provide an answer right away. And if it needs to connect to the VectorStore request, it could generate a dedicated query.

**Pawel Huryn** (01:06:43)

Right now, we just take user input and ask RAC, but perhaps user has written a very long message, and that was only one of the points. So in that case, we shouldn't rewrite the entire prompt, the entire user input, but rather focus on a specific technique, for example, that we don't know what it is, and then retrieve information about it from VectorStore. That would be more intelligent, but I hope it demonstrates how RAC can work.

**Aakash Gupta** (01:07:18)

Yes, absolutely. So let's move on to our next concept, MCP. And you have a really fascinating use case that I haven't seen anyone else talk about.

**Pawel Huryn** (01:07:26)

Yeah. So MCP is a standard for developed bioentropic for... AI agents and agentic workflows to talk to different systems. So previously when you wanted, for example, if you develop an app and you want to integrate with Stripe, you need to read the entire Stripe API documentation and understand how to call different methods. What MCP does is that for every service it provides a set of standard methods. One of them is to explain what actions are what tools this MCP server offers, and another one is a standardized way to execute those tools. So, for example, my chatbot can ask, when using Stripe's MCP server, it can ask, what actions, what tools, what do you support? And one of the responses can be, I can find a customer if you provide me customer ID, And then our chatbot can understand, will understand how to call this method, how to use this tool and what are the required parameters.

**Pawel Huryn** (01:08:59)

And to demonstrate it, I have a demo in cloud. What I would like to achieve is to connect to a Figma design. Uh, which is just a copy of a random Figma design from the Republic repository. Uh, something about task management with desktop and mobile views.

<!-- sponsor -->
**Narrator** (01:09:28)

Okay.

**Pawel Huryn** (01:09:31)

And I would like to create a set of epics and user stories in my Jira. Yeah. Save you a huge amount of time. Yeah. Based on those designs. For that, let's create a new gyra project so that we... Okay, let's just create a project. I will use a standard template for Scrum. Simplified. No need to complicate this. Okay, demo. The project key will be demo. I will just continue and use the default settings.

<!-- sponsor -->
**Narrator** (01:10:27)

Okay.

**Pawel Huryn** (01:10:34)

We don't need a confluence. By the way, the method that I will be demonstrating also allows interacting with confluence. So for example, it could create confluence pages or read confluence documentation. And if you have some standards like how user stories or how epics should be created, it can get those instructions. and it can also use user stories created in the past to to write new user stories but let's let's go to the backlog i will take this figma url and if we go to cloud by default it cannot connect to any tools we need to go to the settings so file settings And after opening the developer tab, I can click edit config. And here is a file where I can define my connections. Those standard MCP servers. We can present those keys. I will remove them after the demo. And I already configured two connections.

**Pawel Huryn** (01:11:47)

One is a connection to Figma MCP server. with my Figma ID and another one is Atlassian so Jira Confluence and other products with some standard parameters And I have recently described where you can find... Basically, it is easy to find NCP server repositories in the internet or you can Google them and what parameters you should put here. If you want to get configuration and very detailed steps on configuring the specific workflows, you can go to my newsletter and I have explained it. Okay, so I have those connections to Figma and Atlassian defined. So now I can... And Cloud, even though those are only two connections, Cloud has asked those MCP servers what are the supported tools. So we have a set of tools related to Confluence, related to Gyra, like adding comment, creating issues, and... searching in Gyra. And also there should be something related to Figma.

**Pawel Huryn** (01:13:16)

Maybe it was hidden somewhere. Yeah. there it is we can download figma images and we can get data from figma so now my prompt will be uh this is the url and i have this prompt that i have prepared previously but yeah maybe we can just write it from scratch so uh please connect to my figma project What it really needs is the Figma file ID, which is only this part, but we can put the entire URL and that's fine. Next, create a set of user epics and user stories, which in Jira are just stories based on that design. Microsoft. short stories follow the interest, which is independent, valuable, possible to estimate, short, and so on, testable. Those are good practices for user stories via loading if possible. Next, in the, and our gyra project is, I forgot, demo. Okay, I can also use the entire.

**Pawel Huryn** (01:15:05)

In a real life example, it would be better to provide some context. We already discussed it when discussing best practices for prompting. So what is the goal of this initiative? How we will measure success? Maybe some examples of user stories or user story templates from the past. We could also ask it to just analyze the existing user stories and create new user stories based on those existing ones. But just to simplify, in cloud, we need to confirm that we allow performing using every single tool I will soon, I'm currently doing a research of using NAN and MCP servers. You cannot do it in cloud, but you can do it when you host NAN for free in Docker or also you can host it in cloud like DigitalOcean. And then there are no restrictions. So it means that if you, from N8N, if you call MCP server, you don't need to confirm anything.

**Pawel Huryn** (01:16:28)

And as we can see, it started reading information, create some epics and user stories in Jira. Maybe to make it better visible, I can split the screen a little bit. And I have a special add-in which will refresh the page every... But before I do that, I will enable an epic panel and now let's refresh the page every five seconds. So as we can see, there are already some epics created. And after creating all the epics, Cloud should start creating user stories. Wow. Based on that design. And we don't need to do anything else. If we used a smaller model, this is Cloud Sonnet, 3.7 Sonnet, so... the best, but also the slowest that we can choose. Yeah, it started creating user stories. Previously, when I did this exercise, it generated about 20 user stories and six or seven epics. And it took it nine minutes with some additional seconds.

**Pawel Huryn** (01:17:59)

Got it. We can already see some user stories, like, for example, just let's stop this out to refresh. Implement site navigation menu. Yeah.

**Aakash Gupta** (01:18:15)

And it's really nice, right? It has a great description. It has acceptance criteria. This is saving you hours of work.

**Pawel Huryn** (01:18:22)

Yeah. We can ask it to add links to Figma design because, yeah, we can do many things and adjust how those user stories are generated. Links to Figma would be We only need node ID and it can access node IDs. So I can imagine that we could generate those URLs and link specific nodes from Figma dynamically or just link to the design. If it has many pages, link to the specific page. Yeah, I suppose we will

**Aakash Gupta** (01:19:00)

not be waiting. That's it for MCDE. We want to finally turn to our last topic, which is AI agents.

**Pawel Huryn** (01:19:12)

AI agents. So this is my platform built with Lovable. And why I call, some of them are just very authentic WordPress. So there is LLM inside, but the process is predictable. So it can generate PRDs, it can review product manager resume. create product strategy and so on. And the most complex one, which is really an agent, at least according to how I understand the agents, is a deep market researcher. So it can use tools like web search. It can scrape a website's content. It can also plan research steps and then delegate those research steps to other agents that will focus on specific, research areas. The goal of this agent is to perform market research for a specific company or product like Netflix movies let's say or We can do

**Aakash Gupta** (01:20:22)

something else. Do you have an idea, Akash? Let's pretend I'm Amazon Prime Video PM, and I want to analyze, you know, what new Netflix, how Netflix is thinking about its content right now.

<!-- sponsor -->
**Narrator** (01:20:38)

Oh, compare with Netflix. Yeah.

**Aakash Gupta** (01:20:54)

Something like this? Yep. We'll focus on

**Pawel Huryn** (01:20:56)

comparison with Netflix and content strategies. So the first thing it will do, it will search for some important context. So what is Amazon? What is Netflix? This is quite obvious, but maybe something has happened recently that can influence our research. And then based on this generic information, it plans up to, if I remember correctly, up to 11 separate tasks, and those tasks are distributed to different agents, which, again, search the web, scrap websites, and then all the results are combined and presented to the user. Very cool. It should take like 20, 25 seconds. It's pretty fast. Of course, it is not... I didn't try to build the second Grok or OpenAI Deep Research, but I think it is more focused on market research and it will also fuel the other agents that I created, like this PRD generator or... product to your ideation so it will also get this context about the company, about the market and use it to generate some product artifacts.

**Pawel Huryn** (01:22:20)

Yeah, deep market researchers. So first, as I explained, planning the research, like the context of about Amazon Prime and Netflix, and then detailed findings. So Amazon Prime video content strategy analysis, Amazon versus Netflix, financial and market insights, potential gaps and opportunities. There is quite a lot of elements. I'm not sure we can discuss everything, but the next one is comparative analysis. Wow. We also have value proposition. What is the difference between value proposition of those two platforms? User demographics preferences. And as you can see, there are quotes to some external websites. Wow. Location, markets, markets for key insights. Yeah, markets for share dynamics. Awesome. It's quite long and quite extensive, and it's focused on product management. There are 50 sources. You can probably get more from some platforms, but my agents focus on this product management perspective. And how it was done? It was done without any platform other than Lovable.

**Pawel Huryn** (01:23:59)

But what is important, the entire business logic is, and this is the default option that Lovable allows you to do, is to host your business logic inside Lovable. super base functions so it is not inside the browser but user interface sends a request and the request is executed on the backend and the backend has information, has secrets about different APIs, other services that are I described the logic, I didn't quote anything but described the logic of how I imagine this entire orchestration should work. And it came up with the edge function. It is called an edge function that is executed in Superbase. Wow. A different approach, probably easier one. If I did it right now, maybe I would approach it differently. You could use N8N. Just like we created a webhook when demonstrating Rack, I could create a webhook or a chat or whatever. It would be easier to test with a chat and Here we can have an AI agent.

**Pawel Huryn** (01:25:37)

There is a special note for that, which can be, for example, Sonnet, or we can use OpenAI or anything else. I will use OpenAI because OpenAI, I already have credentials saved for OpenAI. Okay. Our agent can have memory, so it can remember interactions with the user. or interactions within workflow execution. If there are loops or some iteration inside our workflow, we can use just a simple memory with session ID. So it means that as long as the session is the same session, it can access the old memories. up to five by default. But still, there are also more complex memory types that we can use. Okay, and we can give our agent some tools. In a community edition, and I will demonstrate it in a few days, so probably before this video is published, I will publish how to do that. But even without MCP, NAN offers a lot of tools that you can just connect to your agent.

**Pawel Huryn** (01:26:52)

Like, I'm not sure if Jira is here. Yeah, Jira is here. create issue. You just need to provide parameters. Similarly, you can connect to your Google Drive or do something else like Gmail. Send message and you can say that it will be defined, that the parameters will be defined by the model. So let's say two subject messages are defined by the model. And another tool I will... Calendar. Google Calendar. And... He wants to get information about events.

<!-- sponsor -->
**Narrator** (01:27:55)

Okay...

**Pawel Huryn** (01:28:02)

By the way, I did not plan demonstrating it so I'm not sure it will work. Okay, I have some fake email account that we can possibly use, but this is not my email account. And maybe let's not test it. In theory, even though this is not an MCP server, I can provide a set of tools and there are many demonstrations on YouTube how to do that. those tools can include voice generation or image generation and yeah much more complex stuff than just using two tools

**Aakash Gupta** (01:28:43)

and in

**Pawel Huryn** (01:28:43)

theory we could our agent even without MCP can access those tools so let's say send

<!-- sponsor -->
**Narrator** (01:28:57)

send an email to about

**Pawel Huryn** (01:29:30)

Just random, create an invitation for the next week in my calendar and send an email to someone. probably not idea let's say work it created some event there are also services that allow you to make voice calls so this is really cool an agent can perform a voice call for example call restaurant make a reservation and then add compare it with your calendar and then add it to your calendar And I will check in another screen if it's sent a message to refer it in a moment. Yeah. I just need to present it carefully. So this is the message that was sent from and again. I am planning to schedule a meeting next week. I don't have any events in my calendar and possibly if I look for the next week, maybe it has created something. No, it didn't create anything. It would be nice to Ah, because the only action that we added was getting information about...

**Pawel Huryn** (01:31:20)

Let's add the tool to create something in the calendar and let's save and repeat.

<!-- sponsor -->
**Narrator** (01:31:33)

Okay. requesting him

**Pawel Huryn** (01:31:47)

to attend it. Okay. It has created some event. Yay. Sending an email. Whoa. Okay.

**Aakash Gupta** (01:32:02)

This is so fast.

<!-- sponsor -->
**Narrator** (01:32:07)

Okay, let's I need to...

**Pawel Huryn** (01:32:19)

Okay, so first I have this meeting invitation sent by the agent. And also I hope October... October 9, maybe he doesn't know what is the current date.

**Aakash Gupta** (01:32:42)

In the distant future.

**Pawel Huryn** (01:32:43)

Okay. Who's creating it? We should probably add some other tools so it can...

**Aakash Gupta** (01:32:50)

That's fine. Yeah. So we got the basic idea, right? Which is this agent is going out there. It's creating calendar events. It's sending emails. And we built it all in like... Literally, you built that without any preparation in like 10 minutes. So... That was improvised. I'm

**Pawel Huryn** (01:33:08)

sorry,

**Aakash Gupta** (01:33:09)

but it didn't fully work. I did not plan this. It worked well, I think. So that's it for our live cooking session. We just walked people through a hierarchy of everything they need to know about AI product management, right? We started at the base of the pyramid. We went through prompting. We went up a level. We talked about PRDs. Then we went through fine-tuning, ragging. AI agents, we have given you the full toolkit of how to become an AI product manager. So I just want to end on some hot questions for you here. Are all PMs going to need to become AI PMs?

**Pawel Huryn** (01:33:50)

That's a hard one. I don't think so

<!-- sponsor -->
**Narrator** (01:33:54)

much.

**Pawel Huryn** (01:33:57)

there is a high probability because the market the AI market is growing so fast that there is a high probability that we will meet more AI product managers in the future the market for other product managers might not necessarily grow that fast

**Aakash Gupta** (01:34:13)

Yeah, it's not that everyone needs to become an AI PM, but this market is growing really fast, and we just gave you all the tools to become an AI product manager. Pavel, I literally think there is no one else in the world who could have done this set of demos this fast. Thank you so much.

**Pawel Huryn** (01:34:32)

Thank you, Akash. That was a pleasure.

**Aakash Gupta** (01:34:35)

So if you want to find him, make sure you check him out, his Product Compass newsletter. For my money, it is... A no-brainer. You should check out the paid newsletter. I am a subscriber to his paid newsletter. He gives out demos like this every single week. Is there anything else you want to say before we break, Pavel?

**Pawel Huryn** (01:34:55)

No, actually I started being a full-time focused on my newsletter a month ago. So just as you said, Akash, right now every week we have open hours and for example tomorrow, which is probably, probably it will not be the case because you will publish this later, but for example tomorrow we will discuss MCPs in detail. And yeah, there are slots for AI sessions every week inside our paid community.

**Aakash Gupta** (01:35:29)

He's building up an awesome community. He's already got an awesome newsletter. It's one of the top newsletters in tech on Substack. Check him out. If you haven't seen him on LinkedIn, he has over 190,000 followers on LinkedIn. Pavel Hearn, my very first guest to appear two times on the podcast. Thank you. Thank you, Akash. Take care. All right. Bye everyone. I really hope you guys enjoyed that episode. It would mean a ton to me and the team if you could please subscribe on YouTube, follow on Apple and Spotify podcasts, and leave a rating and review. Those ratings and reviews really help grow the show and help other people discover the show. And they help fund the production so that we can do bigger and better productions. Can't wait to share the next episode with you. Until then, see you later.
