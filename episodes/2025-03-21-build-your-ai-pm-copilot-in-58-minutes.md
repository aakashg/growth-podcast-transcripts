---
title: "We Built an AI Product Manager in 58 mins (Claude, ChatGPT, Loom + Notion AI)"
subtitle: "This isn’t surface-level advice like “use AI for this task.” We’re walking you through live, in-depth examples, showing exactly how to do it. So by the end, you’ll be ready to build your own AI PM"
date: "2025-03-21"
host: "Aakash Gupta"
guests: ["Tal Raviv"]
speaker_names: "substack"
substack_url: "https://www.news.aakashg.com/p/build-your-ai-pm-copilot-in-58-minutes"
youtube_url: "https://www.youtube.com/watch?v=sLI4KCjGXdQ"
duration: "00:58:46"
word_count: 9827
source: "Substack episode transcript (aired audio)"
sponsors:
  - name: "WorkOS"
    url: "http://www.workos.com/aakash"
  - name: "GibsonAI"
    url: "https://memorilabs.ai"
---

**Sponsors:** This episode is brought to you by [WorkOS](http://www.workos.com/aakash) and [GibsonAI](https://memorilabs.ai).

# We Built an AI Product Manager in 58 mins (Claude, ChatGPT, Loom + Notion AI)

*This isn’t surface-level advice like “use AI for this task.” We’re walking you through live, in-depth examples, showing exactly how to do it. So by the end, you’ll be ready to build your own AI PM*

**Aakash Gupta** (00:00:00)

Tal, you have spent more time than anyone I know figuring out how to use AI to help PMs. So where should we start?

**Tal Raviv** (00:00:09)

A really good place to start is analyzing qualitative survey results. And it's really tempting to summarize or aggregate, but it's actually really counterintuitive how you should do this. So what I'm going to do is I'm going to upload, these are real app store reviews publicly available online for, let's use AliExpress. I'm gonna upload the CSV and this by the way is into my co-pilot for Riverside. As a PM, I created a cloud project and I put a lot of context in here and I put like a custom instructions and I'm gonna let the CSV load and I am gonna ask it to analyze that CSV. I've gonna say with app store reviews, but I'm not gonna ask it for a summary I'm going to ask it for specific examples. So I want to say create a document with patterns, themes, and insights. Illustrate each points with five exact quotes and basically provide, give me a bunch of examples, but like tell me how many responses support that point.

**Tal Raviv** (00:01:17)

So because it's app store reviews, there's rating scores. And I'm also gonna ask it for outliers, right? So it's gonna like create these like really cool clusters and AI is really good at that, but then I wanna challenge it. I'm gonna wrestle with it and be like, great, what didn't you include? Okay. And I'm gonna ask it for some statistics and I'm gonna leave some wild cards here. Like just tell me anything else you see. So let's see. This is for AliExpress. And I'm going to send it. Now, the cool thing about AI interacting with data is we know that it's not great at putting all the data rows in the context window, but it's really good at writing code that can run on the data. And that's what it's doing right now. So this is how AI interacts with the world. It writes code that interacts with the world, which is really, really

**Aakash Gupta** (00:02:06)

cool. Has Claude released how big its context window is? Do we have an idea?

**Tal Raviv** (00:02:13)

Yeah, it depends on the model. I always like forget the amounts, but they're all publicly available. The gotcha here is even if the context window is a certain amount, it doesn't necessarily indicate that everything in the context window is gonna be addressed. Like has like a memory drop-off and there's some benchmarks that have come out recently showing. So if you tend to use like exactly the same word as all of the things you put in the context window, it actually has a really good recall. So you actually get more of the context window. But if you're like, conceptually referring to it with synonyms and things like that. There's actually a much smaller context. So it's really nice. Okay. This is some, some basic data statistics, right? You could do this in Excel as well, but here's where it gets really interesting. All right, so it's going to talk about complaints that people have about app performance.

**Tal Raviv** (00:03:01)

And if you ask it just to summarize, if you don't ask it for exact quotes, it's going to stop here. And you kind of have this blurry, summarized reality, like a CEO that never gets in the trenches. But because we asked it for exact quotes, you get the real words by real people. And you can check this. You can go search this back in the CSV. And this is a totally different world, right? This is so much more insights when you say restricted for suspicious activity, the search gets worse, things like popping up. So that's a way more sharper image of reality when you get exact quotes like this. You can keep going like this. And let's see. But then the cool thing is it kind of came up with its own clusters, but then we're saying, well, you know, just because it came up with like really nice clusters, it might feel really satisfying, but you got to stay really skeptical and you want to say, okay, well, what didn't you include in the clusters?

**Tal Raviv** (00:04:01)

And again, here's some more exact quotes. So this is a really great way to get the best of AI without getting all the downsides

<!-- sponsor -->
**Aakash Gupta** (00:04:09)

of This episode is brought to you by WorkOS. If you're building a SaaS app, at some point your customers will start asking for enterprise features like SAML authentication and SCIM provisioning. That's where WorkOS comes in, making it fast and painless to add enterprise features to your app. Their APIs are easy to understand so that you can ship quickly and get back to building other features. Today, hundreds of companies are already powered by WorkOS, including ones you probably know like Vercel, Webflow, and Loom. WorkOS also recently acquired Warrant, the fine-grained authorization service. Warrant's product is based on a groundbreaking authorization system called Zanzibar, which was originally designed for Google to power Google Docs and YouTube. This enables fast authorization checks at enormous scale while maintaining a flexible model that can be adapted to even the most complex use cases. If you're enjoying this podcast episode with Tal, you'll love his course on Maven, today's podcast sponsor.

<!-- sponsor -->
**Aakash Gupta** (00:05:29)

The problem with most courses online, like Udemy, is there's no live component and the instructors aren't experts in their fields, they're professors. At Maven, you get direct live access to experts and operators from the world's best tech companies. You can't get that access anywhere else, in any university, and you usually can't find them on YouTube either. I featured so many of Maven's experts in the newsletter and podcast for that reason. To help you out, I've put together a collection of courses I recommend at maven.com slash x slash Akash. This includes courses like AI prototyping for PMs, product sense for PMs, and getting an AI PM certification. Visit it now at maven.com slash x slash A-A-K-A-S-H.

**Tal Raviv** (00:06:15)

The best of AI is like, take this massive thing and help me roam and navigate and traverse it. But you don't want to go so far to lose sight of like the real words, the real frustrations, the emotions, the capital letters people are using, things like that. Really important to have that.

**Aakash Gupta** (00:06:33)

Yeah. And especially when the volume of feedback is very high, this feels like something that might have taken you even just to calculate those Excel statistics at the top. 15, 20 minutes, and then to read and summarize all these, maybe another 30, 45 minutes. We're talking about a one-hour work session that's essentially taken us two to three minutes here. Right, and then

**Tal Raviv** (00:06:55)

what you could do, right? If the alternative, let's say you're a very diligent PM and you're like, well, I read every single App Store review. Great, right? You can now use this to zoom in and say, okay, hey, can you make me a CSV with everything in this category or all the one-star reviews or everything that people are complaining about split screen? Let's say this is an initiative we have coming up and I want to include those in the kickoff. Great, you can still read every single App Store review. You don't have to give that up.

**Aakash Gupta** (00:07:26)

And in terms of the project that you placed this in, we saw the prompt. What type of context did you put in to make this project so effective?

**Tal Raviv** (00:07:36)

Yeah. So the cool thing about projects, this is, um, in Gemini, it's called gems in, in chat GPT, it's also called projects. Um, the idea is that it's a bunch of context that gets started in every thread that you have. So if you were just to use, you know, open up chat GPT one morning, uh, or cloud one morning and just start typing in a chat, it starts from zero context, maybe has a little bit of memory about you, but nothing serious. If you've created a project and you've put into that for a product manager, it might be, hey, what's the vision of the company? Who's your target customer? You can get personal and say, who's on my team? You can say, what were my last performance reviews, right? And so on and so forth. Basically, you could start with asking yourself, what would you give a new product manager that just joined your company, like what, before they even have a team, what document would you have them sit down and read, right?

**Tal Raviv** (00:08:39)

Just start with that. Like that should be, put that in the context because using LOMs without a lot of context, you've probably heard the expression, you're just gonna get the average of the internet. And so there's all this like latent power you're not getting. But the moment you give a little bit of context, right, a little more context, you are basically turning, you're like focusing all the power of the LM to this like laser through that context. And then you get way more than the average of the

**Aakash Gupta** (00:09:07)

internet. That's where it gets really powerful. So what's our next use case of AI for PMs? So

**Tal Raviv** (00:09:16)

one thing that I constantly wish I had more of my manager's time to help me with is I just need another pair of eyes on my crazy calendar to just like look at it from the side and just give me an audit. Just give me like a fresh view of it. So what I'm going to do is, again, I'm inside the project, so it has all this context on me, including things like feedback I've gotten in the past from my manager, my performance reviews, 360 reviews, things that I have told my co-pilot that I need to work on, right? Things like that. Things like, oh, you don't make enough time for just spending one on one with a designer in that phase. And I'm going to upload a bunch of screenshots of my calendar. So that they look like this without the arrows. There we go.

**Tal Raviv** (00:10:10)

So I'm just going to upload a bunch of these just like random samples. And I'm going to say, Hey, I have attached screenshots on my counter. Um, what observation insights do you notice? What, you know, what do you, what do you see here? Um, and of course it's always a really good tip when you use AI, like give me exact quotes, give me specific example, right? Illustrate what you're saying. Cause otherwise LMs tend to just kind of stay really high level, which feels good, but then backfires long-term. All right, so these are some cool vanity stats. There's like half my work week, okay. Frequent topic switching, multiple interactions in a single day, limited deep work time, oh shit, right? And you can also, if you really wanna be really rigorous here, you can tell the AI, hey, before you analyze my calendar, I want you to go Like ask me about anything that you don't know what it means.

**Tal Raviv** (00:11:11)

So some meeting titles might not be clear to people who don't have context on the company. So ask me what they are and then go ahead and do this. You can go even crazier and say, I want you to visualize it. So I'm going to go back and just change this prompt and say, here's screenshots of my calendar and go over these weeks and tell me about every single calendar event, right? Categorize each event. If it's unclear, ask me what they are and just, you know, summarize it for me. Here are some examples just to help understand Riverside and

<!-- sponsor -->
**Narrator** (00:11:50)

the context there. So let's see.

**Tal Raviv** (00:11:56)

At the end, what we're going to do is we're going to say, great. Now you like created this like raw data. You categorize everything. It's kind of like QuickBooks for my time. Um, create a pie chart, right? Tell me about trends. Then like, yeah, I can have a field day with visualizing, like, yeah, just making it like HTML, CSS, the charts, and then you can. really just have this like very visceral understanding of like, oh, holy crap, I'm spending a lot of time here and I should be spending time here, but that's like a really small slice of pie chart. You can take that to your manager and say, hey, we need to go over these stats of my time, right? Some of you have like mixed panel and amplitude for how you spend your days. So that wasn't possible before I launched.

**Aakash Gupta** (00:12:37)

I wonder if there's a way to give it like a... the description of the events and the attendees and those types of data points as well. That's a really cool idea. I bet

**Tal Raviv** (00:12:49)

with something like Zapier or similar kind of tools, you can even connect it to your Google account.

**Aakash Gupta** (00:12:54)

I haven't tried that.

**Tal Raviv** (00:12:55)

That's a really cool idea.

**Aakash Gupta** (00:12:57)

Or that's a startup idea for somebody. Or a startup idea.

**Tal Raviv** (00:13:01)

Yeah.

**Aakash Gupta** (00:13:01)

Integrate with your Google Calendar. Basically ask for your Google Calendar permission and then download more than just the title to optimize people's calendars.

**Tal Raviv** (00:13:11)

Yeah. I mean, anybody hearing this, I think anytime a workflow with AI gets a little complicated, but still very similar for everybody, you know, involved in a target market, like

<!-- sponsor -->
**Narrator** (00:13:21)

that's a startup.

**Aakash Gupta** (00:13:22)

Yeah. And everybody's always worried about building these wrappers, but I like what Aravind Srinivas said, which is like the LLM models are wrappers on top of NVIDIA. NVIDIA is a wrapper on top of TSMC. Everything is a wrapper at some point. Yeah.

**Tal Raviv** (00:13:40)

I mean, anytime I hear somebody use the term, oh, it's just a wrapper. I'm like, great. One less person that's going to compete with me. Right. Cool. You keep saying that. I mean, just think of how many SaaS products we use that could be done in Google Sheets, right? Or probably a lot of people still use Google Sheets instead of Jira. But Jira is a company. Yeah. You can think of the same Craigslist for a lot of consumer things as well. And so here's like some insights. Nice.

<!-- sponsor -->
**Narrator** (00:14:16)

And then I'll say create a pie chart. Right? So again, nothing special here, just like natural

**Tal Raviv** (00:14:23)

language, create a pie chart, um, like give me some like inference insights.

**Aakash Gupta** (00:14:30)

When do you prefer to edit the prompt versus just continue the conversation below? That's a good question.

**Tal Raviv** (00:14:37)

If you don't like the response and don't want to keep working with that, go edit the prompt, right? It's basically an opportunity to rewind and redo. If you're like, that's cool, let's use that and let's build on top of that

<!-- sponsor -->
**Narrator** (00:14:53)

and continue the chat. That's the best way to think.

**Aakash Gupta** (00:14:59)

I used to rarely edit prompts, but I think I'm going to start editing them more.

**Tal Raviv** (00:15:05)

The, I think that's the most important feature of ChatGPT, Claw, Gemini is the edit pencil icon. That is, um, that's, I think that's like all of prompt engineering, that pencil icon, because you don't really need to know the best practices or the latest like academic papers on what prompts work. You just need to be able to type something and look at the result, apply your taste, say, did they do what I wanted? If not. You know, like a person, what context was it missing? Let me go back, edit the prompt, add another sentence of context. Did it do something I didn't like, right? Then I'll go back, edit the prompt, add another sentence. Don't do this thing, right? Do that a few times. You're going to get really close to what you wanted. So here we go. A little messy. I think it's because we're really

<!-- sponsor -->
**Narrator** (00:15:52)

zoomed in for screen share, but

**Tal Raviv** (00:15:55)

this is... There we go. Here's a concern, recommendations, almost a slide, and it made interactive. So a little out of order, a little weird, but pretty impressive. This is something that I can then export as a CSV. I can say, hey, give me that data back. I can save this for my next model with my manager and go over it. And we still have the raw data. We still have the calendar screenshots as well to really understand what is it talking

**Aakash Gupta** (00:16:28)

about. All right, let's move on to our next use case. All right.

**Tal Raviv** (00:16:36)

So I want to give credit to Alan in my community for this really cool idea. I think one of the challenges as a product manager is just keeping up with new technologies, being able to intelligently hold your own, at least to know what questions to ask. You don't have to be an expert, but some of these concepts are, you know, they're popping up all the time. So for me, one thing that I really need help with is learning the concept of RAG, right? Retrieval Augmented Generation. That's like a... Something that I think is more art than science, but very technical. And so I want

**Aakash Gupta** (00:17:11)

AI... For people who don't know, why should they care about this rag?

**Tal Raviv** (00:17:16)

Oh, okay. So this is a concept that's used often in a lot of AI products and AI applications. It's when you have way more data that can fit in a context window. How do you... How do you still let the AI work? So for example, something like custom GPT is actually, this is how they work. That's where you can upload so many files to a custom GPT. Or for example, like Notion AI is another example, right? Like they don't want you to have to limit how many documents you can traverse, but they also can't fit, you know, a company's entire knowledge base into one context. So RAG is a technical concept that solves that, but Right now, I don't know what that means. I've heard that thrown around in the hallway, but I need to understand. So I figured out, okay, I know what, I know what the acronym means.

**Tal Raviv** (00:18:07)

And you can basically adapt this to your learning style. So for me, I want to teach me the concept like I am five year old and ask, ask me questions. So like interactive. Now, the cool thing is it's inside, again, the Riverside PM co-pilot. So it's gonna use Riverside when it can and like relate it to my job. So this is cool, right? It's like explaining it super simply. This is like, and it's adapting it to Riverside's vision, right? Think of this as like, you found that like perfect blog post that explains this concept just for you and your stuff, but without having to Google. So if I have to go retrieve some data without a helper, I'd have to answer from memory. With RAG, I get a special helper, kind of like an expert librarian or a paralegal. Anyway, so it's them saying, okay, well, it's not over.

**Tal Raviv** (00:19:11)

It's not just like read this as a blog post. It's asking me to engage. So why am I answering a question using only your memory, send this on the top? I might forget details. So this is actually the answer. Let's see what it has to say. Right. So I've created like a little teacher for something that's pretty complicated. But finally, you know, oftentimes engineers on your team, when you ask them to explain something, they might mean really well, but they might make you more confused. So it's really helpful to like do this ahead of time and study up.

**Aakash Gupta** (00:19:42)

All right, let's move on to our next use case. Should I run an A-B test?

**Tal Raviv** (00:19:47)

One of the biggest questions as a PM is like really high stakes for your team, but also like a really difficult thing to explain to stakeholders is why you are or are not running an A-B test for something, right? And it always sounds like really good for somebody marketing or sales or a CEO to be like, well, why don't you just run it as an A-B test? And it's never a good look to explain like, hey, rationally, logically, it's a bad decision to run this with an A-B test. Um, you can do this by the way, for any framework, you know, any decision framework you find online. It really helps sometimes to like say, Hey, I did this AI and it like gives it a little bit more rigor, just like inviting an external, you know, third party consult. Uh, so, um, A long time ago, I wrote a blog post on like, what is the decision tree for running an AB test?

**Tal Raviv** (00:20:43)

I took that blog post. I, at the time I put it into AI and I was like, Hey, can you convert this into like Markdown? Can you convert this into like a text version decision tree? Um, and then I said, great. I'm trying to decide whether a change that I want to make in the product should be run as an AP test. So, um, let's come up with a feature. Akash, what would be like a feature you'd really want to see in reverse?

**Aakash Gupta** (00:21:08)

Uh, thumbnails for podcasts on YouTube. So like automatically

**Tal Raviv** (00:21:18)

generated. Thumbnails for podcasts on YouTube?

<!-- sponsor -->
**Narrator** (00:21:22)

Yep. Cool.

**Tal Raviv** (00:21:23)

Let's throw in the term AI in there. So the rest here is, I didn't write this. I mean, I wrote the blog post, but I used AI to just like convert the blog post to a decision tree. So let's just run it. So this is like a really cool way to apply critical thinking, right? And it also really saves a lot of time in articulating a really difficult, really complex decision that can be testing. What's cool is it's, first of all, answering, asking me a few questions.

<!-- sponsor -->
**Narrator** (00:21:55)

And let's see. Okay. Do we need precise

**Tal Raviv** (00:22:03)

quantification of the change? We don't. There's, we don't. And two, there's not a lot of downside. Like, if you agree, like, even if the feature wasn't super effective, it wouldn't, it wouldn't like set you back as a creator on Riverside.

**Aakash Gupta** (00:22:24)

Yeah. I'm mainly just like a little bit of brand downside, right? Like if you generate something for somebody and they don't like it, they may just abandon the platform, especially as a new user. Yeah. Okay. So there's a downside.

**Tal Raviv** (00:22:36)

Uh, I think could make, uh,

<!-- sponsor -->
**Narrator** (00:22:40)

or

**Tal Raviv** (00:22:40)

say like bad outputs could make bad

<!-- sponsor -->
**Narrator** (00:22:44)

impression. on entire platform, maybe like wonder if other features were working.

**Tal Raviv** (00:23:05)

So on one hand, we don't need to know exactly how much money this made or it affected conversion, but we do need to make sure it's not like ruining people's

<!-- sponsor -->
**Narrator** (00:23:14)

impression on

**Tal Raviv** (00:23:14)

the product.

<!-- sponsor -->
**Narrator** (00:23:17)

I ignored the other questions. It'll be just fine. Okay. So now it's

**Tal Raviv** (00:23:26)

walking me through its thinking. I answered yes here. The secondary requirements. It's cool. It's kind of facilitating me, like, Socratically. Oftentimes if you are doing this in a thread where you've been talking about this feature for awhile, like, Hey, we, this user research, help you write a PRD, things like that. It won't ask you this many questions. And let me just try something like take a guess

<!-- sponsor -->
**Narrator** (00:23:55)

at all questions. So it's kind of doing a

**Tal Raviv** (00:24:07)

PRD. It's all PRD here. And then it'll make a recommendation, which is don't do an A-B test, but make it an opt-in feature. And you

**Aakash Gupta** (00:24:17)

can keep going, right? One

**Tal Raviv** (00:24:17)

thing you can do is like, okay, that's cool, but play devil's advocate. And I want you to argue the opposite. You can keep going with this and make it a conversation. At the end of the day, as a PM, You're kind of like observing your team debate each other and getting informed by all sides of the debate. And you can make a judgment call. But this really helps save a lot of time, a lot of like brain cells, right? Like you have a whole team discussing this really difficult topic with you.

**Aakash Gupta** (00:24:43)

Awesome. Let's move on to our next use case, reverse simulating a hard conversation. Everybody listening to this

**Tal Raviv** (00:24:50)

has had to have a conversation that they were not excited about. It could be with somebody on their team, right, about some friction or missed expectations, the stakeholder on how to better work together, what's not working. And it's really nerve-wracking. I know for me, right, it's something I try to put off, but I know it needs to happen. And, um, AI is a really good way to practice for it, but even better, right? You could use AI to simulate what it's like to talk to the other person. Um, but another thing you can do is flip it. You can have the AI be you and you, let's say the stakeholder. So, um, it's a matter of giving context. So just tell the AI. what happened the way, if you were like really stressed about it and sitting with a friend over a beer. So let's see.

**Tal Raviv** (00:25:47)

Um, I'm really nervous about having a conversation with my product marketing manager about how we're not really, um, let's see. We're really dropping the ball on rollout plans and just clarity on who's getting what feature when and what collateral is going with that and the clarity around that to the rest of the company. So I merged a bunch of hard conversations into like one. So I'm going to say, I'm really nervous about a conversation

<!-- sponsor -->
**Narrator** (00:26:29)

with a marketing partner. about how you need to better communicate the role of

**Tal Raviv** (00:26:43)

company. I've been clear in the past about the workflow, but it doesn't seem to happen. Right. And I'm leaving this ambiguous. Could be the problem is me here, but, um, and I will play I'll play Joe. Okay. So we're asking the AI to play me.

<!-- sponsor -->
**Narrator** (00:27:11)

All

**Tal Raviv** (00:27:15)

right. So this is, I'm already feeling this like empathy. This is me and I'm Joe. So I'm reading this. Hey, Joe, thanks for making the time. I know we've been juggling a lot. What's your take on how it's been going? Where do you think we're getting stuck? I'm already feeling feelings reading this. I already can like, I'm like, oh, okay, that's what it's probably like to hear this. And I'm also noticing, you know, some really good sentences that are really helping me, I guess, be more open to this kind of conversation. And it's talking about impact, right? So I'm noticing what I could be doing And if the AI doesn't do a good job, you can notice what doesn't work either. But this is like a really cool way to understand what it's like to be a person you're going to be talking with. I can say, I think it's going great.

**Tal Raviv** (00:28:05)

I'm going to be really extreme here. So you can keep going on this. You can do this for, you know, really tough. I've done this for like really tough stakeholder situations. You can do this for personal life. You can do this for product interviews. So Ben Arias, another instructor on Maven, I think also on your list, does a really cool job with this and a really specialized, really focused for FAANG interviews. And yeah, it's hard to explain the feeling you get. Even in make-believe land, you have to put the other person's hat on. But it's really, really powerful. And I don't think this was something that was possible before.

<!-- sponsor -->
**Aakash Gupta** (00:28:49)

Today's episode is brought to you by Gibson AI, the future of back-end development. Imagine designing, deploying and scaling your database as effortlessly as having a conversation. With Gibson AI, that's now a reality. Gibson AI is your AI-powered database engineer. In just minutes, you can chat with Gibson to create production-grade data models, deploy them on Gibson's cloud infrastructure and instantly generate secure REST APIs. Connect your front end directly to your Gibson built database or drop the API specs into Cursor, V0, or Bolt to build a full stack application seamlessly. From idea stage to millions of users, Gibson scales with you. Gibson optimizes your database as you grow and enables easy schema updates and migrations. So head over to gibsonai.com slash Akash. That's G-I-B-S-O-N-A-I dot com slash A-A-K-A-S-H to sign up for free and experience the future of automated data modeling. Yeah. And I also feel like it's giving us a lot of good sentences about how to deal with this.

<!-- sponsor -->
**Aakash Gupta** (00:29:58)

You know, like you can kind of simulate the worst case scenario here. They think everything's going well. And then you can see like some sentences or some crutch phrases you can use. So you're not at a loss for words when it comes time for that discussion. Exactly. You can

**Tal Raviv** (00:30:16)

create your Notion document, preparing for one-on-one and copy and paste some of these sentences you really like. And I want to point out, it's using somebody named Abbo. Abbo is a real person. He's actually the head of marketing at Riverside. Jonathan is actually the head of sales,

<!-- sponsor -->
**Narrator** (00:30:32)

right?

**Tal Raviv** (00:30:33)

How does it know that? Well, because it has context on the org chart that I gave

**Aakash Gupta** (00:30:39)

Riverside BMCo. All right. So I think this about wraps up the importance of building out a PM co-pilot with the right context in Claude and then occasionally dipping out into tools like chat GPT or perplexity to build your AM. PIMAI Copilot. Now I wanna move into broader ways that PMs can work unfairly in this unfair role that we have. And the first one, and I love this suggestion of you, and I probably only started doing it in the last two years of my 16 year career, but I saw a huge ROI too, which is demoing the idea of doing meeting next steps live. So let's say we're in a product review. And just for roles, we'll say you were the senior ICPM building, you know, this feature we've been talking about a little bit, which is YouTube thumbnails for podcast creators on Riverside. And you were the PM.

**Aakash Gupta** (00:31:40)

You just led the product review. There were some designers, some engineers. There were a couple product leaders and yourself really driving the conversation. So where do you take it from here? So one thing I

**Tal Raviv** (00:31:55)

really recommend, if you're a PM and you're in a meeting, ask yourself, how can I be screen sharing right now, right? You should be screen sharing. It could be the description of a Jira ticket. It can be the update you're going to write. Whatever the follow-up test that's probably going to fall on you, start screen sharing that in that software during the meeting. Now, that sounds... sounds counterintuitive because your stakeholders might feel fear that your stakeholders might feel that you know you are you know you're not doing your job or that you're wasting their time you should be doing this on your own time it's actually the opposite and it's actually a really good way of playing back in real time what's going on it's a really good way of Showing that you are really diligent about action items and making sure that they're on paper, right?

**Tal Raviv** (00:32:48)

It gives everybody this peace of mind to see. You don't have to finish the artifact in the meeting. You can get 80% of the way there. So, Akash, let's say we just had a sync on a project that we're really trying to show. and you and i are on a team together and we just had a meeting or we we're just um having a meeting right now um on what is like the status of this project okay so uh we're just going to pretend for this that we have some of your recent podcast guests also in this meeting and let's see this is the last time that we had this meeting Um, I took that from Slack channel and I've pasted it back into, uh, the Slack message, and now we're gonna update it. So already it's like an automatic agenda. And Akash, as the engineering manager, you know, we really, really just wanna get it out to like a really small group.

**Tal Raviv** (00:33:51)

We don't have to finish everything, right? We always said like the first release will be the like product partners, like WhatsApp group, the design partners. So Akash, like for the simulation, give me like the worst news possible. uh about that bad bug where the recordings are disappearing

**Aakash Gupta** (00:34:09)

yeah it turns out a lot of people are running into this issue where they do a 90 minute 120 minute recording and there's some sort of stuttering or something and we're not telling them about it and so when they go check the recording afterwards there's a stuttering and they can't use the episode

**Tal Raviv** (00:34:27)

okay so actually the recordings are not disappearing And I'm stuttering. And, you know, with your engineering hat on, where does this stand?

**Aakash Gupta** (00:34:41)

Any progress

**Tal Raviv** (00:34:42)

there?

**Aakash Gupta** (00:34:43)

It's going to be almost impossible for us as Riverside to do anything because it has to do with the guest's camera, actually, their hardware. And so probably if we were to build something, we would build like sort of a frame rate, live frame rate screen, for instance, for the host, for them to understand how many... frames are getting or alternatively, we could simplify that a little bit and give them a little less control and say, okay, if you've selected 24 frames and you're not getting 24 frames, let's put up a red warning light immediately or let's put up some sort of indicator or we have like a built in pop up that we use for error messages already. For instance, when we don't have browser screen sharing permission, so we could just reuse that modal and put up like your guest video may have stuttering issues.

**Aakash Gupta** (00:35:32)

Awesome.

**Tal Raviv** (00:35:33)

And I think, like you said, most of what you mentioned is not a risk or like a thing we're wondering about, except one part, uh, which is like the frame rate detector. So we don't know if that's technically something we can do reliably. So it looks like the next step here would be, um, like just a proof of concept, right. Of the frame rate detector. Uh, we don't even need to do the warning. So that's like the next step. I'll just show you this. And Akash, as the most experienced technical member of the team, I'll say that this is something that you will lead just because it's so high stakes right now

<!-- sponsor -->
**Narrator** (00:36:13)

and

**Tal Raviv** (00:36:13)

goes so deep into

<!-- sponsor -->
**Narrator** (00:36:15)

the code. Okay. All right.

**Tal Raviv** (00:36:21)

And, uh, we can, we can keep going. We'll go like, you know, line by line. Um, the idea is like that we are both, um, like we're having the meeting recording the notes of the meeting and we're creating the summary. That'll go back out for people who, you know, are very in tune to this project, but you know, aren't, it doesn't make sense for them to be in the meeting. Um, So yeah, Akash, what was this like for you as you were talking and you were watching me type?

**Aakash Gupta** (00:36:53)

It was good. I feel like the only risk potentially is if you record kind of the whole 30-minute meeting. I might feel like you're almost like having this meeting to share with others versus having this meeting to productively move forward with me. So should people be doing this the whole meeting or just at the end? That's a really good point.

**Tal Raviv** (00:37:16)

It could be at the end of each idea, right? Like say, okay, cool. We just had a really good discussion on what the next step is. Let me just like write a few notes down. I'll polish it later.

**Aakash Gupta** (00:37:26)

Yeah, makes sense.

**Tal Raviv** (00:37:30)

The key is to ask yourself, How do I have people feel heard and that like what they said is recorded? But with that, the other feeling that you gave, right, which is like, hey, are you paying attention? Why is there so much typing noise? Right. All that stuff. You want to find that really good balance.

**Aakash Gupta** (00:37:52)

Yep. So let's move into our next sort of hack here, which is. Doing Looms, I want to understand, you know, as a PM, when should I actually be recording the Loom? What are some real use cases? And then let's go ahead and see what that looks like.

**Tal Raviv** (00:38:08)

Or let's say there's like a discussion in Slack and somebody's like, well, this is like really complicated. Let's do a meeting. So even in that situation, right, where you're like, oh, geez, another 30 minute meeting. Like, I wish we could have like figured this out in the thread. Even in that situation, most of that meeting, most PM meetings are the product manager for most of the time giving context to the people in the meeting. Right. And then that might be enough. And it might be like, oh, I get it now. Or there might be like five, 10 minutes of back and forth discussion. But most of that is kind of one way, explaining kind of what's been going on or what's new, what needs to be known. And for that part, a loom is really, really ideal. And then at best, you can avoid that meeting entirely.

**Tal Raviv** (00:39:05)

And even at worst, you can cut down that meeting. All right. So let's say that I'm a growth product manager at Riverside. And I found that there's a really strong hypothesis that if we give people a lot more clarity on what plan they're currently on at the marketing page level, that we're going to be able to drive a lot more upgrades. But right now, it's not reflecting that because it's like a different technical stack. So um i you know in slack and discussions were like oh my god we really need to meet with the marketing developer team about this i have some of my engineers some of their engineers and we'll figure out how to like make them all work together but so much of that meeting uh is one way and i can totally uh just like give that context now i already sat with my engineers i know you know what the intro is so i'm gonna uh open loom and I guess just cause we're recording a podcast and just maybe not, not mess with the camera, but like I can have myself in the corner, which makes it like very human and very personal.

**Tal Raviv** (00:40:14)

Um, and I'll start recording. I'm not going to do now just cause we're using Riverside and I'm going to aim for less than a minute. I'm not going to do five minutes, not nine minutes. Aim for less than a minute. And I might hit like two minutes, right? Because I like stutter around and I wasn't sure what I was going to say. So I'll throw that recording out and I'll do it again and try to hit one minute. All that time that I would invest is still going to be less than the amount of time it would take me to do that in the meeting. So let's say I hit start recording in Loom, right? And I'm going to watch the clock here. Hey, marketing team. So in preparation for our meeting, what I wanna do is kind of give you the high level of the flow of how the marketing page continues into the product.

**Tal Raviv** (00:41:00)

And I wanna show you some of the technical details behind the scenes. So you can start thinking about this and let this marinate ahead. So if I click buy now on the pro plan from the marketing site, You'll notice that there's like a plan ID here at the top. And that's only like part of the picture. There's actually a bunch of parameters that get passed as cookies that we didn't want to show in the URL and so on and so forth. And I would watch the clock. I'd be like, OK, that was like long winded. If it's like two minutes, right, people aren't going to. they're going to see, like, oh, this is two minutes. They're going to put it on their to-do list. But if it's like 54 seconds, right, way more people in the meeting are going to hit play. And you can have a much shorter meeting instead of having to explain all the stuff and get right to the good stuff of the brainstorming.

**Aakash Gupta** (00:41:46)

Yeah, I think that's the key, making it less than a minute, because then in sort of the getting things done mentality, you just get it done now instead of putting it on a list. Yeah. All right. So the next technique you've talked about, which I think is really powerful, is to hide, ignore, or automate Slack. So how do people do that? So

**Tal Raviv** (00:42:09)

I'm going to use Lenny Slack just because it's like especially overwhelming. But I think anybody watching this can like really relate to opening up Slack and just having that like mini art attack, right? All these like unreads. So here's a few things that can really make that overwhelm a lot more manageable. The first thing everybody should do, I wish this was default in Slack, is go to settings, click on home and show unreads only. So every time that you go into a channel and you've read it, it won't be in the sidebar anymore. It's like, it's just like cognitively a lot easier to deal with. So

**Aakash Gupta** (00:42:43)

here's an

**Tal Raviv** (00:42:43)

example, right? Let's say I went to the general channel, I read everything and I go to talk AI, the general channel disappears, right? It's like crossing things all. But the other thing that you can do is create more sections. So I like to create sections in order of what's really important to me when I get into, if I get overwhelmed and I'm not functioning, right? I don't want to just be like, whack-a-moling these channels. I need to get to like the most important stuff. So I'm going to create a section called critical initiatives. All right. And I'm going to put a few of the initiatives that I'm working on in that section. And then I'm going to create another section called, you know, once I, once I've looked at all the critical initiatives, maybe I'll say, customer feedback. So like all the channels that are like feedback rivers and I'll put some things there and then maybe I'll create a section called, you know, relevant other, you know, related teams or related initiatives.

**Tal Raviv** (00:43:52)

Right. And maybe I'll create another section that like, let's say I, I ate all my vegetables. I went through all the things that are really important for me as a PM to look at. I'll create one called dopamine. So that could be like the random channel or, you know, the, uh, workout channel or, you know, whatever the food channel. Um, and I'll collapse all of these. Right. Already. It's a little bit more manageable. But I'm actually going to order these in order of how I want to go through it. So when I first log into Slack, I want to look at the top and I want to look at critical initiative. And then I want to look at customer feedback, right? And something like that. So this becomes, this becomes a lot more manageable.

**Aakash Gupta** (00:44:34)

If you

**Tal Raviv** (00:44:35)

remember what Slack looked like when we entered it versus now, it's not just that it's more collapsed and more easy to like see the big picture. It's also, I know exactly, You know, my brain, I'm just overwhelmed. I can't think. I have a step-by-step guide in my sidebar of how to navigate this monster.

**Aakash Gupta** (00:44:57)

Amazing. And how did you manage to automate it or ignore it? Yeah. So

**Tal Raviv** (00:45:05)

another underrated feature of Slack is called Slack Reminders. And when Slack Reminders first came out, I was like, why is Slack doing this feature? Like, is it trying to be, you know, Asana or something? And very quickly I realized like the genius of how this like really simple feature helps me as a PM. So I'm gonna look at maybe a thread. We all know what it's like to have a thread that maybe you write a message and then nobody responds, right? But you forgot about it and you're like, oh my God. everybody was too busy and now I don't have my answer and I have a deadline. Or the opposite, where somebody promises that they're going to do something, right? And then they never follow up. And so as PMs, right, we want to be perceived and actually be the people who are most on top of things, like this airtight aura of us.

**Tal Raviv** (00:46:02)

And so one thing you can do is say, here, this is a great message where we're trying to plan a meetup here in Israel. And I'll right click on this and I'll say, hey, remind me about this. So guy said, oh, I didn't get to it. Okay, cool. So let me, what's like a reasonable time for guy to get to this? Let me ping him in a week. Right. And I'll hit save on this reminder. So, um, this is like my peace of mind for getting ghosted, which is inevitable as PM or for people, you know, not following up or not answering me.

**Aakash Gupta** (00:46:38)

All right. And did you do anything to manage the notifications or how do you make sure that you actually get some time for deep work?

**Tal Raviv** (00:46:49)

So the way to get deep work in Slack is actually zooming out of Slack and only opening this window when you, um, after you've done your deep work. So that's what works for me. Everybody else has like a different schedule, but it's mainly about the idea of like completely separating it out. For me personally and my brain, I know that the moment I go into Slack, it's over for my brain. I'm in like ping pong mode and there's no way that I'm going to sit down and do something that like requires my brain to do hard work. So what I do is I do all that hard work before I ever go into Slack. And it might sound... like uncomfortable, right? Like to not be available during a certain amount of time. Or it might sound like, well, am I being a bad PM by not being there in case something happens?

**Tal Raviv** (00:47:46)

So I've been doing this for almost a decade and I can count on one hand, the number of times that there's actually been a time sensitive emergency where somebody was blocked or, you know, somebody needed me that moment. And in those moments, The problem was still solved because I gave people my actual phone number. And so people knew that I was available. There's just a little bit more of a barrier. So if it was actually important, nobody would hesitate to call it. But if it was like, hey, you know what? He's not answering, but we're not actually blocked on this. People aren't going to call my phone. This works for remote companies and in-office companies. For example, in office companies, right? I'll just be in a different room or I'll be around the corner in a coffee shop if we really need to focus. So it's all about how do you arrange and design your day before you even go to Slack.

**Aakash Gupta** (00:48:42)

Yes. And I think that as you get really senior in those director and VP levels, there is kind of this expectation that you're available within five minutes. But I love your point here about the status. That's what I did when I was last VP is I would put a status in there, deep work, dash call my number if you need me. And so then people kind of felt that security that, okay, he still is available. He's telling me he's doing deep work. And I noticed some people are pretty bad about turning off their statuses. I tried to be pretty good about only using that deep work status in a kind of predictable manner, usually two to three hours early in the day so that people knew that they could find me and they could also see when I was available versus not.

**Tal Raviv** (00:49:26)

Yeah, that's a great example. And I think over time, especially as a leader, right, you're actually setting an example for how you want other people. Everybody should be doing deep work, right? And ideally, if you're, let's say, a PM on a team, other people, everybody's craving deep work. So they're like, wait, I see that Akash is doing deep work every day from 9 a.m. to 11 a.m. That's my opportunity to do deep work, right? He's not going to be pinging me. And I've been on teams where everybody kind of adopted it because they're like, oh, finally, we have a break.

**Aakash Gupta** (00:50:02)

Yeah, it's so huge. So the last sort of way to work unfairly that I think you have written about that others haven't is this idea of getting a head start on discovery with product scrapbooking. So how do people do that?

**Tal Raviv** (00:50:15)

Right. One of the most valuable things that we can do is customer discovery. And yet when an initiative, right, like decided on, that's like the thing we have the least amount of time. Everybody wants us to do it, but they want us to like, okay, let's kick it off as soon as possible. Or let's have. You know, let's just start like speccing it out or brainstorming or testing ideas, but like, wait, what about time to interview some users or, but that takes some lead up time, right? Or go through support tickets or all the things we want to do. Um, one way to really get a headstart is not to wait for that moment. Um, not to wait for the moment that like an initiative is chosen, but actually to be scrapbooking kind of continuously all the time. So as PMs, we're constantly being barraged by, you know, a non-linear messy way by feedback.

**Tal Raviv** (00:51:04)

And if you don't have a place to put it, A, we're just kind of looking at it. We're like, hey, that's a cool idea. But like that's not on today's roadmap or this quarter's roadmap, like kind of slips your mind. So what I started to do I call it a scrapbooking, which means I use notion because like really convenient, but there's so many, you know, great soft piece of software that could do this at Google docs or, um, you know, any kind of project management, anything where you create these like distinct documents. Um, and I. start to notice that there's like a theme. Hey, you know, YouTubers really want AI thumbnails in Riverside. And every time that I hear somebody mention that, it could be in a support ticket, could be on Reddit, it could be in our Facebook community. it could be um hey maybe there's like some quantitative pattern where i notice people like they're always clicking on something and then they're uh clearly like like in full story right or hot jar i see that they're like mistaking a button right and endless things like that um for riverside uh one of the um projects that i was like really monitoring is you know a lot of creators have a lot of pro tips that they're sending their guests we should really build those in sorry We should really build those in to the product.

**Tal Raviv** (00:52:25)

But like, what would that be? That takes a lot of like lead time, right? So every time that I did a user interview, I like made sure to ask that creator,

<!-- sponsor -->
**Narrator** (00:52:33)

hey,

**Tal Raviv** (00:52:33)

you know, what are the instructions that you send in advance? Can you send that to me? And they send that to guests anyways, and they're really happy to do that. So I started to, you know, really save all these PDFs and Google Docs. And I saved, you know, what are some hacks people do? And, you know, you know, what is the enterprise team recommending and what are some things that, you know, the data team already found in like some of their unrelated research, um, And so on and so forth could be user research interviews. So when the time finally came and this did get prioritized, I was able to make a case for leadership. First of all, it was way easier to make that case, right? It's really hard to make a case for discovery without the discovery. And I was already off to the races and I could already do a kickoff like quite soon, right?

**Tal Raviv** (00:53:19)

Because I had these like really vivid examples for design and engineering and I could start to parallelize. I could keep doing discovery, but they already had like a lot of really good context to work with. And all that was done with very minimal effort. Just like take a screenshot, paste it into Notion. Take a link, paste it into Notion, right? Take a gong call, take a loom, whatever it is. And these things really build up over time.

**Aakash Gupta** (00:53:45)

Yeah, what I found is that building a second brain like this, whether it's Notion or Apple Notes or anything like that, the real power is when you start to use the search bar, right? Because you start to find some crazy connections also between these notes. You might have taken some notes on some other product scrapbook about another feature. of, oh, this is this really important problem that this segment of creators has. There's a segment of creators, you know, on Riverside that I think really obsessed with like 4K recordings. Maybe like those people, they're really having trouble like getting guests to use the smartphone. Then when you're working on this, all of a sudden you can search and find, okay, here's the specific learning I've gotten about this specific segment. So it's almost about creating this knowledge repository of discovery facts that you can then go ahead and use later on.

**Tal Raviv** (00:54:34)

Yeah, and it doesn't have to clean. The idea is actually let it be messy. It's really easier to like sort it out and group it and like you said, segment right around the right problem later on. So you don't have to like know in advance which specific problems you're going to be solving. You can just cluster however you feel like and figure it out later. Like you said, with the search feature, especially Notion AI is incredible for like next level search around Notion.

**Aakash Gupta** (00:55:00)

Are there any things people should know about using Notion AI search? Um, I think

**Tal Raviv** (00:55:07)

it's still, it's still an early feature. So sometimes it like blows my mind and sometimes I'm like, how did you, you know, not see that? I don't think it searches images very well. Um, but you can ask it something like, Hey, what was that document where I talk about X, Y, Z, you know? Um, and if you were using notion search, like the classic, you'd have to get the exact keywords. Right. Right. For it to, you have to kind of like do a lot of mental work and like, what did I call it at the time? But if you don't know, and you're like, I know there's a lot of things across the knowledge base around this, but everybody called this different. You can use natural language and it'll use an LLM. That's like what we were talking about earlier, actually. It uses retrieval augmented generation.

<!-- sponsor -->
**Narrator** (00:55:48)

And

**Tal Raviv** (00:55:49)

it can take search to like a next level.

**Aakash Gupta** (00:55:54)

Awesome. So that's it for our demos and screen shares. Hopefully that gives you guys a lot of ways to work unfairly in this unfair role that we all find ourselves in. What are you up to now? You were early PM at Patreon, Wix, I believe, DuckDuckGo, Riverside, all these amazing companies. What are you up to now and what's next for you?

**Tal Raviv** (00:56:20)

So, uh, I teach a course on Maven days called build your productivity, build your personal PM productivity system and AI co-pilot. And I've actually started this full time now and I'm giving it a shot. I'm like, what does it feel like to do this full time? And, um, Yeah, how do I stay sharp without, you know, still being a PM and figuring out all sorts of questions. What is this new incarnation of my career as a creator?

**Aakash Gupta** (00:56:51)

Amazing. And you guys can, he is part of my Maven creation, so you can use Akash X Maven for $100 off that course. When is the next cohort?

**Tal Raviv** (00:57:00)

The next cohort is in mid-May. It's coming up in two months.

**Aakash Gupta** (00:57:06)

All right. And do a lot of people get that expensed with their learning and development budget?

**Tal Raviv** (00:57:12)

Yeah. A lot of PMs, what they'll be able to do is share with the manager. And Maven has excellent templates that saves you a lot of time that have been proven. And tons of Maven students have used this to get it reimbursed if you have a professional development budget or even if you don't. This is like a really high ROI expense for you.

**Aakash Gupta** (00:57:31)

All right. And outside of Maven, what are you up to? Where can people find you online?

**Tal Raviv** (00:57:37)

I post on LinkedIn and Twitter and things I mainly post, I realized that like best thing I can do day-to-day in my like new incarnation of the full-time creator is I just do like a lot of experiments with AI with my PM head on. And because I realized like most PMs just don't have the time for that and I share the results. So if something goes well, I share it. If something goes not well, I find people enjoy that or find that more valuable. So I just kind of a guinea pig for product managers out there.

**Aakash Gupta** (00:58:08)

All right. So if you want to be trying the AI tools but haven't been able to, definitely check out his content online. Tal, thank you so much for being here. Gosh, thank you. See you in the next episode.
