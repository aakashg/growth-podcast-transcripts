---
title: "The Ultimate Guide to ChatGPT Codex: OpenAI's Claude Code Killer"
subtitle: "OpenAI's CLI tool is the best way to build prototypes as a PM - and has a bunch of other powerful use cases"
date: "2025-12-08"
host: "Aakash Gupta"
guests: ["OpenAI's Claude Code"]
speaker_names: "inferred"
substack_url: "https://www.news.aakashg.com/p/chatgpt-codex-guide"
youtube_url: "https://www.youtube.com/watch?v=NYSZ4g7igDg"
duration: "01:00:12"
word_count: 12313
source: "Substack episode transcript (aired audio)"
sponsors:
  - name: "Jira Product Discovery"
    url: "https://www.atlassian.com/software/jira/product-discovery"
  - name: "Vanta"
    url: "http://vanta.com/aakash"
  - name: "Kameleoon"
    url: "http://www.kameleoon.com/"
  - name: "NayaOne"
    url: "https://nayaone.com/aakash/"
  - name: "AI PM Certification"
    url: "https://maven.com/product-faculty/ai-product-management-certification?promoCode=AAKASH550C7"
---

**Sponsors:** This episode is brought to you by [Jira Product Discovery](https://www.atlassian.com/software/jira/product-discovery), [Vanta](http://vanta.com/aakash), [Kameleoon](http://www.kameleoon.com/), [NayaOne](https://nayaone.com/aakash/) and [AI PM Certification](https://maven.com/product-faculty/ai-product-management-certification?promoCode=AAKASH550C7).

# The Ultimate Guide to ChatGPT Codex: OpenAI's Claude Code Killer

*OpenAI's CLI tool is the best way to build prototypes as a PM - and has a bunch of other powerful use cases*

**Aakash Gupta** (00:00:00)

If you're using ChatCBT in the browser, you're using it. Carl Velati is the full stack PM. He knows more about coding CLIs than most PMs do about PRDs. And in today's episode, he's giving you a complete guide to how PMs should be using OpenAI's new codex.

**OpenAI's Claude Code** (00:00:15)

Codex is the most powerful way for product managers to build prototypes, but only if you know how to set it up correctly.

**Aakash Gupta** (00:00:21)

People are saying Codex alone justifies OpenAI's $500 billion valuation. Should you try Sam Altman's new Cloud Code competitor? That's what we unpack today. We do a live demo of Codex for non-technical people so you can get the most out of it. How can a non-technical person ramp up on Codex?

**OpenAI's Claude Code** (00:00:38)

As long as you follow these steps and you're really willing to put in that work upfront, it can be one of the best ways to prototype that exists right now in 2025. And normally, if you ask GBT in the browser, like, hey, here's this video, give me the transcript, it wouldn't be able to do it. It doesn't have the tools.

**Aakash Gupta** (00:00:52)

How should you be using Codex? How does Codex compare to Cloud Code? What are the power user functionalities to get the most out of its prototyping and coding capabilities? That's today's episode. Really quickly, I think a crazy stat is that more than 50% of you listening are not subscribed. If you can subscribe on YouTube, follow on Apple or Spotify podcasts, my commitment to you is that we'll continue to make this content better and better. And now on to today's episode. Quick note for my audio listeners, there are some things that we showed, which you can see on Spotify or YouTube, but we've edited this audio so that it's a really good listening experience nonetheless. Carl, welcome back to the podcast.

**OpenAI's Claude Code** (00:01:36)

I am so excited to be back. Our last episode on Cloud Code was so fun and I'm really excited to cover Codex.

**Aakash Gupta** (00:01:42)

Yes. Past Marty Kagan in less than a week. Amazing episode. How can a non-technical person ramp up on Codex?

**OpenAI's Claude Code** (00:01:50)

Yeah, so let's just go ahead and get started here. Okay, so to get started with downloading Codex, you just go to this developers.openai.com slash codex slash CLI. So today what we're gonna be using is we're gonna be using Codex from the terminal. If you've never done anything in the terminal, I promise that it's gonna be a lot easier than it sounds. Just the very first things you do have to set up directly from the command line. Okay, so on this website, it kind of just gives you the exact commands that you need. So you do need something called npm, but you just type npm install and then you just use this exact command. And when we put that into the terminal, it'll go ahead and install codecs. So I'm going to copy this and then- And for people who

**Aakash Gupta** (00:02:29)

don't know, that's a package manager for Node.js JavaScript, just because we want you to also understand what you're doing here.

**OpenAI's Claude Code** (00:02:38)

Yeah, exactly. That kind of is just the, you'll use NPM for many different things that you're doing from the web. And this is just another one. So we're going to go ahead and copy this into our terminal. If you're on a Mac or Windows, it'll be the same. And what this will do is it will go in and it will just install Codex for us. It's very quick. Okay, so for me, I had it already installed, so it just added one thing. But if you don't have it installed, you just run this one command and you'll be good to go. And then once you have it installed, all you do is we're still in the terminal here. You just type Codex. And now we see this interface and we are all of a sudden, we are in codex. Now we've done the only commands in the terminal you're ever gonna have to do at this point.

**OpenAI's Claude Code** (00:03:17)

In the future, all you'll ever have to do is open up the terminal and then type codex because now we are officially in ChatGPT codex. So just type hi. And now here we are. So just if you've used ChatGPT on the browser, that's all that's happening here is we're just talking to ChatGPT. Let's get acquainted with a couple of the commands. So the first one to know is there is one just model. So we can see what model of ChatGPT are we using. So there's two main options. We can either just use ChatGPT 5, which is what you're probably most used to, or we can turn on GPT 5 codecs. This is kind of an important first thing to know. Even though the tool itself is called Codex, there's also a model that's called GPT-5 Codex. This one is really specifically built for coding and we are gonna cover it later, but it's not great at other tasks where just regular base GPT-5 works the best.

**OpenAI's Claude Code** (00:04:07)

So we'll come back to GPT-5 Codex, but for now, for most of this walkthrough, we're just gonna use regular GPT-5. So we're not gonna use GBT5 Codex, we're just gonna use GBT5. And then once you select it, there's a couple options. Basically, what thinking level do you want GBT5 to have? This is something that I think a lot of people give OpenAI flack for just because there's so many options. But for this tutorial, we're just gonna use Medium. That's what I've used to do all the work that we are gonna demo here. It's a good model because it will intelligently use more thinking power if it needs it, or if it's a quick task, it'll just do it quickly. If you really feel like you have a task that it's not spending enough time on, you can switch to high, but medium works pretty well. And then the other commands that are good to know, if you ever want to just start a completely new chat, you just do slash new, and then that'll start a new chat.

**OpenAI's Claude Code** (00:04:54)

If you're having a long conversation with GBT5 and you're getting low on your context window, which you can see here, it tells you how much context you have left. Then instead of doing new, you can do a command called compact, which will basically have GBT5 just summarize where you're at in the conversation, but in a much shorter way. And then you can continue from there.

**Aakash Gupta** (00:05:14)

Very cool.

**OpenAI's Claude Code** (00:05:14)

Cool. Okay. So, uh, for this demo, what we're going to use today is we're going to use, I have a bunch of files prepared and I'll make these available. Um, we have a bunch of files that are kind of like, as if you were working at a real company so that the demo company here is called task flow. It's a, sort of Jira Asana competitor. So pretty generic, but it will give you the idea. And then what we have here in the files is we have some data. So we have like a user interviews, and then we have some docs like PRDs. So we'll be referencing these sort of throughout the entire podcast. We have this folder, which is where everything is. So we're going to go ahead and open a new terminal at that folder and then do code. Okay, so now we have folder open here and we can get started.

**OpenAI's Claude Code** (00:05:57)

So I'm using a tool called Whisperflow, which I highly recommend. It lets you just sort of talk to your computer and it will transcribe. And so that's, if you see text just appear, it's either probably because of that. So let's try it. please tell me what user interviews we have completed. So now ChatGPT is gonna start searching our code base, our whole entire folder, which isn't really code right now, it's just text documents. And we can see it exploring, listing out the files.

**Aakash Gupta** (00:06:22)

This is the really power of a CLI way to access ChatGPT or Claude for that matter with Codex or Claude code, because you're giving it all the context of this folder. It's a lot easier than setting it up on the web.

**OpenAI's Claude Code** (00:06:35)

Yeah, exactly. So you don't have to provide these files. We're already in the place where those files are, and we can just have it look for them. So right now you can kind of, so it did it. So it was able to list, search, and then read. And then it's telling us that we have these three interviews that were completed. Okay, so now what we can do is it's actually already kind of predicting what we would want. Do you want a quick synthesis of the common pain points? So let's say, yes, please put together the top three pain points across all three interviews. Okay, so it really tells us exactly what it's doing. So it's summarizing, and now here we go. So the top pain points were voice input reliability, integrations, and then template workflow. So now we can kind of already start to see how it is able to use this information.

**OpenAI's Claude Code** (00:07:19)

And then if we wanted, so right now we've seen it search for files and then read and summarize them. You can also create files. Please go ahead and create a single document that outlines all of these pain points along with direct customer quotes. So now what it will do is it will It's already done some of this analysis, so I'm guessing this will be quicker than the first time I had to read it, but it will actually put together a new document for us, and then we can do interesting things like have it pull in those actual customer quotes into that document.

**Aakash Gupta** (00:07:46)

very interesting

**OpenAI's Claude Code** (00:07:47)

planning document creation simplifying so we can also just kind of look at the ui here so it tells us how much context we have left so we haven't really done much so still has 100 gbt5 has a pretty large context window there's a lot of jokes around what context window really means i think one of the biggest jokes is that a 200 000 token context window and a million uh token context window are the same because the way that ai uses it but i will say that gbt5 it it feels like it uses its context window pretty well it fills up very slowly so you can really go pretty far before it starts to like forget everything

**Aakash Gupta** (00:08:25)

Awesome.

**OpenAI's Claude Code** (00:08:26)

The right place

**Aakash Gupta** (00:08:27)

to handle like a whole folder full of all your meeting notes, all of your performance feedback, all of your goals, strategy docs, PRDs, future results right up so that you have like a really nice context window.

**OpenAI's Claude Code** (00:08:39)

Yeah, 100%. And for the tasks that we're looking at here, like classic PM tasks that are more like document-based and not too much code-based, it is just, yeah, it is. You can really easily handle that stuff. It's really when you start doing stuff with like lots of code and logs that that will fill up, but we'll be able to go very far before we have to clear it. Okay, so now it's telling us that we have created this in data user interviews pain point summary, and it's telling us the contents, but the question right now that you probably have is, well, where can we actually see this? So if we go into that folder that we had opened before, then we go into data and we go into, where did it put it? It said it put it in user interviews. So now is where we're going to switch.

**OpenAI's Claude Code** (00:09:17)

We're going to leave the terminal and we're going to go ahead and go into an IDE. So that's an integrated development environment. And so my favorite to use is cursor because I also use it for other types of prototyping. And even if you don't pay for cursor, you can still use the IDE and it's pretty nice. So we're going to go ahead and close this terminal, but we will resume it soon. So I'm going to open up cursor here.

**Aakash Gupta** (00:09:37)

Which is itself a fork of VS Code, so it inherited all the goodness that VS Code had built up over the years.

**OpenAI's Claude Code** (00:09:43)

Yep. And if you want to use VS Code, you can also use that one, of course.

<!-- sponsor -->
**Aakash Gupta** (00:09:47)

Today's episode is brought to you by Jira Product Discovery. If you're like most product managers, you're probably in Jira, tracking tickets and managing the backlog. But what about everything that happens before delivery? Jira Product Discovery helps you move your discovery, prioritization, and even roadmapping work out of spreadsheets and into a purpose-built tool designed for product teams. capture insights, prioritize what matters, and create roadmaps you can easily tailor for any audience. And because it's built to work with Jira, everything stays connected from idea to delivery. Used by product teams at Canva, Deliveroo, and even The Economist, check out why and try it for free today at Atlassian.com slash product dash discovery. That's A-T-L-A-S-S-I-A-N dot com slash product dash discovery. Jira Product Discovery. Build the right thing. Trust isn't just earned, it's demanded. Whether you're a startup founder navigating your first audit or a seasoned professional scaling your GRC program, proving your commitment to security has never been more critical or more complex.

<!-- sponsor -->
**Aakash Gupta** (00:10:55)

That's where Vanta comes in. Businesses use Vanta to establish trust by automating compliance needs across over 35 frameworks like SOC 2 and ISO 27001. centralized security workflows, complete questionnaires up to five times faster, and proactively manage vendor risk. Vanta can help you start or scale your security program by connecting you with auditors and experts to conduct your audit and set up your security program quickly. Plus, with automation and AI throughout the platform, Vanta gives you time back so you can focus on building your company. Join over 9,000 global companies like Atlassian, Quora, and Factory who use Vanta to manage risk and prove security in real time. For a limited time, my listeners get $1,000 off Vanta at vanta.com slash akash. That's V-A-N-T-A dot com slash A-A-K-A-S-H for $1,000 off.

**OpenAI's Claude Code** (00:11:46)

Now that we're in cursor, we can open up a terminal in cursor. So the command is control backtick. And then we're here, and then remember to start codecs, we just type codecs. And so now we're the exact same thing that we had open from before, but just now we're in it sort of with the files themselves. So this is definitely, if you're gonna be working with one of these CLI tools, just open it up in an IDE, because that's the easiest way for you to both do it and then also see what it's actually doing as it works. Another thing that you can do with Codex is you can have it search the web. So let's say we want to search the difference between Cloud Code and Codex and do a summary for us. We will just put that in. So please go ahead and summarize the differences between feature, pricing, ease of use.

**OpenAI's Claude Code** (00:12:35)

So you can also search the web and it's pretty good at it, but we're going to see one of the first sort of limitations of Codex as it starts to do this work. One difference between Cloud Code that's kind of interesting is, so it tells you that it's working and then as it does stuff, it'll tell you what it's doing, but right away it'll start to ask for permissions. So it's like, okay, can I do this search? And we'll say yes.

**Aakash Gupta** (00:12:56)

And I think Cloud Code was showing you like how much you were spending, right? That doesn't do that here.

**OpenAI's Claude Code** (00:13:00)

Yeah, exactly. So it's not actually showing us the number of tokens it's using. All it tells us is the context. So one thing about Codex is that it will keep asking every new website that it finds. It wants to run a command so that it can view what's on that website. Uh, but it will ask for every single one, even though I'm giving it the, even though I'm saying you don't need to ask again because it's doing new commands. It keeps asking me, um, versus on Claude code when you do it on Claude code. So one thing that might be interesting while it's working here is we can actually also run this in Claude code.

**Aakash Gupta** (00:13:36)

I love this. Let's put them head to head.

**OpenAI's Claude Code** (00:13:38)

Okay. So, okay. So we have codecs running here and then let's go ahead and get Claude code running here. So I have Claude on my computer as well, so I'm just typing Claude. And now we have it open. So let's give it the exact same prompt. So we're saying search the web to summarize the differences between the two.

**Aakash Gupta** (00:13:59)

Cloud Code is smooshing.

**OpenAI's Claude Code** (00:14:01)

Yeah, so it's smooshing. This one, ChatGPT is working and this one is smooshing. And so we see it like right away. It's doing like, one thing that we're immediately seeing is that Claude was able to run three separate web searches at the same time. And this is not exactly its sub agents feature, but it is kind of like working in parallel. Whereas Codex is, you know, doing one at a time and it's asking for permissions for every single one.

**Aakash Gupta** (00:14:25)

Seems like they need to dog food their own product a little more over there.

**OpenAI's Claude Code** (00:14:28)

Yeah, so, okay, so it's gonna keep asking. So this is gonna take a really long time. So what I will show is my first sort of pro tip for Codex is so we're just gonna exit and we're gonna run Codex again, but this time there's two options. So one command we didn't look at before is called approvals. And so this is where, right now we're in auto, where it is asking whenever it wants to run a command or make edits. We can put it on full access mode. And the first time you turn this on, it'll kind of give you a warning, like, hey, are you sure you want to do this? Because it gives Codex the power to just kind of keep running commands. My advice, and I know someone's gonna do this, and it might mess someone's up computer, but I think if you do it, as long as you're doing normal stuff that's not sort of interacting you know, with like some sort of base level of your computer, it's pretty unlikely you're going to have any problems.

**OpenAI's Claude Code** (00:15:18)

And this really helps you avoid just the frustration. And there's like lots of memes about this where you run codecs and you give it this long task and it gets started. And then, you know, you got to do something else and you come back and it's just needs permission for some like small command. And so if you run it with this full access mode, then it will just keep going and it's much faster.

**Aakash Gupta** (00:15:38)

Yeah.

**OpenAI's Claude Code** (00:15:39)

And

**Aakash Gupta** (00:15:39)

broken your computer so far.

**OpenAI's Claude Code** (00:15:41)

I haven't broken my computer. And like, so we're in this directory, so it won't leave this directory. So we're not really doing anything that's too risky. So that is a disclaimer is that if that happens to you, I'm really sorry, but I, that's how I use it. So, and then one thing that's funny is you can do codex and then you can do a hyphen hyphen YOLO and then that will automatically launch it into this mode where it won't ask for any permissions.

**Aakash Gupta** (00:16:05)

Best hack ever codex YOLO guys.

**OpenAI's Claude Code** (00:16:07)

Yeah, we're in YOLO. The same version or the version of that that exists in Cloud Code is dash dash dangerously skip permissions, which I also use in Cloud Code. Because it's just really, it's like, it really feels magic when it can just keep doing things and doesn't have to ask you for permission versus when you need to keep giving it permission. So, okay, so Cloud Code finished its answer over here pretty quickly. And even though we weren't in that YOLO mode, it didn't ask for any permissions because it's just doing web searches. And then Codex is working over here. And then yeah, so looking at this UI, it actually tells us, like exploring GitHub API access, and tells you exactly what it's doing. And is exposing, if you saw what Cloud Code did, is it kind of just ran, we'll even just run it again, just to show it while Codex is going.

**OpenAI's Claude Code** (00:16:59)

Let's do the same one. So we're gonna dangerously skip permissions. So that puts it in this mode of, yeah, basically YOLO mode. So let's just run the same command while Codex is running so we can see the differences.

**Aakash Gupta** (00:17:15)

Is Cloud Code generally faster, or is it just on this query?

**OpenAI's Claude Code** (00:17:18)

It's generally a bit faster. And so that's one thing with codex is it's just a bit slower for stuff, even though it also has a different approach where it's searching one website at a time. Whereas with Cloud Code, what we see is that it's doing three at once, and it's just exposing a lot less information. In Cloud Code, it's sort of showing us the exact command and what it's getting back, whereas Cloud Code's kind of hiding more of that. And I think we're already kind of starting to see some of the differences in the design philosophy between these two products, where this one's mustering, and then this one tells you it's looking for pricing info. So Cloud Code, I think, kind of tries to just do the right things in a nicer, simpler interface, and... Codex really wants to show you every single thing that you're doing.

**OpenAI's Claude Code** (00:18:10)

And I think that's kind of like the engineer first, I think is more on the Codex side. Whereas maybe for product management work or document work, Cloud Code hides a bit more of it, but still does it well.

**Aakash Gupta** (00:18:21)

It's almost like Apple versus Microsoft in that way.

**OpenAI's Claude Code** (00:18:24)

Yeah. Yeah. I think that's a good way to think about it. Okay. So cloud code finished. And I think we had actually, we had started it after codec. So it's still working here, but we'll, we'll let it come up with this answer. We can, uh, one thing that you can always do. And as you start to use these tools, that becomes a bit exhausting, but very fun. is while one is running, if it's working on a task, you can always just run another one. So we're just going to open another codex in Yolo mode. And then while the other, while this first codex is figuring that out, we can just keep going into completely new instance of codex over here.

**Aakash Gupta** (00:18:56)

Yep. And you did some tab management there where you linked those two terminal windows. How did you do that?

**OpenAI's Claude Code** (00:19:02)

Yeah, great question. So all I did is you can just right-click, and then you can go ahead and split terminal, and then that lets you have two terminals next to each other. Or in easier ways, you can just drag terminals to wherever you want them to go.

**Aakash Gupta** (00:19:13)

Nice.

**OpenAI's Claude Code** (00:19:14)

Because I think all CLI tools have to have consistency across Mac and Windows in terms of their commands. Command V, which normally pastes on a Mac, doesn't work. You have to do Control V like you would do on a... on a Windows computer. So it pasted it here. It kind of just shows us that it came from the clipboard and the dimensions. Please give me feedback on this image. How could it be more clear? And so you can, you can paste any kind of images in here, multiple images. It's really helpful for like error messages or if you're trying to prototype something, and, you know, the UI isn't right, or you just want to, you know, improve something, you can just, you can give it images and it won't display those images here, but you can sort of trust that it does have them. Claude codes implementation is slightly different, where when you paste an image, it just says the image.

**OpenAI's Claude Code** (00:20:01)

So again, we're kind of seeing it in like another way where Claude just sort of, it just says, just trust me, like I got it right. Whereas with codex, it will say, you know, just give you more information. Like here's where it came from. And then here are the dimensions. So just very, very different design philosophies for sure.

**Aakash Gupta** (00:20:16)

How would you contrast and compare the models themselves and document writing and coding? Like what would be the scores for each?

**OpenAI's Claude Code** (00:20:23)

Yeah. So this is actually a good example for what we just did. So let's look at our question for we asked it to compare codecs and cloud code. We asked them each to do that. And so what we can look at is their actual answers here. So Claude Code is like a bit more formatted. So like we get these like tags at the beginning of these different sections and it is, it sort of really got that we asked for this to be for product managers. And so it's asking for it for product managers. And so kind of giving us what's the difference for PMs, what's the pricing, ease of use, best use cases for PMs. And then let's look at Codex. So it sort of tells you, you know, their high level overview of features. It does also have pricing. also has ease of use, also has best use case for PMs and quick guidance.

**OpenAI's Claude Code** (00:21:06)

So I think in terms of like how they actually write documents, I like the way Claude writes in general a bit more, but I think they're both like we, and we didn't really give a lot of guidance and they had pretty similar answers. Codex is just a bit more, it's a bit more straightforward. Like if you ask for something, it will just give you that. And it doesn't even sort of have like the, the pre tags to these different sections. It just bullet points out the answers. Whereas Claude will kind of try to format it a bit more nicely based on what you might want. And so that's really like the difference. So it really depends what you want. And I would say if you know exactly what you want and you want it to follow like a specific format, then Codex is probably a bit better.

**OpenAI's Claude Code** (00:21:43)

But if you want it to make some decisions because you're not exactly sure how you want something to be done, then that's where Claude will try to guess. And it's pretty good at guessing.

**Aakash Gupta** (00:21:52)

I like that differentiation.

**OpenAI's Claude Code** (00:21:53)

And so that's also very interesting for coding, right? For coding, if you are an engineer and you know exactly how you want something to be built, then that's why a lot of engineers really love Codex because it just follows the rules exactly. Whereas Claude will, it'll do what you say, but it will also like usually do some extra stuff. Like it will create extra documentation without you asking. It'll add more comments without you asking. So if you know exactly what you want, Codex is great. But if you want it to do a little bit of the thinking for you, then I think that's where Claude Code shines.

**Aakash Gupta** (00:22:24)

Hmm. Makes sense. And when a Sahil living good demoed codex on the podcast, we found that it's very industrious, which I think we're seeing here as well. It works for like two minutes, 30 seconds. It'll go off and do stuff versus the Chad Gbt in the browser. Most people are familiar with, you know, unless you have that thinking time, you're not going to get that extended reasoning. And even then it's usually not going for quite as long as it seems like the CLI version would go.

**OpenAI's Claude Code** (00:22:46)

Oh yeah. A hundred percent. One thing with the CLI is you can give it you know, very long running tasks and it will just keep going. Whereas if you're using it in the browser, you know, if you do deep research, it'll do something more, but it mostly will just, yeah, it'll just try to answer your question in, you know, under a minute without really like doing a lot of stuff. Whereas because we're in the, you know, we're in the folder structure, it can go into the files, read them, write them, use the one that it just wrote, run some code and just keep going.

**Aakash Gupta** (00:23:12)

Yeah. Yeah.

**OpenAI's Claude Code** (00:23:13)

So if you

**Aakash Gupta** (00:23:13)

really want that industrious version of ChatGPT, you have to use Codex.

**OpenAI's Claude Code** (00:23:17)

Yeah, that's definitely true. And that's one thing that's just kind of worth, like we're doing a lot of comparison between, you know, Cloud Code and Codex, but a lot of people, they don't necessarily want to have multiple subscriptions or they work at a company that might only pay for ChatGPT or access to ChatGPT. So, you know, there is the comparison, but also it's just good to know what can you do with Codex if that's your only option. Okay, so we're gonna go ahead, so this was just having it review that image and it did a pretty good job. Next we'll move on to, we're kinda just looking at the overall capabilities in general. So we've seen reading and writing files, we've seen viewing images, we've seen web searches. One thing that is another really awesome thing and where we continue to differentiate from the browser is that you can run code.

**OpenAI's Claude Code** (00:24:01)

So of course you can write code, but it's also helpful to just be able to run code. And so for this example, we have an API already installed. but I had ChatGPT install it. So you can just basically imagine this is how you can have your, you know, your LLM actually interface with the world and just basically do anything you can do with code, but in the CLI. So here I found an API that can take a YouTube video and then get the transcript. And normally, like if you asked a GPT in the browser, like, Hey, here's this video, give me the transcript. It just, it wouldn't be able to do it. It doesn't have the tools, but here we have already given it the tool to be able to get those transcripts. using an API, and so it can pull that in for us. So we're gonna say go ahead and use this API to get the transcript for this video.

**OpenAI's Claude Code** (00:24:45)

This video, of course, is our Cloud Code demo from last time. And then it will basically create a new, it'll just put it into a new file for us. So what we see is it's going to go ahead and search our code base, it'll find that we have that API, and then it will run it for us. And so this is where you can really, over time, continue to add tools. to ChatGBT so they can use them for all different kinds of things that you might want. Other examples are you could give it an API to connect to like your database in some way so that it could pull in data for you. Really like any information that's outside of it now, there's probably an API that would let it pull that information in and then do things with it.

**Aakash Gupta** (00:25:25)

This is a really important point. I feel like I'm going to be changing a lot of my prescriptions about when people should be using ChatGPT to be saying, no, you should actually be using ChatGPT Codex because if you want access to tools, if you want to make your LLM actually agentic, Codex is the way to do it. If you want to connect to your database, Codex is the way to do it. That's a really important point.

**OpenAI's Claude Code** (00:25:45)

Yeah, exactly. So we see it running here. It found the files and now it's basically running the script. Okay, so as we did before, we'll go ahead and let this run. And while we do that, we can go ahead and do another instance of codex here. Okay, so for this one, all right, so earlier what we saw is we saw that we were able to give it these interview transcripts and then have it summarize them. Let's say that we had meeting notes and we want them to be summarized. If we just say, hey, summarize this meeting note with action items and decisions, it will do that, but it will always do it a little bit differently every time. And so, what you really want, you know, if you're working somewhere, there's probably some sort of format that you want that's like consistent. So, you know, when you send it out to people, every time it's not different.

**OpenAI's Claude Code** (00:26:33)

So in this, and this is where we kind of start to see a little bit of divergence from Cloud Code, is there are no commands. So you cannot add custom commands to Codex. So you can't say, you know, in Cloud Code, you can say, you can create a command that's like summarize meeting, and then you can just point it to those files. All that the commands in Cloud Code really are, though, is they're just other files that have instructions. And so here we have already created a template for meeting notes summary. And so, of course, this should be anything that you wanted. But here I'm saying that the template that I want is discussion points, action items, risk blockers, and next steps for next item, and then some instructions for the summarizer. So even though we can't actually have a new command, what we can do is we can say, summarize the meeting notes.

**OpenAI's Claude Code** (00:27:25)

And then we haven't actually covered this yet, but if you want to sort of target a specific folder or file, you just do the at sign, so meeting notes. Okay, so we're adding the whole folder, and then we're saying using, and then what we have is this template is called meeting notes summary template.

**Aakash Gupta** (00:27:45)

This

**OpenAI's Claude Code** (00:27:45)

is what we'll do is

**Aakash Gupta** (00:27:46)

reference folders and files. So if you had a PRD template, you could apply this to a PRD template, basically anything.

**OpenAI's Claude Code** (00:27:52)

Yeah, exactly. And we'll do a nice little deep dive into how to use this for PRDs as well. Okay, so we said here's where those meetings are, those meeting notes, and then use this template. And what it will do is it will follow those instructions exactly. So this is how you can sort of really start to define that behavior over time for the LLM. And it's nice because let's say that you run this and then you get some feedback from your manager that your meeting notes are too long or or the key decisions weren't clear enough, or you wanna make sure that the date is like very specifically called out, then you can just edit this template and you can either run it again for those same meeting notes or you can just have that going forward. And again, this is another thing that's just pretty hard to do in the browser.

**OpenAI's Claude Code** (00:28:37)

And this is also a nice way where, you know, when you're on Twitter or you're on X and you see a really cool prompt that would, you know, help you think through something or, you know, there's all those like mega prompts that people post, but you never know what to do with them. You could store them in here as part of your templates or prompts and then trigger them super easily. So you actually have access.

**Aakash Gupta** (00:28:55)

Oh, this could be the best place to build your prompt library too.

**OpenAI's Claude Code** (00:28:58)

Yeah. You know, I think, uh, I don't know if there, if anyone has really built like a good, like open source product management prompt library. That might be a good project that you could pull into these and then use whenever you wanted.

<!-- sponsor -->
**Aakash Gupta** (00:29:09)

Yeah, that'd be huge. Today's episode is brought to you by the experimentation platform Chameleon. Nine out of 10 companies that see themselves as industry leaders and expect to grow this year say experimentation is critical to their business. But most companies still fail at it. Why? Because most experiments require too much developer involvement. Chameleon handles experimentation differently. It enables product and growth teams to create and test prototypes in minutes with prompt based experimentation. You describe what you want, Chameleon builds a variation of your webpage, lets you target a cohort of users, choose KPIs, and runs the experiment for you. Prompt-based experimentation makes what used to take days of developer time turn into minutes. Try prompt-based experimentation on your own web apps. Visit chameleon.com slash prompt to join the waitlist. That's K-A-M-E-L-E-O-O-N dot com slash prompt. Today's episode is brought to you by NIA1. In tech buying, speed is survival.

<!-- sponsor -->
**Aakash Gupta** (00:30:07)

How fast you can get a product in front of customers decides if you will win. If it takes you nine months to buy one piece of tech, you're dead in the water. Right now, financial services are under pressure to get AI live. But in a regulated industry, the roadblocks are real. Naya One changes that. Their air-gapped, cloud-agnostic sandbox lets you find, test, and validate new AI tools much faster, from months to weeks, from stuck to shipped. If you're ready to accelerate AI adoption, check out Naya One at nayaone.com slash akash. That's N-A-Y-A-O-N-E dot com slash A-A-K-A-S-H. Today's episode is brought to you by the AIPM certification on Maven. Run by Migdad Jaffer, who is a product leader at OpenAI, this is not your typical course. It's eight weeks of live, cohort-based learning with a leader at one of the top companies in tech. OpenAI just doesn't stop shipping, and this is your chance to learn how.

<!-- sponsor -->
**Aakash Gupta** (00:31:02)

Run along with product faculty and Mo Ali, the course has a 4.9 rating with 133 reviews. Former students come from companies like OpenAI, Shopify, Stripe, Google, and Meta. The best part? Your company can probably cover the cost. So if you want to get $500 off, use my code AAKASH25 and head to maven.com slash product dash faculty. That's M-A-V-E-N dot com slash P-R-O-D-U-C-T dash F-A-C-U-L-T-Y.

**OpenAI's Claude Code** (00:31:30)

Okay, so we see that it's working. Let's go back to that first one with the YouTube transcripts. So

**Aakash Gupta** (00:31:35)

to review here, Codex can connect to API. So we have connected to the, is it the YouTube API here?

**OpenAI's Claude Code** (00:31:41)

Yes. Or it's not the YouTube API. It's one that someone else built called the YouTube transcript API. And it's using that. Cool. Okay, so save this transcript to data YouTube. So let's go into that data YouTube. I should be charging $999 for this cloud code tutorial. And then, where is this? Okay, and then we have that full entire transcript here. So it worked, basically. So that's cool. This would be very hard information to get into a file that you could then use, because now, of course, we could have it summarize this or do interesting things with it without us having to copy and paste it in or something.

**Aakash Gupta** (00:32:19)

Yeah, you literally can't get ChatGPT to go pull a YouTube transcript like this. Otherwise, it struggles with the browser use and everything like that. So this is a way to connect it to things that you can find via APIs, which is very powerful.

**OpenAI's Claude Code** (00:32:33)

Exactly. Cool. Okay. And then it created the summary. So meeting notes, summaries. So put them into meeting notes, summaries. So meeting notes, summaries. Okay. And then we see that we have all those meeting notes according to that sort of exact template that we gave it before.

**Aakash Gupta** (00:32:49)

Very cool. So connected to APIs here, it used our template to create meeting notes. These are some crazy use cases compared to regular chat GPD.

**OpenAI's Claude Code** (00:32:57)

Yeah, and now what we'll do is we'll kind of take these things that we've used and we'll put them together in a pretty powerful way. So what we'll do is we'll go ahead and launch Codex again, and let's go through a quick sort of tutorial on how you can really use... So, so far what we've seen is we've just been giving... ChatGPT like basic, like, you know, things that we for sure know it can do. Just summarize this meeting transcript, use this code. But one thing that was really useful about, you know, having it in this interface is that we can actually have it, like have a conversation with ChatGPT before we actually create the document. So if you need to do some thinking, GPT can be a really good thinking partner where it can ask you questions about the PRD that you're trying to build before then actually creating it for you.

**OpenAI's Claude Code** (00:33:43)

Because if you just ask an AI to build a PRD, it will do it, but it won't be very good. And because most of the way that you write a good PRD is with good thinking, sort of good upfront thinking as a product manager, so that All of that thinking sort of is embedded in the document.

**Aakash Gupta** (00:34:00)

Yes, exactly. When your company gives you that template, they're actually asking you to think about it, not just prompt AI for it. AI will just make some weird assumptions.

**OpenAI's Claude Code** (00:34:07)

Exactly. And here's where you can do some cool stuff is you can have in your folder, basically, company context. So here we have... in our docs, we have business info. So this tells the AI, like what is, what does our company actually do? Especially if you work at like a startup or a specific, even a specific part of, you know, the company that you work for, you can say like, what are you actually trying to accomplish? So that when you're, when it's writing that PRD, it has so much more context than if you just say, write this PRD without understanding kind of all the other stuff. And this really helps it sort of gives it the context for questions that ask you about how you can improve your PRD. So first what we'll do is just to make sure that it kind of understands its context is we will say, okay, read this doc for business info and give me a summary.

**OpenAI's Claude Code** (00:34:53)

And then next what we're going to do, and this is completely different than anything we covered in the cloud code tutorial is, and this is something I've been playing around with that has been pretty effective. is in our templates, we have something called Socratic questioning. So this is just one example of how when you find one of those really interesting prompts online or something that you think would be helpful, how you can actually use it. So in this case, I saw one about Socratic questioning, which is basically the AI will ask you really open-ended questions that don't have a right or wrong answer, but they are the types of questions that if you're in a meeting with your manager or some execs and they ask, how do you know that this is really the right problem to solve? Or why do you think we should do this when our competitor is doing this?

**OpenAI's Claude Code** (00:35:36)

It will kind of guide you through those types of questions, both to kind of help you think about them, you know, that's the most important thing. And then also think through those problems and then ultimately actually embed those in the PRD when it goes to write the PRD.

**Aakash Gupta** (00:35:50)

Love it.

**OpenAI's Claude Code** (00:35:50)

So what we're going to do is we're going to say, please read the Socratic questioning prompt, and then give me some questions about, and then in this case, we're going to go through an example where we're creating a feature for a voice chat with your to-do list. So that might be useful for, you know, someone who's on the field and they have a bunch of stuff that they have to mark off as they complete it, but it's hard for them to like get to a computer interface or something. So right now we see it, it's opening up that questioning template, it's reading it. And then it kind of understands the context from our company. from what we gave it before, and then it will ask us some questions. And of course, this is where when you started, you'd probably have like a lot more ideas for it.

**OpenAI's Claude Code** (00:36:26)

And one tip that I definitely have, and this is something that people talk about commonly, is with tools like Whisperflow, where you can just kind of talk and just explain your idea without having to worry about formatting at all. because it will all get accurately transcribed. And LLMs are really good at just taking brain dumps or any sort of amount of context and understanding what you're actually trying to communicate. And they can use it. So it's a really good way to just start your PRD is just explain the whole feature and what you're trying to accomplish. And then it will use that to ask you good questions.

**Aakash Gupta** (00:36:58)

And you can even just put a list of like things to remind yourself as you're speaking into whisper flow, you know, the problem, the solution discovery you've done so far, other features that you've launched and that can just really help you create this right context dump.

**OpenAI's Claude Code** (00:37:11)

Yep, just kind of stream of consciousness is sometimes a good way to go. Okay, so the mode that I have it in right now is it's asking like multiple choice questions. And one thing I'm going to do to just make this quicker, because the exact output here isn't too important. We're going to go to like a lower model just to keep it quick. But basically it'll say, okay, here's a question. So basically, so its first question here is asking us like, why do we think that this voice to-do list feature would be helpful? So it's saying, do we have... Quantitative, so do we have data for this? Is it qualitative, we've heard from user interviews, or is it strategic? We just feel like we need to have this feature. So we looked at our data from before, and one of them, we just saw that our user interviews were pointing to this being a good feature.

**OpenAI's Claude Code** (00:37:52)

So we'll go B, and it will just ask us a few questions. And again, the exact answers here aren't that important, so I'm just gonna go ahead and put them in. But it sort of shows the idea of how it can really ask you pretty in-depth questions to really challenge your thinking. I think people

**Aakash Gupta** (00:38:07)

underrate the LLM as thought partner use case. But here, especially because we gave it the context, it's pretty powerful.

**OpenAI's Claude Code** (00:38:14)

Yeah, exactly. And it's actually asking us like a lot of questions here. It's saying, it's following up on all those questions that we just asked. So it's saying, when is the best time to launch it? What has to work reliably for V1? How should we, and then it's also asking about some, like the MVP scope. What should we do when we have only like really low confidence transcripts? Or what fields do we need to start with only for V1? Can it just be title and due date? Does it also need an assignee? So these are the types of things where, you know, hopefully you're already thinking about them as a PM, but there's a lot that you have to manage. you know, as a PM and every product can be much more complex than you expect. So having this LLM like really challenge you on all these different aspects, both kind of to remind you and then give you some options to think through makes it so that once you do present your work to, you know, your engineers or your designer or your manager, it's much more thought through.

**OpenAI's Claude Code** (00:39:02)

OK, so what we're going to do is we're just going to go ahead. I don't want to answer all these questions for this fictional product. So we'll kind of move on to the last step here. So we imagine we're in this world where it understands our business context. We've been talking to it for like an hour answering all these questions. And now we're ready to just have it actually write the PRD. So we can do a similar thing to what we did before where we can say, hey, I have this PRD template I like. And then another cool thing that you can do is you can say, like let's say you're working in a company where there are some like really killer PMs who write amazing PRDs. Maybe they're also using codecs, but you've just seen them and they're great and you want to model yours after theirs.

**OpenAI's Claude Code** (00:39:41)

You can also point to those existing versions and then have it sort of create another version for you that of course is not copying any of the language, but just the style is something that you can pretty easily do with this. So this kind of last thing, just pulling it all together is we're gonna say, please review three PRDs from this folder and then create the final PRD. So please use, and then we're gonna go ahead and add PRD template. So the

**Aakash Gupta** (00:40:12)

ideal PRD structure, first inform it of the context in the folder, have it review the template, have it do the Socratic methods with you, and then you have it review the example PRDs and finally create it.

**OpenAI's Claude Code** (00:40:24)

Yes, exactly. Perfect. And then let's go ahead and just put in this last thing in docs, example PRD. So let's say that you know, like, let's say your manager before they got promoted, they had like a really killer PRD that also makes a lot of sense for the feature that you're building. And so we'll say that maybe that's this mobile workflow editor So please use this template and then this doc as inspiration to write our POD based on everything we discussed above and put this into a new .md file.

**Aakash Gupta** (00:40:58)

And it's crazy how much faster it is dictating.

**OpenAI's Claude Code** (00:41:00)

Yeah. Yeah. Every time I start typing, I'm like, oh, also I have like a, a weird weakness where I, I'm not a super slow typist, but whenever I'm screen sharing, I am just the worst, absolute worst typist anybody has ever seen. So, uh, it's like a thing that like I've actually, people have commented on at work. Like Carl, do you like know how to use a keyboard? Um, so that's why I'm, I'm very extra grateful for a voice dictation in these, these podcasts for sure.

**Aakash Gupta** (00:41:29)

I think the 16K views in seven days begs to differ, but a lot of dictation did help there.

**OpenAI's Claude Code** (00:41:34)

Yeah, for sure. Okay, great. And it's pretty fast at this point and it's putting it into our whole format here. So this is a way that the output that you can get from a PRD just going through this process versus really anything you can do in the browser is just, it goes from being a sort of kind of their PRD that you're going to have to edit a lot to a really good PRD that like it's almost right out of the box going to be like almost everything you want. because you've done all that actual thinking with it, and then it's just embedding that versus it makes it, and then you have to kind of think and respond. And I think that's like the classic thing where, does AI really speed you up if it creates something, but then you have to spend the same amount of time fixing it?

**OpenAI's Claude Code** (00:42:16)

Okay, cool. Yeah. No, definitely not.

**Aakash Gupta** (00:42:18)

PRD workflow.

**OpenAI's Claude Code** (00:42:20)

Yes. Okay, so. Sometimes you always just have to ask your AI, like, what did you do? Oh, an open, okay, please move it there. Also, one thing, I didn't really proofread what I said before, so I said to call it new.md. So it did that instead of new space md. Oh, but here it is. Okay, so let's just look at this. Okay, and now we have this very nice PRD. Customer problem, business impact. goals, with our metrics. And these are all tied to things that the company actually cares about from that folder we had before. Target users, like this is a really, really nice PRD. A lot better than what you're

**Aakash Gupta** (00:43:03)

going to get if you just say, write me a PRD and give it some context.

**OpenAI's Claude Code** (00:43:08)

Yeah, exactly. Okay, so we are getting pretty close to the end of what you can do with Codex in the CLI. So we've kind of seen most of the stuff. We've seen it be able to search, read, write files, seen it be able to create new documents, seen it be able to be a thought partner, seen how you can store prompts and then use them. Um, and so in some ways it's a bit nice because it, you don't have to like, there's no like super complicated workflows and we'll talk about cloud code and how that compares in a second, but really it's just, just files on your computer. And then you can save prompts in those files. You can save templates in those files and you just sort of reference those files when you need to use them. Um, and so that's why, like we talked about already, there's no, there's no custom commands in codecs, but all a command really is even in cloud code.

**OpenAI's Claude Code** (00:43:58)

is just basically pointing to a markdown file. So there's some, it can feel a bit less fully featured and there are some areas where it is less fully featured, but I actually think that there's some niceness to how they haven't overbuilt a bunch of these features that are just basically pointing it to files. Okay, so we already covered that there's no slash commands. Another thing that Cloud Code has that is pretty nice and does not exist in Codex is planning mode. So really quick, just as a reminder, when we're in Cloud Code, this is sort of the opposite of the YOLO mode is planning mode. So that's like, hey, do not do any, you're like literally can't make any changes to any files when it's in plan mode. And so what Cloud Code will do is you'll have a conversation with it and then it will basically tell you what the plan is and you can modify the plan before it starts.

**OpenAI's Claude Code** (00:44:52)

And then it will actually kind of show you the checklist. And they're starting to do some very cool things with that feature where if there are gaps in the plan or there's decisions that have to be made, it will give you multiple choice options for what, like, hey, how do you think we should handle this edge case? And then it says you could do this or do this or you can type your own thing. So that's pretty nice. But otherwise, this type of feature doesn't really exist in Codex. Although it does in Codex. the sense of when we go to those approvals, so the slash approvals command, instead of, so we started with auto, that was kind of where we started this podcast, and then we moved into YOLO mode, which is this full access, never ask for permissions. You can put it in read-only mode, And then that's just exactly what we were talking about where it can't change files or start doing anything because LLMs, they're built to serve.

**OpenAI's Claude Code** (00:45:41)

They just want to start doing stuff. So this stops them from doing that. But I would say it's not really like, it's not as fully featured as Cloud Code. So if you need to do a plan and you don't want to start changing things, then you just tell it like what you're trying to do and it can't start coding, which is helpful. And so this is the closest that you can get with it right now. Got it. And then, okay, so the big thing, the very most important thing that Codex is missing that Cloud Code has is agents. So when you do something in Cloud Code and you can ask it to spin up sub-agents, and what it does is it will basically create clones of itself with different tasks, and then it can parallelize work very powerfully. And Codex doesn't have anything like that sort of out of the box.

**OpenAI's Claude Code** (00:46:32)

And so like we saw kind of before, so what we're gonna do is we'll use an example here where we say, hey, use that YouTube transcript API that we talked about from before. I want you to search for the best ways to use Codex CLI. I want you to get three videos. I want you to run them all in parallel and then create a summary document. If we told that to Cloud Code, then kind of out of the box, it knows how to do it. There is a kind of hacky workaround that we can use to do that in Codex.

**Aakash Gupta** (00:47:00)

How do we do that in codecs?

**OpenAI's Claude Code** (00:47:02)

So as we've seen, you can have codecs running multiple times. We can run it here and give it a task, and then we can go to another terminal, and we can run it here and give it a task. What you can do is you can have codecs to do that on its own. So it basically will make terminals that you can't see in the background and then give those tasks and then they can run in parallel and then it can get the outputs from all of them and put it back together. And functionally that actually works pretty well and it is similar to Cloud Code's agents, but it is definitely a workaround and it's not sort of like a first class feature like it is in Cloud Code.

**Aakash Gupta** (00:47:40)

So how do we do that?

**OpenAI's Claude Code** (00:47:41)

Yeah, so you can actually basically, like with most stuff, you can just kind of tell it to do it. So we'll start a new chat here. And then we're going to give it that exact command that I just said. So we're going to say, find these three. So we're going to say, I want you to find three recent videos for Codex CLI on YouTube and then create summaries in parallel. Here's the approach. And so the first time you do this kind of approach, it will have to sort of like write the... the script for it, but then going forward, it can use that more easily. So search YouTube and give me three video URLs, then write a script that, you know, runs them in the background, uses YOLO mode, so you don't have to worry about permissions, gets a transcript, creates a summary, and then put them all back together.

**OpenAI's Claude Code** (00:48:19)

And so let's actually, this is a good one. Let's do it and let's show the difference between Cloud Code and Codex for this. Okay, and then let me make sure that we're in the right mode. Okay, good. They're both in YOLO mode. So I'm gonna change it a little bit for a cloud code, because it doesn't need to do that. We'll just say, instead of writing the script, instead of writing the script, we'll just have it spin up three agents in parallel to create summaries of each video. Okay, so now we'll really see the difference between how these two approach this. For codecs, there's some things that it has to figure out. Like, it'll have to figure out exactly how to do this. Whereas, we see Cloud Code just starts working. So first, it's searching on YouTube to try to find those videos that we can use for the API.

**OpenAI's Claude Code** (00:49:07)

So it already found... actually yeah it'll keep thinking so did a search didn't find anything but it'll keep thinking and um yeah it's interesting cloud code can be a bit inconsistent here we actually saw it there aren't really okay so cloud code got confused it couldn't actually find those videos whereas it looks like codex actually already found those videos so i'm not sure if it's because cloud code has some sort of limitation for searching YouTube, I think that's definitely possible. There's a lot of websites these days that are kind of trying to block agents from getting into them because of all the data extraction. But let's see when we run this again if it finds them. okay so now with with codex we saw that it did successfully find three videos and now it is creating that script to run itself in parallel and so it's planning that and then okay great so this time uh cloud code did find it so yeah sometimes that's one thing we're just working with llms in general they're sort of they're never deterministic which is the beauty of them and kind of the the pain of them as well

**Aakash Gupta** (00:50:10)

yeah in

**OpenAI's Claude Code** (00:50:10)

the fun

**Aakash Gupta** (00:50:11)

of five demos

**OpenAI's Claude Code** (00:50:12)

Yeah. And the fun of live demos. Some of, some of this stuff, like I have kind of on the rails and then some stuff is like, okay, like I'll, I'll have tested it on my own before, but you never know exactly what will happen when you actually run it. Um, okay. So, uh, I actually would say that so far, I think codex is going to ultimately be slower, but it's doing a better job. Um, it found like more relevant videos where We see cloud code is kind of starting to do some like crazy stuff. Like it has found our original prompt was also to look at codec CLI. And then what we see here is it's kind of, it's like going way off the rails where it's like pulling in medium articles. It's like a, it's like no longer on YouTube. Um, it found a Claude code tutorial for building a YouTube research agent, which is like obviously way off what we want.

**OpenAI's Claude Code** (00:51:02)

I think it's, I think what it's doing is it's looking at these websites and it's trying to find the YouTube videos and it's trying to find three. So it did. Okay. It did eventually get there. It didn't go like completely off the rails, but it definitely took it a lot longer than I would have expected to find them.

**Aakash Gupta** (00:51:15)

Yeah. But it's cool also at the same time that it did like go through the process of, oh, this isn't going to work for me and let me go find something else.

**OpenAI's Claude Code** (00:51:23)

Yeah, definitely. There's that saying that you can feel the AGI. I think it's some of that stuff where it navigates its own problems that you kind of start to feel the AGI. I think for me, like a big one was I was working with Cloud Code the other day and it committed its work before it started and then it tried to do something. And it realized like what it did wrong. And then it went back to that commit and just erased its work. But it's like, okay, let me go back and do it the right way. And then the second time through, it got it right. So these tools are getting, they're getting pretty smart. They're doing some like sort of surprisingly human behaviors in some ways. Because that's exactly how, if you're working with this tool, you're like, oh, okay. Like we were doing it wrong.

**OpenAI's Claude Code** (00:52:04)

We figured it out. Let's go ahead and go back and try it again the right way. They're starting to do that on their own. Okay. So yeah, I think Claude Code had a slow start, but it now started the tasks to run the YouTube transcripts and all three agents have compiled their summaries in parallel. Now let me combine them into one doc. So I think Claude Code at the end of the day is going to win this, this agent race, which makes sense because it's so much more sort of baked in, in first class. And then while this is happening, kind of the last good thing to talk about in comparing these is, so this is just agents where it's sort of like a sub instance of the main thing that it can give its own rules to. But there are actual dedicated sub agents, which we saw in cloud code where you can sort of define like, how it works and what tools it has, like a executive reviewer or a design reviewer or an engineer.

**OpenAI's Claude Code** (00:52:57)

That exists and is pretty first class in Cloud Code, but there's really no version of that in Codex. I think the closest you could get is you could make a file like everything else that sort of defines how it works. But in Cloud Code, you can give them specific tools and just much more configuration. So I wouldn't be very surprised if we saw something like that coming out of OpenAI for Codex soon. But as of right now, there's just no parallel.

**Aakash Gupta** (00:53:23)

So in general, Cloud Code is more agentic.

**OpenAI's Claude Code** (00:53:26)

Yes, for sure. Okay, so Cloud Code is just about done here. It actually, it looks like it did finish. Okay, so Cloud Code won, but... Codex is not too far behind. It's now at the step of, it has all the transcripts and the summaries, and now it's putting them all back together. So that is basically everything to cover in terms of like main PM tasks for these two tools. Okay, Codex, honestly, it was pretty close race overall, despite the completely different approaches. So I would say I wouldn't be too surprised if Codex In general, Cloud Code just kind of like leading the whole CLI interface. I think they were the first ones to really come up with the idea of trying it. And so, you know, at this point, they are pretty far ahead and other teams are playing catch up. But I wouldn't be that surprised if once OpenAI sort of gets to these sub-agents, if it could have probably done this task faster than Cloud Code.

**Aakash Gupta** (00:54:24)

And which one was more quality?

**OpenAI's Claude Code** (00:54:25)

Yeah, let's look. Okay, so this one. So Codex, the Cloud Code one is in... YouTube code, data. Okay, so this is cloud code. Okay, so it's kind of showing each video, step-by-step highlights, key takeaways, video two, video three. Pretty good, kind of verbose. Yeah, they're pretty verbose. Let's see how this compares to what Codex did. So yeah, pretty verbose. I'd imagine that these are probably pretty good summaries. It's really calling out some very specific stuff, the reverse deep seek moment. So it looks quality. I don't think we want to read through all of them right now, but let's just look at like high level, how they look. Providing document location. Okay, final report output. Okay, here we go. And then here is the codex one. Open the preview here. Okay, so we definitely see like a totally different style, right? Like with the cloud code one was like sort of broke it up into sections and then gave bullet points for each one and then kind of gave like a summary of everything at the end.

**OpenAI's Claude Code** (00:55:35)

Whereas if this codex one, it looks like it is It's got some formatting error. That's some weird formatting.

**Aakash Gupta** (00:55:43)

We could

**OpenAI's Claude Code** (00:55:43)

probably ask. Not very good. Yeah, I think that the Codex one, it obviously of course chose different videos. It's got a

**Aakash Gupta** (00:55:49)

lot of stuff like get instant access to all premium courses and stuff. It doesn't seem like it did a good job of actually.

**OpenAI's Claude Code** (00:55:54)

Yeah, this doesn't look good at all. I think there may have been something that got messed up in those, like the execution of the sub agents. So I think for right now, parallel, parallelizing tasks in the same way that you can do in cloud code, just really not that great in codec. Okay. So one thing though, and this is kind of where we'll transition to the next kind of like last thing here is we've been a bit unfair to codecs so far because we are comparing on sort of classic, you know, PM document based tasks. And, Overall, I would say that cloud code is probably a bit faster. It has a little bit more features that are really first class. But what we haven't talked about and what Codex is really actually built for is coding.

**Aakash Gupta** (00:56:35)

Amazing. If we had to summarize, what are the top use cases for PMs of Codex?

**OpenAI's Claude Code** (00:56:41)

Yeah. So I would say the top use cases for PMs of Codex, one is if you just only have access to ChatGBT from your company or something, then it's, it's a very good tool for all the things that we covered today, which are, uh, you can use it to basically do anything sort of like that you would normally think of about for, um, an LLM. So the top use cases are you can use it to get summaries of any document. You can use it to do analysis across a bunch of different documents. You can use it as a thought partner for any sort of thing that you want to work through it, you know, to think through a problem before you actually present it to anyone. LLMs can be really good at challenging your thinking and just any type of thing where you are working on something where you need to be able to pull in information, from anywhere else.

**OpenAI's Claude Code** (00:57:29)

You can use Codex to do that for you and then keep it all in one integrated environment where you can do all of those things. So really like documentation, anything related to documentation is a really good use case for product managers and For product managers that want to do prototyping, as long as you follow these steps and you're really willing to put in that work upfront, it can be one of the best ways to prototype that exists right now in 2025.

**Aakash Gupta** (00:57:56)

Amazing. And then there are all sorts of other use cases that are just valuable for you as a person, I think, to use Codex. Building presentations, automatically creating change logs, working with audio files, extracting image files, changing the format on a video file, cleaning up messy invoices, Clearing space on your computer, basically anything you want an LM to do on your computer when it comes to working with files, where you'd have to go and search it on Google and install something as an app before, now you can just have codecs to it.

**OpenAI's Claude Code** (00:58:25)

Yeah. And I'm so surprised because I really started using cloud code. So like anything in the CLI for the first time, like I didn't use it before our podcast, but as we were kind of, you know, as I realized we were going to be doing it for like the month before I really started using it for like just more and more stuff. And now I almost just live in the terminal. which is crazy and i never would have thought because i'm not an engineer but now it's just so useful that most of my like working stuff that i do on my computer i actually just start in the terminal

**Aakash Gupta** (00:58:56)

that could be you too guys if you want to learn more check out carl at carl the pm on instagram love his meme page it's literally one of the funniest things i wake up to every day check out his newsletter the full stack pm If you want to become a full stack PM, follow him on LinkedIn or X, he's everywhere. And we'll probably have to have him back for another podcast as well. So let us know what we should have him back for. Carl, thank you so much.

**OpenAI's Claude Code** (00:59:19)

Yeah, thank you so much. This was a lot of fun. I learned a lot and I hope that everyone watching learned a lot too. Bye guys.

**Aakash Gupta** (00:59:24)

So if you want to learn more about how to shift to this way of working, check out our full conversation on Apple or Spotify podcasts. And if you want the actual documents that we showed, the tools and frameworks and public links, be sure to check out my newsletter post with all of the details. Finally, thank you so much for watching. It would really mean a lot if you can make sure you are subscribed on YouTube, following on Apple or Spotify podcasts, and leave us a review on those platforms. That really helps grow the podcast and support our work so that we can do bigger and better productions. I'll see you in the next one.
