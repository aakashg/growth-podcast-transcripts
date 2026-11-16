---
title: "How to Build ChatGPT Apps (The Next App Store?) | Live Demo by Colin Matthews"
subtitle: "MCP protocol, live building demo, eval strategies, and why this is the biggest new PM distribution channel."
date: "2026-01-22"
host: "Aakash Gupta"
guests: ["Colin Matthews"]
speaker_names: "substack"
substack_url: "https://www.news.aakashg.com/p/colin-matthews-podcast"
youtube_url: "https://www.youtube.com/watch?v=Q2MfgGBUVwQ"
duration: "01:02:22"
word_count: 13412
source: "Substack episode transcript (aired audio)"
---

# How to Build ChatGPT Apps (The Next App Store?) | Live Demo by Colin Matthews

*MCP protocol, live building demo, eval strategies, and why this is the biggest new PM distribution channel.*

**Aakash Gupta** (00:00:00)

ChatGPT apps

**Colin Matthews** (00:00:01)

are a huge opportunity. How would you describe ChatGPT apps? You can have this kind of built-in experience where you can interact with an application directly in your conversation. I brought in my friend Colin Matthews. He is one of my go-to sources for technical topics on product management. This is a really underrated way to get more distribution. what's the case for other products regular people one you can build is like a spreadsheet or like a to-do

**Aakash Gupta** (00:00:24)

list app that gets pinned to the top what is the architecture of a chat gpt app so underlying chat gpt apps is this protocol called mcp or model context protocol i tried podcasting for a bit i built like probably four or five different sass apps this year this is actually my own prototyping tool wow i'm using opus 4.5 for pretty much everything what might be some interesting examples that we can build live

**Colin Matthews** (00:00:46)

there's

**Aakash Gupta** (00:00:47)

kind of two different ways to invoke apps the first way is to just type out the name the second

**Colin Matthews** (00:00:52)

way is because there might have been some news pieces that you read about what the chad gpt app store is but nobody has broke it down in terms of what it means for product builder so that's what we're going to do today Before we get into today's episode, if you can do me a quick favor and check if you have a following on Apple and Spotify podcasts and subscribed on YouTube, these are free actions you can take that really help the show grow. And if you become an annual subscriber to my newsletter, did you know that you get access to over $28,000 of premium products? That's right. mobbin arise relay.app dovetail linear magic patterns deep sky reforge build and descript they are all free for an entire year if you become an annual subscriber to my newsletter so go take advantage at bundle.akashg.com and now into today's episode Colin, thanks so much for being back on the pod.

**Aakash Gupta** (00:01:49)

Yeah, super excited to be here.

**Colin Matthews** (00:01:50)

So what I wanted to do first was take a look at the announcement video for this, because this was announced about a month ago at OpenAI's Developer Conference. Most people probably watch this video, but they've already forgotten about it. So let's refresh your memory. you All right, Colin. So everybody's seen the cool use cases. We saw an Expedia example, a Figma example, Booking.com, all these different apps that are built into it. How would you describe ChatGPT apps? What are they? And what is the ChatGPT app store?

**Aakash Gupta** (00:03:24)

Yeah, so ChatGPT apps are basically a way for companies to bring in their own designs, their own kind of way users should interact with it directly into ChatGPT. So rather than maybe giving a text summary of something or recommending something from a web search, you can have this kind of built-in experience where you can interact with an application directly in your conversation.

**Colin Matthews** (00:03:44)

Why does this really matter? Because I guess it's kind of hard to discover. That's what I feel like when I gave the example of the iOS app store, for instance, the discoverability was there. It was one of the few apps that people actually got pre-bundled with their new $1,000 phones. They're highly likely to open it up at least once or twice. And then when they open it up, it's showcasing different apps. It feels like ChatGPT apps are kind of hidden. I haven't heard about them.

**Aakash Gupta** (00:04:10)

Yeah, so I would agree at the moment. And again, we're recording this in 2025, so we expect it to change sometime soon. They are kind of hidden. And so there's a couple of companies that partnered with the initial release, as you saw there. Some other ones coming soon, like Uber is on that list as well, planning to release an app sometime in the near future. but yeah, they are kind of hidden. And there are definitely plans to bring together a full app store experience. So very similar to what you have in like iOS or Android, you'd be able to browse apps, find ones that you like, and then download them and use them inside of ChatGPT. There's one other mode of discovery that we will get into a bit more later. But one thing that ChatGPT promises is that if you put in a request that relates to an app, they might actually decide to kind of service that app to you.

**Aakash Gupta** (00:04:51)

So for example, if I say without installing the app, I'm looking for a hotel, I might get the Expedia app kind of surfaced in line, even though I didn't install it or ask for it to be in with.

**Colin Matthews** (00:05:01)

Okay, that would be super cool. So they might be building some sort of tool calling system that automatically figures out, okay, here's a reliable app to help service this particular request. And I guess they've already done some of that because I've actually seen nowadays when I do search for a hotel that they'll pull in some Expedia search results, although they don't always pull in from the app. It seems like they pull in from web search. So kind of how they're pulling in from web search, they'll start to pull in apps.

**Aakash Gupta** (00:05:25)

Yeah, exactly. Yeah. And again, it gives companies a little bit more control, right? There's a very large kind of maybe panic around. getting your content into ChatGPT, right? Because people know that it converts well. Actually, there was some news I saw today that it's like 26% increase in conversion when a user comes from an AI source because they have higher intent, right?

**Colin Matthews** (00:05:45)

Yeah, I see that too in my own sites, that the LLM traffic is much, much smaller in volume to like SEO, but really high conversion rates.

**Aakash Gupta** (00:05:53)

Yeah, exactly. So companies want to be present, but kind of playing this game of whack-a-mole with the ChatGPT web search is hard. And so now you have, from an enterprise perspective, a deterministic way to show up in the application, right? Your app is going to show up, especially if the user has it installed, but even if they're trying to do something and it's a relevant application, it can show up in their chat. and you'll be able to control what that experience is like. It'll be branded and you can even pop them back out. So a good example of this is Target. Target, I've recently announced that they're building an app and you can't finish like a checkout with them inside of ChatGPT. You can't actually purchase items, but you can build a cart. So you can say like, hey, help me find holiday items or Christmas, you know, presence for my siblings, it'll build the cart for you and then you click out and it brings you into Target to complete the purchase.

**Aakash Gupta** (00:06:36)

So I think that's another good example of like building this kind of deterministic catered experience that feels really great inside of Chagiput rather than relying on like web search to do the job.

**Colin Matthews** (00:06:46)

Makes sense. So in that example, at least I highly grok it kind of like the Expedia example as, OK, I'm offering some high ticket service. I might have been getting a lot of traffic from search in many cases. So I need to get into ChatGPT, access its 900 million weekly active users. So I understand that case. What's the case for other products, regular people like you and me? Like what sort of ChatGPT apps have you been building?

**Aakash Gupta** (00:07:13)

Yeah, so very similar to the App Store, you're probably going to see like the eventual Ubers, right, which didn't start at the very beginning. And then you'll see like the apps that are like the flashlight app, right? Like that, if you remember back to the iOS beginning, it was like that was an app you could download. And so I think we'll follow like similar paradigms here. So for example, like I've been messing around and building some apps and One you can build is like a spreadsheet. So ChatGPT can like use spreadsheets as well as you, and you can kind of collaborate back and forth. It's kind of like what, you know, you'd expect out of the AI experience in Google Sheets, but it doesn't quite work correctly in Google Sheets. You can build a little spreadsheet app inside of ChatGPT or like a to-do list app that gets pinned to the top.

