---
title: "Claude Code for Non-Technical PMs, with Andre Albuquerque"
subtitle: "A step-by-step guide from tools like Lovable to multi-agent systems in Claude Code for the non-technical"
date: "2026-05-18"
host: "Aakash Gupta"
guests: ["Andre Albuquerque"]
speaker_names: "substack"
substack_url: "https://www.news.aakashg.com/p/claude-code-non-technical-pms"
youtube_url: "https://www.youtube.com/watch?v=bYiXxeinhbg"
duration: "01:09:37"
word_count: 12654
source: "Substack episode transcript (aired audio)"
sponsors:
  - name: "Customer.io"
    url: "http://customer.io/productgrowth"
  - name: "Bolt"
    url: "https://bolt.new/solutions/product-manager?utm_source=Promoted&utm_medium=email&utm_campaign=aakash-product-growth"
  - name: "Ariso"
    url: "https://ariso.ai/aakash"
  - name: "AI PM Certification"
    url: "https://maven.com/product-faculty/ai-product-management-certification?promoCode=AAKASH550C7"
---

**Sponsors:** This episode is brought to you by [Customer.io](http://customer.io/productgrowth), [Bolt](https://bolt.new/solutions/product-manager?utm_source=Promoted&utm_medium=email&utm_campaign=aakash-product-growth), [Ariso](https://ariso.ai/aakash) and [AI PM Certification](https://maven.com/product-faculty/ai-product-management-certification?promoCode=AAKASH550C7).

# Claude Code for Non-Technical PMs, with Andre Albuquerque

*A step-by-step guide from tools like Lovable to multi-agent systems in Claude Code for the non-technical*

**Andre Albuquerque** (00:00:00)

If you look at a lot of companies that have non-technical PMs in teams, they're bureaucrats. They're stuck in Jira, Linear, PowerPoints. They're dependent on their technical teams. Andre Albuquerque,

**Aakash Gupta** (00:00:10)

he runs Europe's largest product builder school with over 4,000 students. and in today's episode, he is giving you everything for free.

**Andre Albuquerque** (00:00:18)

The product owner culture in Europe, it focuses a lot on a bit of a glorified delivery manager without the actual technical skills.

**Aakash Gupta** (00:00:25)

What's the flip side to this philosophy though? And you even have the word slob here. How do you avoid shipping slop? The

**Andre Albuquerque** (00:00:31)

biggest fear a lot of people have is like, oh, five coded,

**Aakash Gupta** (00:00:34)

bad code. Transformation is a big goal. Can you go ahead and show people how they get started with this new way of working?

**Andre Albuquerque** (00:00:41)

It has four steps. The first one, lovable. The second step, a mix of lovable and plot codes. The third step is plot code and versell. And the fourth step is multi-clot code, multi-versell, and a lot of automation and agents.

<!-- sponsor -->
**Aakash Gupta** (00:00:53)

One of the things you wrote about on LinkedIn is that there are now only four jobs. Can you explain this? Before we go any further, do me a favor and check that you are subscribed on YouTube and following on Apple and Spotify podcasts. And if you want to get access to amazing AI tools, check out my bundle, where if you become an annual subscriber to my newsletter, you get a full year free of the paid plans of Mobbin, Arise, RelayApp, Dovetail, Linear, Magic Patterns, Deep Sky, Reforge Build, Descript, and Speechify. So be sure to check that out at bundle.akashg.com. And now into today's episode. If you're like me, you're getting overwhelmed by all of the AI tools, all the AI noise out there, and 90% of the guides assume that you are technical and you're an expert in cloud code. Today's episode is nothing like that.

<!-- sponsor -->
**Aakash Gupta** (00:01:47)

We are going to show you very step by step how you can start with lovable and AI prototyping, how you can layer in cloud code to your lovable workflow, then how you can move to full cloud code, and finally how you can use Cloud Code with tools like Vercel and Cursor to actually ship updates to your code base. There is not an episode like this on YouTube and I think I brought in the best person to do it. Andre Albuquerque really excels in giving you simple understandings, building up your knowledge from zero. So if you're a non-technical PM and you watch till the end, I guarantee you will feel more confident using Cloud Code and we will even give you the Monday morning roadmap to go talk to your engineer. So let's get into it. Andre, welcome to the podcast.

**Andre Albuquerque** (00:02:28)

Hi Akash, thank

**Aakash Gupta** (00:02:29)

you very much for having me. So I want to address the non-technical PMs from the get-go and give them something they can use. What is the biggest problem non-technical PMs face in their roles?

**Andre Albuquerque** (00:02:39)

If you look at a lot of companies that have non-technical PMs in teams, they're bureaucrats. They're stuck in JIRA. They're stuck in Linear. They're stuck in PowerPoints. They're not actually building. They're not pushing code. They're not adding features. They're dependent on their technical teams to do that. And it's not like they don't want to. It's a combination of their not knowing how, maybe the management culture doesn't allow them, maybe they don't have the skills and the tools to be able to do it, but they're basically, they're waiting independent on everyone. And when we look to a lot of A, You see product managers, technical or not, actually contributing, building stuff. You see CEOs contributing to repositories in GitHub. You look at the Shopify CEO and his GitHub is fully green You see entire teams that are maybe, it used to be like 10, 20 people and now they're super small teams and they're all actually pushing new features, new codes to production and I think This is the reality that if you're a non-technical PM And your job is still managing backlogs Your job is still writing issues Your job is still creating decks or PowerPoints to present to someone And you're not really building stuff Honestly, you're being left behind And I think you want to completely transform the way you see your role inside a team, which then will influence everyone else in the team to rethink their own roles and transform the squads entirely.

**Aakash Gupta** (00:04:16)

So transformation is a big goal. I don't know if we'll be able to Deliver everything on transformation but can you go ahead and share your screen show people how they get started with this new way of working

**Andre Albuquerque** (00:04:26)

yeah so what I'm going to show you just to give you context is how I actually went from I'm not a developer I don't know how to code and I started building now this has multiple steps right and this is the format that worked for me doesn't mean it's going to work for everyone but it gave me a bit of comfort and I'll explain So it has basically four steps, right? The first one, and I'm going to address different tools. Again, you might be more of a fan of a specific stack or a specific tool. I went through all of them and I'll explain why these were the specific steps. So the four levels were first with lovable and I'll explain why lovable. The second step was a mix of lovable and cloud code. The third step is cloud code and Vercel as the infrastructure. And the fourth step is like multi cloud codes, multi Vercel and a lot of automation and agents.

**Andre Albuquerque** (00:05:24)

All right. So that's how it works. So I'm going to show you and kind of explain what happens with each one. So let's start with Lovable. First of all, why did I start with Lovable? Because honestly, it's way less scary than just jumping straight into an IDE or jumping straight into a code environment. The team at Lovable, first, they're European. So of course, I'm going to be a big fan of what they're doing. And second, they built a really easy Product for anyone who has never coded who potentially is a bit afraid to just start doing right this is step number one so you and you can build like really simple tools and my recommendation is you start with something personal you don't start with something on your professional environment because that allows you to actually explore the tool for example I build so my family has a summer vacation home right and we are quite a lot of people and and we needed a way to manage who has the house in certain periods of the year, who's going to be there, is the house fully booked or not.

**Andre Albuquerque** (00:06:31)

And this is not commercial, like this is for the family, right? So I started actually building my first product on Lovable was this simple tool to manage the availability of people. Now, this is actually a great way to start because again, there's no risk like you're not contributing to the company's repository you don't even need access because this is just for you and you can do mistakes the code base it doesn't need to be beautiful because who cares at this level like it's fine so you start building on Lovable and the beauty about Lovable Aakashgupta Like you don't even know that is something important. So with Lovable as a step one, it actually doesn't matter. So it's a great way to get started. So this is my start. And by the way, the app, whether it's an app or landing page, it can be as complex or as simple as you want.

**Andre Albuquerque** (00:07:40)

Doesn't matter. You can play with it. You can start gaining a bit of feedback on how you're building. Like one really cool way is ask, always asking your prompt if you you're missing out on something if you're not questioning or asking or prompting something you should and you'll always get the feedback back like you're working with a senior engineer which for now AI is a senior engineer to you and they'll also give you feedback and it's actually a great So that is step number one. Then step number two, which is actually an accidental evolution, but it worked really well for me, which was I wanted to be able to do more, right? And Lovable, at least back when I was using Lovable, was still a bit limited on a few things. So I installed Cloud Code, right? And I installed Cloud Code on the Cloud desktop app.

**Andre Albuquerque** (00:08:30)

So you start working with Cloud Code on the desktop app. Actually, I'm going to switch screens to the desktop app. All right. So you should be seeing Cloud Code desktop app, right? And you land here and let's be honest, it's... it's a bit scary you land here and it's a bit scary like you don't know what this is you're not seeing a product you just came from lovable where you saw the product in front of you you had a chat you had feedback you don't even know what to do here right okay so what I did was I knew I had to get my code somewhere. That somewhere typically is some repository. So you start an account on GitHub. That's the first thing, super easy. And you connect your cloud code to your GitHub. So when you connect your cloud code to your GitHub, they're linked.

**Andre Albuquerque** (00:09:16)

You can also connect your lovable to the same cloud code and GitHub repository. So they're all synced. That means that if you actually do code on the cloud code desktop app and you update your repository on GitHub, Lovable will also get that update, right? And the good thing about this is that even though you don't have a visual understanding or at least easily a visual way of seeing your product evolving, you can actually use Lovable as your infrastructure. What that means is that you can be pushing codes on Cloud Code with all the flexibility on all the great things that Cloud Code offers, but you can still see the evolution of your product on Lovable with all the easiness of the Lovable platform. And I think this is actually a great transition because you're not fully getting out of it. You don't have to deal with hosting and infrastructure and you don't need to think about deployments because look, let's say that I am contributing to my Lovable project, right?

**Andre Albuquerque** (00:10:17)

I used to think I had a retention

<!-- sponsor -->
**Aakash Gupta** (00:10:19)

problem Turns out I had a messaging problem I was sending the same onboarding emails to every new user whether they activated on day one or never logged in again I had no idea who was slipping or why Customer.io changed that Every message I send is now based on what users actually do in the product Someone hits a key activation They also have an MCP server, which means AI tools like Claude can see directly what's happening in your customer.io workspace. Your segments, your customer data, your attribution, all of it. So instead of explaining your business context every time you need help, Claude already knows it. Notion used customer.io to personalize their onboarding and hit nearly 50% open rate. Improved conversion The idea is simple. Customer.io helps you deliver more impact from every message you send. If you're a PM or founder and your onboarding is still one-size-fits-all, try Today's episode is brought to you by Amplitude.

<!-- sponsor -->
**Aakash Gupta** (00:11:34)

Replays of mobile user engagement are critical to building better products and experiences. But many session replay tools don't capture the full picture. Some tools take screenshots every second. leading to choppy replays and high storage costs from enormous capture sizes. Others use wireframes, but key moments go missing, creating gaps in your understanding. Neither approach gives you a truly mobile experience. Amplitude does things differently. Their mobile replays capture the full experience. Every tap, every scroll and every gesture with no lag and no performance hit. It's the most accurate way to understand mobile behavior. See the full story with amplitude.

**Andre Albuquerque** (00:12:11)

Unlovable, let's say this is a project that I've used in that transition period. So I was building a platform, right and this platform was for my school builders camp in the beginning and I was already using cloud code because I wanted to understand the tool I wanted all the capabilities but I didn't want to completely leave lovable because it was super comfortable like I had my chat here I could see and ask questions anyway but what do you see here on the chat on the left side is merges right what that means is that I'm actually using cloud code to work I'm merging meaning I'm sending the code to GitHub And GitHub is telling Lovable, look, there was an evolution on the product and it changes here. So the beauty about this is that I can actually test the product, do my QA, my quality assurance, directly on Lovable.

**Andre Albuquerque** (00:12:59)

And as I'm using Lovable as my infrastructure, the deployment, meaning putting stuff live for people in the actual URL, comes from Lovable. I don't need to deal with all the more technical infrastructure like Vercel and I'm going to go there next because Lovable takes care of that. So it's an accidental jobs to be done way of using Lovable that I don't think they intended but it worked really well and it's a great bridge.

**Aakash Gupta** (00:13:24)

I haven't seen anybody talk about this. So this is new alpha. This is really exciting information for people. If somebody is just, they need that extra step of you showing them, can you just show us exactly how to connect Lovable and Claude desktop app to the right GitHub repo that's the same one?

**Andre Albuquerque** (00:13:43)

yeah so let me so I need to do some some setup so very quickly let's say let's see if I can use one that I already have because yeah I agree it's it's something different right so let's see if I can do this yeah so what we can do is let's actually build a small tool or a small product right now I think that's that's the step okay but let's also do this one recommendation is that you need to you have your repository okay let's say that you have your github and it's under your name even my my personal one is under my name so it's here and this is where I'm gonna basically keep all the repositories that are connected lovable because again What we're saying is this is for your personal usage or even for your business, not for the company. If it's for your company, the setup is different because your engineering team is going to have their own repository.

**Andre Albuquerque** (00:14:42)

They need to give you access, but we'll go to that a bit later. So let's say you have, these are projects that I have for myself. So let's say that I want to build a new product. Let's say, so I'm going to go to Lovable and I say, I want to build a mentorship project. So I'm going to say a mentorship matching tool Make it simple So I'm going to build So what this does is I'm actually bootstrapping the tool on Lovable Which is way easier to start than starting on Cloud Code If you don't have the infrastructure yet built So let's assume you don't So you start on Lovable, you say, I want to build something. So you explain and then throughout the episode, I'm also going to show you how this gets significantly more advanced without actually you having to know a lot more than what I just did here.

**Andre Albuquerque** (00:15:34)

Level right now is going through its setup so while it's working it's important you need to have your repository here and then what you also need to have is your repository connected to Level but I'll show you how you do this so now it's I asked it to be simple so it doesn't take a long time but it still might take a few seconds in so We want to make sure that, just to recap the flow, is you have your GitHub repository, you're starting on Lovable, but you also have a Cloud Code account. Now you can use, I think you need maybe a pro account to be able to use Cloud Code, not fully sure if the free account allows you to do this, but let's say you're on the lowest plan, which is more than enough to start playing with this, you have your Cloud Code account.

**Andre Albuquerque** (00:16:18)

What I'm gonna do oh and it's important to know that you also need to have your cloud code connected so your github connected to your cloud code while lovable is building I'm gonna switch the share to my cloud code desktop app So you should be seeing my cloud code and if you go to your connectors and you can see I have a lot of connectors here you need to guarantee your github integration is connected and when you're connecting this mine is already connected you're going to choose your account you're going to log in and authenticate you're going to put your password and it's going to link what that means is that when you go to cloud code so if you see here when you go to cloud code Your repository is going to show here. You'll be able to work on it. Okay. And you can choose your repository.

**Andre Albuquerque** (00:17:05)

So these are my repositories right now. So what I'm going to do is as I'm going to be creating a new repository on this new lovable tool, I'll then open I'll open it up here so I'll add it here okay so let's go back to Lovable let's see if we already have our tool available so it's called mentor match all right so we have something that was built this is what I call the bootstrap so the bootstrap is you start with a prompt however big however simple however complex it doesn't matter you're bootstrapping the product okay now it's here now let's say you want to continue on cloud code because you already okay with working with the tool so what are you gonna do is you want to make sure that you connect this to your okay give me two seconds let's say you connect this to your github okay so you should be able to go to github so get github and you're gonna have your account so I'm gonna connect in this case I have multiple accounts so I'm gonna connect to my personal account so I'll connect What that means is now, the code that Lovable built is gonna go straight to GitHub.

**Andre Albuquerque** (00:18:13)

Now, important thing with Lovable, if you create your code on Cloud Code, send it to GitHub, you won't be able to actually port the code directly to Lovable. It doesn't work that way. You need to start on Lovable, They made a product super simple for that specific use case. All right, so this now created a new repository called MinterMatchSimple. So if I actually go to my GitHub and I refresh it, you now see MinterMatchSimple is here. So now you go to Cloud Code. Remember up until now we bootstrapped the product on Lovable, we connected to GitHub, I showed you the GitHub page and Since your cloud code you connected to your github via the connectors now if you actually are in cloud default and you select the repo you'll see that now mentor match is here okay so now I know I'm coding to mentor match so now Whenever I do things here on cloud code, on the cloud code desktop app, I'm going to do something.

**Andre Albuquerque** (00:19:10)

So let's say I want to change the design system to green. So let's keep it simple, okay? I'm just asking it to change. We started on Lovable, so I'm going to switch to Lovable. And as you can see here, the tool is basically beige and red tones, theme that is more on this palette. And I want to change the setup. I asked Cloud Code to do a bit more green. So what will happen is I'm actually coding into the repository and when I say merge or add to the repository, as Lovable is connected to the repository, it's going to update here. And you'll be able to see, so you'll be able to see, do I like it? Is this the experience or the feature that I wanted? In this case, I'm changing the design system, so I'll be able to actually visually see, is this what I was looking for?

**Andre Albuquerque** (00:20:02)

And if I don't like, I can either do the changes directly here on Lovable, or I can continue working on Cloud Code. In reality, what I'm doing is I'm using Lovable as my infrastructure before I bring this to production, before I actually publish. Keep in mind, this publish button is what puts this live, not the actual cloud code merging into that repository. I'm using Lovable as my infrastructure. And it's, in this case, super simple because I don't need to... I don't need to deal with way more complex stuff. Keep in mind, this is non-technical. So we're trying to simplify life. So I am going to now switch to cloud code to see what is happening there. Okay, so the tool is working and done. It says light theme, replaced orange tones, dark theme. So it basically worked on the background. what we're gonna do is we're gonna ask it to actually merge this so we're telling this I want you to update the product itself like I want you to take the code you just built they're gonna be checking for a pull request creates one so it's doing all the stuff that typically your engineering team is doing that you as a product manager you don't tend to see or care and now you can still not see or care but it's happening anyway so now the pull request was created and merged which means that if I actually go into lovable it's gonna be changing remember the previous palette was beige with red tones so now But we should be seeing something different, right?

**Andre Albuquerque** (00:21:46)

And one thing you'll see is that see here on Lovable where you can actually see switch design system colors. This came from GitHub because you just merged something from cloud code directly. If things worked out, we should do some update and the product should have changed. Again, I don't know what. I'll be able to QA or I'll be able to see it. It depends on what happened with the code. But I asked the design system to change. All right. So it's updating. So you already know that something's happening in the background. And by the way, see, this is what happened. So the design system changed. You didn't work on Lovable, but you're able to QA, you're able to test, you're able to see, I don't like this, I want this to be different. So let's do something else. Let's say I don't like this header. So I'm actually going to take a screenshot and and I just screenshot, I don't know if you can see this on the screen, but I took a screenshot.

**Andre Albuquerque** (00:22:41)

And what I'm gonna do is I'm actually gonna go and paste this on cloud code and say, I really don't like the header. So now I'm gonna share my cloud code. Keep in mind, you're using, This format, which is what I call the bridge, is you're using Loveball as a bit of a QA infrastructure, but you're still using Cloud Code and everything Cloud Code brings to the table. And this will include skills and agents. We'll talk more about that. But you can still, in the transition period, use Loveball as a bit of a way of hosting your infrastructure, dealing with your product, visually testing it, which becomes a big part of your job. So I just pasted the screenshot I took and I say, I don't like this header. Do something Different you can go like you don't even need to specify it you can just say to something different and then you'll see it Changing unlovable and that's also a great way to experiment to try new designs in a really simple way I mean there's other new tools like claw design and whatnot But if you're trying to simplify your life because you're just getting started.

**Andre Albuquerque** (00:23:42)

This is actually a great way so it's running everything so guaranteeing that it understands what you asked understanding the screenshot it's having it's going to all the context of the code and now again the same thing is going to happen it's going to give the implementation you're going to ask it to merge it and then you're going to see the change on the lovable environment so now it's done now it's committing so it's actually already knowing what to do because it adapts to the way you work. And we're just going to ask it, is this merged? Because I want to make sure that this is on GitHub. If it's not on GitHub, you won't see it on Lovable. So I can even ask stuff. By the way, one of the most interesting hacks for non-technical people is The interactions with Cloud Code, they don't need to be just, I need this implemented, implemented.

**Andre Albuquerque** (00:24:33)

It can actually be a conversation that you would have with a chat of Cloud, the same way. Yes, it's consuming tokens, but you can ask questions, you can actually ask Cloud Code to ask you You can ask new questions so that you can improve the requirements, do things differently. I mean, all of that is actually a great way of working. You can see it as interacting with your lead engineer or your engineer on your squad you do the same you can treat it the same way so it's asking me do you want to merge it I say yes so let's actually push this so we see the evolution on lovable so now I'm gonna pass the recording to lovable and you'll see what happens

**Aakash Gupta** (00:25:14)

so for a non-technical pm they might be intimidated by merge and branch and pull request so here's the simplest explanation there is a main branch And what you typically do when you're working on coding something is you'll go out and you'll create your own branch off the main. And once you're happy with it, then you'll submit a pull request and somebody will usually review it and that'll merge that back into the main branch. That's like the basics. I'm oversimplifying it. So what we're doing here is we're kind of skipping the pull request review phase, which is usually what engineers do because we're just vibe coding this on our own really quick and we're just merging it to main.

**Andre Albuquerque** (00:25:56)

Yeah, 100%. Keep in mind, we started with personal projects. The moment you go into your company and your squad, you'll be adapting yourself to the development process and the pipeline, meaning the way the engineering team works together. And you'll be able to integrate that the moment you're comfortable and they're comfortable. And you'll gain a lot more knowledge about everything that you explained. So for now, I mean, you don't need to be afraid of this because you don't even need to know that These terms you can just ask it look I don't know what to do just put this life or just add this to my Code or code base Claude code will actually know what it means so now Let's see if this has landed so we're now back to lovable and you can already see that the redesign hero header which was the feature I just asked is already here so it's already showing automatically I didn't need to do anything and lovable takes a bit of time to update but we already know the code is here so we should be seeing the header change I don't think it changed yet so we'll wait for a few seconds and eventually There is a change in the header okay now we're seeing lovable loading a new experience With the code that we just developed on cloud code and it completely changed everything again.

**Andre Albuquerque** (00:27:14)

I didn't give any specifications. I just said different and it did and It's significantly different And now to finalize this, as I said, even though you push that code, if you're using Lovable as your infrastructure, you still need to publish the app, right? So what happens is you're going to click publish, you're going to click continue, you're going to say, oh, is this a public link or is it just for you? Let's just say that you are either the free or the lowest tier, so you can actually do this. So we'll say, this is public, I want people to be able to access it. And you can just actually say yes, yes, yes to all of this. If you are looking to do a commercial application, then I'd recommend you working on this. Otherwise, you can just continue and boom, your app is going to be live.

**Andre Albuquerque** (00:27:56)

So you just publish this, which means that this URL, people can access it. Now, very important here, when you do changes on cloud code and you push them, they'll update here on Lovable and you need to publish it to update the public link while you don't publish Lovable works like a preview you can see the link so you click on this and you'll see that this opens up a preview link this preview link is your way of QAing outside so doing quality assurance or testing outside the Lovable interface you can actually see how it works on mobile how it works on the browser you can send the preview link to someone so this is a way of using lovable as infrastructure love it

**Aakash Gupta** (00:28:36)

so that's level two level one lovable level two lovable plus cloud code via that github integration that we just walked you through what's level three show us that

**Andre Albuquerque** (00:28:46)

so level three level three for me is i got off lovable right because i wanted to start working faster and typically to work faster you need to have branches so now we're going to get a bit more technical the moment you start playing with repositories and Cloud Code and Lovable, you start, if you're curious, you start understanding a bit more of things. And you don't need to be as technical as your most senior engineer, not even close, but you start learning a bit about branches and you start learning about merging to main and you start learning a bit about work trees. And the moment you start playing with Cloud Code, you'll see yourself very quickly wanting to work with multiple sessions at the same time. What that means is that You're going to start building multiple features at the same time, right? So that means you need to have an infrastructure that allows you to work well safely with multiple branches at the same time, that when you branch you can deal with conflicts.

**Andre Albuquerque** (00:29:43)

that basically you can see stuff in a reliable environment, right? For that, that means I transitioned from Lovable as my infrastructure. And by the way, Lovable isn't supposed to be an infra product. I just use it that way to Vercel, which is way more known as the typical way of working. So what happens is you set up your Vercel product. Right, so I'm going to share my own. So I'll actually share the Builders Camp 1 so you can see how it actually works. And in my case as well, you can then decide one of two things. You can keep on Cloud Code desktop app or you can start using an IDE. Let's say that You like to go into the files themselves. You like to see the code. You want to explore. In my case, I like to use Cursor, but I use Cursor with Cloud Code.

**Andre Albuquerque** (00:30:32)

That means I have the Cloud Code extension inside Cursor, and I'm using Cloud Code basically, not the Cursor agents or anything, but I use Cursor as my ID. I get access to the files, to the code, if I want. I don't need to, but I like it. In my case, personally, and I think this is going to be a bit of a spaces versus tabs in engineering, which is like, in cursor and I can actually show you my cursor, the cloud code. So I'm going to share my screen.

**Aakash Gupta** (00:30:59)

Here's the dirty secret about prototyping. You spend two weeks building a prototype. You validate your assumptions. Engineering loves the direction. Then what happens? You throw the whole thing away. Bolt changes this completely. When you prototype in Bolt, you're not building throwaway mock-up. You're building real front-end I use Bolt every single day, I host my LAN PM job cohort on it, and honestly I'm up till 2am some days just vibing in tool having fun and building that's when you know a product is good when you're using it past midnight not because you need to but because you want to check out bold at bolt.new slash akash that's b-o-l-t dot n-e-w slash a-a-k-a-s-h link in the show notes I hope you're enjoying today's episode. Are you interested in becoming an AI product manager,

**Andre Albuquerque** (00:31:53)

making hundreds of thousands of

**Aakash Gupta** (00:31:54)

dollars more, joining OpenAI and Anthropic? Then you might want to do a course that I've taken myself, the AIPM Certificate, ran by OpenAI Product If you use my code and my link, you get a special discount on this course. It is a course that I highly recommend. We have done a lot of collaborations together on things like AI product strategy. So check out our newsletter articles if you want to see the quality of the type of thinking you'll get. One of my frequent collaborators, Pavel Hearn, is the Build Labs leader. So you're going to live build an AI product with Pavel's feedback if you take this AIPM certificate. So be sure to check that out. Be sure to use my code and my link in order to get a special discount. And now back into today's episode.

**Andre Albuquerque** (00:32:37)

Cloud Code shows as tabs right so you should see so you see all my tabs are up here and actually dive deep into this in a few minutes while in the Cloud Code desktop app so I'm gonna share my screen I don't know why, again I think this is something more personal, I prefer the vertical view So Eurser became comfortable for me, but I think every single person will find their own comfort. All right. And again, I'm not technical. It's not like I can write the code directly into the files. I'm not doing that. But I just find some comfort. And what you'll see is that when you're non-technical working, on some technical stuff you want to find the comfort areas right it's going to make you feel less fear and be more focused on on doing stuff okay so let's go into Vercel so as you can see this is my Vercel environment and now this looks a bit scary if it's the first time you're seeing something like Vercel and on the overview you can see like my product this is BuildersCamp web page so website and on the deployments what you see are all the features that I'm building right these are all features that I've been building in the last hours you can see the hours right so busy day in every single one of these lines what it basically is is a branch and inside a branch you can have a feature change or you can have multiple changes that were maybe bundled into a single branch and What is happening here is that every single one of these is showing you a change in the website that is not yet public.

**Andre Albuquerque** (00:34:22)

What's happening is It's saying, look, you just built this and now you can test it. All right. And the good thing about Vercel is it also gives you a preview link where your changes to the codes are basically here and you can experiment, see how it's working, if it goes in line with your requirements. And then you can say, all right, it's all good. Let's merge this. Let's get this into production, which is let's put this on main. Right?

**Aakash Gupta** (00:34:49)

So if I'm a non-technical PM, I'm a little confused right now. Vercel kind of seems similar to Lovable. Can you just clearly help me in my mind understand? Lovable is X, Claude Code is Y, Vercel is Z. What are these exactly?

**Andre Albuquerque** (00:35:02)

Yeah, so Important to say that I'm using Lovable in the most atypical way possible because Lovable is a AI IDE meaning you build projects on Lovable. That's its goal. Vercel also has that which is called V0 but what I'm what I'm showing you is the infrastructure version and this is I'm oversimplifying on purpose is the infrastructure of Vercel for the applications and the projects so what I'm showing here is basically you have your place where you code let's say it's cloud code and then you have the place where the code lives which is github and then you have Vercel which is your bridge between your github your repository and users right you need to have this connection the bridge and what you're doing is you're pushing the code from cloud code to your repository and then you're telling look Vercel now make the code I just created available to users that's basically it

**Aakash Gupta** (00:36:02)

all right so basically lovable has some of this infrastructure hosting databases built into its product so it's a little bit more easy to use. Now we're uncovering one layer. We're showing you one more layer. Even Vercel is a bunch of abstractions built upon a bunch of stuff. But we're basically showing you how you go from GitHub to users. Exactly.

**Andre Albuquerque** (00:36:24)

Exactly. And by the way, one of the The most important things when you're non-technical is you don't really have the time or ability to really deeply understand every technical aspect. You just want to be pragmatic and just make stuff work. That's what I did with Lovable in my beginning and probably this is what I'm doing with Vercel as well. If I compare my usage with technical folks, it has absolutely nothing to do with that, but it works for me and that's what you're looking for. That is the best skill you can develop right now as a non-technical PM who wants to start building. I'm now going to show you my cursor and how I'm using cursor to develop, which is the next level, which is like, okay, you're using cloud code or you're using cursor with cloud code. So I'm going to switch to... So we keep

**Aakash Gupta** (00:37:09)

layering on the complexity for you guys. We had cloud code desktop app plus Vercel. Now we're doing cloud code inside cursor. Plus for sale and Andre gave you a couple reasons why he likes cursor the vertical visual tabs I would add in like at least two more reasons why you might want to use cursor number one cursor has a very very generous free plan So you can use their agents to debug issues that you have with Cloud Code. Let's say Cloud Code isn't spinning up and you're unable to sign into Cloud Code. You're just stuck at step zero. You open up a cursor agent, which you can do in this top right there. You see this like button up there in the top right. to open up a cursor agent or you can go to the top and hit new agent. And then you can literally paste in whatever issue there.

**Aakash Gupta** (00:38:00)

Andres opened it up. You can paste in whatever issue you're getting like, hey, I'm unable to turn on cloud code or whatever. And the free cursor agent will help you debug any issues. So that's reason why I recommend you guys use cursor. Reason two is what Andre mentioned around GitHub. Cursor is really good at syncing up with GitHub. Once you log into GitHub once, everything, all the projects you open up in Cursor with CloudCode will automatically be linked up to your GitHub. So this is the next level. Start using CloudCode inside Cursor.

**Andre Albuquerque** (00:38:30)

so on this level as you can see what you're seeing here on top are multiple sessions and for me a session is I have an epic let's say you work in product and you work with epics or you can even say there are stories but my sessions are at epic level which means inside an epic there's like multiple features right so when I open up or spin up a new session I'm gonna say look I want to tackle a specific epic I want to work on this let's see how we can implement this and Cloud Code is going to basically do the code for you. You're going to interact with it. I'll show you a couple examples. And the moment that you're ready, you're going to say, let's deploy this or let's merge this or let's open up pull request as Akash explained. And it's going to show up as a branch, as a new line on Vercel that you can test.

**Andre Albuquerque** (00:39:19)

And the moment you're happy, you can just come back to the same session and you can say, all right, everything worked. I QA'd. I saw everything I needed to see. It's working. Let's merge it. You can merge this to main, meaning let's put this on the live branch, the main branch, and users can now access it. So this is like level three, which is you are using cloud code, you're inside the IDE, you're pushing this to a Vercel or an infrastructure, you're being able to run multiple branches. As you can see here, the yellow line is a branch that is outside the purple line, which is your main, the branch that people are using and eventually I merge it meaning they combine which means the features that I worked on the yellow line are now available on the purple one and again the visual part of cursor is is nice for non-technical people because it makes it very simple for you to understand what's happening now you don't need to understand git and how branches work and whatnot you don't need to be very technical there because the visual explains you what's happening right so that's level three The last level or level four is agents and having agents and skills and creating your own process.

**Andre Albuquerque** (00:40:36)

I think that is the last level. It allows you to actually run multiple sessions in parallel working on multiple projects at the same and at the same time being able to actually ship very large epics in parallel without actually creating problems for your product and even experiment on Vercel with different approaches. So I'd say that is the last level that we can get to. All right, agents, how do I build those? Okay, so this fourth level, the agents, the most interesting thing is or actually let's say it like this the biggest fear a lot of people have is like oh vibe coded code is bad code or when you're building with agents or vibe coding they're gonna do like they're gonna create a lot of complexity a lot of lines of code and thinking like this is not wrong like it happens to a lot of people especially when you're non-technical you don't know what you're asking it's very easy with very simple prompts to be creating a lot of slop or a lot of trash that's where a good agent infrastructure can help you so I want to show you And by the way, I want to show you also what I bring to my team.

**Andre Albuquerque** (00:41:39)

So what I did was I built my own repository of agents of skills and even my Claude's MD, which is the memory or the culture, I like to call it the value. This is basically what allows me to work very freely without being super considerate about the rules or about what I need to care about when I'm talking with Cloud Code because I know the agents and the skills in my cloud.md will take care of that for me. So let me dive a bit deeper because this is what I call level four because it frees you time. It gives you time to focus on what you should be focusing, which is, am I solving the right problem? Do I understand the problem well enough? Do I have all the requirements? Have I talked with all the people? If you're spending time on solution design, you're not going to be spending enough time on problem discovery.

**Andre Albuquerque** (00:42:29)

And we all know that the best product managers out there, they spend more time on problem discovery, right? But you need to create your infrastructure. I call it the machine that builds the machine to be able to spend that time there. And this is my machine. So we have Claude.md, which again is your values. I'm going to go deep into mine in a few minutes, but I also have my agents and I have my skills. So let's start with my Claude.md. So as you can see CloudMD is something that exists inside your Cloud code and every time you ask Cloud something on the background you don't see this but on the background they're going to be reading this and that means that all the rules everything you decide to put here they're going to use it to define their own way of working it's like when you're inside a squad a team and you tell them You know that your team is going to be thinking about that as they make decisions or as they work.

**Andre Albuquerque** (00:43:23)

ClaudeMD works exactly the same. So in my case, I have a default behavior, I have rules, so this is how I see it working. I have an agent strategy. I'll explain that in a minute. And I have architecture. I have specific things that happen depending on the feature that I'm asking. So all of these rules are here. I'm happy to make this available on the show notes or to send on the podcast. But basically, this is the memory. These are the rules and these are the values that we carry. Very important, as you're working and you see that you're doing things repetitively or that Claude is doing stuff that you don't like, you can actually improve your Claude MD. You can say to Claude, look, I don't like this or I'm repeating this. Can you please add to Claude MD so that the next time It already knows what to do and how to do it and you don't need to keep getting that error or that issue or something you don't like, right?

**Andre Albuquerque** (00:44:19)

So this is like part number one and you can see this can become super complex. You don't need mine is significantly less complex than Claude I've seen a lot of people but it works well now it works well because of my agents so let me go to the agents because I have a very specific agent that I use a lot and this is called what I call the PM agent so this agent which uses the agent infrastructure of Claude is my product manager. I have a personal product manager inside Claude and it's specifically an orchestrator. Now the PM, which is a PMMD, is not going to be building stuff. You're only going to take information and deciding which other agents to call because they're going to be better at doing something, right? So as you can see, I explained very specifically what the product manager orchestrator is, what they do.

**Andre Albuquerque** (00:45:12)

What exactly am I seeing here? I'm a non-technical PM. I've never used cloud code.

**Aakash Gupta** (00:45:32)

You just showed me ClaudeMD which seemed pretty complex and now you're in the agents folder PM. What exactly are these agents? Who is this? Does this mean that you're going to spin up a new Claude Instance every time this agent is called is this agent going to be proactive? Help me understand what this is.

**Andre Albuquerque** (00:45:49)

Yes. All right, so every time you spend a new session your Claude.md is loaded right and Everything that you have inside that folder the Claude folder which includes your agents and your skills They're also there so they always exist whenever you spin up a new session when you start a new session when you ask something to Claude The one thing that Claude always goes to is the Claude.md, right? It doesn't go anywhere else. It doesn't go to the skills unless you call them. It doesn't go to the agents unless you call them specifically. It goes specifically to Claude.md. Now, on my Claude.md, I have a very important rule. Rule number one, for every task, call the PM agent. So it's like, let's say that you're the CEO. And the first thing you're going to do if you're the CEO is you go to the PM. And you say, I'm the CEO, we found a new opportunity, please work on this new opportunity.

**Andre Albuquerque** (00:46:39)

You're kind of doing the same, but in this case, instead of you having a team, you have agents. So it's going to call the agent, which is a PMMD. And then the PMMD.

**Aakash Gupta** (00:46:50)

Not proactive, but because we've architected our CloudMD in this way that says always call the PM agent. CloudMD is always loaded, so then it goes to the PM agent and then it gets called.

**Andre Albuquerque** (00:47:01)

Exactly, exactly.

**Aakash Gupta** (00:47:03)

And then the PM agent

**Andre Albuquerque** (00:47:04)

is going to decide which other agents are actually going to do the work, right? And we have multiple agents here. As you can see here, you have a researcher which does what user research which typically does in the team we have discovery which is a very specific agent and I'll go a bit deeper here because it's a very interesting one we have a designer which is very knowledgeable about design system about best practices of UX we have an engineer which is an agent that is preventing my code from being a bad code or ideally being a bad code we have an implementer which is the final person who's going to actually write the code and implement stuff so these are just a few examples one recommendation I give to people is Don't try to reinvent the wheel try to see how you actually work with your teams and try to represent them as agents like how they work what they care about how they decide write that down and make them the agents right that's one of the best recommendation one of the worst things you could do is Go on x or go on LinkedIn and see all of those skills from really famous people who have very specific ways of working and then just loading hundreds of those skills that you don't even know they exist and you're not thinking in first principles you can learn from them there's great content but dive deep into which skills make sense to you which ones could fit your flow and then only adopt those or ideally write your own based on what you're exploring and seeing, right?

**Andre Albuquerque** (00:48:31)

So this is what my PM MD is basically doing. Let me actually show this working in a production environment. So now we are on a cursor with Cloud Code, right? And we have a feature, right? And whenever I ask for a feature, what it's going to do is going to run my Cloud MD on the background and and my CloudMD already knows that they need to call the PM. I don't need to call the PM. I just need to say what I want it to do, right? And as I built this infrastructure, they are solving the problems that I don't need to care about. I only need to care about the feature, the problem solving, the requirements I raised, like the typical thing you do as a PM, which is great because you just built your team. And I asked this feature, right? And let's see.

**Andre Albuquerque** (00:49:19)

I got an answer. I'm not going to give you the whole context of the feature, but I got an answer from the engineer. The engineer found some things inside the code base and gave me some recommendations. And it's telling me specific things so that I'm aware. I don't need to understand everything that's here. I mean, you can if you spend a bit of time. I understand it, but it tells me this is my recommendation. I'm actually going to go up because I want you to see an example where multiple... Multiple agents are being called okay so perfect we have this example so I asked for a specific feature but I wasn't sure about the design so what the PM decided was all right the myself me Andre is not sure about the design I'm gonna call the designer agent so the designer agent does a brief this is an answer right and it has a summary of the designer's decisions so it talks about a specific layout it talks about the code because it also has an understanding of the code.

**Andre Albuquerque** (00:50:16)

It talks about visual experiences. It gives recommendations and even asks me questions. And these are questions before the engineer agent writes the code or writes the architecture. So it's asking me stuff so that I can answer or make decisions so that the next agent can start working on it. And the beauty about this is that Even if you're not technical, which is the case, you're answering as if your own engineer or your own designer in a team meeting with you would be asking you the same questions. And the fact that you're giving them the information, it prevents your code from being worse, it prevents features from being wrongly built or adding functionality that your product doesn't actually need. And this is the level four, which is like you're starting to build a machine that then is going to build a product for you. And you can focus a lot more on problem framing, on understanding what to build, what makes sense, what priorities, because you have the team.

**Andre Albuquerque** (00:51:14)

Now, I have a final recommendation here, which is when you're building something, let's say you build a functionality, you had this flow going and you get to your branch after building something and you don't like what happened. You don't like the flow or you don't like the design or you don't like the decisions. Your instinct would be, oh, I'm going to just say to Claude, fix these things on the feature so that it's great. And then you can push this and make it live for your users. That's actually not the right mindset. The right mindset is what within the flow, the pipeline, your agents and your skills failed. and led to a bad result. You identify that and you change the agent or change the skill or change your CloudMD. Why? Because the next time you're going to have a feature, you don't want that to happen again so you just improve the machine so that in the future it becomes way easier for you to just again focus on the problem ask your team ask your agents and then ship the feature better I even do something else which is if I don't like a feature I just created I change the machine and I ask it to build it again run the pipeline again and see if the final result is closer or is exactly what I actually want This is what AI native teams are doing is they're working 50% of the time on improving the infrastructure, the machine itself, rather than just tweaking feature by feature, right?

**Andre Albuquerque** (00:52:39)

So if you actually now see an AI native team, what you'll see is like you can have like two or three people, you can still have the typical trio, like a product manager, engineer, a designer. But they're all builders, meaning that they're all shipping code, they're all building features, but then a percentage of their time is improving the agents or the skills with their own knowledge. So the engineer is going to be improving the engineer agents and the engineer skills inside infrastructure. the designer is going to be improving the designer agent the designer skills and even the PM is improving the PM orchestrator skills and agent so that then every single one of them when they build they all have access to this infrastructure and it It's all becoming better over time with their own ways of building. So now you have three builders, you have an infrastructure supporting them, and you have a triple acceleration of what you can build.

**Andre Albuquerque** (00:53:33)

This is how you see small teams in AI-native companies shipping so fast with so few people.

**Aakash Gupta** (00:53:39)

And it sounds like the connective layer is that team-clawed config that you showed because the engineer will be updating the engineer MD and what it's using there, the designer will be updating the design MD. the PM will be updating the PM and they all are connected into that team cloud config. Is that right?

**Andre Albuquerque** (00:53:56)

Yeah, 100%.

**Aakash Gupta** (00:53:57)

Everyone's gonna

**Andre Albuquerque** (00:53:58)

be connected to that. In my case, for example, I create this repository with my skills and every time I make a change, I push it there My team gets a notification on Slack saying, hey, there was an update on the team's repository of skills. Please upload or download or clone it again or update your own so that you're up to date and you're using the best ones. And then you can choose which ones to use, of course, but at least you're creating standards. If your company is bigger, you might even have a whole team, an AI ops team or R&D team just building this for everyone else. But if you're in a small team and those are the teams who need to accelerate more, you definitely want to invest or put time on that specific topic.

**Aakash Gupta** (00:54:39)

One of the things you wrote about on LinkedIn that relates to all of this that we've just shown people is that there are now only four jobs. Can you explain this and what the future really looks like of these roles?

**Andre Albuquerque** (00:54:50)

Yeah, so I love this post. It wasn't me originally writing it. I liked to comment on it. But this is completely true every time you look to a new startup. Like I worked for a while in VC. Investing in early stage and those early stage teams. They're super small So they're gonna be very pragmatic and you're gonna have maybe three founders and you have typically One founder which is significantly more commercial You have one founder who's significantly more technical and you have typically one founder who's significantly more product oriented, right? This is what happens and if you think about these four roles and It's what those founders look like in their inception, right? You have the commercial one, which is the hot one, which is basically guaranteeing that sales are done, marketing happens, you're getting the word out. You have the product person who's basically guaranteeing that something gets built.

**Andre Albuquerque** (00:55:44)

Now they have the ability to actually build it, right? And yeah, they're going to be vibe coding and slopping and doing a lot of stuff because in the beginning when you're trying to find product market fit, who cares if you're doing too much stuff? You're trying to Get shots at the target and then of course your technical person is going to be the person trying to guarantee that what gets done has the right scalability is reliable it's built the right way etc etc so that when you grow the team when people join so it's not that different from this reality but now applied to multiple teams so you can easily see a full-stack squad that is an owner that owns a P&L owns a impact owns an outcome and has this stack and the beauty about this and I want to highlight specifically the security or SRE or infra because the moment you create a great infrastructure that allows a non-technical person to actually code with AI to a production repository It doesn't matter if that person is not technical anymore because what matters is the infra or security person is doing a great job at protecting the repository.

**Andre Albuquerque** (00:56:51)

Protection here doesn't mean prevent the code. It means new code that comes in needs to go through a bunch of checks to guarantee that when it goes into production is safe. This is literally the same thing a senior engineer does when a junior engineer out of school joins a It's not new The difference is now the junior engineer Is a non-technical person using AI To vibe code a new functionality And I see a lot of people making a fuss out of this But this is a known reality And I think a lot of teams are going to be transitioning This way because the velocity To ship is crazy different

**Aakash Gupta** (00:57:27)

what's the flip side to this velocity though and you even have the word slop here how do you avoid shipping slop how do you avoid you know famously like the clod team ships like this but they have bad uptime how do you avoid those issues yeah

**Andre Albuquerque** (00:57:41)

I mean again the the more you invest in infant security the more likely are you to prevent situations like that because you create friction right the friction here is not preventing people from building it's Is this passing all the checks so that when it goes live, it's not creating more risk or more problems? That's number one. Number two, the friction you create on the problem side. This is where product people investing in infrastructure should be putting their time. Because, for example, I have three skills that whenever I run an Epic, I have a jobs to be done skill. I have an opportunity solution tree based on Teresa Torres' amazing book and I have a Moscow skill which goes for the must should could and won't prioritization technique and what it does is like it creates three notion pages on that requirements on that PRD that explores those three frameworks and what I'm actually doing is I want people to read through them and see how Is this making sense?

**Andre Albuquerque** (00:58:39)

Like, have we dedicated enough time? Can we check and go to the next phase of solution building? And until that document or that memo or that addition to the PRD, which is built by the skills with Cloud Code, is completely thought through, like, I don't want people building the solutions. But then that becomes part of the initial process, right? And it's not just PMs or non-technical PMs doing that. Engineers do that. Designers do that because we're all builders. And it completely changes the what you decide to build. And that's the two ways you prevent slop in the beginning and the end. And I wanna highlight something really important here, which is one of the things that decelerates people teams companies the most is collaboration and this sounds contrarian which is like the fact that you have people having to collaborate it's what slows everything down now if you look at the development process in three stages ideation or discovery stage one execution stage two and delivery or enablement stage three collaboration should be happening in the beginning and in the end meaning you get people together deciding working on problem, et cetera.

**Andre Albuquerque** (00:59:50)

And in the end, you get people actually having the product in their hands and helping push it to the market, push it to commercial. But in reality, what's happening is collaboration is happening on the execution, right? It's happening on dependencies. It's happening on I do this, you do that, et cetera. And it slows everything down. And then in the beginning, in the end, there's no collaboration. Only PMs are in the decision. Only like engineers are delivering. And it's completely flipped up. And when you start Changing this, you see acceleration deeply because then people work a lot on, they collaborate a lot on decision making and then every single person, people, teams of one can execute by themselves and then they come back in the end and collaborate on like, does this make sense? Can we merge this? Is this working with the product? And we together deliver the product to the user.

**Andre Albuquerque** (01:00:36)

I think this completely changes the, completely flips but if this happens, we reduce a lot of slop and we accelerate teams a lot.

**Aakash Gupta** (01:00:44)

You caught my eye a couple months ago when you made this LinkedIn post about 90% of European PMs being non-technical. Talk to me a little bit about the differences between PMs in Europe and the United States and the implications for adopting AI tools.

**Andre Albuquerque** (01:00:58)

Yeah, so even though I'm not 100% sure of the number of, if it's 90%, if it's 99, or if it's something in between, it's going to be a pretty, pretty high number. You got to see the product culture in Europe is very different. If you go If you go to a lot of European companies, you're going to see a large number of POs, of product owners, something that you very rarely see in the US or even in the Asia market. And the product owner culture in Europe, it focuses a lot on a bit of a glorified delivery manager without the actual technical skills. In a certain sense, you're paper shuffling between someone defining strategy or roadmap or listening to customers and then the engineering and the design team on the other side and you're kind of in the middle you're trying to do a great translation work you're possibly trying to do a bit of a project management work within these teams but unfortunately your hands are a bit tied by this product culture and Yeah, I think this is one of the biggest problems we see in a lot of tech or software development in Europe is that the people who are talented, who are smart, and who should be able to actually drive a lot of decisions are not being able to drive them.

**Aakash Gupta** (01:02:19)

So if the system is broken, what's a move for a PM in this environment? Go work for a multinational company or how do they get out of it?

**Andre Albuquerque** (01:02:26)

I think it has to do a lot with your personal energy because I mean I don't think you should move because that's your reality I think if you have the energy you should try to fight to make it a better reality I truly believe like a lot of this is ingrained in management right like maybe the managers the product leaders they haven't seen any other way so they're kind of trickling down that format but You just need to spend a bit of time in a US company, for example, or seeing how they build and you see it's very different, right? So if you have the energy, you should definitely try to influence how product is built, create that small pocket of of experimentation of doing things differently because it's not just good for you to actually gain the scope of product management and kind of leave behind the product owner it's also good to the team and specifically because one thing I notice in a lot of companies that I work with is that when you have a product owner what the team is well unconsciously or consciously seeing is that that person alone owns the product and that's actually not true because the entire team the entire squad at least should be owners of the product, but they're not because the title says that person is the owner of the product, which is a lie.

**Andre Albuquerque** (01:03:43)

And you, at the same time, again, unconsciously or not, you feel like you're the owner of the product, which makes you, again, a leader where you're not, or at least a manager where you're not. And again, the title is breaking all of this. And you end up seeing in a lot of European organizations, squads or teams or pods, which are completely disempowered and they don't like that. The engineering teams are not participating in decision making. They're not part of the ideation. They're not part of the discovery. Often you don't see the design teams participating in the final delivery and actually bringing the product to the customer. And it feels like the teams are all siloed. And in my opinion, it actually starts with the fact that there is a product owner rather than a team feeling owner of the product.

**Aakash Gupta** (01:04:27)

So what is the answer here? How can PMs start to build more themselves?

**Andre Albuquerque** (01:04:32)

First of all, I think you need to understand that that is not the reality that you should be aiming for. There's other ways to do. That's the first thing. I had a manager who once told me that to cook great food, you have to have great food. So you need to understand that there is great food out there. There are other ways, better ways of building product. Number two is... Get some coaching or get some mentorship from people who are maybe inside companies who are building this way and spend a bit of time if you can spend a bit of time Asking them like how does it work? What am I supposed to do? How can you do this like my own program? And when you read content Number two is you want to start Getting that report with your manager getting that report with a product culture within the organization and start understanding where you see a gap to start changing the way you operate and number three you want to start getting allies with your team meaning your engineering team your design team your AI team and kind of explaining to them look We don't want you to be in the end of the line.

**Andre Albuquerque** (01:05:42)

We actually want you to participate in every single point of the development process, both from decision to ideation to the discovery to the last delivery and the go to market and the enablement. Like we want a team to be an owner of the entire process. So start with this. And even if you already have a roadmap, you have a track. and your manager has expectations because you have milestones you have a roadmap to deliver start trying to find some things in the roadmap that you can just try to manage differently within the team you don't need to completely change the way you work from one day to the other you can start small as an experiment and try to do things differently now that means that you need to also change a few of the rituals right if you Up to now you have a ritual of discovery or decision making where maybe a significant part of your team is not in the room well start by getting them in the room otherwise they'll never participate right if you're doing all the decisions of scope and requirements and design decisions like that is already a problem like other people should participate or even have ownership of of that process so i think making these small changes is definitely step number one wow

**Aakash Gupta** (01:06:54)

So much ground we covered here today. What's the thing a PM should go do on Monday morning? What's the Monday morning roadmap to becoming a builder PM?

**Andre Albuquerque** (01:07:03)

Okay, so this is ambitious. Let's say it depends a lot on your team. But if I was getting started on this and I went through the levels and I'm getting to the level like three and I'm feeling comfortable, I would definitely go to my engineer and and let's assume you have a github account and I would ask look put me as a collaborator of a low-risk repository meaning even if you can create a repository for me like that is connected to the product a new repository a new feature and just allow me to just do something and then go to your backlog pick a feature that has been on the backlog forever and like literally sorted by oldest doesn't matter right pick something something that you know that is in the bottom of the backlog and it's never going to get done every single PM has a bunch of these and then ask cloud code with that requirements to build it right and you can even push a branch you're not going to merge it to production like the engineers are not going to let you but just try to see the magic happening see the power you just gained by being able to do that as a PM right now imagine a reality where Every single person in the product squad can do this for the actual backlog.

**Andre Albuquerque** (01:08:16)

Like this would be my Monday morning. Like I heard this and this is what I would start doing.

**Aakash Gupta** (01:08:21)

Amazing. Andre, people love the episode. They want to learn more. They want to get in touch with you. Where should they go to find you online?

**Andre Albuquerque** (01:08:28)

I basically use LinkedIn. Feel free to connect. And if you want to know more, builderscamp.com is where we run our bootcamps, where we train people to become builders. So that's basically it.

**Aakash Gupta** (01:08:39)

All right. And I think he even does corporate training. So if you want to get your boss to get Andre to come in, consider him for that as well. Andre, thank you so much for being here.

**Andre Albuquerque** (01:08:48)

It was a pleasure, Aakash. Really appreciate the time.

**Aakash Gupta** (01:08:50)

See you guys in the next episode. I hope you enjoyed that episode. If you could take a moment to double check that you have followed on Apple and Spotify podcasts, subscribed on YouTube, left a rating or review on Apple or Spotify and commented on YouTube, all these things will help the algorithm distribute the show to more and more to get access to nine and many other amazing tools that will help you as an AI product manager or builder succeed. I'll see you in the next episode.
