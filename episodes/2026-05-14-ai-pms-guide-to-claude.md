---
title: "PM's Guide to Claude - When to use Chat vs Cowork vs Code, with Pawel Huryn"
subtitle: "What the PM who tracked Anthropic’s 74 releases in 52 days actually runs on his own machine - from Cowork to Claude Code to Dispatch."
date: "2026-05-14"
host: "Aakash Gupta"
guests: ["Pawel Huryn"]
speaker_names: "substack"
substack_url: "https://www.news.aakashg.com/p/ai-pms-guide-to-claude"
youtube_url: "https://www.youtube.com/watch?v=bITUsUsrxjM"
duration: "01:32:39"
word_count: 11985
source: "Substack episode transcript (aired audio)"
---

# PM's Guide to Claude - When to use Chat vs Cowork vs Code, with Pawel Huryn

*What the PM who tracked Anthropic’s 74 releases in 52 days actually runs on his own machine - from Cowork to Claude Code to Dispatch.*

**Pawel Huryn** (00:00:00)

There's no good reason to talk to Claude just over a normal web chat anymore. I don't use chat at all. I use it sporadically, just if the window is open, I can ask some questions like, is this grammatically correct?

**Aakash Gupta** (00:00:10)

Claude is way better at using PowerPoint than it was. There is no excuse to walk into a meeting with a bad presentation anymore. You basically get a McKinsey-level output in a minute or two. Core is not

**Pawel Huryn** (00:00:20)

adjusted to working with codebases. As a product manager, you will be working with codebases a lot.

**Aakash Gupta** (00:00:25)

Pavel Hearn is the number one AIPM voice in Europe with over 200,000 LinkedIn followers and over 100,000 newsletter subscribers. And today he's going to break down everything you need to know to get the most out of Claude as a product manager. In Co-Work we can organize

**Pawel Huryn** (00:00:55)

working projects or folders. So what you can see here, most people stay in chat forever. That's like using Photoshop only to crop photos. And today we are going to discuss chat, which is part of the cloud desktop, but also co-work, cloud code, dispatch, which allows you to control remote sessions for co-work and code, web sessions, and how to use them all to 10x your productivity.

**Aakash Gupta** (00:01:18)

Before we go any further, do me a favor and check that you are subscribed on YouTube and following on Apple and Spotify podcasts. And if you want to get access to amazing AI tools, check out my bundle, where if you become an annual subscriber to my newsletter, you get a full year free of the paid plans of Mobbin, Arise, RelayApp, Dovetail, Linear, Magic Patterns, Deep Sky, Reforge Build, Descript, and Speechify. So be sure to check that out at bundle.akashg.com. And now into today's episode. So Pavel is the guest behind our most popular episode ever with over 65,000 views when he gave an impromptu complete course on AI product management. He did the NAN video which absolutely crushed with over 10,000 views. Before that he did a discovery masterclass. Today he is back for a record fourth time. to help you understand how to get the most out of your Cloud Enterprise subscription.

**Aakash Gupta** (00:02:17)

When to use Cloud on the web, when to use Cloud Cowork, when to use Cloud Code, when to use Cloud Dispatch, Pavel has tried all of the combinations of PM task versus tool and he is going to break down when you should use which tool for what and he is going to break down how you can create a self-improving system that builds upon itself so that every time you do something the system gets better at doing that task. Pavel, welcome back to the podcast. Hi, Akash. Thanks for having me. I love getting your newsletter in my inbox one of the most interesting things you've been writing about recently is how Anthropica has gone from a billion to 30 billion in 16 months on the back of this insane shipping velocity

**Pawel Huryn** (00:03:06)

you

**Aakash Gupta** (00:03:06)

tracked 74 releases in 52 days which is pretty mind-blowing. Putting aside what's happening at Anthropic, what I want you to help us understand is what does this velocity say about the future direction of product management?

**Pawel Huryn** (00:03:21)

So what I can say by observing Anthropic is that they are adjusting and many companies not just Anthropic are adjusting their workflows to AI so they do not use AI to replace steps in their processes but to redesign their processes around what is currently possible what I can see in many companies is that those roles so Product Manager, Product Marketing Manager, Designer and Engineer are maybe not merging but coming closer together and many of the things that required a separate role like maybe prototyping, maybe testing writing release notes even this designing an interface based on the design system this is all being automated and for a PM to be to thrive in this new environment and in those new workflows product managers must understand technology they must get comfortable with tools that previously were designed for engineers traditionally, so like the terminal. They also need to go outside their comfort zone and understand strategy, understand how they work, drives revenue for the business, how it connects to business goals, product strategy.

**Pawel Huryn** (00:04:44)

understand how it translates to revenue. The future is super PM or super individual contributor with maybe a PM focus, maybe engineering focus, but having skills from multiple areas, not just one. You cannot be a product manager who only interviews customers and creates items in the product backlog.

**Aakash Gupta** (00:05:06)

Yeah, the nature of the role is shifting, but for my money, this is the most fun version of product management yet. Yeah, yeah, absolutely. In the 16 plus years I've been in this field, I've seen it evolve a lot, which is one of its constants is that it's always evolving more than the average profession. And I think this version of it is the closest to the bare metal of the product, which I think is incredibly exciting. So for this future model of product management, I want to break down for everybody who watches this episode to the end. how to embrace it, how to actually redesign their processes from the ground up like Anthropic, how to use the right tooling from Anthropic to behave like a next generation AI product manager. So that's the goal for this episode today. We're going to break down for folks. You and I spend a good amount of time chatting on DMs and WhatsApp and one of the craziest things you told me was that there is no good reason to use chat anymore.

**Aakash Gupta** (00:06:10)

That is, there's no good reason to talk to Claude just over a normal web chat anymore. Can you break this down? Because this is going to surprise a lot of product managers listening.

**Pawel Huryn** (00:06:18)

yeah like i i personally i would lie if i told you that i don't use chat at all i use it sporadically just if the window is open i can ask some questions like is this

**Aakash Gupta** (00:06:30)

grammatically correct or something

**Pawel Huryn** (00:06:31)

both most of the time when starting a session you don't know what exactly you will need and when you start a session in chat there are certain restrictions that you will face sooner or later, like you cannot continue. So let's imagine you have started your work, you're in the middle of the work and you have to leave your desktop. You cannot continue. You can copy the entire chat history to another window and maybe start a remote session, but you cannot continue in this window where the conversations happened. You cannot continue on mobile. and there are restrictions related to what if you decide that now I want to code something. Chat cannot do that and you want to create a HTML page then export this HTML page to infographic and you need this infographic in your email. once again you need to start a different session with a different context and explain what you have been discussing with chat so for me it's easier just to start everything either in with co-work with dispatch or with cloud code and then you can easily navigate between those interfaces does it make sense Aakash?

**Aakash Gupta** (00:07:44)

