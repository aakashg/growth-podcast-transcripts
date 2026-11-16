---
title: "Advanced Guide to AI Prototyping with Sachin Rekhi (Reforge)"
subtitle: "The exact system to go from AI slop to production-grade prototypes."
date: "2026-01-26"
host: "Aakash Gupta"
guests: ["Sachin Rekhi"]
speaker_names: "substack"
substack_url: "https://www.news.aakashg.com/p/sachin-rekhi-podcast"
youtube_url: "https://www.youtube.com/watch?v=74kamD2jUng"
duration: "01:12:39"
word_count: 12752
source: "Substack episode transcript (aired audio)"
---

# Advanced Guide to AI Prototyping with Sachin Rekhi (Reforge)

*The exact system to go from AI slop to production-grade prototypes.*

**Aakash Gupta** (00:00:00)

Whenever I tell this to people, the first thing they say is all AI prototypes are slots.

**Sachin Rekhi** (00:00:04)

When you first start using AI prototyping tools, you get enamored with something like this because all you typed in was, hey, create me a CRM application that lets me track my opportunities, my contacts. With such a simple prompt, you ultimately get an incredible output, but it still is AI slot.

**Aakash Gupta** (00:00:22)

Meet Sachin Reki, the former head of product at LinkedIn's Sales Navigator. He now teaches PMs AI prototyping. He's taught AI prototyping at SF Tech Week. He's taught it to thousands of PMs at Reforge. And today he is dropping all of the sauce for free. Could everybody be building this way or is this only possible for the leading edge AI companies like Anthropic?

**Sachin Rekhi** (00:00:42)

I call this concept product shaping. This idea that we're taking

**Aakash Gupta** (00:00:47)

our

**Sachin Rekhi** (00:00:47)

ideas, prototyping multiple solutions to multiple problems, testing them with customers, and then deciding what to go build in production. That's the concept of product shaping.

**Aakash Gupta** (00:00:56)

Can you walk us through this AI prototyping mastery ladder and what it shows?

**Sachin Rekhi** (00:01:00)

There's actually 15 unique skills you kind of have to master to be able to do AI prototyping well.

**Aakash Gupta** (00:01:10)

And now into today's episode. Sachin, welcome to the podcast. Thanks. I'm excited to be here. I want to start with something you posted about how Anthropic builds product and how it's pretty wild. Can you walk us through what's so interesting about how Anthropic builds product?

**Sachin Rekhi** (00:01:51)

Yeah. So let me talk about how we normally build product to create the contrast and make that clear. So the way it works is normally when we're thinking about our roadmap, we're trying to prioritize problems that our customers have. We might be saying, hey, look, here's a feature that our customers want us to build. Here's experience they're struggling with. So we start by prioritizing that problem. We then put it on the roadmap. And then what we do is figure out what solution we want to build. Designers, PMs get together and start ideating what a potential solution to that problem is after we've already prioritized it. Now, let me contrast that to the way that Claude actually does this. Anthropic does this for Claude code. They say, actually, let's build a bunch of prototypes for all the customer problems that we're thinking our customers want us to solve.

**Sachin Rekhi** (00:02:45)

And so they'll create a bunch of these prototypes. They'll launch them internally. and then they'll see hey internal users who are dogfooding it what do you think what do you like what's working what's not working and then they decide to productionize the best prototypes now what's so unique about this is that they're prioritizing not only what is actually a problem worth solving, but a problem solution pair that's already vetted based on the fact that people have tried it out. And that's what's so exciting here that they're now prioritizing based on really great solutions that they know they're actually going to work in the market.

**Aakash Gupta** (00:03:28)

Should everybody be building this way, or is this only possible for the leading edge AI companies like Anthropic?

**Sachin Rekhi** (00:03:35)

Yeah, that's a great question. I call this concept product shaping. This idea that we're taking our ideas, prototyping multiple solutions to multiple problems, testing them with customers, and then deciding what to go build in production. That's the concept of product shaping. I actually do think... That to date, the only people who've been able to do it are frankly, largely these incredible companies like Apple that ran into a huge lab. Prototypes, right? Johnny Ive was in the lab prototyping all sorts of things and then ultimately showing it to Steve Jobs and other folks and then deciding what to prioritize. The best story of that is actually the story of the iPhone. What happened was Johnny Ive had this incredible capacitive touch interface that he was playing with in the lab for a tablet. He ended up showing it to Steve Jobs and Steve is like, look, this is really cool, but I think this will be better on an iPhone on a phone as opposed to a tablet.

**Sachin Rekhi** (00:04:35)

And ultimately they canned the tablet project. They created a phone and obviously the rest is history. Now, in the past, most companies couldn't do this. They couldn't justify building thousands of expensive prototypes that we're all just going to throw out. But what is now possible with AI prototyping is that it's so cheap for us to go build these prototypes. It's incredibly easy for any of us to do that without thousands of dollars being spent on these wasted lab projects. And so I do think now we're going to bring this product shaping company from just the best companies to a broader swath of companies can be doing this. And frankly, I believe most should be doing this.

**Aakash Gupta** (00:05:17)

So whenever I tell this to people, the first thing they say is, well, All AI prototypes are slop. And you actually recently wrote about this. You talked about how people will often get wowed when they type in something here. You know, we've just typed in create a simple CRM and it's created something that looks pretty good. Why is this slop and how do we avoid it?

**Sachin Rekhi** (00:05:37)

So, you know, at first, when you first start using AI prototyping tools, of course, you get enamored with something like this because you look at this and all you typed in was, hey, create me a CRM application that lets me track my opportunities, my contacts and my companies. And with such a simple prompt, you ultimately get kind of an incredible output, right? The reality is this is a fully functioning mini app. I can go click on contacts and click on opportunities. I can actually go and actually add new items. And this is all from such a simple prompt. And so I get it why people first love this. Now, here's the reality. When we really dig into this and we look at it, first, it has very generic styling. Frankly, it almost looks like a wireframe. It doesn't have the design sense that any product I would ever build has, right?

**Sachin Rekhi** (00:06:33)

So I would never ship this in the way that it looks. And so that's the first challenge. Second, it's kind of very generic. Yes, it looks like every other CRM application. I can't launch into the market a new CRM application that looks like every other CRM application. I need to differentiate. How am I going to win against incumbents if I just launch with something that looks exactly like every other CRM application, right? And so there it falls apart. And finally, it sort of implements these very basic, um, scenarios like, okay, add a contact and whatnot. It created a dashboard, but is this really the view that we realize based on understanding our customer needs that they need to be productive on a day-to-day basis? And so when you look at it, it's magical that we used AI to produce this in just a couple of minutes, but it still is AI slop because we could never ship this.

**Sachin Rekhi** (00:07:31)

This would never be considered high craft work. And so I think that's where we need to get beyond to do this. Now, it turns out AI tools are usable to create high quality work, but we have to learn how to use them well.

**Aakash Gupta** (00:07:45)

So that's the roadmap we're going to give everybody today. Can you walk us through this AI prototyping mastery ladder and what it shows?

**Sachin Rekhi** (00:07:52)

