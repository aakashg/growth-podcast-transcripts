---
title: "The Complete Guide to OpenClaw for PMs [EXCLUSIVE]"
subtitle: "How to install OpenClaw from zero in three terminal commands, connect it to Slack, and build five automations that replace hours of manual PM work every week."
date: "2026-03-17"
host: "Aakash Gupta"
guests: ["Naman Pandey"]
speaker_names: "substack"
substack_url: "https://www.news.aakashg.com/p/naman-pandey2-podcast"
youtube_url: "https://www.youtube.com/watch?v=YLXRg078EKs"
duration: "01:40:51"
word_count: 18923
source: "Substack episode transcript (aired audio)"
sponsors:
  - name: "Jira Product Discovery"
    url: "https://www.atlassian.com/software/jira/product-discovery"
  - name: "Vanta"
    url: "http://vanta.com/aakash"
  - name: "Mobbin"
    url: "http://mobbin.com/aakash"
  - name: "AI PM Certification"
    url: "https://maven.com/product-faculty/ai-product-management-certification?promoCode=AAKASH550C7"
---

**Sponsors:** This episode is brought to you by [Jira Product Discovery](https://www.atlassian.com/software/jira/product-discovery), [Vanta](http://vanta.com/aakash), [Mobbin](http://mobbin.com/aakash) and [AI PM Certification](https://maven.com/product-faculty/ai-product-management-certification?promoCode=AAKASH550C7).

# The Complete Guide to OpenClaw for PMs [EXCLUSIVE]

*How to install OpenClaw from zero in three terminal commands, connect it to Slack, and build five automations that replace hours of manual PM work every week.*

**Aakash Gupta** (00:00:00)

It's up to 245,000 GitHub stars. There's over 2 million weekly visitors. OpenClaw is going totally viral.

**Naman Pandey** (00:00:07)

Today, we're going to break that down. How to set it up the right way. Security stuff that seems benign, but you really can't skip.

**Aakash Gupta** (00:00:14)

The question on everybody's minds is how do PMs actually use this tool?

**Naman Pandey** (00:00:19)

versus the traditional LLM, which is more reactive. Here, you can really take the reins of whatever you're trying to do and be proactive. Here, you can set it up to execute even when it's 3 a.m. and you're asleep, you're not even at your computer.

**Aakash Gupta** (00:00:32)

I know one of the toughest parts is actually setting it up. I've tried to teach a couple of people this, and this is the part that once they do it, they're unlocked. So can you walk us through the easiest no stress setup guide you could find on YouTube?

**Naman Pandey** (00:00:43)

There is a simple three-step process that you can just use on your terminal. If you're not seeing red, you're good.

**Aakash Gupta** (00:00:49)

Should you be using a VPS or Mac mini, Telegram or Discord? What about the security risks everyone keeps talking about? We will answer all your hottest questions.

**Naman Pandey** (00:00:57)

We are going to turn any Slack channel into an AI-powered knowledge base that answers team questions from your product documentation. Every morning at 9 a.m., OpenClaus scans your team's Slack channels. It summarizes what happened overnight, identifies blockers, and posts a concise stand-up brief to product stand-up that replaces the 15-minute context-gathering ritual.

<!-- sponsor -->
**Aakash Gupta** (00:01:16)

So product managers are getting one step closer to Iron Man. Before we go any further, do me a favor and check that you are subscribed on YouTube and following on Apple and Spotify podcasts. And if you want to get access to amazing AI tools, check out my bundle, where if you become an anal subscriber to my newsletter, you get a full year free of the paid plans of Mobbin, Arise, RelayApp, Dovetail, Linear, Magic Patterns, Deep Sky, Reforge Build, Descript, and Speechify. So be sure to check that out at bundle.akashg.com. And now into today's episode. Naman, welcome to the podcast. Thank you for having me. So we've all seen the hype. It's up to 245,000 GitHub stars. There's tons of forks. There's over 2 million weekly visitors. OpenClaw is going totally viral. And it's had a tumultuous history. It used to be called Claudebot. Anthropic asked him to change the name.

<!-- sponsor -->
**Aakash Gupta** (00:02:14)

He changed it to Molpot. He realized that it wasn't such a good name. He called Sam Altman. And Sam said you can call it OpenClaw. It was called OpenClaw. And then a week later, Sam bought him for over a billion dollars. And the question on everybody's minds is how do PMs actually use this tool? So why should PMs actually care about Open Claw Nomen?

**Naman Pandey** (00:02:35)

Well, so the biggest reason would be that versus a traditional LLM, which is more reactive, here you can really take the reins of whatever you're trying to do and be proactive and plan ahead in terms of whatever you're willing to accomplish. What that looks like in practice is that instead of conversationally asking it to do things or asking it questions, here you can set it up to execute even when it's 3 a.m. and you're just, you know, you're asleep. You're not even at your computer. Finally, the biggest benefit in terms of usage itself is that it's not cloud locked, which means that you can plug and play whichever LLM you want based on the use. If you're doing more deep research type work, you can plug in Opus versus if you want a faster response to a customer, maybe you can just use a faster. You can just use the fast Gemini model.

**Aakash Gupta** (00:03:24)

So I've been playing with Open Claw for weeks now and I know one of the toughest parts is actually setting it up. I've tried to teach a couple people this and this is the part that once they do it, they're unlocked. So can you walk us through the easiest no stress setup guide you could find on YouTube?

**Naman Pandey** (00:03:40)

Yes. So when it comes to setting it up, there are two broad ways to do this. And I say broad because just the only thing in common they have is the first step. After that, they look completely different. The first of those two will only take me 15 seconds to demo. It's actually kind of crazy how easy it is. But really all you have to do So for the first easy, almost, you know, your training wheels setup, all you have to do is go on emergent.sh. Some of you might be familiar with emergent. It's, you know, like it's a competitor to lovable, give or take. And what they've done here is they've put in this moldboard feature right here. So what this lets you do is literally one click your installation. It just pastes everything you have to run here. The only thing you replace is your LLM key itself, which just goes in there.

**Naman Pandey** (00:04:28)

You do that, hit this little enter button. It just sets it up for you. The reason why we will not focus on this approach is that, as you can probably guess, it is restrictive in nature. It does not allow you the full freedom to run OpenClaw on your computer machine, use your RAM, run your LLM locally. So, but in case somebody is looking for a really quick and easy out of the box type setup that is available simply by going on here. I'll now close that. Before we start actually pasting commands, remember that anytime you get stuck here, this stuff seems... this stuff can be intimidating but really if you just reverse google whatever error you're getting it's very easy to figure out we might run into a few here we'll see but the first command you want to paste is quite simply called npm install hyphen g open claw at latest what this does is it finds out the latest version that's available you hit enter i'm hoping this gets us some errors so i can live troubleshoot them but looks like it's going fine for now we'll see

**Aakash Gupta** (00:05:36)

You might not have NPM or something like that installed, and you might need to install that. So that's Node Package Manager versus from Node.js. And you'll run into these kind of issues when you're using Terminal. The most important thing to do is persevere. Just Google or take a screenshot of your screen and drop it into Clutter Chat GPT, and they will help you.

**Naman Pandey** (00:05:56)

Perfect. So that looked like it worked. So my quick and easy way to figure this out is if you're not seeing red, you're good. Sometimes you get a bunch of warnings, but they're fine and acceptable. So as long as you're not seeing bright red and like error, you're probably fine. The second command is the OpenFlow onboard. Before I run this, I want to walk through what happens when you actually do this. So just for context, Peter Steinberger, who invented this, the origin of the problem he was trying to solve was to have a bot that he could WhatsApp. So it started there in his head, but then he was like, why stop there? He wanted this bot to have a complete personality of its own. And I know you can give personality to your Claude or whatever, but he really wanted to bake this into the entire soul of what he was creating here, which is why I think you'll find it interesting that there's actually a soul.md file that gets generated that you can impart whatever you want, you know, type of attributes to.

**Naman Pandey** (00:07:00)

And then the way it is configured is that you cannot skip all that stuff. Like it will force you to give it a name, tell it how you want it to interact, tell it how you want it to interact with you and so on and so forth, right? So this is very interesting. We'll hit enter here and see what it throws at us. Okay, great. So now we're officially in, right? So there's obviously, you know, a big security warning. I don't think anyone has read this, not even Peter Steinberger, if I were to guess. You just say yes here. This is just saying that it requires lockdown in terms of your environment. It's not really that scary. You just hit left arrow, hit enter. That's the thing,

**Aakash Gupta** (00:07:39)

guys. Your mouse isn't going to work here. Don't get scared. You can either use the arrow keys on your keyboard or you can actually use tab too. And then you just hit enter.

**Naman Pandey** (00:07:48)

Great call out. So here you can go down the manual route. But the reason I would not recommend that is the quick start is actually comprehensive enough for the manual to start feeling like just way too much work, especially when you're trying to set it up. Also know that even if you skip steps here, it's very easy to set them up later. So it's actually not a big deal at all if you pretty much just speed run through this entire thing and go from there. So next up, as we were talking about, because we said that this is agnostic of model, these are literally all of your options. I'm sure there's probably more, even if there's something not mentioned here, there is a way to run this. What I would like to do is use Google because of late, I've just been a Gemini API kind of guy.

**Naman Pandey** (00:08:34)

Just random side note, I do feel in terms of dollar value, it gets me the farthest while still not compromising on quality that much. That's just my reasoning. I'm sure it just depends on what you do. So I'll pick Google and then I already have my API key. If you want to create one and

<!-- sponsor -->
**Aakash Gupta** (00:08:52)

don't have it already. Today's episode is brought to you by Jira Product Discovery. If you're like most product managers, you're probably in Jira, tracking tickets and managing the backlog. But what about everything that happens before delivery? Jira Product Discovery helps you move your discovery, prioritization, and even roadmapping work out of spreadsheets and into a purpose-built tool design for product teams capture insights prioritize what matters and create roadmaps you can easily tailor for any audience and because it's built to work with jira everything stays connected from idea to delivery used by product teams at canva deliveroo and even the economist check out why and try it for free today at atlassian.com slash product dash discovery That's A-T-L-A-S-S-I-A-N dot com slash product dash discovery. Jira Product Discovery. Build the right thing. Today's episode is brought to you by Vanta. As a founder, you're moving fast toward product market fit, your next round, or your first big enterprise deal.

<!-- sponsor -->
**Aakash Gupta** (00:09:58)

But with AI accelerating how quickly startups build and ship, security expectations are higher earlier than ever. Getting security and compliance right can unlock growth or stall it if you wait too long. With deep integrations and automated workflows built for fast-moving teams, Vanta gets you audit-ready fast and keeps you secure with continuous monitoring as your models, infra, and customers evolve. Fast-scoring startups like LinkChain, Writer, and Cursor trusted Vanta to build a scalable foundation from the start. So go to Vanta.com slash Akash. That's V-A-N-T-A dot com slash A-A-K-A-S-H to save $1,000 and join over 10,000 ambitious companies already scaling with Vanta.

**Naman Pandey** (00:10:41)

Perfect, yeah. So you just go on, I mean, you literally just Google, Google Gemini key, create, it'll bring you to the site that I've been on many, many times. Wait, is it that one? Yep, so create a viewer Gemini API key. Actually, there's no blurring needed. We'll be fine. But really, you just click this create API key. You give it a name. You might want to call it open claw. And then I'm not going to do it. But when you create a key, it'll just generate the key. Make sure you copy it and put it somewhere safe because sometimes it doesn't let you reaccess it once you've created it. So really straightforward. I won't be doing this again because I already have a key stored separately that I'll just be using over here. So I'm just going to hit enter here. I'm going to use paste API key now.

**Naman Pandey** (00:11:29)

So, okay, great. So you can just paste your key. Just try to not broadcast it over the internet. And then you hit enter. So then next up, this is also kind of what I was mentioning. It lets you choose exactly which model within Google to use. You can just go with your like the biggest, brightest one, which right now as of recording is Gemini 3 Pro. However, like as I was mentioning, if this is going to be a Slack bot that you think end customers are going to be interacting with, they probably don't need to wait 10 to 15 seconds for each response. In that case, if you just pick any of the flashes, those are known to be really quick. So it just depends on your use case, right? For now, you know, we'll just use the just quote unquote default, which is 3 Pro.

**Naman Pandey** (00:12:13)

Hit enter on that. So the other really cool thing about OpenClaw is that it really has one gateway that then connects to all of the rest of the Internet. So what this means is if you're running it on your WhatsApp versus also on your Slack, maybe you also have a Discord going for some reason. You don't need to create different gateways for that. All of it sits under one place, neatly organized. And you can then also use that one gateway to monitor and even delete any of your operations that you have going. I'll also be sharing how you can see the UI version of that increase in case the terminal scares you. But what this is asking in terms of our setup is what we want to set it up first. Again, you can add on to these incrementally. You do not need to create a new gateway.

**Naman Pandey** (00:13:01)

really really straightforward now because this is catered towards progress towards product managers obviously i know you all love to live and breathe on slack so we'll just be choosing slack socket mode some of you might be familiar with what socket mode is but don't fret if you're not because we'll be going through the entire setup on slack end to end for you all so great we can just use you can just have this be open claw Great. So the way this works is when I was setting this up before, these instructions are pretty bare bones, if I can put it that way. So what I did was I compiled actually easily followable instructions. Because the terminal instructions aren't the greatest, what I did was compile all of these instructions for you. If you're wondering where these came from, there's actually a TUI of OpenClaw itself where you can ask questions that you want it to do.

**Naman Pandey** (00:13:56)

So say you're stuck at any given stability, anything you're trying to do, you can actually ask OpenClaw to help you figure it out, right? So that's just what my source was for getting this. So we're going to be toggling back and forth between what it wants and how to get it. So as you can see here, the first thing it would like is the Slack Watt token. And it always begins with an XOXB. We see here the steps that we need to follow. So we're just going to be doing that step by step. Great. So just for this demo, I actually set up a brand new Slack for you guys just so we would be able to go through this together. Because as Akash was saying, there's a decent amount of pitfalls here to dissuade even the most... persistent of you all so we'll just go back here as you can see step one is go to api.slack.com forward slash apps so we'll just go there great so this is what you want to do create an app again for the pms out there i'm sure you know what i'm doing this is all very familiar for you all um next up like this explains literally everything right so it says choose from scratch and name it open claw so we'll say from scratch we'll say open claw here and then i'm just going to pick the one workspace that i have so this is straightforward enough we'll do create app so this is where the magic begins next up you want to select click socket mode on the left sidebar socket mode like this is really dummy proof you literally just have to follow these steps as you can see enable socket mode you just click that anytime you're confused just go back here toggle on a box will pop up asking for a token name call it secret token great no need to overthink this secret hyphen token hit generate perfect so it generated what looks like is something we need it starts with x app so we're just gonna copy it and keep it somewhere safe for now we'll be needing it in just a minute so this part is done as you can see though in our terminal setup it wanted the slack bot token so what we just did was kind of a stepping stone to where we're trying to get but we need that as well i think it lasts this after that but we'll just continue down our process so we did this we have we did this done part now we'll go back left sidebar oauth and permissions I lost my little window here.

**Naman Pandey** (00:16:13)

Great. OAuth and permissions is right here. Scroll down to scopes, bot token scopes. So, yep, this is right here. So we'll be adding all of the scopes that we want our bot to perform. What this translates into is we're going to be giving it permissions to read certain channels, respond to certain channels, make sure that it has all of the background knowledge really that it needs from all over the workspace to do its job really well. So as you can see, this goes over exactly all of the permissions that we need. So I'm just going to make this slightly thinner so we can see. So all we want to do here is, as it says, bot token scopes, make sure you don't do user token because that's something different. We don't want to do that. We just want to add all of these scopes. So you click that.

**Naman Pandey** (00:16:57)

First up, it says chat, right? You know, when you start typing chat, it just shows up. You click that. Then you go on to the next. So I am Reid. You keep going until you do all of these things. Obviously, feel free to skip any of these that you wouldn't want. It does explain what each of these things do. I would say all of these are important. But if you have an organization that has rules against these, by all means, feel free to skip. Channels, history is right. And then finally, groups, history. I

**Aakash Gupta** (00:17:27)

am right.

**Naman Pandey** (00:17:30)

Great catch. And actually, that is the most important one because we would not be getting any messages otherwise. Great. So that ends our screenshot here, but this is our final one. So we'll bring back our application. I'll just go full screen here. So once you save these, there won't be an option to save. What you want to do is go all the way up and you'll see this install to NPSpace option that you did not have before. So you just click that. It'll ask you for these permissions. You hit allow. Great. So now if you see this, this should now look familiar because this is exactly what we want to paste into our terminal. There are still a few more steps, but I'm curious to see at which point we will be prompted. That's not what I wanted to do for them. But for now, we'll go back to our terminal, paste our guy, hit enter.

**Naman Pandey** (00:18:23)

Great. So remember how I said the first, the stepping stone, quote unquote, this is where we'll grab that. Thankfully, we already expected this and we have saved this. So we'll just throw that here. Hit enter. So yep, we do want to configure channels access. I'm just, I have the liberty to just allow all channels. Again, if you have restrictions, feel free to act accordingly. Great. So if you see here, this is actually kind of important. So these directories that it's updating, remember that these don't live on the cloud somewhere. These are all on your computer. These are all local files that are saved on your machine. And as I was mentioning before, if you think this is too much work to just go through the terminal and do this, you can do one of two things. First, you can simply ask Claudebot or I should say open Claude to do all those things for you.

**Naman Pandey** (00:19:16)

Second, you can go into your finder, go to the file path, open the file using sublime text or whatever have you. and do whatever changes you want it to do manually. So those two are your options. So essentially what this is saying is that our Slack configuration is complete. When it says configure skills now, what it's talking about is unrelated to Slack. This pertains to one of the things that we were talking about before, which is a capability that OpenClaw has. So the two really important things that you want to set up, you can choose whether you want to do it while installation or later, are skills and tools. So the way Peter Steinberger, literally the inventor of this thing that we're demoing, chose to describe each of them was, and I quote, tools are organs. Can the agent do it? Versus skills are textbooks. Does the agent know how to do it?

**Naman Pandey** (00:20:07)

I feel like that really, for me, really put into perspective what these things are. Again, like I said, If I just hit yes to show you what goes on here, these are all of the skills that are... So these are all open source. These are just people and like good-hearted developers of the world. They just developed these once Peter Steinberger already made his project live on GitHub. So a lot of these are constantly evolving. I remember seeing one for Philip's home. Let that sink in for a second. You can use, you can WhatsApp something to a bot and it changes the light in the room that you're sitting in at 4 a.m. to wake you up. I don't know. I've just, that just breaks my brain to think that, you know, that's a possibility. Like I said, we'll just skip for now. The way to select it is by hitting space.

**Naman Pandey** (00:20:51)

And then if you hit enter, it'll just skip. Again, the reason why we skipped. Yep.

**Aakash Gupta** (00:20:55)

If you build

**Naman Pandey** (00:20:56)

it space,

**Aakash Gupta** (00:20:56)

it won't select it. If you just hit enter, you'll like hit this annoying issue. So just space, then enter.

**Naman Pandey** (00:21:02)

Exactly. Yep. And then, as I was saying, you're not really missing out because we will be going over how you can add hundreds of skills if you want. I just found it easiest to modify the text file. You can even use an LLM to generate a really long, verbose, super comprehensive skill and then paste that in versus having to do it this way. So this is just my preference. I think most people would agree. I don't think we need to set up go places just yet. So we'll hit no there. we're not generating images for now so we might as well just hit no but i think because you're using google one of the benefits is you can use your same api for pretty much everything vertex api allows you to use the same key for text generation image generation even if you're trying to do video generation using vo you can use that again it makes no sense to do this right now so we'll just hit no nope we don't want to do any of these things for now Great.

**Naman Pandey** (00:21:53)

So hooks is basically what we just talked about. These are the TypeScript trip that run inside the gateway when lifecycle events file. So what this means is once we have this all live, there will be one TypeScript pile that will run concurrently to everything that's going on. Hooks is how you set up that TypeScript file. This will make sense when we're doing the demo in a little bit. Again, as I was saying, everything is easily customizable after the fact. We'll just hit space to skip for now. Hit enter. And this is a really important step where it installs the gateway that we talked about. And finally, the moment we've all been waiting for. I just love that they say they're trying to hatch the board. I imagine like a little dinosaur hatching. I haven't seen this in other tools that I've played around with. It's I don't know.

**Naman Pandey** (00:22:36)

It's just like these little things that I appreciate so much. There is a web UI. I will be showing that in a bit. But for the full experience, we're going to be just using the hatch in TUI. So we'll hit enter here. And as it says, wake up, my friend, and we'll have the first message from OpenFlow here. Great. So we're

**Aakash Gupta** (00:22:53)

building this locally. Some people say you should build this in a VPS. Some people say you shouldn't. What's the truth about that?

**Naman Pandey** (00:23:00)

So really it depends on two things. First, your usage and second, your risk for appetite. So I'll be candid. One of the things that I was trying to do and we will be demoing that is there is a secure folder that you can make called docs and you can configure it to only interact with the documents inside the docs folder. However, when I was setting it up, I wasn't the most careful. And what ended up happening was on my Slack, it looked through all of the files that I had on my computer and it answered a question with a response that it really had no business knowing. So that is really the criteria here. If you use a VPS, sorry, not a VPS, but if you use the cloud, You have that one layer of abstraction that protects it from making changes on your computer, on your local files.

**Naman Pandey** (00:23:45)

You forgo that privilege the moment you just, you know, are not careful. I don't want to say that you're for sure you're going to be baking things, but you just owe yourself to be that much more careful and really kind of know what you're doing, which is obviously our goal here with, you know, content like this. So hopefully, does that answer your question? Any follow-ups to that?

**Aakash Gupta** (00:24:04)

So VPS, it can make it so your bot doesn't fall asleep. It can be a little bit more secure, but it doesn't have access to your local file system. And then also people use the Mac Mini, which is a totally different computer. Of all of the three, I think Mac Mini or a different computer is the best, most recommended after that local, after that VPS. But look in your own situation. For this demo, just continue with the local, I would say.

**Naman Pandey** (00:24:25)

Yeah, the only thing I would add to that is a VPS is actually also capable of making changes to your local or whatever. So VPS is, if we were to rank them in terms of risk, the riskiest, right? Because your computer need not even be on and stuff could be changing inside it and your bot could be actively creating or destroying things, you know, just like running amok. So what we have here, what we're doing right now, and thankfully what happens by default is that the moment I shut my laptop, the bot, you know, refuses or it just like falls asleep. So then we come back here. There's a command to wake it up again. And that's when things go live. So that is what I would recommend for most people. Again, there can be use cases where you don't, you're in a different room, you're in a different country and you want your computer to do something.

**Naman Pandey** (00:25:10)

It just depends. Yeah. To your point, Akash.

**Aakash Gupta** (00:25:12)

Awesome.

**Naman Pandey** (00:25:13)

So quick note on in terms of what just happened here. So as you can see, it says I'm awake, but I'm in a bit of a blank slate. So random, I guess, little segue here. The way this is configured is it auto runs a file called bootstrap.md and it tells it that what it is, right? That it's open claw. It has skills. It has hooks. It has a soul, a whole personality. And what it does then is that then it just kind of disappears, leaving it in like a dazed state. So which is why it's saying, so who am I and who are you? And this goes back to what I was sharing earlier with Peter's vision for this to force it to not just be, you know, like whatever, you know, chat GPT. Well, there's no personality. It's just something that you've typed messages to.

**Naman Pandey** (00:25:56)

He really wanted to hard code the experience feeling like this is truly your companion and not just, you know, somebody that you go to with your problems. so we are going to be speed running this we don't need to recreate the movie her here but I'll just say this is where I like to give it a name so you can just say your name is we'll just say fella right because it's just something I like to say so you can just be like hey fella can you you know blah blah and then I'll say I am Naman your lord And I will try and spell my name correctly because that will be problematic if I don't.

**Aakash Gupta** (00:26:31)

And how do you go backwards in the terminal? Some people don't know that.

**Naman Pandey** (00:26:33)

Yeah. So again, all arrow keys. And sometimes you can hit the up arrow to invoke previous commands that you've used. But as you pointed out, there's no such thing as a mouse. You're just completely reliant on your arrow keys. Great. So I'm just going to hit that. It's going to ask me a couple more annoying questions. i say annoying but you know you know what i mean i appreciate the you know idea or whatever okay yep so here's yeah so it forces you to pick one of these three options it can be a creature a vibe or an emoji do you want to help me fill this out akash any any of these looking good for you oh my gosh

**Aakash Gupta** (00:27:09)

it

**Naman Pandey** (00:27:10)

says just a really good

**Aakash Gupta** (00:27:12)

fella Um, PM sidekick that is a proactive helper with no emoji signature.

**Naman Pandey** (00:27:24)

I said that 10x is my career. Act like you mean business and no signatures ever. It's going to say something snarky if I were to guess, but we'll see.

**Aakash Gupta** (00:27:39)

I've never actually run it in Gemini, so this is like a little bit slightly different. I always use Codex, so I decided to see this.

**Naman Pandey** (00:27:45)

Interesting. So look, pretty much this, like it's live. We're ready to fire. We can get into... Actually, this would be a good point to flash the UI. Like I said, at this point, my first question is, is the gateway connected or not, right? Like that's a perfectly normal question to have. Instead of fretting, I'm just literally going to ask it. Is our gateway live and connected? And the good thing is, if it's not, it will actually connect it for you. One time it needed like a token for its gateway, which I did not know where to find. So I just asked it, where is the token? And it just gave me the token. So look, it says it's live and active. Perfect. So once you're done setting up, we hashed our bot. It will allow you to go to this front-end gateway, which is the UI version of the gateway, which lives on 127-001-18789.

**Naman Pandey** (00:28:34)

That's just the default port it uses. So this is what that looks like. I can just share a brief overview of what this all is. So the chat is really just the way you can communicate with OpenClaw itself. Usually, and as we discussed, The best way for it to do something is just ask it to do a certain thing. And it's really good at programming itself to do whatever you asked it to do, right? So that is still the biggest USP of why we want to use OpenClaw. Like that is the unlock that it brings. That you don't have to sit and build all the components that you need. You just tell it that, hey, build this for me. And it almost architects itself, spins up other bots that it then manages. It does all of that autonomously for you. So all of that happens in the chat.

**Naman Pandey** (00:29:17)

This overview just shows your gateway token and such. Just, you know, stuff that you need to know, everything that you've been doing. A couple other things. If you ever want to change what API you're using, so say you want to swap from Gemini to Anthropic for some reason, you can go into config. If you scroll down, you'll see this option called secrets. This will sometimes not open. That's totally normal. If you click raw, it'll show you what model you're using. So within Gemini, right, you know, we have one API key for all Gemini offerings. So if you want to use like a faster model, you just have to change this out, hit save, update. And that's how you can swap out your models and such. Having said that, as we know, you can also simply go on the chat and just say, hey, I want you to use model name, blah, blah, blah.

**Naman Pandey** (00:30:03)

And it will automatically program itself. So that's that section finishes the setup of open claw itself now for our pms we want to obviously live and breathe within slack so we already set up our new app we called it open claw you saw us do that now there are some important settings that we need to make sure we have before we we can start talking to our bot add it to slack channels have it read and write messages and such we already did the two most important steps which was the app token and the bot token in addition to those, you want to make sure that when you go on OAuth and permissions, you should be able to see these bot token scopes. So the thing that's finicky with OpenClaw is that it doesn't tell you this right out of the gate that you need to do these things, which is somewhat understandable, right?

**Naman Pandey** (00:30:49)

Because most people maybe aren't trying to read groups or they aren't trying to look at what users are trying to do on Slack. So these are the three things that we will be using for all of the demo cases that I have prepared. It can very well be the case that something that you want to do needs a certain other permissions. Adding that is really straightforward. You just click that, mention whatever you want to add. The most key important thing here is no matter what you do in Slack when it comes to your app, you always want to click reinstall to your space because unless you do that, it will not work. It will not persist. So make sure that no matter whatever changes you make, you always reinstall to NPSpace. Very rarely that makes this OAuth token change. It doesn't happen all the time. Very rarely it will change.

**Naman Pandey** (00:31:33)

In which case, make sure you just copy and paste it back to your OpenClaw gateway, which we had right here, and it will automatically update everything it needs to do in order for you to get to this OpenClaw within your app. like that's just how so as you can see i tested here when you just say hi it just responds to you at first it will ask you to use this key which you as we as we know now we will just go back and paste that key and once you do that as you can see it'll just come alive now from there it's obviously very straightforward it's simply a matter of adding it to whatever channels you want to add it to again this is just some testing that i was doing here but as you can see You can just invite it to its channel and then add it.

**Naman Pandey** (00:32:12)

And then once you do, it'll be able to just, you know, lock and load right from that point. This section completes the setup of OpenClaw within your Slack. I'll pause real quickly, Akash. Any questions that come to mind? Anything you want me to shed more light on?

<!-- sponsor -->
**Aakash Gupta** (00:32:26)

Before we dive deeper, let's talk about something every PM faces, getting alignment on product decisions. You know that feeling when you're trying to explain a user flow to engineering or justify a design choice to leadership and you're just describing it with your hands? That's where Mobbin comes in. Mobin is the world's largest library of real-world mobile and web app designs from industry-leading apps like Airbnb, Uber, and Pinterest. Instead of spending hours taking screenshots or hunting for inspiration, you can instantly find exactly how successful products handle onboarding, paywalls, checkout flows, whatever you're facing. Over 1.7 million product builders use Mobin to benchmark against best-in-class products and show their teams proven solutions. Whether you need to convince stakeholders there's a better way to handle user activation or research how top apps approach future discovery, Mobbin gives you the visual proof to back up your product decisions. Check out mobbin.com slash akash.

<!-- sponsor -->
**Aakash Gupta** (00:33:19)

That's M-O-B-B-I-N dot com slash A-A-K-A-S-H and get 20% off your first year. AI evals are one of the most important skills for PMs. And I know you know they matter. The question is, are you doing them right? Most teams are winging it with basic metrics and hoping for the best. Meanwhile, the teams that actually ship reliable AI, they've cracked the code on systematic evaluation. Today's episode is brought to you by the AI evals for engineers and PMs course by Hamil Hussain and Shreya Shankar. This live Maven course will teach you the battle-tested frameworks from Hamil and Shreya, who are the engineers behind GitHub Copilot's evaluation system and 25-plus production AI implementations. Four weeks, live instruction, next cohort starts July 21st. Start shipping AI that actually works. Enroll at maven.com with my code AG-product-growth for over $800 off. That's AG-PRODUCT-GROWTH. I hope you're enjoying today's episode. Are you interested in becoming an AI product manager?

<!-- sponsor -->
**Aakash Gupta** (00:34:32)

making hundreds of thousands of dollars more, joining OpenAI and Anthropic, then you might want to do a course that I've taken myself, the AIPM certificate ran by OpenAI product leader, McDad Jaffer. If you use my code and my link, you get a special discount on this course. It is a course that I highly recommend. We have done a lot of collaborations together on things like AI product strategy. So check out our newsletter articles if you want to see the quality of the type of thinking you'll get. One of my frequent collaborators, Pavel Hearn, is the Build Labs leader. So you're going to live build an AI product with Pavel's feedback if you take this AIPM certificate. So be sure to check that out. Be sure to use my code and my link in order to get a special discount. And now back into today's episode. When I use OpenClaw in Slack versus the TUI dashboard that we're seeing in the other tab, are there any limitations or is it fully featured in Slack?

**Naman Pandey** (00:35:25)

Great question. So the way to think about the TUI and this UI dashboard, so we can just call it the gateway dashboard because that's what OpenClaw likes to call it. So what you'll see is that whatever you talk about over here will automatically get reflected in the terminal UI as well. So it's the same thing. There's really no difference. So, you know, so hopefully that answers that part of the question. These two are the same things. Most people will want to use this just because of the benefit that pasting images unlock when you're talking to any LLM, right? It's just, it's worth a thousand words, especially in this case. So that's where, so you can think of this as your control center, your command center, if you will. What I mean by that is, as we were seeing here, I was running into some issues with setting this up in my channel, right?

**Naman Pandey** (00:36:08)

So to troubleshoot that, where am I going to go? It's not going to work if I ask OpenClaw on Slack to fix itself. So we need to go back to our control hub, which is this gateway dashboard. So really, suppose we were trying to do WhatsApp as well, right? You can ask OpenClaw on Slack to set up your WhatsApp for you. Actually, as I say that, maybe it will be able to. But even for that, you'll need an entry point. So really, this gateway dashboard is an entry point to any and all of the other apps that you want to leverage. OpenClaw on, be it WhatsApp, be it Slack, be it Telegram, all of those things. Like the first hub that you go out into the world is still this. Does that answer your question?

**Aakash Gupta** (00:36:44)

Yeah. So are we fully set up? Are we ready to see it in action?

**Naman Pandey** (00:36:47)

We're ready to see it in action, actually. And there will be some other things that we'll be learning. But the way I have it constructed is we can just go through them as we go through our use cases itself. So with that, I'll launch into use case one. And as is tradition on your channel, we will be leveling up, right? So we'll start kind of dipping our toes a little bit, just exploring what's possible. And then for the final use case, I have something that hopefully will leave at least some of your viewers' jaws on the floor. That's my goal with all of this. So yeah, let's jump right in. So use case one, and I can throw this on the screen as I talk to this. So use case one is that we're going to turn any Slack channel into an AI-powered knowledge base that answers team questions from your product documentation.

**Naman Pandey** (00:37:30)

So what we'll be doing is we'll be dropping our PRD, FAQ documentation, any product wiki into the workspace folder, which I'll show you where that is and how to find it. And then anyone in the channel can simply mention the bot to get instant contextual answers. Why should PMs care? Because it just simply eliminates the product questions channel problem where PMs have to spend hours answering the same questions about feature specs, launch dates, and edge cases. Again, it's important to note here that this repository is not locked in. It lives and breathes as a living space. You can add and remove stuff to it. The memory persists. So if you ask it, hey, what is an FAQ that we added three months ago that wasn't there six months ago, it will be able to tell you that, right? Because it's not just locked in time, it lives and evolves with you.

**Naman Pandey** (00:38:13)

So we will be basically building this out for our first use case. So now as we do that, the first question that naturally is probably arising for our listeners is what is this workspace that I mentioned? So this is tied in perfectly to the really cool capabilities of OpenClaw because I'm sure at least some of you are wondering what exactly is the USP or the use case for using OpenClaw against Slackpot, right? Because if it's just answering questions on a channel, Slackpot could probably be configured to do that as well, right? Here's the difference. Slackpot does not have access to local files that live on your computer. Neither does it have the ability to read or write into those files. So this folder here, which is just called dot open claw, and some of you will struggle in trying to reach it. So I'll show you a quick tip on how you can easily access it.

**Naman Pandey** (00:38:59)

So if you click your little finder icon, right click it, sorry. And then if you go to go to folder, if you just press a period, it should show you an option to go to open claw. This is really annoying because it doesn't, it's not like a folder that you can just go to, at least not on my computer. So it took me like 10 minutes annoyingly to figure out how to get here. this folder that we have here now yours will not look like this exactly because i've been as i said playing around with it a decent amount what you need to know is this workspace component this you will find already pre-setup for your for your own computer as soon as you install openclock with some of these files such as agents heartbeat soul tools memory and user what are these i have these written here real quick soul md is your d personality or values identity is the agent identity User is just all of your preferences, which in my case, as we saw, we had it be really direct, not no beating around the bush, super to the point.

**Naman Pandey** (00:39:59)

Memory is stuff that persists. So even when you close your bot, you shut your computer down, this stuff still continues to be alive. And then tools are your local configuration nodes. And finally, heartbeat, which is really important, is a list of all of your cron jobs that it signals that, hey, now is the time to run this recurring task. So I can just open one of these just for you guys to look at. So we'll look at heartbeat. You can simply open with sublime text. Otherwise, it tries to open Xcode, which is kind of annoying. Some of you might not have that. But look, this was all pre-setup. This is something that I set up. So this you will not have. So originally your heartbeat.empty will be empty, right? Because you don't have any activities that you wanted to do automatically. One other cool thing about this is if you go back to your gateway dashboard and if you go to cron jobs, here is also a really cool way to see all of the activities that you have running along with the ability to edit or modify it.

**Naman Pandey** (00:40:54)

So we'll be going over the use case for this in just a minute here. But for now, as we were discussing, we wanted to have a repository for our files where we can throw our documents and then query the Slack channel. So in my case, I simply just made a document or a folder called docs. Once I go into it, it has this PRD document, which I can flash. The quote unquote made up slash semi real product that we'll be working with through these demos is something that I'm actually working on. It's really just a one click setup of websites for podcasters just using their RSS feed. So that's my whole big idea. You just submit your RSS feed. It gives you a fully functional, really nice looking website. So what I did was I just generated a PRD for that. As you can see, it's just like, you know, pretty run-of-the-mill stuff.

**Naman Pandey** (00:41:39)

And I threw that here. What I have not done is I also have this file called an FAQ, which I had not added to this folder yet, but that I'm going to in front of you. So my goal here is to demo that even though this file was just added to this, it will still work and it will continue to do its thing, right? So I just, as you saw, drag this over here. I'll make sure to rename this in a way that it can read that hopefully. Will it enter? Will it add? Great. So now our initial document setup is ready. So as we talked about, we will now be querying our bot. And you can do this on any channel or you can do it directly. It kind of really doesn't even matter. But maybe we'll just use a channel that I'd added it to, right?

**Naman Pandey** (00:42:22)

Or maybe we'll go to bug reports. Really, it can be any channel that OpenFlow is added to or just the directly OpenFlow channel itself. So we'll go here. We'll say look through the docs in your workspace folder and tell me the... I actually even had a question ready for this. So let me pull up that question. It should be right here. Yep. So I wanted to outline the database schema for handling this RSS and AI data. So I'll just simply post that. So we will run this. I expect it to... Oh, and remember, guys, you always have to tag it. Otherwise, sometimes it can be iffy. So just to be sure, I'm going to resend with having tagged it. Although I do think it should work, but we'll just resend it just in case. And now we wait for it to respond.

**Aakash Gupta** (00:43:10)

So what do we expect to be doing in the background?

**Naman Pandey** (00:43:14)

yeah so great questions okay great so as you can see it's churning out some stuff so yeah akash what it does in the background is that it goes into its root folder it knows that docs exists there it can see inside it to find whatever it needs right so then it looks through that document and then comes back to the original request and then in this case it answered my question based on the dock that it found. Let's test and make sure that it found the FAQ that I just pasted in as well. We'll say, are there any FAQs that we missed in the FAQ dock? My plan is whatever it comes up with, we'll actually have it right to the dock itself just using Slack without me lifting a single finger. So let's see how it fares with that.

**Aakash Gupta** (00:44:05)

So it has access to docs and can edit them if they're in Markdown.

**Naman Pandey** (00:44:10)

Exactly. That's exactly right. Realistically and technically, it has access to every file on your computer. Right now, it doesn't. Look, interesting. So it did find the FAQ.txt without me telling it explicitly that I just pasted that in, right? So it found those things. Look, it even offered me I can append these. Let's say, sure, let's do that. So the important thing outside of this little toy demo here for, you know, your listeners is that these can all be lifetime. Remember, I am right now sitting here doing these things, but it can very well be that maybe one of your leaders or one of your customers reach out saying, hey, this is a question I have. Why is this not on your FAQ? Maybe you can even get an email on this. And that is actually subject for the next use case. But you can have it set up to be automatically making doing these operations in real time.

**Naman Pandey** (00:45:02)

So apparently it claims to have added it. So we'll go back to our thing here. It even added the SQL schema that I'd asked it to just to make sure that I can access it later outside of Slack as well. So if I open this file now and I'm now realizing it would have helped to show a before after. But hopefully we can see any differences in the way they're written. Yeah, they even labeled it with additional features and infrastructure. And it added those four questions that it thought that it should have. So again, going outside of this toy example, you can have... dozens of files in this folder, right? This is not limited to just one PRD and one FAQ. It has the ability and the context to sift through all of them and really customize its responses to what it's seeing in that folder.

**Naman Pandey** (00:45:47)

That concludes demo of use case one. Before I launch into the second one, do you have any questions, any clarifications that I can do?

**Aakash Gupta** (00:45:55)

So I see this as an instant knowledge base. This is about if you can construct a really strong repo of, Hey, these are the features we're going to build. This is the strategy. These are the transcripts of every customer conversation. These are all the relevant data charts. You can scale your impact. And the flow can be that your engineers and designers, they go out there and they come up with a future idea. They chat with your knowledge bot to come up with the proposal. Then the human actually comes in and actually reviews it. And the PM can actually really scale their impact this way. So with the way ratios are going, PM's supporting more engineers than ever. I see this as a really important tool to multiply your leverage.

**Naman Pandey** (00:46:33)

Not only is that a great call out, but the aspect to that that you mentioned where you can build that repository, I would put a little asterisk in that and say that you actually don't even have to build that repository. OpenClaw builds that for you, which it's funny you say that because that is exactly what use case three is. But for now, for use case two, what I had was the pain point, quote unquote, being which I will paste here again. And you know, I know enough PMs to constantly hear about this being a huge pain in their behinds and honestly even like software people, right? So automated daily stand-up summaries. What it does? Every morning at 9am, Open Clause scans your team's Slack channels. These can be as many channels as you want. It summarizes what happened overnight, identifies blockers and posts a concise stand-up brief to product stand-up.

**Naman Pandey** (00:47:24)

Why should PMs care about this? Because it replaces the 15-minute context gathering ritual I actually saw a post on LinkedIn just earlier today where somebody was like, the bane of my existence is on every Monday. I have to sift through all of what happened last week and compile that to share on my weekly standup. So you walk into your first meeting already knowing what shipped, what's blocked and what customers complained about. Before I launch in, any thoughts on, you know, this particular use case? Would you agree that this is kind of a pain point for PMs? It would be helpful if you can add your take to this sort of detail.

**Aakash Gupta** (00:47:57)

Yeah, sounds great. Especially if your teams are reporting into Slack channels. And if they're not reporting into Slack channels, we can configure other data sources, which I think we'll cover in a bit. But if they are in Slack, this is perfect.

**Naman Pandey** (00:48:08)

Perfect, yep. So as you can see, in this case, I have an engineering channel setup and a design. So what I was hoping to do, and you can, you know, you can tell me if this is a bad idea, was for you to even have an addition to me, just write tough here that, you know, this broke, this doesn't work, I'm going on leave, whatever you will. So our goal is to really like confuse it. If you know what I mean. And then we'll run the cron job. And by the way, because I was testing it, you can see the morning stand-up summary that dropped sharp at 8 a.m. my time because I'm CSD. So, you know, it did its job. But obviously, it's not limited to just 8 a.m. We can even run it whenever we want, right? So, what do you think if I invited you here?

**Naman Pandey** (00:48:53)

Akash, would you... Help me spam this. Here, I'll grab your email and we can like blur out your email, but I thought this would be a fun activity. We will directly add you to NPSpace. Great. And while that happens, I guess I'll add you to design as well. Let me know if you were able to access. But in the meantime, I'm just going to start, you know, we'll just pretend this is an actual engineering Slack channel. We'll say, I guess I'll say I'm going on leave starting tomorrow. So my sprint will be extended. by two days and we'll just and i'll just hyphenate and say my name just so it knows and then for design i'll say um the back button is broken and i don't know how to fix it without talking to my design lead okay we'll just send that right so we're obviously just trying to you know yeah exactly just a bunch of updates come in all day and as i as i showed you on the product stand up this will be generated tomorrow morning when we are no longer on the call but we'll just have it generate now right so for that i'll just say open clock um And yeah, so one important thing here, you can obviously ask it to generate the morning standup summary.

**Naman Pandey** (00:50:11)

The other thing you can do to set this up is, and I guess I can now show you guys how you can do this. But the way to do this is set up a cron job. And this is what that looks like. So you just go on your chat and you just mention that the following command, right? So what I like to do is go on whatever Claude or what have you and just type out in simple English that at 8am I need to know blah, blah, blah. Basically the problem statement that I just shared. Now, you can even paste that here directly. What it will do is it will automatically convert those English instructions to system readable code, quote unquote, if you will. Which, what does that look like? The following. Set up a cron job. That's the command for that. This 09 stuff refers to the time zone.

**Naman Pandey** (00:50:55)

Session isolated message. Yeah. So it reads the last 12 hours in those two channels. You can add a certain channel here if these aren't enough and it will summarize what shipped, what active blockers or escalations, key customer complaints, right? And then post a summary too. with clear headers. What you can also do is have an associated catchphrase for this to trigger. Just, you know, like Iron Man style. If you use Whisper Flow, you just press your little activate button and you just say stand up and you just hit enter and it does everything else for you, which is, you know, it's really cool. So I'll just be trying to demo that here. So I'll just say stand up and we'll make sure there's no space and we'll see if it's able to run the cron job and give us all of these new updates that it now has.

**Naman Pandey** (00:51:42)

So fingers

**Aakash Gupta** (00:51:43)

crossed. Product managers are getting one step closer to Iron Man.

**Naman Pandey** (00:51:48)

Okay, so tell me if any of this feels accurate because you inputted some of those things. Five features have been shipped. Three new templates have been shipped. There's a few blockers. UI development is on leave. Unable to fix broken back rate. I'm also going on leave extending by two days. So, I mean, again, I don't think anyone is surprised here. Oh, if this surprises anyone, it's because of testing that I was doing earlier. But... Yeah, you no longer have to comb through a bunch of Slack channels. And as you will see in our next use case, even stuff outside of Slack, it just constantly lives, breathes. It's pulling all of these various avenues and then consolidating them for you to just, you know, be in your own bed and not even have to join the call or whatnot and, you know, just be relaxing. Not that that's what PMs do, but...

**Aakash Gupta** (00:52:37)

Yeah, we all live in Slack hell with way too many messages and notifications. It's impossible to keep up. So now you have somebody who's there that you can converse with basically and get caught up on Slack.

**Naman Pandey** (00:52:49)

Actually, on your point around the conversing, we can even ask it, what's here that needs my immediate attention, right? Because if you're trying to not get overwhelmed by all of this stuff going on, it is smart enough to figure out what you need to immediately act on. In this case, I'm hoping it will bring up this print stuff because that's a big blocker in my view. Yeah, exactly. Right. So you're going on leave. Also, notice how it knows that Naman is me. So it didn't say Naman here. It said you. Ensure your tasks are handed off or documented. Anyway, we don't need to like check its work. But what's the takeaway here is that unlike other LLMs, right, which constantly lose memory, run out of context size, run out of token windows, this is built to constantly make sure that it regurgitates, if you will, the right context size to not lose sight of what's important here.

**Naman Pandey** (00:53:40)

That's really the headline here and not, you know, the nitty gritties of what we have here. So before I move into use case 3, just wanted to pause. Any thoughts, questions, anything else that's coming to mind with this?

**Aakash Gupta** (00:53:52)

Let's

**Naman Pandey** (00:53:53)

move on to 3. Perfect. So for use case 3, we have the following. What this is, is really competitive intelligence pipeline on autopilot. It basically monitors all of your competitor avenues. Right now, this just says websites, Captera reviews, product hunt launches, hacker news mentions. You can have this list be 15, 20 items long, right? There is literally no stopping this. What it does then is that it synthesizes a competitive intelligence brief. using SWOT analysis, and it posts it to a private competitive Intel Slack channel. Why should PMs care? It's because obviously doing all of this manually is really critical. In addition to that, say there were certain changes six hours ago on a competitor website, you happen to be sleeping, right? When you woke up the next morning, they had overwritten that for change C instead of change B. In a normal world, that is gone forever.

**Naman Pandey** (00:54:47)

You have no way of ever finding out that that happened. Not with this, right? OpenClaw never sleeps. It's just out there, you know, doing its thing, monitoring it every hour, every half hour, if you can set up to do that. And then, yeah, that comparative brief lands in your Slack without anyone lifting a finger. So the way I want to show this here is by actually building this out. So I did not, in fact, end up building everything because I did want to show what the building looks like. So really what we're doing is what I just said, right? We go on here, remove that. And I have the prompt pre-ready just because I didn't want to waste time. But in your competitive Intel Slack channel, just mention the bot with something like I need blah, blah, blah. Search the web. And I customized this to our use case, which was latest news, product updates, and user sentiment about PodPage, which is, and TransistorFM, which are my competitors for the toy example, toy slash series example that I was trying to build.

**Naman Pandey** (00:55:45)

Organizer findings highlight anything that represents a threat or opportunity for a mid-market podcast website builder site. Poster analysis will say there. So what is going to happen is, first of all, it will say there is no competitive Intel Slack channel. And it will make us do all of that rigmarole. So let's actually build this out so you guys can see what exactly that looks like. I mean, while it does that because, you know, we like to be proactive, we can simply make that channel right, make sure we have the right name. So we'll simply just copy that, make that channel, hit next. You can just have it be public. Great, we'll just add everyone. And then I guess we'll also add the app because I don't think that is added. Yep. Great. So we did that. It's still thinking. We'll give it some time to

**Aakash Gupta** (00:56:32)

think some more. So when you want to look at the context and that it has, is there a way to look at that? Because I know with Cloud Code, managing the context is a really important part.

**Naman Pandey** (00:56:43)

yeah so a big part of the context lives on these files itself so for instance if i showed you agents right like what are the agents that it's working with so i'll flash it up here so this is you can think of it as its consciousness if you will right so this has everything that it needs to run so for safety this is just all default so don't exfiltrate private data Don't run destructive commands, so on and so forth. Ask first, right? So for anything like sending emails, tweets, publics. Again, this is just boilerplate. You can change all of this. So again, the way to work this is you can go on your Claude or Gemini, whatever, and then have that build out the entire markdown document. Suppose you want five different agents that Fela, in our case, leads. So you can have that organizational map that Fela, Bot A will just say Naman is responsible for marketing.

**Naman Pandey** (00:57:38)

Bot B is responsible for so on and so forth. And then if you just paste that markdown file into your workspace here, it will know exactly what you want it to do at any given point, right? So that is the way to manage not just what you want it to do, but also what you want it to work with in terms of the documents and such.

**Aakash Gupta** (00:57:57)

And in terms of those documents, agents, what are the best practices? What goes in what document?

**Naman Pandey** (00:58:01)

Yeah, so the good news is that this will all be set up for you by default. You will not have to worry too much about changing a lot of things. Again, if you were to want to change this stuff, there is a line here that it always makes me feel philosophical. But I forget exactly where it is. Like, for instance, look, remember what I said about the stand-up stuff? Look, and this is not something I've written. This, it wrote itself. So if Naman types the exact words stand-up in any context, he must use the message to, instead of replying directly, call message with action read. This is all, this is like my Slack channel stuff. So it configures itself to act according to, you know, how you want it to.

**Aakash Gupta** (00:58:44)

Nice. So you could just chat with it and it'll update those files over time.

**Naman Pandey** (00:58:47)

Yeah, that's exactly right. Perfect. So it did its business. It actually started doing the analysis first, which is not something I was expecting. So this error around the missing Brave key is just, Brave is really just an API that any agents do, even if you use Cloud Cowork or now today ChatGPT came up with their entire task-based thing. But it really makes it simple for agents to browse the internet. So we can set up Brave API key. That's straightforward enough. But for now, it says, yeah, it didn't find the channel, which is something that we had forecasted. So what we will do now is as firstly, we have this channel. So something you need to do to point it to your channel is go on here. And if you click channel details over here, you'll find the channel ID. So you can just simply copy that.

**Naman Pandey** (00:59:39)

Go here and say the channel ID. ID is that. So, and then as we just talked about, it will configure itself to be able to talk to that channel and such. Now, while it does that, we can go ahead and do the Brave API key setup. This is important because pretty much any type of web browsing activities that you're going to be doing will involve this. I believe it starts at $5. Yeah. I think that was where we had started. So I think I already should. Okay, I do have an account. I don't think I have an API key. So I guess I'll just like configure this up real quick. So we have our API key. We'll just add that. We'll just say open clock. We'll hit add searches. There is fine. That's our guy. We'll copy that, go back here. Great. So I successfully posted that message.

**Naman Pandey** (01:00:32)

We can verify. So if we go back, great. So it was able to do that. All it needs is an API key now, right? Everything else is ready to go. So we just come here and we say Brave API key is... And this can stay because I'm going to delete this immediately after. But the important takeaway here is normally for anything else, what you would have to do is go into your VS Code file, go into your environment variable, paste the API key, then attach that variable to anywhere else in the code where you would need to access it. Here, you just dump it on this nice little interface and it puts itself to use and it pastes the API key everywhere it needs to without you having to lift a single finger. So, yeah, and the reason it disconnected is because it needs to refresh.

**Naman Pandey** (01:01:18)

And I think that's the API response. If I'm not mistaken, apparently it did it. So we'll say, we'll just say, run the competitive analysis right now. And we'll hit send. And then we should see a message here. Actually, what I should have done was write that, you know, prompt here. But it's really the same. You can use them interchangeably at the end of the day. They're all going to the same source, if you will, even though the avenues are different. Great. So as we know, it is smart enough that it knows that it's supposed to go there. So, okay, let's look at the analysis. So I actually use port page and I've used transistor as well. So let me quickly just eyeball this and see if it's looking accurate. Aggressively targeting podcast. Okay, that's That's accurate. Allowing multiple shows. Yep, that's true. Many built-in sites are rudimentary.

**Naman Pandey** (01:02:16)

Yep. I mean, I can show my site that's on Port Beach and it's just the worst. Sorry, no shade, Port Beach. Migration tooling. Since Port Beach relies on a white glove, seamless could be a massive conversion driver this is gold so i'll show you what i have been working with this is like my very rudimentary pre-mvp stage something i had not thought about so far was exactly how to make it really easy for other folks to import their pages um into into this this is just what i have right now and my plan was to go away from the whole wordpress type route So it did accurately identify this super cool, at least to me, angle or wedge here that it could be a massive driver to seamlessly allow people to go from WordPress to, you know, platform migration in terms of opportunities. Video integration. This is one of the biggest reasons why I even had this idea and I have that or at least I'm working to have that be built in.

**Naman Pandey** (01:03:18)

Because most podcasts now are video enabled, right? So I wanted this to be video first. So I have not seen this before. This is the first time I'm seeing this in work. And like, at least I'm definitely impressed by what it's saying. Let's look at risks. They are pushing native network websites, reducing the need. That's a fair call out. If hosting platforms improve their native site builders, standalone will lose market share. perfect so i mean in a sense that does conclude our uh this demo but what's important here

**Aakash Gupta** (01:03:48)

one question i have is any ai tool you ever build like i've had agent ceos like lindy and relay you and i did the agent browsers and People talk about Cloud Code and co-work. They always use this comparative analysis use case. So how does OpenCloud differentiate from all those other AI tools?

**Naman Pandey** (01:04:08)

I would say the biggest differentiator, and at least I know for a fact that this is not possible to do using any of your AI first browsers. Definitely not when we are recording this on 5th March. But the biggest takeaway here or like the wedge, you know, if you will, here is that first, we don't have VPS set up right now, but you can have it be polling Google reviews. You can have it be polling a bunch of different avenues that it would just be really hard. for any other or even Claude Cowork for that example, for that matter, to look at actively every 30 minutes and then persist with its memory so that six months down the line, if you asked it to say generate a trend line of all the changes that a certain competitor made that helped or hurt their business when it came to reviews on Reddit or on Twitter, it's like basically having a watchdog across any website that you can think of that literally never sleeps.

**Naman Pandey** (01:05:10)

And along with the ability of it being really smart and you being able to converse with it in real time in a way that it never forgets a single update it saw like 7.35.2 hours ago at like 1 a.m. when you were randomly sleeping. I will say with Covert, the difference is a little bit lesser. For me, the differentiator then becomes cost. Because remember, you can run Quint 3.5 on this. Quint 3.5 is one-tenth the price of Anthropic APIs. I am, like, mortally afraid of ever using Anthropic APIs because... One prompt and it burns through $20 like it's nothing. I don't know if you've had a similar experience. But when you couple similar-ish abilities with the ability to be really agnostic with your AI LLM usage, I do think that's the democratization of it all that really makes it click together. And for me, I actually don't even do a bunch of things just because of how expensive it is with co-work in particular.

**Naman Pandey** (01:06:17)

I'm actually afraid to use co-perk, but not with this, right? Because Quen can get you, I would say, per my experience, at least 60-70% of the way there for one-tenth the cost. And for most people I'm willing to wager, that's a fair enough standoff or trade-off, I should say.

**Aakash Gupta** (01:06:35)

Okay. And you mentioned about the VPS part of that. Can you say more on that?

**Naman Pandey** (01:06:41)

Yeah. So you can have this be doing operations within your file system when your computer isn't even on or, you know, when it's like shut down. You've shut down your computer and it still will be able to do things without actually you being around or being in the same country. Again, that is risky. I have not, I'm just personally worried to play around with it and not to go off on a tangent, but I was trying a bunch of WhatsApp initiatives yesterday with OpenClaw. It decided to message everybody that I was talking to for two hours after I'd done my demo, just with trying to pair with their phone numbers. So I would say, and nothing I ever did would have prompted it to do that according to my brain at least. So Yeah, yeah. Like I was talking to my mom and it auto sent her.

**Naman Pandey** (01:07:33)

And firstly, I asked it that, do you have access to my other chats? And it was no, I can only chat with, you know, like how you have your own chat on WhatsApp. I was like, great. Except clearly that's not true because it sent her the like secret code to attach to her number as well. And my mom was like, what is this? What is going on? And I was like, don't worry about it, mom.

**Aakash Gupta** (01:07:55)

Okay, so beware connecting your open claw to your work Slack and your WhatsApp. It can go off and do autonomous crazy things. So you need to do it in a safe way.

**Naman Pandey** (01:08:07)

I will say to just to caveat with Slack and with any here, I'll put it this way. Any default things that you're doing, quote unquote, are probably fine. I've not seen it misbehave on my computer so far. Not that I can see at least nothing that I've noticed. So for most use cases, you are probably fine. But just remember that it comes built in with most security guardrails in place. And just make sure you're not trying to move them around unless you have a really strong reason or if you really know what you're doing. For most people, for most use cases, if you stick to the default guardrails it comes with, I think, and please don't quote me on this, but you will probably be fine. With Slack and such, you don't have a lot to worry about, right? Because the moment you start to worry, you just disconnect it, right?

**Naman Pandey** (01:08:58)

It's literally a one-click operation to delete this app from your Slack and you're good, right? It's as simple as that.

**Aakash Gupta** (01:09:03)

but I will say famous last words famous last words I think it was the meta super intelligence safety lady on twitter that's she posted about how she had to like run to like physically unplug her open claw from like deleting her emails or contacts or something like that

**Naman Pandey** (01:09:20)

it's true Yeah. So, and it's funny you bring that up because to do that, OpenClaw would need, that's right, Brave API, which we just gave it, right? And I do have a use case around that as well where that concerns with email. But it's a good point. Now, I guess what's not reported is she probably taught it or asked it at some point to do delete related operations on her email. I'm not trying to victim blame here, but, you know, we can go on. But that's just my two cents

**Aakash Gupta** (01:09:51)

on the topic. So while we're talking about it, we have to give people the guidance. How do they launch Open Claw safely, securely, implement the stuff we've been teaching them so far without being worried it's going to WhatsApp their mom a secret key or delete their emails? Beautiful.

**Naman Pandey** (01:10:07)

So the way I like to do this is instead of guessing, let's just simply go to the source of the quote unquote problem, which in this case is also the solution. So we will directly say, based on the way you are set up on my machine, I need you to do a thorough analysis of security vulnerabilities and tell me where I am at risk and what we need to do to fix things. Do not make any changes. I'm just looking for direction here. The good news here is that it doesn't know how to lie to you yet. So it will just tell you. But I'm so glad you brought up this question, Asash, because no two cases are the same. And I really encourage people that are dabbling in this to consistently run this. You can even have a cron job for this every week so that it automatically tells you that, hey, last Sunday when you were playing with email, you left this on.

**Naman Pandey** (01:10:56)

This could be a problem. Let's switch that off. so it's really just hygiene you know it's in the industry we call it security hygiene and thankfully in this case it's there's an easy way to do that but i am actually curious to see what it tells me because i have been according to me pretty reckless so so we'll see great we'll let it load here yikes firewall is disabled that's never fun okay So yeah, a bunch of risks around Slack, which in my case obviously makes sense because this is my toy Slack, you know, I'm not actually, you know, doing stuff. Unrestricted file system access, all of this stuff needs to be fixed. So if a malicious or rogue user in Slack tells OpenClaw to read your personal Mac files, it will likely execute it. Which is interesting because you're on my slack. So you could just ask it that, hey, how much, what's Naman's personal bank statements looking like?

**Naman Pandey** (01:11:54)

And it will probably respond to you. So yeah, no good, right? We definitely do not want that. Inbuilt application firewall is completely turned off. I think that's literally a no-brainer to switch it on. Again, we can keep going this. Like I told you, it came up with the remediation plan. And you can even choose what degree of paranoid you are. So I can literally tell it that I'm extremely paranoid. I don't even want to take the slightest chance of something going rogue. So just change all of your settings to match that. And it will do it. You don't even have to go around... snooping into its stuff for it to figure that out. It will just clear itself, so to speak. Sweet. All right, let's move on to the next use case. Great. So this next use case is something that we've hinted on here and there through our chat.

**Naman Pandey** (01:12:40)

So now in this case, instead of just Slack, we'll be moving away from Slack support channels, I mean, we will have those, but in addition, we'll also have forwarded emails. We'll have intercom transcripts if you need. We can even have Google reviews, Reddit threads, whatever you need can all be thrown into this together. And what the goal here, especially if you have a product that is fairly new, it's very, you're trying to iterate really quickly. What you can do is that it generates a voice of the customer report posted to Slack. So then PMs can mention the bot to drill into any theme as well, right? Tell me more about the authentication-related complaints this week. Maybe because on your stand-up, somebody reported an unrelated issue related to authentication. So now you're wondering, could something have broken that we just don't know? Well, the easiest way is to just poll what your customers are saying, right?

**Naman Pandey** (01:13:33)

Why should PM scare? Because this is the PM dream. a living queryable customer feedback system that doesn't require an analytics platform the bot maintains persistent memory so it tracks trends over weeks which is something that i was mentioning before and it can also tell you authentication complaints increased 40 compared to last week and again this is extendable to quarter year you know even probably five year time things so The persistent memory is the key aspect to this. And as we were talking about it, we have a memory file, a markdown file right here, which it makes sense to flash, which right now just has this. But, um, sorry, wait, I think for the persistent memory, okay, it is memory.mdcrate. It's always helpful to check. So when we are done building out this use case, you will see this file, this memory markdown file automatically updated with our particular use case.

**Naman Pandey** (01:14:26)

So similar to last time, I already, I think I have the prompt ready. Oh, I do not have it ready. Great. We can just quickly write it here. And then the way I wanted to demo this was, Atash, you can just email me pretending to be a customer on my email, which I can attach, which I can just send to you. So just like, you know, feel free to send an email saying that just, you know, any issue, just be like, I hate your software or like I hate your... Yeah, just be like RSS feed onboarding did not work for me. This product sucks or whatever, right? Because most products have their support email that usually some sad person has to monitor. Not to the fullest extent, but it can happen where it's getting filled up real quickly by just complaints from people all over the world.

**Naman Pandey** (01:15:16)

So... We will just be demoing the email aspect here, right? But we can extend this for it to poll Google reviews, Product Hunt, literally Twitter, whatever you need to be polled, you will just make a list, which I will do now as you email that to me. And we will set that up here. So again, I'm trying to show you like the art of the possible here. So I'm literally just going to like paste the entire prompt itself directly in here. I want for it to struggle. I don't know if that it will. We just have to be careful about what channels we're mentioning. So I know we have competitive Intel. So we'll just say that. Otherwise, they just have to add it again, which is just, you know, kind of annoying. And we already know how to do that. So we'll just remove that. Maybe what we can do is have conflicting feedback.

**Naman Pandey** (01:16:07)

So maybe you email me saying RSS is bad. We can say RSS is good. So, you know, so just to see what it actually does. The rest of the prompt just kind of tells it what it needs to do. So it creates a heartbeat, which is, you know, every six hours scan these things. We will update those channels one more time. just to make sure that they're not lost for new messages. And then I'll add and my email inbox that you have access to. Quick note on that, if you don't want to use Brave API and all of that, that's totally fine. Most Mac users have the Apple Mail app inbuilt on their laptops. If you have that, that is all it needs to access your email. Just by extension, we won't really be covering this. But if you can think of any use cases that involve email, it can do it, right?

**Naman Pandey** (01:16:58)

Because think of the two things that it has. One, access to your email. Two, ability to do things. So say somebody sends you an email where they want to schedule a podcast recording with you. You just go on your Slack. You just be like, check my emails for any new requests. If there are any, schedule them using my Google Calendar, which again, it does have access to that as well. So it just does everything for you while you're just like watching TV or something. Again, we will not be covering that, but just wanted to call that out. Any and all use cases involving emails are just solved now across the board. So yeah, and then the rest of it is categorized each by area and severity. Update the running tally, all of this, you know, good stuff. And we have it set up every 30 minutes by default, keeps the data fresh.

**Naman Pandey** (01:17:43)

And the weekly cron produces this synthesis of all of these 30 emails. 30 minute increments so really this is two ongoing cron jobs bundled into one right so the mini version is every 30 minutes and then every week it gives you the summary of those 30 minutes because obviously if you you know you don't want to be reading it every 30 minutes unless you really have to as usual we just hit send sit back have a sip of your coffee go on a walk while it just builds itself which I'm hoping by now you're beginning to really appreciate that pattern Well, that is the biggest unlock here where you don't do any of the setup. It does the setup. It sets itself up.

**Aakash Gupta** (01:18:26)

One of the things that I like to do with Claude and Claude code is have like five, six chats going at once so that I don't have to wait ever. Can you do that? You can.

**Naman Pandey** (01:18:35)

What you need to be wary of is all of these activities, right? So when it thinks that, okay, I need to access browser or finder in this case, then I need to click and open this file. Then I need to dump all of this text into this file, which they're not going to come up from thin air. I need to write them. So it depends on how context heavy your ask is. If you're doing a lot of polling type stuff, 100% you can, you know, really just go all in on it. Where I found its struggle was just yesterday. I was fine. I just gave it the command on WhatsApp that, hey, find five people on LinkedIn like me that you think I will be friends with and auto reach out to them for me. On my phone is what I told it. And then I saw it open the browser.

**Naman Pandey** (01:19:20)

I saw it do its searching. I saw it find a profile, which, you know, it's probably a conversation for another time who that was. I saw it click the message button, like when, you know, you're sending a new message. And that's when it gave me the API rate limit. But that makes sense because if you think about it, just to get to that stage, It's such a compute-heavy operation. Like my human brain would need 10 minutes to even figure out a plan on how to solve this weird problem. I don't know who's like me. You know, it's like, I don't know how to solve that. So that's the only thing to keep in mind with this, that if it's not super heavy, you can definitely concurrently run stuff as you can see apparently it's just done um it just did everything we asked it to we should see a custom skill let's actually inspect that so we go here it says it should be inside voc taxonomy voc maybe we refresh this or maybe made it some memory i see a memory here that does not look right so here's what we'll do right since we can't find it i will literally just copy this and i'll say open I don't know why that's copied.

**Naman Pandey** (01:20:34)

I'll just like have it open it for me, right? Because why am I finding stuff in my finder on my computer? And hopefully it does that. We'll see here. Okay. There you go. So now if I right click, do that. Great. This is pretty much what we had asked it to do.

**Aakash Gupta** (01:20:57)

So it's really excelling in computer use compared to your average AI. Exactly.

**Naman Pandey** (01:21:02)

Yeah, like there is a version of this where you're like actually completely hands-free. That made me think of another really cool use case. It's like a mini use case, but I'll show that here. We'll take a pause from this real quick, right? So we were talking about all of this, right? We even had this database schema. So you can actually have it draw the entire schema diagram on your browser so the way to do that is we'll say earlier you talked about a schema diagram i want you to draw it on my browser so that i can edit it you can use mermaid

**Aakash Gupta** (01:21:35)

and we probably

**Naman Pandey** (01:21:35)

need it at open claw right exactly yep so when i so i accidentally stumbled across this i actually didn't even know it could do that what should happen and i really hope it it happens here as well because i don't know if it will for shark But it'll open like that entire drawing like a mirror almost. And you're probably familiar with Mermaid, but maybe some of your audience. Okay. Wow. Like it just drew all that. And obviously to edit, I just need to change that. I can then export it. I can probably have it exported for all I know. Right. So again, constant theme here. go hands-free if there's a thing that you can imagine yourself doing on your browser and your file system or any combination of the two don't do that anymore just speak into your you know OpenClaw bot and it'll do it for you so coming back to our little use case here did you send me that email yet for the feedback

**Aakash Gupta** (01:22:38)

yes

**Naman Pandey** (01:22:38)

perfect

**Aakash Gupta** (01:22:39)

I sent you both the conflicting emails okay

**Naman Pandey** (01:22:42)

Yeah, exactly. So if we combined feedback from the Slack channel as well as email, you can see that it said competitive Intel failed, but that's just because we didn't give it the ID, which we know how to do. What's more important is that it identified this correctly on the customer support channel, which I believe what had we sent? Okay, that you needed more customization. Perfect. So it included that. Um, In your email, I believe, I'm not sure what you sent me, but it said your RSS builder has people somehow both complaining and raving about it.

**Aakash Gupta** (01:23:14)

Yes, that's right. I tried to confuse it. So I sent from two different emails, your RSS is great. Your RSS sucks.

**Naman Pandey** (01:23:23)

So interesting. I mean, at least it's accurate. But so, yeah, even though it says status failed, we know that it's not, you know, anything to worry about because all we have to do is give it the right channel ID. So that concludes use case four. We can jump to the final one here, if that's okay, Akash. Let's do it. Perfect. So for our final use case, something we haven't done so far, which is really critical with anything useful, quote unquote, that you're doing is decision making, right? Like you don't just want it to be a monitor, which we've covered or do something if something happens, which we've covered. What we've not done is for it to make decisions for itself based on what it's seeing and then doing different things based on what it sees. So what we're going to do is that we will supply it with a user CSV, if you will, right?

**Naman Pandey** (01:24:18)

So any product has paid as well as free users. So what we will do is we'll try to mimic how it adjusts to bugs reported by an enterprise user versus a free tier user. And we'll have it do different things based on checking the data and the identity of the user that submitted the bug so what that will look like is just in the interest of time i like saved the prompt already and i mean this is what that looks like right great so this is our little use case that i just scribbled in like my notes app but what we'll have it do is that we'll ask it to build an automation when somebody posts a bug report in a slack channel i want you to read the message and extract the reporter's name Check if the name appears in the customer list or CSV file in your workspace.

**Naman Pandey** (01:25:05)

So this can be just a CSV, which literally can be as long as you want. The way this is configured is Sarah Chen is an enterprise user. James here is pro. Lisa is just a free personal user, right? So most production apps or products have a similar segregation. Somewhere in their, you know, repository, they have a way to figure out which user is what. And because not all users are the same, right? So if they're not a paying customer, it will post it to a different channel. If it is a paying customer, escalate to engineering urgent with the full bug details and flag it as high priority. And then finally, it even replies in a thread on the original message, acknowledging the bug and giving an estimated response time. And finally, if all of this was not enough, it appends the bug to a tracking log in bugs.csv with the date reported severity and which channel it was routed to.

**Naman Pandey** (01:25:57)

So a few quick things here before we jump to building this. All of these CSV files can be B, your online, if your company uses Jira, it can be that. It can be Asana, which can be pretty much whatever API that you're working with in your organization. In this case, because this is not an actual production thing, I just stuck with a CSV. But my goal here is to demo that it doesn't end at a CSV, right? It can append a CSV, obviously, duh. But in addition, it can also make those live changes on wherever your company's work, you know, workstation lives and breathes. So I guess before we go about actually building this, Akash, is this looking like a decent kind of use case that might maybe surprises you? I'm just kind of curious to get your thoughts on what you make of this.

**Aakash Gupta** (01:26:47)

Love it.

**Naman Pandey** (01:26:48)

So as usual, right, we just need to imagine. So the prompt that I just showed will simply go to our gateway, the UI gateway, and we will simply paste it over there. So let me quickly bring that up. So interestingly, it gave me the API rate limit for that.

**Aakash Gupta** (01:27:11)

Hmm.

**Naman Pandey** (01:27:12)

Usually when this has happened in the past, you have like there's two major options. You can either change the model that you're talking to or sometimes if you just wait, that does it as well. I think we'll maybe just change. Okay, so apparently that was just a lie because it looks like it's doing that now. um the problem here is we will need to create these channels so let me quickly just edit this for us to just use the channels that we have so give me one second while i do that okay cool looks like it's fully set up great so we can now pretty easily test it right so to test it what we can do is go on here interesting i i didn't know you tried this so you know it's so funny I think it's because of what we talked about in terms of remember it's soul.md said to not share private details on the internet we can obviously double down and ask it why it said this but this is really cool actually I didn't actually think it would be smart enough to not do this but for now I will just say that your landing page won't let me log in And I think here we have to tag it, Akash, or it doesn't work.

**Naman Pandey** (01:28:29)

So we'll say your landing page, and that's a good reminder for me as well. And we'll say one of our users who was an enterprise user, so Sarah Chen. So normally this would be her account, but I'll just say a hyphen and say Sarah Chen just so that it knows that, you know, I'm an enterprise user. Maybe you can post... Actually, where did we ask it to check? We asked it to check engineering urgent. Do we have that? No, we said and design. Yeah, Akash, maybe. Well, damn, I guess that's we'll just let it be. And for design, we'll just say there are resizing issue. And we can have this be said by Lisa Park, who was a free user so that she should be routed somewhere else. and we actually don't even have to tag openglo for this so we'll do that once this is here we'll say run the run this automation above with we'll just say run that above and i think that that's usually enough okay rate limit no worries just need it to run this one last time Yeah, it's funny how it's just like a fake rate limit issue.

**Naman Pandey** (01:29:48)

Oh no, that was not fake. Oh, just refresh. Come on. We're so close. We are so close. We'll just change the model, I guess. That's straightforward enough. So it did work. But the problem is this. It says it's clear the user is impatient or their interface is lagging. So, yeah. Yeah, I really should have just waited, but... Okay. I'm now hunting for the channel ID. Okay. But are you too great? I guess we'll just say, what's going on now? We beat the rate limit stuff though, so that's at least... Yeah. That's on the brighter side. Okay. So it looks like it did a bunch... Okay. So let's just now try rerunning this and see what happens. We have to tag it. While it does that, I'm trying to run the, okay, I'm shooting a snag. Okay, as usual, it's the channel names that throw it. Reading messages?

**Naman Pandey** (01:30:57)

Okay. Bug reports, it doesn't have. Oh, interesting. So it did work. Look. So I just mimicked Sarah Chen, who, as we know, is an enterprise user. So she just submitted a bug. Let's assume this is our public-facing bug reporting channel, or maybe she's a tester or whatever. What matters here is that you can... distill users into various privilege levels really is what the takeaway here and based on some of their privileges that come from a different file a CSV file that lives on your file system or it can live on your workstation like Asana or whatever tool your company uses It automatically flagged it. So high priority issue detected. Reporter is Sarah Chen. She's an enterprise user, Acme Corp. That's her issue. Escalated to engineering immediately. This is a critical blocker for a paying customer. It did it twice because I ran it twice and it finally caught up to that.

**Naman Pandey** (01:31:51)

I am curious though in terms of where it escalated it. Customer's code? um so lisa park according to our csv is a she is just a free personal user nothing should not be flagged as a high priority issue but we shall see okay so we got a reply from our bot okay bug report you know free tier everything's we're pretty much just chilling it was routed to design for review low priority So if you go and design, in my prompt, I had asked it to generate the bug report in this channel. So as you can see, it even picked this. I don't know who asked it to do that. But it's a UI resizing issue reported by Lisa Park, who is a free new year personal user, which, as you know, we did not tell it that. That came from the CSV. So it looked at the CSV, filtered according to the direction branch that we asked it to, mentioned the issue and the status.

**Naman Pandey** (01:32:49)

So the real way this works in the real world, as I'm sure some of you are already guessing, is with GitHub, right? GitHub is where all your customers are going to report bugs, issues, whatever have you. This exact same scenario can play out with GitHub connected directly into OpenClaw. And so I just described what I wanted in plain English and throughout all of these, you know... Use cases, as we saw, this is really just you prompting things into existence. Buy the thing that does the thing into existence as well, if that makes sense. So that was all I had in terms of my use cases. I hope some of this hopefully was helpful for some of you. I'll pass it back to Akash for his thoughts and any questions.

**Aakash Gupta** (01:33:36)

So we just went over five use cases. This one was basically a self-building agent, right? Without all the node workflows that you would be creating in Zapier or Lindy. So pretty powerful. What are the other use cases people should be thinking about to stretch their abilities after they implement these five? What should they go do next?

**Naman Pandey** (01:33:53)

I would say building in media or baking in media-based usages for me is the next frontier. A lot of my time is spent, you know, drawing designs, making those mouse-type movements or even just on Canva for sometimes, right? You need it sometimes to just make process maps and all of that. For me, the next unlock here is anytime you're trying to do a map or a map-based visual of any sort, For me, maybe I'm just a dummy, but it takes me hours to first visualize it and then actually draw a bunch of boxes and such to bring together the map for a particularly more complex process. So I would suggest think about more media-based use cases, be it pictures. you know, videos aren't even that far. From this point, you can have it configured to generate automatic, you know, VO videos or AI videos based off something, right, which you can configure.

**Naman Pandey** (01:34:50)

So I would really encourage your listeners to start thinking about it the next stage here in terms of more multimedia-based operations.

**Aakash Gupta** (01:34:58)

So you've spent hours using OpenClaw. Most people don't have that time. What are the biggest mistakes, configuration challenges, things you had to debug that people can learn from? I

**Naman Pandey** (01:35:08)

would say by far the biggest one was just worrying about the security piece of it all, which, you know, we did cover. The best thing here, somehow, you know, the best and the worst thing at the same time is that while it is really easy to go berserk, break a bunch of things that you were not trying to break, really what this boils down to, be it setup of a new tool, right, or be it like a security thing. Whatever it is that you're trying to do, when in doubt, just ask your bot, right? Remember, it is the first of many that you will make. What I'm working on next is something that I described, right? I want to have an entire family of agents that are all controlled by Fela, who is like my main major agent here. So I'm going to have Fela report just things that I need to know of the various like 16 different bots that are doing underneath it.

**Naman Pandey** (01:36:00)

It's kind of like a CEO type model, right? I don't need to know all the details of everything that's going on. So that is my biggest thing. That is what I'm really excited about and what I would encourage people to do. Again, when in doubt, just ask the question, right? Your friendly UI gateway here. That's not it, but that one. is here for you to not just gain any insight into how it works, what it does, why it does it, but also anything you want it to do. You can even lock yourself out from making any dummy mistakes by giving it a system command as soon as you set up that, hey, whatever we're going to do, Flag me and stop me when I do say one, two, three, four, right? Whatever you're worried about, no two people are the same. Draw that line in the sand nice and early and you can rest assured that it will not fail you.

**Naman Pandey** (01:36:47)

At least in my experience, it has not.

**Aakash Gupta** (01:36:49)

So OpenClaw, ClaudeCowork, ClaudeCode, those are the three hot new AI tools. How would you compare and contrast them?

**Naman Pandey** (01:36:56)

Okay, so right off the bat, I think there is an imposter in those three tools that you mentioned, with it obviously just being clawed. So clawed, while really powerful for about, I want to say, 98% of the population, you know, we already are pretty familiar with what it can do and cannot. Lives on the browser is completely reactive in that you have to... invoke it for whatever you're trying to do. It lives on the browser, cannot really do anything. I think that's the biggest distinction here. So yeah, I guess, again, without beating a dead horse too much, that's just Claude. Really, the conversation gets much more interesting when we contrast co-work with OpenClop. That's when some of the lines start to blur a little bit more. For me, rather than trying to go through the similarities, which there are a lot of, I think it makes more sense for me to go through what's the biggest difference here, which is that in the case of OpenClaw, we have a continual daemon, D-A-E-M-O-N, that just lives and runs consistently on your machine.

**Naman Pandey** (01:38:02)

Unlike Clawed Cowork, which is still to a large extent reactive, right? You still have to point it to stuff. You have to set it, give it skills, make sure that it's still trying to do what you want it to do. For me, the biggest differentiator between the two is the idea of consciousness. Open Claw almost has, you can even imagine it like a version of you that lives in your computer, actually, that jumps through your RAM and such, has access to your file systems. It never sleeps. It's able to do things on its own, using its own consciousness, based on things that it inferred from what you told it, not always directly what you told it, which is, again, where we start to get a little philosophical. But there is nothing co-work does that is actually autonomous, right? It cannot make decisions by itself based on an idea that it has about you.

**Naman Pandey** (01:38:54)

Open Claw can, which, as you can imagine, make it really interesting, but somewhat exciting and dangerous at the same time. Happy to drill into any of what I mentioned. Did that make sense?

**Aakash Gupta** (01:39:04)

Yep. Perfect. All right. Cool. All right. You had a Google Doc you wanted to show people, right? Yeah.

**Naman Pandey** (01:39:11)

Yeah, I can't find it because it was on X and I tried finding it for a while, which so it didn't, I wasn't able to find it, but I'm sure it'll turn up at which point can I just send that to you? Would that work? I'll do it. Whatever

**Aakash Gupta** (01:39:22)

is

**Naman Pandey** (01:39:24)

good for you.

**Aakash Gupta** (01:39:24)

Cool. Yeah. So let's just end the podcast then. Naman, this was awesome. If people want to learn more, where can they find you?

**Naman Pandey** (01:39:32)

My YouTube channel, Naman Pandey, has me just constantly breaking stuff, operating on the cutting edge of all of these tools. I already have the next three tools apparently now that OpenClaw is old. So feel free to check out my videos. Feel free to say hi on LinkedIn. Always love to engage with fellow builders such as you all.

<!-- sponsor -->
**Aakash Gupta** (01:39:52)

Amazing. Thanks so much, Naman. We'll have to have you back soon. Bye, everyone. I hope you enjoyed that episode. If you could take a moment to double check that you have followed on Apple and Spotify podcasts, subscribed on YouTube, left a rating, a review on Apple or Spotify and commented on YouTube. All these things will help the algorithm distribute the show to more and more people. As we distribute the show to more people, we can grow the show, improve the quality of the content and the production to get you better insights to stay ahead in your career. Finally, do check out my bundle at bundle.akushg.com to get access to nine AI products for an entire year for free. This includes Dovetail, Mobbin, Linear, Reforge Build, Descript, and many other amazing tools that will help you as an AI product manager or builder succeed. I'll see you in the next episode.