**Aakash Gupta** (00:07:49)

So if you want to complete multiple tasks with ChatGPT, maybe you have like three things you want to do, it can check off those tasks for you. So you get like a visual indicator. So those are like the little utility type things that you could build. then you could build like more fully featured experiences right so things like you saw inside the demos there with like apps that have maps navigation search and like integrations with whatever you want on the back end i guess that's the last thing i'll mention here is that like there's actually no strict limitations in terms of what the apps can or can't do it's just that they're so early that most companies are releasing like very very bare bones versions of them to get into the marketplace but i think we'll see like a lot more complex apps than what exists today

**Colin Matthews** (00:08:25)

I love that you've been building these. You've even built a platform to build these. So you really understand the technical details. What do we need to know about how ChatGPT apps are made and built?

**Aakash Gupta** (00:08:36)

Yeah, so underlying ChatGPT apps is this protocol called MCP or Model Context Protocol. This is invented by Anthropic. It's about a year old. Basically what allows AI agents, so things like ChatGPT and Claude, as well as like Gemini, you know, Cursor, really like anywhere where you would be talking to an AI. It allows those tools to reach out to other things over the internet, other tools, and use them for whatever purpose. So you can think about like web search as an example of this, like a common tool that would be built into a chat application. Any other tool that you might want to think of, right? So things like booking a stay with Expedia or getting Figma to maybe do some design work for you. Those could also be defined as tools that ChatGPT or Claude or any other AI chat could call over this protocol of MCP.

**Aakash Gupta** (00:09:20)

So a quick diagram here. This one basically just shows us what it might look like to help book a short term stay. So as the user, you would say something like that. You know, I want to book a stay in New York for this time period. And Chachapi is going to decide first, does this request need an app or would it be beneficial to use an app? And if it does want to use an app, then what are the available tools that we can use in order to help facilitate this request? And so the first thing it's going to do is actually going to go ask for the list of tools that are currently available. And you can see that we have two tools available. We have book a listing and then browse listings. ChatTBD does cache this information, which basically just means that it holds onto it and it doesn't refresh unless you kind of force it to refresh.

**Aakash Gupta** (00:09:58)

But there is this kind of underlying need to know what tools are available before we actually go ahead and call the tool.

**Colin Matthews** (00:10:02)

If you're enjoying this episode, Colin literally teaches a course on this. The next cohort starts January 30th. It is on Maven. You can use my code to get a special discount off this course. I highly recommend Colin's content and courses. You all seem to love what he's doing and I personally love reading it. I gained so many epiphanies just out of this one podcast recording. So think about what you could get if you were working with Colin extensively over a live cohort course. Check out his course and now back on today's episode. Today's episode is brought to you by Vanta. As a founder, you're moving fast toward product market fit, your next round, or your first big enterprise deal. But with AI accelerating how quickly startups build and ship, security expectations are higher earlier than ever. Getting security and compliance right can unlock growth or stall it if you wait too long.

**Colin Matthews** (00:10:51)

With deep integrations and automated workflows built for fast-moving teams, Vanta gets you audit-ready fast and keeps you secure with continuous monitoring as your models, infra, and customers evolve. Fast-scoring startups like Langchain, Writer, and Cursor trusted Vanta to build a scalable foundation from the start. So go to Vanta.com slash Akash. That's V-A-N-T-A dot com slash A-A-K-A-S-H to save $1,000 and join over 10,000 ambitious companies already scaling with Vanta.

**Aakash Gupta** (00:11:24)

And the last thing is ChatTBT is gonna decide which tool to use for this request. So the browse listing one might make sense to start because we need to know what listings are available so we can show that back to the user. And so we get asked for New York on a specific date and we get back a list of listings from our MCP server. And then ChatTBT would kind of describe that information. So this is the bare bones version of MCP, right? There's no actual UI or app being involved here, but you could build this if you wanted to and just like have it say, here are the top five short term rentals in New York for that date. And it would literally just write it out as a description. The addition here on top of MCP is this thing that actually OpenAI kind of invented and is now being incorporated into the MCP, MCP spec, which is the idea of like widgets or these little interfaces.

**Aakash Gupta** (00:12:08)

So in addition to the raw data, the listings, it can also return a position or URL for a widget that we want to return. And so the last thing that ChatGPT is going to say is, okay, now that I know that there's a UI element or a widget that goes with this, let me go get that code and then render the code inside the chat. And so that's how we end up with like that code that shows up where your app that shows up inside the chat. And then it's still going to respond with something. So it can say like, here are the best options, some small description. Really, we're going to be interacting with the UI that you see here as like the main interface rather than the text.

**Colin Matthews** (00:12:41)

Makes sense. So how do we build one of these ourselves?

**Aakash Gupta** (00:12:44)

Yeah, so there's, let's say, the easy way and the hard way. So as you mentioned, I've been working on a platform to make this a little bit easier. It's called Chippy. And we can go ahead and take a look at maybe an example really quick before we hop into building it. But basically what Chippy does is it spins up everything you would need in order to build a ChatGPT app for you. So it spins up an MCP server for you. And when you prompt it, it's going to basically be specialized in building tools. So not full-stack web applications, but literally just what you need to build a ChatGPT app. And then there's some nice UI UX stuff that I built into it to help you build the app. So this example here, this is a coffee guide. So I kind of wanted something where I can look at a map and see maybe a good place to get coffee.

**Aakash Gupta** (00:13:25)

As you can see on the left-hand side, inside of Chippy, I just asked it to make me a quick location guide. And this is what it decided to build. So on the right hand side, we can see the component that it built. This is a tool, by the way, I'll go through that in one second, but has this little left hand pane. You know, we can kind of click through on this and it'll kind of pull up the right side for me and I can get directions. So this is what I decided to build. The other nice thing about using this inside of Chippy is we can kind of get a preview of what it's going to look like inside a chat experience. So I can say, where should I get coffee? And there's an LLM working in the background that'll actually call that tool and then throw it into the UI for us.

**Aakash Gupta** (00:14:00)

And there we go. So there's actually a full screen UI by default. We can see that's what that looks like there. And again, we can interact with it in this kind of, you kind of think of like a simulated ChatGPT, right? So a quick way to test what you've built to see if you like it or not.

**Colin Matthews** (00:14:11)

Okay, makes sense. So just to play that back, right? The easier way, what you're doing is you're bundling together an MCP server, which if we recall from the diagram, that's like how ChatGPT is going to get connected. It's the universal USB-C plug for LLMs to call tools like this. This is a tool. And then it's got the right understanding of what needs to be built to create one of these tools. So it simplifies the tool process to basically just prompting with an LLM. That's the easy way. What's the hard way?

<!-- sponsor -->
**Aakash Gupta** (00:14:40)

Yeah, so the hard way would be basically spinning up your own MCP server. That's the first thing. Getting that hosted on the internet somewhere. And then understanding how to write the code to build these tool definitions, as well as to build the UI. And there is something called bundling that has to happen, which is when it translates your UI code into something that ChatTPT can actually understand and render. Because the code that you write doesn't just get downloaded and rendered in the same format inside of ChatTPT. It has to go through this little process, bundling. And so you'd have to also bundle your kind of UI code. And then the last thing is just understanding what the options are. So like, you know, how to interact with the full screen version of apps versus maybe like the picture in picture or inline. All that kind of like guidelines that ChatGPT provides or OpenAI provides on how apps should be built.

**Aakash Gupta** (00:15:23)

All that stuff is kind of built into this agent. But

**Colin Matthews** (00:15:25)

if you want

**Aakash Gupta** (00:15:25)