Yeah, so, you know, I've been really on this kind of journey to help PMs and product teams figure out how do they go from AI slot to really great, valuable AI prototypes. And so as I was really digging into this, I started asking people, what do they do in their process? And ultimately, I discovered there's actually 15 unique skills you kind of have to master to be able to do AI prototyping well. And what I wanted to do was sort of create a succinct framework around those skills. And so what I did was create the AI prototyping mastery ladder. And so the idea here is that you need to learn each of these 15 skills to prototype well. And I broke them out into different levels. It turns out learning this is like any craftsperson. You need to move from apprentice to journeyman to master and really sort of nail the foundations before you go up to another level.

**Sachin Rekhi** (00:08:48)

And that's kind of what I'm trying to show here. And so when you're first starting out prototyping, you have to learn the basics. And this is really the apprentice level, which is how do you prompt in a AI prototyping tool to do it? Well, how do you actually, in fact, edit your prototypes? We're going to spend most of our time, not one shotting a prototype, but editing it. And so learning how to edit well ends up being really important. The third challenge is really about design consistency, right? How do we get our prototypes to look like our product? And by default, they don't look like our product, but there's a set of skills we can learn to ensure they do. And so that's sort of some of these core skills around kind of the apprentice level. Now, as we go to the journeyman level, we want to start learning things like versioning and debugging.

**Sachin Rekhi** (00:09:36)

It turns out when we're actually AI prototyping, we're going to run into all sorts of bugs. And so knowing how to prototype well ends up being so important. Now, another core capability here is what I call diverging. It's this idea that, hey, look, AI shouldn't be used just to create one output. We should be using it to create multiple outputs, just the way we'd use a designer. A designer would come up with three variants and then help us think about the pros and cons of each. It turns out if we learn how to use AI in that way, we can get that same benefit. Now we're creating these prototypes largely to validate with customers. And there's some techniques and skills we need to learn around how do we validate with customers well. And so those are some of the key skills around the journeyman level. Now, finally, we have the master prototyping level.

**Sachin Rekhi** (00:10:29)

And so this is really the kind of cream of the crop skills to do this really at a expert level. Now, things like functional prototyping. It turns out we can turn our prototypes and actually make them usable products. That is something that was never possible with any of the things that we did before with static mockups. And so that now becomes possible with this idea of being a master prototyper. Another great one is this idea of product shaping. It's that product prioritization process we were just talking about, which is we should now be creating multiple prototypes, putting in from our customers, and then deciding what to put on the roadmap, which is an entirely different way to build products, but is now unlocked with this idea of AI prototyping. And so this is the ladder of skills that we need a ladder up into to turn our prototypes from AI slop to well-crafted product designs that we're all

**Aakash Gupta** (00:11:30)

excited to ship. Amazing. I'm bought in. I agree completely. Can you walk us through this ladder, do some demos and show us how this is done? Let's

**Sachin Rekhi** (00:11:38)

do it. So the

**Aakash Gupta** (00:11:38)

skill

**Sachin Rekhi** (00:11:39)

I want to start with is this idea of design consistency. And what that is, is we want to make sure that the designs that we produce via the AI prototypes actually look like our product. And we need to learn how to go do that. And so the first skill is this idea of baselining, which is creating a baseline of our prototype of our current product design so we can use that for prototyping. Now, I want to do this for my own product, Notchoy. So what I'm going to first show you is just a screenshot that I took of Notchoy. Notchoy is a note-taking app for both individuals and teams, and it has kind of a classic notating view. You have a sidebar, a list of notes, and a main note content area. So let's start actually building our prototype. I'm going to be using a tool called Bolt, which is one of the popular AI app builders that can definitely be used for prototyping.

**Sachin Rekhi** (00:12:34)

And so I'm going to start with a very simple prompt. I'm saying, please recreate the attached screenshot. And all I've done is given it that same screenshot I showed you. And so I can go in here and just say build now and have it go and actually start building that.

**Aakash Gupta** (00:12:51)

What do you think about the benefits of a recreate prompt versus I've seen some people try a prompt like look at this screenshot and understand the design system or match this design style?

**Sachin Rekhi** (00:13:04)

Yeah. So, you know, I find that what I found actually kind of gets you the highest accuracy is starting with recreating a screenshot. Once you have that screenshot, improving it manually through edits. and then creating a baseline that ultimately ends up getting used broadly by the team. And so there's a little bit of setup work in this approach, but I find it's worth it because you can ultimately create a baseline that ultimately gets used across everyone on the team. Only one person has to set this up and create it. Now, some of the skills that you mentioned, which is like, hey, let's give it our design guidelines are certainly helpful. But starting with a core product baseline ends up being even more helpful because it will then inherit the styles automatically based on what's in that screenshot.

**Aakash Gupta** (00:13:58)

Very cool. And I actually didn't know about this on the enterprise side. So like if you bought like an enterprise bolt license or something, you could like seed it with a design style like this for all of the members on your team.

**Sachin Rekhi** (00:14:09)

That's right. Collaboration is core here where you can actually ultimately turn this into a reusable template that everyone on the team uses. And frankly,

**Aakash Gupta** (00:14:19)

we should be

**Sachin Rekhi** (00:14:19)

doing this, right? Because all of us are going to build new features on a given experience. And so we should have a baseline that we're using that's shared across the team. And in fact, we can make it so that only one person on the team is responsible for keeping that up to date. Maybe someone on the design team, for example,

**Aakash Gupta** (00:14:36)

and the

**Sachin Rekhi** (00:14:36)

rest of us get to benefit from that.

**Aakash Gupta** (00:14:38)

Totally. It should be somebody who owns the design system. Probably that's like enabling both Figma and your AI prototyping tool to plug into it. That's right.

**Sachin Rekhi** (00:14:47)

And you know what? I have this already loaded here that I can jump right to. This was that exact same prompt of recreating Notchoy. And so when we look at this, you can see it actually did a decent job of recreating the core note show interface. I have my sidebar. I have my note list. I have the note content area. I have my core actions, like adding notes. And so it's not bad, actually, in terms of a first run at recreating it based on the screenshot. Now is when I can get to work to actually improve this to really make sure it looks exactly like my core product. And as I said, this effort is worth it because we're establishing a baseline that not only am I going to use for future projects, but everyone else is going to be using as well. So to show you that, let me give you examples of how I might improve this.

**Sachin Rekhi** (00:15:40)

We're looking at this recent header. It turns out it's actually centered in the actual product. So I can just basically select it using the selector tool and say, please center the recent text. And so that's a very small edit that I'm able to make to try to get it to look more and more like my product. And so we'll give it a minute here to go actually do that.

<!-- sponsor -->
**Aakash Gupta** (00:16:04)

Today's episode is brought to you by ReForge. You know that feeling when you try to prototype something with AI and it spits out something completely generic? The problem is that most AI app builders aren't built for product teams, for product managers like me and you. They're built for founders who are starting from scratch. But product teams aren't building from zero. You have an existing product, real customers, design guidelines. Reforge's new product, Reforge Build, generates prototypes that reflect your real pricing tiers. Real features, real customer language, not generic placeholder. so stop fighting tools built for founders start using a tool purpose built for product managers to ai prototype well in the way that we're teaching this episode with todd try it for free at reforge.com akash that's reforge.com a-a-k-a-s-h and use the code build for one free month of premium

**Sachin Rekhi** (00:17:04)

And so now I can start planning the other little edits that I'm going to want to make here. I noticed that the color schemes are slightly off in terms of the sidebar and the background colors of the main columns. And so I can plan on making that change next. Let's let it finish this particular change just so you can see what that looks like.