Yeah, it does. The issue wasn't the prompts or the tools, it was that I wasn't actually evaluating anything. I didn't have a way to see what my agent was actually doing step by step. Every tool call, every decision. That's where Arise comes in. Let me show you. I'm going to open ClaudeCode and install Arise with just one command. npx skills add arise ai arise skill skill yes. Now ClaudeCode already knows how to instrument my agent. I tell it set up tracing to arise and it automatically analyzes my codebase, figures out where the LLM and tool calls are, and adds instrumentation automatically. Now I can see everything, every trace, every span, every decision, and more importantly, I can evaluate it. That's the Trace what's happening, evaluate where it fails, then fix it. This trace right here, my resume feedback agent was supposed to pull the company's tech stack from the job posting, but instead it hallucinated that they use React when the posting started.

**Aakash Gupta** (00:08:59)

And here's the part that blew my mind. I asked ClaudeCode to look at these traces and tell me what I should be evaluating. It came back with four eval criteria I hadn't Things like picking the right tool and staying grounded in the input. I wrote the evals, ran them, and found that my agent was making the same kind of mistake about 12% of the time. Claude pushed to fix, I re-ran the evals, and it dropped to under 2%. That whole loop, trace, evaluate, fix, took me about 20 minutes and now it runs automatically. If you're building AI products and not evaluating them, you're shipping blind. Try Arise Free at Arise.com and get a year free, a 1260 dollar value with my bundle arise check it out it's one of the top ai evals platforms used by all of the top ai teams for a reason so let's make this more concrete though most pms i talk to they're finally on like a claude pro or max or api enterprise subscription and what they really need is a very clear mapping of if this then that you've mapped all of this out for us can you show us when should a product manager be using co-work versus dispatch versus code so chat

**Pawel Huryn** (00:10:17)

is like it's like a chatbot like chat GPT so you type a question it answers sometimes it can execute a simple script and for example reply with spreadsheets but other than that nothing complex so it can draft an email it can Pretend to be some person, summarize information, very basic stuff. When it comes to co-work, it's about working with real files and executing workflows. So by real files, I mean reorganizing voices on my desktop or create HTML infographic. Co-work can also plan Long running tasks. So for example, if completing a task requires taking five, six, seven or more steps, it can do that and it can then execute those steps one by one. It can also spawn sub-agents. So some tasks can be executed in parallel. So for example, you want to write an email you want to summarize your product strategy inside this email you also want to add some presentation as an attachment but the presentation should be converted to PDF so it can start one agent to summarize strategy or whatever another agent to create a HTML infographic and then maybe convert it to PDF and then another one to do something else maybe find personal details in your in some CRM system.

**Pawel Huryn** (00:11:54)

And then all those agents finish the work, it can get the results, maybe reply some steps or adjust and finish the work. So those are real, real workflows, real identity workflows with the access to real files on your desktop. And code is the same, but it's coding. except other than connecting to all those systems and working with real files, it can execute scripts on your real machine because co-work runs in a virtual machine and code can execute scripts can execute system commands on your laptop and it can also it is also adjusted to working with code bases so it means it has different set of plugins not adjusted to knowledge work but adjusted to designing front-end working with databases debugging and so on

**Aakash Gupta** (00:12:56)

A PM who's non-technical, who's watching this is probably thinking code is scary. The IDE is scary. Can I just skip it?

**Pawel Huryn** (00:13:04)

No, you can't because engineers are going to use code. And even though many features, when talking about personal productivity,

**Aakash Gupta** (00:13:14)

like

**Pawel Huryn** (00:13:15)

working with files, analyzing information, even organizing a self-improving knowledge database, you can do that in co-work. You will not have the explorer review which is about presenting the hierarchy of folders and files, but other than that, Cork can do almost everything. But there are certain features in cloud that only Cork has. So for example, the code has, so for example, one example can be SAP agents that you define in your solution. Cork cannot do that. call dynamic sub-agents but you cannot have those agentic personas that you so for example the researcher for example an agent that tests your solution an agent that creates release notes you cannot have this structure in co-work and similarly

**Aakash Gupta** (00:14:10)

there are also other features that are like

**Pawel Huryn** (00:14:13)

code specific or working with code basis specific like hooks that do not work in co-work so eventually as a product manager working with engineers you will have to work with code

**Aakash Gupta** (00:14:27)

I can't emphasize this enough as a product manager you should be learning cloud code you need to get over the initial sort of hump of this doesn't look great but claw work co-work is super powerful and so Pawel you have spent more time in co-work than almost anyone you use it for a lot of your everyday day-to-day tasks even though you are a former engineer who could use terminal just fine so can you walk us through what a power user what a master setup looks like in co-work and how you use it mm-hmm okay

**Pawel Huryn** (00:15:01)

so in co-work so first thing to understand that we can organize work in projects or folders So what you can see here, here are some of the recent folders have been working in and also predefined projects that can have custom instructions. So one of those projects is Editor, which is my project that helps me with copywriting, research, writing infographics, and other things related to content creation. But maybe we can first use it without it, so I will just select some random folder on my desktop. It's not entirely random because I prepared it before. Okay, so here is the folder with invoices. And yeah, after granting permissions, coworker can have access real files. in this folder. And the files inside are just random invoices that I collected from two months, so like Atlassian invoices, I'm not sure if preview is relevant, but yeah, like different invoices, different receipts and so on.

**Pawel Huryn** (00:16:35)

So what I can now ask it to do is to organize, analyze, pdf in voices in this folder and group them by month in folders like Jan, Mar, Jun, et cetera.

**Aakash Gupta** (00:17:10)

Yeah.

**Pawel Huryn** (00:17:11)

the duplicate the duplicate files some of the files have duplicates so which it should figure out how to do that the names might be different but the content is the same

**Aakash Gupta** (00:17:25)

and so now you guys are seeing immediately why co-work pretty much always is preferable to chat in this case it's actually manipulating things in your file system

**Pawel Huryn** (00:17:34)

Yeah, and as we can see, it created a list of steps, so it needs to extract dates from PDF invoices, it needs to identify and remove the applicates, maybe it will use a hash function, it needs to create month folders and move files and verify that if everything is correct what we can see is also the context so context for this because this is an agent the context for this agent is this file cloud md instructions There are no special instructions inside but if this file existed that would be this Cloud MD that everyone is talking about with like custom instructions when working in this folder. So the next time I could prepare an inbox and just drag and drop new invoices inside and every time a new file appears this process is repeated and the file is sent to the right subfolder. and it also dynamically loaded skills which are like procedures skills are activated based on the task that the agent currently is executing so skill has a description and based on this description an agent can decide that yeah this skill is about working with PDFs I'm working with PDFs so let's see what is inside and then it will read detailed instructions, detailed procedures of how to work with PDF files.

**Pawel Huryn** (00:19:15)

