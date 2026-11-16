---
title: "How to Turn Claude Code into an Operating System with Carl Vellotti"
subtitle: "What the top 1% of Claude Code users actually do differently with context management, sub-agents, self-checking skills, and a file system that makes every prompt 10x smarter."
date: "2026-03-30"
host: "Aakash Gupta"
guests: ["Carl Vellotti"]
speaker_names: "inferred"
substack_url: "https://www.news.aakashg.com/p/carl-vellotti-3"
youtube_url: "https://www.youtube.com/watch?v=Eqh2iwSl570"
duration: "01:06:48"
word_count: 14050
source: "Substack episode transcript (aired audio)"
---

# How to Turn Claude Code into an Operating System with Carl Vellotti

*What the top 1% of Claude Code users actually do differently with context management, sub-agents, self-checking skills, and a file system that makes every prompt 10x smarter.*

**Aakash Gupta** (00:00:00)

Cloud Code just hit $2.5 billion in annualized revenue in nine months. It is the fastest B2B software product ramp in history. So why are most people still using it like a chatbot?

**Carl Vellotti** (00:00:12)

Everyone says it's not about prompt engineering anymore. It's about context engineering.

**Aakash Gupta** (00:00:15)

Why are we so obsessed with managing the context? What happens if you hit the context limit? Where

**Carl Vellotti** (00:00:20)

does that data actually come from and how is it calculated is a major area where people just do not trust AI.

**Aakash Gupta** (00:00:25)

Carl Velotti has turned cloud code into a operating system. Native skills, data visualization, and sub-agents managing content.

**Carl Vellotti** (00:00:33)

When you have a sub-agent like this, what's awesome is that instead of doing that in its main session, it has spun up basically a clone of itself that is now doing all that work. So what I think is so amazing about this skill is that it actually doesn't give Cloud Code specific new abilities. All it is is it's just a really good prompt.

**Aakash Gupta** (00:00:51)

This is how most people use Cloud Code. Type a prompt and get output. Carl Vlade flipped it. He built skills that interview through a framework before building anything.

**Carl Vellotti** (00:00:59)

When you understand how Claude works, it makes it feel less like you're just prompting Claude and watching it and more like you understand how it works and you're working together.

**Aakash Gupta** (00:01:20)

where if you become an anal subscriber to my newsletter, you get a full year free of the paid plans of Mobbin, Arise, RelayApp, Dovetail, Linear, Magic Patterns, DeepSky, ReforgeBuild, Descript, and Speechify. So be sure to check that out at bundle.akashg.com. And now into today's episode. OpenAI just acquired OpenClaw, Anthropic released Cowork, and the question on the top of everybody's minds is, does Claude Code still matter? Karl Velati has been knee deep in these tools and he says the answer is yes. His last two episodes crossed over a million views across platforms and if the first episode was the beginner version of Claude Code and the second episode was the advanced masterclass, today is the operating system layer. If you're already an 80 out of 100 on cloud code, we're going to bring you to a 95 out of 100. And if you stay till the end, you will understand context management, creating sub agents to manage your context for you, auto triggering skills and building an operating system around it all.

**Aakash Gupta** (00:02:22)

So let's get right into it. The question on the top of everybody's minds is, should they still be using cloud code in a world of co-work and open claw? What do you think?

**Carl Vellotti** (00:02:29)

Yeah, so a lot of these new tools, they're amazing. Cloud Code was the first, kind of the most powerful where all of the everything else is built on top of. You have tools like Cowork, which is basically it's a UI that builds on top of Cloud Code that tries to make it easier to use. And it's good for the for the use cases that it does have of like managing files and things like that. It is a good tool, but ultimately it is built on top of cloud code. So all of those features, they exist in cloud code first in a more powerful way. And then they kind of get constrained by co-work. So if you want the most power just to be able to do things and do work, cloud code is still it's still the number one tool. And I would say with OpenClaw, it's a lot like Cloud Code, where essentially it is a way that you can connect to Cloud Code or a Cloud Code-like service from other channels.

**Carl Vellotti** (00:03:21)

You can have it running all the time. It's really good for monitoring and tasks where you really can let it run autonomously. But if you need to be in the loop and you need to be in the driver's seat and you really want the most power in the tool, then you don't really do that in OpenClaw. You do that with Claude code and then you can set up OpenClaw to do some of that monitoring type of work. But if you need the person doing the most powerful work that you can, you really you have to be in Claude code.

**Aakash Gupta** (00:03:47)

Yeah, for product managers where you need to be the driver's seat, AI still can't do the thinking for you. CloudCode is still going to be the tool of choice. OpenClaw is really cool for living and having the heartbeat feature and being able to chat with it. But CloudCode is still the most powerful. Both you and I have been living in CloudCode pretty much eight hours, 10 hours a day for the last six to eight months. And we've encountered four major friction areas that we're going to help people solve in today's episode. If they listen to the whole episode, what are they going to learn?

**Carl Vellotti** (00:04:17)

Yeah, so when I kind of look at our first two episodes we've done, we did kind of an intro, we did advanced, and I would consider this one the mastery course, where you're really good at using cloud code, but there's still another level deeper that you can go to solve the biggest problems that you might have with cloud code. So the first is just context management. How can you make it so that your context window doesn't fill up so fast and then you have to wait and compact and then you do a couple more messages and it compacts again. So what are some strategies that you can really manage context to use cloud code just way more effectively and not have to wait

**Aakash Gupta** (00:04:48)

as

**Carl Vellotti** (00:04:48)

long? The next one is just figuring out how can you use skills to shore up other major weaknesses of cloud code. People will say cloud code is not very good at research. They'll say it's really not that good at UI design. They'll say that... it really can't design slides and things like that very well on its own most of the time what you need to do is you just need to figure out how can you provide the tool that cloud code can use to do those things better so just shoring up all of those weaknesses with skills and then we'll answer one of the biggest questions that people have when they're working with ai which is how can you trust the results for a lot of people it They don't really need AI to just be able to do tons of mass produced work, you know, for product managers or people where they're really accountable for a very small number of documents.

**Carl Vellotti** (00:05:35)

They don't need lots of work to be done. They just need the work that they do do to be very high quality and very trustworthy. And so today we'll look at an example of how you can do that with data using cloud code where you can know exactly how it got its answers and that you can reproduce them. deterministically every time. And then we'll put all of this together. And that's kind of like the last major question that people have about Cloud Code is, okay, it can do all these things, but how do you actually put it together in a cohesive system so that when you're using it, you're not just kind of having files go all over the place. So really today I would say is taking all of that Cloud Code knowledge and Cloud Code usage that you already have and just taking it to the absolute next level with giving Cloud Code its own skills inside of a really strong operating system.

**Aakash Gupta** (00:06:19)

I'm so excited for this. It's going to improve my own cloud code usage. So show us the sauce. How do we handle context better?

**Carl Vellotti** (00:06:25)

Yeah. So the first thing to do, and this is kind of like a fun little trick that I just recently learned, is you can actually, there's a lot of different elements of the cloud code UI that you can actually customize. and so right here uh and just kind of a quick note on the setup we're in cursor here but we're not using any cursor features we have cloud code open here on the side and we're using the cloud code cli and uh we'll just use that for this entire podcast so the first thing i really want to show is uh there's something that you can customize calls the status line and so you can actually have cloud code show you how much context you've used at any given point throughout a conversation And what's nice is that you really get a much better sense of how is your context filling up?

**Carl Vellotti** (00:07:08)