**Aakash Gupta** (00:17:27)

Do you like to do one change at a time or are you okay with batching like three or four?

**Sachin Rekhi** (00:17:30)

Yeah, so the next one I'll show you on batching specifically to solve for this round trip time. You know, we spend a lot of time when you're prototyping just waiting for a response. So things like batching is actually kind of pretty important. So we can see it did center the recent text as I showed you. Now, let me give you sort of a more of a batch example here. What I wrote here is set the sidebar background color to a specific hex color, set the note list background color to a different hex color and set the note content background color to, um, again, a different hex color. So firing that off. And so that's kind of three changes batched into one here. I find that when I batch and I do it like this, where it's like three color changes, this works really well. Now, if I batch by doing three completely unrelated types of changes that I put in a single prompt, you get yourself into issues because then you can't version if it got something wrong.

**Sachin Rekhi** (00:18:25)

So you got to be thoughtful about kind of the batching level that you're doing here.

**Aakash Gupta** (00:18:28)

Makes sense. What bolt plan are you on? How many tokens do you end up burning with this?

**Sachin Rekhi** (00:18:33)

On this one, I think I happened to get through Lenny's newsletter when he's like offering a specific plan. And so I think it's the lowest pro plan.

**Aakash Gupta** (00:18:47)

Well, I think that's like 10 million tokens per month. It's a lot, but I have a Bolt account too. And I burned through like 30, 40 million a month easily on my site. So you have to be careful.

**Sachin Rekhi** (00:18:57)

Yes, no, that's definitely true. Cool. So now it's set the colors appropriately on the sidebar and whatnot. So it's looking a little bit more like my actual product. Maybe I'll make some changes to this add note button because it doesn't look exactly right. So let me fire this off. I'm saying make the button fully rounded, remove the plus button and center the add note text. And so that way it's going to look a little bit closer to kind of the actual button that I have.

**Aakash Gupta** (00:19:24)

We'll get to see how it handles a batch, which I think ever since like 4.5 especially, it handles them pretty well. Back in the like 4, Claude 4 Sonnet days, I used to like try to stick to one change at a time, but now I feel like I can give it like five or six and it's okay.

**Sachin Rekhi** (00:19:38)

Yeah, that's right. I think it's gotten a lot better in the batching sense. And now you look at it like the add note button, like great. Now it looks way more like my actual product. And so part of what I'm showing you here is you can make all these little edits to get this template to look way closer to your actual product. And so let me fast forward here and show you the actual baseline I ended up building for NoteJoy. And so this is probably after about an hour of those edits to try to improve the template to create this baseline. And so that's what we're looking at. And we can see this actually looks very close to the actual underlying note joy product. And what's great about this now is that now that I've created this template, I can save it. And now anytime I want to actually create a new prototype, all I do is fork based on this.

**Sachin Rekhi** (00:20:34)

And so I create a new project based on this fork. And now I start prompting to actually create my new features.

**Aakash Gupta** (00:20:42)

So that's what I want to save as template button or do you just take this one and then you just hit fork? Like what's the actual workflow look like?

**Sachin Rekhi** (00:20:49)

Yeah. So what I did here is I named it no joy baseline. And so in this tool with Bolt, it's basically a project that I've labeled baseline, like baseline V1 baseline V2. And now all I have to do is press duplicate. At that point, I create a new project based on that template. Now, certain tools like Magic Patterns and Reforged Build literally have a template feature which let you take any project and convert it to a template. If you have that, that's an even better way to do it, but you don't even need that. As long as you can name the project and fork from it, which all the tools allow, you can then go ahead and use it as a template regardless of whether it's called that in the tool or not.

**Aakash Gupta** (00:21:33)

And for those of you who are worried forking, it doesn't affect the one that's original. It's basically creating a copy and then you can do whatever you want with it.

**Sachin Rekhi** (00:21:40)

That's exactly right. So let's take a look at doing exactly that. So what I did here is I simply forked that template and now I'm going to ask it to actually start prototyping a feature. So let me describe what this feature is. We get a lot of requests at NoteJoy that are saying, I'd love to be able to add an AI chat bot to NoteJoy that allowed me to query my notes. Wouldn't it be great if I can ask it to summarize a note or ask it a question to find something in my notes? And so it's been a pretty frequent feature request. And so let's say it's my job to go and prototype this to go figure out what this might look like. What I can do is take this baseline template and then give it a very simple prompt. The prompt I gave it here is I want to add an Ask AI feature to NoteJoy to allow you to ask questions of your note, which will leverage an LLM and your notes content to answer the question.

**Sachin Rekhi** (00:22:39)

I'd like to explore a couple of different entry points into the Ask AI chat experience. So that's all I told it. Now, I call this style of prompt an explore style prompt. And the reason is because it's fairly generic. I didn't give it a detailed spec of what I want this feature to look like. And it's because I'm still in the exploration phase. I want to use AI to help me explore what a potential solution might look like. And so let's see what it came back with. You can see it's actually introduced these Ask AI buttons, both in the header and in the footer. And so I asked for multiple entry points, and these are the two that I came up with. You know, fairly logical locations for where this might exist. Now, when I open this up, I can actually see that it's created a full AI chat experience.

**Sachin Rekhi** (00:23:28)

I even already asked it a question, which is, what is this note about? And it's telling me this note is about the Q1 roadmap for a company outlining planned product and sales initiatives, as well as highlighting what is not prioritized and any backlog requests. So there's a couple of things that are remarkable about this. First, it actually looks like my product, right? The fact you look at the styling of this, the way the buttons are, the color scheme that's being used, it looks like a product that belongs on Notchoy. And this is because we established a strong baseline template and we're using that baseline template to then create our features. It automatically knows to inherit the styling that's inherent in that baseline template. And so that's why I love this approach of baselining before creating any new feature on top of it.

**Aakash Gupta** (00:24:17)

Pretty powerful. And I'm guessing what this is doing in the back end is it's hopefully using Tailwind and it's kind of defining those design elements. So then they're just reusable everywhere.

**Sachin Rekhi** (00:24:26)

That's exactly right. So each of these are being created as actual components that are reusable, not only from the styling perspective, but also from the window perspective. It created a sidebar component, a note list component, a note view component, plus now this new Ask AI component as well. And so it's fairly modular in the code. Now, what's amazing is I asked it this question, what is this note about? And it actually told me. And so what's amazing is it actually is giving me those actual interactions that I'll want on the product, right? It's me even making these decisions like, OK, when I asked the question, it right aligned my question and then it left aligned the actual chat response. And so we can start quickly getting at the interactions and deciding whether that's what we want or not. And in addition, it is actually even created a database in the backend to store these.

**Sachin Rekhi** (00:25:24)

And so the conversations were automatically stored. And in fact, it's calling an LLM with the notes content to go pull out this content. And so in many ways, it's done a lot for us from a simple prompt. And we're getting much more quickly into the design considerations of what this product would look like. Now, to even get to this point, it would have taken a designer in Figma way longer just to even get the static mocks, let alone getting to the point where we're actually getting design interactions being represented.

**Aakash Gupta** (00:25:58)

Makes sense. Yep. So huge time saver.

**Sachin Rekhi** (00:26:00)