to do it the hard way, you kind of have to learn some of that stuff and then host it, build it, and then eventually connect it to ChatGPT would be the last step.

**Colin Matthews** (00:15:32)

Okay, so you'd probably be using like a cursor cloud code sort of format versus here you have more of like a AI prototyping interface to build that.

**Aakash Gupta** (00:15:42)

Yeah, exactly. And you know, you can kind of get the experience of testing the tool that you built without going through all the steps of connecting it to ChatGPT. The reason I built this actually is because I was working on a completely different app for ChatGPT. And it was such a pain to go through the iterations of like, every time I wanted to make a small UI tweak, I had to rebundle the code, make the change, go back into Chat2PT, update it, and then see if I liked it. Whereas here, I can at least visually see it and then kind of play with it in the UI without having to go through that whole process every single time. Cool.

**Colin Matthews** (00:16:10)

Awesome. So what might be some interesting examples that we can build live?

**Aakash Gupta** (00:16:14)

Yeah, sure. So obviously, we have this one here. Maybe I'll just quickly spin this one up inside of Chat2PT. So in order to do this, there is one last step, which is just connecting. So if we go up to test here, we'll get a little URL that's generated for us. I'll copy that. And then we'll head over into a chat to BT year and we'll go into our connections in our settings. And you'll see here that, I mean, I have a bunch of enabled apps cause I play with these all the time. So you can see, I have a few that are built elsewhere and then a few that are built by myself as well. But basically the last step here is click create paste in the URL in this MCP URL field, turn off the authentication unless you really want authentication, and then also give it a name of some kind.

**Aakash Gupta** (00:16:54)

So this one we call like a coffee map. I think I already have one because I'm going to call this one coffee map too. And then finally click this little button. So it's a little bit involved when you're testing, Obviously, for installing apps, it's a lot easier, like the end kind of consumer experience. Even think about this more like the developer experience, right? Like I'm a developer. I want to build my own app. Those would be the steps that I go through to test it before I release it to everyone else. Obviously, installing like, you know, Canvas app isn't as involved. You just go in, click the button and click install. And that's pretty much it.

**Colin Matthews** (00:17:23)

Mm-hmm. Makes sense. Yeah.

**Aakash Gupta** (00:17:25)

And then we'll give this one a try. So just to show you, there's kind of two different ways to invoke apps. The first way is to just type out the name. So when I say coffee map, you'll see that it pops up automatically, that it knows that there's an app and I want to use this app. The second way is to actually tag it manually. So if I go into my apps here, I can click coffee map. And again, it comes up. And the last way, theoretically, we can give it a try afterwards, is if I don't even, if I say something alluding to it, like I want to get a coffee, where's a good location, ChatGPT may decide to use my app. And that's a lot of like where the kind of finesse comes in in terms of getting it to be better, is you want your app to show up on relevant queries.

**Colin Matthews** (00:18:00)

Yeah.

**Aakash Gupta** (00:18:00)

And so you're going to have to play with that and actually go through like an eval process, very similar to, you know, other AI tools.

**Colin Matthews** (00:18:07)

It's an eval process. Say a little bit more about that. I guess I was thinking it was almost like another AEO process. Like you need to somehow develop the reputation through queries over time that Chad GPT is feeling like you're a good tool amongst the millions of other tools trying to get called for this query.

**Aakash Gupta** (00:18:23)

Yeah, that might become the case. You know, there might even be ads for, you know, tools and stuff like that. But for now, really what it is, is like, when you type something in, is ChatGPT going to do a good job of calling your tool? And that's just based on like the very limited set of tools that even exist, right? I mean, there's less than 20 right now, different apps. How's that? And anyone can get access to publish a public tool? Yep. So right now there's no marketplace where you can kind of publish them publicly. You kind of have to be part of the launch partners. So if some of these large companies, but in the very near future, then there'll be this kind of public marketplace where you can launch your own apps directly. Very similar to what we're doing here. Okay. So right now, if you build one of

**Colin Matthews** (00:19:04)

these, you can't launch it.

**Aakash Gupta** (00:19:06)

Yeah, correct. Not to the public. I mean, you can always do what I'm doing here, right? Which is like, give someone a URL that they can play with. Yeah. But yeah, ChatDuty has said, or OpenAI has said, by the end of the year. So we're getting there. It's December now. So we'll see if that comes through or not.

**Colin Matthews** (00:19:21)

But yeah, we're on the end of the year. We're basically learning how to build for a platform that's about to become available. And so you're kind of just on the bleeding edge of the distribution of this and making a bet that OpenAI will support it. Yeah.

**Aakash Gupta** (00:19:35)

Yeah, exactly. Yeah, you got it. Cool. Cool. So yeah, here is our little coffee map. Again, you know, it's a nice little demo application. Doesn't do too much. But yeah, why don't we go ahead and build something new? So we'll flip back over to Chippy here. And yeah, any thoughts on what might be interesting? We'll give it a try.

**Colin Matthews** (00:19:52)

I feel like I want to do something in the healthcare space. Healthcare or legal? I feel like those two spaces are just like... infinite value for me on chad gpt doesn't really have anything to do with product management but i could imagine like let's say like you're a healthcare product manager i guess so if you're a healthcare product manager let's say you're a healthcare product manager at a hospital and you want to be able to give access to your customers like some information about your hospital system through chad gpt how would we think about it what would be a good unit for an app for that product manager

**Aakash Gupta** (00:20:27)

Yeah. So like actually like kind of hospital reviews and surgeon reviews are a really big thing. There's actually like SaaS companies that help, you know, hospitals and surgeons manage this because it's related to revenue. Obviously, like if you have really garbage reviews, you won't have as many customers. So maybe what we'll say is something like build a solution. that helps hospitals manage and share their Google reviews, something like this. And I'm actually going to turn on plan mode so that we can kind of see what we get back before we kick it off, just so that we don't end up building something that's completely

**Colin Matthews** (00:21:03)

unrelated. Cool. So plan mode is going to give us that thinking reasoning model that gives us the plan first before it executes.

**Aakash Gupta** (00:21:11)

Yeah, exactly. And under the hood here, I'm using Opus 4.5 for pretty much everything. So it's a brand new model that just came out like last week. The nice thing about it is that has this effort parameter that you can turn down. So you get a really high quality model. You can kind of reduce the amount of time that it spends on a task. And so for things like this, I'm using a higher quality model. So better thinking, but kind of low effort so that it doesn't spend forever like spinning its own wheels. It gets back the response pretty quickly. Yeah. Cool. So here's what we have. We've proposed three different tools to build. So one is viewing reviews, one is sharing reviews, and then one is review analytics. So we'd be able to see a dashboard of our reviews of some kind, a shareable card that we can share with other people, and then some summary stats and so on.

**Aakash Gupta** (00:21:56)

What do you think about that? Does that sound

**Colin Matthews** (00:21:58)

good? Yeah, I love it. This is what I was trying to figure out. What is the takeaway for PMs? One thing that's just kind of on my mind, though, is the PM really going to be building it? The PM is mainly probably going to create the spec for this. So this could be like, they could create their prototype here. yeah exactly

**Aakash Gupta** (00:22:14)

i think it's a little bit hard to really understand like if you're a pm how would you spec this out without ever like using one of these or even like testing how they might work

**Colin Matthews** (00:22:23)

yeah

**Aakash Gupta** (00:22:23)

so yeah i think using this as kind of like a prototyping tool is is a great use case and then in the long run i think that like there's an opportunity for solo builders to also build apps and distribute this exact same way as the ios app store right where like yeah um they'll be building their own apps So that's kind of the way I'm thinking about this platform is prototyping primarily for PMs and then like for solopreneurs or people want to build their own apps that you could do the whole end to end of like hosting your application on here as well.

