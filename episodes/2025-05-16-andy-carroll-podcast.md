---
title: "Vibe Coding Tutorial in 72 mins, No Technical Background Needed (Windsurf)"
subtitle: "What if you could launch a product next week without writing a single line of code? Today, it's possible. Andy Carroll (16 year PM) is showing you exactly how to rock Windsurf."
date: "2025-05-16"
host: "Aakash Gupta"
guests: ["Andy Carroll"]
speaker_names: "substack"
substack_url: "https://www.news.aakashg.com/p/andy-carroll-podcast"
youtube_url: "https://www.youtube.com/watch?v=oLmHdymHHg0"
duration: "01:12:14"
word_count: 12043
source: "Substack episode transcript (aired audio)"
sponsors:
  - name: "Maven"
    url: "http://maven.com/x/aakash"
  - name: "Miro"
    url: "https://miro.com"
  - name: "Amplitude"
    url: "https://bit.ly/4hl25RG"
---

**Sponsors:** This episode is brought to you by [Maven](http://maven.com/x/aakash), [Miro](https://miro.com) and [Amplitude](https://bit.ly/4hl25RG).

# Vibe Coding Tutorial in 72 mins, No Technical Background Needed (Windsurf)

*What if you could launch a product next week without writing a single line of code? Today, it's possible. Andy Carroll (16 year PM) is showing you exactly how to rock Windsurf.*

**Aakash Gupta** (00:00:00)

What is

**Andy Carroll** (00:00:00)

vibe coding? I think it's really about humans and AI tools vibing together to create new products, new services, to bring new things to life. Business leaders overwhelmed with the amount of noise that they're hearing about AI. But many struggle how huge a time-saving this is. But to me, this just feels effortless, right? It's click a few buttons. And you do need to be really kind of careful, though. I've actually been working in product for about 16 years and didn't come from a technical background. So the right answer on the internet is to post the wrong answer.

**Aakash Gupta** (00:00:31)

Yes. The fastest way to get a good design is to put a bad design in front of your designer.

**Andy Carroll** (00:00:37)

Exactly. When we start out, let's define what it is that we're actually trying to achieve, what is going to make this unique, and let's focus almost all of our energy on making that part of the product really, really great.

**Aakash Gupta** (00:00:51)

In today's episode, I sit down with Andy Carroll, a PM of over 15 years, and we walk you through how to vibe code. We'll specifically use Windsurf and show you how you can deploy websites, create mobile applications. If you have been interested in learning more about vibe coding or Windsurf, and if you are a PM interested in understanding whether you should be vibe coding or using Windsurf, we will cover all of that. So without further ado, let's get into today's episode. Really quickly, I think a crazy stat is that more than 50% of you listening are not subscribed. If you can subscribe on YouTube, follow on Apple or Spotify podcasts, my commitment to you is that we'll continue to make this content better and better. And now on to today's episode. Andy Carroll, thank you so much for being here.

**Andy Carroll** (00:01:41)

Thank you, Akash. I'm extremely excited to be here.

**Aakash Gupta** (00:01:45)

We're both longtime PMs. Neither of us are particularly technical in our last few roles. And so today I want to break down something that a lot of people in our position might be looking at, vibe coding. What

**Andy Carroll** (00:01:57)

is vibe coding? Sure. I think you've hit the nail on the head. I've actually been working in product for about 16 years and didn't come from a technical background. I describe myself as technical enough to be dangerous, but to be able to have an informed conversation with engineers and with designers and to understand how things are built, but certainly not to really get stuck in and actually write the code myself. And I think one of the most transformative developments in the AI space over the last few months and years has been the introduction of these AI-powered integrated development tools like Replit and Cursor. bolt new lovable and the list goes on and on and um vibe coding is the process i think i think they may be drawing some inspiration from uh the jazz kind of movement but um i think it's it's really about humans and ai tools vibing together uh to create um new products new services to bring new things to life and um So certainly, although the term does make me cringe a little bit, for me, it really is about making something and really just sort of seeing where it takes you.

**Andy Carroll** (00:03:16)

So a lot of the time it's planning enough to get to the next step and then really being open to exploration. And this is where I think these AI tools are just, you know, unbelievable.

**Aakash Gupta** (00:03:28)

Yeah, I believe the term came from Andre Carpathy. He was early at OpenAI. He worked at Tesla AI. He himself is pretty technical, but he talks about this process of vibe coding where he just lets the tools do most of the coding. And so that's what I want to walk people through today. What is your tool of choice for vibe coding?

**Andy Carroll** (00:03:47)

Sure. So like I mentioned, there are many and I've probably forgotten quite a few. And as I said to you earlier, you kind of have to pick your weapon of choice. The one that I use most heavily is called Windsurf. I think the company that built it was called Codium and they may have rebranded as a result because Windsurf has become the flagship thing. But I suppose when I think about these tools, there are a number and they sort of hit different kind of moments, I think, in someone's exploration sort of journey. Starting out, I think one or two of the better ones for getting started quickly are probably V0 and Lovable. They have really amazing, I mean Replit similarly and Replit's got an amazing kind of mobile experience as well. Those are very easy places to start and to get something to do to put together a quick landing page.

**Andy Carroll** (00:04:46)

They've got an amazing community section where you can draw inspiration from other platforms. other things that have been built. But as soon, where I found myself a little bit limited was actually wanting to get into the full kind of stack and see exactly what was going on throughout sort of the code base. And I suppose Windsurf provides more of that experience. So it's more of a full powered kind of coding editor with an AI co-pilot that is also, which also provides access to all of the leading LLMs.

**Aakash Gupta** (00:05:17)

Awesome. So can we see this in action with a little bit of a live cooking session?

**Andy Carroll** (00:05:21)

Definitely. So a little bit of background quickly before we do that. So I'd say I created a GitHub account about, you know, like I said, 15, 16 years ago. And there wasn't a lot to see in my GitHub account except for a couple of cloned repos and a few other things that people had shared with me. And then just over the last sort of three, four months, and mainly the last two months, the number of things that I've started doing has really kind of exploded. And this is all thanks to live coding. So let me share my screen with you. Now, looking at this can be a little bit overwhelming. I think before I started doing this, I kind of I'd used VS Code as well, and so I had some familiarity there, but certainly looking at this was very much the same to me to begin with as looking over a developer's shoulder and seeing loads of complex things, file structures, as you can see over on the left-hand side, and various other things.

**Andy Carroll** (00:06:30)

But actually, in terms of a simple structure, what you have over here on the left-hand side is just a set of folders. These are just my sort of active... or some of the active projects that I've got running that I've added to my workspace. So these are the things that I'm currently using actively and developing. And like I said, to my point, I've probably got a few too many things going on, but this kind of gives you a sense of just how creative I think these tools can enable you to be and also how much you can achieve in a fraction of the time and with a fraction of the resources that was previously possible. And so if you go in here, so what I've got over here is a project for, you know, a few of the clients that I'm working for, as well as some of my private projects and sort of personal website.

**Andy Carroll** (00:07:22)

And then what Windsurf gives you is, so the co-pilot that I mentioned is called Cascade. And you can see over on the right hand side, top right corner. Over here you've got this little chat widget on the right hand side. So I'll just close the conversation that was open there. Now again it looks like there's quite a lot to look at but once you get the hang of it it takes a little bit of getting used to but it's actually pretty simple. You've got write over here. And as it says, when write mode's turned on, Cascade will be able to make changes to your code. This is crucial. I think I didn't realize that this existed for about the first 40 hours that I used the tool. And one of the things that I would say is that these tools do have a habit of being slightly overzealous in their, let's just say they're very proactive.

**Andy Carroll** (00:08:25)

So you could give it a prompt that said something like, hey, like I'm trying to change the font color over there on this page. And then suddenly the whole page would break. And then I'd say, well, you know, why did you do that? And it would just reply, oh, sorry, that was a mistake. You know, I just went in and refactored the entire landing page. So, dude, be quite careful. But chat is a safe place. So chat basically switches off access to all of the live coding editing capabilities. And like I mentioned, you then have access. And I know with Cursor, there's a similar thing. You've got access to all of the big ones. What I have noticed is that DeepSeek is not available in Cursor. And I don't think Grok is either. So I think that what you have access to here gives you a lot more sort of capability, a lot more variety.

**Andy Carroll** (00:09:17)

One of the things I do find is that different things are good for different sort of aspects of a project. And this is where I think, or this is what I found sets WindSurf apart from my initial experience with some of the other simpler tools. You know, what you have here is the ability. So for instance, you can see that you've got Claude 3.7 Sonnet, the thinking model, which is slightly more expensive. And then you've got DeepSeek R1 as well. Now, both of those models are really useful. I find when you want to go broad with something, for instance, if you just you really want to kind of you want to think something through without getting to a final answer in one shot. So often if I'm sort of trying to establish context, you know, saying, OK, well, I'm thinking about building this thing. Help me think through the different pros and cons of various tech stacks that I might choose.

**Andy Carroll** (00:10:06)

for that kind of thing going broad is really useful and what i've also found really amazing is just sort of seeing um how these things work right so as you're doing that and let's you know let's uh use that as an example so if i pick 3.7 sonnet and start having a chat um hi there um i and i'm i'm still probably overly polite i think there's something about um you know i do say please and thank you but maybe that's because of my fear of uh

<!-- sponsor -->
**Aakash Gupta** (00:10:32)

today's episode is brought to you by maven the problem with most courses online like udemy is there's no live component and the instructors aren't experts in their fields they're professors at maven you get direct live access to experts and operators from the world's best tech companies you can't get that access anywhere else in any university and you usually can't find them on youtube either i featured so many of maven's experts in the newsletter and podcast for that reason To help you out, I've put together a collection of courses I recommend at maven.com slash x slash Akash. This includes courses like AI prototyping for PMs, product sense for PMs, and getting an AI PM certification. Visit it now at maven.com slash x slash A-A-K-A-S-H. Today's episode is brought to you by Miro. Let me ask you something. How many tools are you juggling just to get a single project across the finish line?

<!-- sponsor -->
**Aakash Gupta** (00:11:27)

One for brainstorming, another for planning, something else for tracking tickets. That's where Miro comes in. It becomes an all-in-one collaboration workspace. Whether you're consolidating user research from several interviews, developing and synthesizing product briefs or a wireframe, or project managing development. Miro brings everyone into the same space. It's fast, intuitive, and fully loaded with features like project templates, two-way Jira Sync, and integration with software like Draw.io and PlantUML. Miro's AI features can be used to synthesize elements in a board to develop a ready-to-review product requirements document in seconds. If you're tired of tab overload and scattered workflows, try Miro. Head to Miro.com and see why over 90 million users choose Miro to guide from idea to outcome.

**Andy Carroll** (00:12:16)

The robot's taking over at some point, but I want to start a new project and want to build a full stack... Web app with mobile corresponding mobile applications. Talk

**Aakash Gupta** (00:12:49)

me through... so you want to start a new project you want to build a full stack web app with corresponding mobile app and you're

**Andy Carroll** (00:12:57)

going to talk me through the process uh you know ask me questions now typically you know um you know with the the idea of vibe coding here is very much you know you can start with uh an idea a very clear idea and we'll i think we'll get to one of those um in just a moment But you can also start with something completely open-ended and just get, you know, and just say, well, you know, and what's probably going to come back is, well, what do you want to achieve? Who might this be for? But you'll see here, so because I've got Claude 3.7 Sonnet thinking, you should see a thinking process there, right? The user wants to start a new project. Okay, cool. And then it goes back on itself and it goes, right, let's go. You know, what problem are you solving? Feature requirements.

**Andy Carroll** (00:13:39)

What are the three to five most critical feature requirements? Technical considerations, et cetera. Now, one of the big things that I've also been doing recently is actually to structure a series of prompts. I've got a very detailed prompt library as well, which I can show you over here, which is all around building out basically like the process of learning all of these things, some of them in really sort of painful and quite expensive ways. has made me get back to a lot of the basics of being a product manager. Sorry to interrupt.

**Aakash Gupta** (00:14:12)

Can you don't allow on that Riverside pop? I'm sorry. Sure. Sure. All right. Let's go back.

**Andy Carroll** (00:14:18)

No problem. So like I said, one of the things that one of the most expensive mistakes that I made actually when I started out using this was to dive in kind of headfirst with a bit of a, like, let's have a chat and cool, let's do that. And let's build, I don't know, let's build a React app, because I'd used React quite a bit. And obviously, it's very popular and well supported, etc. And I didn't actually run through some of the planning sort of process with any kind of real methodical rigor. and that really came back to bite me and actually you'll see like i may may get a chance to show you but i've had sort of two or three false starts with that specific project where i actually ended up having to just start again um and so what i've done now is actually built out a very detailed set of prompts which basically helps you you know and this is the kind of thing that i'd love to sort of share with uh with you and your users and and your audience but um It's really just something that I think can help people to structure their project in much the same way.

**Andy Carroll** (00:15:19)

And this is when I think about the value that this can provide. I'm thinking largely about not just sort of individuals trying to use this, but sometimes really non-technical sort of business founders who may not have any history of product management expertise. A lot of the things you can do with these, and this is where they really come into their own, is to actually prompt it with, you know, help to act as a CTO and advise me on the ideal tech stack. You know, that's one example. Or help me establish a sound kind of product vision and strategy. And, you know, and then I've got a few different frameworks, some common ones, jobs to be done, user story mapping. You don't need to do all of these either. So, you know, again, you know, you can probably get lost doing documentation forever, which is definitely not the goal.

**Andy Carroll** (00:16:02)

And Amazon PR FAQs, you know, working backwards type thing. But the real kind of thing to me is actually that starting with context, like really clear context and overinvesting in the planning process of actually setting this up pays for itself, you know, many, many times over. So I'll get back to Winsurf. What I'll do, I'll just bin that. Now, the thing that I created today was actually, and this goes back to my kind of, one of my initial sort of origin stories with using these products was actually two of my sons, I've got twin boys, play football on the weekends. And after one of the football games, one of the coaches put together a match report and um did so just you know manually wrote it wrote up a lovely match report highlighted each of the players contributions someone scored a hat trick you know various other things and shared that with everyone and all the parents loved it and someone said hey you should start a podcast you know have you got a thought of a career in journalism i thought well You know, I was just kicking the tires with lovable and a few other things.

**Andy Carroll** (00:17:01)

And I thought, well, actually, that could be quite a lot of fun. Like, why don't I, you know, why don't I think about a little AI sort of match reporter, which could be a thing that, you know, people might use. And I can show you the sort of first sort of version of that. which was this guy. But basically what I then ended up building was a very simple match report generator. So this is just a simple waiting list idea. And then basically you could run through, record your event, submit your details, generate a match report, both in terms of a written match report and then an audio one. And this was really my first kind of experience of building these things and using them to basically, you know, do whatever you want. And like I said, I ended up not really doing very much planning.

**Andy Carroll** (00:18:00)

And that really came back to bite me. But now what I do, so as you can see over on the left hand side, as I mentioned, you've got a series of projects and folders. And I created this new sort of fresh version of this AI Sport Reporter sort of project for us to use today. And one of the things that, as I've just mentioned, that I always do now is to produce a series of different documents. You know, really what you call these things I don't think really matters. But the common one is obviously that you have some kind of readme file, which is really just a... And as you can see, as you open that, it opens up in the middle. Let me just bring up Cascade on the right. So you can see that this is the typical kind of view that you have.

**Andy Carroll** (00:18:48)

So you've got code in the middle. You've got your chat on the right-hand side, and you can choose which model you're chatting to. And then you've got your file system on the left-hand side. And that really is all there is to it. Now, when you're chatting to LLM on the right-hand side to the model, you're basically going to be asking it to then make edits, code edits to these files over on the left-hand side. And as it starts doing so, it'll open the relevant file. But like I said, starting out, so I now will start with a series of sort of simple prompts. And like I said, I literally just did this yesterday. But putting together a strategy document, you know, what are we trying to achieve? Who's this for? So AI sport reporter transforms everyday sporting moments into professional shareable stories, core product principles, value proposition, target market, all of these things now.

**Andy Carroll** (00:19:42)

When I think back to doing a lot of these things as a product manager, you know, these things often frequently take many weeks to draft and review and decide and all of those things. And this is certainly not replacing the process of, you know, it's not saying to everyone, hey, you should just go off and vibe code on your computer on your own in isolation and come up with a product vision. But what it is doing is enabling people to go from zero to 90% or 80% very quickly. And I think that to me is what's so exciting about these tools is how they are collapsing the feedback cycle, not just in the sense of actually building new products, but also in all of the stuff around these products. So in addition to creating a product strategy and a project overview, I also then worked through what the architecture might look like.

**Andy Carroll** (00:20:36)

And to the point earlier about wanting a full stack web app and mobile apps, that was one of the things I didn't really think through very carefully first time up. And I started building in React and then realized I'm either going to need to go with React Native if I want to have an iOS app or an Android app, whatever. And actually one of the technologies that is also kind of in that single code base, multiple apps sort of space is Flutter. I've never used it before. But, you know, this is one of those opportunities. So actually what I've decided to do now is actually to use Flutter to develop this next incarnation, which, you know, is something that I'm planning to get live in the next week or so. And shall I stop there? Is there anything? Do you want me to just keep going?

**Andy Carroll** (00:21:21)

How did you develop these? Did you use AI to develop these? How much time did these take? So certainly sort of heavy use of AI and then tweaking things along the way, given what I know and what I've done before. There are obviously massive benefits of kind of knowing how these models and frameworks can be useful, which many who start out using these tools don't. And I think there's very well-documented information examples of people diving in and then just building something with AI and putting it live and then having massive security problems and various other things later. So a process here of basically sort of drafting some things and then chatting to AI and then building a repository of these things, which is sort of developing over time. So as I come across new things, I go, should I really need to formalize that? I basically just sort of add to that over time.

**Andy Carroll** (00:22:20)

But as you can see, you know, it's certainly not mandatory for everyone starting out to have, you know, seven or eight different files over here. You could very easily have one or two. But what is key is that you start with something that really kind of clarifies what you're trying to do. And then another really big development, sort of recent one actually, for me, has been to map out in a lot of detail a product roadmap, which then becomes a living document. And again, these are things that frequently take product teams many weeks to put together. And this is something that I put together in just a couple of hours. But what you can also see is that I've been updating it as I've been going and all the green check marks are things that I've done in just a few hours. And now I can see, okay, well, where am I going?

**Andy Carroll** (00:23:11)

In terms of what I've actually achieved, I've now set up a full Flutter project and structure. I didn't actually realize, and this is another big learning curve, I didn't realize how heavy, I suppose, the Flutter development framework actually is. It installs a huge number of things. Here you can see all of these Flutter build files. And I actually ran into quite a few sort of challenges with deployment. So that's actually another key lesson to really emphasize is that with V0 and Lovable and a couple of others, I think Replit, for instance, the process of putting something together and then just one hit deploy is seamless and really easy. You know, I don't know if it can go wrong, but certainly it's never gone wrong for me. Whereas one of the biggest kind of sort of head in hands learning moments with this tool was certainly that not getting something live, not deploying something, not sort of committing code to GitHub regularly, and then integrating with a hosting and deployment platform like GitHub.

**Andy Carroll** (00:24:26)

Netlify is the one that I use, but there's also Vercel, which is a very popular one. I've not used it personally. But what I would say is that getting a simple, I suppose, dev tool ecosystem together that you're comfortable with is a crucial sort of early step. Because what you want to do is to get the simplest version of the system live and deployed, and then to iterate in complexity, constantly sort of increasing what's in there, but making sure that there are those checkpoints. And the mistake that I made early on was that I was making loads of development changes and seeing how things were developing locally. And then as soon as it came to deploy, I had just hundreds of errors. I spent days trying to get the thing live and all sorts of refactoring. So again, this is also why I'm so passionate about this is because I'm now teaching other people how to use these tools.

**Andy Carroll** (00:25:29)

And I see people running into some of these problems early on, but I can spot them very early and I can help them avoid a lot of the pain that I experienced. um but yeah so so the other great thing about this and this is where i where i think a little bit about how these tools are so profoundly impactful for um sort of product teams is also that um if you use something like this and you you know github and um deployment pipelines and various other things were typically the domain of sort of the software engineers like i knew where they were but i didn't spend a lot of time actually looking at them i was more in notion or jira or wherever else um you know looking at you know how we were documenting things and visualizing what was going on in the roadmap and working through you know figma designs and and and those kinds of things um whereas what i've now been doing is is putting everything into these file systems so i've got this one one system kind of cockpit i suppose for driving all of the things that are open so as you can see on the left i've got this ai sports reporter i've now got all of my documents relating to to this including my prompt library so i go in here and i say okay cool you know this thing's enormous um but you know here he has a set of different prompts that i might want to use what's my architecture okay great um product strategy product overview roadmap Now, when you cross over to GitHub, I'll show you over here, you can see on the left-hand side that I've got exactly the same.

**Andy Carroll** (00:27:03)

Obviously, the whole repo, the whole thing's just been committed to the GitHub repo. But when you look at the roadmap, what's amazing now... is that I've got my roadmap perfectly laid out in a series of phases. Now I could turn this into a PowerPoint slide deck or whatever the case might be. But the fact is that anyone working on this project and anyone in the team now could be given access to this code base, this repo. So anyone can look at this and make sense of what's going on. Right. I know what you're doing. I know what the strategy is. I can challenge it if I want. But, you know, and here I can see. So here's what we're planning to do. You can see what's been ticked off and you can see what's in progress over here with a little progress sign. So. These are the kinds of things that, again, teams spend, I've been guilty of it.

**Andy Carroll** (00:27:48)

I know I've spent hours and weeks producing this kind of thing. And then what I've also done is actually created a little prompt, of course I have, which is to create a comprehensive project status report based on what you've achieved in the roadmap so far. And because you can run that in the context, so the whole system has all of the context for this project, you can say, review the roadmap, review the recent chat that we've been having, review all the files, and then provide a detailed report for our exec team. And what I've actually done, and it's something we don't need to demo here, but one of the things that I do now is that you can then take that detailed report. Here's an example output format. And then you can plug it into something like Gamma, which is the slide deck creation tool. And in moments, you know, instead of spending weeks on PowerPoint decks and whatever else, literally in 30 seconds, max a minute, you've got a beautiful detailed project summary for anyone's consumption, you know, to be able to share with anyone.

**Andy Carroll** (00:29:00)

And so let me quickly show you, because I'm sort of talking a lot about the tool itself, but let me show you the results. So this and, you know, we can certainly, we can change this live as we'd like to. But this is the thing that we've come up with that I've created, a simple landing page. So step one with this project was, okay, well, we want to build this whole multi-application kind of AI sport reporter tool, but that might take us at least a few days, probably a few weeks. If I think about kind of what many companies do with really big teams, you know most would look at that and go okay that's going to be a few months right i sort of i reckon that this is the kind of thing that might take two weeks but the first step for me is just okay well can we just validate whether there's actually something there so step one is just let's build a landing page and the prompt that i used to create this was really just i want to build a coming soon landing page i want it to look sort of modern and slick and whatever else give it some kind of interesting background with some kind of you know uh kind of treatment so it's gone a little bit wild with the colors um but as you can see so this coming soon the red doesn't look great on um on uh on the background over there so if i just and this is the beauty of this right so i'll just say okay cool let me take a screenshot of that now um let me go back to cascade um where are you okay um sorry i

<!-- sponsor -->
**Aakash Gupta** (00:30:31)

don't want that Today's episode is brought to you by Amplitude. Building great digital products is hard. You know that better than anyone. Getting teams aligned, measuring what matters, and scaling your product strategy isn't easy. But what if you had a clear framework to guide your next steps? That's exactly what Amplitude built. They studied the best product teams to understand what really drives impact. And turned those insights into the Digital Experience Maturity Assessment. In two minutes, you'll be able to see where your team stands and what you can improve to build better products faster. Click the link in the caption to take the free assessment and get a clear path to product growth.

**Andy Carroll** (00:31:10)

Here we go. Back to AI. AI. So you asked her to go back to AI Sport Reporter. Yeah, exactly. So, I mean, that's another key point is that working with this tool, like what is really important is that, so as you can see here, now it's re-familiarizing itself with everything in the project. I have had, and this again is something that, you know, probably beyond the scope of this chat maybe, but... getting into managing the memories that the tool has. So there's a couple of different things that I didn't really sort of understand or really know or pick up existed early on. I knew that I had to provide a lot of context. But what ended up happening was it was auto generating these memories of certain projects. And then sometimes when I was in the middle of coding a landing page for one product, it would just spit out a whole pile of content for something else.

**Andy Carroll** (00:32:26)

And I'd be like, what? You know what I mean? Like literally one of my clients is a fitness business for prenatal and postnatal sort of mum transformations. And that's quite different to another project, which is about AI driven talent acquisition, which we're working on. And you can imagine that those two things can create quite interesting results when they mix. So what is really important is that when people come back to this, they then re-familiarize the tool with what they're working on. So let's look at the landing page. This coming soon doesn't look good on a red background. Let me just change models here, like I said. So I've typically used Claude 3.7 most of the time. What I have found quite useful, actually, and one of the big benefits as well, is sometimes when you get stuck sort of debugging something or whatever, for some reason, if you throw a different model at a problem that another one's been struggling with, it can actually, I think it uses the previous context and the things that the other models tried to And then, you know, so sometimes I find if I'm stuck with 3.7, I'll then switch over to 4.0, to OpenAI's 4.0, GPT 4.0.

**Andy Carroll** (00:33:53)

And it'll, for some reason, just move forward. So that's one of those little sort of tips that I found actually really helps. So let's look at the landing page. As you can see, some of the models accept sort of screenshots. Some of them don't. So let's look at the landing page. This coming soon doesn't look good on a red background.

**Aakash Gupta** (00:34:14)

So 3.7 does accept screenshots, luckily.

**Andy Carroll** (00:34:17)

Exactly, and so does 4.0. So let's examine the learning page, okay? Yeah, okay. So let me just do something quickly. Don't change the background. Please change the text's color to a dark charcoal. Okay. And as you can see, that's going to be happening now. Like I said earlier, it's going to... Oh, sorry, I'm in chat mode. So let me just switch over. So key point there, it was trying to make the change, but it actually couldn't. So make the change directly...

**Aakash Gupta** (00:35:15)

So once we switch it over to write mode, it's able to directly change those code files.

**Andy Carroll** (00:35:20)

Exactly. And so what you'll see, the file opened over here, you can see the change. And this, I think, also gets to the key excitement for me has been, as I mentioned, this kind of Cambrian explosion of learning. But I've actually just been learning by doing rather than something theoretical. So sort of seeing exactly what gets changed and how it works, you know, You know, I started out by, I suppose, leaning heavily and just letting the AI do all of the coding. And latterly, I've started making small tweaks myself kind of manually and then getting the code to, you know, getting the AI to check that I didn't mess anything up. And some of the time, you know, it's like I changed the title over there and it'll pick up immediately and it'll say, You change the title over there, but there's a JavaScript script that actually picks up that title, the old title, and uses it.

**Andy Carroll** (00:36:14)

So the build process is going to now fail. And so there's all of these kinds of things where it spots these dependencies. Not always, but it teaches you as you go what to look out for. And so often I'll go in now and I'll say, look, I'd like to change that title. Are there any dependencies or is there anything else I need to be aware of? Here we go. So what's happened now, as you can see now, I haven't walked you through the full kind of setup process. I've actually like what I think is a better use of people's time if they are interested. I've actually got a separate guide on some of that. And then also the windsurf kind of getting started guide is a good place to start. But basically, like I mentioned, the major thing that you want to do early on is make sure you've got a GitHub account, free to set up and very easy.

**Andy Carroll** (00:37:04)

And to create, I recommend Netlify. I've been really impressed with everything that they've done. But, you know, we can share all of those details later. But basically, once you've got the Windsurf integrated with GitHub, you're good to go with a local kind of code repository and being able to push those changes to a remote repository. And then what you do is you set up Netlify to automatically pull. So you set up a sort of CICD kind of pipeline within Netlify. And let me just show you that because it should have started building now. Here you go. So you can see the range of different projects that I've got open. And like I said, a couple of months ago, I didn't have anything that I'd built beyond a simple kind of personal website. And now these are the things that are going on. You can see that within Netlify, you can see now that that change, which was pushed automatically to GitHub, has not triggered a build on the production pipeline, the production deploy here.

**Andy Carroll** (00:38:08)

And you can see that it's also added a nice little commit comment, coming soon text color to dark charcoal for better contrast. And that's another really key habit that I think is easy to miss is sometimes you get so excited about making changes that then something breaks and you go, when was the last time that I actually committed to GitHub? And that's something that, you know, really kind of I've become fairly sort of I probably have over indexed now on committing too frequently. And I'm sure some of your developers will tell me that my, you know, my technique is not sort of quite perfect. But I find it very useful. So you can see here that it's now initialized. And there you can see that coming soon has been changed. Now, it's obviously a little bit of a wait to have to see the full kind of deployment to production process.

**Andy Carroll** (00:39:03)

What I'm going to do is just ask Windsurf to bring this up on a local port. Can you get this up on local 8000? I think that's the one I was using.

**Aakash Gupta** (00:39:20)

And the difference here is what we saw was live on the web deployed via Netlify. Exactly.

**Andy Carroll** (00:39:25)

Look at

**Aakash Gupta** (00:39:26)

it locally.

**Andy Carroll** (00:39:27)

Exactly. So you can see over here, you know, Netlify has just given it a little Netlify app, but I've called it a sport report. But what you can do as well with Netlify, which is amazing, is that you can choose your own custom domain, even on the free tier on Netlify. I don't know if there's limits as to the number of sites that you can use. But certainly, I don't think that that's offensive. I wouldn't sort of not click on it if I wanted the product. But it is always nice to be able to have your own custom domain on something that you want to look kind of really pro. And so let me just see if that's come up. Okay, so another key point, actually, which is around the idea of this being a fully integrated development environment is the fact that terminal... You can run terminal as a separate window.

**Andy Carroll** (00:40:24)

So you can open terminal and basically it'll open your terminal view. But what you can also do is hit it directly from within the chat. So here you can see it's come up with the command. And this just saves you having to use a separate product, right? So again, back to just bringing everything into one place. Instead of jumping around between four or five different things, one for notes and one for strategy documents and the mirror board and whatever, it's just all here. And from a coding perspective, it's very similar. So running the background terminal command, so it's bringing that up. Okay, let's see this. Localhost 8000. Okay, so now we've got that. Now when we make changes in here locally, obviously those will appear immediately. So why don't we sort of take a look at this now? I suppose if you were to look at this for the first time, And actually, one thing that sort of sprang out to me earlier was one of the things that many product teams, I think, spend a huge amount of time doing, certainly early businesses, is on coming up with kind of design systems and brand logos and various other things, especially for new businesses, for new products.

**Andy Carroll** (00:41:46)

And in my mind, that's actually a really kind of low value activity until you validate it that there's actually something that other people want. So again, what I've done is just created a simple, so sort of thinking about people who want to start this out or want to experiment with some kind of, you know, set up your own sort of site. I've actually created just a little AI prompt, again, which is somewhere in here, which enables you to sort of create a brand logo. So a little bit further down. But so our print library brand logo. So Hulk founders quickly create a simple professional SVG based logo in Favicon. So let's just put that in here. Focus on creating something simple, distinctive. The logo should be professional enough to establish credibility, but can evolve as the company grows. Let's just put that in here. Okay. I'd be happy to help you create a simple professional.

**Andy Carroll** (00:42:43)

What's your startup product name? Okay. It's already got all of that. You have all these answers. Obviously, if I was doing this for a new business, I would spend more than five minutes or more than 30 seconds doing this. You have all these answers. Yeah, so okay. It gave me a little prompt. I'm creating a logo for AirSporter. Great. so it's parents color preferences cool using a gradient style preferences symbols or imagery competitors and you can see here that it's got some suggested actions right and again back to you know if you're doing this on your own and you don't have access to a designer or your design is busy and actually you know you don't want to wait two days to get something done and This is the kind of thing that can enable you to just get something good enough to start the process.

**Andy Carroll** (00:43:37)

I mean, a colleague of mine used to also say that the fastest way to get to the right answer on the internet is to post the wrong answer.

**Aakash Gupta** (00:43:45)

Yes. The fastest way to get a good design is to put a bad design in front of your designer.

**Andy Carroll** (00:43:51)

Exactly. So, you know, I don't know. I like concept one. I didn't even read them, but I'm sure it's good enough. now i'm still in right mode i should be able so it's going to give me the svg code for my logo there's no you know i'm not running through some separate tool to do this um you know who knows what the result is going to be but it's given me that and it's also given me a favicon um To be honest, it almost gives you a little bit too much information. Yeah. But this is what's been a lot of fun. Okay, great. So... Yes, please implement the new brand logo and favicon. The logo should be top left of the website and should, yeah, okay, that's fine for now. I actually don't, it doesn't need to resolve to a homepage. For now, but I suppose, you know, the other thing that you end up having to do is to work through kind of navigation structures and that kind of thing.

**Andy Carroll** (00:45:14)

Now, okay, it's creating a favicon file and that's being put into the, as you can see, static landing and it's created an assets folder. So it's doing all of this automatically. I'm not messing around with file structures and that kind of thing. You often do find that you have to start moving things around a little bit later because sometimes it gets things wrong. But, I mean, if you just kind of think about, I don't know if you've ever had a similar experience where deliberation over what we're going to call it or what the brand might be takes up almost as much time as talking about what the product should do. And I think that's what you're trying to get out of, really. So here you go. The new logo perfectly captures the essence of AI Sports Reporter. The other thing is that these, you know, they are amazingly optimistic at all times.

**Andy Carroll** (00:46:14)

Right, let's see. So I'll just clear cache over there. Has it been applied? Ah, okay. Not sure that that's what I would have gone for. But it's a logo. Exactly. So I've got a logo and you can see that it's got a little favicon up in the top left, you know, of the tile. Now, what are some other things that I suppose people are going to be thinking about? If you were coming to this fresh and going, cool, what does transform sports moments into stories? Maybe we can co-create a little feature together.

**Aakash Gupta** (00:46:49)

I think it would be cool maybe to have an infographic explaining what's going on, right? So I think maybe we show... Input, recording of match, output, match report, something like that, that we

**Andy Carroll** (00:47:06)

put in. For the homepage, we need some kind of how it works infographic that can walk users through the iLevel. I'm walking you through the high-level process and what it entails, step by step, what to expect.

**Aakash Gupta** (00:48:06)

Okay, how is it dealing with our infographic?

**Andy Carroll** (00:48:09)

Yeah. So, I mean, like, you know, again, it's sort of gone through and this gets back to kind of if I was to do this with the team, right, often this is just a great starting point for what are we trying to achieve here? Now, you know, capture the moment, input key details, AI magic happens, choose your format, you know, text, audio, PDF, and then share and celebrate. Right. So nice, really nice little summary, right, of what's actually required in 10 seconds. Design considerations, right? Layout options, placement on the landing page, free versus premium indication. Okay. Now, just for the purposes of time today, obviously, we could spend a bit more time deliberating. Okay. I'll take your stare on this. Okay. Sounds good. Let's keep it clean.

**Aakash Gupta** (00:49:07)

And I see that little accept all button. Is that another way to do

**Andy Carroll** (00:49:11)

it? Yes. So actually, so that's just telling me that three files have actually been changed. So those were, it basically created the brand logo and the favicon logo. And there are a few other little things. So the index file also changed, which you can see over here. So it's been modified. That little M over on the left-hand side. And that gives you a nice little visual cue of when something's changed, a code change that may not yet have been committed to GitHub. And so when you start seeing that you've got 10 of those open, you know that it's probably time to push. Let's keep it keen and simple for now. We don't have any graphics at the moment, so use... These are probably not my best quality prompts either, but we'll see where we get to. I'll blame you if it doesn't look good.

**Aakash Gupta** (00:50:21)

Quality of the prompt is everything, right?

**Andy Carroll** (00:50:24)

Always. I think this is also why the usefulness of having a detailed prompt library is really powerful. It's something that you can basically refer back to at all times, but just knowing that... You know, you don't need to think all of it. There are established ways of thinking through many of these things. And it's just so useful to be able to kind of do something like that, see what the output is, keep some of it, you know, delete some if you don't want it. But it really is very powerful. as a tool. So it's generating that at the moment. I think what might also be useful is we'll add a little FAQ section or something like that down at the bottom, and then maybe we'll keep it to a single page. I don't want to introduce too much complexity now, but we can add anchor points to a hard work section and an FAQ section and something like that, and maybe something else lower down on the page.

**Andy Carroll** (00:51:25)

Now, obviously, time doesn't permit us to go in and build the full kind of AI experience. But some of the key components, I've mentioned GitHub, I've mentioned Netlify. Another sort of major thing is obviously to have some kind of back-end database system in place as well. The tool that I've been using is Superbase. Again, there are a few different options. I've heard of a serverless option called Neon, which I've not tried myself. But I think, again, it's about sort of picking your weapon and getting comfortable with something. You know, there is also the option to integrate with something like Airtable as a very lightweight, kind of, I suppose, less technical option, especially for something like... So something like a sort of content driven, you know, marketing type site or whatever, where there may just be the need to update certain sort of content elements, but actually you'd rather have something that's slightly more user friendly from a CMS perspective.

**Andy Carroll** (00:52:31)

that can be really useful. But if you actually want a fully-fledged, fully-featured sort of database structure with everything required to store user details securely and everything else, having a SuperBase account is a really important step. All righty, hard works. Let's see what we've got. Looks great.

**Aakash Gupta** (00:53:00)

So we're hitting accept on a few things.

**Andy Carroll** (00:53:02)

Accept, accept. Now these are just, it's committing sort of, these are terminal commands. Typically, you know, what someone would be doing without this is typing all of these things manually into terminal, I believe. Again, not having done this outside of this tool, I'm not sure how huge a time-saving this is, but to me this just feels effortless, right? Let's click a few buttons and... You do need to be really kind of careful, though. And so this is another thing that I've learned is you do actually need to familiarize yourself with some of the key sort of commands, because some of the time it just recommends doing something that you immediately know it shouldn't. And some of those things can be quite difficult to undo if you get them wrong. Let's see what we got. So how it works. Capture the moment. Take quick notes or photos during the game.

**Andy Carroll** (00:53:54)

Input key details. AI magic happens. Choose your format. Share and celebrate.

**Aakash Gupta** (00:53:59)

Amazing. So interactive, too. So it's not just like random little things when we hovered over it, it did it. So that covers our walkthrough of vibe coding. People have got to see us ship features live. We shipped a logo. We shipped interactive walkthrough of what the app actually does. If you were

**Andy Carroll** (00:54:20)

to

**Aakash Gupta** (00:54:20)

summarize, what is the power of these tools and how should people be thinking about using them?

**Andy Carroll** (00:54:26)

Absolutely. So I think this is where I'm kind of most excited about all of this is that I'm passionate about helping people and teams to do more with less, to create more. And I think a lot of people are thinking of AI as something that's taking away human creativity. I'm actually passionate about the ability of these tools to make people more creative and to enable them to explore more ideas more quickly. I've worked in various product environments where it may not have been a one-to-one mapping of ideas to production code, but sometimes it was pretty close. And a lot of that came down to the cost of experimentation, the cost of getting feedback. There's a big overhead there and there's often a big pressure to deliver. And what that often does is that it sort of pressurizes teams to commit too early to an idea that hasn't yet really been explored.

**Andy Carroll** (00:55:24)

And some of the things I've shown you today, I think, I hope have shown you how very quickly you can, you know, and I think the really big thing to your question about like, how are these things most useful? I think, is to align people around a common goal really early. I think there are going to be some barriers to access, but getting people to use the same set of tools, I think, is really key. So where the benefit, I think, is going to lie and where I'm hearing of people facing challenges is that People are kicking the tires with certain tools, but you might have five different people in the same team all using a different tool to try and bring to life a new idea. Where I think the huge kind of benefits are going to lie will be when teams can establish a shared mental model and playbook and sort of toolkit for how to use these things effectively.

**Andy Carroll** (00:56:18)

And that's where I think true transformation can take place. Can somebody monetize

**Aakash Gupta** (00:56:24)

an app with Vibe Coding?

**Andy Carroll** (00:56:27)

I think there's good examples of that happening at the moment. There's, is it Peter Levels is a well-documented sort of celebrity, I think, in the vibe coding space. And there are a few others as well. You know, you spend a bit of time on X and I think there's a whole thriving communities. I think there's another guy named John Rush who I follow quite closely because he's doing Some really great stuff in the space, you know, building an ultra lean. I don't know if it's a one person business, but it's, you know, it's him and maybe one or two others. And he has, you know, 10, 15 different projects running at any point in time. And I think Peter Levels similarly talks about how quickly he will trial something. And then just with zero emotion, just kill it if it doesn't work. Right. And he just said that's one of the big things for him is actually I'm going to go out with a hypothesis.

**Andy Carroll** (00:57:25)

I might pivot here early on. But if it proves if people just don't really want it or I haven't quite nailed the solution, that's OK. Right. And I can cut and I can reload. So I think yes is the answer. I think that's just one example, building products and getting them live, you know, micro SaaS type propositions where you can get something live in a weekend that solves a specific customer problem, just one problem, but does so really well. That's the kind of thing that people will definitely pay for. And then I think the other side of this is doing, you know, largely what I'm focusing on at the moment. I think helping others to build these products and services quickly and then also establish the processes around using them. So I think there's a few different sort of monetization options in this space. And aside from that, it's also just, you know, addictively fun.

**Aakash Gupta** (00:58:18)

Yeah, John Rush is coming on the podcast. He has agreed to come on the podcast.

**Andy Carroll** (00:58:22)

I

**Aakash Gupta** (00:58:22)

think his episode will come out like two months after this. So I'll

**Andy Carroll** (00:58:26)

give

**Aakash Gupta** (00:58:26)

you a little teaser for you all about the John Rush episode. And hopefully Levels is listening and we'll get him on as a result as well.

**Andy Carroll** (00:58:34)

How

**Aakash Gupta** (00:58:34)

should PMs think about using

**Andy Carroll** (00:58:37)

these tools? Good question. It's something I'm grappling with at the moment. I think, you know, you... You really want to empower people to explore things more freely, but also to focus on the stuff that actually drives differentiation and value. And I think with a lot of these tools, what I'm finding most powerful, and certainly something that I think I've been guilty of in the past, is thinking that everything in the product that I was building was actually unique. Everything deserved the same amount of attention. And the fact is, you know, that's just not the case, right? And I think the way that I like to think about this is that you can almost remix and borrow and pick from, you know, choose, draw inspiration from other things very quickly. So it might be we need a landing page. Let's not spend two weeks on it, right?

**Andy Carroll** (00:59:32)

There are 30 examples. I can take a screenshot of a great landing page and I can get it live in an afternoon. If we want to change it, that's fine. But I think the ability to then say, okay, well, When we start out, right, let's define what it is that we're actually trying to achieve, what is going to make this unique. And let's focus almost all of our energy on making that part of the product really, really great. Right. And these tools, I think, enable you to, I suppose, eliminate 90 percent of the busy work and the sort of the drudgery so that product managers can actually focus everyone on the stuff that really is the secret source, the stuff that their customers really want.

**Aakash Gupta** (01:00:09)

So you've been a PM since 2008, actually, coincidentally, when I started as a product manager as well. What shifts have you seen in product management? And do you think vibe coding will be one of those shifts?

**Andy Carroll** (01:00:22)

Um... Yes, so 2008 was an interesting year for me because I got into product very much accidentally by losing my job in finance as a result of the trading business that I was working for closing down. I'd been in London for 10 days, so I'm South African, had moved here and had envisaged myself working in finance as a trader. And 10 days in, I was handed a cardboard box and told that the company was no longer. But they said, you know, do you want to fly back to South Africa or do you want to stick it out on your own and just sort of find your feet? And so I chose the latter. And a friend of mine was actually working at a music startup of all things. And it was kind of the early heady days. post Napster, but pre Spotify and Apple Music and various other things.

**Andy Carroll** (01:01:20)

And certainly everyone knew that the world was shifting to a digital, you know, the music world is going to be shifting to a digital model, but no one really knew how. So he said, look, we are completely oversubscribed. We've got, you know, everyone wants what we're doing. We're a small startup in West London and, you know, all of the world's hardware manufacturers and mobile phone networks and everyone else wants digital music. So we've got way too much, you know, if you can start soon and basically, you know, without really having a job title, that'll be great. And so, like I say, like I joined the Take Startup. I was still wearing a suit at the time and that only lasted about a day because everyone was wearing sort of hoodies and T-shirts and wondering, you know, who the finance guy was. And I sat down with various others in that space.

**Andy Carroll** (01:02:10)

And just within a couple of weeks, I realized that this kind of job of working with... I was given an assignment to work with the design team on something and then to work with the QA team and then to work with the developers. And coordinating all of those things to then ultimately bring a product to market was the thing that I learned there. And over the last 15 years, so I think early on, we didn't really have a job description of product manager. So my first, it was about six months in, I was actually told, well, actually, the thing you're doing is kind of, you know, this thing called product management. And we have a new product that's going to be going live. And we think you'd be really good at kind of taking the reins on that. And I think, you know, very big shifts sort of took place both while I was there.

**Andy Carroll** (01:02:58)

But, you know, the agile movement was actually sort of fairly, fairly new, you know, certainly something that, you know, wasn't something that had been formalized or certainly wasn't practiced everywhere as it more commonly is now. But in terms of real development, I don't think that I've seen a shift, anything like what the potential of this new sort of vibe coding kind of movement, I think, can provide. I think in terms of shifting people out of a delivery focused mindset where everything is about measuring velocity and tickets delivered, et cetera, rather than sort of actual demonstrable value. I think, yeah, I mean, to answer the question, I don't know that there's been a shift quite like the one that we're seeing right now.

**Aakash Gupta** (01:03:52)

Agreed. I think it's allowing PMs to get back to bare metal. You know, we spent so much time in the documentation and stuff like that, but it's nice to actually get back into the pixels, into the product. Yeah, no, exactly. So what are you up to today? You're running Aisle Partners. What is that?

**Andy Carroll** (01:04:13)

So, yeah, so sort of 15, 16 years in or after building and leading product teams in various sort of startups and corporates and a bit of time in consulting as well. I sort of went out on my own last year. So it's still sort of very, very early days, but really kind of focusing on everything we've been talking about today, but very much. So what we do is what we offer is a combination of highly targeted sort of AI training for typically mid-sized businesses, but a couple of our clients are quite a bit bigger. And then we also offer a combination of training and then also implementation. So sort of agentic AI and automation tooling, very targeted to building, I suppose you might call them sort of hybrid teams, but digital human kind of hybrid teams. to help businesses, you know, like I said, do more with less.

**Andy Carroll** (01:05:16)

And I think, you know, a big part of this has been kind of in response to what we hear really frequently is that many businesses or business leaders are overwhelmed with the amount of noise that they're hearing about AI, but many struggle to actually know how to apply it to what they're doing. And a lot of these tools and capabilities can also be introduced without requiring monstrous upfront sort of planning processes and whatever else. And there's almost a bit of a collision of how these things can be introduced in a matter of days or weeks. to win back enormous amounts of time for an entire team. And really like what we're hearing is a lot of businesses spend more time planning and talking about AI than they actually do implementing. So that's kind of what we've been set up to address is really help people kind of cut 90% of the discussion and the workshops and the massive sort of detailed upfront planning.

**Andy Carroll** (01:06:15)

And what we do is go in and say, right, your specific team in your specific industry, your marketing team, for instance, is doing certain things. Talk us through what they're doing. What tools are they using? What are they trying to achieve? And then we help them very quickly map out. how those processes can be improved with a goal of typically sort of winning back sort of two to four hours per person in the team within two to four weeks of engaging and if you think about it you only need to do that two or three times and then everyone in that team has a four-day work week you know and and that's the kind of model that um you know so the roi on what we can deliver is massive But really, it's that combination of, you know, high quality training, targeted training, and then also implementation.

**Andy Carroll** (01:07:01)

And then the other thing that I'm doing sort of personally is more in product and digital kind of strategy consulting, or with a view to introducing these tools to teams and helping them to get up and running fast.

**Aakash Gupta** (01:07:13)

And what I've noticed is that the retention, the viewers who are retained to this point, it's something like 20, 25 percent. An abnormal amount of them are like us. They're thinking about, oh, should I do consulting? Should I stay a full time PM? How has that shift been for you? Have you been able to earn as much as you were earning before? Has it been as rewarding?

**Andy Carroll** (01:07:35)

um it's i mean really really challenging to be honest um just because it has been so so different i think um very early on um i actually um you know managed to get a few early clients out of um just word of mouth and basic sort of just organic network just discussions about what i was doing and people knew who I was and so certainly a lot of kind of our early business has been that way but other parts of the sort of the more challenging side of things have certainly been to do with personal brand development so I feel like I'm very much in the sort of starting phases of really kind of getting out and publicly sharing my knowledge and establishing myself as a I suppose, a thought leader in the space. That's one of the things that I think is really challenging, but pays enormous dividends.

**Andy Carroll** (01:08:29)

This conversation, for instance, was the result of me just engaging with the chats on LinkedIn and you responding, which I think is amazing. And I think a lot more people need to realize that. So I think... Some of the guidance that I might provide is that I think I sat around on LinkedIn consuming a lot and maybe posting here and there. And I actually think that people have more to say than they think they do a lot of the time. And I certainly was very guilty, I still am, of overthinking a lot of things. And sometimes you don't need to write an essay every time you want to post something. If something's on your mind... If you've had a great conversation with someone, you know, put it out there. You might get three sort of reactions, you might get 50, but it doesn't really matter. I think it's much more about the compounding impact of actually just being seen.

**Andy Carroll** (01:09:15)

So that would be sort of one big difference. In terms of sort of financial sort of rewards, et cetera, very much kind of level with where I was previously, but I think that the potential upside is And I mean, bearing in mind I'm just a few months in, that's been gratifying. But certainly the kind of the need to balance pipeline development with existing client work is a really challenging kind of balance to get used to. You know, you can't drop the ball with existing clients, but equally, you've got to make sure that you've got new things coming in. So that's something that you don't face if you're working for a company where you've got a guaranteed salary at the end of the month. And then the other side of it, like the final thing to me has really been about lifestyle flexibility. I would say at the moment I'm working much longer hours, but much more flexibly than I was before.

**Andy Carroll** (01:10:15)

And I'm planning to certainly sort of dial things down as I start to kind of firm up a lot of the systems required to be able to operate the business much more efficiently. um but yeah i've got three young kids um and it's been amazing for me to be able to say well you know i'm just going to be there that afternoon or whatever the case might be um so from that point of view you know it's been it's been really amazing um the last thing is really about variety uh i've loved the fact that i am now just talking to meeting like just so many different people who face this common themes in some of the problems but also I'm dealing with so many different, more, I suppose, a broader variety of different things, which is great.

**Aakash Gupta** (01:10:58)

Really resonates with my experience.

**Andy Carroll** (01:11:00)

The

**Aakash Gupta** (01:11:00)

first year of going independent, I was probably working way more than I used to work. Now that I've figured out some of the systems, it's better, but that doesn't mean that selling podcast ads isn't a slog that I need to keep doing, doing all this work. There's so many different things that go on with creating your own business. But this has been an awesome introduction into Vibe Coding with Windsurf. Andy, thank you so much.

**Andy Carroll** (01:11:26)

It's an absolute pleasure. It's been really good to be here. Thank you, Arkash. We'll be in touch.

**Aakash Gupta** (01:11:32)

All right. Bye, everyone. Bye,

**Andy Carroll** (01:11:34)

everyone.

**Aakash Gupta** (01:11:35)

I really hope you guys enjoyed that episode. It would mean a ton to me and the team if you could please subscribe on YouTube, follow on Apple and Spotify podcasts and leave a rating and review. Those ratings and reviews really help grow the show and help other people discover the show. And they help fund the production so that we can do bigger and better productions. Can't wait to share the next episode with you. Until then, see you later.