Yeah. And so this is the whole idea of design consistency, that when we can actually establish a baseline, prototyping on top of it becomes really straightforward and ensuring it actually looks like our design. So that's the first skill I wanted to go into. Now, the second skill I think it's really worth diving deep into is this idea of diverging. and diverging is that idea that we want to ultimately figure out multiple design directions for a given product. Let

**Aakash Gupta** (00:26:32)

me set

**Sachin Rekhi** (00:26:33)

up a scenario for that. I want to go back to my LinkedIn days when I used to work at LinkedIn. LinkedIn has this feature called LinkedIn News in the top right corner, which shows you what's trending overall. But the feature I wish LinkedIn always had was this idea of what's trending within my network. What's the news articles that just my connections are sharing? Because that's what I really care about. And so let's say I'm back at LinkedIn. I'm a PM that's trying to prototype some ideas around that. Let me show you how I'd actually go about doing that. This time around, we're actually going to use a tool called magic patterns. And so the first thing I asked it to do was please recreate the screenshot of LinkedIn. I gave it that exact screenshot I just showed you. It then faithfully recreated it. And it did a decent job of recreating most of the interface.

**Sachin Rekhi** (00:27:25)

And so that's how I start with a typical baseline. Now, the reason I'm showing magic patterns is magic patterns has this idea of diverging built right into the tool. And so you can see here, I used a slash command that it supports called inspiration. And I'd said, I want to add a feature on the LinkedIn homepage called News in Your Network. I want to explore multiple designs for this. It should show the top articles most frequently shared by my network with the people who shared them, as well as provide their commentary on those articles. And so it's now generated four different variants of this feature. And so let's take a look. This first one here is showing a core newsfeed item. It says tech giants announces new AI ethics coalition. It's showing me the 14 people in my network that shared it. It's even showing me a bunch of, uh, uh, commentary from those people in my network.

**Sachin Rekhi** (00:28:27)

So this is a pretty useful design variant, right? It's matched the styling of LinkedIn. It looks like a truly native, uh, newsfeed experience, um, inside the product. So that's a great direction I can go in, but here's the power. I got three other directions to consider. It's given me this now, which is a, uh, another top, um, card format, um, and showing me four different cards of different articles in a different layout. And so that's an interesting one to consider whether I'd want to do something in that direction. If I then look at the next one here, it's actually decided to create a news in your network sidebar right below the top news section. And so that's an interesting idea.

**Aakash Gupta** (00:29:13)

Might want to go in that direction or not. At least you have different options to test. And I feel like the goaded sort of workflow here is like, take these three, upload them to a website where you get real humans to use them, like usertesting.com or something, so that you get real feedback on it instead of just using your gut. Totally.

**Sachin Rekhi** (00:29:30)

You know, I find what I typically do with this is I start with these four and then my designer and I might have a conversation about like, okay, great. Where are the pros and cons? What's the general approach or directions we want to go in? Maybe pick two directions that are like really interesting and then, you know, build them out a little bit. Maybe we'll do some iteration on them and improve them a little bit and then put them in front of our customers and start showing them what they look like and getting their feedback and then ultimately solidifying on the path that we wanna go down. Makes sense, yeah. If

**Aakash Gupta** (00:30:02)

you have those steps of iteration with your designer, you're gonna be able to build something that everybody's bought into.

**Sachin Rekhi** (00:30:07)

That's right.

**Aakash Gupta** (00:30:09)

You know that feeling when you try to prototype something with AI and it spits out something completely generic? Then you spend hours tweaking colors, fonts, copy, and features just to make it feel like your actual product? Here's the problem. Most AI app builders aren't built for product teams. They're built for those starting from scratch. But product teams aren't building from zero. You have an existing product, real customers, design guidelines, a backlog full of ideas you need to explore and validate fast. That's what Reforge Build does. AI prototyping that starts from your product. Add your customer feedback, strategy docs, and product features as context. Create reusable templates using your product design. Explore multiple variants side by side. Collaborate with your team in one place. Reforge Build generates prototypes that reflect your real pricing tiers, real features, real customer language, not generic placeholder. Stop fighting tools built for founders.

<!-- sponsor -->
**Aakash Gupta** (00:30:57)

Start prototyping like a product team. Reforge Build. AI prototyping built for product teams. Try it free at reforge.com slash akash. That's R-E-F-O-R-G-E dot com slash A-A-K-A-S-H. and use the code build for one month free of premium.

**Sachin Rekhi** (00:31:14)

And so it's great that a tool like Magic Patterns has this functionality built in, but I want to show you that even if the functionality isn't built into the prototyping tool, you can still do this. So let's go back to Bolt and do the same thing here. I basically gave it the same prompt. I want to add a feature on the LinkedIn homepage called News In Your Network. And the only difference I added here is I said, I want to explore multiple designs for this. And then I gave it the rest of the description of the feature. And so simply by saying, I want to explore multiple designs for this, Bolt did the right thing and gave me multiple designs. And so what it did was produce this initial design and it added this little toggle in the top right corner, which is showing me all the different designs I can basically select between.

**Sachin Rekhi** (00:32:00)

And so we're currently on the detailed view. And so this is a card style laid out that's pretty detailed with multiple articles and the people in my network that shared it. It then offered a compact view. And so this is like a very compact version of it. And I'll take a quick look at a third one, a card view, so much broader card view. Now, this is great. So regardless of whether your tool has native support for diverging, you can certainly use these tools in that way. But here's a really interesting subtlety. One thing you might notice is these variations look nothing like the variations in Magic Patterns. which is kind of shocking, right? Because frankly, most of these are still using Cloud Sonnet underneath that hood as their core model. But because they have different system prompts, you're actually getting different designs. And so I often do this.

**Sachin Rekhi** (00:32:50)

I often go to multiple tools with a simple explore prompt like this. Now, just by going to two tools, I have eight different design directions. And this gives me so much inspiration to quickly start whittling down what are the pros and cons of these different approaches. I can either have that dialogue with myself or with a designer or with my engineering counterparts. And I get so much more exploration and ideas than I would have if I simply use these tools to visualize whatever one idea I already had in my head. 100%.

**Aakash Gupta** (00:33:21)

I think this is the hidden superpower of AI prototyping. especially if you maybe ask your tool to diverge with three, six, nine, 12, or ask three or four different tools. Because before, a lot of times we were constricted to like, let me go ask the designer to come up with some divergent solutions. Now, the PM itself can come to the table with some different divergent options. And the more divergent options you look at, I think the better likelihood you will of having a feature that succeeds.

**Sachin Rekhi** (00:33:49)

That's exactly right. And I think this is where we're going from sort of that concern of AI slop to, wow, AI is doing craft better than humans could, right? Because we don't have the time to ask our designer to come up with 15 variations. It's just unrealistic given the constraints and time it takes to build a Figma mockup, right? And so now we're getting to the point where we're using AI to do more brainstorming, more exploration than we've traditionally done in an effort to get to kind of the right solution for our customers.

**Aakash Gupta** (00:34:20)

So does this take us to that journeyman level?

**Sachin Rekhi** (00:34:22)

Yes. And so now we're really at exploring that journeyman level of capabilities and skills here. Now that we're diverging, for example, I want to now talk about really getting to that master level and showing you what is really possible with these tools when we get there.

**Aakash Gupta** (00:34:39)

So

**Sachin Rekhi** (00:34:39)