**Colin Matthews** (00:22:49)

Makes sense. So there's a really big opportunity here, I think, for anybody who wants as a PM to create a side project or something like that, a portfolio project to improve their AI PM credentials. But in terms of actually coding up the prediction version of your ChatGPT app, you're probably not going to be doing that. You're going to be creating the prototype here and then your engineering team is going to take that and they're going to kind of create the real version.

**Aakash Gupta** (00:23:15)

Yeah, exactly. And actually kind of funny. So a lot of the things that you would do in a normal AI project, as we mentioned, you have to do those here as well. So things like running evals on the prompts that are triggering your tools to make sure that the right kind of phrases are triggering the right tools. And you might have to tweak the tool descriptions a little bit. to try to improve that, you know, this type of request should trigger this tool or even like have it where someone writes a request and it doesn't trigger your tools at all because it's not relevant. So you need to kind of go through the very similar process of like what you might choose to do to improve a regular AI application or AI agent you do in the same case here.

**Colin Matthews** (00:23:51)

Hmm. Makes sense.

**Aakash Gupta** (00:23:53)

Cool. So it built us our three different tools. Again, I'm going to just for fun, share a little bit about the behind the scenes here. So you can see it actually viewed some examples of code that I built in the background. So this agent that I built, what it does is it can choose to look at relevant files to kind of get inspiration for what it should be doing to build the thing that we've asked it for. And so I took a look at some kind of technical stuff, as well as a list example that kind of covers like some UI UX for lists. And then it decided to build those different tools for us. So here's a little preview, right? I don't know if I love the UX, I'll have to kind of see how it looks like in line, like when it actually has some data in it.

**Aakash Gupta** (00:24:30)

It's hard to tell when there's no data in here. But anyway, we have view reviews, we have share, nothing in there. And then we have review. And yeah, so we'll give this a try in a second. I'm wondering though, like, if this has data that's going to be passed in by the model or if it needs better mock data. So I'm going to go ahead and ask that same question. We'll say, does this rely on ChatGPT passing in the data or should we have mock data. And the nice thing about this is because the agent has like, you can think about it being like an expert in chat to PT apps. It can answer questions like this one, right? Where like maybe you're unsure about the best pattern for how this should work. You can just ask the agent, it'll kind of read through, read your code, take a look at how everything works and then make a decision for you.

**Aakash Gupta** (00:25:18)

So here it's saying that it already has some built-in mock data. And if it's using the correct pattern, that it should be passing in data from ChatGPT and then falls back to the mock data. So what I'm just going to tell it is that the mock data is not very good if there's mock data. And so I'm going to say, please improve the mock data just to get a little bit more information in here so we can take a look at these components. And then, yeah, the only other thing I'll mention while we're waiting here, this will just take a second, is you can kind of see that the UX for this building experience is a little bit different, right? So I can see each individual tool. I can also modify the parameters, but these would be the same parameters that ChatGPT would be using, right?

**Aakash Gupta** (00:25:56)

When it decides to call this tool. it's going to be passing in data for these. So it would be deciding what the filter is, what the sort is, or any other parameters that are necessary. And so, yeah, you can kind of mess around with the prompts directly in here or the parameters in order to get different UX or different experiences that might be rendered inside of ChatGPT, depending on what gets passed in.

**Colin Matthews** (00:26:16)

I'm keen to see this with the real data because then I want to actually, like you mentioned, like you gave us that teaser that really, really perked up my ears around was the evals for the prompts calling it. Cause I think that part is really interesting.

**Aakash Gupta** (00:26:29)

Cool. So we'll hop over into chat TPT and then we'll get this hooked up. So first thing we need to do is just go back over to our settings, our apps and connectors, and then create a new connector here or new app. We'll paste in the URL. Again, we'll turn off authentication for now. Just keep things simple. And we'll call this one healthcare reviews. Cool. and connect. So this will just take one second to connect and then we'll give it a try. We'll see if it works. And then after that, as mentioned, we'll go back and look at the kind of the logs. We'll create an eval really quick and see how that performs. So we're gonna spin up a new chat. You don't have to, but I just kind of don't like to see the old ones and I'm gonna tag it this time. So we'll say healthcare reviews.

**Aakash Gupta** (00:27:11)

We'll say, how are my reviews doing for St. Mercy Healthcare? And we'll see what happens here. I'm actually unsure. The tools are a little bit janky in that like that one didn't have any mock data. It didn't look like, but okay. So ChatGPT is actually generating the mock data and then filled it in. We saw for a second there. Yeah, I popped back out for some reason.

**Colin Matthews** (00:27:36)

Yeah, I swear I saw it.

**Aakash Gupta** (00:27:38)

Yeah, yeah. So I think what happened maybe is that like there was some underlying mock data that tried to override it there. Probably have to do a little bit of iteration on this one, but let's see if we can try to call one of the other ones. So let's say like, I want to share a view. And this should call the other tool, maybe, hopefully, right? So the tool that kind of generates, yeah, there you go, our reviews here. So you can see our Mercy Hospital. There's a little problem with the underlying data that you saw for a second, and then it disappeared. So you have to clean that up. But yeah, so you can see the different tool calls kind of in action. And then one last thing I'll show you is if we go back over into the connector here, We can actually see those different tool calls directly inside the connector, right?

**Aakash Gupta** (00:28:18)

So we have our review analytics tool, we have our share review tool, and we have our view reviews tool. So those three different tools that we've set up. Oh, wow. Okay. Cool. So yeah, let's go ahead and look at the other side, so the logs, and we'll kind of create a quick eval for this.

**Colin Matthews** (00:28:33)

Yes. This is like that full-stack AI product building, which is why I think this is a pretty cool portfolio or site or learning project for an EPM. It's two prompts. We spin up something. spun up something, then we're testing it. Now we're already getting to the evals process. So it's simulating a lot of the things. And some people, you know, they may not have access to building AI features in their current job, but they want to get that job building AI features. This is one way to simulate those learnings.

**Aakash Gupta** (00:29:01)

Yeah, exactly. You kind of do the whole end to end, but it's simplified, right? Like you don't have to worry about as much complexity.

**Colin Matthews** (00:29:07)

Yeah. But yeah, so we'll take a look. Worry about time in between the steps or somebody else is doing something. So

**Aakash Gupta** (00:29:12)

yeah, for sure. So we head back over to our kind of main view here. We do have an observability tab, and this will show us all the various tool calls that we have so far for our tools, right? So you can see we have the hospital reviews manager was called twice, one for view reviews and one for analytics, and then our other ones from before with our coffee guide and so on, right? If we click on this one, we can see a little bit of information about what happened. So we can see that the input was, the sort was for newest and the filter was for all. So ChatGPT is the one who decided these, right? Just to be clear, like those are parameters for the tool call. And then ChatGPT decided based on the user's request that these were the correct relevant kind of parameters.

**Aakash Gupta** (00:29:49)

And then I also stored the user prompt here. So what I typed in was I want to share a view. And we have that kind of tracked here. And this is what gives us the ability to run an eval, right? We can say like, does I want to share a review? Should that result in the tool call of view reviews or not? Is there a different tool call that would be better? We can also see some of the output data and so on and so forth. But from here, there's kind of two options that you have. So one is you can run like some quick annotations. This is really just like if you have a team of experts who you want to quickly label the data with, you can do that.

**Colin Matthews** (00:30:18)