What types of requests are filling up the context? Where is it getting eaten into if you just set this up? So the first thing to do is just set up a nice status line. And it's incredibly easy to set up a status line. There is a slash command called status line. And I'm just going to go ahead and just put in a really nice one. So there's a bunch of different things you can include in this status line. So here we're going to have it show us what model we're using right now, what folder are we in, and then make a little UI for the amount of context that we've used so that we can visualize it as we go. It's almost like a tiny little piece of software or a tiny little UI where you can have it like when you have a lot of context left, it's green.

**Carl Vellotti** (00:07:51)

When you have a medium left, it's orange. And then when you're almost filled with your context window and CloudCo is about to compact, it turns red. And this is something I discovered from another plugin we'll look at later. But it's incredibly easy. And you can just literally do slash status line, explain what you want, and Cloud will build it into its UI right there. So we're about to see that. We see here it spun up its own custom sub-agent called Status Line Setup and is now going ahead and building that. And if you see just a second ago, we had nothing under here. And now we have this status line that we just described. So we have, it tells us that we're using Opus 4.6. We're in this demo file that will be available to anybody that watches this video. And then this is how much context we've used.

**Carl Vellotti** (00:08:31)

So we're only at 20% and we're in the green. So number one thing, set up a nice status line, and then that will help you really kind of learn about how to use context as you put in different prompts.

**Aakash Gupta** (00:08:44)

And for people who maybe haven't encountered this issue, right? Why are we so obsessed with managing the context? What happens if you hit the context limit? Doesn't it just auto compact? Isn't there no problem really?

**Carl Vellotti** (00:08:55)

Yeah, that's a good question. First of all, I would say the compacting is kind of one of the worst things about using cloud code, especially if you give it like a long task, like, hey, can you go research this thing for me? And then it runs a bunch of web searches. And every single time it uses a tool call and every time it reads a web page, it's eating into that context window. And so if you have a bigger project where you're working with a lot of files at once, It's easy for this to get to 100% with just like five messages. And then you're waiting a long time. You're waiting two or three minutes for it to compact. And it can just really get in the way of your flow of using the tool. So avoiding that is, for me personally, That's why it's helpful to kind of have the context get used up slower.

**Carl Vellotti** (00:09:36)

But the real kind of the real even like bigger and more important lesson is that as I've been using AI more and using cloud code more, I knew this before that everyone says it's not about prompt engineering anymore. It's about context engineering. But that's just absolutely, it's kind of the golden rule of using these AI and using these really powerful tools. They are able to work with the information that they have. And so you want to make sure that they're only having the information that you actually need them to have, but that when they need that information, it's kind of everything that they could possibly use. And so you can, if you're limiting the things that they don't need, then it provides a lot more room for you to include the things that you do need. And the overall quality just really dramatically goes up.

**Aakash Gupta** (00:10:18)

Exactly. And I think that there's still this phenomena of context rot, which has been measured, which is that as you get longer into the conversation, the quality degrades. And as you use up your context window, you're going to see that happen. So you actually want to give AI minimal amount of context to actually have it understand what you want it to do. Exactly. Exactly. Here's the dirty secret about prototyping. You spend two weeks building a prototype. You validate your assumptions. Engineering loves the direction. Then what happens? You throw the whole thing away. Bolt changes this completely. When you prototype in Bolt, you're not building throwaway mock-up. You're building real front-end code that integrates with your existing design system. So when you hand it to engineering, they don't throw it away. They ship on top of what you've built. I use Bolt every single day. I host my LAN PM job cohort on it.

<!-- sponsor -->
**Aakash Gupta** (00:11:07)

And honestly, I'm up till 2 AM some days just vibing in the tool, having fun, and building. That's when you know a product is good. When you're using it past midnight, not because you need to, but because you want to. Check out Bold at bold.new slash akash. That's B-O-L-T dot N-E-W slash A-A-K-A-S-H. Link in the show notes. Today's episode is brought to you by Amplitude. Replays of mobile user engagement are critical to building better products and experiences. But many session replay tools don't capture the full picture. Some tools take screenshots every second, leading to choppy replays and high storage costs from enormous capture sizes. Others use wireframes, but key moments go missing, creating gaps in your understanding. Neither approach gives you a truly mobile experience. Amplitude does things differently. Their mobile replays capture the full experience. Every tap, every scroll, and every gesture with no lag and no performance hit.

**Aakash Gupta** (00:12:00)

It's the most accurate way to understand mobile behavior. See the full story with amplitude.

**Carl Vellotti** (00:12:06)

And so one of my favorite ways to do that. So again, this was just setting up, okay, now we have an idea of where our context is. So of course, you can always just do the nuclear option of clear. So that basically starts a new session. So the most effective way, and I have been using Cloud Code for months and months, but I honestly only just realized in the last few weeks how amazing sub-agents can be for controlling context. So as an example, so right now, one thing you can always do is you can run, let me get rid of this. Ah. okay one thing you can always do is you can always run slash context and that will show you where is the context of claude getting eaten up and so right now we see i have a couple things already enabled so i have um right if you go to the top it gives you like your overall summary so here we have 16 of our context is used which is crazy that's just i haven't done anything we just cleared so 16 is just eaten up for doing well for me let's see what is taking it up So the system prompt, which you can't really get rid of, that's just like part of cloud code.

**Carl Vellotti** (00:13:05)

So that's taking up 2%. And then all of my tools that I have enabled right now, I have some MCPs, some custom agents, all of this together is taking up another 8%. And then I have a bunch of these, like right now I have cloud and Chrome enabled. So this is one thing just right off the bat. Do you have a bunch of stuff that's turned on that you don't actually need? And then you could go through and turn it off. So that is like the quickest way to just make sure that you're not eating up all your context. Yeah. But let's go through an example here. So let's just give Cloud a task where we're going to see it eat up a lot of its own context. So we just saw right now to start this off, we're at 16%. So I'm just going to run a pretty normal command here, which is research the top five Cloud code tips from this week.

**Carl Vellotti** (00:13:49)

So when we ask it to do that, actually, I do have one tool turned on for search, which we'll use later, but I'll turn that off for now. Okay, so let's go ahead and run that again. So research the top five cloud code tips from this week. And so what is Claude going to do here? Well, it's going, it has a web search tool and it has a web fetch tool. Oh, okay. It's getting ahead of me here. It's what it's doing here and what it's decided to do is it's decided instead of running that search on its own, which is oftentimes what you do, or if you ask it to do a task without telling it specifically to use agents, then it will just start running that prompt and then it will kind of Do all of that in your chat session and it will eat up a lot of that information or a lot of that context window that it has just doing the searches and then just getting the results and then summarizing them.

**Carl Vellotti** (00:14:40)

Yeah. But when you have a when you have a sub agent like this, what's awesome is that instead of doing that in its main session, it has spun up a like basically a clone of itself that is now doing all that work. And what we're going to get back here in our main session is we will just get the summary of it. So you save your main session from having to do all those tool calls and read all the information and then just get the summary. And so that right off the bat, if you can remember to use Claude or tell Claude to use subagents to do its work instead of having it do it in its main thread for many things that will automatically just save a lot of its context because it's just getting the result instead of all of the work to get that result.

**Aakash Gupta** (00:15:23)

And to implement this agent, I believe it's two parts, right? In your ClaudeMD, you tell it what you just told it, use subagents to use your work, and then you create the subagent, the research agent, correct?

**Carl Vellotti** (00:15:33)

So yeah, great question. So Claude can do two things. One, it can either just make it on the fly, make a new instance of itself and give it a task, which I think is what it did here. versus earlier when we saw it do that, the status line, that's like a dedicated sub-agent that is already sort of defined of how it works. And sometimes it can also use those. So those both work. If you don't want to take the time to like actually define a sub-agent, this will work for even just like on-the-fly tasks as well. Awesome. Okay. So here what's cool is we have the result here and let's go ahead and look at our context from when we started. We had 16% to begin with and now... we're only at 16.5%. So if we did this type of thing without doing that, and when I was testing this on my own, it would fill it up to 25%, which is a lot for just a basic web search, right?