let me kind of bring up a prototype that I've built for that Ask AI NoteJoy feature. And so here's the prototype I built. I can actually publish it, get back a full URL. And so now let me go to that URL. And so what we're looking at is my deployed prototype for the Ask AI feature. And so I've built this out as a fully functional prototype. And so let me show what I mean by that. So you can click on different notes here and you're getting actually the note content. I've even loaded actual articles in here. So Dan Hockenmeyer had written this great article called Vibe Analysis. I basically loaded the entire content of it. Lenny a while back did a whole podcast with Brian Chesky and I've copied the transcript into here. And let me show you how we can actually use this. I built out my Ask AI feature as a sidebar.

**Sachin Rekhi** (00:35:35)

And I don't know if you remember this podcast from a few years ago. It kind of went viral because everyone thought that Brian Chesky said that product management is dead. And so let me just ask it here and say, did Brian Chesky really say that product management is dead?

**Aakash Gupta** (00:35:56)

One of my newsletter subscribers said I had to stop talking about this podcast because I talked about it so many times after it came out.

**Sachin Rekhi** (00:36:05)

Yes. And, you know, it's a great example of virality because that's obviously not what he actually said. And short answer, no. Chesky said we didn't eliminate the people or declare PM as dead. He restructured the role. He combined inbound PM and product marketing. And so this is sort of getting into some of the details of what he said. Now, what's so cool about this is... This is literally my Ask AI feature built and being used, right? This is so far away from what we can do with mockups today. And so what's great about this is not only did I basically prototype the interactions, I'm seeing what an Ask AI feature in Nocho might look like, but I'm actually getting responses. It's calling OpenAI's API. And I even prompted it to add this little feature at the bottom. You might see that there's a little dropdown that's a model selector.

**Sachin Rekhi** (00:37:04)

And so I prompted it and told it, hey, can you use both GPT-5 and GPT-4-1? And I can actually go here and compare the responses. This is really fascinating because not only am I prototyping interactions, I am literally able to see the different output coming from different models. And now as the PMs start to decide, do I have preferences in terms of what models should we really provide in the NoteJoy Ask AI feature? And when you think about this, this used to only be possible when engineering built prototypes. An engineer would have to go code this up and go implement multiple models. And now we can do all of this thinking and decisioning and playing with an actual product experience well before engineering even gets involved.

**Aakash Gupta** (00:37:53)

How did you embed the OpenAI API? Because I've had multiple people tell me that they have trouble with that. Like you give it an API key or like they often just assume it'll work off the bat because it's already using AI. But how do you really build those features under the hood?

**Sachin Rekhi** (00:38:08)

Great question. So what I said was, I basically took the previous prototype that we had that was not fully functional and said, I want to turn this into a fully functional Ask AI feature. To do so, please use OpenAI's GPT-5 API to actually answer the question based on the content of the note. So that was basically my prompt. Now, what it ultimately came back with is, okay, if you want to do that, I need the API key for OpenAI. And it even just gave me directions of like, here's how to go get an API key. If you don't have one, make sure you fund it with like five, 10 bucks. Here's the URL to go to. And it kind of walked me through all those directions. And then it said, paste back the API key. I pasted it back and then it incorporated it into its actual code.

**Aakash Gupta** (00:39:00)

Awesome. And then I think people are always worried about putting API keys into a vibe coded tool. How do they make sure that that's secure and it's not just eventually posted out there and somebody else can just use their API key?

**Sachin Rekhi** (00:39:12)

Yeah, that's a great question. Actually, many of the tools, what they have done is created these new secret repositories. where they actually store it. So there's a couple of different approaches that are taking. Bolt, for example, has an entire dialogue all around where you put those secrets, and then it stores them securely and only gives specific backend access to these things. One of the challenges that vibe coding tools often had in the past was these secrets would show up in your client-side code that anyone could steal and then go charge against. And so the tools are learning now that that's obviously a no-no and really creating these workflows for how do you get around that by storing them securely and not making them available in the front-end code. Each tool does it a little bit differently. Another one of the tools has you put it in a environment file, which is again, securely stored.

**Sachin Rekhi** (00:40:05)

So they've really figured out some of those early challenges that I think a lot of these Vibe coding tools suffered from. Got it.

**Aakash Gupta** (00:40:11)

What else do we need to know about to become that master level AI prototyper?

**Sachin Rekhi** (00:40:15)

What we talked about now is creating a fully functional prototype. But what we're going to want to do with this now is test it with real customers. I want to talk about this idea of customer validation and why that is so critical in using AI prototyping well. I want to show you a few interesting things that I've done with this prototype. The idea here is that we can take this URL and send that URL to our customers that we want to validate with. Now, after they played with this feature, see what happens when I press the X button. I've set it up to have a built-in survey question as well. I have it say, how likely are you to use the Ask AI feature if launched in NoteJoy? Maybe I'm enamored with it and I'll say, oh, maybe I'll use it weekly. I then have it ask, could you describe a personal use case where you think the Ask AI feature would be helpful?

**Sachin Rekhi** (00:41:07)

Maybe I'll say something like for summarizing notes and submit that. Now what's great about this is I'm getting survey feedback right in my prototyping tool and in the prototype. And so I could go and do one-on-one customer interviews, which I should certainly do, but now I'm showing you how do you scale that feedback? Beyond the one-on-one customer interviews, you can start doing things like this, send this out to a hundred people, get them to play with it and integrate this. Now, let me show you what else I've integrated here. I've also integrated analytics. And so I like to use PostHog, which is one of the many analytic tools that you can use. You could use Mixpanel, you can use Amplitude, any of the common tools. I happen to like PostHog because they have a fairly generous free plan. And for prototypes, you don't need that much usage.

**Sachin Rekhi** (00:41:59)

So it actually works pretty well. And so you can see it's giving me default analytics, things like daily active users and weekly active users of my prototype. Now, this is really interesting from the perspective of, I can say, do people even come back to my prototypes, right? After people use them, are they coming back? Am I getting good retention? And so that becomes really valuable as I'm trying to understand, is this prototype useful? Now I can even instrument custom analytics. And so you can see here, I have the Ask AI header button, floating action button, the close button. I've instrumented each of these individual actions. And now I'm seeing how many people click the header action, how many people click the floating action button. And so now I'm getting detailed analytics on my prototype. Now, again, you could never do this with a Figma mockup. And we've done all of this before ever involving an engineer.

**Sachin Rekhi** (00:42:59)

What I find really cool here is I can even get into session replays. And so let me play this one here. You can see that red dot is the user's mouse and you can see exactly where the user is clicking, what they're clicking, what questions they're asking the bot. And these session replays end up being, again, an incredible way to scale your feedback. I can watch a bunch of these just based on people using it, decide where the friction points are and where the friction points are not. And so this ends up being really valuable as I think about how do I understand how people are using my prototypes.

**Aakash Gupta** (00:43:40)

Just to get it like that's a huge hack, just like integrate post hog, which seems like it's pretty easy. Then you get session replays and default analytics built in. I don't think many people are using that. So that's one to steal from such in here.

**Sachin Rekhi** (00:43:52)