And we call this progressive disclosure. So you're gonna have dozens of hundreds maybe. of skills and Cloud will read them, so Cloud will read the detailed instructions only when the skill description matches what you are trying to do. So in this case only one PDF was identified. What it did? It created four folders, we can see it. It removed some duplicates and the names suggest that suggests that indeed those were duplicates. Let's see the folder. Okay, April, February, then March, if I open January, then I have some invoice from January. This is not a secret, maybe this one is, so let's try a different one. Yeah, like postmark, it is not a secret, I can present it. So it's February, is that correct? Yeah, it's an invoice from

**Aakash Gupta** (00:20:23)

February.

**Pawel Huryn** (00:20:26)

and that's it and I asked about PDF but you can also see that it also processed images yeah and this is some fuel invoice let me verify that it is correct it's in polish but yeah it's February I hope you can see it

**Aakash Gupta** (00:20:46)

so

**Pawel Huryn** (00:20:47)

it just it just understood that maybe Pavel didn't know that there are images inside let's let's move them to this folder uh

**Aakash Gupta** (00:20:57)

but powerful not Gemini is not the only thing that can read images these days Claude can too

**Pawel Huryn** (00:21:03)

yeah no problem what else it can do so it can work with files so we have presented that it can load skills which are instructions but skill can also have scripts to be executed inside, not necessarily, but coworker can also execute them inside a virtual machine. It can connect to external and local services and the most popular format is MCP server, so it's like the USB for agents. and by MCP servers I mean in cloud they are called connectors. So we have connector for Google, for Google Drive, for Gmail, for Slack and for dozens of other apps or hundreds of other apps. Some of those connectors of MCP servers I provided by Anthropic and others, you can just download them and configure locally and yeah, talk to your apps. So for example, I can ask, let me demonstrate. We are still in this folder, it doesn't matter, but how many unanswered emails I have.

**Pawel Huryn** (00:22:27)

Oh, this is a good

**Aakash Gupta** (00:22:28)

one. I don't want to run this on my inbox live on the podcast.

**Pawel Huryn** (00:22:33)

Do not reveal any personal information or emails. Yeah, let's just see. So it connected to my Gmail account. It can also draft emails since it can, this one cannot send, it can only create the drafts, but you can also connect a connector that can send emails for you.

**Aakash Gupta** (00:23:04)

How do you process your email inbox today? Do you recommend most PMs do it with Claude?

**Pawel Huryn** (00:23:09)

yeah I create all the responses yeah this is my current configuration so yeah cloud the system that learns drafts replies but it doesn't send them automatically so I'm using this default connector that cannot send and similarly on slack theoretically you can ask cloud to response automatically if you use this connector there is a footer sent by cloud so everyone can see it instead I ask it to draft replies and I verify them in many cases someone asks about the URL so no reason to find for this to spend time looking for this I just approve messages or edit them I send it manually so there is a button in the interface send and after every session co-work or code depending on what interface I'm using verifies my responses and tries to learn from them so the next time it will get better and that's basically it.

**Pawel Huryn** (00:24:24)

So a big thing are those skills that you can either use, predefined skills or skills from third-party marketplaces like my marketplace. That's basically it when it comes to coworkers.

**Aakash Gupta** (00:24:46)

Can you show us the pmskills marketplace? This hit 1300 GitHub stars in 72 hours. So it's gone pretty viral. Yes, of course.

**Pawel Huryn** (00:24:55)

So it's this one. It's p-h-u-r-y-n pmskills slash pmskills. It's currently 10,000 Github stars and what I have done is I created a set of plugins. So a plugin is like a collection of skills and comments and for different domains like data analytics, execution, go to market, micro research and you can load each of those plugins separately. next inside each plugin you have skills so for example if we open let's say product discovery inside there are there is a documentation so there are analyze feature requests brainstorm ideas plan experiments create metrics to track your feature and so on and also I have defined workflows that aggregate more than one skill so for example product discovery this can be okay this is a better example so discover it is from ideation then we map assumptions then we think about we think about so we analyze actually this description is not correct so it analyzes customer needs then based on those needs it will map the opportunities and how important certain problems are for the customers and how satisfied they are with what they already have then it will ideate so how we can solve those problems map the assumptions related to value, usability, feasibility, viability, maybe some ethical considerations, and it will plan experiments to prove or disprove our assumptions.

**Pawel Huryn** (00:26:53)

So this is like the entire product discovery workflow in one comment. How to use it? You can go to the home page, and there is a script, but basically you can just take this URL, go to cloud, Open Customize, let me see. Personal Plugins. Add Marketplace, yeah, like, yeah, this interface is really changing all the time, so it's, let's see, this one, I think that owner slash repo doesn't work despite the description, so let's try this one. That's my gut feeling that this can work. Okay, and those are not mine, so yeah, we can see it here. So data analytics, execution, go to market, market research, and so on, and if I click Product Discovery or Product Strategy. Yeah, maybe this one. Now it is added, installed and ready to use. What is inside? Analyze. Strategy. We have Ansof Matrix pricing strategy. So now when I go to the chat, let's start a new task in coworker.

**Pawel Huryn** (00:28:40)

help me design. And theoretically, I can count on skill being activated automatically, but yeah, if you want to read, be sure that the skill is activated. Yeah. Use the slash

**Aakash Gupta** (00:29:02)

command, which I do recommend.

**Pawel Huryn** (00:29:05)

Yeah, it's kind of messy and sometimes if cloud has general knowledge about a certain area like Product Strategy it thinks it knows something but you want to override this knowledge and without doing it explicitly it can default to to the training data so yeah if you know that there is for amazon 2.0 whatever it means

**Aakash Gupta** (00:29:33)

so it loaded the skill and now

**Pawel Huryn** (00:29:36)

it will interview me to get more information but it is it is all part of the skill so What is the core concept? Output format, then it will create product strategy canvas, by the way, based on my product strategy canvas. When you type in Google product strategy canvas, it will

**Aakash Gupta** (00:29:58)

be what I created.

**Pawel Huryn** (00:30:01)

Nice. So it looks like this. And of course, there are those famous plugins that Anthropic created. The GitHub repo with plugins and skills. The main plugin was legal. Hundreds of millions of dollars evaporated from the stock market. That's because people understood how easy it is to describe certain processes and automate them.

**Aakash Gupta** (00:30:29)

yeah with a proper markdown file written by a subject matter expert these days opus 4.5 and opus 4.6 they can really use the tools whether it's powerpoint or excel or for pms notion or google docs and they can operate it like a competent person if they have the right instructions it's pretty crazy so can you walk us through a couple of these skill files and how you constructed them and how somebody constructs a good skill file

**Pawel Huryn** (00:30:57)