Are you looking to land your next product management job? I am accepting a group of just 30 product managers into a 12-week cohort led by me where every Monday for 90 minutes, I help you through your job search, creating your candidate market fit. updating your LinkedIn, updating your base resume. You're going to get personalized feedback and one-on-one mentorship sessions with my co-teachers, Ankit Farmani, who is an AIPM at Atlassian and was a group product manager at Meta. Prasad Reddy, who is a CPO and has been in product for over 26 years. as well as my other live instructor, Bart Jaworski, who's gonna run another 90 minute session per week. So if you want coaching from me to land a PM job, this cohort is a no brainer. It is a premium priced product. It is more expensive than the average product out there, but the return is huge.

**Colin Matthews** (00:31:05)

Most people who join the cohort see a salary raise anywhere from 10 to $100,000 in the first year. And so the ROI will be there within a year. And we guarantee two plus interviews. So if you don't get two interviews after completing the 12-week program and following all the steps, we will refund the money to you. So it's a no-brainer. Check it out at landpmjob.com. And now back in today's episode. Before we dive deeper, let's talk about something every PM faces, getting alignment on product decisions. You know that feeling when you're trying to explain a user flow to engineering or justify a design choice to leadership and you're just describing it with your hands? That's where Mobbin comes in. Mobin is the world's largest library of real-world mobile and web app designs from industry-leading apps like Airbnb, Uber, and Pinterest. Instead of spending hours taking screenshots or hunting for inspiration, you can instantly find exactly how successful products handle onboarding, paywalls, checkout flows, Whatever you're facing.

**Colin Matthews** (00:32:03)

Over 1.7 million product builders use Mobbin to benchmark against best-in-class products and show their team's proven solutions. Whether you need to convince stakeholders there's a better way to handle user activation or research how top apps approach future discovery, Mobbin gives you the visual proof to back up your product decisions. Check out mobbin.com slash akash. That's M-O-B-B-I-N dot com slash A-A-K-A-S-H and get 20% off your first year. Today's episode is brought to you by Naya One. In tech buying, speed is survival. How fast you can get a product in front of customers decides if you will win. If it takes you nine months to buy one piece of tech, you're dead in the water. Right now, financial services are under pressure to get AI live. But in a regulated industry, the roadblocks are real. Naya One changes that. Their air-gapped, cloud-agnostic sandbox lets you find, test, and validate new AI tools much faster, from months to weeks, from stuck to shipped.

**Colin Matthews** (00:33:00)

If you're ready to accelerate AI adoption, check out Naya One at nayaone.com slash akash. That's N-A-Y-A-O-N-E dot com slash A-A-K-A-S-H.

**Aakash Gupta** (00:33:11)

And the second thing is kind of start to build up your evals or your golden set. So let's say, for example, that this was correct. We want this prompt to trigger this tool. I can add that to my set of evals. And I just click this button here and I have three different types of evals. And this comes directly from OpenAI's guidance. So there's a direct and indirect and a negative. So direct meaning that the user actually typed in the name of the product. So this would be like, Canva, can you do X for me? That'd be a direct request. Indirect would be they typed in something that's irrelevant to the tool. So what we did here, I want to share a review, right? That's not naming the tool or naming the application. And then a negative eval would be where the user types in something completely unrelated, like, I want to go shopping this weekend.

**Aakash Gupta** (00:33:50)

And if it called your tool, that'd be a bad thing, right? Because you don't want that to happen. And so in this case, we'd say that this one is an indirect. The user describes the outcome without naming the tool. And we'll go ahead and add that to our evals. Cool. And then last thing we have is the actual eval. So now we have one eval that we can run. We have this one set up as an indirect. And the way that I built this is there's two ways to run the eval. So the first way is if we open it up here, You can run it on auto. So what this does is it literally sends the same prompt and the same set of tools to an LLM and asks the LLM to decide which tool to call. And it can also decide to call no tools.

**Aakash Gupta** (00:34:24)

And so this is a very quick way to test a bunch of different prompts at the same time. You can basically run your whole eval set through auto and you'll see what will happen. And so for example, this one failed when we passed it back over to GPT-5. And we'll take a look at the reason why. So let's take a look at, cancel out of here. Okay. So when it said, I wanna share review, we had the expected of view reviews, because that's what happened inside of ChatGPT. But this is telling us that the correct tool to use probably would have been ShareReview, which makes sense. So we have these two different ones. One is called View, one is called Share. Inside of ChatTVT, what happened is it called this one. But what we would have wanted is for it to call ShareReview. And that's kind of picking up on that issue there for us automatically.

**Aakash Gupta** (00:35:04)

And so this is a good example of like, OK, in order to fix this, we have to go back into our tools and probably modify the description of the tools To be more accurate, so ChatTBT has a better idea about when to use this view reviews tool, because it accidentally used this in the case where the prompt was, I want to share a review.

**Colin Matthews** (00:35:20)

Yep. So what does that look like? Maybe we can just look at the full cycle of improving performance. Yeah,

**Aakash Gupta** (00:35:25)

absolutely. So now that we've run the eval, I'll show you one more thing in here. So that was an auto eval. The auto evals are like a great way to get a quick kind of directional input, but it's not necessarily going to match one-to-one with what ChatTBT provides. And so if you want to actually manually run your evals, you can basically build an eval set and then go through and just type in what, like type in the prompt to chat to PT. I want to share a review and just log what happened, right? So that's what this is here for is to just literally go through one at a time and log what happens with each one.

**Colin Matthews** (00:35:53)

Nice.

**Aakash Gupta** (00:35:53)

Yeah. So let's say we want to make that change. What we do is we go back into our application. our hospital reviews manager. And we can either prompt our way through this or we can just edit it manually. So in this case, I'm gonna edit manually. I'm gonna go into the config. I'm gonna find view reviews, that's my tool call. And we can see that this is the description that my LLM or my agent decided to write for this, which is display hospital reviews with filtering, sorting, and sharing options. And so what likely happened here is because it has the word sharing in the tool description, when I said I want to share a review, It decided to call this one by accident. And so we'll just get rid of the word sharing just to kind of clean that up. So say filtering and sorting options.

**Colin Matthews** (00:36:32)

So improving the metadata, if we think about it, like from like an SEO sort of standpoint, like they type in a keyword, they're using the title and the metadata to match it. Kind of ChatGPT is doing the same thing with these MCP tools it has available to it. So we're trying to give it the right metadata here. Yeah, exactly.

**Aakash Gupta** (00:36:50)

And these descriptions can be pretty verbose. I mean, there are character limits, but you can put in things like examples of how to use the tool, right? For example, I built a spreadsheet tool before and it supported formulas, but I needed to tell ChatTPT what those formulas were so that I knew how to use those formulas inside the tool, right? If it was going to be writing any data to that spreadsheet. So it's not just about necessarily SEO, it's really just like, how should ChatTPT use or behave with that tool? Makes sense. Yeah. So clean that up a little bit and then I'll probably just add something here. Like this is intended to fetch existing reviews for the purpose of showing the user it's probably not the best description but trying to get more the idea like this is not for sharing this is for retrieving information

**Colin Matthews** (00:37:40)

yep makes sense modifying that metadata to just get it called at the right time and then we're going to keep iterating on that and that's how we have this end-to-end cycler on evals and we can run those manual evals as you said so is there another category of evals then about like how effective the reviews were if we pulled the right reviews how would we write that category of evals

**Aakash Gupta** (00:38:03)

Yeah, so that's less about did the tool get called based on the prompt, but more around did the user get the expected result or was the behavior good? Yeah. So very similarly, if we go back over into our observability, we can take a look at the logs. And that's really the best way to get a good idea of what's happening is we can see, again, what the user requested, what tool got called, and then what some of the data was that basically got filled in. And using these logs, we can kind of get an idea for what happened. Again, you kind of have to have more context on reading through these logs. What did you want to happen? And it's the same thing with any type of eval, right? You have to have an idea of what ground truth is. What do we want to occur when a user types something in?