That's right. And like, look at this. I just got a heat map of where everyone is clicking inside of my prototype. Now, this is across an amalgamation of all the different users that I've sent my prototype to. Maybe I sent it to 100 people and I got a bunch of people to use it and look what I'm seeing. This makes it absolutely clear, for example, that Ask.ai button in the top right corner, really red, lots of clicks. That little button in the bottom left corner that was another alternative entry point, almost no clicks. And so it's making clear to me, hey, Maybe I should ditch the bottom floating action button and just stick with the top right Ask AI button. That's incredible feedback that I can visualize and get in a scaled way through these prototypes that I couldn't get before.

**Aakash Gupta** (00:44:37)

Huge. Simplifying your interface is always the hardest part. And this is giving you literally, you can see it where you can.

**Sachin Rekhi** (00:44:43)

That's right. And I think this is, again, some of the really master techniques that get us beyond the AI slop where I think right now there's just such a desire to add, add, add. Let's add features. Let's add more. Oh my God, it's so quick and easy to build features with AI. Let's add it to our interface. But we all know cluttered interfaces don't make great products. And the fact that we can be using these tools to help us refine our interface, clean up what's working, what's resonating, where the usability issues are versus not, That really takes us to the next level with our prototyping. So the other thing I want to speak to is how did I do this? Right? So how did I do the functional pieces of customer validation? Now, all I really had to do was prompt and say, please integrate posthog analytics.

**Sachin Rekhi** (00:45:28)

It then went off, found the PostHog API, integrated it, and then said, I need your API key. Here again is the URL to go to, to go get your personal API key. You can then hand it to it. And then it went and basically implemented the basic analytics. Now, when I wanted it to actually instrument the specific product analytics, I then just prompted again. I said, please instrument in post hog any clicks to the ask AI button and call that event ask AI header button clicked. I did the same thing for all the other actions. And so I didn't have to do the manual tagging that you typically do when you're trying to add this custom instrumentation. I could just do it purely from prompts.

**Aakash Gupta** (00:46:15)

Much faster. So I want to ask you this. How does AI prototyping change when you're building a new feature versus thinking about a new product?

**Sachin Rekhi** (00:46:22)

It's a great question. And in fact, the actual skill is fairly different, right? When we have an existing product, what we're entirely focused on is design consistency with that existing product. How do we get it to look and feel like our own, the product that we have right there? And so the tools that I described on design consistency become really important. leveraging baselines and templates. Now, a brand new product is a very different beast. We don't actually even have a set of style guides in the same way for that new product. In fact, actually to build a new product and build prototypes for it and not make it look generic is actually a bigger challenge. And so we need to be thoughtful about how do we create that design aesthetic that we want for our product and avoid that generic AI slot. Now, the ways to do it is the number one tool I use is what I call inspiration sourcing.

**Sachin Rekhi** (00:47:19)

And what that is, is really as we're designing any part of the experience, find some inspiration as a screenshot. okay, I wanna build a feature like this. I kinda like the style that we're using in this screenshot, incorporate that. And then it will actually build it using that design. You could then do that for any given feature. And so that helps you to establish an aesthetic and establish best practices in the new product. And so I find that actually works really well. Now, part of it is how do you source all these great ideas? And I love using sites like Mobbin that is a kind of a directory of screenshots of every product that's ever existed. Even places like Dribbble have a community of content out there. What's interesting is this traditionally used to be the job of designers, right? But as we're blending roles, now that us product folks as well are getting involved in the actual prototyping process, we need to start improving our own design inspiration as we're thinking about how do we make prototypes that actually look great.

**Aakash Gupta** (00:48:31)

You bring up an important point. I think it was Itamar Galad who talked about how there's probably 20 other things the PM needs to be doing. Talking to customers, learning from the business, analyzing features, writing out the strategy, looking at prior results. There's like so many things that they have to do. Why should the PM be picking up what the designers did? Like, why are we bringing this into the PM's role? Is that the right thing to be doing when the PM already has so much other stuff to do?

**Sachin Rekhi** (00:48:59)

It's a great question. You know, what's fascinating about this is I think the jury is out still in who is actually doing the prototyping. As I've looked in the space, I've seen three different paradigms currently being used. First is PM lead. So a PM is the one in the tool doing the prototyping. And so that is sort of taking over the responsibilities of design. Now, the second mode I've seen is actually design lead, where designers are the one prototyping. And in fact, they're finding actually it's faster for me to build stuff in a prototyping tool than it is in Figma. I can do many more variations. And then the PM is informing the design requirements just as they've always done. And the designer is the one that's doing the heavy lifting, learning these tools. And what I find actually is designers are incredibly good at making compelling looking prototypes because that's the skillset they have.

**Sachin Rekhi** (00:49:57)

Now, the third paradigm I've seen is collaborative. PM and designer are collaborating together to create these mockups. Now, almost all of the tools support collaboration where we can share a project. I could be adding prompts. You could be adding prompts on top of it, and it actually works pretty seamlessly. And so we can collaborate together on it. And so I've seen different organizations doing one of these three approaches. And there's pros and cons to each. I mean, you brought up a great point like, hey, a PM has so much else to do. Should they really be taking over some of these other responsibilities? At the same time, I've seen some product folks who have such strong domain understanding of the problem space because they're so steeped in the customer feedback that their ability to bring it to life all on their own in a prototyping tool is actually beneficial compared to the lossiness when they try to communicate those requirements to designers.

**Sachin Rekhi** (00:50:59)

And so in some cases, even having the PM sort of take over some of those traditional responsibilities is actually turning out to be helpful. So I think part of the challenge is there's different modalities of prototyping that are common right now and still to be seen, which is gonna become industry norm.

**Aakash Gupta** (00:51:19)

Don't assume, I think, guys, after watching all the PM content and PM influencers, that you should be spending 20, 30 percent of your time on AI prototyping. And another thing that I see people do is they think about prototypes as literally helping with delivery, like delivering the first version of the code. You've been beating the drum on why prototypes are for discovery, not delivery. So can you explain that?

**Sachin Rekhi** (00:51:39)

I think that if a PM is trying to get a full version of their product out through these vibe coding tools, they're doing it wrong. And the reality is we have at our disposal in these organizations, incredible engineering organizations that have access to incredible AI coding tools, and we don't need or shouldn't be thinking about replacing them. And instead we should be thinking about is, using these tools for the discovery phase. How do we figure out what product to build and what solution is going to resonate most with customers? And so that's what discovery has always been about. These tools are incredibly good at that. They're incredibly good at generating multiple iterations, helping us get that in front of customers, doing validation based on that, even creating multiple prototypes and testing multiple directions with customers, and then deciding which one to go with. That is incredible value to PMs.

**Sachin Rekhi** (00:52:34)

And I think that's enough. And then when you hand it off to engineering, it turns out the code that's been generated by the prototyping tools is not scalable, not maintainable, not robust. And that's okay because it turns out our engineers can then do that work and translate this prototype into production level code.

**Aakash Gupta** (00:52:55)

And I just want to act as the skeptic here, but doesn't Claude Code, isn't the way that they're using it that the PMs actually do build the first production version of it?

**Sachin Rekhi** (00:53:04)

Yeah, so what's interesting about this is the tooling ends up being pretty different when most people are using AI prototyping tools. For example, if you're using a lovable bolt or magic patterns or whatnot, it doesn't have access to your existing code base. And so it's creating from scratch, not following any of your code rules, not following any of your established norms. And now when you ultimately want to convert it yes you can take the designs out of your prototyping tool and when you're using cloud code it's going to create components that match up with ultimately your actual code base and so we're not there yet in the prototyping tools to make that happen automatically Now, one day, I think where this is certainly going is this idea that hey, look, you have these components that are reusable that are in your code base that your prototyping tool also uses.