yeah sure so the skill is basically how to do something so some procedure or a domain knowledge about doing something so you don't really have to create those skills manually you can describe this process to co-work or cloud code and ask it to create a skill So, basically, if you can teach, graduate how to do something, just repeat the same to cloud and it will create a skill. That's the easiest way. We can, of course, look inside and I usually don't do that, so I just use the chat interface to to talk to Cloud but yeah it's not this repo it's this one so if we open for example product discovery skill identify assumptions for an existing product we have this skill.md file and you can also have additional files in this folder but yeah basically the main file is skill.md and the format is markdown, we can see the preview in GitHub, but if I switch to the code view, there is this intros, there is this section that agents read, so they do not load the entire skill, they load name and description and when to use the skill, what it is for, and as I said when doing a specific work like use when stress testing a feature idea so if the user will write in the chat that hey I want to test this idea and assess the risk the agent will see the skill it will see the description it will just trigger it it will use it other than that this is just a prompt so it can have instructions it can be general knowledge without step by step but it can also be like step one get information from place a step b is formatted in a specific way step three is something so it's just a prompt so in this case it is yeah it's the context so you are a devil's advocate we are stress testing idea and there are those arguments so we have seen that cloud when working on strategy asked me a few questions so those are the arguments and then instructions what it should do step by step and that's all and by the way this is if someone wants to learn more they can either they can see it as a markdown file or if they keep talking to an agent the agent will suggest my articles about identifying assumptions so this is like marketing inside skills but relevant to what the person was trying to do so all the knowledge is inside skill but then the agent will also have those articles in a short-term memory

**Aakash Gupta** (00:34:35)

I would tell everybody like iterating on your skills is one of the highest ROI activities I personally have done. So take Wavel's skills as a baseline. So at least you have a baseline. But then as you encounter some feedback for his skill, give that feedback to Claude and say, I want you to improve my assumption existing skill. Read our chat and see the feedback I gave you. Understand the root cause of what drove you to give output that I had to give feedback and rewrite the scale from first principles so that it doesn't make that mistake again. I have found this to be the single highest ROI activity I do. So I think once you get the initial skill, you've got to really iterate on it to really get the ROI.

**Pawel Huryn** (00:35:24)

Like I agree, Akash. I don't know to memorize prompts. It's like in Evals and you also have been writing about Evals that when building some AI system or some AI pipeline you need to see how the system performs in real life and then identify failure modes and in this case you don't create evals but you can just give feedback to cloud say what was wrong it will understand the context because it already has this context and yeah what were your expectations it will fix that and you test it again test it again and eventually it will eliminate like maybe 99% of the of the failures so that's that's the

**Aakash Gupta** (00:36:09)

only way

**Pawel Huryn** (00:36:10)

and you cannot just see it and yeah use some magic magic technique to to get it right on the first try it doesn't work like that

**Aakash Gupta** (00:36:22)

so pavel now that people understand about self-improving skills can you show us what our skill develops

**Pawel Huryn** (00:36:27)

so we already presented that I just asked to design product strategy and it loaded this built-in so it loaded two skills one skill was designing presentations and we should see it yeah PPTX so this is a skill by Entropic and another one was my skill about product strategy from my plugin and it used it to create this slide deck. We can see it directly in Cowork. I can see it in Google Drive or displayed here, directly here. So we have product strategy canvas for Amazon. We have that product vision. Market Segments like Conscious Customers, Independent Brands Relative Costs so it adjusted colors it figure out what the layout should be this is not my branding it's like Cork's invention also icons and the difference between orange and green This is interesting, so buyers have this, whatever it means. It looks like something smart. Trade-offs, so what we are not going to do, so we have this focus on our strategy and the things that we want to say no to.

**Pawel Huryn** (00:38:09)

makes sense key metrics so how we are going to track that our strategy is working like nps order value seller retention seems to make sense north star star icon it even suggested guard line metrics so when we focus on on our notes north star how what should we monitor to make sure that our other areas do not degrade and carbon neutral delivery rate this can have an effect on I'm not sure like public relations our growth strategy why in different market segments and unit economics like this is pretty advanced and it's not a single layout it's not just those are not just tables it's yeah diverse layouts diverse icons diverse and it makes sense if I ask a graduate to do that like I'm not sure I've got that in in a few hours hours

**Aakash Gupta** (00:39:16)

yeah so there's two really mind-blowing insights for everybody here one Claude is way better at using PowerPoint than it was a month or two ago. And so you need to look at this output and see like it can use PowerPoint to create great presentations. There's no excuse to walk into a meeting with a bad presentation anymore. And the second is that it used this skill, specifically some of the things Pavel had defined in this skill around have a North Star metric, have guardrails, and it has implemented those. And so that's why if you have a good skill, you can now create things. This is why people say rip McKinsey, right? You basically get a McKinsey level output in a minute or two.

**Pawel Huryn** (00:39:55)

yeah I have defined 60 something skills but you can find hundreds of skills or thousands of skills defined by others I would recommend you to verify every skill that is not defined by entropic and make sure that it really fits your specific scenario and specific use case but other than that the knowledge is there are many free repositories I can also share those links with

**Aakash Gupta** (00:40:25)

So we'll include those in our newsletters when we talk about this podcast so that you guys get all of those. Be sure to subscribe to both. That's the Cowork segment. So you guys just got the wow moment. Cowork can generate amazing presentations for you. We showed you how Cowork can organize your file system for you. Now talk to us about CloudCode, Pavel. Why does a PM even need CloudCode? At this point, they think, oh, Cowork is good enough.

**Pawel Huryn** (00:40:50)

Corework is not adjusted to working with codebases and as a product manager you will be working with codebases a lot and also if you are building complex systems that involve multiple files then this view that what we see in Cowork is not adjusted to it so for example if I want to find this presentation I can click show in folder and it is somewhere probably in our yeah we've been working with this invoices folder so it's placed it there but imagine I have like 100 files or a few hundred files like different invoices different contractors contracts maybe some some article drafts some marketing strategies pictures brand guide and so on so those files will be organized in some hierarchy and You cannot browse them from here You can just drag and drop or select single files Just by browsing your local folder or browsing Google Drive but there is no way to easily work with those large codebases, one example, but also a list of contractors, a list of invoices, a lot of graphical files, some templates.

**Pawel Huryn** (00:42:29)

You need to upload them, find those files, upload them here, and once the agent delivers something, you need to find that in the folder or save it to the folder. Even though this is my real folder, I still need to find this file to do something with it. especially in case of code bases you need this view in which you see folders you can expand folders and you can see what is inside so for example I have infographics folder and inside infographics folder I have Cloud Code Pricing and inside Cloud Code Pricing I have some files generated by Cloud so let's see it in I will just view it here so this is not the best picture that it generated yeah but this was published today in my newsletter and also generated by cloud another one can be this picture with calendar that went viral this was also generated by cloud not by me so this one

**Aakash Gupta** (00:44:00)

This one is so good. So a lot of people, they struggle with getting faces and images and logos. So you've gotten the Anthropic logo and you've gotten those eight people's faces. Also, you've actually gotten the data from Twitter. So can you show us all three components of how you did that?

**Pawel Huryn** (00:44:20)