**Aakash Gupta** (00:38:44)

And so again, you kind of look at this data to get a feel for what did happen. But separately from that, you'll have to decide what you wanted to happen in whatever case.

**Colin Matthews** (00:38:53)

This is kind of expanding my conception around what a good AI prototype is, you know? I think some people might have the tendency to want to, like, ship the AI prototype when we did right at the beginning. Like, all right, two prompts in, good to go. Let's ship it. You know, we had our initial prompt. We changed it to add in some dummy data. Good to go. Let's see it. But it seems like actually going through this eval process along the major categories of evals. Here, the major category was like discoverability and then good result, tweaking it and improving it. This is going to help you really understand the corner edge cases, like some of the things we used to have in a deeper PRD, help you understand what's going to move the needle in this feature success or not.

**Aakash Gupta** (00:39:33)

Yeah, and a lot of these things, honestly, you can't really necessarily predict how is ChatGPT going to interpret the way that you wrote your tool description, right? And so you could spend a very long time trying to figure out what the best thing is, but really you should just test it and run evals against it and see what works rather than thinking about it for a long time. And so I totally agree. Getting into the process of this type of iteration provides a lot more information than thinking about it or like, you know, writing it in a purity and then handing off the engineering team, because eventually your team's going to go through this iteration anyway. It's just a matter of like, are you getting through some of that on your own quickly? Or, you know, you can obviously bring in your counterparts, but you have a mechanism to do it quickly versus like the full handoff between teams back and forth, back and forth.

**Aakash Gupta** (00:40:17)

Right. I wish can take like weeks or months or even longer. Yeah.

**Colin Matthews** (00:40:19)

Thank you so much. talking to partners, looking at user and business data, identifying opportunities and threats, setting goals, evaluating ideas. Sometimes I wonder, like, are we just endlessly expanding the PM role? What is the right way to think about the prioritization of this work that we've been going over so far versus some of the other work that Itamar has listed here?

**Aakash Gupta** (00:40:58)

Yeah. So I think to start, just skip on the ChatGPT app side of things and just address this first. I think it's a skill the same way that like a PM who knows how to use Figma is probably more useful in certain contexts, such as like talking to design stakeholders, or even like spitting something up really quick to show to a customer or someone like that. Like you're not dependent on other people to do every single kind of touch pointer element for you. And so I wouldn't say that like using Figma should be an extra line item in here. Using Figma is a skill that supports talking to customers and talking to stakeholders. You know what I mean? So it's not, they're not independent things. It is, yes, these are the responsibilities of a PM. And then they have a way to do that. Like the same way that talking to customers involves some type of skill around interviewing and they needed to learn that skill, right?

**Aakash Gupta** (00:41:46)

Talking to stakeholders involves a lot of skill around like stakeholder management and, you know, even managing up and stuff like that. I would say using some of these tools is complimentary. So I personally wouldn't advocate for like AI prototyping to be an extra line item or vibe coding to be an extra line item on here. I think these are tools that we can use to support these ideas or these kinds of tasks. And that to me, at least it's obvious that if it's very difficult for you to visually communicate something, that that's a great use case for AI prototyping. Like if I want to kind of explain, hey, this is how I think our AI product should work. You know, I'm building some type of agent that's going to do some task. It could be hard for me to kind of explain that to my stakeholders or to my customers.

**Aakash Gupta** (00:42:25)

And so spinning up a quick prototype in whatever prototyping tool you like is an easy way for me to start to have that conversation and improve the fidelity of the information that I'm sharing. I can be like, this is kind of what I was thinking. Is this a resonate? And so that's to me how I would kind of, I guess, have a rebuttal to this is it's not an extra line item. Vibe coding is not something a PM should do for no purpose. It should be related to some reason that they're building that prototype.

**Colin Matthews** (00:42:51)

So AI prototyping enhances some of the activities on this list is the way you should think about it. And you shouldn't necessarily think about not doing this stuff on this list. This stuff is important. But how can AI prototyping help you do some of this stuff better?

**Aakash Gupta** (00:43:06)

Yeah, exactly. And this isn't really new. Like PMs have been trying to brainstorm and communicate ideas forever, right? So like Balsamic was popular for a long time. It's the same thing, right? It's just like helping someone who's not a designer communicate something visually to get the idea out of their head and kind of like onto some form of paper that people can see. And so, yeah, I would say it's literally for the exact same purpose. And so, again, if someone's vibe coding first, like if you're a PM and you don't have these other skills and the only thing you know how to do is vibe coding, I don't think that that will be like a way to be super successful in the long run. Maybe there's like some short term game because it's popular at the moment, but these skills are super critical. And vibe coding can support some of those or AI prototyping can support some of those.

**Aakash Gupta** (00:43:49)

Amazing. So I

**Colin Matthews** (00:43:49)

want to do some mind mapping together. What are the benefits for creating a chat GPT app for your product? What would you put those major groups as?

**Aakash Gupta** (00:44:01)

Yeah, I think we'll kind of classify this into two categories. I think there's some benefits from like the perspective of learning how to like build agents basically or build tools that agents are interacting with. So there's kind of like a career benefit or a skills benefit for an individual person, right? A PM, a designer, an engineer. that that's one kind of classification i think the main one is enterprise focused to be honest i think the vast majority of early adopters of this is actually going to be large enterprises not small companies and the main thing is getting clicks or views it's basically growth right so i want people to see my app see my product and chat tpt has hundreds of millions of active users per week and the intent when a user comes from chat is higher than the intent when they come in from seo or another channel And so every company on Earth, given like the proper tools to capitalize on that, will do so, I think.

**Aakash Gupta** (00:44:54)

And so I think that's really like the main benefit is what is the right form factor for us to get in front of customers, get in front of users and help them interact with our brand, interact with our company so that we can kind of pull them into our ecosystem.

**Colin Matthews** (00:45:07)

All right. And then the next part of this mind map I want to understand is who should be building a ChatGPT app? How would you create the major buckets or like, if I'm a PM, how should I understand if I should be?

**Aakash Gupta** (00:45:17)

Yeah. So in a typical enterprise setting, like we think about the Canva app or, you know, any of the ones that exist today, I would expect it to be like a pod, to be honest. So you'll probably have a designer who needs to understand, like, what are the form factors? And it's actually, for a designer, I think an exciting place because It's very unique. You have these kind of like little micro apps that you can build, and each one can do a very small amount of things. You can build more than one if you want to. They can communicate back and forth. So yeah, understanding the form factor is pretty critical. The second to that would be the engineering team. So like, how do we actually ship this thing? There's a couple of technical complexities, like authentication is very complicated as compared to regular authentication. So you need to make sure you get that right.

**Aakash Gupta** (00:45:57)

And so engineering is going to figure out like, how do we actually get this into the world? You know, how do we support these different types of tool calls that are coming in? And then lastly, it would be the PM. And like, as a PM, the reason I might choose to do this, like, what is the kind of guiding light? It is growth, right? I would decide, like, is a ChatGPT app a good method for us to drive, you know, higher conversions from AI, basically AI search or AI, you know, chat. And maybe this is a priority that we have that like, we want to capture more market from, you know, open AI from that type of search. And so the PM would prioritize this as, you know, something that is relevant. And then we'll also hopefully be involved in this process of like building evals, you know, shipping small incremental changes to the application, understanding how users are using that application and then sharing back with anyone who cares about it internally, what's happening with that application.