**Sachin Rekhi** (00:54:05)

Now, that's where we get to the dream state of actually the prototype code you're producing is production code, because all it's doing is assembling a set of reusable system components that already exist. Now, the only way to do that today is through tools like cursor and cloud code, which are the engineering oriented tools. And I'll say some PMs are embracing those tools. But a lot of PMs are still finding those tools to be too technical. And the existing tools that are really designed for product managers don't yet have those capabilities. And so we may eventually bridge the gap. But to date, I think even if we just get the win of better discovery, we're already winning with these tools.

**Aakash Gupta** (00:54:47)

So a lot of people, they're embracing these tools and they're saying prototypes replace the PRD. Just deliver a prototype, just deliver a prompt set. I think Microsoft CPO even said something like that. Why is the PRD not that? So

**Sachin Rekhi** (00:55:00)

I've been harping on this drum as well, that I think a prototype is incredible and should be a primary artifact that all of us are producing. But what a prototype actually speaks to is the user experience. and the functional requirements. It doesn't touch product strategy and all the strategic questions that a good PRD includes. For example, how is this feature that we're implementing going to help us differentiate from the competition? How are we going to acquire users for this feature or this product? How is this going to improve our monetization position by adding this feature functionality to the product? All of these are critical strategy questions that we should be asking ourselves that our PRD should cover, but a prototype never will. And so I think we are losing so much if all we do is produce the prototype without the strategic lens of why we're building this in the first place.

**Sachin Rekhi** (00:55:58)

And so I do think our PRDs, we can now remove all the experience details from them. We don't have to just say, here's the user scenarios, here's the features I want to implement. We can put that all in the prototype. But we still need to ask these very basic strategic questions of why we're building the feature in the first place and how it's going to improve our strategic position in the market.

**Aakash Gupta** (00:56:19)

Yeah. So I think the strategy component, a couple other components I'd highlight. What is your hypothesis? Because we always want to be using the scientific method. What is your North Star metric, your guardrail metrics, your diagnostic metrics? Because we always want to set that out in advance so that we can then look at, you know, in a statistically significant way, whether things are working and we can experiment and test with things. And what are the open questions? Like, what are we trying to test? What are we not trying to do with the feature? All those things, a prototype doesn't answer those questions. So really, the ideal unit of work for a PM right now is a prototype plus a PRD. Now, a lot of people, they come to me and they're saying, hey, I don't have access. And you actually shared some really, really interesting data on this.

**Aakash Gupta** (00:57:02)

Depending on what access people have, what AI prototyping tool should they use?

**Sachin Rekhi** (00:57:06)

This is a great question. So we can get into my specific perspective on all the AI prototyping tools, but... probably something i encourage a lot of organizations to start with is think about what is the lowest friction way for you as a pm to start prototyping today now what's interesting about that is you could go do an investigation of what the top tools are available to go use and that's useful but the reality is you might actually have access to something already and And what I'm finding is, for example, organizations may have access to Figma Make because they already use Figma as their design tool, and it's easy for them to get access to Figma Make. Or for example, if you're already heavily invested in the Google suite of tools, you're using Gemini, for example, you probably have access to Google's prototyping tools, whether it's AI Studio or Firebase Studio.

**Sachin Rekhi** (00:58:04)

They just launched a new great tool, Antigravity. Or if you're on the Microsoft stack, they also have GitHub Spark. And so part of the decisioning here isn't just finding the best tool for you, which is still a worthwhile exercise, but to get playing with these tools as soon as possible, finding the least frictionful way to go do so. And oftentimes that means accessing the tools that you could easily get access to because they're easily approved within the organization. Now, a meta point on this that is so fascinating is I think what's happening despite AI being as revolutionary as it is, we're actually seeing kind of traditional B2B enterprise tactics working that large organizations may not have the best prototyping tool, but they have a win. They have an in with the customer, whether it's because they have distribution, because folks are already using it, whether they built a suite of tools that this is the additional win.

**Sachin Rekhi** (00:59:05)

It's been fascinating to watch that we're quickly seeing even in this innovation cycle, some of the classic B2B enterprise tactics actually leading to a lot of adoption. That was what I was really sharing in that data. But it's amazing to see how much, for example, Google's tools are already being leveraged because of how easy it is for organizations to adopt it because they're already Google customers. 100%.

**Aakash Gupta** (00:59:28)

So we're about to walk you through what the best tools are, but use the existing tool you have and then go make the IT request. So if you are going to make the IT request or you are the product leader who's controlling the budget and going to make a tool, can you walk us through the AI prototyping tools market, the different ones out there, what the pros and cons are of each?

**Sachin Rekhi** (00:59:47)

All right. So let's talk about the various tools that exist in the market. Now there's really three high level categories of tools that exist. The first one is AI app builders. Now an AI app builder is just an AI tool that you can use to build a fully functioning app. And so you could use these as full vibe coding applications to launch entire applications to customers. Now, of course, I'm not recommending that PMs go in Vibecode apps. I'm telling them to use it for prototyping, but you can certainly use all the apps in this category for prototyping. And so these generic AI app builders is that first category. Now, let me just kind of give you my quick opinionated take on each of the popular tools in the space. I showed you a bunch of prototypes in Bolt, which is one of my favorite tools. I love it because it's just fast.

**Sachin Rekhi** (01:00:43)

You notice that you spend a lot of time waiting for prompts to actually be answered. And Bolt has one of the fastest tools, but some of the interesting technology decisions that they made. Another great one is v0, v0.dev. What people love about this one is it's really optimized for front-end UIs. It's actually pretty quick and good at building beautiful UIs from scratch. Another really popular tool is Replit. Now, when we think about Replit, it's known for building really robust, full stack applications, including backend, front end, and giving you control. Now, if you really want to build a robust solution, Replit is one of the best solutions. Now it comes at a cost. All of that backend capability that it supports actually slows down the overall prototyping process. So you really want to ask yourself, do you need that capability or not? Lovable is another fantastic prototyping tool that's really made a name for itself as optimizing for non-technical users.

**Sachin Rekhi** (01:01:44)

Now when you look at Lovable's own marketing, they even show how kids nowadays can even build prototypes. And so if you are intimidated by how technical some of these other tools are, you're going to love Lovable. Now, Google has actually ended the market with a couple of different app builders. The first is Firebase Studio. Firebase Studio is kind of like a replet in that it's really optimized for building both backend and frontend applications, using Firebase for the backend and building on a frontend as well. Now, I think if you're in the Google ecosystem, you're going to love this, especially if you're already existing Firebase customer. Now, another AI product that Google launched was Google AI Studio. This one is optimized for building Gemini apps. If you're thinking about building applications that use any of Gemini's APIs, whether it's things like Gemini, NanoBanano, VO for video generation, it's so easy to prototype solutions that use those APIs in Google AI Studio.

**Sachin Rekhi** (01:02:47)

The final one I mentioned here is Microsoft has also entered the app builder game with their own GitHub Spark tool. And again, that's going to be optimized if you're in the Microsoft ecosystem. If you're using GitHub, you might like that because it's already working with the tools that you're already using.

**Aakash Gupta** (01:03:03)

