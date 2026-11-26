---
title: "Bolt Tutorial from the CEO: We Live Build a Remote Job board"
subtitle: "Well, this is crazy at this point! Eric Simons LIVE shares how to build a full-stack remote job board with Bolt handling the UI, backend, debugging, and more. No setup. No engineers. Just prompting."
date: "2025-03-25"
host: "Aakash Gupta"
guests: ["Eric Simons (Bolt CEO)"]
speaker_names: "substack"
substack_url: "https://www.news.aakashg.com/p/bolt-tutorial-from-the-ceo-we-live"
youtube_url: "https://www.youtube.com/watch?v=FE20SlPGSMw"
duration: "01:08:33"
word_count: 11955
source: "Substack episode transcript (aired audio)"
sponsors:
  - name: "Maven"
    url: "http://maven.com/x/aakash"
  - name: "GibsonAI"
    url: "http://www.gibsonai.com/aakash"
  - name: "Amplitude"
    url: "https://bit.ly/4hl25RG"
---

**Sponsors:** This episode is brought to you by [Maven](http://maven.com/x/aakash), [GibsonAI](http://www.gibsonai.com/aakash) and [Amplitude](https://bit.ly/4hl25RG).

# Bolt Tutorial from the CEO: We Live Build a Remote Job board

*Well, this is crazy at this point! Eric Simons LIVE shares how to build a full-stack remote job board with Bolt handling the UI, backend, debugging, and more. No setup. No engineers. Just prompting.*

**Aakash Gupta** (00:00:00)

Eric, we've been hearing so much about how quickly Bolt is growing. Can you share with us the latest on how ARR has been going since your launch in October?

**Eric Simons (Bolt CEO)** (00:00:14)

Yeah, it's continued to grow like a weed. In the first two months, we went from zero to 20 million of ARR. And since then, we've just about doubled it. So we're closing it on 40 million of ARR at this point. And I think we're about to pass like 4 million registered users. It's continuing to just keep growing like a weed. At this point, we have 70, 80,000 active customers using the product. And our team is still like 20 people.

**Aakash Gupta** (00:00:38)

Your new Figma integration, because a lot of people listening, especially, they might be product managers or designers. They might be living a lot of their lives in Figma. How can you go from Figma design to working prototype with Bolt?

**Eric Simons (Bolt CEO)** (00:00:52)

Basically, we've worked on this. There's this company called Anima that's, for the past, I think, like seven years, they've been making the number one Figma plugin for, like, turning a Figma design into code.

**Aakash Gupta** (00:01:01)

So you're busy. Everyone watching is busy. I want to go straight into a live cooking session with Bolt. People can see how the creator uses it. Can we build something together? Yeah, let's do it. I would love the opportunity to do that. So everyone knows Levels.io. He's like the most famous indie builder, maybe before yourself. And he built a remote job board and it's doing crazy well for him. It was like his first really successful product. So let's try to build that in bold. Can we build something together?

**Eric Simons (Bolt CEO)** (00:01:38)

Yeah, let's do it. I would love the opportunity to do that because I don't often get opportunities to sit down for like an hour and build some cool stuff with Bolt just with all the insanity going on. So heck yeah, let's do it.

**Aakash Gupta** (00:01:54)

All right. So everyone knows Levels.io. He's like the most famous indie builder maybe before yourself. And he... built a remote job board and it's doing crazy well for him. It was like his first really successful product. So let's try to build that in bold.

**Eric Simons (Bolt CEO)** (00:02:13)

Yeah, that sounds good. I'm in here. I can share my screen. I'm going to pull a bolt here and do. Okay. So here's Bolt. And okay, so we want to make a job board. Yeah. And I think levels is, it is like called like Nomad List, right?

**Aakash Gupta** (00:02:35)

Yep, he has Nomad List and Remote OK. So we're going to do more on the lines of Remote OK. Right, okay,

**Eric Simons (Bolt CEO)** (00:02:41)

right, right, right. Okay, so I want to make a job board app for remote job seekers, similar to Remote OK from levels. but ideally better and more beautiful. Levels is cool, but I think he'll be proud if we make something even more amazing for end users. Do we have any specific... Anything else we should feed to the LLM here?

**Aakash Gupta** (00:03:18)

So the growth strategy for him is not being beautiful or anything like that. He has two... things right so he's really well integrated with SEO so if you search like remote product manager his page shows up and he's good at monetizing where people who want to share their job are paying to be listed higher so I think those are probably the two things we eventually want to build into this

**Eric Simons (Bolt CEO)** (00:03:45)

Okay. Love it. Um, okay. So basically, uh, okay. So maybe not as not beautiful. I'll leave it. Um, okay. So the, the, the two things, two things that will make this app super successful. Um, I'm really curious to see what this fits back out of, out of the vibes we're kind of throwing it. Um, one, um, SEO presence, um, feasible presence. Is that it? So it'll know what I'm saying. So each job can be directly linkable slash indexed by Google to the ability for promoted job

<!-- sponsor -->
**Aakash Gupta** (00:04:30)

Today's episode is brought to To help you out, I've put together a collection of courses I recommend at maven.com slash x slash Akash. This includes courses like AI prototyping for PMs, product sense for PMs, and getting an AI PM certification. Visit it now. Today's episode is brought to you by Gibson AI, the future of backend development. Imagine designing, deploying and scaling your database as effortlessly as having a conversation. With Gibson AI, that's now a reality. Gibson AI is your AI-powered database engineer. In just minutes, you can chat with Gibson to create production-grade data models, deploy them on Gibson's cloud infrastructure and instantly generate secure REST APIs. Connect your front end directly to your Gibson built database or drop the API specs into Cursor, V0, or Bolt to build a full stack application seamlessly. From idea stage to millions of users, Gibson scales with you. Gibson optimizes your database as you grow and enables easy schema updates and migrations.

<!-- sponsor -->
**Aakash Gupta** (00:05:56)

So head over to gibsonai.com slash Akash.

**Eric Simons (Bolt CEO)** (00:05:59)

Listings. IE Modestation.

**Eric Simons (Bolt CEO)** (00:06:06)

All right, let's see what this thing spits back, yeah? Sounds good. Okay, I'm curious. I have a lot of fun. Like when I feel like that's, that's something that like when, you know, we very, very may well get back something that's like not right and kind of weird. And that's, I like doing that. Even if that's the case, because you kind of get a feel of like, okay, how can I, it's like talking to like a pro coworker, right. Where with certain like coworkers or collaborators, you kind of like, you'll get to a point where you kind of like talk to them in a way where you can, you know, just kind of literally like say things that are just kind of like vibes, but they like understand it and they can like turn that into something actionable. I think that for me, like working with bolt and just like any AI chat based product, it's like, I always try and find that where it's like, how can this thing and I be kind of on the same page?

**Eric Simons (Bolt CEO)** (00:06:58)

Cause then in the future, a lot of things I can just, instead of being super verbose, verbose about stuff, I can just go and say, Hey, like, here's, this is kind of like what I'm looking for or whatever have you. Right. Um, And it looks like, so I'm going to need to connect Supabase. I think that's why this error might be popping up. So that's kind of a cool thing about Bolt is that we've got integrations with deployment providers and database providers built directly into the product. And so this actually spun up Supabase stuff for us. And so what I can go ahead and do here is just say, connect to Supabase. And I'll go ahead and just create a new project here with Supabase. And so I'll say, this is my job board. it a little password and go and just create new project and i'll go ahead and spin that thing up um

**Aakash Gupta** (00:07:45)

yeah so um and for people who don't know supabase is how we're going to be building a database into this right

**Eric Simons (Bolt CEO)** (00:07:53)

yep exactly exactly so basically for like all the authentication that we're gonna need to do um actually storing the files, right? Sorry, storing the job listings, you know, so that they can be retrieved and rendered and all that good stuff. That's effectively what we're, you know, why we need to use Superbase for the backend of this thing. Let's see where this thing ends up.

**Eric Simons (Bolt CEO)** (00:08:15)

Do, do, do, do.

**Aakash Gupta** (00:08:19)

And behind the scenes here, is this 3.5 Sonnet, 3.7 Sonnet? What's working behind the scenes?

**Eric Simons (Bolt CEO)** (00:08:25)

Yep. So we're using multiple different models at this point for Bolt. So we use 3.7, we use 3.5. We also use like new Gemini models. We also use, you know, other types of models. And so that's like, you know, when we first started, it was like very heavily based on 3.5. But as we continue to add more and more functionality, you know, we've expanded the different models we're using simply by because it allows you to do more and more things and have a better and better experience. That's kind of one of the cool things about Bolt is like, we've got like the integration of the, cause what's running under the hood here, right? This is like what we spent seven years of this company doing was it's very, very small. When you look at it, this is like a full operating system running inside of your browser here, right?

**Eric Simons (Bolt CEO)** (00:09:08)

It's not like running on a server. So you're not having to pay by the minute to use it, et cetera. It's extremely fast. It's very reliable. And so when it's actually the AI agent is actually interacting with this, There's no latency and it has full access to everything that's going on, including different errors that are happening. And you kind of saw it click, just said, hey, fix the error. And it's kind of clicked through and figured out what to do. And we actually have like a working application over here now that we can start iterating on, right? And so it's called Remote Hub. What do we think of that name of this thing? Yeah,

**Aakash Gupta** (00:09:42)

it's good with words usually.

**Eric Simons (Bolt CEO)** (00:09:46)

Yeah, totally. Totally. So we can say post a new job. And so out of the box, I don't really like these input fields. So one thing that's cool about Bold is we actually recently added vision capabilities because a lot of times you're like prompting these AI tools and it's like, hey, that button over there, make it better. What's cool is we actually have the ability for the agent to see what you're seeing. So if you actually click this button over here, you can actually choose the part of the application that you want to look at for you. And so I can just go ahead and click on this input and say, yeah, the form fields are pretty cramped. Add some padding, make them pretty. And just hit enter. You'll go ahead and get to work on that.

**Aakash Gupta** (00:10:35)

And like a good colleague, you don't need to like necessarily give it all the specifics. It's going to go out and make some decisions for you. Exactly, exactly.

**Eric Simons (Bolt CEO)** (00:10:45)

And you can also like write up PRDs, right? And just kind of post it in and it can go and just rip through those as well. And so it kind of depends on what you're looking to do, right? Like if you're looking to, you know, really take an application that you've like scoped and designed in Figma and et cetera, it's like, you know, what we're doing here, this is like pure vibe coding. Um, but if you really wanted to like, uh, you know, build something that's like very meticulous, um, it's totally capable of doing that as well. Um, we actually just today launched an integration with Figma where you can just like turn Figma designs into full stack apps, like pixel, you know, pixel perfect, um, over into bolt. Um, And so here, so now you can see we have more padding, et cetera. But just really simply kind of point and shoot at what you want to do.

**Eric Simons (Bolt CEO)** (00:11:31)

And so I'm curious if it's going to let me actually post this job. I'll go ahead and put my own job up for sale here. And I'll say it's remote. Good luck getting this

**Aakash Gupta** (00:11:42)

one, folks.

**Eric Simons (Bolt CEO)** (00:11:43)

Run the company. Minimum salary, a buck. Maximum salary, two bucks. Bolt.new. Company logo URL, let me go ahead and find our logo on the internet here.

**Eric Simons (Bolt CEO)** (00:11:57)

Yeah, what's

**Aakash Gupta** (00:12:00)

this

**Eric Simons (Bolt CEO)** (00:12:01)

one?

**Aakash Gupta** (00:12:02)

image address. It's funny you mentioned the PRDs. When Colin demoed this on our channel, Bolt, he had Bolt write a PRD for itself as the first step.

**Eric Simons (Bolt CEO)** (00:12:15)

A lot of people, that's not an uncommon approach, actually, for people that are heavily using the tool. I think that's kind of the cool thing about Bolt. There's a clear path for power users to meaningfully improve the experience for them by having it write PRDs. You can have it write markdown files in the code base. So it's like, remember certain things that you think are important or whatever. But yeah, I need to add HTTPS

**Eric Simons (Bolt CEO)** (00:12:43)

probably.

**Eric Simons (Bolt CEO)** (00:12:45)

Okay. So I was like, I don't think I should be able to do this because I'm not logged in. And so that's kind of exactly what's going on here. So, you know, let me see, we can just hit attempt fix and let's see if it figures out that we need to log in. It probably does actually need that. But we will certainly want to allow people to sign up and log in and that sort of thing for this product. So once this thing's done, going ahead and doing those migrations, I will go ahead and tell it to add some login.

**Aakash Gupta** (00:13:21)

I think we both have done some software engineering. It's kind of mind blowing to just hit attempt fix. You're not like even thinking about what is the problem or how to solve it.

**Eric Simons (Bolt CEO)** (00:13:31)

Totally. Totally. It's, it's, it's really cool. And we actually just added like reasoning, um, into, uh, the product to the debugging experience. So it's actually like thinking very hard about it. Um, so let me say like, um, add a way to, to register and log in. Um, So when you actually hit a time fix, it's now actually going and you're spending a significant amount of inference to actually think through the problem. and can actually go and perform searches on the internet, pull in content and documentation, whatever have you, right? Because a lot of times these things are like the LLMs themselves are out of date. It just might be confused. And so if you look at how developers do debugging, it's often they're thinking hard about it. They're going into a Google search. They're reading some documentation. And so that's kind of the funny thing about building this sort of product is I feel like the developers on our team were just okay, how do we do this?

**Eric Simons (Bolt CEO)** (00:14:27)

And then how do we, how do we turn that into something that's like kind of deterministic that you can, that you can do, you know? So anyway, so it's kind of, kind of fun. Let's see what error popped up here. Okay.

**Eric Simons (Bolt CEO)** (00:14:40)

Let me see. Do, do, do, do. I think we might

**Eric Simons (Bolt CEO)** (00:14:46)

be able to actually get rid of that one. Just ignore it. But let's go ahead and try and create an account. So I'm going to sign up. Eric at stackwoods.com. use the most secure password in the world, which is password. And I'm signed up. So now I can actually go ahead and sign in. Chrome actually just gave me an alert. It was like, yeah, that's not a safe password. Are you sure? Yes, I'm positive. I'm positive. Look at that. We're now logged in here. We have authentication. I think this is, to me, so cool because normally when you do this sort of thing, if you had to write this from scratch, doing something even just like authentication is a pretty big lift, right? um and so now we actually have a real you know off and sign in flow here and actually one thing that's cool is um if we want to preview this in another tab we can actually kind of get the uh the full experience um i'd say this like you know in full screen or whatever have you but um

**Aakash Gupta** (00:15:48)

so much easier from october because i feel like when i first tried this late last year it took a little bit longer to get authentication in

**Eric Simons (Bolt CEO)** (00:15:55)

Yes. Yeah. So, so that's, that's actually been a big thing. Like our integration with Superbase has been one of the main things that we've been working and landing. And this is actually like in the next two weeks, like next week in the week after we're rolling out kind of the final steps of that, that, take it to a whole nother level even. But for making it super easy to add backend functionality and payments and different integrations and that sort of thing. But yeah, when we first launched, it was like really, we had no idea that anyone would find this useful, honestly. Like we were like, this seems cool. It seems like maybe some developers will find it interesting. But what we ended up finding is that you know, we had hundreds of thousands of people that were not developers that were coming to this to try and build applications.

**Eric Simons (Bolt CEO)** (00:16:46)

And, yeah, and often like going and manually setting up Supabase auth and this and that all these different places was really, you know, at a minimum, just a pain. But for folks that aren't doing development day to day, it's like it can, it's a kind of a, you know, a blocker, right, to actually proceeding and building these things. So we're spending a lot of time, like doing a lot of deep integrations that just turn a lot of this stuff into one click. So you don't have to think about it, you know, et cetera, et cetera. Right. Um, yeah, so that's definitely one of the new things that we've shipped here. And let's see if we can go ahead and get this thing. Uh, if we actually post now, so I would say stack blitz, um, mirror remote, uh, run the company, $1, $2 and, uh,

**Eric Simons (Bolt CEO)** (00:17:36)

Alt.new.

**Eric Simons (Bolt CEO)** (00:17:40)

See if that works. But boom, take a look at that. So we actually see, if I open this up on our other page, give us a little more room and reconnect to that. We should see the, yeah, our CEO job listing here. I can click in and see the salary range of this thing. And it's actually like, you know, even the small things here, right? Like it actually, you know, put the correct logo kind of in a little square box so it fits and whatnot. Right. So super cool. So that's the beginning of this app. So what should we add next here?

**Aakash Gupta** (00:18:18)

I feel like the next thing we need just to get it kicked off the ground is we need to load in some jobs. Like how can we get it to pull from somewhere? We'll need some other job. I guess, do we need to find like a free API to another jobs board or how could we think about approaching that?

**Eric Simons (Bolt CEO)** (00:18:36)

Yeah, that's a good question. Yeah, I wonder if there are, like, if there are, you know, are there free job board APIs that we could actually pull a job from? This is kind of what you're saying, right?

**Aakash Gupta** (00:18:52)

Yeah.

**Eric Simons (Bolt CEO)** (00:18:53)

Okay, let's see.

**Aakash Gupta** (00:18:54)

Because I imagine repeated scraping will hit some sort of limit at some point.

**Eric Simons (Bolt CEO)** (00:19:01)

I have no idea if this is going to work. I have no idea what this is. Firework or find work, find work. I still don't know what it is, but find work.dev API immediately. That's cool. So we get 100 requests per month. And let's see what it does. And the nice thing too is like, if this doesn't work, we can just roll back to the previous version and go, okay, that was not a good idea and revert the thing.

**Aakash Gupta** (00:19:31)

Yeah, I like how it took the initiative. It's like that employee with really high agency who just goes.

**Eric Simons (Bolt CEO)** (00:19:39)

Okay, so we need to get an API key. Assisting's probably complaining about that. Let's see. So your API key from the dashboard. Do

**Aakash Gupta** (00:19:50)

you want to do this? Yeah, I want to see what we have to do. Like I want people to actually see the real steps, how you have to get out of the app sometimes.

**Eric Simons (Bolt CEO)** (00:19:57)

Okay, and let's go ahead and pull this up. So findwork.dev. the larger search engine. Let's go ahead and

**Eric Simons (Bolt CEO)** (00:20:04)

actually pay money for this thing. All right, let's send it with GitHub. Take all my

**Eric Simons (Bolt CEO)** (00:20:10)

data. Oh gosh, don't. I trust you. My own product recommended you. Okay, which email though? Okay, so that's my personal. Let me go and pull that up.

**Eric Simons (Bolt CEO)** (00:20:22)

Let's take a look. Okay, I am confirmed. So this should now, I should now be able to, yeah, I'm signed in. And so what did Bolts tell me to do? It said, API key from the dashboard. Okay, developers, is that what I'm doing? All jobs, API, REST API, maybe

**Eric Simons (Bolt CEO)** (00:20:55)

go there. Oh, let's go. Okay, copy. I think everyone's going to see this on screen. Let's take a look at this thing. All right, take a look at it. It's all its glory. I don't know what this thing is. They don't have my credit card. So anyone who's watching, feel free to have fun. And I'm going to go down to my env file. And so it says, oh, sorry, findwork.tsfile.

**Eric Simons (Bolt CEO)** (00:21:18)

Where was that defined?

**Eric Simons (Bolt CEO)** (00:21:21)

There we go. So I'm going to paste that in there. and

**Aakash Gupta** (00:21:26)

so here we just went straight to the code but it gave us a really clear instructions yep

**Eric Simons (Bolt CEO)** (00:21:32)

absolutely um and uh so now how do we actually use this so

**Eric Simons (Bolt CEO)** (00:21:42)

there other uh okay

**Eric Simons (Bolt CEO)** (00:21:43)

so let's like i guess like um it gonna how do i

**Eric Simons (Bolt CEO)** (00:21:54)

see results from the find work api if only see the ones from my super base right now let's see what it says okay so is that my api key it is okay

**Aakash Gupta** (00:22:22)

So it's now going to connect the search to the API, I think. I think so. I

**Eric Simons (Bolt CEO)** (00:22:28)

think that's what's going to give it a shot on. All right. So it's telling me like open up my console to make sure that, um, to see if there's any like errors that are happening and there are, so that makes sense. Okay, so what it's complaining about here is that it's getting blocked by cores. Okay, so that's unfortunately an issue. So I think I can just tell it actually, like it says it's getting blocked by cores.

**Aakash Gupta** (00:23:08)

Coresproxy.io. Okay, let's see if this works. Sometimes people get most scared when they get into this debugging stage, but I think it's about trying one thing at a time. Totally, totally.

**Eric Simons (Bolt CEO)** (00:23:21)

And let's see. So it's still actually saying there's a cores issue. So I can actually tell what to do is, you know, use a local node server. for the request instead. This is me being a little more technical and just telling him what to do. But basically, you can effectively tell Bolt, like, hey, because this is a full operating system running in the browser here, it could actually just go and create servers on demand to go and do stuff, right? And so what this should do is create, so yeah, it's actually gonna just create an endpoint, which is the proper way probably of doing this if you're a developer, creating an endpoint that you can go ahead and punch into. And I need to flip to the correct port here and

**Eric Simons (Bolt CEO)** (00:24:07)

let's see if this works. Okay. Is there an error being thrown?

**Eric Simons (Bolt CEO)** (00:24:22)

okay valid time value okay so it did the good news is it actually did forget the jobs um and so what i will do here is uh is going to paste this error

**Eric Simons (Bolt CEO)** (00:24:34)

in okay so hopefully with that we should actually see

**Eric Simons (Bolt CEO)** (00:24:46)

the job results come in properly

**Aakash Gupta** (00:24:52)

kind of like a two-stage debugging wasn't actually that scary. It's just when you get that window, your heart rate rises. You just got to work through it. Yeah, exactly, exactly. And

**Eric Simons (Bolt CEO)** (00:25:04)

by the way, the other cool thing too is like, because this is all running in the browser, like in bold, like we're not using remote VMs, If something's ever going wrong, like often we're using like Gmail or something, right? Like things will like get wonky or like any web app for that matter. It just like might be acting weird. You can always get back to a clean state in those apps just by hitting the refresh button. And the same is true for bold. And that's not true of any other stuff out there because if there's something wrong with the VM, hitting refresh is just going to like reconnect you to that VM. So like if I were just, again, hit refresh on this project, it's actually going to like pick this up, you know, go ahead and boot this thing up from the ground up. I can go back here and actually pull this up while it's booting up.

**Eric Simons (Bolt CEO)** (00:25:43)

But it started this from scratch. So if there's anything specifically wrong with our setup, it's going to go ahead and just clear that out, et cetera. I don't know why this error keeps popping up because it's not actually an error. But if you don't mind, I want to just delete this just because it's like some random

**Aakash Gupta** (00:25:58)

guy. Yeah, let's do it. Wait, what is this? We've seen a couple times a potential problem detected. So you're finding that file and you're going to delete it. I don't know why. OK, no,

**Eric Simons (Bolt CEO)** (00:26:10)

sorry. We are actually getting a real error at this point, error parsing date. So we go ahead and hit attempt fix on this one.

<!-- sponsor -->
**Aakash Gupta** (00:26:21)

today's episode is brought to you by amplitude building great digital products is hard you know that better than anyone getting teams aligned measuring what matters and scaling your product strategy isn't easy but what if you had a clear framework to guide your next steps that's exactly what amplitude built they studied the best product teams to understand what really drives impact and turn those insights into the digital experience maturity assessment In two minutes you'll be able to see where your team stands and what you can improve to build better products faster. Click the link in the caption to take the free assessment and get a clear path to product growth.

**Eric Simons (Bolt CEO)** (00:26:56)

And so this is also interesting because we're integrating an API that like, I've never used this API. We did not design Bolt to work with this API, right? Like this is just pulling in whatever the LLM has, you know, in context. When we're hitting debug, it's maybe going to the internet, going like, you know, parsing API documentation, et cetera. But that's like it, right? I mean, like this is, you know, to kind of give you like a range of like the sort of things you can do, this is not like the happy path that we're doing here. Like we're using... some random thing. And it's actually pulling in real like engineering roles. It looks like,

**Aakash Gupta** (00:27:27)

right. That's

**Eric Simons (Bolt CEO)** (00:27:27)

amazing with real. Yeah. And so as you can see, there's like, there's another, uh, you know, another, another, uh, role here that, uh, you know, seems to not be working. So let's see if this works. But basically we click on the job now it's like not showing the proper job. Right. Um, And okay, so it looks like it's actually the job page is only pulling from Supabase instead of from the provider, right? So we're kind of doing a weird thing here because we have like our Supabase ones and then we're like pulling from some external service, right? So it kind of makes sense. When we started off, we didn't tell it that we were going to do that. We were like, hey, we're going to have a job site where we're posting things. But we just kind of changed the scope of this thing halfway through.

**Eric Simons (Bolt CEO)** (00:28:08)

So it's like, okay, now this is probably still not going to work because it's trying to look at our database and not what's out there. So what I need to say is like, okay, you know, when

**Aakash Gupta** (00:28:18)

I

**Eric Simons (Bolt CEO)** (00:28:18)

cache what we get from the API into our super base or something like that. That's a good question, actually. Um, you know, that's, uh, we, we could, we could totally ask it to do that. If we want to like, if we want to like clone the results in, we could probably have it do that. I wonder if, um, like for those results, do we want to own the results or do we want to actually link people out? to the you know wherever that job board is for it

**Aakash Gupta** (00:28:43)

i guess if we're trying to create an seo optimized site we want to have like individual pages for those okay

**Eric Simons (Bolt CEO)** (00:28:49)

so um when we pull in results from the api um make sure they're stored in supabase in a cache way um What I could see out is they could just keep growing in the Supabase over time. I wonder if there's a unique way. If there's some unique way to de-dupe them, that would be great.

**Eric Simons (Bolt CEO)** (00:29:21)

Let's see what it does.

**Eric Simons (Bolt CEO)** (00:29:31)

I'm like, this is definitely not easy. We're throwing this thing for its pace this year. Yeah, exactly. When you want to build a real app, this is the exact, you'll run into this stuff you're trying to integrate external APIs or whatever have you.

**Aakash Gupta** (00:29:48)

Yeah, and neither of us had ever heard of this API before, but it's managing to successfully work with it really nicely. Yeah.

**Eric Simons (Bolt CEO)** (00:29:55)

Yep. And so you just created the migration file. It looks like that got applied properly. And now we have a couple of issues. We go ahead and attempt

**Eric Simons (Bolt CEO)** (00:30:04)

fix on this guy. Let's see if we can.

**Aakash Gupta** (00:30:06)

I feel like getting this far, if I'd gotten this far in one day as an engineer, I would be pretty happy at this point. I'd be like, yeah, good,

**Eric Simons (Bolt CEO)** (00:30:13)

good job. Day one done. Good to go to sleep. Wake up tomorrow. Get back. Yeah. This is like day one of the weekend project, right? Yeah.

**Eric Simons (Bolt CEO)** (00:30:20)

Yeah. that's kind of, it's

**Eric Simons (Bolt CEO)** (00:30:23)

kind of unbelievable. You know, um, I, I, I guess I, I, you know, I'm used to it personally, not just cause we've been, you know, building this thing since, uh, you know, October or whatever, but, um, um, okay, let's take a look. Uh,

**Eric Simons (Bolt CEO)** (00:30:38)

why is this thing failing? Let's see. Let's click clear that. Let's see if that actually.

**Eric Simons (Bolt CEO)** (00:30:42)

Okay. So that might've just been a transient error. Um, but, uh, So when, wait. Okay, so I think because now it's showing search results that are coming from the database and the API. So we actually only want to show stuff that's coming from the database, not the API, right? Because we don't want to, we want, if people are going to click in and see the details of the job post, that would have to be coming from the database and not like, you know, So it kind of needs to be tied together in that way, if you know what I mean. So I think we say like when I click on, or actually in the job listings, don't show the stuff directly from the API anymore, only list from Supabase, including the cached job listings. And on every page load, feel free to update the cache

**Eric Simons (Bolt CEO)** (00:32:03)

if needed. Let's see what it does there.

**Eric Simons (Bolt CEO)** (00:32:13)

So this is definitely like... this is definitely like a situation where upfront, if you spend time thinking through what you wanted to do, right? So like a lot of, we're actually gonna add a discussion mode into both, but like, which is effectively, like it won't actually write code. It's not like agent mode basically. But so whether you're using that, which is coming out, I think like next week, or if you're using a cloud or chat GPT, it's like going in like, hey, I wanna go and make a job listing site that use it, you know, that's gonna pull stuff, you know, from APIs, like puts in the database, et cetera. you're basically making a PRD, right? It's like, this sort of application would be a great camp for like a PRD. Because like one of the things I think a lot of people that haven't used these tools before can kind of run into is like, if you kind of come here without a plan, you try and vibe code your way all the way through, you can end up in these scenarios where the AI is building out in a certain direction.

**Eric Simons (Bolt CEO)** (00:33:07)

And then when it has to kind of change course and start meaningfully changing the application, it has a much more difficult time to kind of go a brand new way then versus if kind of upfront, you're like, hey, this is kind of like the scope and the spec and kind of how we generally want to do this and, you know, et cetera. But,

**Eric Simons (Bolt CEO)** (00:33:26)

okay, let's see. It's still claiming that there's an issue with the cached jobs thing. Let's just try and hit fix issue there. Okay. Add a migration. Let's see if this works. Okay. Does not seem to be an error.

**Eric Simons (Bolt CEO)** (00:34:00)

But I still, when I click, it says job not found. But it does appear that we are caching the jobs.

**Eric Simons (Bolt CEO)** (00:34:16)

Yeah.

**Eric Simons (Bolt CEO)** (00:34:17)

Oh, okay. Yeah, there we go. Cool. So it just wasn't pulling from the cache jobs table. kind of blowing my mind that it's figuring this out, honestly, because this is like, as a developer, if I had, if I had a, you know, PM or designer, you know, that was telling me to like, okay, now go do this. I'd be like, seriously, like you're telling me that now, like, I've already built it this way, you know, like, are you kidding me? And it's, and it would take a while. It would take, you know, the frustration would be, it would take a while, like go and read, you know, configure this thing to like be a point from

**Eric Simons (Bolt CEO)** (00:34:50)

different stuff. Absolutely.

**Eric Simons (Bolt CEO)** (00:34:52)

OK, so it's still saying the job is not found.

**Eric Simons (Bolt CEO)** (00:34:55)

Improve the search logic. Let's see if this searches.

**Eric Simons (Bolt CEO)** (00:35:05)

It's actually pulling in the tags, too, and putting it in the UI. That's really cool. It says where it came from as well. Let me go ahead and open this in a new tab again. Because I want to see what the deal is with what URL it's kicking it back to

**Eric Simons (Bolt CEO)** (00:35:23)

when I open this up. So I click on this URL. And what's

**Aakash Gupta** (00:35:28)

happening exactly when you open it in a new tab?

**Eric Simons (Bolt CEO)** (00:35:30)

Yeah, so what's going on with this thing is it's basically it's running a local dev server inside of your browser. So you can actually preview the app just in its own browser tab effectively. Um, what's cool is you get, you know, it's like a normal web app where you get access to, uh, you know, the URL, like you can just control the URL, type in whatever URL path. Um, also for debugging, it's nice cause you can like pull up the console and you're just seeing, you know, the errors that are happening on this page. Um, and so let's go ahead and just hit refresh and see if any errors happen actually. Okay. So there is, there's no error that happens. Um, and what's interesting. So it's pulling from sube basis, not getting anything, anything back. Um, One thing we can do is we can actually go to our Supabase project and we can look at the table itself

**Eric Simons (Bolt CEO)** (00:36:24)

and go into cache jobs. How do I do this? In table editor. Okay, so.

**Eric Simons (Bolt CEO)** (00:36:30)

Looks like it does have the job data there. It's absolutely storing the data, which is honestly, this is like the hard part typically. So there's some like bug where it's just not pulling from, the right location or something. Um,

**Eric Simons (Bolt CEO)** (00:36:44)

and

**Eric Simons (Bolt CEO)** (00:36:44)

what's interesting is, you know, typically you're looking at the URL path, which here is this, that, uh, slug. So my question is where is, cause this is the unique identifier. Where is the slug for this? Um, I think that might be the issue is it's not actually pulling, um, it's not pulling the correct job listing slug. Um, so maybe, um, You know, on the job post, on the job page, it looks like it's not using the correct, what is it

**Eric Simons (Bolt CEO)** (00:37:22)

called? Yeah, UUID in the URL to pull the listing from cached jobs.

**Aakash Gupta** (00:37:43)

So here, a little technical knowledge definitely helped.

**Eric Simons (Bolt CEO)** (00:37:45)

Absolutely. Absolutely. And I think that's like, you know, it's kind of like, you know, like I have a DSLR camera, right? And I don't know how to use it. You know, my wife and I got it because we were like, oh, we're going on a honeymoon. We should, you know, like we should bring this thing. And we know enough to how to like turn it on and like take a photo. And that's like it, right? Right. And the problem though is it's, you know, oh, we're in motion. So how do we do that? How do we kind of capture the right frame of it? It's like kind of, and the thing with these AI tools is like the more that you can kind of dig in a little bit deeper, it doesn't have to be like understanding fully out of code, but like what we're talking about here is not even like coding.

**Eric Simons (Bolt CEO)** (00:38:28)

It's like, okay at a high level when i go to a website and you know i land on a profile page or something how is that uniquely getting tied you know how is like my profile showing up right it's like okay that's what's in the url path there's some unique thing there you know that gets that gets sent back right um and uh okay let's

**Eric Simons (Bolt CEO)** (00:38:48)

see

**Eric Simons (Bolt CEO)** (00:38:52)

so i think i think the home the i think that what's going on is the job listing page um oh is there an external id Oh, okay. There we go. Okay. And let's see, look at the jobs one. So there's no external ID.

**Eric Simons (Bolt CEO)** (00:39:06)

Yeah. Okay. Let's see if this works. Let's see if it passes that along.

**Aakash Gupta** (00:39:14)

If this is scaring you at this point, hopefully it's also building some empathy for your developers because they're normally doing this stepwise, trying four or five things to solve the bug, but it takes a longer for each of those cycles.

**Eric Simons (Bolt CEO)** (00:39:26)

Absolutely. Absolutely. It's a lot of this is just trial and error, right? So that's like a very natural, if you're going to try and like throw this, like, you know, build something that is again, touching external APIs, connect to them, et cetera. like a lot of it is is simply like what we're doing here is debugging and like and that is still part of the process of like building apps with you know uh with these ai you know text to app tools you are going to run into these types of things um and our job as a company is to continue like making this receding pocket of the experience where like you run into fewer and fewer things because we're indexing more and more stuff or whatever have you um And, uh, let's see, I, I suspect this might not work still. Yeah. Okay. So, and I, I think the reason for that, let's go ahead and pull this up over here.

**Eric Simons (Bolt CEO)** (00:40:09)

Um, I suspect the reason for that is that, uh, so it's using this, it's, it's, it doesn't look like it's using this external ID. Um, and, uh, let me go and reconnect. Yeah. I don't think it's using the external ID because, uh, on the job listing page where I don't think we're sending the right unique ID

**Eric Simons (Bolt CEO)** (00:40:40)

for the job listing pages because I still get the not found error. Let's see what it says. Yep, dead right. Okay, let's see if this does it.

**Aakash Gupta** (00:41:12)

And does Bolt typically

**Eric Simons (Bolt CEO)** (00:41:13)

use React or always use React? We'll prefer to, largely because most of the training data out there, I mean, React is the most popular framework by no small margin. And so you're going to get the best results with React apps. We support everything, though. So you can actually tell Bolt to use Vue or Svelte or Next.js or whatever have you. We can run all of it. Let's see. Hopefully this works out. Let's go, finally.

**Eric Simons (Bolt CEO)** (00:41:39)

Let's

**Eric Simons (Bolt CEO)** (00:41:39)

go. This is pretty crazy. I mean, I got to tell you, I'm pretty, I'm actually pretty impressed because again, we're like, we're pulling from some external API here, storing in our own database. And all of this content now is coming from our database and not the API, right? Like that's, and it was smart enough to actually break down the fields it was getting back from the API like these tags, it's like actually showing up as like UI for that, right? So this is pretty cool. Because again, if you had to code this from scratch, this would be a lift. We came to this not knowing what API we're going to use, how we were going to do it. And it's actually like pulling these things in, right? So if

**Aakash Gupta** (00:42:29)

we were excited and we wanted to deploy this to the web, what would we do next?

**Eric Simons (Bolt CEO)** (00:42:34)

Yeah, totally. You would just hit this deploy button, which will actually put it on Netlify. So the one thing is I think with the proxy thing we're doing, it might not be able to actually pull the job listings. It would take a little bit of work, I think, to do that. We can do it and I'll show you what it'll look like. But this is what's really cool about Bolt is you can actually do a production build of this thing. It's built directly into the experience. You don't have to know how to do this stuff. We have this partnership with Netlify where we can actually deploy live sites to Netlify. You don't even have to log in or have a Netlify account. I mean, actually, you know, this is now live on the internet. I can crack it open. Oh, no, it's actually, sorry, it is working.

**Eric Simons (Bolt CEO)** (00:43:19)

So in post, go ahead

**Aakash Gupta** (00:43:21)

and

**Eric Simons (Bolt CEO)** (00:43:21)

edit

**Aakash Gupta** (00:43:21)

out the

**Eric Simons (Bolt CEO)** (00:43:21)

part where I said it might not work. But yeah, so this is actually, this is working. And I can go in and view the different job listings. And this is like, this is real, like Netlify is a real production host, right? And so I can actually attach, if we wanted to buy like remotehub.com, if it was available or whatever, In Netlify, I can do that. And just clicking this link will actually take that web app, attach it to my Netlify account, and then I can point that domain at it. And then from there on out, as I am prompting here and hitting deploy, it's just updating this production version of the application, right? Like live on the internet, which is pretty wild. Because it's like, that's, you know, again, setting up, even just setting up deployment properly is typically a pretty big lift, you know? So just having this kind of seamlessly tied together like that is wild.

**Eric Simons (Bolt CEO)** (00:44:12)

And let's see if the search works. So if I type privacy, yeah, I mean, even the search works on the thing. This is nuts. I don't know why these logos, are these logos not, what's it, using some placeholder API. That's why they're not showing up. So I guess these don't necessarily, not all of them have correct logos on them, but anyways, yeah. So we actually have like a production deployed app now of this thing, which is pretty cool. And then

**Aakash Gupta** (00:44:38)

the next step, I guess, People will normally want to upload the code base to GitHub and start using GitHub for version control and stuff. How do they handle that?

**Eric Simons (Bolt CEO)** (00:44:49)

Yeah, totally. So today, you can actually export. You can either download it to Zips to your local. We're adding in direct Git functionality this month. So you'll be able to just push this to a repo and just keep committing there. Our previous product to Bolt was a web-based IDE. So what's kind of cool is that you can just one click to actually open this project up in our full IDE. So if you want to actually have like VS code cursor type editing in the browser, you can do that here. And actually in here, you can actually go through the flow of creating a Git repo out of this thing, which is pretty cool. So today you can actually from Bolt create a Git repo out of this, commit to it, et cetera, by using StackBlitz, but we're going to be taking this and just bringing it back into bolt.new itself.

**Aakash Gupta** (00:45:40)

Awesome. So that covers how you literally build websites that you could buy remotehub.com for and start competing with levels if you wanted in Bolt. I want to showcase two other sets of features that we've talked a little bit about. The first being your new Figma integration, because a lot of people listening, especially they might be product managers or designers. They might be living a lot of their lives in Figma. How can you go from Figma design to working prototype with Bolt?

**Eric Simons (Bolt CEO)** (00:46:13)

Totally. Yeah, and I'll clear out a couple of tabs here. So we actually just announced this today. I'll pull up the tweet. So this is pretty cool. Basically, we've worked on this. There's this company called Anima that's for the past, I think, like seven years, they've been making like they're the number one Figma plugin for like turning a Figma design into code. And so we partnered up with those folks and they're, they're awesome. And, uh, really simple. Like you can actually on any Figma URL, you can just put bolt.new in front of it and it'll actually suck in that design, split it apart and create a pixel for pixel version of it perfectly. Um, and then, you know, load it into bolt, into bolt as a full stack app that you could actually start like prompting functionality onto, you know, and et cetera. Right. Um, And so I can go ahead and show this here.

**Eric Simons (Bolt CEO)** (00:47:02)

So if you want to do this from our homepage, you just click Import Figma. You can just go ahead and paste a Figma URL there. I've got a Figma pulled up over here. This is just one of our examples. So I think I always think kind of the coolest, most fun way to do this is to just change the URL out. So if I go ahead and put bolt.new in front of the Figma URL, as you can see there, and hit Enter, what's going to happen is it's going to go ahead and actually pull in this design from Figma. And so now it's actually taking each layer and splitting it apart. So if you actually have like things that are, you know, not meant to be like market, but like actual images, what this thing is doing is actually converting all those into individual image assets.

**Eric Simons (Bolt CEO)** (00:47:43)

They can be linked, et cetera, properly. Um, it's actually writing, you know, uh, production grade code. I think out of the box, we default to like shad CN, um, you know, and react, but you can also, uh, I think in a, like under the hood, we, we support view and Svelte, but, uh, I think we're going to roll out the ability to pick those, um, you know, in, in a future update here. And, um, so yeah, it's going to go actually just, you know, take this thing apart and generate the code for it. Um, and let me go ahead and show just to like, kind of give you the side by side. Let me pull this back up in another tab here. Um, But yeah, I mean, to code this from scratch would take a good amount of time, just if you're doing like a one-to-one on this thing, right?

**Eric Simons (Bolt CEO)** (00:48:25)

But that is like, if you actually want to make it functional and have, if I click sign up, it like pops up a modal for me to sign up or whatever, that can take a good amount of time, right? And this process, by the way, if you're on the screen, you try this, Yeah, this can take a couple of minutes and I imagine we're underneath heavy load right now. So like fingers crossed,

**Aakash Gupta** (00:48:46)

knock on

**Eric Simons (Bolt CEO)** (00:48:47)

wood that this finishes because I have a feeling that we're rapidly increasing the amount of GPUs on hand at the moment to handle this thing. But it can take a minute because it's especially for like a big design like the one we just looked at, which is like pretty, pretty substantial. I mean, this is a pretty big page, like a lot of different elements and stuff going on in this thing. Um, well, I go ahead and finish up a creation here.

**Aakash Gupta** (00:49:16)

And what's interesting is like, unlike if users are used to using like Claude, just through the Claude chat interface where it often runs into like context limits or things like, uh, that it does, it seems like you guys have built technology on the backend to handle that and be able to do more.

**Eric Simons (Bolt CEO)** (00:49:35)

Yeah, absolutely. And yeah, cause like we did the name of the game for us to be able to handle like, you know, sufficiently large projects. Right. Um, You can build pretty large things today in Bolt. I can't remember how large it gets once. We'll put a warning up that says, hey, you may see degraded performance. Because this is the problem that all these, even things like Cursor or Windsurf or whatever, once your app gets to a certain size, just because of the limits of context windows and LLMs, you have to selectively slice out context, right? Um, but with bold, we may be able to actually squeeze the, the amount that you can really kind of keep in context pretty far. Um, and I'm, I'm getting a little suspicious about this thing. Um, this is taking, I mean, we, we might be underneath extremely heavy load. Um, let me go ahead and I'm going to pop open another tab and see if I can run it side by side.

**Eric Simons (Bolt CEO)** (00:50:23)

Um, hopefully you can cut this out in post. Um, okay. And so you can see once it actually, uh, converts to code, we actually have the, uh, the application here. And again, just to kind of compare it side by side, this is what we're looking at. And I'll go ahead and full screen this here so we can kind of get the full experience. But it's even got, you know, a little dropdown stubbed out and everything. You can scroll through. Again, these are like real images that are like split out from that design. And, you know, has responsive view built in. So it's really like, you know, this just took a lot of the work out of, you know, what you would normally have to do by hand. And again, what's cool is that I can say, you know, when I click log in or sign up, you know, pop up a modal, you know, or the user.

**Eric Simons (Bolt CEO)** (00:51:16)

And let's see what it does. So I can actually add functionality onto this to turn it into a real full stack app. Because we see a lot of PMs and designers, what they've been using Bolt for to date has been rapid prototyping. And they'll take a screenshot of a Figma and then they'll use Bolt to add functionality to your pages on because it's faster than having to manually kind of create a static prototype that the user clicks through. And so with this, it kind of takes that to the next level because you can lay out your design system. You can lay out a couple of the key you know pages that you want or whatever and then from there you can if you want to add another page you can just say

**Aakash Gupta** (00:51:51)

hey

**Eric Simons (Bolt CEO)** (00:51:51)

oh add a page for this add a page for that have a modal pop up for this um and it'll just go ahead and actually go and do that for you right um so that's i think like really the magic uh the magic experience of like having that like direct figma integration you know it's as of today is like is you know going to give people so um let's see it's going to go ahead and finish up here And we should have a new landing page where I can go ahead and click the sign up button, get a modal back, et cetera. A few seconds here.

**Aakash Gupta** (00:52:25)

And what kind of adoption are you seeing amongst engineers for this, like just speeding up their workflows? Is that still the core user group?

**Eric Simons (Bolt CEO)** (00:52:34)

Yeah. So it's, yeah, funny enough, it's like, you know, maybe like 30, 40% of our users are engineers at this point. And, you know, 60, 70 are PMs, designers, entrepreneurs, right? Like people that have always been really great at building products, but just have never had the ability to themselves, you know, do it before, right? Other than having to, you know, do it through a developer's fingertips. But that's basically kind of what Bolt did is this is, it's like your developer co-worker that you can use. I don't know why this is popping up. Yeah. But that's basically, you know, PMs and designers kind of treat it as like their developer coworker that they're having to go and build this thing out. And so if I go ahead and click on login, you see

**Eric Simons (Bolt CEO)** (00:53:16)

now.

**Eric Simons (Bolt CEO)** (00:53:18)

Yeah. So just a simple example, but like, again, I mean, you could, you could then say, okay, add authentication with Supabase and like, and it would go and do that. Just like we had in our last app. Right. So. you can actually go and turn this into a fully functional full stack app with auth backend accessing APIs, et cetera. And we're talking about like minutes, not even hours or days, right? To get basic versions of these things working, so.

**Aakash Gupta** (00:53:47)

The final functionality I wanted to showcase to people, because it's pretty unique to Bolt, is building a mobile app.

**Eric Simons (Bolt CEO)** (00:53:52)

Yeah. Yeah, it's a fun one. So let's go back to the homepage here and close out these tabs. This was a cool one we worked on with the Expo team. So yeah, building web apps is awesome, right? But building native iOS apps is even more of a pain, even if you're a developer. You have to be on a Mac. You have to know how to use Xcode and da-da-da-da-da. And so we did this integration with Expo, which is these are folks that make the best React Native ecosystem in the world. And it works like magic. So on the home page, you can click this, build a mobile app with Expo, and it teaches you how to build mobile app, which is just tell Bullet you want a mobile app basically. So just as a simple one, we can say, you know, mobile app that is a to-do list, you know, for my day or something, something simple.

**Eric Simons (Bolt CEO)** (00:54:47)

And what this is going to do is it's going to go ahead and get to work, you know, creating a Expo project. And with Expo, one of the awesome things that they've developed is a way to basically live preview your application. while you are developing it. Um, cause like, you know, there's also a web view that you can use, you kind of preview it on your, uh, your, you know, a web browser, but, um, you know, there's nothing quite for a mobile app, especially there's nothing quite like touching it and feeling it like as it is being built. And especially if you're building for iOS and Android or, or one or the other, um, you want to make sure it like works great specifically for each platform. Um, And so that, you know, typically that can be kind of a process, you know, if you're not using a cross-platform sort of framework.

**Eric Simons (Bolt CEO)** (00:55:33)

But with Expo, they have this app called Expo Go, where once this thing's done, punching out the initial code here, it's going to spin up the dev server. I'll be able to like take a screenshot of this thing. You can too, actually, by the way. But a little QR code is going to pop up. and it can actually render the app on my device and your device. And as we are prompting, it's just live updating, right? So you can see here, we got this QR code. So I'm gonna go ahead and take a photo of this thing. And you have to have the Expo Go app installed on your phone, but it's like free from the app store, et cetera. And so it's building the JavaScript bundle and it's downloading to my phone. Do, do, do, do, do. So this is the current screen I'm on.

**Eric Simons (Bolt CEO)** (00:56:18)

It's just waiting. And I'm going to go ahead and there we go. So this is the tasks. This is like the current UI. And so you can see it in kind of the preview here. I'll zoom in a little bit. But so this is the web version that we're looking at. And in a second here, I imagine we are going to get the iOS version done.

**Eric Simons (Bolt CEO)** (00:56:45)

Just finishing compiling all this stuff. Okay. Let

**Eric Simons (Bolt CEO)** (00:56:53)

that finish. And on my device, you can see looking at the same to do app on this thing, right? So we can go and test out the functionality. See, I have a little to do. I'll try and do like an over the shoulder shot here. But you know, if I type in a to do on my phone, and hit the blue button, I can actually see that the to-do down here shows up. I typed in, right? So anyway, so it's like, we have like actually like a real to-do app that we just like vibe coded, you know, that's running on my device and I can say, you know, make it a dark theme and it'll get to work, update the code. And as it is changing the code here to make it a dark theme, I'll kind of, I'll keep my phone pulled up here so you've got to see it.

**Eric Simons (Bolt CEO)** (00:57:49)

um once it finishes but it's kind of like magic i mean it's just like you're you're able to actually like feel the app as it's being developed now you can actually see the bottom bar there is already in dark theme um and so now it's updating the other page so once that's uh once it's done writing that code on my phone you should see it go from uh yeah there you go so now wow yeah right so and you can again you can try this from anywhere around the world this is you know it's synchronizing this um and you have so you know imagine if you have a remote team or if you have a co-worker or a customer that you want to like give a preview of a prototype like a real one they can actually try it and then you know give real feedback in real time and you can update the app and and you know let them actually play around with it and use it, you know?

**Eric Simons (Bolt CEO)** (00:58:37)

So this is like, this is pretty cool. I mean, I think we launched it like a month ago. It's been one of the most used features, I think, on Bolt simply because, I mean, there's just like, it's never been easier to create a mobile app that's like real that you can try, you know? And so yeah, that's a pretty fun one.

**Aakash Gupta** (00:58:56)

That is insane. This was an insane set of demos. That concludes the demo portion. Now I have to pick your brain a little bit as this story is just crazy. And a lot of people listening, their product managers, product designers, they want to know how are you deciding what to build? How are you prioritizing these features well? How did you really crack this nut to keep growing with... really awesome product feature releases, not with expensive marketing campaigns.

**Eric Simons (Bolt CEO)** (00:59:30)

Yeah, I think we listen to the folks that are using the product a lot. And I think there's a good mix of just really understanding the challenges people are running into, but then also kind of looking at the aspirations of what do people want to be able to do, right? Because I think that's where the fun stuff, like the mobile expo stuff that we did kind of kicks in because people were like, hey, I want to make... native apps you know and um and then from our side we understand technically okay how how could you do that what sort of experience we want to provide um you know we kind of like we're able to really glue together something that just feels like magic but um but yeah so i think a lot of it and this is just you know i think a lot of just building building great products is just like listening listening to your you know your users your customers and um and just thinking you're trying to figure out how to build the the best experiences that you possibly can you know

**Aakash Gupta** (01:00:26)

And internally, how do you guys organize the roadmap or like kind of decide what is going to go in what sequence?

**Eric Simons (Bolt CEO)** (01:00:32)

Yeah, really good question. It's especially tough now because we just have so like there's so many things on fire at a given time. It just has been that way since October, basically. And we have 20 people total at the company. I think engineers were like 15. We have to grow a lot. We're hiring, by the way, you know, on all fronts, product design, engineering. So go to stackwiths.com slash careers if you're interested. But yeah, so for prioritizing, though, a lot of it is like, I mean, if there's kind of things that are obviously urgent, breaking the experience, that gets kicked to the P0. Beyond that, what we look at is what is, to the degree that we can measure the impact and demand of this that we're seeing from customers and et cetera, we try and stack rank based on, okay, how big of an impact do we think this is going to make?

**Eric Simons (Bolt CEO)** (01:01:24)

And the hard thing is that there's a lot of things that seem to fall in the same categories. And so it's like, okay, well, do we do that thing or that thing first? And the answer is, we just have discussions and, you know, make a call and move on. And sometimes we get it right. I feel like a good amount of time we get it right. And sometimes we're like, oh, we should have, you know, maybe prioritize that one a bit more. But generally speaking, it's just better to just take action and, you know, I think get moving versus, you know, have a, spend a whole bunch of time figuring out, having the conversation about what to build or whatever, you know what I mean? But, yeah.

**Aakash Gupta** (01:02:01)

So a lot of people are going to be comparing Bolt to other things out there. I think like the most like for like comparisons are tools like Lovable or maybe Replit. Then you also have tools like Cursor and windsurf so how would you kind of explain and compare bolt to those other options

**Eric Simons (Bolt CEO)** (01:02:23)

yeah i think um i think the key thing for us uh and this is like a bit under the hood is how that the in-browser operating system i was talking about like That is a huge differentiator. And it's not one that's going to be visible. Like, it's not like a thing you can necessarily like see, but from an experience perspective, this thing is fast and it's really, it's reliable. Like, again, if something goes wrong, you can refresh the page, get back to a working state, et cetera. That's the big problem with a lot of these other things is they're having to spin up a VM for every single user that's coming to the site. which introduces latency between the user and the VM, if things go wrong at the VM, then how does the user get back to a fresh state? Often their support team of that company has to step in and like, you know, force reboots or whatever that VM that can take days, weeks, whatever, you know, for to actually get a response from someone.

**Eric Simons (Bolt CEO)** (01:03:14)

And then just a lot of downtime to across these things.

**Aakash Gupta** (01:03:17)

So I

**Eric Simons (Bolt CEO)** (01:03:18)

think that's like kind of one, the main thing of us versus kind of everything else. I think the other thing that we do, you know, like kind of capabilities wise, I think the Figma integration that we've got, I think Level might have one, but I mean, as far as how seamless that is, where I think you have to sign it from some other service and then click a whole bunch of things to do it. Whereas with this, it's just kind of built and you paste the link, boom, it just converts it. And I don't think Replit has Figma. Yeah. I think we're the only guys that have really a direct fitment integration like that, the ability to make mobile apps, where you can support any framework that you want to use. And so that's kind of an important thing if at your you know, startup, your company or, you know, whatever have you is using something that's, you know, anything that's specific, a certain UI library or whatever, you know, compared to like Lovable and V0, like Bolt can run anything.

**Eric Simons (Bolt CEO)** (01:04:13)

It can, you know, if you have your own custom design system, if you use Material UI or ShadCN or anything else, it can go and actually use those things. Whereas a lot of the other experiences, they kind of like lock them down to like only one thing. largely because of the issues around the compute side, because they have to pick up the cost for it. So they want to make sure you're not going to like run Bitcoin miners or something like that. Right. So, so typically, like I would say generally we're going to find this like tends to be a lot more reliable, a lot faster. It's extremely flexible kind of capabilities wise is like second to nine. I think it's good to like try all these things on, you know, kind of come up with your own, you know, perspective on it. But yeah, at least as of right now, like Bolt is, you know, by like DAUs and ARR is the number one, like web-based text app thing, yeah, by no small margin.

**Eric Simons (Bolt CEO)** (01:05:04)

And so I think that, I think it kind of speaks to like some of the stuff that I'm saying is like that it tends to be true just kind of from the market pull that we're seeing.

**Aakash Gupta** (01:05:14)

So yeah, I want to end with how people should be using this, and I'm going to go ahead and pitch my way, and then I'd love you to add any more color, which is all the PMs out there need to stop just thinking about PRDs as their output. I think like the new way is we always said like a picture is a thousand words. A prototype is 10,000 words. You know, if you can go out there and write a great PRD, maybe even with Bolt help and then plug that into Bolt and then you go share that out to executives. It's way easier to get buy in from executives or sales or customer success or. or even your own designer and tech lead about a particular thing if you come to them with a working prototype. And then on top of that, it's way easier for you to learn and get feedback because you can go put that prototype in the hands of users using a tool like user testing or something like that and iterate before you actually go ahead and ship the thing out to all of your users.

**Aakash Gupta** (01:06:21)

So that to me is like the killer use case for PMs today. Is that right? Did I miss anything there?

**Eric Simons (Bolt CEO)** (01:06:28)

I think you're dead right, right? Effectively, that's what we see a lot of PMs using it for, especially at existing companies, is rapid prototyping and going and building real POCs. They're not just some static thing that you're clicking through in Figma or whatever, but it's a real thing you put in someone's hand, whether it's a web app, a mobile app. um and because it just it helps it accelerates kind of getting buy-in from all the various stakeholders and like not just like having to believe in the vision but like seeing it right and um so that's a huge one and of course uh you're kind of beyond that too it's the code you're generating often is you know people are just taking that and that is the first version of the app right like they're using that as the scaffolding so anytime you're kind of going from zero to one whether it's you know a web app, a mobile app, if it's a marketing landing page, if it's like a dashboard, whatever, we see a lot of developers and PMs and designers coming to Bolt starting there to scaffold the 0.0 to 1.0 and then like going to cursor for the, you know, 1.0 to 1.1, you know, et cetera stuff.

**Eric Simons (Bolt CEO)** (01:07:34)

So I think those are like the kind of the primary use cases there. And of course, if you're starting your own startup, like there's a lot of like PMs that are using Bolt as kind of their technical co-founder and like going and they are building the MVP of their app and launching it and like making money, you know, integrating Stripe and, you know, whatever for their app. So actually taking you from idea all the way to production and, you know, launching. So I think that's the full spectrum of the stuff that we're seeing across the board.

**Aakash Gupta** (01:08:03)

I think that is the most exciting is outside your job, go build a side project. We've all been admiring levels, but you can do it now with a tool like Bull. Eric, thank you for ushering us into this crazy new reality. The world changed in October, 2024 when you guys released. So thank you. Yeah,

**Eric Simons (Bolt CEO)** (01:08:22)

you bet. Thank you for having me. I really appreciate it.