**Aakash Gupta** (00:46:48)

So it's really like, it's kind of its own, form factor of software it's not like it belongs to one persona or group in my mind it would be a pod and then they're going to ship this together and each one should have some skill kind of around this new form factor so if you're a pm deciding whether this is an important opportunity how do you decide that i think for now it is like definitely uh give it a try first of all so that you have some familiarity with like what the options are so building you know full screen applications how that differs from building like just a quick inline card And then the second thing I would say is really like pay attention to what other people are doing. So, you know, larger companies like Target and Uber bringing kind of incoming into the space when you interact with chat to BT, like is it pulling up Target for you?

**Aakash Gupta** (00:47:34)

Is it pulling up Uber for you? Is it pulling up Coursera for you? And if it is, you can see it happening like in real time, like what the benefit is of having these apps. um and then lastly the thing i would think about is like is this an opportunity to re-engage customers off of your product so for example if x percent of your customers are using chat cpt they might not be logging into your application like coursera but they could be using your kind of micro app right and still getting benefit from your product and still feeling like they're connected to your product and so i think there might be a kind of a value out here around you kind of think about like retention right you'd have to think about how it affects retention a little bit more but something around that space but of consumers or users interacting with your brand and your product without necessarily having to go directly into your app experience makes sense

**Colin Matthews** (00:48:19)

all right i think i can play with that arrow infinitely so we got a little bit of this package here of chat gpt app if you're building it for an existing product here right on the right now i want to go to the other side on the left and talk about what are the good chat gpt app ideas to build if you are a cell opener or a side project person

**Aakash Gupta** (00:48:40)

Yeah, I think so to start with, I would start thinking about like unique ways that ChatGPT can interact with your application. So we saw a brief demo of that here. You know, we had a little bit of data issue in the background, but ChatGPT actually can fill in the data for you. Right. So it is the one who's deciding what to call your tool with. And so a good example of this, I'll kind of go back to what I referred to earlier. is a spreadsheet application where ChatDBT kind of partner with me on it. So for example, a spreadsheet app that has financial modeling support, some person drops in some financial data into ChatDBT and says like, hey, can you help me model this? And it pulls up the spreadsheet app, puts in the relevant formulas, generates some nice charts and graphs, all that kind of stuff that's deterministic so the user can go back and actually change the data in the spreadsheet and say like, oh, you got that number wrong.

**Aakash Gupta** (00:49:28)

Let me just quickly fix it. That'd be a small example of like, a utility or an application that is embedded with ChatGPT. It's not just like showing you stuff. It's not a search tool actually has the ability to collaborate directly with ChatGPT in some form factor, like a spreadsheet or a task list or a whiteboard or whatever, right? Like you can imagine this ChatTBT that has memory of you and knows you really well and has access to all the tools that you want to use, then you don't need to hop into like Miro or Google Sheets. Like you can do a lot of work very quickly directly with these embedded applications. So I think there's a lot of like potential for these types of embedded apps to kind of take over smaller use cases of like where ChatTBT kind of falls short right now. But it'd be useful for ChatTBT to help you with these types of tasks.

**Colin Matthews** (00:50:14)

Okay, so maybe like a domain that ChadGBT is interesting in, like healthcare or legal or productivity or writing, but maybe a use case within that that's neglected.

**Aakash Gupta** (00:50:25)

Yeah, exactly. Yeah, yeah. And, you know, you can think about like any example you can find out in the world where there is an AI company building a product for this. So another good example, this is Gamma. So Gamma is a very large company building a presentation tool, an AI presentation tool. Theoretically, we could build a ChatGPT app that also makes presentations. And so you could provide a really great experience in building presentation or software inside of ChatGPT. You maybe won't be as good as Gamma. I expect probably not. But you also don't have to be. You just have to be good enough that it is a good alternative that someone who's already inside ChatGPT goes like, oh, yeah, this presentation is a good starting point. Right. And so really like the strength of the distribution with these kind of embedded applications is what I think will kind of win the day there.

**Colin Matthews** (00:51:12)

Yeah. Anything that might benefit from embedded distribution? What else? It seems like there was a lot of like e-commerce examples, right? Yeah,

**Aakash Gupta** (00:51:19)

I think. Well, I mean, there's a ton of work going on right now in terms of like shopping. Right. So I think it'll be pretty common that people like Target or, you know, you know, other kind of consumer facing companies want to be in this space if people are searching for products inside of ChatCPT. Right. And so they want you to be able to build a cart. They want to be able to check out because they want to be in front of you the same way that they're in front of you on Google or any other, any other product like, you know, so on. It'll be interesting to see if Amazon does this because like Amazon has their own LLM activities going on. But I think Amazon would be an obvious example of like, can you imagine just hop in chat to BT, you say like, hey, reorder me the Thursday order.

**Aakash Gupta** (00:51:56)

It fills out your cart for you from like whatever you ordered last Thursday or whatever you currently get. And then you just buy it. Like there's a lot of good examples in the e-commerce space that I think would be consumer friendly.

**Colin Matthews** (00:52:06)

And then we saw Figma and Canva in there. So I guess those are like if you have any sort of media or content creation tool, right?

**Aakash Gupta** (00:52:12)

Yeah, these are still early days. So I think Canva is the best example from a functionality perspective, so I'd encourage you to give it a try. But basically, the idea here is you can use some kind of mini version of the Canva app directly inside of ChatGPT. So it's more fully featured than just showing you information. You can actually interact with the application, move stuff around, like I said, a mini version of Canva. And again, like you're reliant on Chattaputee to like help you do that. So rather than me, you know, clicking through everything or all that, like I'd use Chattaputee as an agent that understands Canva. And so in some ways, like we're moving towards a future where Chattaputee is like this operating system more. It's like the universal agent. And then these are all different applications that I can call or use as needed rather than every company building their own agents.

**Colin Matthews** (00:52:59)

Yeah. And all this is built on MCP. So theoretically, if Claude or Gemini win, they could also pull into these? Or what about that?

**Aakash Gupta** (00:53:07)

Yeah, exactly. So this is probably the best part, kind of icing on the cake to some degree, is that this started as an open AI initiative, this kind of like apps inside of chat. But using MCP, which Anthropic is responsible for, they pretty quickly amended the MCP kind of protocol or standards. So now Claude actually is like today working on the same thing. You can see screenshots of it if you look around on Twitter or LinkedIn. of the team sharing how these apps are going to work inside of Claude. And so you're not just building for one distribution channel. You're actually building for any distribution channel that supports MCP, which right now primarily is Claude in ChatGPT. But Lovable actually supports MCP. Cursor supports MCP. There's a lot of tooling that supports MCP already. Gemini does not, interestingly enough. But maybe they will at some point in time.

**Aakash Gupta** (00:53:58)

Maybe it's just not the focus. But yeah, I think that like there is a potential future here where you can get yourself plugged into multiple different chat applications through one app that you've built on top of MCP.

**Colin Matthews** (00:54:10)

Okay. So it currently isn't in Gemini. So that is one sort of downside here, but it is in Claude. They're working on it. It's not released yet. Maybe by

**Aakash Gupta** (00:54:18)

the time the podcast goes live, it will be. But yeah, there's basically like, you know, the engineering builds of it. They're working on it. It has been approved. Like it's part of the MCP spec. It just needs to go through like the actual development process at this point of time.

**Colin Matthews** (00:54:30)

Okay. Is there anything else people need to know or add to this mind map to get a good understanding of chat GPT apps? I think this

**Aakash Gupta** (00:54:37)