**Carl Vellotti** (00:16:26)

And the other thing that's really cool is that we saw it run this search and it kind of reports back on exactly what it did. It ran 10 tool uses and it used almost 30,000 tokens. So all of that information is saved from our main session because we had it use this subagent.

**Aakash Gupta** (00:16:43)

Nice.

**Carl Vellotti** (00:16:44)

Yeah, so that's a good one. And this is where I would say it really starts to feel when you can kind of understand how does cloud code work and where are its weaknesses. It should dynamically create these agents. And we actually did see it do it here. Oftentimes, it will not do it when it would be a good idea. And the kind of like mental framework to have in your mind is, do you need this main session to do all the work? And so sometimes if you're like coding something or you have like a specific question, it's helpful for it to have all the context of like all those files so that you can ask it something directly and it doesn't have to see what its agents did and then pull that context in. But here, when you understand how Cloud works, you can kind of tell it how to operate itself, which really just levels up and it makes it feel less like you're just prompting Cloud and watching it and more like you understand how it works and you're working together.

**Aakash Gupta** (00:17:32)

Love it. So I assume you could just say something like use a research subagent in the prompt if you want to force it or it hasn't done it and it's doing the context filling up way. Is there a skill or something we should be using to further encourage Claude to use subagents?

**Carl Vellotti** (00:17:48)

Yeah, great question. So in fact, I do have in this in this file, I have a skill called spin up, which it's kind of the lingo is that it spins up at sub agent. So sometimes when I'll be giving it a long task, I can say, you know, research all the top cloud code creators. in the world and i'm sure you would come up and then we can just add to the end of this spin up so instead of saying please make sure you use dedicated sub agents we have this rule here where um basically it'll run the skill of spin up and then it knows that it should parallelize that and use a sub agent instead of doing it itself so that's just kind of a shortcut to make this quicker

**Aakash Gupta** (00:18:28)

nice can you just show us the rest of the spin-up skill once we execute that

**Carl Vellotti** (00:18:32)

Yeah, so let's go ahead and run it here, and then I'll make this bigger. So spin up, so set up a new product. Sorry, what this says. When the user runs spin up, you help them configure. Oh, sorry, this is actually not quite what we would want. Okay, so this is a good opportunity. So let's stop this. So this spin up command, I think, has some stuff that we don't want.

**Aakash Gupta** (00:18:53)

For people who are wondering how you stopped it, You hit.

**Carl Vellotti** (00:18:56)

Yeah, great question. So and yeah, and this is where you just when you really get familiar with the UI. So escape will stop it. And then one thing you can always do is you can always hit escape two times. And then that will give you all of the messages that you've done. And this is also actually another way to like kind of save context. If you if you ask a question and you realize it was the wrong question, instead of having that in the memory or if it did a bunch of stuff wrong, you can always just roll back to earlier. And then that will just get rid of all of that. And it just puts you right back in there with that exact same sort of wherever the context window was at that. So anything that you roll back and you erase is literally completely gone.

**Carl Vellotti** (00:19:31)

So you have to be a bit careful. Make sure that you do that. And it wasn't something you maybe wanted, but it's a good way to kind of continue to conserve your context window.

**Aakash Gupta** (00:19:39)

So I think we're going to fix the spin-up age skill now and show people how to edit skills. Yeah?

**Carl Vellotti** (00:19:44)

Yeah, let's do it. So we know what we can do. We'll just go ahead and delete the skill because it actually has some stuff that's a bit wrong. So we'll just delete it and we'll show how can you make a skill with clock code. So please make a new skill that helps me. tell you when you should use dedicated sub-agents instead of the main session to preserve your context window.

**Aakash Gupta** (00:20:12)

Nice. And you guys see how easy and natural language it is? Skills is the unlock. Like Carl said, whenever you feel like there's a weakness, in this case, there's a context management weakness, spin up a skill. And now it's going to write its skill for itself.

**Carl Vellotti** (00:20:26)

Yeah, exactly. And so now it's looking at the existing skill structure. It'll make sure it matches the format. And Anthropic recently made a nice change where you used to have to restart Cloud Code for it to pick up skills that you made. But now it'll actually, it should just pick it up directly in here. And I didn't tell it what to call it, so it's going to come up with its own name.

**Aakash Gupta** (00:20:45)

Oh, yeah. It won't be Splash spit up anywhere.

**Carl Vellotti** (00:20:47)

Yeah.

**Aakash Gupta** (00:20:48)

I think this is now a good time to warn people, don't download too many skills from random skill marketplaces. especially if you're probably running Claude Dangerously skit permissions. There have been a lot of malware and prompt injection attacks in those skills that people have been analyzing online. So it's generally best if you're going to get a skill, get it from me or Carl, somebody you super trust or just create them yourself.

**Carl Vellotti** (00:21:14)

Yeah, exactly. Your own skills are good. And then we'll look at one other marketplace that Vercel recently came out with. It's maybe not perfectly safe, but it is a pretty well-validated marketplace. But yeah, I think most of the benefit from skills is you know your own workflow. Once you've seen that you're repeating something multiple times, then it's time to make a skill and it will be customized to your exact project. Mm-hmm. So let's see, it came up with one called context guard here. Before starting any non-trivial task, evaluate whether it should run in the main session or be delegated to a sub-agent. So let's try this again. So we had our question from before, which was research the top five cloud code tips from this week. And then let's ask it to use context guard. Context guard. There

**Aakash Gupta** (00:21:58)

we go. In the last episode, we sometimes had trouble triggering skills. It's best to just have this invocation with a slash command or use context of garden skill in your prompt so that you don't run into the issue of it sometimes not using it.

**Carl Vellotti** (00:22:12)

Yeah, exactly. I did figure out how to fix that. So we'll cover that. We'll cover that quickly. But the most surefire ways, you know, know your workflows, know the skills that you have. And then, yeah, just use them when you need them. OK, so it looks like it went ahead and did it. It said applying the context card. This is a web research task. High context, multiple searches, page reads, delegating to a subagent. So now anytime that we need to do this type of thing, you can just run this run this command context guard and that will preserve your main session a lot. And again, the rule is, do you need the main session to know it? No, we don't need it to like see what all of the web results like web search results were. We just need to know what the final output is.

**Aakash Gupta** (00:22:51)

This is fire. So how do we fix the skill invocation issue?

**Carl Vellotti** (00:22:55)

We'll get to that in one second. Um, the other things to show that are good is so while this is running, one thing that's cool is when you have a subagent running is here, it says use control B to run in the background. So I'm going to do control B and what that will do is it actually now, uh, if we see down here, it says, um, one. one local agent. And so we can go and see what that's doing. But now it's kind of nice because we can actually just continue our main chat while that's running so that we don't have to wait for it. And so this is really nice if you have like a bunch of stuff running in the background that you're not like immediately dependent on the results. You can have that agent run in the background and then you continue your conversation.

**Carl Vellotti** (00:23:32)

And then as soon as this local agent finishes, it will kind of inject itself into the chat and then Cloud Code will read what it came up with.

**Aakash Gupta** (00:23:40)

Nice. And you just clicked on the local agent to see that, right?

**Carl Vellotti** (00:23:43)

So I just navigated it down and then hit enter. Ah, down and enter. Yeah, cool. And so here we see what it's kind of cool, too. You can see, like, what was the initial prompt that Claude gave to it. And then we can see it's fetching and searching. When it's done, the next thing I want to show is my absolute favorite Claude Code feature. It's like my absolute favorite. I like subagents. I think they're probably my second favorite feature. My absolute favorite feature of Claude Code is the Ask User Questions tool. have uh do you have you used it you find yourself using it

