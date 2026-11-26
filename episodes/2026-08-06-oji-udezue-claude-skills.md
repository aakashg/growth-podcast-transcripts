---
title: "3x CPO Oji Udezue on the Essential Claude Skills for PMs"
subtitle: "Former CPO of Typeform, Parsable, and Calendly teaches how to build immaculate product judgment as skills. "
date: "2026-08-06"
host: "Aakash Gupta"
guests: ["Guest"]
speaker_names: "inferred"
substack_url: "https://www.news.aakashg.com/p/oji-udezue-claude-skills"
youtube_url: "https://www.youtube.com/watch?v=Eo26_4JcyNA"
duration: "01:04:41"
word_count: 9776
source: "Substack episode transcript (aired audio)"
sponsors:
  - name: "Bolt"
    url: "https://bolt.new/solutions/product-manager?utm_source=Promoted&utm_medium=email&utm_campaign=aakash-product-growth"
  - name: "Customer.io"
    url: "http://customer.io/productgrowth"
  - name: "Ariso"
    url: "https://ariso.ai/aakash"
---

**Sponsors:** This episode is brought to you by [Bolt](https://bolt.new/solutions/product-manager?utm_source=Promoted&utm_medium=email&utm_campaign=aakash-product-growth), [Customer.io](http://customer.io/productgrowth) and [Ariso](https://ariso.ai/aakash).

# 3x CPO Oji Udezue on the Essential Claude Skills for PMs

*Former CPO of Typeform, Parsable, and Calendly teaches how to build immaculate product judgment as skills. *

**Guest** (00:00:00)

The era of mono skilled professionals is dead. So I'm going to demonstrate the future of product builders.

**Aakash Gupta** (00:00:07)

Meet Aji Udezwe, former CPO at Typeform, Calendly, and Parsible, as well as former head of product of creation and innovation at Twitter. How much of this thinking like viability gates and sure problem tests should we really be outsourcing to LLMs? Is LLM basically the first draft just to get some thinking going and then we improve and react?

**Guest** (00:00:28)

You really do need to look through all the output and make sure that it makes sense for you. We do this all the time because, you know, I think it's hard to fully trust 100% LLMs.

**Aakash Gupta** (00:00:37)

Can you open up that scaffolding skill and we can see what is inside it and how it looks?

**Guest** (00:00:42)

Yes. So it's, it is multi skills here. You can see that it has a master skill that MD, and then it has a bunch of sub skills where it would do market research. I've been a product manager for 25 years and I've never really felt that coding was worth my time until now.

<!-- sponsor -->
**Aakash Gupta** (00:01:03)

Before we get into today's show, please take a second to check that you're subscribed on YouTube and following on Apple and Spotify podcasts. If you want access to all of my favorite AI tools, I've gotten them to give you an entire year of their paid plans. Check out bundle.akashg.com for an entire year of Bolt.new, Airtable, Speechify, Descript, Magic Patterns, Linear, Dovetail, Arise, and Mobbin. And now into today's show. OG, what are people going to learn today if they stay till the end?

**Guest** (00:01:36)

Well, people are going to learn, the most important thing they're going to learn is that we won't just focus on code skills. The landscape of product right now or coding or engineering or the shipyard, whatever you want to call it, is full of repos in GitHub with skills to token max or token minimize or to change costs, all in the coding layer. But we know that A tech company, a successful tech company is really three layers. It's the software and the hardware. It's the product, which is about customers and about the business model. And it's about the business. They're thinking about allocating resources to the rest of the chain. What you're going to learn is how to take the raw harness, like Cloud Code, And apply not only coding skills, but product skills, product judgment on tap and business skills that will help you make the very best decisions about how to build a successful product.

**Aakash Gupta** (00:02:38)

So I'm really excited about this. Where should we start?

**Guest** (00:02:43)

So Aakash, where I want to start is something I think is really important. So we see, Product Mind consults with lots of big companies, big and small. The things that we get asked to do is, first of all, come in and reconceptualize a product as much more AI native. Well, very quickly what happens to us is that we get pulled into the shipyard, like how people are organized, new skills for people in an AI era, how do things work together, how do people work together. And what we're seeing immediately is the developers are speeding up very quickly, surely if they're early adopters, and then we see everyone else being a bottleneck. And particularly we see PMs who are not speeding up their product judgment, speeding up their orchestration skills to match the new speed of the engineers. So what I'm about to show you is we made a set of product judgment skills, not just code skills, but product judgment and business skills that product managers can use to Think at the business layer, at the product layer, while not sacrificing code fidelity and things like testing and quality and so on.

**Guest** (00:03:57)

The best instantiation of this is the new project scaffolding skill. There are all kinds of skills here. We have things like finding the aha moment for your new product, whether it's agentic or not. We have things like figuring out whether it's a sharp problem. But the scaffolding skill is special because it starts with you describing a business problem. And then it really makes decisions, helps you make decisions, whether it does market research for you, tells you whether it's a viable problem and how to solve it if it's not a viable problem, makes architectural decisions for you based on asking you questions, figures out how to test the thing based on those architectural decisions, and even sets up continuous integration and continuous delivery for you. So we're going to work directly in Cloud Code, not in Cloud Desktop or anything, just in the same So what I'm going to tell this thing right now is to scaffold a new project.

**Guest** (00:04:52)

One of the things I'm obsessed about is the fact that people won't read any code. So what I want to build is either a SaaS or an agent that helps vibe coders, people who don't have a lot of software experience, helps them Figure out if their code is any good. Security, robustness, complexity, simplicity, all of that tells them the story of their code because no one is looking at it, even in a corporate environment. And so hopefully if we tell it to scaffold this, it'll run all the processes of the scaffolding for us. I'm going to hit enter. If you pause and read it, you'll see that it's just a first idea. And so what this is going to do It will run a viability gate. It will take a look at some frameworks and try to figure out if this project is even viable at all.

**Guest** (00:05:41)

And so that first gate is still sort of loading the skill. There you go. It's an 11-step workflow. That makes sense because it's a very powerful skill. And it'll skip straight to the viability gate.

**Aakash Gupta** (00:05:59)

Let's see. Can you open up that scaffolding skill and we can see what is inside it and how it looks?

**Guest** (00:06:05)

Oh yeah, let's do that. So if you look at the skills, you'll see a bunch of the product skills, sharp problem. So the first one is, yeah, so it's multi-skills here. You can see that it has a master skill.md. And then it has a bunch of sub-skills where it will do market research. It will actually fetch skills for you, new skills for you if you need it for your project type. It will set up testing, and the core skill is basically the viability gate. So let's go back to see what it's doing here. And so what it's trying to do is to do web search. So I'm going to tell it that it can absolutely do web search in order to find out what's going on. So it's conducting market research. So I think I interrupted it, so I'm going to continue. And it's going to conduct market research on the idea.

**Guest** (00:07:13)

And the next thing it's going to do is to write a product brief. And once it's done with the product brief, it will start to get to the code level at all. Claude takes his time a little bit, but what it's doing is that it's spitting up a website session. Sometimes it will do that through Chrome. If you have Chrome tools installed, sometimes it will do that itself with HTTP. And of course, I didn't give Claude all my permission, so it's there. So yeah, so the viability gate, this is going to be interesting. It's going to tell me whether this thing is worth my time or worth your time very specifically. And you have to understand that what it's really doing is taking frameworks from product management from our book and it's trying to see Is this thing worth spending time on? Some of the dimensions include things like the frequency of the problem, whether we have a clear customer.

**Guest** (00:08:29)

And there we go. Let's run that. So what does it tell us, actually, with the Viability Gate? Viability gate passed, proceed. Zero weak, three strong, three moderate. Not a silent pass, three moderates are flagged as de-risk and agenda. Now step four, market research. And if we go into the repo, we will start to see this document show up. So if we go away from skills and go to code memo one, it'll start to actually write for us what it's finding out from doing a web search. So right now we know that usually if there are three weak things, it will kill it. It will recommend you stopping. But according to it, the viability gate is strong. So it has like six dimensions, revenue, technical feasibility, differentiation, competitive landscape, target user definition, and the problem clarity and urgency. So if we go back to its... It's work.

**Guest** (00:09:45)

It's literally going in and doing deeper market research for you now. It's scanning competitors, it's scanning pricing, it's scanning what people have done in the space. And so right here, it's created it. It's done your market research package for you. I set it so that it's not narrating itself in full. What you can see has a market overview. It has trends shaping the space. It has direct or near competitors and what they're charging for. It has key takeaways. It has adjacent products. This is really, really comprehensive guys about what it's doing for you. And now it's writing a product brief. We have tools that help you write a PRD. This is literally your new project brief where it codifies that into a problem, into target customers, core value proposition, success criteria that will help you know whether you succeed or fail, and then starts to write goals for you that will help you sort of gauge where it's going.

**Guest** (00:11:04)

Okay, now it's done that. It's done some of the business level skills. And what it's working on now is trying to find out how to scaffold the rest of the project in code for you. So now to the code layer, you can see that. CodeMemo's core is an LLM Analyze and Repos are wired for clog with correct current model IDs.

**Aakash Gupta** (00:11:30)

So the scaffolding skill is basically an orchestrator skill. It seems like it's calling some of these other skills, creating documents, walking through this 11-step process.

**Guest** (00:11:39)

Yes. So if you look at these skills here, they're all really dense. They have built-in product frameworks that Some of them we've written from our book Building Rocketships. Some of them are well-known product frameworks that we've included in part of this. Building Rocketships is actually pretty comprehensive and it's a very good resource. But what it does is it combines some of these things. The most important one it combines actually is the sharp problem test. So it's doing an internal sharp problem test and it's orchestrating a few more skills within that in terms of new product scaffolding. Well, the thing that's special about this one is that by the time it's done, you will have a full repo. So you can see that it's created a prototypes folder. It's created your package of thinking. It's also created your first milestone folder for you to get started. By the time it's done, architecture is settled.

**Guest** (00:12:45)

Continuous integration is settled. And if you give it its GitHub repo, it can start the project and make the first push into GitHub for you. Why is this important? When you are a PM and when you are a vibe coder, The things that are difficult for you are all the things. It's doing the right kind of market research, figuring out if this is the right thing to work on. But then immediately the way you hand off to developers is also a problem. It's like, what's the architecture? I've seen a lot of via coders who don't have continuous integration. They don't know how to test the code because They don't know how to do that. So this sets it all for you so that you have the bones of a really solid product and a really solid code base to start to work on. I think that's the power of the scaffolding.

<!-- sponsor -->
**Aakash Gupta** (00:13:43)

Here's a quick word from our sponsors. Here's what I did last week that changed how I think about AI coding tools. I built a full internal dashboard in Bolt at noon. Took me about two hours. Looked good, worked well, had all the functionality the team needed. Then I did something you can't do I sent the actual source code to my engineer. In Base44, in Lovable, in most of the tools, the code lives inside the platform. Your engineer can't pull it. They look at your prototype, say cool, and rebuild the whole thing from scratch. Boltat knew is different. The code is pullable. Real, production-grade, front-end code. My engineer opened it, reviewed it, and started building on top of what I'd already made. No rebuild, no start from scratch. The prototype became the product. I use Bolt.new every single day. I built my entire paid cohort platform on it.

<!-- sponsor -->
**Aakash Gupta** (00:14:30)

75 product managers log into something I made in Bolt.new. Try it yourself, Bolt.new slash A-A-K-A-S-H. That's Bolt.new slash Aakashgupta. Here's the problem with most AI tools. They just sit there waiting for you to prompt them. You do all the remembering, they do the typing. Ari from Ariso flipped that for me. It connects to my email, calendar, Slack, and it works the other way around. It comes to me. Monday morning, there's a briefing waiting. It reminds me what we covered last time and what I promised to send. When a follow-up slips, it nudges me before the other person has to. Every commitment, every thread, every contact, tracked and organized without lifting a finger. And because it has continuous memory, it actually gets smarter the longer I use it. It's not a chat window. It's one AI partner that knows my whole working life and it keeps me prepared for all of it.

<!-- sponsor -->
**Aakash Gupta** (00:15:16)

If you're tired of being your own chief of staff, try ARI at oriso.ai slash akash. That's A-R-I-S-O dot A-I slash A-A-K-A-S-H. Can we scroll through that file a little bit just to see how it's put together?

**Guest** (00:15:30)

So which particular file?

**Aakash Gupta** (00:15:32)

The scaffolding skill.

**Guest** (00:15:34)

Oh yeah, so the skill. So yeah, if you go to new project scaffolding, you have the main skill here.

**Aakash Gupta** (00:15:41)

So if we scroll through that, how is it... Okay, so it's got each step defined. And if we keep going, like for instance, the sharp test, is it going to go call that skill?

**Guest** (00:15:59)

Yeah, so for example, the workflow is to gather context. It will ask you questions if you don't have it. It will find a project type. Is this an iOS app, Android? Because of my prompt, it was pretty clear what it was. It will... Look for reference projects around the internet, some of the best practices, and it will try to understand how to build this. It will run a viability gate. This is a compressed version of the SHARP problem, state where it will go through, run clarity, target user, competitive landscape, differentiation. The sharp problem test is even more specific. The thing that differentiates that is that it tries really hard to focus on three times value that you create. That's not in here. This sort of looks at the market space and see, is there a lane for you to be in this lane? And the sharp problem test will do something even deeper than that.

**Guest** (00:16:56)

Whether you will make money, that's really what sharp problem space is. This is about, is there a lane for you? And if there are three dimensions of our week, it will just recommend that you don't do this at all. This is very important. LLMs very rarely tell you no, and this skill will tell you absolutely no, don't do this. And I'll demonstrate that in a second. I'll tell it to scaffold a new thing. That I think if we look at it, it might look on a boundary, but it will say, it will probably say that we can't do this. And then market research is huge. You know, we tell people like, you know, market research is weird. Like you probably shouldn't do market research with only LLMs, but you can do a lot, 60%, 70% with LLMs before you go find real sources. And I want to step back and also tell people the danger in this kind of workflow is that You take it as gospel, right?

**Guest** (00:17:52)

You really do need to look through all the output, make sure that it makes sense for you. We do this all the time because, you know, I think it's hard to fully trust 100% LLMs. So if you go here for, okay, we're still in skills, so let's finish that and we can see. So it will generate the perfect Claude MD for you for this project. So if you look, you'll see people spend a lot of time thinking, okay, How do I author my ClaudeMD? What's the thing in the front matter and in the rest of it? This says for this project, here is a ClaudeMD that works the best for you. It'll create a ClaudeMD that does the project well, hunts bugs, follows the patterns of the folders, follows the patterns of the prototypes, and it's perfect for this project. And then it will create a folder structure.

**Guest** (00:18:42)

So it will say here's where you need to put the documents. Here's where all the milestone things. And by the way, all this is in the Cloud MD. So this is basically a self-organizing repo already. If you're going to use it, here where the prototypes go. And for each folder, it just tells you, it tells Cloud and it tells you exactly what goes into it. It creates a test folder for you. And then crucially, it sets up your continuous integration, your quality system. So every time you check in, All your code is tested and it sets up security. It starts to find things that you shouldn't, your secrets are particularly get ignored so it knows how to do that so you don't have leakage when you push things to GitHub. And it starts quality, right? It starts key quality documents, you know, how to, you know, do bug classification, how to learn.

**Guest** (00:19:32)

It starts to catalog Over time, bugs are made and how to learn from those bugs. So there's a lot that goes into this. And then some of the harder things that it offloads are the CI templates, CloudMD patterns, so it gets the perfect CloudMD. So these are all called within that skill. And so if you go back here, What you have is essentially, we start out with a very clean, empty folder, but this is all you have now. And so it gets ready for you to commit your first check-in on this project. So why don't we try this? Why don't we try another project that may or may not, we won't say anything. May or may not pass the viability gate. Should we do that? Let's do it. Okay. Okay. So let's do this. Run the scaffolding. Scaffolding. Run the scaffolding skill on a new problem.

**Guest** (00:20:51)

Use a new folder for it in this one, in this repo. Okay, let's do that. And so I am going to try to solve a standup problem. I'm going to try to ask it to build something for a project called Stand Up Zero that sort of uses Slack comments and creates a daily standup digest and ask it to run a viability gate first. Let's see what happens.

**Aakash Gupta** (00:21:29)

So while this is running, how much of this thinking, like viability gates and sure problem tests, should we really be outsourcing to LLMs? Is LLM basically the first draft just to get some thinking going and then we improve and react?

**Guest** (00:21:43)

Yeah, the very specific thing that we are trying to solve is that if you start in chat and start with, hey, I have an idea, you know, Unless you prompt really well, and unless you sort of sold on adversarial prompting, or even some people go as far as they will check with multiple different kinds of LLMs, what you're going to see is it will tell you that you have a good idea. The thing about this is that It's built in, it has a built in sort of responsibility to tell you whether you're smoking crack or not. And I don't, I mean that jokingly. Tell you whether your idea makes any sense. And it doesn't just ground it in the model's sense. It grounds it in a really clear framework that has evals that goes through very systematically. So I think that's the main difference. Now, should you trust it completely?

**Guest** (00:22:50)

I've already said you shouldn't. It produces real artifacts that you should go check. So it will create a viability gate document. You should look at that viability gate document and see if you agree with it, see if you can do extended research with it. What is your first draft? It's your first thing out of the gate that has the ability to say yes or no, and here's where you need to go. Okay, so it doesn't have enough information, so it's asking me questions. What should standard 0 be built as? Let's call it Slack, TypeScript and Slack. How far should this scaffold go? Let's go to the gate first and then pause. Because if the gate says no, then what are we doing? Submit our answers. All right, let's see what it says. So it's gone off and done some crawling, some competitive research, as we saw.

**Guest** (00:23:58)

And it's trying to figure out if this is worth it. I've read some of the stuff it comes up with for the market research, and it's really good. It will do a real, basically as high quality as perplexity will do to go look for whether there's a space for you.

**Aakash Gupta** (00:24:21)

Okay. And does this apply only to new products or what about like features for existing products?

**Guest** (00:24:27)

That's a really, really good question. So because we realize, you know, a lot of vibe coders will say, I could never build before I need to build. So this is perfect for that. When I started the first demo of CodeMemo, I used these skills to do it. But really, Most PMs don't start brand new projects. So we have features for them. So for example, this is called the vet a feature. I have a feature idea. Should I even bother building it? I have opportunity costs of other feature ideas. And so this particular skill will take a feature idea and tear it apart. Look for anti-patterns. Confidence. So it's like a scaffolding skill but very specific for a feature within a product. I think this one's actually even more interesting because this one actually focuses very hard, not just on the lane, but whether it's worth building at all amongst other features you have.

**Guest** (00:25:34)

So the sharp problem test is baked in really hard into this.

**Aakash Gupta** (00:25:42)

So the key lesson here for any PM is like create a skill like better feature. You can grab OGs, which we're going to link down below in the description, but fundamentally you need to work with LLMs to actually figure out, is this a problem worth solving? Is this the right problem space? And before we used to do that all by ourselves or skip that step entirely. And this is really helping us have a thought partner, make sure we actually do it every single time.

**Guest** (00:26:09)

That is correct. That is correct. We want you to think about the full stack of the problem. Again, business, product, and code together. When you work in triads or quads or whatever that is, because of the people around you, if you're lucky, thinking about all those things together, and you're like, is this worth solving as a PM? And the developer is like, oh, here's how we're going to do it. And the product marketing is like, here's how we tell the story. I'm going to go off and do research. What we're doing is compressing all that into one really smart orchestrator and builder can get started really fast. It doesn't mean you don't need specialists, by the way. Big companies always need specialization. That's a given. But in small startups, in smaller companies, and even as you scale up to big companies, the ability for people to, one person holding a critical skill, say product, To really have agents that help them with the first draft of these things is incredibly powerful.

<!-- sponsor -->
**Aakash Gupta** (00:27:13)

Quick thought experiment for you. Is there anything in this video you should be trying on your own? If there is, try it, take a screenshot, post it on LinkedIn or X, and tag me. I'd love to see what you're learning. Now a quick word from our sponsors before we get into the back half of the pod. I used to think I had a retention problem. Turns out I had a messaging problem. I was sending the same onboarding emails to every new use, whether they activated on day one or never logged in again. I had no idea who was slipping or why. Customer.io changed that. Every message I send is now based on what users actually do in the product. Someone hits a key activation. And when I want to know how something is performing, I just ask They also have an MCP server, which means AI tools like Claude can see directly what's happening in your Customer.io workspace.

<!-- sponsor -->
**Aakash Gupta** (00:28:11)

Your segments, your customer data, your attribution, all of it. So instead of explaining your business context every day, Notion used Customer.io to personalize their onboarding and hit nearly 50% open rate, improved conversion by 6-7% with localized campaigns, and pushed open rates up another 20% through The idea is simple. Customer.io helps you deliver more impact from every message you send. If you're a PM or founder and your onboarding is still one size fits all, try Customer.io at Customer.io. Are you looking to land your next product management job? I am accepting a group of Just 30 product managers into a 12-week cohort led by me where every Monday for 90 minutes, I help you through your job search, creating your candidate market fit, updating your LinkedIn, updating your base resume. You're going to get personalized feedback and one-on-one mentorship sessions with my co-teachers, Ankit Farmani,

**Guest** (00:29:05)

who is an AIPM at Atlassian and was a group product manager at Meta.

<!-- sponsor -->
**Aakash Gupta** (00:29:09)

Prasad Reddy, who is a CPO and has been in product for over 26 years, as well as my other live instructor, Bart Jaworski, who's going to run another 90 minute session per week where we really help you deliver on all of the deliverables in an actionable way and get you custom resume feedback, custom LinkedIn feedback. This program worked So, if you want to get a higher paying PM job, be sure to check out my The next cohort starts in February, runs through the end of April. The next time I'm opening up a cohort is in May. So if you want coaching from me to land a PM job, this cohort is a no-brainer. It is a premium priced product. It is more expensive than the average product out there, but the return is huge. Most people who join the cohort see a salary raise anywhere from $10,000 to $100,000 in the first year.

<!-- sponsor -->
**Aakash Gupta** (00:30:09)

And so the ROI will be there within a year. And we guarantee two plus interviews. So if you don't get two interviews after completing the 12-week program and following all the steps, we will refund the money to you. So it's a no-brainer. Check it out at landpmjob.com. And now back in today's episode. Do you know how to take an AI product from idea to development to evaluation to deployment and eventually to scale? That's exactly what Product Faculty's AIPM certification helps you do. I even took the course myself. You'll learn directly from Rohan Varma, the product lead working on codecs at OpenAI. You'll go deep into AI prototyping, evaluations, agents, AI-native workflows, cloud code, OpenClaw, latency, cost, guardrails, rag, routing, fine-tuning, and production systems. You'll even build your own AI product as your capstone with unlimited one-on-one support. So if you want to stop just learning AI and actually build AI products that work, join Product Faculty's AI PM certification on Maven.

<!-- sponsor -->
**Aakash Gupta** (00:31:09)

5,000 plus students have graduated and they have 1,000 plus reviews. Use code AKASH550 to get $550 off your enrollment. So maybe we can turn over to the other one that's ran and you can show us like how you apply your PM judgment on top of what it's written.

**Guest** (00:31:28)

Yeah, OK, so that's a good point. So I'm back in the first one. And let me just make sure that it's done. So I'm going to ask you to continue and share the final results in a table for me so that we can know that it is done done. And we're going to get out of, so yeah, so here's the result. Okay, so it's done market research, it's decided what's viable, quad, structure. So the way to think about this now, once you're here, It's to go back into this and start to take a look. I've worked with developers in the past who I've had to insist that they actually do code review even if they're working with AI. And so the first you start first is these two documents, right? The other ones are sort of boilerplate. So I'm going to create some space here. So this is the market research document.

**Aakash Gupta** (00:32:46)

And then I think if we double click, if you like two finger click on the market research, I think you can open as preview so it looks a little better, right?

**Guest** (00:32:57)

Okay, let's do that. There we go.

**Aakash Gupta** (00:32:58)

Perfect.

**Guest** (00:32:59)

Okay. Well, you know a VS Code trick that I don't. So that's good on your cash. All right. So market overview, it sits at the intersection of AI code. So look, I don't want to read through all this. The first thing is to take this for yourself and for PMs, PM leads in your space, and see if it covers all the ground that you need. The things to look out for is does it mention the kinds of tools you expect it to mention? Well, these are a really good set for this kind of tool because these are your competitors. Does it mention in each of these categories all the things that you wanted to mention? You take a sense check of these things like if it mentions tools that are old, Tools that are not functional, tools that are sort of decrepit, you shouldn't trust it.

**Guest** (00:33:56)

If it mentions tools that are current, adjacent, things that you were thinking about as you were thinking about the problem but they didn't actually solve the problem for you, then you are on the right track. Take a look at this differentiation map, for example. Does it seem right? No? Yes? Where does code memo sit? Does it seem right for you? And so this is your first scan for credibility. Imagine that you are doing a PRD review in a room full of PMs. This is what essentially you should be doing with this one. And then it actually writes a PRD for you. And so this is the real PRD review. So is the stuff in the market consistent with what it's writing for you? So let's scan this very quickly. Code is now produced faster than anyone can read it. AI code gen has split order ship from understanding.

**Guest** (00:34:53)

The person who wrote an app via prompts often cannot evaluate whether it's safe, correct, or production ready. This bites two groups hard. Solo founders ship AI generic code they cannot audit. Corporate developers Onto an unfamiliar codebase. So it came up with all this by itself. And if you stare at this and say, shit, I would invest in that. I would spend time on that. It nailed exactly what I want. Or you should be asking yourself, what did it miss? What persona did it miss? For example, what I notice here is that It says the primary is a non-technical founder. Makes sense. Small company, sure. It's probably not a big company founder though, right? They have more resources, more tools. So I'm glad that it said non-technical founder, but it didn't qualify by the size of the company, for example. It sort of doesn't think the corporate developer is the strongest thing, right?

**Guest** (00:35:57)

Antoine and Harry, who needs evolving story? Well, it's completely out of scope to protect focus. That makes sense, I guess. I read the output and it mentioned that it's much lower value proposition for the corporate developer because they have so many more tools to do these things. And so the Vibe Coder is a real target for this. Value proposition, paste a GitHub URL, upload a viacoded folder. In under a minute, get a plain English verdict on whether the code is production safe. So this starts to tell us that the value loop is really good. It's really powerful. Okay? Right? And so I would scan this and see, is this the kind of high level product brief I would write? What's missing? What's missing if I wanted to present it to other people? And that's how to evaluate this.

**Aakash Gupta** (00:36:48)

Cool. Let's go take a look at the other agent and see what it did with our other idea.

**Guest** (00:36:54)

Okay, let's do that. So let's step back here. It looks like it is still crunching through the viability gate. So let's go to that folder. And you can see it's called Stand Up Zero here, and it is... Crunch through the viability assessment. And so scorecard. So it's weak, right?

**Aakash Gupta** (00:37:34)

So this is the real sort of alpha from using a skill like this. It's going to help you separate out which features, or in this case, we showed new products that you should be building and shouldn't be building.

**Guest** (00:37:45)

Yeah. So here it says there were three moderate scores. So it's saying, I'm not sure about this, basically. You should proceed with eyes open. And then it goes into the details. Problem clarity and urgency is moderate. It's just workflow convenience. It's not very deep. Target user definition isn't very strong for what I pasted in. The competitive LangSafe is very strong. It's actually a bad thing. There's a lot of competition here. And so it's calling out all these things for you. Differentiation isn't very strong. So all of this is basically pointing out to like, it's going to be very hard for you to enter this market. It's not defensible for you. Everyone can build exactly what you're building. So if you really want to continue this, you should maybe pause and think about it, basically. Now, I don't know about you, but I think that's worth a lot from start, right?

**Guest** (00:38:52)

This is you thinking... Hard about where you're going before you start thinking, I can write code because what we see today is people just build. People build and then there's no customer for it. There's nobody for it. In fact, it's super puzzling right now because it feels like GitHub is the only place that people can express themselves. When they have cloud code, they just build anything, put it on GitHub and just languish with zero stars, if that makes any sense. Now, if you are someone who wants to make an impact in the world, this kind of thing will help you conserve your time, attention, and focus on all the right things.

**Aakash Gupta** (00:39:32)

So where do we go from here? We promised that we'd help people become a builder PM. What's the next step once you've figured out the right idea? In this case, we're knocking out stand up zero, but we're in favor of code memo.

**Guest** (00:39:45)

Yes, so let's go back to code memo, right? And I think we get to tell it to continue. All right, fantastic. So the next thing I would do is prototypes, right? And this is a fun one. What should What does the code memo look like? I want to establish the basic interaction model that delivers value. Can you first ask questions about user interacting with code memo? And then we will generate a set of X prototypes to evaluate what direction to take this in. Now this is very compressed, right? Like you don't necessarily start with prototypes, but you do start with interaction. And by that I mean specifically, does this have user experience? Is this just a chat interface talking to an agent? Like what does it look like? How do you initiate it? And so I'm going to ask it to use its survey skill to help me make the choices.

**Guest** (00:41:32)

So now that it says go, what I'm trying to do next is really to start to build a baseline of the code, start to build a baseline of a product. If you look at these skills, there are a few directions you can take this in. For example, the interesting one that I would do right after this is a customer discovery week. Okay. I'm going to ask it to use this skill to tell me how to get to better confidence and to answer the unknowns. Okay. So while it's doing that, I'll prep that question. So I need you to Develop my customer discovery plan by running the customer discovery week skills. So on one hand, I'm trying to generate ideas of what interaction is. On the other hand, I need to ask a bunch of questions. So let's tackle the questions about the interaction model first. So paste a good hub URL.

**Guest** (00:42:47)

So I don't like any of these. So what I'm going to say is I think It's both one and two. So I need you to paste the GitHub URL, but I'm going to connect it to GitHub because I need to analyze the code that I'm writing because I'm a Vibe coder. How is the verdict delivered on screen? This is a score, single verdict card, narrative scroll, conversational chat. So I think that it needs to be a dashboard and drill down. Once the verdict is on screen, what should the user be able to do? Depth of engagement? Nope, I needed to do two and three. So two and three and four. Okay. In the first 60 seconds, this is interesting. It's getting to the aha. What was the core value the user came for? Two, understanding. Submit those answers. All right. I need to develop my customer discovery skill plan.

**Guest** (00:43:56)

We're in the customer degree with skills on the product brief and the Market research. Do this in parallel while finishing up. It's going to spin up a thread finishing up the interaction model. OK, so I'm basically doing two things now. I'm grounding my sense of what interaction is. And I want to launch additional research to really figure out if I fully understand the problem. Now I would ordinarily do the first one, the second one before the other, but I just wanted to demonstrate the two different ways. You can go straight to build or you can start to talk to customers about it. Okay. So what we're seeing is summarizing the tension. And so it's going to generate three self-contained HTML CSS prototypes. The skill itself tells it to do this, prototype before you react. So it's going to go off now and it is going basically start to write prototypes.

**Aakash Gupta** (00:45:11)

So the last set of skills in the diagram we started with was really the business layer. Like, is there some business viability? We talked about in terms of new product for a feature, there might be some more nuance there. Then this next layer is really that product layer, right? We're figuring out the prototypes, what actually works. And we're going to go through and find a prototype that might potentially actually demonstrate a viable solution so that we can test that. Is that right?

**Guest** (00:45:36)

Yes. Can you still hear me?

**Aakash Gupta** (00:45:38)

Yeah.

**Guest** (00:45:46)

Yeah, so that's exactly right. We started out with a business problem. Is there a lane for us? Are we thinking about the customer correctly? There are other business problems that you get to later, pricing, access to market, what's your marketing plan? But what we're doing now is a product. It's like, what's my customer discovery so I can dig deeper into the problem? What does this even look like? Just for, you know, PMs, you know, we get this, like as PMs, we own usually, usually we own, why is this a thing that we've spent time on as an organization? What is it, which is, how does it instantiate? What does it look like? What does it feel like when it's solving the problem? How does it generate delight? And of course we share this with designers and So we're still early in that process. Is this prioritized by my CPO?

**Guest** (00:46:41)

As you mean, you're a bi-coder. What don't we know? What does it feel like? What does it look like? These are all the things that you take to developers. What you have now is that because you're doing it all in one shot, inside Cloud Code, you can compress all of that within one Cloud Code session. You notice that we are not in Cloud Code desktop and co-work. You can do all this Within one session. So what we have here is it's done some prototypes. What's that shortcut you liked again? So while this is running in the background, I am going to show you some of the prototypes it's made. I really hope to God because we didn't install a lot of design skills. Can you see this? Yeah, so it's made a few things for us to take a look at. The way you should think about this is prototypes.

**Guest** (00:47:38)

You should just get a feel. This isn't real design yet. This is definitely about where do you start. So here you see it, you paste in the GitHub thing here and it tells you the story of the code very quickly. Here, more of the same, but more data Logic up front and here's sort of a side panel where it does similar things. So what I usually do when I start to work on these things is I will have, in practice I'll have ShadCN, I'll have UI, UX, Pro Max skills. I'll have like five or six design skills and I'll tell it to use one design skill. To make a prototype. So if I have six design skills, it will make six prototypes. And I'll ask it actually, because you can make hundreds and hundreds of prototypes, I'll ask it actually to combine two skills each. So it will make like six more skills, but using two design skills at a time to do it.

**Guest** (00:48:38)

And so I can see what this could look like for us. But all this is baked into the skill directly. I'm going to go back to Cloud Code and share that screen again. And then we'll take a look at the other task that we asked it to do. Okay? So by the way, it is asking me about the interaction model I want. We're not going to spend time figuring that out yet. So we decline that. So we're going to instead say the discovery plan agent finished. So it's created a customer discovery plan for us. So we're going to go to docs. And we're going to go to customer discovery plan. And we're going to take a look at it. Okay? And it says, the plan itself is complete and executable. Every script, a survey, the synthesis template, and the week's time budget are below. What is missing is a one input.

**Guest** (00:49:34)

The skill will not let a plan proceed. A confirmed list of recruitable people with real target cohorts, not adjacent contacts from the founders network. The skill treats fewer than five real target contacts on validation signal. It means you may not have access to the market. Again, very important. It says you can't just wing this. You need actual people to talk to. And if you tell me who they are, then I know that you're ready for this. And so what we can see here is the three-step interview process that it wants us to do. So let's see. It tells you how to recruit, what the gates are, where to go shop for targets. The hypothesis you want to validate. Step one, motivation. So it walks through. In the book, we talk about this three-step process where the first step is figure out what questions to ask. Open-ended questions, no motivation, no direction, no prototypes whatsoever.

**Guest** (00:50:41)

So it walks you through that. Tell me about. Walk me through the last time. So it's walking through people's workflows. And then step two is when You take those things and say, okay, I now think I have the questions I need to answer. And then it will codify those questions that you answer. So the first step, you learn what questions to ask. The next one, you use those questions to ask. And then the third, you expand it so it becomes data. So once you really solidify the questions you're asking, you can start getting sample of the answers. You turn it into a survey so you can quantify the responses that you get. So it builds all this for you, ready to go. In this case, it's saying, listen, you sound like you're still winging it. You need very specific people. Go find them and I will help you validate that you have a real customer discovery plan.

**Aakash Gupta** (00:51:36)

All right. So what I'm really hearing from these skills is that they're forcing you to do the PM fundamentals. And what they're doing is they're giving you the first draft of those things. And to be a true builder PM, you need to be able to do this at engineering speed. And that's why we're relying on these skills. We're not just doing it hand as we did step by step in the past.

**Guest** (00:51:59)

Correct. So what we, there's something we call the three speed problem. Which is for the past 40, 50 years, whatever you want to call it, the longest pull has always been development. And it's long in many ways. It takes time to actually write quality code. It takes time to do quality. It takes time if you're in the cloud to make it robust, not fail, to do DevOps, recover very quickly. All of that is being cut down, maybe by 10x, maybe in five years by 20x. But really, the process of building is not just code. It's like, why should we build, build it, get it to customers? So if this middle speeds up very quickly, you start to have almost an equation imbalance. And the reason it's imbalanced is because The why should we build is customer bound. You have to talk to people. You have to talk to the market.

**Guest** (00:53:01)

And the other side, access to the market, getting it into people's hands, is also customer bound. Because, you know, Antropic has shipped, what, maybe like 60 features in 30 days? They're becoming recursive, correct? By the way, that's a whole other thing to talk about, which is how to build feedback into the skill. So some of these skills build feedback deeply into the product automatically for you. And we're trying to refine some of those things. We haven't shipped that one. But I don't use, like we were flexing with slash commands just now. I don't know all the slash commands. So I can actually absorb all the features that they make, right? I'm limited by that. And so you see them, I don't know if our audience knows this, but Cloud Cowork was just completely redesigned, right? They shipped it. And it seemed amazing, but there was no adoption.

**Guest** (00:53:59)

And so they've just sort of blended it back into chat, right? A bit versus having three tabs, code, co-work and chat. Because it didn't stand alone by itself. So people are having to not just ship very quickly, but make sure they have the right thing. And by situating this in the same skillset that Your developers use that you can learn very trivially. You see a massive amount of speed up, right? Because this repo can be your developers repo as well, right? It's not different, right? If your developer, if your founder and your developer is working on this, they can see All the business skills themselves, they can run it themselves or you can run them, right? So we are seeing people essentially collapse the separation of tasks of PM, live in Notion, designers live in Figma, and collapsing it into one GitHub repo. With everything. And the coders will live here on their source, tests, all the security stuff, playwright, test, vitest.

**Guest** (00:55:15)

You live up here. But it's joint context in one repo for every member of the team who needs to touch this stuff. And everything is always available to them at all times.

**Aakash Gupta** (00:55:31)

Amazing. If people want to go grab these skills, can you show us where they can go grab them?

**Guest** (00:55:37)

Yes, I can, Aakash. So I am going to share a different screen. So one of the fun things we've done at Product Mind as we start to build is start to collect these things. Some of them are private. They're not available yet. But if you go to the labs at ProductMind.com, just ignore these things. This is not a monetizable site yet or at all. This is just to show the products that we can actually share from our engagements. But everything you've seen actually can be accessed more trivially through what we call skills at ProductMind.com. So you can chat with it without going into cloud code. So that's the first thing. The second one, and we have a lot of people who do this now. And the second one is a skills library. The skills are open source. So you can come here and you can browse through them, read them.

**Guest** (00:56:43)

Here you have the new project scaffolding, vet a feature, Vibe Memo. I'm very, very excited about this one. Vibe Memo is a simple system, we installed it, that captures your decisions as you build. So right now when you write code as captured, But VibeMemo says capture the why. Why are we making these decisions in the code? So it keeps the why with all the decisions in the log for you. I find this very exciting. So every time we have a big code base, we want to take a look at why did we even make that decision? What were we thinking? Vibeba captures it. Sharp Problem, Test, Reverse Femia, there's so many. Let me just point out a few more favorites. One is Roadmap from Strategy. So to construct a whole strategy for you, Another one is a listening machine. It will turn all the surfaces in your product into feedback tools that constantly collect information.

**Guest** (00:57:41)

These are things that people spend years and years trying to figure out. We build it into a skill that gets you started immediately. Scope Cutter. We all do this. We've got to cut scope. And Scope Cutter gives you a very succinct way to reduce how much you do. There's even a simpler one, which is once you want to build the first thing, Are you going to do an MVP, which is just for learning? Or are you going to do an SLC, which is actually to put in front of people for them to be amazed? And how do you even do that? And how do you cut? And so on and so forth. And of course, advanced things like pricing, like how should you design pricing? All built in. So again, business and product level skills that merge with code skills in one place for you to become hyperproductive.

**Guest** (00:58:28)

We think this is the new frontier. I think code skills alone are becoming passe. The other day I saw someone remove superhuman skills from their repo because the models are so good. Some of these skills are breaking. But these business skills, these product skills, these are still the things that give us the ability to build the right thing. So I'm super excited about that.

**Aakash Gupta** (00:58:51)

And today we showed the harness as Claude Code in anti-gravity. Is there any particular reason you should be using anti-gravity or can you use any harness for Claude Code?

**Guest** (00:59:00)

No, it's any harness. I don't even particularly. So anti-gravity is a fork of VS Code. So it looks a little bit like cursor. It looks like VS Code. That's just what I have on my screen. I'm running through a terminal. And so I actually don't use any features of anti-gravity. It's just, you know, it's a nice interface, but nothing special about it.

**Aakash Gupta** (00:59:20)

So if you're a product leader, right? You go ahead and you download these skills, you make these skills your own, you distribute them to the team, the team is starting to use them. You are one of the few people who's actually helped teams do that. So you've gotten to see what are the mistakes that people make? What are the problems or the pitfalls in rolling out this new way of working that people should know about so that they can avoid them?

**Guest** (00:59:45)

I think that the most important thing A shared context. You know, I heard Boris from Claude talk about the fact that his Claude.md is a very thin, it has only a few lines, maybe six lines. And what it's actually doing is that it's referencing a shared Claude.md. Now you should think about Claude.md as some kind of like base skill. Basically. And so centrally, they author CloudMD and optimize it like, think about once a minute. Everything that everyone is learning is being put into that central CloudMD. It's small, it's short, it contains essence. It connects people to all the right tools within the organization. So I think that the biggest lesson for putting this into an enterprise is don't let people fork these things willy-nilly. For example, I was working with an enterprise that had a ways of working document and then they had a very specific SDLC that was supposed to produce very specific artifacts.

**Guest** (01:01:11)

What I would do in that situation Is to take the relevant skills here, for example, the scaffolding skill or the vet a feature skill. And I would harmonize it with what they need to come out of it. Why would our product brief be different from what the organization wants? It shouldn't be, right? Why would market research document be different from what the product marketing team would produce or what they believe is right to produce? And so we would essentially centralize this modified so that it creates artifacts that our organization needs and just prevent people necessarily from forking it themselves. Now, to be clear, I like organizations where it's sort of open source and if people learn new things because, you know, the CPA doesn't know everything, you give people the license to innovate. Well, if they innovate, they should innovate into a central place so everyone gets the innovation, if that makes any sense.

**Guest** (01:02:08)

So I think that's the biggest thing is when AI rollouts are completely ungoverned in a way that doesn't have shared context. Because, listen, I think in science fiction we always sort of We're afraid of the hive mind. We're afraid of AIs collaborating because they'll kill us. But it turns out that we are the original hive mind. The only reason that we've survived through the centuries as humans is because we learn from each other. And so this is very imperative. When you roll out AI, try to force it into a structure that one person learning means everyone has learned. That's one of the big powers of it.

**Aakash Gupta** (01:02:52)

OG, you've generously shared these skill files. You guys can find the link in the description to this GitHub repo. As he said, you can make these your own. That's really the key, adding it in to make it your own and then deploying it as an open source repo for your team to use. This is the playbook. If you've been wondering, how do I become a more AI native team? How do I get my PM team to work at an engineering speed? We've just given all of that away for free. Thank you so much for being here.

**Guest** (01:03:22)

Thank you, Aakash. And I hope people become even more effective product builders and hyper creators with the stuff that we've made. Super happy to share.

<!-- sponsor -->
**Aakash Gupta** (01:03:34)

I hope you learned as much from today's episode as I did. If you can do one thing that's totally free that would help the show, it would be to check that you're following on Apple and Spotify podcasts. Check that you've left ratings and reviews on those platforms. Check that you're subscribed on YouTube. Leave a like and a comment on this video and then share it with your friends. We're trying to make better and better podcasts. After two years, we think we've gotten something pretty good going. So let us know what we can do to make it even better, who else we should interview and we So check that out at bundle.akashgu.com if it interests you. And I can't wait to share our next episode soon.