I think I need to explain how my system works and how it is organized to do that otherwise I can repeat the process but to explain how it works I need to just to explain the system so recently Carpathic presented this system in which you use LLMs to build the personal wiki or knowledge base for humans so you upload some information give random articles and random attachments to an agent documents and the agent organize them and then you can browse those files, browse those information and how different facts are connected I've been doing it since February 2026 and instead of building the second brain for myself I started building second brain for my agents so I'm the curator of the information and what I do is I send articles I send infographics that I find on social media I can also ask hey let's analyze the last 10 posts by akash above 200 reactions what why they worked voice hooks Emotions.

**Aakash Gupta** (00:46:13)

And a lot of people struggle with editing their terminal prompts. You were using the to do that, right?

**Pawel Huryn** (00:46:18)

Yeah, yeah. There is the second way to use cloud code. I'm using CLI inside Visual Studio code, but you can also use Visual Studio extension. They are both similar and they are not super user friendly. okay so yeah in February I started making screenshots on social media and I just I was giving different types of information to my agents so back then it was cowork and I asked what made this post or what made this infographic work and then the coworker replied with some information. In some cases, it knew the answer, so I was able to note it. In other cases, it replied with a hypothesis, so this worked probably because something. I decided that instead of noting this myself I will ask an agent hey build a knowledge database and can you please every time I give you some article or infographic organize it by domain so in this case the domain is social media so this can be x it can be LinkedIn it can be Substack and then Write the rules for which you have a lot of information.

**Pawel Huryn** (00:47:46)

If you see the repeating patterns, save this pattern as a rule. And if you are not sure, save it as a hypothesis that you can later prove by analyzing more data. So what we have ended up with is this knowledge database and I have yeah for example sound bites so what creators use to yeah core patterns that work across platforms based on data what are the core techniques like interpretation layer Unconvertible Clause Credibility Before Claim and this is confirmed across multiple, many platforms, all platforms and all creators and all successful posts. What is the award choice? A list of hypotheses. A cross-platform specific to index rejected, so also things that we have been considering in the past, but now we know they are not correct. Like, let's say on cross-platform, this

**Aakash Gupta** (00:48:58)

is...

**Pawel Huryn** (00:49:03)

Yeah. Achievement as proof, hooks outperform, achievement as point hooks. Or... Emotional diversification Correlates with Higher Average Engagement

**Aakash Gupta** (00:49:16)

Hypothesis

**Pawel Huryn** (00:49:18)

I formulated I have not even seen them I'm seeing it for the first time This one It's the numbers 46 And it's like Not even defined So it extracts this information And yeah Every time it analyzes more posts More graphics It tries to confirm Or reject those hypotheses and at the end of the day, I have information how to write the files for X, what are the hooks that work on X, what are the accounts that we monitor, what are the rules, hard rules like probably more technical ones. and some templates that we know we have tested and we know that this template will work. This doesn't mean that it's right for me. I previously demonstrated in the newsletter that the conversation that I suggest ideas, I suggest takes, so like raw knowledge and raw opinion what I think about the specific news. but then Cloud adjusts the format, adjusts the style, adjusts the hook to the information, to the platform, and to what I'm trying to say to make it resonate with others.

**Pawel Huryn** (00:50:41)

About your posts, I'm not sure why.

**Aakash Gupta** (00:50:51)

So is the X API free that you've hooked into, or how did you, are you paying for it? I haven't seen somebody connect into it before.

**Pawel Huryn** (00:50:59)

Yeah, I am paying for X API. So in many cases, you can fetch posts for free. Like it's this FX Twitter, something like that. I'm not sure why we are seeing errors. Usually it is not the case. So this...

**Aakash Gupta** (00:51:19)

yep I saw API FX Twitter

**Pawel Huryn** (00:51:22)

yeah so this one is free but it is limited it it doesn't always work so just to save save costs the agents tries to use it by default if it doesn't work it uses this custom tool that we developed together like I just gave it documentation of the Twitter API and it created the tool for itself so it wraps this API to something that is easy to use. okay I'm not sure what one formula let me see what it told about you pure analyst voice radical topic diversity he doesn't need to stay in PM he can serve whatever wave is biggest on any given day because the mechanism reveal pattern transfer to food science neuroscience physics okay that's the his top 10 has two tech posts and eight random curiosity posts that's the opposite of Favo Lane strategy the question isn't whether to copy some hypothesis you already have it documented the question is whether the mechanism reveal voice can work within your lenses i architecture agent design pm2 link at the same scale like we have many of those conversations with Cloud Code and co-worker yeah just to demonstrate and similarly I feed it with infographics and it tries to extract some patterns that catch the attention or work in other creators we select infographics that are easy to codify as html and when they are easy to codify then we design we extract components that we can reuse and then it uses the growing library of components to design infographics for that makes sense

**Aakash Gupta** (00:53:31)

yeah it does the last component is how do you personally did it pass fetch the profile pictures of Boris and Tariq and uh

**Pawel Huryn** (00:53:41)

this one yeah but it was like a custom

**Aakash Gupta** (00:53:46)

custom

**Pawel Huryn** (00:53:47)

query like to I'm not sure what it was it was ad hoc ad hoc maybe article maybe something else let me see calendar no assets no maybe drafts no it was like a temporary artifact I asked it to create a script and go through first find so I knew the free Anthropic accounts so then I asked it to analyze their recent posts and reposts and I assumed that they will eventually retweet every other cloud code team member then it analyzed which team members used we or we just released or my team just released if it was unsure it verified the comments so that yeah just to make sure that the person was was an entropic employee and then yeah it went through like 15 people from Anthropic mapping for every feature mapping who first wrote about it. For those people we got pictures also from Twitter from X and then we iterated several times on how to visualize it so that was the final result but this is just like done by cloud code this this particularly this one was done by cloud code and this is html based on the research and the the most difficult part was the research so just getting all this information from twitter

**Aakash Gupta** (00:55:37)

yes it was difficult but in the end you were just you were talking to cloud code over hours in natural language so it's not impossible for other people to do

**Pawel Huryn** (00:55:48)

yeah i do not quote at all I don't write any code I don't even review the code if I want to know how something works I just ask questions in the chat window

**Aakash Gupta** (00:56:02)

so how do you make this system self-improving and what are the tips and tricks that people need to know around ClaudeMD files and folder structure to make their system really sing

**Pawel Huryn** (00:56:14)

okay so first a lot of people so people are discussing cloud.md file that you can put your instructions there but the problem with cloud.md is that if you put all the instructions inside it it will grow maybe not exponentially but it will keep growing and growing and growing and eventually it will consume a lot of your of your context window and every time you ask a simple prompt in your project all this CloudMD context will be included it is part of your prompt so a smarter approach is to organize your knowledge in files dedicated to specific domains and let me demonstrate mine so I have CloudMD

**Aakash Gupta** (00:57:07)

so i have

**Pawel Huryn** (00:57:09)