**Aakash Gupta** (00:24:11)

actually no oh really okay this is i feel like i'm missing out i feel like this is why i love recording these episodes so i can learn the latest alpha

**Carl Vellotti** (00:24:20)

Yeah, the Ask User Questions tool is so awesome. So what we're going to get back here whenever this finishes, it's being very thorough, is we'll have this big list of cloud code tips that it found from the internet. And then let's say that we wanted to implement some of those into our system. Then normally we'd have to read them and we'd have to say, OK, can you tell me about this one? Can you tell me about this one? Or how can we implement this? So we got these five top cloud code tips. So now what we're going to do is we're going to say, please use And then the magic phrase here is just ask user questions. I don't think it has to be in one word, but that's kind of like the official way that it is. So ask user questions tool to help me see if we should implement any of these.

**Carl Vellotti** (00:25:07)

And what's so cool here is that Claude will now go through that and it will dynamically come up with a list of questions to ask us, but it will be in like a new custom UI within Claude code. So what we see here is it says, which of these Claude code tips would you like to implement? And so it's giving us these in like a UI. So we can say, OK, I want this one and I want this one. And then when we hit Submit, it will now have that in its memory and it will be able to go through it directly. This tool, I just use it all the time. Like if you are coming up with a list of requirements for a feature, then you can say, please use your Ask User Questions tool to grill me on all the possible requirements for this spec so that we can fill all that in.

**Carl Vellotti** (00:25:48)

And what's so awesome is that this will kind of take it from where Cloud Code is The main reason that people don't like the output from AI is because there's just so many assumptions and so many things that it gets wrong because it really didn't have that in its context. But if you have it ask you, it will predict like, where are my weaknesses that I have? Or where are the assumptions that I'm making that I need from the user? And it will ask you questions. And if you really make it strong, like a strong prompt, like, please ask me as many questions as you possibly can. It will just keep asking you. And sometimes it'll be like 10 or 12 questions or something. I know one person on Twitter said that it asked them 67 questions. So they probably had a very vague starting place.

**Carl Vellotti** (00:26:26)

But it's just this really nice way to be able to work with Claude directly in this session rather than... Otherwise, it's actually pretty hard to answer questions. They might do one at a time or might ask you a bunch and then you can number them in the chat. But this is just this beautiful UI that it will do right here in Claude code, which I love this feature.

**Aakash Gupta** (00:26:44)

I like it. So it's sort of like that idea that you're not engineering this massive prompt or building this massive skill to solve the problems for you. You're saying, please ask the user question if you need clarification.

**Carl Vellotti** (00:26:57)

Yeah, exactly. And you can use it in all different kinds of ways. You can say... hey, I have the spec, use your ask user questions tool to like shore up any areas where you think might be unclear. Or we're about to start this project, use your ask user questions tool to ask some clarifying questions, things like that. So really just like anytime it would be helpful for the AI to get more context to help you have a better output, use that tool and then you can just do it right there. And it's just so nice. It's just right there in the chat, better than anything else I've seen. I would say it's one of Cloud Code's like most probably creative features.

**Aakash Gupta** (00:27:31)

Amazing. So what other skills should people be creating?

**Carl Vellotti** (00:27:35)

Yeah. So I would say in general, whenever you're kind of like going through your workflow and you realize you're doing the same thing multiple times, that is a great time to add a skill. The other main time I would say it's really good to figure out how can you build a skill or how can you find a skill is areas where you think cloud code is really weak. Then you might be able to just come up with like a prompt or skill that gives it the tools or just the knowledge it needs to do much better work. So an example here, if you type slash plugins, it will show you kind of like the overall Cloud Code marketplace. The kind of most the most safest possible skills that you can have are, of course, Cloud's own official plugins. One of the most impressive of all of the skills I think that people have talked about is so Cloud has they have 56 of their own plugins is this front end design skill.

**Carl Vellotti** (00:28:24)

So, you know, it's very commonly talked about that. AI always makes this sort of purple gradient generic kind of UI, right? If you just say, please make me a landing page like this. And I actually have a really good example. When we, let me open the browser here. When we did our first episode, I kind of did like a small lead magnet so that people could get the code that we did from that. And then I now have a cloud code for everyone as my main thing, but I had a cloud code school. So this is a real example. I actually shipped this. This is a real live page right now. This is the kind of output you get if you say, hey, just make me this. And this is just incredibly AI, right?

**Aakash Gupta** (00:29:07)

Yep. Screens written by Claude.

**Carl Vellotti** (00:29:10)

Yeah, you just know. But I also, for our next version or our more advanced one, I had it use its front-end design skill, and this is what it came up with, where it's just much cleaner and nicer and feels, you know, it's still... you know, still a classic kind of web page, but now it just has so much more personality in this than the first one. So I would say this is a perfect example where, okay, I think AI is bad at this. Well, maybe all you actually need is a skill. And what's cool about this skill in particular. So let's go ahead and look at it. We'll have Cloud Code open it up for us. There's a couple different ways that you can approach skills. So what I think is so amazing about this skill is that it actually doesn't give Cloud Code any specific new abilities.

**Carl Vellotti** (00:30:00)

All it is is it's just a really good prompt. I'm going to have it open it for us here in cursor. One thing that's interesting is when you install a plugin or you install something from the marketplace, depending on how you have it configured, it's not actually in this repo. It's kind of like at the computer level. So we're not seeing front-end design over here in skills. It's like a couple levels back. But this is what we have here. It just shows like this is what all skills have, which is their name and then their description and when they're supposed to be used. But this is just the prompt that Anthropic has come up with to tell the AI just better rules for how to do front end design. So like think about the purpose of what you're building. Make sure that you have a clear conceptual direction.

**Carl Vellotti** (00:30:46)

Here's the aesthetics. And it basically tells it to don't be AI. Instead, follow these rules. And so I think it's good just to show you can have an incredibly powerful skill. that doesn't have any MCPs or APIs or any code with it, just a really good prompt that you perfect over time can make a really, really good skill.

**Aakash Gupta** (00:31:05)

Although skills with tools are pretty powerful, right?

**Carl Vellotti** (00:31:08)

Yes. Skills with tools are definitely more powerful. So that's what we'll look at next.

<!-- sponsor -->
**Aakash Gupta** (00:31:13)

Today's podcast is brought to you by Pendo. Welcome to the SaaS plus AI agent era, where every product team, no matter the size, can build world-class experiences. Meet Pendo AI agents, virtual teammates that read your product data, chat with users, and take smart in-app actions so you don't have to. With Agent Analytics, Pendo shows exactly how those agents drive adoption, complete tasks, and even cut churn. No extra engineering lift, fully SOC2, and HIPAA ready. And because Pendo's behavioral insights sync straight back into your BI stack, you get AI-ready data to fine-tune models and prove ROI in one place. Smaller team, bigger ambitions. You no longer need an army to deliver software your customers love. Grab early access at Pendo.com slash Akash. That's P-E-N-D-O dot com slash A-A-K-A-S-H. Today's episode is brought to you by Naya One. In tech buying, speed is survival. How fast you can get a product in front of customers decides if you will win.

**Aakash Gupta** (00:32:14)

If it takes you nine months to buy one piece of tech, you're dead in the water. Right now, financial services are under pressure to get AI live. But in a regulated industry, the roadblocks are real. NIA1 changes that. Their air-gapped, cloud-agnostic sandbox lets you find, test, and validate new AI tools much faster. From months to weeks. From stuck to shit. Thank you for listening. making hundreds of thousands of dollars more, joining OpenAI and Anthropic, then you might want to do a course that I've taken myself, the AIPM certificate ran by OpenAI product leader, McDad Jaffer. If you use my code and my link, you get a special discount on this course. It is a course that I highly recommend. We have done a lot of collaborations together on things like AI product strategy. So check out our newsletter articles if you want to see the quality of the type of thinking you'll get.