So this is the first cat. I'd throw in a couple more that people might have heard about. Miro has its own AI prototyping tool. You mentioned Reforge Build. That's one that uses your contacts. There's magic patterns. There's Dazzle. This space, there's Base44. There's like a million tools right now rushing into this space.

**Sachin Rekhi** (01:03:20)

Totally, yeah. No, you just mentioned some in the next category that I want to talk about in the actual specific AI prototyping tools. But yeah, I'd add Base44, a couple of the other ones you mentioned as these generic app builders. As we get into the next category, these I consider true AI prototyping tools. Now, what do I mean by that? I mean that they're purpose built for product teams to generate prototypes, not fully vibe coded applications. And what's great about that focus is they've now created unique capabilities that product teams actually care about when they're prototyping. And so these four fall into this category. And in fact, I actually think product teams are best off using these tools because they are purpose built for their purpose. Now, the first one we'll talk about is Reforged Build, which is really optimized for product teams focused on full stack experiences.

**Sachin Rekhi** (01:04:18)

And it has some of these really unique capabilities like diverging. Both Magic Patterns and Reforge Build make it really easy for you to diverge and come up with four different variants of a given idea just by using a command. And so that's an example of where they really shine. They're also really good at bringing in your external context from your product specs, your PRDs, your design guidelines, and easily incorporating that into the tools so you can get feedback. Another cool thing I love about Reforged Build is they now even make it easy to get scalable feedback. You can use this AI interviewer to actually send out your prototype, interview people based on their feedback, and it recreates the one-on-one interview experience. And so that one's pretty great. Magic Patterns is also a fantastic tool in this category, focused on front end experiences. So they've made the decision to not care about back end because again, we're not building full vibe coded applications.

**Sachin Rekhi** (01:05:19)

And given that they really optimized around design, they even have some cool capabilities where you can take your Magic Patterns built prototype and then export it to Figma if you do need to complete the process that way.

**Aakash Gupta** (01:05:32)

If you guys want to know why they didn't choose back end, the CEO was on the podcast and he explained why. But let's keep going. Oh, perfect.

**Sachin Rekhi** (01:05:40)

Now, Figma Make is another great solution. Obviously, Figma is heavily used by designers. And so designers are going to love this tool. It's got one of the best importers of Figma files directly to Figma Make. And it has broad adoption from the fact that Figma is already in a lot of organizations. And so I think it's going to get a lot of particular excitement from there. They are quickly adding a ton of functionality to sort of catch up with some of these other tools. And I'm pretty excited about where Figma Make is ultimately going to go. The last one to mention here is Alloy. Now this is a fairly new one, but what's really cool about it is they've really optimized for recreating your product experience. As I said, the best way to start is with a baseline. And what they did is they created a browser extension that can extract your product from the website and recreate in high fidelity pretty much the entire user experience.

**Sachin Rekhi** (01:06:38)

And you'll find that compared to some of these other tools, it actually does a phenomenal job of really capturing the exact design. And so another one that's worth checking out in this category. So the final category of prototyping tools I want to talk about are the AI coding tools. So these are the tools that your own engineers are already using to write production code. Now, what's interesting about them is all of them have introduced agentic capabilities that enable you to not only use it for AI coding, but also for prototyping. And so tools like Cursor have an agent that works very similarly to the agent that you'll find in a Bolt or Lovable. And so you can simply prompt to create your application. Now, the challenge with these tools is you have to then do a bunch of the heavy lifting on your own. For example, they don't have built in deployment solutions.

**Sachin Rekhi** (01:07:31)

So you're gonna have to use something like Vercel or Netlify to deploy your prototype or ask your engineers to ultimately do that part. So there's a little bit more of a learning curve with these tools. The next category is really the CLI tools, the command line tools, things like Claude Code and Codex CLI. These tools you actually use in a terminal window. And so you open them up in a terminal and you can actually start actually prompting similar to how you'd prompt anywhere else, but now at the terminal. Again, sometimes people find these intimidating from a technology perspective, but actually they're very robust. Now, I call these AI coding tools my upgrade pick, you know, kind of like wire cutter upgrade pick. The reason I say that is because they'll become a point where you build your prototype, it gets pretty robust, that you're going to start running into errors or speed issues in the traditional prototyping tools.

**Sachin Rekhi** (01:08:29)

And that's when you're going to need to upgrade to these AI coding tools. Another scenario, if you want to use your existing code base, for example, you have an existing set of reusable component library that your engineers have created, and you want to leverage that, you're going to have to use the AI coding tools for that sense. And so even though these come at a more technical ramp, they do become appropriate in those kinds of scenarios.

**Aakash Gupta** (01:08:55)

So this is a podcast we have to ask for your hot takes. You can't choose Reforge Build because you're affiliated with Reforge. If you were the head of product at LinkedIn Sales Navigator like you once were, and you could just buy one of these tools for your team, but you had the budget to buy one, which tool would you buy?

**Sachin Rekhi** (01:09:11)

Great question. I'm biased because I am fairly technical. And recently I've been very impressed by Cursor in its ability to, especially with the new Composer 1 model, to actually be exceptionally fast. at prototyping. And so there is a bit of a learning curve. But if it were me, I'd invest in educating my team to go whole hog into these efforts. And so I think that is sort of the great place to start. Now, if I'm advising a buddy of mine starting on these tools, I do think the AI prototyping category is a realistic place to start to get going and go from there. And, you know, I'd pick Magic Patterns right next to Reforged Build as the top set of tools that enable you today to do incredible stuff. The inspiration feature in Magic Patterns is so good at coming up with so many different design variations.

**Sachin Rekhi** (01:10:16)

I think if you adopt that, you're very quickly going to start to see the value of prototyping. And it might be a faster on-ramp to getting your organization going with tools like this.

**Aakash Gupta** (01:10:25)

All right, guys, you heard it. Reforge, build, and magic patterns. And you know what the crazy thing is? Both of those are part of Akash's bundle. So if you become an annual paid subscriber of my newsletter, you literally get 12 months of Sachin's top two recommended AI prototyping tools for free. If you have watched this far, it's a no-brainer. Check it out. Sachin, what else are you doing with your time these days? If people want to learn more about AI prototyping from you, where should they go?

**Sachin Rekhi** (01:10:52)

So first thing to do is follow me on LinkedIn. I always share my hot takes on product management, especially as it has to do with AI. So it's a great place to start. If you really want to go deeper on this stuff, I built out a course called AI Productivity with Reforge that not only teaches you all of these prototyping skills in detail, but is really about how do PMs use AI in general to be more effective in their role. We talk customer insights, we talk product strategy, we talk product execution, and all the tools that you could use to really do that well. So I encourage you to check that out as well.

**Aakash Gupta** (01:11:30)

Sachin, thank you for dropping so much knowledge. There are a lot of PNs and product leaders who you have just saved hours of time and you have just helped them do their job much, much better. Really appreciate you dropping all this knowledge. Of course. Happy to help. All right, everyone. See you later. All these things will help the algorithm distribute the show to more and more people. As we distribute the show to more people, we can grow the show, improve the quality of the content and the production to get you better insights to stay ahead in your career. Finally, do check out my bundle at bundle.akashg.com to get access to nine AI products for an entire year for free. This includes Dovetail, Mobbin, Linear, Reforge Build, Descript, and many other amazing tools that will help you as an AI product manager or builder succeed. I'll see you in the next episode.