this main cloud md so the only goal of cloud md is to explain what this project is about it doesn't have detailed instructions or detailed information about like good practices or bad practices of what to avoid what to do more often all this information is inside the in other files and the only way a goal of CloudMD is to give those instructions how to find the knowledge and what to do with the new knowledge so project structure this is just what we can see on the left side so I can skip that like there are tools there are scripts just so the agent knows without scanning the repo another one is where things live so this is similar and by the way this was also created by cloud I didn't wrote this so I just discussed in the chat how we organize things and cloud writes instructions for itself who I am, like basic information, and the knowledge system, this is the most important part, so this is the self-organizing system where I have index of all files, like X files, LinkedIn files, Substack Files, Substack Notes files, voice archetypes, craft, so those are, this is general knowledge across platforms and then for every platform when different elements live.

**Pawel Huryn** (00:58:46)

And now, There are also workflows that the system should follow. So how to fetch data for Twitter, how to work with LinkedIn posts, how to work with Substack. The most important part is when asked to study and analyze. So every time I give it some posts, like let's study the last 100 posts or I like this one, let's analyze what made it work. It knows what tools to use, so it will extract hook pattern structure, sound bytes and engagement metrics. Only if I request visual analysis it will also analyze the attached graphic, this is to save tokens, so I don't analyze the graphics every time I analyze the post. check against the existing patterns and false beliefs and then if there is an existing hypothesis it will update the existing hypothesis with the new evidence if there is an existing hypothesis but we see that the specific post didn't work we can demote the hypothesis that the hypothesis is less likely or it will become rejected and it will append the post that was analyzed to the database so I think we may need to simplify this but basically it gets information about posts and it tries to decompose this knowledge and organize this knowledge itself into rules, into hypotheses and other elements like structure hooks, sound bites, engagement metrics and so on.

**Pawel Huryn** (01:00:40)

So the system learns itself without me telling it why the specific piece of content worked. The cloud does it itself. And the next time I have an idea, or I express opinion about something that the other person tweeted, then I can say, I like this, but I think this is connected to another idea, or for example, I like Carpati Post, but it will degrade over time, and by the way, you don't need obsidian where if the person if the user is not a person because we are building a knowledge base for agents and yeah how can we retweet that or maybe i can add some additional details and then cloud it will suggest it will use my ideas it will it will use my my take but it will format it in a way that resonates

**Aakash Gupta** (01:01:34)

so this is very content focused

**Pawel Huryn** (01:01:38)

Yeah.

**Aakash Gupta** (01:01:39)

A PM watching this might say this is kind of content focused. What's in this for me? And I don't write code. So what is the minimum viable setup for a product manager and how they should be setting this up?

**Pawel Huryn** (01:01:51)

Self-improving system that's yeah I have recently shared that and let me demonstrate it so I have actually I have a poster for this so how to create a knowledge system that learns itself and the prompt is very simple so you don't have to build everything I did you can start with just this prompt before starting a new task review existing rules and hypothesis for this domain then apply rules by default so for example if we know that so basically this is the most important part that you need to paste to your CloudMD that and this is not content specific so that whatever cloud does something in a specific domain like testing software writing marketing materials maybe writing release notes it should review the rules and hypothesis from this domain and it should apply the rules that were confirmed to its work so for example how a good test case how good user stories formatted or how how the acceptance criteria should be written or what are the good examples of release notes or customer offer whatever you do what are the good examples of something and what are the bad examples of something and it will try to extract the rules and then when you ask it to perform a task like hey you saw the 10 good examples to bad examples then let's try to create another offer for this new customer.

**Pawel Huryn** (01:03:44)

It will review the existing rules and hypothesis because you didn't write it. It reasoned what are the good rules and bad rules, what are the hypothesis from the data that it has seen, and it will also keep learning. So every time you give it a new information, it will update its knowledge, it will update the hypothesis. It can also ask you questions if this is something that were You can give agent a feedback Basically it keeps learning, keeps adding knowledge and the knowledge is organized by the domain so pricing, so marketing, testing, quality, strategy

**Aakash Gupta** (01:04:27)

Yeah so you want to create that knowledge with an index.md that has a router and in your cloud.md you want to give it this prompt so that it's self-improving

**Pawel Huryn** (01:04:36)

It will figure out what to do and every time you ask it to do something it will use the existing knowledge that is growing and every time it sees new information with the context like when I quote a tweet the tweet has some metrics like this tweet worked or didn't work or how many people liked it but maybe you can feed it with the offers that worked or with resumes of successful candidates and it will start generating those rules and the next time you will get a candidate you can ask cloud hey is this a good candidate

**Aakash Gupta** (01:05:20)

love it so one of the things that you've written about that i haven't seen a lot of people write about and maybe you can show us is the chrome mcp when and how should we be using that

**Pawel Huryn** (01:05:30)

I don't use Chrome MCP anymore and the reason is that I've been testing different approaches and Chrome MCP it's basically MCP that controls your browser it works well probably similarly to Cloud in Chrome which is an anthropic extension that you can use like this guy here you can ask to do something or you can also call it from you can schedule tasks here or you can call to Cowork and Cowork will call this Cloud in Chrome the problem with those extensions is that they rely heavily on taking screenshots and screenshots mean a lot of tokens and if you have some tasks that you want to repeat regularly or complex processes, you can easily consume like $100 in an hour especially with Opus So what I do instead is I use, let me check, but I think my agents right now use agent.dev. So what agent.browser does by Vercel Labs, this is the most reliable according, like in my tests, it also uses the real browser, but it can do that in a headless mode and it explains the structure of the page to the agent without presenting the entire HTML so this is it is token efficient and so the agent doesn't have to see HTML it doesn't have to interpret HTML but can take actions so it will see buttons with specific IDs even if the original button didn't have ID so

**Aakash Gupta** (01:07:33)

So this is

**Pawel Huryn** (01:07:34)

real browser, real rendering. It can execute JavaScript if needed. It waits for rendering, which is important. So if this single page application or there are some additional resources that load a few seconds later, it will wait for it. And yeah. It presents this page to an agent without taking screenshots. So the agent can see the text, it can see the layout, it can see different components, the content, it can say, hey, agent browser, click this button, but it doesn't have to interact with parse or interact with HTML itself. It is very simple, simple protocol. It's not an MCP, it's a CLI tool.

**Aakash Gupta** (01:08:23)

Very cool. from Vercel instead of Chrome MCP and what do you use it for exactly like what is the use case that a PM should think about this is when like

**Pawel Huryn** (01:08:33)

everything where you don't have an API to get data from external system so for example if I want to get data from LinkedIn of course I can

**Aakash Gupta** (01:08:45)

fire Chrome MCP or

**Pawel Huryn** (01:08:47)

trigger Cloud in Chrome but it will start taking screenshots every half a second or every second so it's like crazy token consumption and it is also visible in most cases on your screen so it's not something that you would like to see and with this I can just ask it to go to LinkedIn, check my inbox or analyze the top last posts by aakash and see the comments or something like that. Maybe more enterprise use case will be accessing some legacy software without API or without MCP servers. Maybe SAP, maybe some old CRM system that the agent can access just by using a web browser.