**Aakash Gupta** (00:33:19)

One of my frequent collaborators, Pavel Hearn, is the Build Labs leader. So you're going to live build an AI product with Pavel's feedback if you take this AIPM certificate. So be sure to check that out. Be sure to use my code and my link in order to get a special discount. And now back into today's episode.

**Carl Vellotti** (00:33:35)

is there's kind of two ways that you can power up your skills. The first one is just you make a skill and in that skill, it tells Claude to use like official tools. So in this repo, I have a skill called web research. And so Claude, if you just have it do a general web search, like we did earlier in this uh demo where we had to look up the top five um cloud code tips from the week those results that cloud code gives are just notoriously unreliable um one it's basically just running google searches and it's just grabbing stuff from the first page and i think you kind of know if you're just searching stuff on google and you're clicking the first links you have absolutely no idea if those are actually good links i think uh Pre-AI, the internet was really starting to feel just like so much SEO generated slop, even before there was AI slop.

**Carl Vellotti** (00:34:28)

And do you really want that to be in the context window for Claude? So I would say this is another example of where people say, oh, you can't really trust Claude to do reliable research. Well, again, this is an area where if you just give it better tools, it can actually do better research. Mm-hmm. And so in this skill, basically we have it connected to two tools. One is an MCP called Tavali. I'll zoom in here. MCP called Tavali. So this is really good. It basically is just like a much more powerful, almost perplexity type of search that gets much higher quality results than just a classic web search. And so here we're turning it on. It's a very generous free tier if anyone wants to try it. And then what we also have in this skill is we have it connected to something called Firecrawl, which Firecrawl basically is once you have a URL that will scrape it and get really clean markdown.

**Carl Vellotti** (00:35:25)

And so it's a nice way where normally when you go to a website and Claude looks at it, there's a bunch of extra HTML and like maybe JavaScript and things like that. Firecrawl will just get just the sort of like raw information that the AI actually needs without all of that other stuff. And one thing that's cool about this is that Firecrawl is actually, the way I have it set up, is actually not an MCP. So if we look at the MCPs I have set up here, MCPs are good, but as we saw earlier when we were just looking at our context window, they eat up a lot of context just right off the bat. Like if we look at our context, we see that... Tavali is taking up like a couple thousand tokens just by existing versus what you can also install are CLIs. So a CLI is kind of, it's interesting.

**Carl Vellotti** (00:36:12)

It's kind of like an older technology. It used to be the way that you would operate a computer in the beginning with a command line interface. And they kind of fell away, of course, with people wanting like better UIs for most things. But AIs are really, really good at using command line interfaces. And essentially what they are is it's like you have a tool and then you download it onto your computer. And so it's just sitting on your machine. And then the AI can use the command line directly just through because we're basically in the CLI here. And so you have all the power of that tool just installed on your actual machine. So that when the AI wants to use it, it doesn't actually have to have context just holding it in there. It can just use that CLI directly from your machine. And so what we're seeing is, you know, originally there was MCPs, but I actually think MCPs are kind of starting to be the less preferred way over CLIs.

**Carl Vellotti** (00:37:01)

And most tools already had CLIs and there's becoming a lot more. So for example, if you've ever tried to connect the Google Workspace MCP, I actually tried to do that on another podcast live and it's just it's such a hassle. But there's actually a Google Workspace CLI. And that's what, for example, OpenClaw uses. So it's just way more reliable than using an MCP because it's just on the machine and it's easy for the claw to figure out how to use it. And I think what we're going to see in the next over the next year is just a lot more CLI tools because AI are so good at using them.

**Aakash Gupta** (00:37:33)

Yeah, Andre Karpathy said it himself, like you should prefer a CLI connection. And I think the hierarchy is basically MCP at the bottom because it eats up so much context, then API, CLI at the top. And funny enough, CLI is basically just usually a wrapper on top of the API, but agents like to work with CLIs.

**Carl Vellotti** (00:37:52)

Yeah, exactly. The other CLIs I would say are just awesome. GitHub CLI, I would say basically mandatory. If you're really doing anything with GitHub, the CLI cloud is just aggressively competent at the GitHub CLI. It's amazing. And the Vercel CLI is another really good one where if you want to deploy your app, then it can check the logs. It can configure your environment variables. Those two, if you're doing any vibe coding, if you have the GitHub CLI and the Vercel CLI, so much easier, so much more powerful.

**Aakash Gupta** (00:38:23)

I think this is one of the most underrated hacks. If you take anything away from this episode, stop using MCPs, start using CLIs.

**Carl Vellotti** (00:38:31)

Yeah. And just literally, if you just say, hey, Claude, does the CLI for this exist? More often than you'd probably guess, the answer is yes. And just download that and use that because it's just so powerful. So what I did is I went ahead and ran our web research, which uses Tavali to find stuff and then Firecrawl to kind of scrape the pages. And this is, again, a really good way to shore up that web search is not that good for AI. But if you give it access to these tools, it can be way more powerful. but then I have those wrapped into a scale.

**Aakash Gupta** (00:39:02)

Amazing. So we covered front-end design, web search. I think the other thing people talk about is making slides.

**Carl Vellotti** (00:39:08)

Yeah. So another area where if you just say, if you just tell Claude, hey, can you, like if it's something, web pages are, I think, easier for Claude to understand. There's tons of web pages in its data, so it kind of knows what they're supposed to look like. But if you ask it to do something like make a graphic for this or make a slide for this, then, and you look at his result, They're usually not that great. Like they're usually not laid out the best. There's usually like alignment issues that could be better or like the space isn't filled very well. So one of the best things that you can do, and this is, again, all across the theme of just, okay, well, I'm saying that Cloud Code is bad at these things. But for example, what a lot of people will do, and you might find yourself doing this, is to say, okay, please make a slide in HTML that covers,

**Aakash Gupta** (00:39:51)

you know,

**Carl Vellotti** (00:39:51)

this thing. And then it makes it, and then you screenshot it. And then you say, hey, can you fix this, this, and this? And then it does it again. And you say, hey, can you fix this, this, and this? Instead of you doing that, think, can I give Cloud Code a way to check its own work? And that is just a huge unlock for anything that you're doing with visual design with AI, is give it a way to see its own work. And so what we have here is we have a skill called Make Slides. And this is a bit more advanced. So, so far we've had just words and then we had words telling it that it has access to a couple of tools. This one actually has a code in kind of telling it how to use code in the skill so that when it runs the skill, it will now know that it can run that code to help it check its own work.

**Carl Vellotti** (00:40:35)

So here we have our make slides skill. It tells it like, OK, I want to tweak these dimensions. I want it to have these layouts. So this is similar to the front end design skill we saw. But what's new is that there's an actual build process. So it's step one. And it's telling it that kind of the different types of code that it can use. And it's saying, hey, you can measure overflow. So it's using a tool called Puppeteer, which is like a very classic front end development tool. So you can take screenshots of HTML pages just exactly as they look when they're rendered. And we're saying, hey, you have access to Puppeteer. Use it in this particular way. So it's telling it like the dimensions that it should grab. And then it's doing a calculation here to see, does any of this text fall off the page?

**Carl Vellotti** (00:41:18)

And that's a thing that if Claude doesn't have a tool to check it, to check that, it can't really do it on its own. But with a tool, it can do it basically perfectly. And so that's what this skill does is just embeds that code-based tool directly in the skill so that when we say, hey, make a slide, it will run these tools that it knows it has access to.