is pretty, pretty comprehensive. Obviously, like as we talked today, it's, it's still early days. I think maybe that's, that's the last thing I'll mention is I don't want to try to hype it up too much. Like, It's a cool form factor. It gives you a great experience in terms of like testing and building AI apps without having all the infrastructure yourself. So it's a great way to learn. But obviously there's only like less than a dozen companies that are currently partnered with ChatGPT. And so I think a lot of this is going to depend on OpenAI's ability to execute like can they actually get this marketplace over the line you know do people start to use these apps what does the discovery experience really feel like and look like and so yeah just I guess with a grain of salt I'm super excited about this space obviously I think there's a ton of potential but it does depend on kind of a couple of things getting across the finish line but I'd say we're like 70 to 80 percent of the way there and I would guess by March like we'll know one way or the other if this is the case

**Colin Matthews** (00:55:29)

So I think this is what you're highlighting, that critical PM skill. Is this an important opportunity? That's what you guys all need to think about for yourself in your unique situation. That is our masterclass on ChadGPT apps for PMs, hopefully the best guide on YouTube that you have seen yet. Colin, I want to talk a little bit about you because you're one of the most interesting men in the PM content tech space. You just finished a year as a solopreneur. So you were a PM for a long time. We all know you have very highly ranked on the Maven leaderboard. So that could be one thing you did with all your time, I imagine, and you'd be financially fine. But you didn't really stop there. You did some experiments this year. You launched a podcast. You launched a couple of SaaS apps. This, obviously, Chippy, you built.

**Colin Matthews** (00:56:13)

What is the pie chart of Colin's time and attention and focus these days?

**Aakash Gupta** (00:56:19)

Yeah, so as mentioned, one year, almost like maybe a week ago, two weeks ago, which is really exciting because I've actually wanted to work for myself for literally my entire career. So a dream come true for me. But yeah, in terms of time and attention, I would say it's like, maybe 40-ish percent keeping the whole thing running. And I have some help with that, which is great. My wife actually helps me a ton with operations. I have a TA named Paulo who helps me with some of the core stuff. And so I have some support with that. And then the other 60-ish, maybe 50% of my time is spent on new bets. And when I think about bets now, it's actually changed over time. So partially it's like, is this going to work commercially? And then the second part is like, do I actually want to do it?

**Aakash Gupta** (00:57:01)

And sometimes I don't know if I want to do it until I try. So podcast is a good example of that. I tried podcasting for a bit. I think I was creating interesting things. But the thing I think about is, am I going to be in the top 5% to 10% of this thing? And if I'm not, I kind of drop it and I think of something else that I want to do. And so for podcasting, I don't think I'm going to be in the top 5% or 10%. Maybe I'll come back to it one day. But for now, it's not really a bet that I have the same amount of conviction about. And so, yeah, I tried podcasting for a bit. I've built like probably four or five different SaaS apps this year. This is actually my second AI prototyping tool that I built, like my own prototyping tool.

**Aakash Gupta** (00:57:37)

This one obviously catered to this use case, but I built one earlier in the year as well. A lot of learning, like obviously knowing how to build these tools takes a little bit of time. So like learning how to build agents, learning how to like run these systems. And, yeah, like, I don't know, testing other stuff, to be honest. Like, I spent time this year on a RAG app for a little while that I built from scratch. What else? I don't know, a bunch of different stuff. I just try different stuff. Obviously, I have a sub stack. So it's been a little bit scattered, to be honest, which I don't like. But it is nice to try different things, fail quickly and then move on rather than just like doing the one thing forever. And I think I know you didn't ask this, but my kind of end goal is to have a software product and continue teaching and kind of like balance those two things.

**Aakash Gupta** (00:58:24)

But I'd love to have like a software product that's that's super cool, that's valuable that people want to use. So that's that's what I'm trying to shoot for at this time.

**Colin Matthews** (00:58:32)

Got it. So you're like a Mark Louvian plus course instructor. Sure. Something like

**Aakash Gupta** (00:58:37)

that. Yeah. I just mess around with stuff a lot. I write about stuff when I find it interesting mostly. And then that's pretty much it. I do have to get better at marketing. This isn't a side, but just being transparent. That's like one muscle that in the next year I'm hoping that I improve on because my marketing activities are very haphazard at the moment. And so I need to get more consistent at marketing and just showing up so people know I exist. But yeah.

**Colin Matthews** (00:58:59)

And what's your stack for building these SaaS apps? How did you build the app we just saw today?

**Aakash Gupta** (00:59:04)

Yeah, actually, this might be really interesting for you all. I built the UX entirely on Replit. So like the Gemini 3, the new design mode they released recently.

**Colin Matthews** (00:59:15)

But in

**Aakash Gupta** (00:59:15)

terms of like actually shipping stuff, so I use ES Code and Cloud Code for the vast majority of like CodeGen. I'm obviously using Git for like version control. I use a database provider called Neon. I use a hosting platform called Render, and then lots of different libraries depending on what I'm doing, right? So like for the reg app that I built, reg is a whole world on its own that's kind of complicated and hard to optimize. And so like I was using this vendor called Voyage for the embedding models and different vendors for different things. So like you end up with this whole stack of like random stuff that you learn about and try to build and then, you know, maybe it works, maybe it doesn't. But anyway, My core tools are like Cloud Code, VS Code, GitHub, and Render for building stuff.

**Colin Matthews** (00:59:57)

Why VS Code and not Cursor?

**Aakash Gupta** (00:59:59)

Yeah, so I don't use Cursor. I use Cloud Code predominantly. I use the Codex tool as well sometimes. And I just find the integration inside of VS Code is a little bit nicer for those tools than it is inside of Cursor. Cursor has its own AI, obviously, and it tries to use that AI, and I don't want to. I don't want to use Cloud Code or Codex. And so, yeah, I don't really use Cursor. I find Cursor at times kind of tempts me back because they release new features. So for example, they release embedded websites. So you can interact with whatever you're building inside of Cursor, and the AI has some context on it, can actually debug for you. But more often than not, those things don't really move the needle for me. What really moves the needle is quality of code gen. That's like 95% of what I need and care about.

**Aakash Gupta** (01:00:38)

And all the other stuff is just bells and whistles. And so right now for me, Cloud Code is like the highest quality code gen with the fastest pace. And so I just, that's like my daily driver.

**Colin Matthews** (01:00:48)

Fascinating stuff, man. We're going to have to have you back again. Maybe you can show us this stack of how people can build stuff. I'm sure there's a million different other episode ideas we could come up with. You guys leave a comment below. Should we have Colin back on for a third episode? By the way, for those who don't know, he used to have our number one episode of all time when he did our top five AI prototyping tools. Since then, we've managed to release some episodes better. Thank God for us as a podcasting team. But hopefully we can break the records with this one. Drop a comment below what you liked about this episode, whether we should have Colin back on. Colin, thank you so much for dropping all this sauce.

**Aakash Gupta** (01:01:22)

Yeah.

**Colin Matthews** (01:01:23)

Yeah. Happy to hear it. All right, everyone. See you later. I hope you enjoyed that episode. If you could take a moment to double check that you have followed on Apple and Spotify podcasts, subscribed on YouTube, left a rating or review on Apple or Spotify and commented on YouTube, all these things will help the algorithm distribute the show to more and more people. As we distribute the show to more people, we can grow the show, improve the quality of the content and the production to get you better insights to stay ahead in your career. Finally, do check out my bundle at bundle.akashg.com to get access to nine AI products for an entire year for free. This includes Dovetail, Mobbin, Linear, Reforge Build, Descript, and many other amazing tools that will help you as an AI product manager or builder succeed. I'll see you in the next episode.