**Aakash Gupta** (01:09:46)

This is pretty epic. So as a PM, you need to hook your cloud code into absolutely everything, and you should use agent browser for the stuff where you don't have an MCP, CLI, API to hick into. Now I want to move into remote work. Anthropik shipped four remote surfaces in recent months. Web sessions, remote control, dispatch, and channels. You use all four of these remote methods. Walk us through how you actually combine them for the same project and when a PM should use WIC.

**Pawel Huryn** (01:10:19)

so the one issue with Anthropic is that those surfaces overlap and I don't use them in the same proportions so I have tested channels I have abandoned channels because I didn't see value like having this telegram interface because I have cloud I have a dedicated cloud app where I can do everything

**Aakash Gupta** (01:10:47)

okay but starting with maybe let's start with this patch so

**Pawel Huryn** (01:10:52)

this patch is a new tab that appeared in the desktop app and also on your phone and this is exactly the same so here okay I'm not sure what it is So this patch is like this single interface in which you can interact with cloud code and co-work. It is displayed under co-work. It is a bit confusing. It's a completely different product. It's like walkie-talkie. So it can start multiple background tasks and every time the task is completed it will report back what is the status so for example create an infographic in anthropic style for the following text and let me find something following text and the text will be about Bolt and Windsurf and some it's probably your work so in Anthropic style for the following text and this will be LinkedIn Resolution then I can ask it to hey how many emails in the last two hours did I receive no names no personal data and it doesn't have to start the previous task, it will just start another one and if we open the recents, I will show them, we should see that it should delegate them to other threads.

**Pawel Huryn** (01:13:20)

Three emails in the last couple of hours, so maybe it did it directly. And let's go to code. Ah, analyze akash posts. Normally it would delegate those tasks to SAP agents and you will see them as dispatch tasks in the left panel. So you can start multiple agents and use a single interface to communicate with all of them. And I can take my phone, open the, let me open the cloud app. and I will try to demonstrate that but first I will ask it are you there I'm not sure this will be visible but like I have the same interface here

**Aakash Gupta** (01:14:16)

yeah I can see it and so you can basically talk to it on web and mobile now and so there's really no excuse you're out on a walk you're at a meeting whatever it might be you're at a conference you can have your agents running for you

**Pawel Huryn** (01:14:29)

yeah

**Aakash Gupta** (01:14:30)

and what about code web sessions you said you use those roughly 60% of the time and dispatch 40%

**Pawel Huryn** (01:14:36)

Yeah, I don't remember the exact stats. I really use all three surfaces and the proportions differ from day to day, but most of the time I use dispatch and web sessions, maybe like 70% together and then 5% chat sometimes and the rest is cloud code. And the reason I use dispatch so much is that I just don't work with my laptop. I go for shopping, I go somewhere with my kit and I just dispatch tasks. I already explained that I don't code, I don't. I just provide feedback, text feedback in the chat and then co-work dispatch presents me the results. I look at the results, I dispatch another task and then I can continue what I was doing. So yeah, it really transformed my ways, my days.

**Aakash Gupta** (01:15:41)

Amazing.

**Pawel Huryn** (01:15:41)

Yeah, we have not covered web sessions, so web sessions are something different. So here in cowork, in dispatch, depending on the task that you give it, it can either dispatch task to cowork, like I asked about last three tweets and you see there is a dispatch thread here so this is something where I don't have to interact with it it's dispatch talking to this agent but it is visible for humans and similarly I can also dispatch some coding tasks from this project it will it will implement that and report back oh it even created a graphic for your post like let's say IA prototyping graphic

**Aakash Gupta** (01:16:31)

oh I want to see it

**Pawel Huryn** (01:16:35)

open like

**Aakash Gupta** (01:16:37)

whoa pretty good

**Pawel Huryn** (01:16:39)

yeah sometimes you need a few iterations but it is not the worst point to start

**Aakash Gupta** (01:16:47)

very cool

**Pawel Huryn** (01:16:50)

okay so this is the dispatch so we can think as dispatch normally you don't use it on your desktop you have the single chat single interface that you use on mobile and but sometimes for dispatch to work your computer must be online and sometimes this is not the case and sometimes there is a problem and it stops working or sometimes you have so many parallel threads that it is difficult to manage them from a single chat interface there are no tabs here on your phone you will see just one big stream of messages you cannot organize them so when I do a more complex work I switch to this code task and this is you can think of it as Visual Studio Code and Cloud Code is just in the cloud so it is hosted by Entropic so it's just a list of sessions where I can select a specific folder either my local folder or folder in github like my editor project it is synced with github so all those files so knowledge files hypothesis sound bytes hooks this is all synced with my private github repository and even when my laptop is offline I can go here from my mobile phone and ask it some question and it will it will work in the cloud without any device

**Aakash Gupta** (01:18:42)

Yep. And this is actually a more secure way to run stuff, guys, because it's in anthropic servers. So I highly, highly, highly recommend everything you build, all your operating systems, you put them into GitHub, you point them via code web sessions, and you work with stuff here. You can also, the coolest thing, as we've just showed with Dispatch, is you can start a chat here, start something here on your desktop, and then you can go to your phone. And so it's like you can be working 24-7 with us.

**Pawel Huryn** (01:19:11)

Yeah, that's correct. And I don't work at 24-7, but like I feel that my life is now much more works much, much better integrated with life. So I don't have to have these blocks dedicated to work. I can go on the shopping and

**Aakash Gupta** (01:19:30)

yeah, maybe

**Pawel Huryn** (01:19:32)

when shopping, dispatch some tasks and then check 10 minutes later when I have a graphic, provide some feedback and then continue what I was doing. so this is really transforming and when you need a better organization or when you know that you want to focus on coding like my akridia.io platform then I switch to code and I also do it primarily on mobile and yeah like in some cases I also use co-work and visual studio code but primarily this is remote most of the work is remote work

**Aakash Gupta** (01:20:11)

This is epic, guys. So hopefully you can understand how your life will change once you set all this up. I want to draw out some key lessons, Pavel, from all of the hundreds of hours you've now put into these things. Starting with, what's the biggest mistake PMs make when setting up Claude?

**Pawel Huryn** (01:20:25)

yeah I think that the biggest mistake would be to prompt it every time from scratch instead of using cloud I force myself to organize knowledge and this is very difficult to me when writing articles and but cloud can do it without effort so instead of collecting prompts and figuring out how to do something it's much easier to just to build a system where cloud can learn from its mistakes and either from your feedback or from data and it can figure out, hypothesize and figure out the better ways to do the work. Yeah, not doing that, not organizing your knowledge, not learning from mistakes and just having everything in your head and yeah, this is the biggest mistake that PM can make, just hoping that you can learn the better prompts you can there's too much data to analyze.