**Aakash Gupta** (00:41:38)

So this is the implementation of the advice when I asked Carl the question, what skills should you make? And he said, well, anything that's coming up in your workflow. If it's coming up that you're iterating on these slides by having to look at it, build a skill. And now you guys are seeing the most advanced way to build a skill with the code in it.

**Carl Vellotti** (00:41:52)

Yep. And so here I said, use your make slide skill to make a single detailed slide for a presentation called from watching, collaborating, kind of the theme of this. And so now what it's going to do is it's going to go ahead and create that screenshot itself, calculate. And then one thing I found is if you just say like, you must iterate three times before you show me, it'll be much better than if you say, oh, just go until you're done. I would say this is an area where you really see AI just really have like great taste. You know, if you give it an infographic that just has tons of information on it, they're like, wow, this is so amazing. But the actual content or the layout might be terrible. So it's helpful to just say, hey, you have to improve it three times and then it will find some ways to try doing that.

**Aakash Gupta** (00:42:34)

Yes. And there's also this crazy phenomena where if you repeat yourself with your skills, the AI does better. There was just a Google paper released where they showed that literally just pasting in a prompt twice helps. And this is, I've been using this in almost all my skills these days. I'll say, after I execute it once, I'll say, go double check against the skill again, and it really improves it. And so Carl's technique is a way to sort of encode that so that it builds it into itself.

**Carl Vellotti** (00:43:01)

Yeah, that's super interesting. I've heard that called the builder-validator pattern, where when AI just runs its own work, it doesn't really have that self-reflection to really know if it did it. It tries to follow the rules. I've never heard of just running the prompt the same time. That's very interesting. But I have had it just like, okay, do this, and then here's the rules that that was supposed to do. Did it follow those rules in the second pass? And the quality just goes up so much.

**Aakash Gupta** (00:43:30)

So while this is building, can you show us how to auto-invoke skills? Because I'm just on the edge of my seat about this.

**Carl Vellotti** (00:43:35)

Yes. Okay. So... This is the riskiest part of this podcast. So last time I said that there was, okay, well, actually taking a step back, the way that skills are supposed to work is if when we look at this skill, for example, we have this skill and it says, okay, use when the user mentions, make slides, make a slide, create slides, presentation. So it's supposed to just know from when you message it that, okay, great. The person just said, make slides. So now I know I have this skill and I should use it. It doesn't really work that way. And it is kind of just like a funny thing about Cloud Code is this, that auto invocation of skills is really finicky. And I think most people have seen that it doesn't work. One thing you can do, like the most dead simple way is CloudMD, the skills that your AI has access to.

**Carl Vellotti** (00:44:23)

It actually does make a difference, but then you're adding your CloudMD and it's kind of hard to like, if you add a new skill, you have to go back and update the CloudMD. Plus then you're also like eating up context for no reason. So the way to do it is with hooks, which is another thing that we covered last time. But then the demo didn't really work, but I think it's going to work this time. I really heavily tested it. So what we have, a hook is basically... some sort of like thing that you can have happen around the whole Cloud Code workflow. So it can be when you send a message, it can be when a message comes back, it can be before compaction, it can be after compaction. So if you just think about like all of the things that Cloud Code can do, just the whole lifecycle of everything that's possible within what runs a tool, runs a web search, all of that, you can add a hook before or after.

**Carl Vellotti** (00:45:11)

And that basically says, OK, this type of thing has to happen. An example would be maybe every time a new markdown file is created, it has to have some formatting at the top, for example. So here, what we're going to do is we're going to use a hook that OK. So we're going to use a hook. It's a user prompt submit hook. So basically, every time I run a message, then that's when this hook will fire. And what we already have configured before I type this is we have a script that runs. And it just says, OK, are any of the words in the thing that the user just typed in, are those in the keywords of the skills that exist in the skills? And this is nice because it's just a script. So it's not like a... There would be a way to do it where you would have the LLM actually look, but that's very slow.

**Carl Vellotti** (00:46:06)

Whereas this is a script that just says, if there is a match, then I will give it to the LLM. And then the LLM can decide, oh, OK, now is the right time to use that or now is not the right time to use that. So what we did is we just added this hook. And then what we see happens is the way hooks work is so we had the hook here, but it wasn't activated because you have to put it in your settings. And so that was how I set this up. So now there is a hook on user prompt submit. So it's whenever this command is run, user prompt submit, then run this code. And that code sees was one of the words that I just put in. Does it match a keyword of one of my skills?

**Aakash Gupta** (00:46:46)

The biggest question that PMs have about AI outputs is how can I trust this? And you've built some workflows that people can use to enhance that. What are they?

**Carl Vellotti** (00:46:55)

Yeah. So one thing I've realized is that for product managers and people who, you know, they have a few things that have to be right and they have to really be able to rely on it to be right. One of the biggest areas that people are just really concerned about is using AI to do data analysis. Because on one hand, it should be really good at that, right? Like it can run code and you see it do all this other type of code stuff. But For data analysis, you really need the result to be correct. And I think it's an area where if you're not a data analyst and you don't really know exactly how the LLM is coming up with its results, then you're going to be relying on these. You're going to be presenting these to people. You're going to be showing your boss this data.

**Carl Vellotti** (00:47:34)

Where does that data actually come from and how is it calculated is a major area where people just do not trust AI. But it turns out they're actually, like the other things we've been talking about, this is a weakness, but there is a sort of a tool or workflow that we can use to give cloud code we can get much more visibility in the Cloud Code's process so that we can trust its results more. And so the best way to do this is, this is something I've kind of been playing around with more over the last few months, is Jupyter Notebook. So this is the kind of like standard artifact that analysts will use. And it's actually a really good thing to use within Cloud Code. And the very cool thing is that we can basically create a Jupyter Notebook, which is just, it shows what were the exact queries used for this, What were the results?

**Carl Vellotti** (00:48:20)

And I can visualize that all for you. And the really cool thing about Jupyter Notebooks is that a Jupyter file will render natively in cursor or VS code. So you can actually just stay in the tool without having to look at it somewhere else. And it's honestly one of the nicest types of things that you can have be displayed here, like right in your terminal or your IDE. So here what we have is we have in our data folder here, we have survey responses. So we have 213 survey responses from all different types of people in this sort of like fictional company around how they're using this to-do tool. And so what we're going to say is, please analyze this data in a Jupyter notebook and show me what we're working with. So just to start, you can, and this is kind of like a very small, quick example of how can you work with data in cloud code.

**Carl Vellotti** (00:49:10)

And so here it's going to go ahead and it's going to look at this and it will just kind of show us what we're working with. It's pretty hard to see CSVs. There are some extensions that make it easier to see, but they're not great. So it's kind of nice to just have cloud code like show you what you're working with. And right off the bat, we have here, we see this new file was created, this Jupyter notebook, and it's just showing us a very simple, it's actually still working here.

**Aakash Gupta** (00:49:33)

So

**Carl Vellotti** (00:49:33)

this is the code.

**Aakash Gupta** (00:49:35)

Yeah.

**Carl Vellotti** (00:49:35)

Yeah. So it's running Python. And then what it will do is it's, it looks like it has to install a few things to make this like actually render. But what we'll see is we'll see like an actual UI example of what this code is running for us. So we see that it's kind of just getting the columns and data and it will present that to us. We're seeing Claude do some live debugging here.

**Aakash Gupta** (00:49:56)

Yeah, if you ever go look over your data scientist shoulder, they live in Jupyter notebooks. And so how do we add proof of work to our analysis? That's really what we want to do. We want to create traceable analysis. The Jupyter notebook is solving that problem for you.

