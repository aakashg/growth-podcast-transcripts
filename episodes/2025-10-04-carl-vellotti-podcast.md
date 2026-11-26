---
title: "The Claude Code Tutorial for AI PMs: Why You Need to Use It + How"
subtitle: "The complete guide to the tool that hit $500M ARR in 4 months."
date: "2025-10-04"
host: "Aakash Gupta"
guests: ["Carl Vellotti"]
speaker_names: "substack"
substack_url: "https://www.news.aakashg.com/p/carl-vellotti-podcast"
youtube_url: "https://www.youtube.com/watch?v=4nthc76rSl8"
duration: "01:37:04"
word_count: 19065
source: "Substack episode transcript (aired audio)"
sponsors:
  - name: "Linear"
    url: "https://linear.app/partners/aakash"
---

**Sponsors:** This episode is brought to you by [Linear](https://linear.app/partners/aakash).

# The Claude Code Tutorial for AI PMs: Why You Need to Use It + How

*The complete guide to the tool that hit $500M ARR in 4 months.*

**Aakash Gupta** (00:00:00)

Cloud Code hit 500 million ARR in four months with just two product managers, no advertising, no marketing, massive growth that is replacing tools like Cursor, Lovable, Replit, and Bolt.

**Carl Vellotti** (00:00:11)

It's funny how quickly expectations of how good these things should be can change.

**Aakash Gupta** (00:00:15)

Carl Velotti, who runs the largest PM Instagram account in the world and is an expert with this tool. While some of us are vibe coding, he's building tons of agents to coordinate his life, and this episode is going to break it down. If somebody with zero technical experience is listening right now, why should they care about learning Cloud Code?

**Carl Vellotti** (00:00:32)

It takes you out of the interface in just a chatbot, and it lets you build new workflows.

**Aakash Gupta** (00:00:37)

This is the power, right, of Cloud Code that you were saying. The

**Carl Vellotti** (00:00:40)

last thing that makes this really cool and much more powerful than an LLN. This is actually crazy.

**Aakash Gupta** (00:00:46)

Why has cloud code taken off so fast? How do you think it's reached? 500 million ARR in a few months alone. This

**Carl Vellotti** (00:00:52)

is my secret weapon for helping me create.

**Aakash Gupta** (00:00:54)

The last question you wanted your coworker to say, did you use ChatGPT to do this? Really quickly, I think a crazy stat is that more than 50% of you listening are not subscribed. If you can subscribe on YouTube, follow on Apple or Spotify podcasts, my commitment to you is that we'll continue to make this content better and better. And now on to today's episode. In today's tutorial, we're going to take you from beginner to Cloud Code hero so that you can create a co-pilot to make you more productive. And today's guest is Carl Velotti. He runs the largest product management Instagram account out there. He has been a senior PM for many years. Carl, welcome to the podcast.

**Carl Vellotti** (00:01:35)

Hey, thanks for having me. I'm super excited to be here and I'm really excited to talk about Cloud Code. It's one of my favorite features that I've found in sort of the new AI era. And I have a lot of really good stuff to show you guys.

**Aakash Gupta** (00:01:46)

If somebody with zero technical experience is listening right now, why should they care about learning cloud code?

**Carl Vellotti** (00:01:51)

Yeah. So cloud code, as you start to do more product management work and you start to see all these different use cases for LLMs, you sort of start to feel a little bit limited. You're in the chat interface and you're prompting and then now there's projects and you can bring in files and you can manually tell the AI, hey, please reference this file or hey, I found this prompt online. I'm going to copy and paste it in here. But then you want to reference that prompt in the future and it's not really easy to get to. And Cloud Code really just does all of that. It takes you out of the interface of just a chatbot. It puts you into a file system where you can just bring in and dynamically use any of these things really however you want. And it's super flexible so you can really easily adapt it to sort of any kind of workflow that you already have.

**Carl Vellotti** (00:02:38)

And it lets you build new workflows as you get better and better at using it.

**Aakash Gupta** (00:02:42)

How is Cloud Code different from GitHub Copilot or Cursor or Lovable or Replit? We keep hearing it's better if you're on Twitter, but what makes Cloud Code better?

**Carl Vellotti** (00:02:52)

Yeah, so Cloud Code, really, it is just an awesome way to use an LLM for all types of things. So you can use it for code, of course, it's in the name. But Cursor and these other IDE-based systems, they're really meant really just for coding. So if you want to do stuff like research, you want to do stuff like writing a PRD, you can prompt them to do it, but they're not really built out of the box for it. And the really nice thing about Claude code and one thing that just makes it sort of nice by default is that Claude is really, in my opinion, is the best writing agent or is the best writing LLM. For sure. You can use it for... writing documents and creating, doing research in ways that ChatGBT, while they're good models for coding, they're just not as good at writing.

**Aakash Gupta** (00:03:38)

Everyone can recognize ChatGPT's writing. Claude is the writing partner of choice. How does Claude Code compare to other CLIs out there?

**Carl Vellotti** (00:03:45)

Yeah, so the really amazing thing about Claude Code is that it is a completely new interface, an interface that I think people wouldn't even really expect a revolutionary new product to go to, which is the Terminal. So it's just purely text-based. It basically doesn't even have its own interface at all. And there are a couple other products like this. Google has come out with one since Claude, their Gemini CLI. OpenAI has their codex. I would say because Claude was first, it's just the most polished of any of the models or any of these options out there. It's tool use is basically perfect. It's use of agents and sub-agents is basically perfect. So, you know, the meta around this changes really fast and I've heard good things about OpenAI's codex, but I think right now Claude Code is just, it's the first one and they just really have it the most polished and sort of the best vision for this early on.

**Carl Vellotti** (00:04:38)

And that's why of these sort of options of the CLIs, it's still the best.

**Aakash Gupta** (00:04:42)

And people, this is not $200 a month. Whenever I talk to people, they're like, I don't want to shell out the money for Cloud Code. You can use it on the $17 per month pro plan. So I'm really excited to get into this. Can you show us in action how this looks, Carl?

**Carl Vellotti** (00:04:55)

Yeah, for sure. One thing I'll say on the pricing is we'll talk about it a little bit today. I'm going to be using the max plan, but I'll show you some sort of hacks and things that you can do so that you can do basically everything we're demonstrating today just on the pro plan.

**Aakash Gupta** (00:05:09)

Awesome.

**Carl Vellotti** (00:05:10)

Okay. Let's get into it. So to start off, we'll just go ahead and get it working. Yeah. So in order to get us started here, we're just going to go to Anthropics quick start guide. As you can imagine, it makes this very quickly to get going. They have this NPM install method, which was the original one, but they have an even newer way that just makes it really fast and basically only one command you have to do. So if you scroll down here to this native install section, I'm on a Mac, but this works on Windows or really it's the exact identical process for Windows. But for the Mac, you just copy this command. So now what we're going to do is we're going to take this command and we're going to do something that's going to seem a lot of scary to anyone who's not an engineer.

**Carl Vellotti** (00:05:50)

We're going to open the terminal. And so what a terminal is in general is it's just sort of like a command line interface for you to input commands, and they will just talk directly to the files on your computer. So to starting, we're not really in a folder or anything. We're just at base, so we're just on my computer. And all you do is you just take that command that we copied from the quick start guide, you paste it, and then you hit enter. And what this will do is it kind of runs the command, it's going to this website and it's grabbing the code it needs to set this up, setting up Claude code, and now it's installed. So that's it, literally one command, you put it in and now we're here. And then to get Claude going, you just type Claude. And now we are in the terminal and we have launched Claude code.

**Carl Vellotti** (00:06:35)

So to start, this is going to be very familiar if you've ever chatted with an LLM. It's that interface, but just with no images or no text or anything. So we'll just say, hello, Claude. And now we'll kind of talk about the UI here that it does have a little bit more, but now we are just talking to Claude and we are in Claude code. So there's not too many commands or anything you really need to know. You can basically just work with it exactly like you would talk to anyone or talk to an LLM. The commands that are good to know Uh, we're going to use one a lot called clear, which we'll just basically take whatever conversation we're having and we'll reset it. Uh, that's just to sort of manage context so that as you're going, it doesn't pull information from the past conversations.

**Carl Vellotti** (00:07:23)

And we'll, we'll talk about the other commands as we go, but really at this point, all cloud code is, is even though we're in a command line interface, we're just using natural language to talk to it.

**Aakash Gupta** (00:07:34)

Awesome. How does this differ from like a full IDE?

**Carl Vellotti** (00:07:38)

Yeah, so we actually are going to jump into an IDE in a little bit. The main thing that's different here is we don't have a good way of referencing files from this because we can't see what they are and drag and drop them. So as I mentioned, when we launched this, we're in just the base level of my entire computer. What we actually want to do and the way that you'll use Cloud Code is you're going to open it up in a specific folder. And so what I'm going to do here is I'm going to go ahead and close this terminal. And I have a prepared file for us today. And what I'm going to do is you just right click and then you're going to create a new terminal at that folder. And just to kind of show you what's in this folder, this is sort of, you can imagine this as a demo internal wiki that you might have at your company where you have a bunch of sort of data that you've uploaded from, you know, that you're already working with at your company.

**Carl Vellotti** (00:08:31)

And so we have, we have data, like some customer interviews in here. We have We have docs from business meetings, and then we have some code. So we'll be using these files sort of throughout this whole demo. And just kind of to call it out, you can either create these files as you're working with Cloud Code, and it will do that. Or if you're using this at your company or using this for any personal use, it's really easy to pull in files from Notion or Google Drive. And we'll get into that later. But for now, just sort of assume that we have this information about our company in here, and we'll work with that for the demo.

**Aakash Gupta** (00:09:03)

So

**Carl Vellotti** (00:09:05)

back to the terminal. So now we are in this specific file for Cloud Code. So again, we'll launch Cloud by typing Cloud. Now we are in this. So we can ask questions about sort of anything that's in here. And so one thing that we'll do is, for example, we have these customer interviews. So we can now ask Cloud, how many customer interviews have we done? And this will just go through that, that project and it will search for us anything that's in there. So right now it's searching, you can see it's hustling. Okay. So it found those three interviews and then you can ask questions about, you know, any of those interviews. So, um, I'm going to use, I'm using a tool here called the whisper flow to help me just dictate commands. Cause it's a little bit faster, which I highly recommend. Uh, can you summarize the top takeaways from the interview with Jessica?

**Carl Vellotti** (00:10:02)

And so it has all of its little, it's smooshing. So what it's doing is it's reading that file and it is using these tokens, which you can see here, and is basically going to read that file and just respond to us like it would, like any LLM would. And so it's kind of summarized here those points. And then you can ask it, you know, can you summarize the differences between the interview with Jessica and Marcus to tell me what's different between healthcare needs and retail needs? And the sort of demo project here is based on a fictional company that I called Streamline AI. So it's like an automation builder. So the answers will be sort of based on that. You can kind of imagine, I think we'll talk about this product later, N8N. It'd be kind of a version like that where you can build workflows.

**Carl Vellotti** (00:10:48)

So here it's telling us, it's done this analysis. So it's taken our, these are just raw customer interviews that we had in this file. And it's looking at them between healthcare and retail, and it's given us this summary. So

**Aakash Gupta** (00:11:01)

this is the power of cloud code that you're saying where it's a better interface than chat. It's automatically reading the folders. It's figuring out how many files are in there. It's going in there and reading them. It is the ability to context engineer much faster.

**Carl Vellotti** (00:11:18)

Yes, exactly. That's a really good way of thinking about it is, you know, as we've moved from prompt engineering into, you know, we've gone into context engineering, what you can give the LLM to work with is so key in what it's able to actually do. And that's a through line that we're going to see through everything that Cloud Code is good at is just a really fast, simple way to give it the right kind of context for any of these different kinds of things you want to do. Okay, so we've seen it search files and kind of analyze files here. It can also search the web. So as I mentioned, we're gonna use clear a lot just to keep the context clear. We've seen it use files and read files and analyze files. Let's go ahead and show how Claude can search. So we're gonna go ahead and have it Do a quick search on the iPhone that just came out this week.

**Carl Vellotti** (00:12:06)

Date this video a little bit. But what it's doing here is it's running the search. It's looking for anything that came out September 2025. And it usually seems like it checks 10 sources. So we'll see what it comes back with.

**Aakash Gupta** (00:12:21)

I love it combobulating.

**Carl Vellotti** (00:12:23)

Yeah, convobulating, we can see the time, we can see the tokens, which is a pretty interesting aspect of the Cloud Code interface. When you're using ChatTBT or using Cloud, they never actually tell you the amount of tokens they're using. So I think when you see the pricing is $2.50 for a million tokens or whatever it is, you never really know what that means. So this shows, so it's counting up these tokens really fast. Okay, great. So here it got a little confused about my exact request, so it's something we could probably make better, but it did grab the iPhone Air key specs. It just didn't do the direct comparison. So I think that's probably something just with the prompt. But yeah, so just interesting. You can ask it to sort of do any sort of search, and it's very good at search. I know early on there's sort of people thinking you had to implement perplexity in order to have it do the search, but overall Cloud Code is quite good at doing the search on its own.

**Carl Vellotti** (00:13:22)

Nice.

<!-- sponsor -->
**Aakash Gupta** (00:13:23)

I hope you've been enjoying this tutorial on Cloud Code. This episode is brought to you by Linear. And if you love coding AI agents, you will love Linear. because you can actually use linear to call your coding agents. So in your task management software linear, you can create beautiful tasks, then you can call coding agents like CodeGen and linear to actually execute on those tasks. This is a magical way of working. If you've been watching the podcast, you've heard from numerous startup founders about how the linear method for building products has revolutionized how the way they work. because they go away from enterprise software that's very complex to startup software that's really fast. It's no wonder Cursor, OpenAI, and Perplexity are using Linear. So visit Linear.app slash partners slash Akash. That's Linear.app slash partners slash A-A-K-A-S-H. And take advantage of this revolutionary new way of working.

<!-- sponsor -->
**Aakash Gupta** (00:14:28)

Now, back to your Cloud Code tutorial.

**Carl Vellotti** (00:14:31)

Okay, and then the last thing I want to show before we kind of get into more complicated stuff is just that even though this is a completely text-based interface, you can bring in images. So you can either drag them in. So this is a graphic that I prepared and posted on LinkedIn recently. So I can say, can you please analyze this image and give me feedback? I didn't clear the context, which normally that would be the best thing to do. In this case, I think it will be okay. And so when you give it an image, it just sort of says like image one. You can, of course, do, you can post in screenshots or anything like that. And it will use it. So that's very helpful for like debugging. So in this case, you can kind of see it was able to see the image and then give us, give me some feedback here.

**Aakash Gupta** (00:15:17)

Nice.

**Carl Vellotti** (00:15:18)

Yeah.

**Aakash Gupta** (00:15:19)

Search images, context from files.

**Carl Vellotti** (00:15:23)

And the last thing that makes this really cool and much more powerful than an LLM, for example, or one like a normal interface that you're using, is it can actually run code. We're going to ask it to do something that you could never really ask ChatGPT to do, which is I'm going to give it the repo for a YouTube transcript API. And I'm going to say, please get the transcript from this video. And then the video I'm giving is a past product growth one, really good one on building agents. And then put that output in an MD file. And what we're going to see is that all by itself, without really us needing to know exactly what the code is or really looking at it, but just knowing that this API exists, we can give CloudCode this information and it will... Just run it. And now we're also seeing the first really, really unique feature of Cloud Code, which is its ability to create plans for itself.

**Carl Vellotti** (00:16:16)

So do you see this to-do file or this to-do here? So what it did is it, instead of just sort of immediately starting, it actually created a task list for itself. So it says, I need to install the YouTube API. I need to create a script that will use that API. And then I need to extract the the video and then I need to put it into a file. And so what that basically means and what really helps Cloud Code be much more agentic is it's creating a task list for itself and then it will go through those one by one and it will check itself and it won't move forward onto the next task until it actually has done those things. And so here we can see that it wrote the script. It ran it. It was able to pull in the file. It put it into this.

**Carl Vellotti** (00:17:03)

It was able to pull in that information, and then it put it into this new file. And it's just sort of confirming here that it did all that. So very cool. And you can already kind of see, like, you can bring in any code that you find on GitHub or that you see people posting. And Cloud Code can just basically use it right away.

**Aakash Gupta** (00:17:22)

I think a lot of people shy away from those GitHub repos and stuff, but this is a great way that you can actually interact with it, even if you're pretty non-technical, because we're just talking into Whisperflow here.

**Carl Vellotti** (00:17:32)

Yeah, exactly. I think for me, since I've started vibe coding, that's been one thing where I remember used to see cool stuff in a GitHub, and anytime it's a GitHub link, you know you can't really use it or you know it's going to be hard to get set up, but now those are perfect for just giving LLM and they can work with it right away. So, okay. So we created this file. We created YouTube transcript.md. And if we go into like our overall sort of file that we're working in, we'll see it here. But now the question is like, how do we actually work with these files? How can we actually view them? How can we see what's going on? So what we're going to do now is we're going to go ahead and we're going to exit this terminal and we're going to go ahead and we're going to enter an actual IDE.

**Carl Vellotti** (00:18:14)

So, um, you can use any IDE for this, my preference, just because it's like sort of the one that I've been using otherwise is cursor.

**Aakash Gupta** (00:18:22)

And so

**Carl Vellotti** (00:18:22)

this is kind of meta because we're using cloud code in cursor, but I'll show you why we're doing that.

**Aakash Gupta** (00:18:28)

And it seems like just about every tool has released this functionality where you can use cloud code in it now. Yeah.

**Carl Vellotti** (00:18:34)

Anything with the terminal. And that's going to be basically like any IDE. Um, so here we're in a cursor and there's really the main feature that makes cursor cursor is this sidebar. um, where you can, you know, you can prompt here and then it will do the coding. We're going to not use that at all today. Instead, we're just going to, I'm going to close this. And what we're going to do is if you hit control, um, the squiggle, I'm not sure back to back tick, control back tick, it will open up the terminal down here. And

**Aakash Gupta** (00:19:03)

again, we're

**Carl Vellotti** (00:19:03)

still in that same folder. And then to start get Claude started, we go ahead and type Claude. And so now it's the exact same thing that we just saw, but instead of being in like an isolated terminal window, we're just in the terminal in cursor.

**Aakash Gupta** (00:19:16)

This is a good point. And this is

**Carl Vellotti** (00:19:17)

a reason where being in cursor, one thing that's really nice is we saw those plans from earlier. There was the pro and the max and the pro max. If the pro plan can really do almost everything that you're going to want Claude to be able to do. Sonnet is still a really good model for researching and for writing documents and just writing in general. Where you might want the max or the higher level plans is for coding because then you get access to Opus and those models. But honestly, if you're in Cursor and Cursor is only $20 a month separately, you get access to that model plus all the other really good models. And so you can pretty easily use Claude Pro for the Claude code things that you want to do. And anytime you actually really want to do some heavier coding, if you just get cursor and then you use, you can use the absolute best models for quite a lot cheaper.

**Carl Vellotti** (00:20:05)

That's a good sort of hybrid way to use Claude code for non-coding things. And if it gets too complicated, just go into cursor and use the better models.

**Aakash Gupta** (00:20:13)

Nice. So $37 a month.

**Carl Vellotti** (00:20:16)

Yeah, and I'd say very high ROI for most product managers on that. Okay, so we are now here in cursor, and we can go ahead and we can, the transcript that we just pulled in, we can look at that here, and now here it is. So easy way to visualize it, and then in cursor, you can always preview, which will basically take that markdown, which is just sort of a, here it's just raw, but if you can actually format it and see how it would be published online, if you just preview it. So here we can see the bold is nice and everything here. And then if there's anything you wanna edit, you can double click and that will take you into the file and you can edit it here. But, so this is just basically showing the rest of the demo we're gonna be in here just because it's a faster way for us to kind of see what's going on and pull in files to give the LLM to use.

**Aakash Gupta** (00:21:08)

Got

**Carl Vellotti** (00:21:08)

it. Okay. So the first thing that you're going to generally want to do when you start using Claude code and you open up any project is it has a command called init, which is just the initialization command. What this will do is it will basically just take whatever, Claude just imagines it gets dropped into this file structure and now it has to figure out what's going on. And that's kind of what it's like as a human too. Even if you know what a project is supposed to do or the files that are supposed to exist, you still have to look around and kind of try to figure it out. Claude will just go through and analyze everything. And what it will do is it puts together what's called this Claude file, all caps Claude. And it's basically saying, okay, here's what I found. Here's the structure of this file.

**Carl Vellotti** (00:21:58)

Here's like the core components of how it works. And here's how a person can get it working. And so in this case, because I already had one, but now I've run it again, it will update this. And so on one hand, this is just like a helpful sort of thing for you to see how the whole sort of repo is structured. But what's really powerful about this is that every single sort of session that you have with Claude, it will reference this Claude file. And so you can imagine this is very helpful for it when you ask it a question. It doesn't have to newly search or newly find that context every time. It just already kind of knows how your project is built. And this is also where you can give it rules like never commit to GitHub without asking me first. Or I always want to use this style of writing.

**Carl Vellotti** (00:22:48)

Or when we're doing a research or when you're doing a web search, make sure that you give me the results back in this format. And so it will always have this. And it's different than even like a prompt because in a prompt, let's say you're having a conversation. and you know you say something you say never commit without asking me first and then you know five or ten messages later it might start doing it again that's because it's sort of it's getting further back in its context and its context window is only so large but everything that's in this clod file is in its sort of memory all the time got it and uh the quickest way whenever you're, let's say you, you realize Claude did something that you didn't want, or you want to, you're like, Oh, this would be a good thing that I should add to the Claude file.

**Carl Vellotti** (00:23:31)

If you just do sort of number sign and then, you know, always ask before committing anything to GitHub, then that will just automatically add it to the project memory and it will be there. And, uh, we won't go into it too much today, but the other sort of main use of this Claude, uh, types of files is you can put them into sort of subfolders. And then anytime it's doing something in those subfolders, it will follow those rules. So let's say you have a folder that's really all about helping you write PRDs. If there's specific rules you always wanted to keep in mind for those, you can create that file there.

**Aakash Gupta** (00:24:05)

Okay, got it.

**Carl Vellotti** (00:24:07)

Yeah. Okay, so speaking of creating PRDs, now we're going to go ahead and we're going to look at how does all this sort of easy context engineering within Cloud Code really make it powerful for, you know, doing things that product managers do all the time. So in this file, and this is something that would be really helpful to have for your own self, is we have... this business info. So this is basically like information around just how does this business work? So as I mentioned, it's a fictional company here called Streamline AI. It's an automation builder. So you can have cloud code anytime you're doing something where you want it to give a very specific response that makes sense for your business rather than just, you know, a general LLM response or, you know, you just, instead of you just typing, you know, one sentence about what your business does, You can have this document that it can reference at any time that tells it what your business does.

**Carl Vellotti** (00:24:57)

And as another example, you can also have writing styles. So let's say whenever you're writing something for an internal audience, you want it to have one style. If it's a more technical document, you want it to have another style. And so what we can do is you can sort of combine all of these things really quickly. Okay, so now what we'll do is we will show off, we've looked at how Cloud Code can read files and write files and can reference some of those dynamically. What we're gonna do here is we're gonna use all those capabilities in sort of one prompt to show you why is Cloud Code so awesome. And so what I have here is I have this prompt Basically what you want to have as part of your project is you want to just keep information that you might want to reference often.

**Carl Vellotti** (00:25:42)

So in this case, in this project we have We have some writing styles. So we have like an internal audience style, a technical style, user friendly style. And then we also have business info. So this is a great one for whatever you're trying to build or whatever you're doing. If there's information that you want the cloud code to actually really know, instead of just saying, oh, I have a business that does this. If you put together a document that says, here's my business, here's all the different things that it does, here's key information, then anytime you need to do something like write a PRD, you can reference that information all together without having to go copy and paste it in. It's just easy to bring it in here. And then the other thing that's also helpful to have, LLMs are always much better if you give them examples.

**Carl Vellotti** (00:26:29)

You can, instead of even just providing individual examples, you can build a folder that has a bunch of examples of things that you like. So in this case, I have this example PRD. So let's say I'm working at this company, a bunch of killer PMs who are writing some really great PRDs. You can use those as examples for your own PRDs. And so what we have here is we have this sort of super prompt that is taking in saying, build this feature with GPT real time, which is OpenAI's new speech to speech model. You can use this business context from this document and then use these example PRDs with this writing style. And so just by having that stuff already pre-created, we can run this prompt and then we'll do all of those things altogether without us having to go like try to find all that information and create this prompt.

**Aakash Gupta** (00:27:17)

I love how the folder structure is coming in clutch again here.

**Carl Vellotti** (00:27:22)

Yeah, exactly. That folder, just keeping this organized and keeping all of your information sort of where you, in a way that you can quickly give it to Claude makes all this so fast. So what we're seeing here is it's come up with another one of those plans for itself. So it recognizes that it doesn't know what GPT real time is. It just came out like two months ago. So it's researching that and then it's gonna read the business info and it will create the PRD and then it will make sure it goes with those writing style. So it's taking all of that information that we just gave it and it made a plan for itself. And we can kind of see it running through it here. reading business info, it's figuring out what that technical style is, and right now it's mainly doing this web search.

**Carl Vellotti** (00:28:07)

So it finished those things, and then the tokens are counting up again. So it finished those tasks, and now it's going to actually write the PRD.

**Aakash Gupta** (00:28:15)

It's fun to watch it just cross off to-do list items.

**Carl Vellotti** (00:28:18)

Yeah, there's a little bit of a little dopamine burst as you see it work through it, almost like when you complete your own to-dos.

**Aakash Gupta** (00:28:26)

Yeah.

**Carl Vellotti** (00:28:27)

Okay, so it did all the research and now it's putting it together into a PRD. Yeah, we see these tokens. At first, you can see every individual one and then it just becomes a decimal point. Tokens definitely get used up very fast. Luckily for Sonnet, which is sort of the... the main model and not their best model, which is Opus, you get a lot of usage on both the Pro plan, which is the $17 one, and the Max plan. With Opus, which is the better model, which is helpful for things like coding, these tokens, as you can see, they're counting up very fast. They get used up quickly. So that was kind of more of my recommendation for using Sonnet for... you know this type of stuff that we're doing here but then maybe coding in another less expensive tool might be the way to go so now we can see that it created the prd and sometimes the first time it does something when in a session it will ask to make sure it's allowed to make that change in the code base uh here it's just saying okay i made this can i add it and then what we're going to do is we'll go ahead and just say yes and you don't have to ask again one command i'll probably demonstrate later is there is like a YOLO mode where you can just have it do whatever it wants and it never has to ask.

**Carl Vellotti** (00:29:47)

We're literally having it like, you know, really work with the files on your computer. So in this case, we're in a contained environment, so it probably couldn't do too much damage. But you have to be very careful, especially if you're doing code based stuff with that permission.

**Aakash Gupta** (00:29:59)

Yeah.

**Carl Vellotti** (00:30:00)

Okay. So I said, yes, that's fine. And then it created our PRD. So let's take a look at this quickly.

**Aakash Gupta** (00:30:10)

What was the command to make it look better here?

**Carl Vellotti** (00:30:13)

Oh, yeah, sorry. We're just looking here, and then what you can do is you can right-click, and then you just go ahead and go Open Preview. Oh, nice. And then I just did the Shift Command V. Nice. Okay, now we're seeing this. So it has our format that we wanted. This is modeled after the Akash recommended PRD. It has the problem statement and the goals. And of course, you'd still want to go through this and make sure it's good, but it's looking pretty thorough given the information that we gave it. And we asked it to use a more technical voice, and definitely it looks like it really thought through those technical constraints. And it even linked to a bunch of documents for us to use here. So this is a really good first draft of a PRD that you want to go work on from there.

**Aakash Gupta** (00:30:58)

And that prompt was so simple. It's really the power of the searching online to figure out what the real-time API is and then connect it back. So that's so cool.

**Carl Vellotti** (00:31:07)

Yeah, and ways that you could definitely... This is sort of still very hypothetical. I didn't give it a lot of guidance on the user experience we're expecting from this. But you can imagine that you might have met with your designer. You have a meeting transcript. You've met with your engineers. You have meeting transcripts. You have all this information from... other things that you've sort of put together and then now you can give it all of that and it will really use it correctly in these files. So that's just a good example of how it can put together all this information and then output something really awesome without you having to do a ton of extra work.

**Aakash Gupta** (00:31:40)

you just mentioned correctly i think that there was this paper which was basically like as you give things these lms more context sometimes like there's a dip in the quality if you just i think it's like token degradation or something like that is the context they're talking about there do you see that where you can overload it with too much context

**Carl Vellotti** (00:32:01)

I think the nice thing about Cloud Code is that it makes it pretty easy to not do that in the sense of like, okay, we finished this task, now we can clear. And I think it makes you a lot more cognizant of the fact that you are using context because it's telling you the tokens and it makes it really easy to start new sessions. Where I think in like a chat bot system or something, it's very easy to just keep chatting, keep chatting, keep chatting. And that's where I think it starts to get a lot worse. I think if you're able to just give it all of that information upfront, then it really actually does use it better than if you're kind of putting it together over time.

**Aakash Gupta** (00:32:38)

Makes sense.

**Carl Vellotti** (00:32:39)

Yeah. And the context windows for these things are still pretty huge. You know, like if it's a million tokens or if it's, you know, 200,000 tokens, even if we were giving it like a lot of information, we're not uploading like books into this. So I think it's still usually like well within the context window of what it's able to handle.

**Aakash Gupta** (00:32:58)

Got it.

**Carl Vellotti** (00:32:59)

Yeah. And then, yeah, so that we just did kind of like a pretty beast mode example. One other sort of quick use case I'll show is let's say we had a folder with these meeting transcripts. You can also just have it say, hey, please, please take these transcripts and then just add a summary with action items to the bottom. So it doesn't always have to be super beast mode. It's also useful for just like smaller things as well. So here it's going to just go into our folder. Let's say, for example, you are, you know, all day you just were in meetings back to back, which I'm sure product managers can relate to. And you haven't had time to go back through everything here. You can just say, Hey, all of everything is in this document or in this folder. Can you help me figure out what all the action items were?

**Carl Vellotti** (00:33:42)

And this one, it's very fast, right? The last one took some time because I had to search, but this one it's, um, looking at the directory, it's reading the transcripts and now it's adding the summary.

**Aakash Gupta** (00:33:52)

And it looks like it's going in and changing your files right then and there, which is not anything you're going to be able to do with a chat bot.

**Carl Vellotti** (00:33:59)

Exactly. Um, So here we're opening up this document, and then we scroll down to the bottom, and we're seeing the meeting summary and then the action items. In this case, what we're going to look at next is how you can get more structured outputs. I didn't tell it really what types of information I was looking for for these outputs, but Claude is still, like we were saying, it's good at writing and still pretty smart. So it figured out that the person that it needs to assign these to, exactly what they were going to do, and then a due date. So let's say that you did have a much more specific format that you wanted these action items in. Now I'll kind of introduce this concept of you can build your own commands. So we looked at, there's a bunch of sort of pre-built commands that Claude has, but you can also create your own commands.

**Carl Vellotti** (00:34:48)

And you can think of these as basically stored prompts. So let's say, for example, that we had, a specific format that we always wanted notes to be structured in.

**Aakash Gupta** (00:34:59)

What we can do is

**Carl Vellotti** (00:35:00)

we can build a command for that. So I have this command that I've created here called meeting notes. And let's say here it's like extract key information. I want it in this format. And then some things that the one that we just prompted without telling it anything that we wanted. We can say, make sure that you list the action items, the important metrics of data that were mentioned in the meeting, and then specifically next steps and risks. And so what you can do is you can do something similar to what we just did, but you can run a command. So you can say meeting notes, and then you can just, for example, one nice thing for the cursor, you could just even bring it in here. And now it will use that command, which is basically the saved prompt for that file. And so you can kind of think like when you're on Twitter, you're on LinkedIn, people like to share these big prompts all the time.

**Carl Vellotti** (00:35:47)

But, you know, it's kind of like, what am I exactly going to do with it? Or when am I really going to use it? If you start to... figure out which ones are really useful to you. You can save those into your file so that when the right time comes, you can just easily trigger it rather than, you know, having to go into your bookmarks and in Twitter that you probably never use, um, and find it and then copy and paste the image.

**Aakash Gupta** (00:36:08)

Well, yeah. Or go into your outdated prompt library that you set up two months ago and be like, Oh shoot, I didn't even put this prompt in there.

**Carl Vellotti** (00:36:16)

Yeah, exactly. Uh, so this is pretty similar to what we just saw, but we asked it to do that on this folder. And then, um, Yeah, for this one, I asked it to put it at the top. So it's kind of, these are maybe much better summaries from the meeting rather than the one that we just sort of prompted it to do. So

**Aakash Gupta** (00:36:34)

again,

**Carl Vellotti** (00:36:34)

you can create all these commands and you're really starting to see how you can mix and match and put these things together in like almost any flexible way. It's actually crazy

**Aakash Gupta** (00:36:44)

because I think one of the big challenges, if you're using, let's say, chedgpt for meeting notes or whatever out of the box is making things in your own style, right? Putting it in your own voice. The last question you want is your coworker to say, did you use chedgpt to do this? Because that usually means that they didn't think it was very good, right? And so here you're inflecting your own style through these simple markdown files that you then reference in the prompt and create commands around.

**Carl Vellotti** (00:37:12)

Yeah, exactly. And then you can kind of do... I don't have this demo prepared, but I just thought of it. You could do something like... Let's say you had a file or something for your writing style. I have this internal audience style. You could do something like... Please write... Okay, let's do this. Please write a Slack message for me to send to... Sarah asking her the status update on her items. It's January 28th and she hasn't completed them yet. So I just wanna double check. So here we're saying, okay, we have this file that says the things that Sarah was supposed to complete. So we're gonna give it that file. And then please use the tone in this file. And then we can say, please use this tone for my internal audience. And so this is sort of, now it's gonna, it has the context of what happened in this meeting.

**Carl Vellotti** (00:38:04)

It knows the action items that Sarah is supposed to be completed and it knows the style that you wanna write in. And so it can help you put together the Slack message really quickly.

**Aakash Gupta** (00:38:12)

And could you connect this actually to your Slack?

**Carl Vellotti** (00:38:15)

Yeah, you could. We will talk about MCPs a little bit later, but Slack is pretty easy to connect into Claude. I think in that case, though, I don't think it would look like it was sent from you. But what you could do is you could have it send it to yourself as a message from the Slack MCP, and then you could copy and paste it. Awesome. And so this is like a pretty good message. Like, hey, Sarah, quick check in on the items that were due yesterday from the meeting that we had last week. And then it's saying the roadmap proposals. I know these directly impact our objectives. And now it's kind of a good message. Like this might be even more information than you would include and you could decide. But like it even knows. like what was talked about in that meeting in relation to the business.

**Carl Vellotti** (00:38:58)

And so it's saying, I know these directly impact our Q1 strategic objectives and the ARR recovery plan that we have. Can you please make sure that we actually get this done because we have dependencies here. So this is an example where you can do pretty like interesting stuff, even as like a product manager that would be hard to do otherwise all together with cloud code.

**Aakash Gupta** (00:39:19)

Very cool.

**Carl Vellotti** (00:39:19)

Yeah. Okay, so we just covered slash commands. And what we're going to move on to next is we will move on to planning mode. So, so far, all that we've done is we've seen Cloud Code create plans for itself. But sometimes if you're going to be doing something a lot more complex, then you want to actually sort of plan with the LLM first. If you've ever done any coding with LLMs, you know that you'll say, what would it take to change this so it operates this way? And then LLMs, they're just built to be helpful, and so it will just start doing it. It will just say, okay, I will change that file. And then you realize that pretty much as soon as it gets started, that wasn't exactly what you wanted it to do, or you know it didn't really have the requirements that it was supposed to have before it got started.

**Carl Vellotti** (00:40:05)

And so One thing you can do is you can always say, you know, don't code. Tell me, talk to me first. But even then, it won't really give it in like a consistent format. And for quad codes planning, there's just a much better way to do it, which is we've been on this auto accept mode. But what we're going to do is we're going to go into this plan mode. So you just do shift tab. And now we're in plan mode. And this basically does what I just explained where now it can't edit files. It can still search and it can still read files, but it can't edit anything. And so this is where you can kind of take a step back and you can work with Claude to sort of come up with a plan. And what it will do is it will actually pre-create that checklist that we saw before.

**Carl Vellotti** (00:40:42)

And you can look at that and you can make sure that the steps there make sense and that it's not forgetting anything. And then you can sort of let it go wild.

**Aakash Gupta** (00:40:50)

Nice.

**Carl Vellotti** (00:40:51)

So in this case, we're going to do something more complex that's going to combine a lot of the things that we've seen so far. So let's say we pulled in those YouTube transcripts earlier. Let's say that we are building a tool where we wanted to build a YouTube transcript summarizer, and we want to use an LLM. to summarize those transcripts for our product that we're building. There's a couple things that you have to figure out there. One is, what is the prompt that you want to use to summarize the transcripts? And then let's say that you can use any model you want. And so you want to know, is Gemini the best? Is ChatGBT the best? Is Grok the best? And so you want to create multiple prompts and you want to test against multiple models. And that would be pretty hard to do on your own because you'd have to take the prompt and you'd have to take the transcript and then you have to copy and paste it sort of into each chatbot and then you have to copy and paste.

**Carl Vellotti** (00:41:41)

You have to do all this comparison. But what we can do with Claude is we can literally have it write those prompts and then we can have it run those prompts against the LLMs using code and then we can have it put together the files for us in order to review. So I have this prompt sort of already made, but just saying, I'm making this tool that analyzes YouTube transcripts. I want to test these prompts. So I want you to come up with three unique prompts, one for short, one for medium, and one for long. And then I want you to run the models that I have in this project against those prompts. And then here I've already uploaded the keys for it to be able to run that code. And then use this transcript as an example. So we're still in plan mode. So let's see what happens.

**Carl Vellotti** (00:42:23)

So we're asking it to do a lot. So we want to make sure that it's going to get it right when it does actually go execute on this. Because there's some things here that, you know, this is a lot to ask the LLM to do at once. saying, I'll help you do this. So right now it's going to basically explore the code base and figure out what we can do here. So it's seeing the code that we added earlier, which was the YouTube transcript API. So it's looking at that. It's looking to see if we already have any prompts. And then it will come up to us and it will tell us a plan. So it says, perfect. I have a comprehensive plan or understanding of your project. But I understand that you already have this transcript tool, but now I understand what you're trying to do.

**Carl Vellotti** (00:43:04)

So what it's done here is it's come up with this plan. And so it's saying, okay, the current state is you have this, and then I'm going to create these three prompts. So you want to look at these. One is going to be an insights prompt. One is going to be an educational breakdown, and one is going to be a critical analysis. So that's the short, medium, and detailed. So that looks pretty good. And then we're going to look at these steps. But then let's say I just realized, oh, I don't really understand. It's going to put these new files as .txt. But for everything that we're doing, we actually want those as markdown files. So what we can do is we can say, no, keep planning. I actually want these to be in markdown files. And then another thing that we can kind of see with the output is that maybe it's not going to put those in the right types of files.

**Carl Vellotti** (00:43:54)

So please give me these files, one file per prompt, and for each prompt, show me the three different responses from the three LLMs. So now we've basically modified the plan. And if we had just had it run through that first time, then I think what it would have given us is basically like nine files for all the different prompt outputs, which isn't what we would want. And that's sort of a small example of a correction, but sometimes it'll really get like much bigger pieces trying to infer what you want wrong. And this lets you catch those before it happens. And then now this looks pretty good. And now we can say, OK, go ahead and run it. And

**Aakash Gupta** (00:44:30)

now it's

**Carl Vellotti** (00:44:30)

going to go ahead and do all of those things that we just said all at once without us having to watch it at all. So this kind of gives us an opportunity to do something kind of fun, which is while this is running, we can actually just launch Cloud Code again. So we're going to go into another terminal. And we're just going to launch Claude again. And so this is a completely new, fresh instance of Claude. While this other one, it's doing the work for us. It's created this long to-do plan. But now what we can do is we can go into Claude here and we can do something different. And so you can kind of imagine, and I've heard that there are engineers who are really good at this. They'll have like six instances of Claude code all running at the same time.

**Aakash Gupta** (00:45:16)

Nice. Yeah. I sometimes have like three or four cloud chat windows, but this is like even better.

**Carl Vellotti** (00:45:21)

Yeah. Yeah. It's kind of like, um, I feel like maybe I'll do it with like a deep research in chat GPT where that will be running in one place and then go somewhere else and use, use chat GPT in another place. But yeah, this is where you can just really have it doing like all this work at the same time. This is kind of a good opportunity to start talking about agents. So what we've looked at so far is we've seen sort of some like agentic capabilities where It comes up with this, yeah, it's figuring itself out over here. Where it comes up with this plan and then it will go through that and that's kind of agentic. But one, another thing that you can do that's really cool is you can, just like we right now have two versions of two separate instances of Cloud that are running.

**Carl Vellotti** (00:46:03)

Cloud can actually make itself have multiple versions of itself that are running. And that's

**Aakash Gupta** (00:46:09)

where

**Carl Vellotti** (00:46:09)

the agentic sort of capability of Cloud code starts to become really cool. So as an example, Let's say that we, you can like parallelize tasks. So right now we have these three customer interviews, the ones that we referenced earlier. So let's say that we wanted to get summaries from like key insights from all three of those interviews. We could say, hey, Claude, use this folder and then go through each one and tell me the insights. But what we can also do is instead of doing that, we can actually say, I want you to go through those interviews and I want you to analyze them all in parallel. And what that will do is it will create three instances of like a UXR agent and then it will, for each one, it will give it one transcript and then they'll just work completely in parallel. So I'm going to start this.

**Aakash Gupta** (00:47:01)

Is the UXR agent defined in your files or it'll figure out what that is?

**Carl Vellotti** (00:47:05)

Yeah, great question. So in this case, this is an agent that is not defined. So it will actually just create like a new, it'll just sort of spin it up on its own. It'll figure out what that should be. But it's kind of like what we looked at earlier where you can ask it to do something or you can create a command that has that thing structured in a way that you actually want it to have happen. So here it looked at the files of those interviews and now we have three tasks all running at the same time.

**Aakash Gupta** (00:47:34)

Very cool. Can't do that in regular ChatGPT or Claude.

**Carl Vellotti** (00:47:40)

Yeah, exactly. And so, you know, this is a very basic example of these are just, you know, sort of an input, you know, analyze this thing and then append your insights to each one. But for some of the things that we've looked at that were much longer tasks, it could also do that. It could also, you know, run much longer tasks in parallel. So let's say you had some sort of prompt around wanting to do competitive research where you wanted to check these different files and use these different tools and uh do a bunch of different competitive research and then you could have it do that you could even have it figure out who your competitors are and then have it research all of those competitors in parallel so something that might take you know you it would take like a whole week if you're using an llm uh regularly it might take a whole day but this can get those types of tasks down to like a single hour

**Aakash Gupta** (00:48:28)

because it

**Carl Vellotti** (00:48:28)

can run all those things in parallel

**Aakash Gupta** (00:48:30)

crazy i'm sure burn a lot of tokens too

**Carl Vellotti** (00:48:33)

yeah exactly Okay, so it's just appending those insights onto these files. So now if we click into them, we can see that it's added key insights to the top of each of these. Okay, let's go ahead and go ahead and check back on that other one. Okay, so it's still working. It's still creating those prompts, and it's still running them. So that's just happening in the background, and it is... Yeah, still working. So another thing that you can do with agents, so what we just looked at is we just looked at using one agent or one type of agent multiple times at the same time. What you can also do is you can also have the same take one task and have it be approached by like multiple different types of agents at the same time. So an example of where that might be useful, let's say you have a slide in a deck and you want some feedback and you can just say, Hey, Claude, give me feedback on this.

**Carl Vellotti** (00:49:29)

But you might actually want a different perspective on how would an exec look at this? How would an engineer look at this? How would a designer look at this? So you can get multiple different types of feedback. And so Kind of to the point that you mentioned earlier, before with this UXR, this was not like a real agent that we defined. It was just it made its own version of that agent. You can actually build your own agents. And so here what we're going to look at is a couple different agents that we'll use to do this review. And what these are, they're kind of just sets of conditions of when this agent is... called up by Claude, how does it work? And they're really powerful because they are basically, as soon as Claude will give this agent that task, that agent is kind of spun up into like a new universe.

**Carl Vellotti** (00:50:15)

It doesn't inherit the context that it was in the rest of the chat. It doesn't really take any other information. It's just this agent as you can define it here with the task that it's given. And then it will output and then it will go back kind of to the original main Claude agent. And there's a lot of these. So here what I have is I have three sort of review agents. Once we go through these, I'll show you a bunch of other examples of the types of agents you might want to use in the Claude code project. Okay. So here... Okay, so to show this in action, what we'll do, so I'm gonna go ahead and clear this. And then what we're doing is we're gonna say, please review, let's say this PRD that we had written earlier, from the perspective of a designer, from the perspective of an engineer, and from the perspective of an executive, and then put it all into a new file.

**Carl Vellotti** (00:51:12)

And so what it will do, is it won't just create like new agents, it'll use those ones that we have defined here. And one thing that's kind of cool is with these agents that you've defined, you can give them a color. And so for example, if we go into the designer, at the very top, the color is pink. So we actually see that in the UI. I've seen one thing that people, it's very common on Reddit and I should have done it here. People will add like text faces to the beginning.

**Aakash Gupta** (00:51:38)

And so

**Carl Vellotti** (00:51:39)

you can, you know, you can really give these kind of like personalities and their own ways of approaching work. And so you can have like a skeptic or you can have a more like a more enthusiastic or more like a yes and type of agent. Just all these different sort of ways of approaching the work from these different agents that can, really tackle work in different ways. And it's interesting because the way that you define the agent, it really will sort of like approach tasks differently and will give you types of outputs that you will never really get if you're just using the main cloud code agent. And one thing while this is running that I can show, there are a lot of these agents, they're just basically like text files, right? If we look at this engineer one, like this is just a text file.

**Carl Vellotti** (00:52:23)

There are some really cool databases of these. One that I like is this sub-agents. And so there's just these big databases of like all of these different types of agents that will, can do work in different ways. And so in this particular database, there's like a few for product and these are really easy to bring in. So let's say that we, a legal advisor, of course, if you're working in a company, you're gonna wanna actually talk to legal, but maybe before you talk to them, you want to like get, just get an idea of like what are the big things that you might be missing. You can just come in here, you can either copy this file or you can just get this command And then you can come back to cursor, wherever it is. And then you can run that command. And now it just pulled it in.

**Carl Vellotti** (00:53:18)

So just like that, we now have a legal advisor in our project.

**Aakash Gupta** (00:53:22)

Oh, wow. That

**Carl Vellotti** (00:53:23)

we could use to review a PRD. I think it would be helpful in this particular instance for saying, I think it's easy as a PM to completely forget to consider what are the different types of regulations that might exist. So you can have an idea of what those are before you actually go to talk to legal and they tell you that you missed these big things.

**Aakash Gupta** (00:53:43)

Yeah, I imagine like this is really gold for experienced PMs. As you have like a year or two of knowledge, you can put in, here's all the other things we've encountered with legal issues. These are the main laws that end up coming up for a particular executive. This is what he said in past product reviews. So make it that executive's agent and just really load it up on real life context.

**Carl Vellotti** (00:54:05)

Yeah, that's a great example. That's like a really good example of where for your specific product and your specific industry, if you build up that knowledge and that file in here, then it's really easy to reference later, just like you're saying. Okay, so we had two tasks running in parallel. We had the first one, which was creating those prompts and then running them against the different types of LLMs. Then we had the other one, which was reviewing that file from the perspective of all those different agents. So let's go ahead and see how that first one turned out. Okay, great, perfect. I've successfully completed all tasks. Let me write a quick summary of what was accomplished. I created three unique YouTube prompts, ran them, and then you can see them in these files. So now we can go into these files and we can see, okay, so this was the, this was like, this is the actual insight.

**Carl Vellotti** (00:55:00)

So this is the one where it's supposed to just give the answers really short. And what we can see here is that it ran, It's basically saying, what was the prompt? And then here is the Gemini response. Here's the ChatGBT response. Here's the Grok response. And then you can easily kind of go through and decide, okay, well, I think this is the best prompt in general, and now which model responded to that the best. And again, this is the type of thing where doing this manually... would take a long time. And you also now, you sort of have everything already built that you could do this, you know, again with, you give a different example transcript or you could, you know, try completely different types of prompts or you could have it use different versions of these models. So it's just example of where you can do a lot of work in cloud code without having to manually do it all on your own.

**Aakash Gupta** (00:55:47)

And where did we get the tokens for these chat GPT and crock? Yeah, good question.

**Carl Vellotti** (00:55:52)

So in this case, I already added the, environment keys. So, um, so these are, I have accounts on, uh, for these other LLMs and it's just using those. So cloud code doesn't natively have those. Yeah.

**Aakash Gupta** (00:56:05)

Yeah. It's not some free way to get access.

**Carl Vellotti** (00:56:09)

Um, okay. And then this other one, uh, okay. So it's still working on, it looks like the engineer review is still happening, but the other two are done. So we can come back to this one in a bit, see what happens with this, with this engineering one. One thing you can always do as well. So It's showing us, it just says that the designer is done, the executive is done. It also tells us that if we do control R, that we can see more information around what is actually happening in the agent. Although in this case, that didn't work. Oh no. Okay, so now we've covered a lot of ground here so far. So we've looked at all the different ways that Claude can research files, research the web, put that all together in pretty complicated ways, and we started to look at agents. Kind of the last main things to look at are, right now we've just been giving Claude the base tools that it already has access to.

**Carl Vellotti** (00:57:11)

You can really power up any sort of LLM, especially Claude code, by giving it access to more tools through MCPs. Have you used any MCPs or are there any that you found that you think are really interesting?

**Aakash Gupta** (00:57:25)

Well, I guess let's do the Slack MCP since we mentioned that earlier.

**Carl Vellotti** (00:57:28)

Yeah, so... In this case, okay, well, we're gonna... Usually helpful, give me one second to try to find the... Let me see if there's an official one. Okay, we'll ask Claude.

<!-- sponsor -->
**Aakash Gupta** (00:58:11)

This episode is brought to you by Linear. You know what's broken about product development right now? It's not the coding. We've got AI helping with that. It's everything else. The planning, the feedback synthesis, the endless context switching between tools. You're drowning in PM busywork while the actual product work suffers. Linear started as that issue tracker engineers actually wanted to use, which, let's be honest, is pretty rare. But it's evolved into something way more powerful, your entire product development hub. Their new AI features are a game changer for product managers. Product intelligence automatically surfaces insights from customer feedback and support tickets. No more manually combing through hundreds of reports. And their AI agents help draft PRDs, scope projects, and handle all those status updates nobody wants to write. Product teams from OpenAI to Vercel use Linear to build complex products at speed. There's a reason they call it magical.

<!-- sponsor -->
**Aakash Gupta** (00:59:00)

So visit Linear.app slash partners slash Akash. That's Linear.app slash partners slash AAKASH.

**Carl Vellotti** (00:59:11)

So, so far we've really covered basically all of the like main functionality of, you know, what they might call vanilla cloud code, which is all of the things that cloud code comes with on its own, which, which is quite a lot. It can search files, read files, put it all together. You can add, it can create its own sub agents. You can add sub agents. The last thing to sort of really cover to sort of show the full power of Cloud Code is that all of the tools that we've shown are just the tools that Cloud Code comes with. But you can also add tools. The main ways that you can do that is you can either give it APIs to work with, which is kind of what we saw with giving it the ability to pull in transcripts from YouTube. We gave it the API and now it has this new superpower and it can go use that.

**Carl Vellotti** (00:59:51)

The other way, which is sort of an API built just for LLMs are called MCPs. And so these are, they're a lot like APIs, but they're just specifically built for LLMs to be able to use in all these different types of workflows. And so here what I have is just sort of a simple one for Reddit. So Reddit in general makes it a little bit hard to get information off their platform if you are an LLM, if you want to doing sort of like scraping or anything like that. But if you use the MCP for Reddit, then it's actually quite good at getting information straight from Reddit. And so as an example, let's say, What we could do, and we'll show like sort of a bigger example after this, but what you could do is you can just say, hey, I found this thread on automation.

**Carl Vellotti** (01:00:42)

We have like this automation product. Can you go through and can you extract all the information and find the pain points? And so it's gonna use the Reddit MCP because if it tried to do that on its own, it wouldn't really be able to do it.

**Aakash Gupta** (01:00:54)

And now we

**Carl Vellotti** (01:00:54)

can see that right away using that tool, it was able to pull in that information and get all of that. And

**Aakash Gupta** (01:01:01)

you

**Carl Vellotti** (01:01:01)

could sort of imagine how you could build some agents that use this MCP that are really powerful, where you can have it run every day, like, summarize the top posts on r slash product management today and tell me what the top things that people are writing about, you know, if you're maybe trying to create content or something, or, you know, Tell me like maybe competitors have their own channels. You can have that run every week and say what were the main pain points that people brought up this week. And by giving it this tool, you give it access to that information that it wouldn't be able to get on its own. So here we see that it went through that automation thread and now it summarized these. And you could put these in a file or you could have it. even what you could do at the very last thing with demos, we could even have it sort of build a prototype that gets at these pain points, and then we could go show that to our boss, and they'd be really impressed because we have real users that we're demoing it, or real feedback from the real world that we're basing our prototypes on.

**Aakash Gupta** (01:01:59)

Yeah, that's amazing.

**Carl Vellotti** (01:02:01)

And then, yeah, just the last thing for these MCPs, as we kind of saw, they do take some setup to get going, but there are some really awesome registries of these, For example, there's a couple that people have put on GitHub where they're just these huge lists of all the different tools that you can give to To LLM, so there's like a Google Drive one, which, you know, in this example, I had all these files sort of that I added already. But if you're working at a company or you're doing personal work, you could use a Google Drive MCP to pull that information in really easily. And there's tons of these. One thing I think is kind of an interesting thing maybe for product managers to think about is, as we've seen, cloud code is... really good at a lot of stuff outside of code but just I think based on who the users are and like what the use cases are so far most of this is really really coding and this AI agents base that I built or that I didn't build this that I showed off earlier it's like really if you look at it it's mostly coding it's like We see a lot of architecture and integration and engineering and things like that and not a lot in the other use cases.

**Carl Vellotti** (01:03:13)

So while there are a lot of tools today and it makes it really good for coding, I think there are for sure, as these tools become more widely available and used by the more general public, a lot of opportunities to build these types of agents and tools for things that aren't just for coding.

**Aakash Gupta** (01:03:29)

Mm-hmm.

**Carl Vellotti** (01:03:32)

Yeah, okay, so that kind of takes us through all of like the absolute sort of core abilities of Cloud Code. You can kind of imagine how as you go, you get better at mixing and matching all these things. The one thing we didn't really demo, which I think would be good just to show off, is while I was kind of recommending that you You might want to use cursor for, you know, more code based things. Sonnet is still a really good model, uh, that you get with the base level of, uh, of cloud code of cloud pro.

**Aakash Gupta** (01:04:01)

So

**Carl Vellotti** (01:04:02)

it'd be good just to sort of quickly show how it is pretty good at prototyping. So in this case, I created a spec earlier, um, that just sort of has like a workflow that we might want it to use. And so it doesn't have it already built though. It just has like a quick little spec. We'll just show off the kind of capability of it to actually do code. So for example, if you did want to build a prototype from, you know, you just talked to, you just did a user interview and you summarize those pain points and now you have an idea. You don't necessarily have to jump into another tool. You can just ask Claude to, code up a quick prototype for you to look at and so as we see here this is a good one where in the real world we probably want to do plan mode first but here i'm just sort of trusting claude to to get it right and so it's created its its little to do's here and it is going to check those off and we'll see what it comes up with

**Aakash Gupta** (01:04:50)

and can we take a look at what the workflow builder spec was

**Carl Vellotti** (01:04:53)

yeah So basically the spec here for the workflow builder is just, let's say that we want like a very starting point where we just want to say, I want to be able to sort of do a classic workflow builder where you can add nodes and then connect them together. Because if you're going to, you know, building, starting with a prototype, you need sort of like somewhere to start. And so it's still, there's still some like real sophisticated aspects here where it needs to be able to manage adding nodes onto this, uh, this canvas and then it has to be able to connect them. So we're gonna see sort of how it does with that. And I have a feeling it'll probably do pretty good.

**Aakash Gupta** (01:05:38)

Okay.

**Carl Vellotti** (01:05:44)

All right, it's working through it. Any other things we could try or you wanna see demoed?

**Aakash Gupta** (01:05:54)

One of the things that I think a lot of people have on their minds is building out evals. Is Claude a good tool for doing that?

**Carl Vellotti** (01:06:02)

Yeah, so that's a good question. I think... Cloud Code could definitely be used for building out evals. It's a good way to sort of just make sure that the prompts, like we kind of showed earlier, where we had it write the prompts and then test those prompts in different models. You could definitely imagine a workflow like that where it's also helping you figure out what are the evals, or you could have a bunch of data that you're pulling in that shows what good responses are. I think Cloud Code would actually be really good at helping you integrate evals into your overall workflow.

**Aakash Gupta** (01:06:34)

And then a lot of PMs are thinking about, what if I have a really easy front-end change and I just want to vibe code that front-end change? Would CloudCode be a good tool for that?

**Carl Vellotti** (01:06:48)

Yeah, so I would definitely say CloudCode is very good at front-end. And for example, what it's building right now, is mostly front-end. Cloud Code is very good at front-end, and for those simpler types of things that don't necessarily require a deep understanding of how the back-end is architected, it could definitely do that. And even within these demos that we've done today, it's done some pretty complicated stuff where we gave it the YouTube API without really any instructions on how to use it, and it got it right basically on its first try. So it is definitely a good model for that type of work.

**Aakash Gupta** (01:07:21)

So if you can get read access to your code base, you could potentially use Cloud Code and it could just pick up the existing code base, design system, tech stack, et cetera.

**Carl Vellotti** (01:07:32)

Yeah, exactly. You just have to be really nice to your engineers.

**Aakash Gupta** (01:07:38)

And get yourself a very safe testing environment.

**Carl Vellotti** (01:07:42)

Yeah, testing environment. And I think the main thing with all of that type of stuff, because I think there's like a little bit of... You see it on social media. There are some engineers who I think are very, I don't know if they're exactly anti-vibe coding, but I think they do sort of really want to reiterate that it's like not real engineering, which I think is true. So as long as you're talking to your engineers or you're working with them and you're coding these things up, I think as long as you don't present it as something that is really production ready, but it's more in terms of I'm showing you an idea. And of course, we need to figure out how we would actually build it. But here's a way for me to think through what it would look like in a very visual way, in a way that kind of helps you figure out what are those edge cases that you would forget about if you're just thinking of Figma.

**Carl Vellotti** (01:08:28)

So I think this is a little bit outside the scope of your question, but I think that type of stuff is awesome. And you can definitely do those types of tweaks and explorations. But I think if you want it to be production ready, I wouldn't use any LLM right now, and I wouldn't use Cloud Code for it.

**Aakash Gupta** (01:08:43)

Okay.

**Carl Vellotti** (01:08:44)

Yeah.

**Aakash Gupta** (01:08:45)

Because, yeah, these experimentation tools are building it in now, whether it's Optimizely or Amplitude or Chameleon, where you can just prompt, like, a front-end change. And they're trying to push, like, you can run the experiment.

**Carl Vellotti** (01:08:59)

Yeah, I... Yeah, for front-end stuff, that's probably fine. I think you probably still want an engineer to review. Yeah,

**Aakash Gupta** (01:09:08)

you still need it, I think, yeah.

**Carl Vellotti** (01:09:12)

Let me see. Sometimes it'll just get stuck, so we're going to just exit. Oh, one thing we didn't actually, as kind of attested into how good Cloud Code is, you can always exit by just hitting the escape command. We actually haven't had to do that at all today. Oh, actually, it looks like it was working. Yeah, sometimes you just have to wait. So here in this instance, we're kind of like sitting here watching it go through the commands. And then now we can see that the main thing you can always tell if it's like actually working is if the tokens are going up. In this case, we see that we see the tokens. That's just kind of like it's thinking effort. So it is it is going through them. But yeah, this is a good example of where, in this case, you could go open another clod, or you could go read Twitter, which I think is like, there's kind of some memes about how a lot of times you'll try to figure out what to do in the intermediate steps when AI is coding.

**Aakash Gupta** (01:10:12)

Yeah. Something that's like not too deep

**Carl Vellotti** (01:10:16)

work. Yeah. Honestly, that's kind of a funny thing you mentioned. It's really hard to do deep work when you're coding because you're kind of in this state of when you're like vibe coding where you're kind of in this state of you're using it and you're engaged and you still have to be like pretty paying attention to what's going on, but there's never enough gaps to like actually do anything that's useful. Yeah. Okay, so let's see what this did. So it kind of surprisingly checked off everything at the end, and now it's telling us that we can start it. So let's see what we get here. All right, so it ran the server itself. Okay, we're going to.

**Aakash Gupta** (01:10:56)

So it's maybe not as fast as like if you were just to use v0, like sometimes those prototypes come in like 20, 30 seconds. This took 300 seconds, but let's see what the quality is.

**Carl Vellotti** (01:11:06)

Yeah, it's true. Okay, so we have our canvas. We have this like dotted grid. All right, we click add node. We have our node here. We can add another one, node two.

**Aakash Gupta** (01:11:18)

Nice.

**Carl Vellotti** (01:11:19)

That's pretty nice. Oh, let's see if it actually connects.

**Aakash Gupta** (01:11:24)

Love it. Why has CloudCode taken off so fast? How do you think it's reached 500 million ARR in a few months alone?

**Carl Vellotti** (01:11:31)

I think CloudCode has really hung in there by just the skin of its teeth with just having a really great product. You know, ChatGPT was first, absolutely sort of just dominated the market. And even today, it's definitely... the most used model of all of them. But Claude just did a couple things, I think, really right. I think one is they really figured out that coding was just an absolutely killer use case for LLMs. And they were the first, I think, to make really big bets on making sure their model was fantastic at coding. And in the developer community, it really got picked up. So I think they kind of... Even though... mainly like overall usage definitely went toward ChatGPT. Within the niches that they realized they could be good at, Cloud Code has just really, really done a good job. And I think the other thing is they just, Cloud is just a really, it's just a really great model.

**Carl Vellotti** (01:12:23)

Like, I think when you compare it to ChatGPT, ChatGPT is good at, like, sort of factual information. But writing is just definitely the best from Claude. And I think understanding intent from Claude is also what it's just really good at. As an example, you know... I don't do this a lot, but I know it's sort of a very common use case to, you know, ask for advice from an LLM. Sometimes I'll, you know, give a whole bunch of information about some sort of, you know, maybe interview I'm prepping for and asking for different ways to approach it or some decisions that I'm trying to make. And you'll give that to ChatGPT and ChatGPT will say, okay, let me come up with a structured plan. The pros of this option, the cons of this option. And then Claude will take that and then we'll say, hmm... it seems like you've actually already made up your mind.

**Carl Vellotti** (01:13:08)

And you know, there's just like this like deeper understanding of intent that I think Claude has that even though it wasn't the first to market and wasn't sort of the first with like mainstream adoption, it's just a really good product.

**Aakash Gupta** (01:13:20)

Nice. So Cursor was, I think 500 million ARR in like 36 months, 500 million ARR in four months. I think both of them are benefiting from the amazing work that the Anthropic team did generally for how Claude codes, but it seems like with Claude code in particular, they've developed a really genius user interface. You can use it inside of Cursor or any other tool. And so I think that that accessibility they've created around it is really something else. How would you summarize? What are the top use cases of product managers in cloud code?

**Carl Vellotti** (01:13:58)

Yeah. So it's really good for all different types of things. I would say that the main, you know, it's good for coding, but product managers don't necessarily only need to code or they maybe shouldn't be coding that much, which is where I think when you, when you have cursor or these, things that are using LLMs like only for code or they're mainly built for code, then they actually kind of get worse at other things that, you know, product managers really need to do. So for example, research is a really good thing that Claude is for because you can have it go out and do this research and put it into files and you can sort of give it that context really easily. So research is one. Any sort of like handling of written information, so handling... meeting notes or handling user interviews or writing PRDs. Those types of things are another area where Claude, just because it understands intent so well and because it's just such a good writer, those are absolutely great use cases for product managers.

**Carl Vellotti** (01:14:57)

And it is still good at coding. So even though these other tools might be more specifically built for heavier duty engineering work, you can still do coding and you can still build prototypes pretty well within CloudCode. I would say research, anything with written documents and VibeCoding simple prototypes are some of the best use cases for product managers to use

**Aakash Gupta** (01:15:21)

CloudCode. Just to summarize one more time for folks, anything to do with writing where you need to load it up with context, CloudCode is a much better way to interact with stuff. Anything you need to do with research, simple prototyping. And I think the fourth thing people are really interested in is what about AI agents? When should I be building my AI agents in Linde or N8N or Cloud Code?

**Carl Vellotti** (01:15:45)

Yeah, that's a good question. So I think this is where the term agent, I think, is getting a little bit overloaded in general, like in the space. So cloud code as an agent is a little bit more tactical. So it's more you say, hey, here's a task that I'm giving you right now. Like I'm sitting here and I'm giving you this task and I want you to go do these specific things. And then it will go out and it will... Come up with a plan for itself and it will work through that plan and it will do it. And it's very good at that. And I think that's where it's sort of an agent or agentic where it can think for itself and come up with a plan. Whereas, you know, N8N or I think Lindy, they're more of they're more based on like an automation.

**Carl Vellotti** (01:16:28)

where you have an LLM brain inside of it that helps guide the automation. But they're more of something that's a recurring task that you feed information and then it will sort of figure out how to navigate that and give you an output. But it's not as tactical as cloud code. So I think they're just sort of different types of products. And I think if you... If you want to build an agent that helps you accomplish new types of tasks or things that you can't automate, then that's where cloud code agents are really useful. But if it's something that's a recurring thing that you're going to be doing over and over and you just need an LLM integrated, that's where platforms like N8N or Lindy are really good.

**Aakash Gupta** (01:17:07)

So you're way deeper in N8N and Cloud Code than 99.9% of people listening. So having used those tools so deeply, what are the top AI agents that a PM should be building and which tool should they be using for each of those agents?

**Carl Vellotti** (01:17:21)

Yeah, so I would say if you are... In general, I think the guiding principle for when you should create an agent is when you find yourself doing something that's sort of the same type of task frequently and it's something that an LLM is actually good at. So let's talk about both of those things. First, anything that you're doing frequently. So if you are... If you need to really closely watch competitors because you're in that kind of industry and you find yourself going to the same blogs or doing the same type of searches every week, that's where you should build an N8N automation that can do that search and then have an LLM summarize it for you and then put it in a database for you. That's a great example of something where an LLM can really help you just... do that thing that you're doing all the time.

**Carl Vellotti** (01:18:13)

Or if, you know, you need to structure your meeting notes in a specific way, you know, you build an agent in cloud code where you just say, hey, here's all my meetings from the week. Can you help me get the, summarize the main takeaways and then write some Slack messages for me to ask people for status updates next week. Like any type of like recurring tasks like that. And then you'll kind of notice that those examples that I gave, those are like text-based, not too much creative work type tasks, which is where LLMs are... really good. They're amazing at those types of like, you already have existing information and now you need to summarize it or put it in a new format. I think where it can be sort of like a trap is trying to create too many agents for, you know, too many things.

**Carl Vellotti** (01:18:56)

There's certain types of work that, you know, LOMs just really, really aren't that good at. So as an example, if you need to Like if you need to come up with feature ideas based on user research, then summarizing that user research and getting key insights from it, that is something that LLMs are good at. But actually figuring out what to do with that information, that's probably like, I would say that an LLM agent that comes up with feature ideas that you're supposed to be able to implement or would like actually solve user problems. I would be very skeptical of those types of things. So thinking about what is the rote, sort of work that you're doing that is text-based and LLMs are good at, and then give that to the LLMs. And the principle I like there is also have LLMs do the work that you hate, not the work that you love.

**Carl Vellotti** (01:19:45)

So you don't probably love doing the Google searches. You probably like trying to get the insights from the information. So I think that's how you should think about when you should use each one.

**Aakash Gupta** (01:19:56)

So there's all this hype around multi-agent systems. When do you use a single agent versus a multi-agent system?

**Carl Vellotti** (01:20:02)

Yeah, it's a good question. I think it's another type of example where it sort of depends what the use case of the agent is. But the more complex the thing that you're doing, it's like you can always add... basically more layers so like let's say that you have a system where you both first you need to get a bunch of information from online and then you need to come up with some key insights and then you let's just you know even though i just gave a counter example or let's say that you um you have you're giving it ideas of things that you want to prototype and then you wanted to go build those like the more layers that you have the more like multi-agents you can start to add but i think the thing to keep in mind is that The more that you add, and we're already starting to see this, and I have some engineering friends who I talk about this who are very into trying to get LLMs to code, is these models aren't perfect, and there are some hallucinations in there, and there are just decisions that it will make that the less the human is in the loop, and the more creative work that you try to give it, and the more agents that you do involve...

**Carl Vellotti** (01:21:12)

the more risk of the output just not being very good or getting stuck somewhere that they sort of can't get past goes up. So I still think that for the most part, where you are heavily in the loop using agents in ways that you exactly understand, rather than having a whole chain of agents that are supposed to do tons of different things, is where we're at now. I think as the models improve, multi-agent things will be more powerful. But Right now we're still in this mode where there still needs to be pretty heavy human supervision over these things where you can't go too many layers without it kind of starting to get really ridiculous.

**Aakash Gupta** (01:21:49)

So if you're trying to build out your AI tool stack, it sounds like you do want N8N and you do want CloudCode in your tool stack. Do you also want an AI prototyping tool? Like, is it better to have a V0 that's a lot faster or should you just allow CloudCode to do all of that for you?

**Carl Vellotti** (01:22:07)

Yeah, it's a good question. I think, uh, for me, like I, my main sort of tools are, I use cloud code for all this sort of like text-based awesome interface for using the LLM. I use NN for those types of, um, automations that we talked about. And then for me, my prototyping tool is really just cursor where I'm using the better models. Um, directly. I think that if for like the specific prototyping tools, like lovable or V zero, I think they are still helpful because if you're not as comfortable with like the heavier duty tools, they can still get you that like quick interface and they can connect to a backend really quickly in ways that, uh, Cloud code can, but unless you're like really comfortable working in like a more step-by-step way that's closer to, it sort of gets further away from vibe coding and it gets closer to AI assisted development.

**Carl Vellotti** (01:22:59)

I think if you are not that comfortable with doing stuff like more in the architecture and in the code, then it's still useful to actually have a prototyping tool.

**Aakash Gupta** (01:23:09)

And I think you referenced this a little bit, but the meme out there is that Cloud Code is just spending a bunch of time manifesting. What are the right ways to avoid kind of manifestation hell?

**Carl Vellotti** (01:23:20)

Yeah, the best thing you can do is you can just spend time in plan mode, which is one of those things where I think a lot of times with all these LLM tasks, if you go slower up front, then you can go much further and much faster overall. And so I think where... If you just give it too general of a task, then it will do its best. No matter what you give an LLM, they will try to do the task in any way that they can think of. But if you can really make sure that it knows what you're actually looking for, like the type of output, and you can... have it tell you its plan so you can see mistakes that it's going to make just from, you know, just being a human who has more intelligence than these models, then I think that's a way that you can really keep it from getting stuck.

**Carl Vellotti** (01:24:06)

And the other thing, and this is sort of what I was mentioning earlier, it is helpful to just pay a little bit of attention. I think there's the... The hope that you can have all these agents doing all your work at the same time and that you don't need to supervise it. But we're not really there. And so it's easy for them to get stuck in loops. So I'd say it's still sort of using them very tactically in a way that you're still paying attention to what they're doing can make them like you're a partner rather than something you can just delegate too much of your work to.

**Aakash Gupta** (01:24:32)

Amazing. That about covers it for really deep tutorial on Cloud Code. I want to shift gears a little bit and talk about you, right? You actually run the largest Instagram product management account. I think I had my Instagram account posting for like two years and I acquired like 360 followers or something like that. And I acquired, you know, maybe like a hundred K lifetime impressions. Then I reposted like three of your memes and I got like 200 K lifetime. impressions right away. So you have mastered Instagram for product management. Talk us through your story with Instagram. How did you even discover this meme space? How have you grown to become the king of PM memes on Instagram?

**Carl Vellotti** (01:25:14)

Yeah, you know, it's sort of, it wasn't really intentional. I started out with, it's funny, I started out on Twitter. It was sort of like where I started posting product management content. And as soon as I posted, like my first good meme, it got a lot of engagement. You know, it's sort of easy when you're posting on social media to start optimizing for things that maybe you shouldn't optimize for just because they're getting the most likes or the most engagement. And so I realized, you know, I can't have my Twitter because I'm still trying to create real content on there. I can't have it only be memes, even though there's, even to this day, there's still some temptation to do that. Yeah. So I was like, okay, well, what is a platform I don't necessarily care about as much and is a much better place for memes?

**Carl Vellotti** (01:25:58)

And right around this time is also when Threads was coming out. And so that was when Twitter was in its early Elon days. People were saying that maybe Twitter was going to completely die as a platform. That was the only place I was posting. So I started posting my memes there. And then, I don't know, I just like making memes. I think that was what it was early on. And the nice thing, which I kind of look back on it and a little bit fondly is this was like sort of pre-LLM or when LLMs were still pretty bad. So they were all just like genuinely like, I was just coming up with these memes and it was just this challenge of like, I have to think of these completely on my own. And so just really being consistent, like posting images like two times a week, sorry, two times a day, every weekday.

**Carl Vellotti** (01:26:41)

And then I started posting reels and then Instagram just loves, loves, loves reels. And That was where it got a little bit harder because with memes, with like image memes, there's a bunch of examples, you know, for any given popular meme format of an image, you can find like tons of examples and then you just kind of think like, okay, well, what's a product manager version of this? And with reels, you have to take videos where you can't really find like a large database of where that video has been used for a meme before. And so I would say the challenge of writing good jokes with those video-based memes went up, but then just like the rewards from Instagram also went way up. And then as you go, you kind of just start to find common themes. So one of the most common themes that... There's two common themes I'll just say that if you're making PM memes, they just always work the best.

**Carl Vellotti** (01:27:30)

One is the relationship between engineers and product managers. Everyone just thinks it's so, so funny. And the key of... really having, like, good Instagram or, like, things that go viral on Instagram is that it's a little bit less, like, on Twitter, it's, like, how witty and, like, how insightful is your meme? That's, like, really the main thing that will make it go big or almost, like, how, like, irreverent. Whereas on Instagram, it's how shareable is it? And so if you post something, like, about the product manager engineering relationship where... you know, the very common trope of the engineer being sort of the grumpy smart one who does all the work and the product manager being like the peppy sort of dumber but like people person one who just takes all the credit. That type of format I think is just so shareable because I think PMs relate to it and share it with their other PM friends.

**Carl Vellotti** (01:28:23)

I think engineers relate to it and share it with their engineer friends. So I think just... optimizing for what is like relatable and shareable is what I've realized is like the absolute sort of key to Instagram. And so there's the product manager engineering relationship. And then there's just in general, the PM not doing any work. So like, Anytime you have a meme where there's a whole construction crew and there's one guy who looks like he's working, but he's just walking around, those types of memes just always do well.

**Aakash Gupta** (01:28:55)

And then besides that, it's just

**Carl Vellotti** (01:28:56)

consistency. I think I've posted two memes every weekday for two and a half years now, and that

**Aakash Gupta** (01:29:01)

just

**Carl Vellotti** (01:29:02)

compensates over time.

**Aakash Gupta** (01:29:03)

And a story, right?

**Carl Vellotti** (01:29:06)

Yeah, I post them all to stories as well. That's... Yeah, that is like a it's less of like a growth tactic, but it's like a good way for people to be able to like respond to you. Anytime I get a DM, I respond like every single DM, which I think also helps kind of keep it in people's feeds.

**Aakash Gupta** (01:29:23)

Yeah, for sure. And are you using any agents or anything for your Instagram?

**Carl Vellotti** (01:29:27)

Oh, yeah, good question. So I have built... So I mentioned that as, like, pre-LLM, because now it's, like, it's funny how many things these days I feel like it's hard to do them without, like, at least trying to use an LLM. So I have built something. I don't really use an agent, but I have, like, an automated... I don't really have an agent, but I have a thing that I built. I guess we're not doing the screen share, but I could screen share it. Okay, so this is sort of my top secret weapon. So what I have is, I call it Meme Mage. This is something, I do eventually want to turn it into something that is a real usable tool, but for right now, this is just... just mine. It's not quite, it's very optimized just for myself, but it's still, this is my first vibe coding project ever.

**Carl Vellotti** (01:30:14)

So it has some, some things in here that are, I don't think are the best user interface. So the making jokes with LLMs is like a really interesting kind of context engineering challenge because, you know, when you're, so just to show the, or illustrate the type of meme that I mainly post on my account are these like, uh, image or video that's happening in the middle with a caption on the top. And so very simple. So you can kind of imagine how this type of joke is or this type of format is common. But if you just say, if you just tell an LLM like, hey, here's some screenshots of this video, can you help me make a meme out of it? Then they won't really understand. And so what I have built is I've built this little database of like templates for these different types of memes.

**Carl Vellotti** (01:31:05)

And what it does is it uses, Gemini has a model that can watch videos. And basically I will give it a meme And it will try to understand like what the joke of the meme is. So in this video that we're showing here, there's like a train that just usually the joke will be like, you know, when the weekend finally comes and then it rushes by super fast. So what I have here is I have like this template that sort of explains like everything about how this joke works. It's like, what is happening in this video? And then what, how exactly does this joke work? And then what are examples?

**Aakash Gupta** (01:31:41)

And then I

**Carl Vellotti** (01:31:42)

have this, small little database of like personas. So I have like a product management persona At one point, I was trying to make a bunch of these different accounts, so I was testing this. But it's like, okay, product managers are this role, and then it's like examples of the types of jokes that that person, that that likes. So then you kind of have like the right context that you need for the LLM, where you have who is the person and what types of jokes do they find funny? And then what is the template and what types of jokes can you make with that template? And then this is my sort of interface here where it will go and it will... In this version, it just randomly selects templates and then matches them against that persona. And so now it's, you know, basically sends off all that information to the LLM and now it's writing captions.

**Aakash Gupta** (01:32:30)

Very cool. And I assume you edit these because it's an LLM, of course, but it's giving you so much fodder to, like, react to and improve.

**Carl Vellotti** (01:32:40)

Exactly. So now it has the videos, and then it shows, like, you know, product manager realizing they accidentally shipped to the staging environment prod. And, like, this is still pretty experimental, but I have, like, a bunch of different options. And it's one of those things where... um because it's an llm like one of these 10 caption or one of these 20 captions that makes for the videos will be like 90 of the way there and then you still have to like kind of workshop the actual text

**Aakash Gupta** (01:33:08)

um

**Carl Vellotti** (01:33:08)

usually usually they're like a few words too many or there's like oh that's an interesting idea but it needs to be worded a little bit different uh it's how you like really really get these to be good but yeah that's uh this is my sort of my secret weapon for being able to helping me uh create memes with LLMs.

**Aakash Gupta** (01:33:26)

Amazing. That's the secret weapon behind two and a half years of consistency, guys. You're not going to grow to, what is the latest Instagram follower number? I

**Carl Vellotti** (01:33:35)

think we're at about 55K.

**Aakash Gupta** (01:33:37)

Wow. 55K for PM Nish is insane. They're like, I think that's higher than Lenny. That's insanely high. So good for you. What is this all turning into? What is the business of Carl looking like these days?

**Carl Vellotti** (01:33:53)

Yeah, so I left my job earlier this year. I've been a product manager, senior product manager for about eight years. And just based on that thing that we just looked at, which my meme made, I realized I had been writing, I've been creating product management content for a couple years. And about two years ago, I had a newsletter that I called the Future Proof PM. And I was writing about AI use cases for product managers. And it was just a little bit too early, I think, because after writing that for about like 20 weeks, there just wasn't a lot of new stuff because it was mostly like AI rappers that weren't or LLM rappers that weren't that good. Or it was, you know, here's a new prompt. Here's a new prompt. And so I sort of stopped that newsletter and then I really sort of stopped content creation for almost a whole year.

**Carl Vellotti** (01:34:38)

I moved to a new city and then I started my new job and I sort of just wasn't creating any content for most of 2024. And then at the beginning of 2025, I like finally, finally decided to start Cursor because Vibe Coding was really going viral as a concept. And I was blown away. I could not believe like how much you could do So that whole thing, that whole meme mage thing that I just showed, that was like my first project. And I was like, this is incredible. And then I just got really, really deep into it. And I realized that the space had just evolved. The models had just gotten to a point and the tooling had gotten to a point where... so much more is possible and so i've always wanted to start my own business but i didn't know exactly what it should be and then you know i'm still you know i still love product management and creating product management content and now there's just all these new capabilities that i left my job earlier this year and then i started a new newsletter called uh the the full stack pm and i'm building that now and so you know i creating content on on instagram is a piece of it because that's like a like a good place to sort of like interact with my audience.

**Carl Vellotti** (01:35:44)

But now sort of building out this this, you know, community and newsletter specifically for like product management builders is is what I'm working on.

**Aakash Gupta** (01:35:53)

So you're monetizing. Yeah.

**Carl Vellotti** (01:35:54)

So far, I'm early, like no monetization, just sort of trying to grow it and build a community.

**Aakash Gupta** (01:36:00)

Wow. One of those people who just dared out, ventured into the unknown, no monetization, really excited to see the journey. We'll have to check back in a couple months. Carl, thanks so much for being on the podcast.

**Carl Vellotti** (01:36:13)

Yeah, it was great. Thank you for having me.

**Aakash Gupta** (01:36:15)

See you later, everyone. So if you want to learn more about how to shift to this way of working, check out our full conversation on Apple or Spotify podcasts. And if you want the actual documents that we showed, the tools and frameworks and public links, be sure to check out my newsletter post with all of the details. Finally, thank you so much for watching. It would really mean a lot if you could make sure you are subscribed on YouTube, following on Apple or Spotify podcasts, and leave us a review on those platforms that really helps grow the podcast and support our work so that we can do bigger and better productions. I'll see you in the next

**Aakash Gupta** (01:36:54)

one.