**Aakash Gupta** (01:21:26)

Co-work versus cloud code if a PM only had a little bit of time to learn one which one should they choose and why?

**Pawel Huryn** (01:21:32)

This is not an alternative I will start with co-work because everything you you will learn in co-work will help you better understand code I use the same repo from Cowork and from Cloud Code so for example I already presented that but once again I can select this Editor Project maybe let's remove this one and it has CloudMD it will see the same files it will so this is CloudMD that I presented in Visual Studio it will see the same files the same structure so I can ask it to analyze tweets here in this interface I can do it on my mob using this patch I can do it in Web Session, Web Cloud Session, I can do it in Visual Studio, this is all connected to the same repo. I will start with Cowork because this interface is more simple, you don't have to get used to Explorer and Terminal, it's more user friendly, you can see files, you can open those files directly here.

**Pawel Huryn** (01:22:44)

without plugins without how to display markdown or how to display html if you see html here you click html and it will show you html and in Visual Studio there are certain tricks that you must learn so I will start with co-work and just understanding how to work with agents how to aggregate this knowledge how to define your workflows and then once you feel comfortable with co-work then add this terminal aspect that in my opinion that This is more effective, should be more effective for many people than trying to learn cloud without experiencing core before.

**Aakash Gupta** (01:23:31)

What's your hot take on where AI PMs are headed? What does a PM's daily workflow look like in 12 months?

**Pawel Huryn** (01:23:37)

I doubt that in 12 months the role will disappear or something, but yeah we are heading into like super individual contributor PM and then CPO CEO at the top so I imagine that most of the time you will be working with agents orchestrating multiple like multiple agents at the same time switching switching the context it will not be easier it the work might be even more demanding but at the same time you will focus on there will be less trivial things because those can be automated like writing tickets or debugging something preparing a presentation those are the things that should be automated so

**Aakash Gupta** (01:24:29)

and eventually

**Pawel Huryn** (01:24:31)

people who develop skills from multiple areas. So like a P-shaped or even broader shaped that understand marketing, understand strategy, understand technology, understand products, can talk to customers and understand enough to delegate the work and assess the results.

**Aakash Gupta** (01:24:52)

What's overhyped versus underhyped in the cloud ecosystem right now?

**Pawel Huryn** (01:24:55)

I get the impression that people still have not realized what agents can do, especially with the right harness and with the right systems around them. I just started experimenting with that. I've been working with cloud and with agents for two years or more, but I just started to like investing heavily in automation and hardness myself and I know that I can be much more effective I doubt there is there is something that is like there's no hype there's not enough hype

**Aakash Gupta** (01:25:30)

so everything is under hyped right now guys in the cloud ecosystem go learn what we've showed you right now yeah final question for you pavel your n8n episode it did really well is n8n over I mean should everything just be done in cloud code now

**Pawel Huryn** (01:25:47)

no and then it's still relevant there are two types of there are two types of automation one automation is when you automate things for yourself like I want to analyze 100 tweets or I want to draft a response to custom email then you have this personal automation and you can use cloud code for it also we can automate specific processes inside your code base like code review or release notes or front-end design and have those sub-agents that's fine but when you want to automate production processes you The logic that I presented, this is part of the prompt. The agent can respect it, it may not respect it. All we do is edit text files within hardness that was defined by Anthropic. We cannot tell the agent that, hey, if Entropic API fails, try three times. Or for this, you should always use this tool before, you should always verify that customer email exists before doing something.

**Pawel Huryn** (01:27:07)

Or that customer has access to this data. We just create text files and we hope that agents will follow our instructions, more or less. You can add hooks, you can add some There are some exceptions from this rule, but overall, we rely on anthropic hardness interpreting our text files. This doesn't scale. This is not secure enough, and this is not effective enough for production processes. So if I want to design a system that replies to customer tickets or maybe chats with the customer, I want to have a hard guard not prompts that the customer cannot access data of another customer for example or that cannot delete data or if you want to send an email then yeah like copy a file that has one gigabyte from one place to another we don't want the agent to do that or maybe even we don't want agent to look at this data it should be handled by the code I'm not sure why you remember that we built an agent in three versions and why one was fully autonomous and we started with the least autonomous one where most of the process was code and there was one LLM call then we built a hybrid scenario and then the last version was fully autonomous and in production everything that doesn't have to be autonomous shouldn't be autonomous so we should have code we should have conditions we should have guard lies like If there is a process that should be followed it should be coded and maybe in this process there are some LLM calls for agents inside so this is more difficult to implement but it is much more cost effective and much more safe than relying on agents respecting instructions

**Aakash Gupta** (01:29:10)

So when it comes to the takeaway from our N8N episode, as we showed you guys, you want to actually be like less vague. And with these anthropic based cloud code systems right now, there's a lot of room for interpretation, less controls. If you're going to build a true production grade automation for your company, you're still going to be using N8N. You're going to be defining as much as you can. Some of those hard rules Pablo talked about. Did I summarize it correctly?

**Pawel Huryn** (01:29:35)

yes and you can also use Entropic API to to define agents in code but that's a separate story and yeah you can use Entropic API to define your workloads in code but this is not the same as organizing text files so that the agent follows the instructions we can also code code our workflows with Anthropic API or OpenAI, Agentic API or other APIs. The simplest way for a person that doesn't code is using an AN.

**Aakash Gupta** (01:30:16)

Makes sense. All right, guys, we have walked you through the AIPM tool universe in today's episode. If you haven't yet, be sure to subscribe to Pavel's newsletter. He has an upcoming quad-a-thon starting May 9th, which you may want to participate in. Check out our other episodes if you want to learn more about AI product management, N8N, or customer discovery. On

**Pawel Huryn** (01:30:40)

May 9th? So in a month? we are starting build aton cloud aton with cloud and the previous edition it was 250 students we were building Real products with NAN and with Lovable and this time we will focus on cloud code and NAN and trigger dev to build real agentic workflows so yeah I encourage you to check the program there are only 60 places in total and you can also see the gallery of the real things that our builders have shipped so this is not the theory there are a few dozens of solutions that are available to browse in the gallery and you can vote for your favorites and also understand how they were built what is the architecture and yeah even download some documents so all this is public and the next class starts next month

**Aakash Gupta** (01:31:39)

already Pavel thank you so much for being on the pod

**Pawel Huryn** (01:31:42)

thank you Akash it was a pleasure I hope you enjoyed that episode.

**Aakash Gupta** (01:31:46)

If you could take a moment to double check that you have followed on Apple and Spotify podcasts, subscribed on YouTube, left a rating or review on Apple or Spotify, and commented on YouTube, all these things will help the algorithm distribute the show to more and more as we distribute the show to more people we can grow the show improve the quality of the content and the production to get you better insights to stay ahead in your career finally do check out my bundle at bundle.akashg.com to get access to nine and many other amazing tools that will help you as an AI product manager or builder succeed I'll see you in the next episode