**Carl Vellotti** (00:50:12)

Exactly. And yeah, so now we see that there's this notebook. It just got the columns. It's showing us like what is the overall shape. So it has this many rows with this many columns. And here's an example of what some of those look like. So what we're kind of just seeing here is what is a Jupyter? How does it work? It's the code. It's kind of like some example output. And then it's rendering that nicely for us. But of course, you can do much more sophisticated things. And it's honestly amazing that once you get more familiar with the types of data questions that Cloud can answer, it's like you're working with a data analyst that will just answer any questions you want about your data. It will segment it in any way. You can do pretty sophisticated statistical types of analyses, all types of things that if you're working at a company, getting access to an analyst's time to ask questions that sometimes you're not even sure exactly what you want to learn or what you're hoping to learn.

**Carl Vellotti** (00:51:01)

or if it would be worth it to do an analysis. That used to be something that had your whole process. You probably don't have that many analysts at your company. Long time for them to look at it. And you have to get it on their own research or data roadmap. Now you can just do a lot of that exploration right here on your own and you can actually trust results. So for the next thing we'll ask here is just show me the distribution of enterprise interest scores as a chart. So now we're moving from just looking at the raw data to now actually creating like a nice visual that shows a bar chart of the distribution between these different groups.

**Aakash Gupta** (00:51:34)

So step one, it'll help you visualize the CSV. Step two, it'll help you create charts. And

**Carl Vellotti** (00:51:39)

we see it running its code over

**Aakash Gupta** (00:51:40)

here. The really powerful mental model for cloud code in general is take the roles that you work with. You almost want to create versions of cloud code for those various roles. That's kind of what the front end design skill is doing. It's taking the designer role. It's trying to like distill what some of that person is doing here. We're trying to distill sort of what an analyst might be doing.

**Carl Vellotti** (00:52:03)

Yeah, I love that. That's a really good framing. It's like, what are the tools or thought processes that these roles have? And then how can we give those types of things to clog code so that it is able to do stuff like that? And of course, it won't always be the exact same, but it approximates it much more. And that's usually good enough for what you need to do as a PM, at least to start. So we see now there's a whole nother set of code here. And now we have this nice distribution.

**Aakash Gupta** (00:52:30)

Wow.

**Carl Vellotti** (00:52:31)

And so just to kind of round this out as one example, so we're going to have it do like a really crazy analysis. We're going to say, show me a correlation heat map of all the numeric columns, satisfaction, feature important scores, enterprise interest, and NPS, what patterns jump out. So now we're going from just, you know, we know what we are hoping to get like out of the data. And now we're having it actually do a much more sophisticated analysis and then also look at it and tell us what it's noticing. And this is where you can really become a collaborative partner with the AI. Of course, you're going to see the things that it's saying, but oftentimes with this type of stuff, it's pretty good off the bat, especially if you give it some of those more ways to think about what would be interesting in the data.

**Aakash Gupta** (00:53:11)

And if you're feeling like I couldn't craft a prompt as good as Carl did, think about creating an analytics manager subagent. And this is your analytics subagent and say analytics manager agent really good at formulating prompts for the analyst. And then the analyst goes execute. If you create this sort of subagent structure, again, replicating what it would be like in a real company, you can outsource a lot of the thinking to cloud code.

**Carl Vellotti** (00:53:37)

Yeah, a hundred percent that, that is a good way to do it. You can have it like kind of know what are a bunch of different types of analyses that it could do. I think this is a really good example of where like, it's much more fun to learn these things because now there's an actual way that you could immediately apply them. So here we have this like awesome correlation roadmap. I don't think we need to go like too deep into it, but this is, it looks cool. And if you, if you knew that this was the right type of analysis that you wanted to do, then, uh, Now we have it here. And what this type of analysis does is it just shows correlation between things. So like in the survey results, how often do people talk about enterprise interest and security? Okay, well, that kind of gives us a sense here that like enterprise cares about security.

**Carl Vellotti** (00:54:18)

Enterprise cares about team management. Enterprise doesn't care as much about pricing, right? They're a little bit more price flexible. And so this is just one example of like a really cool analysis that like... You know, the analyst at your company, I'm sure they could do it, but it would take them some time. You're not even sure if it would be the right thing to ask. But now we have this like awesome analysis and there's all different types of regression testing and all that kind of stuff where if you learn what those things are, now it's really easy to execute them. And you can have a lot more confidence that when you show your analyst or you show your manager, Here is where we got that data from. And then they can look at this and tell you if there's anything wrong with that rather than, you know, just having no transparency to help that AI actually got to that end result.

**Aakash Gupta** (00:54:59)

So we've put together all these features for people, context management, skills, sub agents, hooks, even Jupyter notebook Python analysis. I think the biggest roadblock for people is like putting this all together into a system. So how do people build the right operating system for their cloud code set up?

**Carl Vellotti** (00:55:18)

Yeah, I would say this is something that it's the main way is you kind of use it. And then you probably like even here, we haven't really been doing stuff in the system. So every file that Claude has been making has been getting kind of like dumped out here. And then now we have to figure out, you know, where should it go in the overall system? So just figuring out, like, where should the context layer live? Like where where are the types of information that you want to easily be able to provide to cloud code? Where does that live? What are the different types? And then the other thing is thinking about, OK, well, I'm not just going to have this be a static workplace where I'm just going to only reference, say, oh, hey, in my knowledge folder, like I have these different people I work with.

**Carl Vellotti** (00:55:59)

I have like stuff about my company. You're actually going to be creating new work as well and figuring out where that should go. So I'll just do kind of a quick kind of rundown of the system that I have found works really well in talking to other PMs. I think it's a good starting place. And of course, you'll customize it yourself. So for things where you just want to be able to reference that don't change very often, having just a knowledge folder with some of like the key things that you want to be able to say, hey, Claude, I have a meeting with David Chen, who in this case is, we'll say it's the director of core. It's your direct manager. These are the things that they care about. How should I structure, you know, this piece of writing or things like that. So just keeping in mind, like, who are the people you work with?

**Carl Vellotti** (00:56:38)

What are like different reference material, research, having that in like kind of a static knowledge folder, somewhere for meetings to go. And

**Aakash Gupta** (00:56:45)

Carl's

**Carl Vellotti** (00:56:45)

being

**Aakash Gupta** (00:56:45)

pretty humble

**Carl Vellotti** (00:56:46)

about this,

**Aakash Gupta** (00:56:46)

but... actually putting in the time to build this guys i'm not kidding it will 10x the outputs so if you spend the hour to add in this really important context and then structure it in this way he said the outputs you get will look nothing like the output somebody else using cloud code is building and that's how you we talked about ai slop for a second right earlier that's how you avoid that ai slop label

**Carl Vellotti** (00:57:09)

Yeah, 100%. And there's so much cool stuff you can do with this type of knowledge in here. So one, people love this people folder, which is kind of like a little dossier about different people at your company. No one even ever has to see this, right? This can be your way that you communicate with those people, or what you've learned about those people. But what's so cool is now that Cloud Code is becoming more central to all these You can connect to everything. You could, you know, Granola, which is the meeting transcriber, I think sponsor of this show, they have an MCP that connects. You can pull in your meeting notes. So you could literally have a workflow. Like you have a skill called like update people that would look at what did people say in the meeting that you just had with them and then add notes around like what are the types of things they care about or don't care about into their file.

**Carl Vellotti** (00:57:54)

And then when you go to draft a message to them or you're thinking about something related to them, you have this like, really golden type of context from real meetings in here and that that just provides such a totally different level of information and specificity that you can give to these models than just saying oh yeah my manager he likes you know communication or something like that exactly Yeah, so just having somewhere for it to live so that then you can build on top of it is really the most important thing. I will say the, so having your knowledge folders and meetings and stuff like that is helpful. I would say the other main one that I personally find is the absolute most helpful thing for me is I have a project folder. And the way I use a projects folder is anytime I'm starting any kind of new task, like I'm preparing for this podcast, for example, I'll create a new folder called, you know, product growth, cloud code app, Three.

**Carl Vellotti** (00:58:47)

And then now anytime that I'm doing any work, like, for example, like a real example for when I was preparing for this podcast is this is our third episode on Cloud Code. And so I said, I have my own like transcription. There's actually a YouTube transcribing CLI. So I said, hey, please grab the transcripts from our first two episodes. What did we cover? What did we not cover? And then it drops those into this folder. And then I say, okay, let's draft. What can we do look at in this next episode? That goes in this folder. And so you kind of have a place for all that stuff to live. And what's so cool is that the next time, like, let's say I leave cloud code or I'm on a different machine or it's just another day. Instead of having to sort of figure out like, OK, what was all the information related to that project?

**Carl Vellotti** (00:59:30)

What you can do is you can just literally take this folder and then I'm going to hold shift and you just drop it in here and say, hey, we need to work on this board deck. Here's all the research I've done for before. Get up to speed and then let's work on it. And so the projects folder is just, it's just such a nice way to have everything be couched, you know, somewhere in your system. And then, uh, next time you're coming back to it, it's all there and then you archive it. But anytime you want to go back to it, you have all of the initial artifacts and anything else that you created with cloud code all right there, right in that project folder.

**Aakash Gupta** (01:00:00)

Nice. So I think it might be worth people doing a one-time download to build a projects folder, right? So like, hey, here's our linear and our notion. Please build out my last five projects folders. Pull the initial PRDs, pull the features, results, write-ups. And that's how you can practically implement this pretty fast.

**Carl Vellotti** (01:00:16)

Yep, exactly. And then just kind of like the very last thing to show, like once you do have this all set up, like what are some things that you can do? One, I'll just show quickly that people like a lot is you can have like a kind of start standup command. So what this does or yeah, start standup skill. So when we go to our skills and we look at standup, What this does is it will pull in information from GitHub. It'll pull it in from our tasks folder. It'll pull it in from our calendar. If we had our calendar connected, it'll check linear, and then it'll put it all together for us. I don't have all of that hooked up right now, but it'll use the information that it does have available locally. And so it'll go through and it will pull in on that information and all of those tools and all of those skills and all of those things that you have set up from the system.

**Carl Vellotti** (01:01:01)

You can just start to, you know, mix and match them and having it all in one place. Let's see you just use all this stuff in a completely different way so that it just right there. It has all the information it needs without you having to go and check all those places, you know, one by one. And so when I say I'm living in cloud code all day, Once you get to a certain point, it's like, oh my gosh, I do not want to have to leave cloud code. Like I do not want to have to go to check Google Analytics for how my website's doing. I really want to just be able to ask cloud because then I can say, hey, how is my website traffic? And can you compare that to the post I've made on LinkedIn this week? And that would be almost an impossible analysis to do if I was just clicking into those individual UIs.

**Carl Vellotti** (01:01:41)

But when you have cloud code here set up and connected to everything and you have a place for that information to go, then it just becomes more and more compounding and more and more powerful.

**Aakash Gupta** (01:01:49)

And that's something, to be honest, guys, I haven't done. So I need to do that right now. And what about your CloudMD file, your GoalsMD? What else? Just walk us through the rest of this operating system, how you set it up so that people can kind of get to your expert level fast.

**Carl Vellotti** (01:02:04)

Yeah, sounds good. So the other ones that I would say the other ones that are good to have. Yeah. So data, like we were kind of dropping all of our data analysis into here. Tasks. So just some, and I would say that, you know, you can connect Cloud Code to Apple Reminders or Todoist or things like that. Oftentimes you kind of, as you use cloud code more, you just kind of start to become like a little bit more Markdown native, I would almost say. And so I like just having a file that just says, okay, what are the things that I'm currently working on? And then what are like other things that if I don't have time to work on them now, just drop them into this other folder. And so this is a good way when I just ran that standup command that says, okay, these are all the things you're working on.

**Carl Vellotti** (01:02:45)

These are the things that are not done yet. So having somewhere to manage like the work and then also a place to help house ideas that you don't have time to get to is really helpful. And then the other important ones, tools. So this is where, for example, here we have our meeting prep as kind of a tool. So this is something where what it will do is this one will actually go through and it knows how to run the code in order to put together a meeting preparation for me. And so if I'm, for example, building my standup skill, I can say you have access to this tool that lets you prep meetings or you have access to this tool that will pull metrics. So, for example, I have a big script that will pull in like my beehive newsletter information and it'll check my analytics.

**Carl Vellotti** (01:03:33)

And that's much better to have as like a prebuilt script that you can then test. And what's nice about having it in a tools folder is that anytime you build a new tool or like a new capability for Cloud, it goes here. And then you can in the future, like include in your Cloud MD, hey, you have a tools folder. Use that to figure out like what access to other things that you actually have. And then the last thing that's just really good to set up and keep updated is your overall cloud file. If you're not familiar, the cloud file has like a really kind of like special use in cloud code, which is that it's automatically in context all the time. So for example, when we run context over here in cloud code, And we see like, what are all the things taking it up?

**Carl Vellotti** (01:04:16)

The Claude MD will always be there. And what's cool is it's not just there in the first message, it's there in the background for every message. So this is the type of context you want it to just always be aware of. And so here I have like a fictional company set up called Gradeflow. and this is just like good to include things about how you like claude to work with you who you are what are you working on so that every prompt is kind of through a little bit of a um like it's through a little bit of a lens of what you're actually working on rather than just being generic and this is the type of thing where people love open claw because it is so has so much personality and memory about you this is like the very light very lightweight version that exists in cloud code

**Aakash Gupta** (01:04:54)

It's not quite a sole MD file, but I would say, guys, there's a lot of alpha in continuing to iterate on your Cloud MD file every week, every month, every time you run into an issue with Cloud code. Pull it into your Cloud MD file and update that Cloud MD file. We have covered a lot of stuff, Carl. You have a lot more, too, at cc4pms.com, at the Full Stack PM newsletter, on your hilarious Instagram, your awesome LinkedIn, and Twitter. Is there anywhere else people should be going to find you and learning from you?

**Carl Vellotti** (01:05:21)

No, I think you hit the main ones. CC for PMs is my free Cloud Code for Product Managers course. I have another version, ccforeveryone.com. That is just a more general version that covers the same thing. The cool thing about those courses is that they're Cloud Code taught in Cloud Code. So you'll say, hey, start lesson. And then Cloud Code will actually guide you through a bunch of the stuff, for example, that I kind of showed you today. And then my newsletter, the Full Stack PM. Those are the places you can find me.

**Aakash Gupta** (01:05:47)

Amazing. Do check him out. Do subscribe. And like and comment if we should have him back

**Carl Vellotti** (01:05:52)

another time. I hope we see some likes and comments. I love being on this show.

**Aakash Gupta** (01:05:56)

Amazing. We love having you, Carl. Thank you so, so much.

**Carl Vellotti** (01:06:00)

All right. Thank you. Bye,

**Aakash Gupta** (01:06:01)

everyone. As we distribute the show to more people, we can grow the show, improve the quality of the content and the production to get you better insights to stay ahead in your career. Finally, do check out my bundle at bundle.akashg.com to get access to nine AI products for an entire year for free. This includes Dovetail, Mobbin, Linear, Reforge Build, Descript, and many other amazing tools that will help you as an AI product manager or builder succeed. I'll see you in the next episode. you
