---
title: "How to Design like OpenAI and Figma"
subtitle: "Ed Bayers leads design on Codex at OpenAI and Gui Seiz leads AI design at Figma. Today, they drop a masterclass on the new design workflow"
date: "2026-04-10"
host: "Aakash Gupta"
guests: ["Guest 2", "Guest"]
speaker_names: "inferred"
substack_url: "https://www.news.aakashg.com/p/ed-bayes-gui-seiz-podcast"
youtube_url: "https://www.youtube.com/watch?v=C_eXo6oCvRA"
duration: "00:53:35"
word_count: 10680
source: "Substack episode transcript (aired audio)"
sponsors:
  - name: "Bolt"
    url: "https://bolt.new/solutions/product-manager?utm_source=Promoted&utm_medium=email&utm_campaign=aakash-product-growth"
  - name: "Pendo"
    url: "http://www.pendo.io/aakash"
  - name: "NayaOne"
    url: "https://nayaone.com/aakash/"
  - name: "AI PM Certification"
    url: "https://maven.com/product-faculty/ai-product-management-certification?promoCode=AAKASH550C7"
---

**Sponsors:** This episode is brought to you by [Bolt](https://bolt.new/solutions/product-manager?utm_source=Promoted&utm_medium=email&utm_campaign=aakash-product-growth), [Pendo](http://www.pendo.io/aakash), [NayaOne](https://nayaone.com/aakash/) and [AI PM Certification](https://maven.com/product-faculty/ai-product-management-certification?promoCode=AAKASH550C7).

# How to Design like OpenAI and Figma

*Ed Bayers leads design on Codex at OpenAI and Gui Seiz leads AI design at Figma. Today, they drop a masterclass on the new design workflow*

**Aakash Gupta** (00:00:00)

So there's this debate that I'm seeing with the new wave of designers. What is your guys take on this design in code versus design in the canvas debate?

**Guest 2** (00:00:08)

And the Overton window has shifted so quickly from my teams being AI curious to like banging down the door. They can't move fast enough without it.

**Guest** (00:00:16)

Developers have been accelerated, say, like 10x. Designers have maybe been accelerated, like 1.5 or 2x. So, you know, design can become the bottleneck.

**Aakash Gupta** (00:00:23)

This is Ed Baes, Head of Design for Codex at OpenAI. And this is Guy Sayed, Head of Design for AI at Figma. Where is the line now? These designer and engineer roles are clearly merging.

**Guest 2** (00:00:37)

The empowerment that has come from AI has meant that this idea of roles and rigid old structures is kind of slight starting to diffuse a little more.

**Guest** (00:00:45)

Yeah, I would agree with a lot of that. I can then copy a link to this component, and then I can just paste it in here and say, update my code with change I made here. I also think it's a really fun time to be a designer because your imagination really is the only upper limit.

**Guest 2** (00:01:00)

Now I don't need to. Now I can just ask a question and be like, can you build this? And if it starts to do something, I can ask,

<!-- sponsor -->
**Aakash Gupta** (00:01:11)

Before we go any further, do me a favor and check that you are subscribed on YouTube and following on Apple and Spotify podcasts. And if you want to get access to amazing AI tools, check out my bundle, where if you become an annual subscriber to my newsletter, you get a full year free of the paid plans of Mobbin, Arise, RelayApp, Dovetail, Linear, Magic Patterns, Deep Sky, Reforge Build, Descript, and Speechify. So be sure to check that out at bundle.akashji.com. And now into today's episode. When should you start in code and when should you start in Canvas? What does this step-by-step roadmap look like for designing in the new AI design workflow? And how should PMs be working with designers and engineers in 2026? They share everything. There's a million people talking about design with AI, but few sit at the frontier like Ed Baes and Guy Sayes.

<!-- sponsor -->
**Aakash Gupta** (00:02:03)

Ed is the head of design for Codex at OpenAI and Guy Sayes is the head of design for AI at Figma. These are the two companies defining the future of AI design. And today they're answering how you should design with AI, how you should move from Codex to Figma and back again, how you should start in code and when you should start in Canvas. They're giving you the roadmap so that as you are designing any product, you can design it with the latest and greatest tools. This is never before seen access and they rarely do podcasts. You're getting a once in a lifetime opportunity to learn design from the best. Guy, Ed, welcome to the podcast.

**Guest 2** (00:02:37)

Thank you for having me.

**Aakash Gupta** (00:02:38)

So there's this debate that I'm seeing with the new wave of designers. One prefers the flexibility of designing with code, using codecs to actually lead the design process and maybe bring Figma in later. The other still prefers the free form of the canvas, the more traditional design process. What is your guys' take on this design in code versus design in the canvas debate?

**Guest 2** (00:03:03)

Yeah, I think it's such an interesting time right now where finally we don't really have to choose. And so the two camps to me are really interesting because I've often found the canvas to be a place where I can just quickly riff on ideas and do a lot of lateral exploration. And I still feel it's the gold standard for that. Whereas code has just enabled me to go super deep and really make my ideas real very quickly. And before I used to have to choose, Which kind of mode do I have to engage in to get to the thing that I want to do? And now I kind of don't. And I think the new kind of shift that we have to embrace, that we should embrace, is navigating seamlessly between both, which is why I'm really excited to be here and talking with Ed about how we enable designers and PMs and teams just to move fluidly between AI coding and agents like Codex, to kind of move between exploration and convergence.

**Guest 2** (00:04:02)

And so,

**Guest** (00:04:02)

yeah. Yeah, it's a good question. And I think it's a little bit of a false dichotomy in a way because as a designer, as a creative, you have a toolkit and there's the right tool for the job. So, you know, if you can code and you want to test out some interactions, hopping into a code base, you know, is maybe the easier option, right? You can just even create a branch off main and you can kind of play with a prod version of what you're jamming around with and you can test stuff out and it can all be live. But, you know, just like there are still architects out there who still work, you know, by pencil, like there's a sliding scale of like how you represent ideas. And I think less than kind of, you know, getting into this kind of like deeper, like philosophical debate around, you know, what is a designer today or what should they use?

**Guest** (00:04:48)

I think I just come at it like really practically. And I think most of the team here do that as well, which is You know, if you're being super exploratory, you want to sketch stuff out. If you want multiplayer, you want to be able to collaborate and comment and show work and print it out and put it up on a wall and, you know, tear it down. But, you know, the role of the designer is pretty expansive. And if we're shipping a product and we want to get the last, you know, mile of the product up to this, you know, the bar that the kind of designer aspires to, then it just opens up the opportunity for, designers to hop in and ship PRs and do that side of stuff so yeah I think I think less of it in some grand philosophical take and more around like what's the right tool for the job and if I was a young designer today I would be like so excited to hop in and like have these insane new kind of like box of toys frankly to just like build all this fun stuff so I also think it's like a really really fun time to be a designer because Your imagination really is the only upper limit.

**Guest** (00:05:46)

And now you have this like really broad range of flexible tools that can help you bring your idea to life.

**Aakash Gupta** (00:05:52)

So I'm hearing from both of you that it's a false dichotomy. Really, it sounds like designers need to be able to use both tools effectively with each other. What are the tactical ways one should think about this? When do you start in code versus start in a freeform canvas? How do you go back and forth? How do I think about when to use it?

**Guest 2** (00:06:11)

It's a really interesting question because it's kind of grounded on this dogmatic approach we've had to the workflow historically because of tool constraints. We've had to start in low fidelity and work our way up into high fidelity because it's expensive to do high fidelity. And so we've created this very standardized way of working that started from that, from paper doodles and low-fi prototypes all the way to code. And now... Like our low fidelity start can just be jumping into codecs and doing a functional wireframe. Like the point is, can I start working from something that gets the team talking and gets us thinking about the shape of the material, the shape of the solution. And then from then I can start bringing that into Figma and working into like, okay, well, My wireframe no longer needs to be a doodle that I made with a marker pen.

**Guest 2** (00:07:00)

Like it can just start being something that's functional and gives me a lot more dimensionality to the problem. And so it really just depends on the level and the scale and the type of problem. working on how to finesse a certain component, maybe you want to start straight in code. If you're trying to figure out how you might lay out a whole flow, it might help you visualize the whole flow in front of you and try to understand where it breaks versus building into a flow. If you're trying to go wide and really try to break a paradigm of interaction, you might want to just do a lot looser fidelity rather than try to wrangle a model to get to what you're trying to do. So it really just now, like I said, you get to pick whatever tool helps you get further with your team.

**Guest 2** (00:07:39)

And I think that's, yeah, it's a really interesting and challenging time for teams that have been reliant on a specific type of workflow that now you kind of get to invent whatever workflow you want because we're making it easy for you to extend that workflow, uh, however you want it.

**Guest** (00:07:57)

Yeah. I think just to add, you know, I think it feels like we're going through this kind of like rapid pace of change where like weekly is a new thing, right? There's some very cool and these things from Figma around this week, which we're going to chat about, but like the underlying design process hasn't changed as well, right? You're solving problems. You're representing things in different ways, right? You're, you know, rallying teams and you're like building a vision of a future and you're kind of bringing people into that future. So it really depends. Um, you know, what your objective is when you're designing might be. Maybe you're, you know, designing a hero image to rally people around it. And you probably want it picked perfect. So maybe you want to, you know, you want to stop in, you know, step into Figma and spec stuff out there.

**Guest** (00:08:34)

Or maybe you're getting really crisp on design systems and you're thinking about how different components interact with each other and how they might look in different states. Again, maybe you want to be in Figma and you want to have all of your tokens. You want to be able to do all the color tests and like really kind of like in the weeds detail kind of you know draftsmanship type stuff um but then say you know you're doing something that's more responsive so you're like testing a product on like how does it look on mobile web or like across different breakpoints or like you want to really test like you know a bunch of different um different kind of like approaches to something or some really interact interesting like interaction design paradigm and there it's like well you kind of want to get into the messiness of code and be able to kind of you know play around with it shape shift things So, yeah, it's funny.

**Guest** (00:09:23)

It's not as simple as kind of like, okay, let's start in say Figma and then we end up in code. It is this often back and forth. And I see this on the team, you know, when we bring people in, they're like, you know, so like, what's the current state of play? for the product and it's like where's the figma and it's like okay well it's really well specified here at this early stage and then there's other but you probably just want to like bring up the product and look there so um yeah it's not as simple as like start in one place end up at another you kind of like you know weave in and out um and it becomes way more fluid which is why i think a lot of these These cool new integrations that we're going to chat about today are really amazing because then the handoff between these tools is a little softer and it becomes like way more fluid and just like easier to work across these different materials.

**Aakash Gupta** (00:10:06)

I think that's where a lot of people's heads are going to go, is can't you have a lot of lossiness as you translate between these tools? How do I do this seamlessly? So instead of talking about it conceptually, can you show us, Ed, how you actually practically day-to-day are bouncing between these tools, what this design workflow actually looks like?

**Guest** (00:10:24)

Yeah, totally. Cool. So I've opened up Codex, which is our desktop app, right? You might have seen there's a terminal product, there's an IDE extension. um but this is our kind of standalone app and the way that it works is you basically just open up um you add a new project so you can open up your local local folder it could be anywhere it could be desktop could be downloads could be like a you know like a repo that you already have open and you can kind of just get jamming so i've opened this thing it's called codex composer system so this is a good example actually about what we're talking about so i've already specced out a composer in in figma but i want to test out some interactions and this is where i think like working in code works really well right so if anyone's used our product we have this kind of dynamic composer system so if the model is asking you for permission to like run a command for example it'll pop up this like permissions kind of special composer treatment like this or if you're in plan mode it might ask you some questions and you can kind of toggle through and go back and it's just like dynamic systems so i built this out in code because i wanted to test these interactions right how the buttons morphed into each other how the size works like you know where the different you know tap targets and things but say i want to like go deep on a particular part of this and i want to maybe go okay i've sketched this out now i just want to get really pixel perfect i want to make sure the icons are my icons i want to change maybe some of the labels right i could then basically bring up codex and i'll use this fun thing that i use a lot which is this pop out window and i can just drag it over the top and i can say um okay i want to import my home page and a few composer states what should we do let's do kind of like composer permissions and plan um into a new figma file um in my, you know, default account.

**Guest** (00:12:28)

And then I'll just type in at and I'll tag in Figma here. You actually don't need to type in Figma. It will just, um, you know, if you, if you say Figma, it will probably just trigger it yourself, but this is another entry point. We also have this like plus menu here and you can install a plugin, um, which you install from the app itself. Uh, and then you get going and you know, because it's getting to know the file system first, it might take a few moments just to get going and to read everything. But maybe as it's doing that, I can just talk through what's going on here, right? So first it's getting to know what's going on. So I just have like a React app and then it's going to Dig into the Figma MCP, which has a few really cool things, which, you know, he's probably a better place to speak to than I am.

**Guest** (00:13:14)

But there's some really cool functionalities that the team has used, which is one is it will go into file and it will basically kind of pop open a window, which should happen any minute now. And this very cool interaction happens and it basically like takes a kind of snapshot of what's going on. And then it will take it and then you just kind of click open in Figma and it will open a Figma file and it will kind of basically copy anything that you want. So you can do interactions, you can do whole websites and then it kind of specs it out in kind of full flow.

**Guest 2** (00:13:47)

The other thing that you can do, especially given your prototype, is you're able to also select specific components. So in that example, for example, you only had the text box and you probably don't need the big white rectangle behind it if you're already working on that. So it also allows you the ability to go down your kind of nodes and select the one you actually want and just iterate on that. So we want to give you as much flexibility as possible to just work with the data that you want.

**Guest** (00:14:13)

Cool. So as I say, it's just popped open and it's pretty cool. It's like, so yeah, to your point, right, you can go in, you can choose to select an element. There's a whole bunch of other fun stuff that you can do here. You can do the entire screen. And then I just click open file. And it will just open up a new file and it will have that composer stay in there. and i think that's the thing that has been very cool for me as a designer okay it's doing a few different screens now

**Aakash Gupta** (00:14:44)

so in the background

**Guest** (00:14:45)

yeah so it's pasted in these files here and as you can see it's pasting the screens that i mentioned and the very cool thing is as you click in everything is like responsive so all of the exact pixel perfect things um right the padding the the border radius it's exactly one-to-one with the file Whereas previously, you know, engineers might have to go in and they have to look at the separate numbers and like, you know, pull out the different, like, oh, what's the, you know, what's the shadow of this? And like, what are these like X, Y values? Like it just does that out of the box, which is I think very cool. And then you as a designer can go in and like, maybe I want to spec this out. Maybe I want to play with color. Right. And I can in here, you know, test out a few different, um, you know, shades of shades of green or like, you know, change some colors.

**Guest** (00:15:29)

Um, And then the very cool thing, so like, you know, this is just a small change, but let's say I end up changing the model and we've recently like reached another model. I can then copy a link to this component, copy the selection, and then I can just paste it in here and say, you know, update my code with the change I made here. And now this will go the opposite way. So if I bring up Codex again and I just run localhost so I can get it running. Okay, sorry, demos. But yeah, you make some local changes and then you can just paste that link back into Codex and then it will make that change in your code. So yeah, this handoff is kind of seamless. So like maybe you're a designer who can code and you can kind of weave between these, but maybe you're not.

**Guest** (00:16:34)

But this doesn't block you, right? Now you and your engineer can kind of collaborate in a more seamless way and it no longer becomes these like siloed areas. It's like way more fluid and the handoff is like much simpler.

<!-- sponsor -->
**Aakash Gupta** (00:16:45)

Here's the dirty secret about prototyping. You spend two weeks building a prototype. You validate your assumptions. Engineering loves the direction. Then what happens? You throw the whole thing away. Bolt changes this completely. When you prototype in Bolt, you're not building throwaway mockup. You're building real front-end code that integrates with your existing design system. So when you hand it to engineering, they don't throw it away. They ship on top of what you've built. I use Bolt every single day. I host my LAN PM job cohort on it. And honestly, I'm up till 2 AM some days just vibing in the tool, having fun, and building. That's when you know a product is good. When you're using it past midnight, not because you need to, but because you want to. Check out Bolt at bolt.new slash akash. That's B-O-L-T dot N-E-W slash A-A-K-A-S-H. Link in the show notes.

<!-- sponsor -->
**Aakash Gupta** (00:17:30)

Today's episode is brought to you by Amplitude. Replays of mobile user engagement are critical to building better products and experiences. But many session replay tools don't capture the full picture. Some tools take screenshots every second, leading to choppy replays and high storage costs from enormous capture sizes. Others use wireframes, but key moments go missing, creating gaps in your understanding. And on the lossiness thing, it's really interesting because

**Guest 2** (00:18:12)

Like it only gets better from here.

**Aakash Gupta** (00:18:14)

It's already

**Guest 2** (00:18:15)

like very good. But as you know, OpenAI releases new models, the better AI gets, the better all of this gets. And so we've just created the pipeline for this to work and it can only get better. And so that to me, is also a really interesting thing because it feels like we're already at such a point where this is so much easier to do than have to, for example, like, you know, in the past I've inherited files from or surfaces from other people. since left the company. And I'm trying to figure out where is the Figma file for this thing? Some of those decisions got made in engineering. They didn't even get recorded in the Figma file. They got all added in to solve some edge cases. And I just want to recreate all that so I can work on top of it. And just being able to capture all of that in the highest fidelity possible is incredible.

**Guest 2** (00:19:04)

And I think now with some of the new releases that we've made with the use Figma tool, we're able to do that in relation to your actual design system. And so when you copy right now, the stuff that Ed copied, because it's just a snapshot, of a website, it doesn't yet bring in your design tokens. With this new tool, you're now able to actually reference your design library and have that pull in those design tokens and local styles. So you're not just working on a facsimile of the thing, you're working on a representation of the thing that is using your style guides. And I think that just unlocks a whole new level of fidelity where you can start having these aligned sources of truth. I saw an engineer actually not that long ago on Twitter showing their process of aligning their storybook to their GitHub to Figma with these AI kind of like running the kind of loop and finding the diffs between them.

**Guest 2** (00:20:01)

Now you don't have this kind of overhead of maintenance of like, oh, but we haven't updated that component in here and it only exists in there. You can just run a loop and have anyone, irrespective of their preferred modality, whether it's their engineers or their designers or their PMs, be able to have the latest materials available to them. And I think this is kind of why we're talking about it. It doesn't really matter whether you want to start in code. It's like, what do you want to do? And the tools will be able to interoperate between them.

**Guest** (00:20:30)

Totally. And, you know, while you were chatting, I made a very dummy change. I just changed the string, changed it to our newest model and ran it. And, you know, here it is in the model picker here. So a dummy example, but yeah, this point of like, you know, you can basically go deep, you know, you can build out the component in, you know, in code and then in parallel, your designers can go deep and then you can just, you know, one click kind of update the master from there.

**Aakash Gupta** (00:20:57)

So practically when you guys are using this day to day, how much do you have to update either the Figma or the code? How often does it get things wrong where things stand just technologically today?

**Guest 2** (00:21:09)

There are limits to the kinds of things that it's able to infer, right? There's going to be a bunch of stuff that just doesn't translate to Figma. Like, you know, maybe you have some shader effects and we're not set up to run that kind of stuff. Maybe you have specific transitions that you're trying to dial in and, you know, a static canvas yet doesn't support for that. But the reality is you can get to a lot through even annotations. Well, a trick that we use a lot is actually being able to read annotations into the MCP. And so we were able to communicate a lot of this stuff back. But it is that point of the designer's job and that labor of love of being able to go in and do things an absolutely leveraged amount of work just from a design industry into code and then be able to also do all these things you used to have to manually spec out and stuff, just be able to do with natural language and say, hey, by the way, I want this to kind of feel like that.

**Guest 2** (00:22:07)

because, you know, it's hard sometimes for a model to infer kind of a lot of intention there. And so it often to us doesn't get a lot of the things wrong. Once you've set it up with your design systems and everything, you tend to be okay. It's going to be on the more kind of web specific kind of effects that, you know, and that's kind of like an opportunity there for us to kind of evolve some of the tooling to be able to like support you there.

**Guest** (00:22:32)

Yeah, I think my mental model is kind of like working with a colleague as well. To your point earlier about, you know, you bring in your colleague on and you have to kind of bring them up to scratch. And if your, you know, maybe Figma files are a bit of a mess or like, you know, things aren't named correctly, then it's a little bit harder for your colleague to get up to speed. That kind of stuff I think is like basically is the same for agents. So, you know, like in terms of kind of like hot, you know, hot tips, I think things like, you know, making sure that you like name your components well and like really thinking through there's a lot of great stuff um from the figma mcp about like aligning your design system with like the css tokens in your um you know in your code base and like once you get those foundations which are good for working with humans or agents then i think it like makes things much simpler but with our most recent model 5.4 as well i have had like a number of designers internally reach out to me and they're like has like is it this model is like way just like way better at like working with these tools.

**Guest** (00:23:33)

And like, obviously there are limitations, but I do think if people haven't tried 5.4, give it a go with the Figma MCP because I think it's like materially better than the things that we've, you know, released before. And I see more and more folks internally now using these tools in like a day-to-day way, which means I think that the reliability has improved and the interoperability and the kind of, you know, new MCP features that like Figma have released are really starting to help.

**Aakash Gupta** (00:24:00)

So you guys have been involved in shipping some pretty important AI features used by tons of people. I'm curious if we can get a behind the scenes of what it looked like when you or someone on your team was working on one of these features, what the back and forth looked like between code in the canvas.

**Guest** (00:24:16)

What's funny, I think, you know, on the Codex team, we're building products for developers. So the designers who work on the team are pretty developer forward already. So, you know, many of us code, you know, I probably spend around, I don't know, 70, 80% of my time coding. So like, you know, the nature of the role has changed. There is less of this kind of handoff process on my team specifically. But, you know, we're also we've been building these zero to one products and we've been moving extremely fast. So it's kind of all hands on deck and hopping in. From speaking with folks across the team working on, you know, other products or like products that have been around for longer or, you know, maybe folks who are like newer to working in code. What I've seen is a kind of like gradual onboarding and a gradual change.

**Guest** (00:25:03)

So, you know, we have some like work in progress, like Slack channels. uh and design reviews and i just see more and more people arriving with like a hybrid of like there'll be a link to a figma but there'll also be like a url link and people will just like hop in and we'll click through and we'll show interactions or you know the other day i was speaking to one of our um you know content designers who typically you know works through all of the like ux copy and and and and like text across our products you know she was telling me that she's been shipping to prod and she's been like submitting prs herself so i think it it it really um varies but i see a lot of people more and more like prototyping early stage using some hybrid of kind of ai tools in figma and then a lot of people at that last mile of like helping bring the polish up and just you know getting in and doing like very small maybe it's a starting to its tweak maybe it's like changing a string Um, but yeah, I mean, if, you know, even if you look at how design has changed on Codex over the past year, I would say it's, it's, it's kind of radically changed.

**Guest** (00:26:06)

And I think particularly with the app, right? We released it, I think, gosh, I don't know, maybe like six to eight weeks ago. Um, but we've been dog fooding it internally. And I think like something changed in December when we were dog feeding the app, the models hit like a certain capability threshold and just felt like anyone could hop in and change. And like the, you know, the, the pace of PRs and development was, you know, was really, was really moving fast. And I think there was, I forget where I read it, but someone had an interesting quote recently, which is, you know, I think the challenge now for design is like choosing when to go slow if you're building. um ai products and like if developers have been accelerated say like 10x which i don't think is an overstatement designers have maybe been accelerated like 1.5 or 2x so you know design can become the bottleneck um if you're kind of not coding yourself So then the trade-off is like, when do you just kind of, you know, meet the speed of engineers and make sure that you, you know, keeping up with the velocity of shipping that's kind of required in this like crazy committed market with when you choose to go slow and actually go through, you know, deep design process, you know, deep in Figma, deep in collaboration and crits to make sure that you get those fundamentals right so that you can have some velocity rather than speed and you kind of can set a direction where you're going.

**Guest 2** (00:27:24)

Yeah, it's such an interesting moment. Even if you look back to even maybe just mid last year, I would have given you a completely different answer. And the Overton window has shifted so quickly from my teams being kind of, you know, AI curious to like banging down the door. They can't move fast enough without it. And it's just this really... kind of interesting kind of challenge because I have teams now that are working directly in staging, right? And they're designers. And, you know, like they have now given you superpowers that are able to do this. And to Ed's point, it's like, okay, well, come back a bit. When are you doing the exploration? You're able to do stuff and you're almost just so empowered by this that you have to think about, okay, this is cool that I can, but then what should I? And I think that's really interesting.

**Guest 2** (00:28:15)

And so for a lot of our work even just like mid last year, we were still working from designs to prototypes. We do prototypes and make. We would then kind of work with engineers to kind of put that into production. Now, you know, we might like... put something, a flag into production. And then we kind of finesse some prototypes and make and just try to get like little details right. And then we will bring that back out to GitHub and then use codecs to kind of work into that. And so it's this kind of constant jumping around between the right tool for the right job. That being said, it's The thing that surprised me the most is how kind of prevalent across Figma this became. When I started, it was very much the, you know, I'm in this area called the build tools area. And so it has a lot of like very technical learning.

**Guest 2** (00:29:11)

leaning folk. Whereas other teams, you know, they work on kind of the editor problems and they work on trying to help you give you better tools, more deterministic tools. And so suddenly now I look around and I have people from monetization, building these incredible, you know, prototypes that are just so incredibly technically accomplished in a way that, like, just as a designer that in the past might never have given themselves permission to do so. And so what we're starting to see is a sprouting of interesting concepts because people now have not just the vocabulary to do it, but the ability to get something in front of people without having to task an engineering team to help them bring that to life. And so... So we see projects starting at all different stages, lots of new zero to one projects, lots of like revisiting old projects that used to be P2s, where we joked about like, there's no more P2s.

**Guest 2** (00:30:07)

Like now everything could just like be shipped, that cutoff line is almost arbitrary because you have polished stuff that you want to do. A designer can now just go and work on that polished stuff. And that's become just really empowering for the team where they have this kind of sense of self-determination that they're able to ship PRs and stuff. And I think as a designer, as a builder, as someone that values agency, there's never been a more exciting time to be a designer.

<!-- sponsor -->
**Aakash Gupta** (00:30:37)

I think both of those points are massively illuminating. On the OpenAI side, people might say, okay, well, OpenAI, especially Codex, they would be operating at the frontier. So Ed's spending 70%, 80% of his time in code. Maybe people would expect that, although I still think it's mind-blowing. And then... Today's podcast is brought to you by Pendo. Welcome to the SaaS plus AI agent era, where every product team, no matter the size, can build world-class experiences. Meet Pendo AI agents, virtual teammates that read your product data, chat with users, and take smart in-app actions so you don't have to. With agent analytics, Pendo shows exactly how those agents drive adoption, complete tasks, and even cut churn. No extra engineering lift, fully SOC2 and HIPAA ready. And because Pendo's behavioral insights sync straight back into your BI stack, you get AI-ready data to fine-tune models and prove ROI in one place.

<!-- sponsor -->
**Aakash Gupta** (00:31:32)

Smaller team, bigger ambitions, you no longer need an army to deliver software your customers love. Grab early access at pendo.com slash akash. That's p-e-n-d-o dot com slash a-a-k-a-s-h. Today's episode is brought to you by Naya One. In tech buying, speed is survival. How fast you can get a product in front of customers decides if you will win. If it takes you nine months to buy one piece of tech, you're dead in the water. Right now, financial services are under pressure to get AI live. But in a regulated industry, the roadblocks are real. NIA1 changes that. Their air-gapped, cloud-agnostic sandbox lets you find, test, and validate new AI tools much faster. From months to weeks. From stuck to shit. If you're ready to accelerate AI adoption, check out Naya One at nayaone.com slash akash. That's N-A-Y-A-O-N-E dot com slash A-A-K-A-S-H. I hope you're enjoying today's episode. Are you interested in

**Guest** (00:32:30)

becoming an AI? AI product manager,

**Aakash Gupta** (00:32:33)

making hundreds of thousands of dollars more, joining OpenAI and Anthropic, then you might want to do a course that I've taken myself, the AIPM certificate ran by OpenAI product leader, McDad Jaffer. If you use my code and my link, you get a special discount on this course. It is a course that I highly recommend. We have done a lot of collaborations together on things like AI product strategy. So check out our newsletter articles if you want to see the quality of the type of thinking you'll get. One of my frequent collaborators, Pavel Hearn, is the Build Labs leader. So you're going to live build an AI product with Pavel's feedback if you take this AIPM certificate. So be sure to check that out. Be sure to use my code and my link in order to get a special discount. And now back into today's episode. You're building upon that, that

**Guest 2** (00:33:18)

even

**Aakash Gupta** (00:33:18)

at Figma, we're seeing the new wave of designer. They are putting things in staging. They might even be shipping polish on their own. That is what the new wave of design looks like. But the funny thing is I talk to designers every day, PMs every day, engineers every day, and a lot of them are maybe at a more traditional company and especially true in compliance or regulatory heavy industries. So I'm thinking specifically about our colleagues over in healthcare and financial services. You know, if you're working at like a university, UnitedHealth or Ginkgo Bioworks where there's huge design teams. You don't, you aren't working in this way yet. You might not even have access to these tools yet. But if you're listening, what is the step-by-step roadmap to get to this new way of working? If you're kind of still stuck in the 2024, 2025 way of working at your guys' companies, how do you come into this new way of working?

**Guest** (00:34:10)

Yeah, I would just say, give it a go. I mean, it's kind of, you know, it's a kind of maybe kind of simplistic statement, but like, you know, I think to some of the examples that Guy was talking about, folks all the time kind of DM me questions about it. And then, you know, I look at kind of what's their role. And it's like, you've got people in GTM, you've got people in finance, you've got people from all backgrounds, technical, non-technical, hopping in and trying these things out. And it's kind of like, once you start using them, you kind of realize, how, um, you know, creative you can be. So, you know, just to give you a few examples, like someone on our GTM team, like just built this whole iOS app that was like on her phone that she showed me at a, you know, at a work event.

**Guest** (00:34:53)

And, you know, as, and she's like, I don't know anything about iOS. And then, you know, just this morning, someone from our comms team, like she wanted to design a seating plan for events. So she like designed the HTML file and you could like drag people around. You could like type in their name. And I think, you know, having chatted to folks across the org, it's, you know, it's like, how did you, how did you learn to do this? And like, oh, I just downloaded it and gave it a go. So, you know, maybe you don't have access um, in the company for whatever reason, but, you know, in the evenings and weekends, you can still download these things yourself. Um, you know, try it in the terminal. If that's a little intimidating, like try, you know, um, try the app or, you know, if you've, if you've ever coded in like, you know, an IDE, like maybe try the extension.

**Guest** (00:35:35)

Um, but just get going. And, and if, and if you're not sure what to do, or, you know, it's, it's a kind of similar problem that we have with chat, which is it's this kind of like blank box and you can do anything. And then, the limitation becomes your imagination. So I would just say kind of like remove that limitation. And if at any point you get stuck, you know, just ask, um, So like, you know, I'm going to Japan next week on my honeymoon and my wife and I are like building this little app. So we're like mapping out our like, you know, the cafes we want to go to and the restaurants. And my wife is like not technical, but she's hopping in and she's making stuff and like, you know, sending prototypes over. So I think just like really kind of like removing these ideas that like it's not for me and just like giving it a go, I think is like the best place you can start.

**Guest 2** (00:36:19)

It's also worth pointing out that, you know, you don't have to start with code. You don't have to start with, like, that has to be your thing. You know, we all have access to, you know, ChatGPT on our phones. You're able to ask any question. I remember when I was trying to learn how to code the hard way before AI and doing all these bootcamp courses and trying out to, like, figure out how to keep up to pace with new frameworks in HTML and CSS and, like, what do I need to learn? And where do I actually invest my precious time into building a skill and a muscle? And now I don't need to. Now I can just ask a question and be like, can you build this? And if it starts to do something, I can ask, how does that work? Help me figure this out.

**Guest 2** (00:37:01)

And so it's really up to me how deep I want to dive into. If I don't care about how it's built and I just want it to work, I can just keep asking it for new stuff. And so there's never been an easier way to get started because it's just like if you can ask a question you can do the thing and i think that to me is really interesting and the question doesn't always have to be about code maybe you're asking about strategy maybe you're asking about how your team dynamics can be improved maybe you're asking about your org chart maybe you can ask anything and that will build confidence to like ask more complex questions And before long, you're asking questions about code. You're asking questions about, hey, I've just inherited this system. Can you help me explain the data architecture of this, just so I understand where we're making calls to?

**Guest 2** (00:37:46)

Are there any systems here that are redundant? look through all my code base. You can ask a bunch of stuff that before you'd have had to ask someone incredibly proficient in this to do, but you can gain at least a surface level understanding of the problem. And it's just through the exposure of that, as Ed was saying, you're going to build facility with this. What happens at places like Figma and I imagine OpenAI is that you're constantly doing this as part of the thing. And so you build that facility very quickly. And I think there's going to be moments where, you know, we're not asking designers and healthcare companies go and start shipping, you know, updates to, you know, to Maine. But at the same time, I think you can start interrogating the systems around you and you can start finding where opportunities for me to contribute or to think differently about something, whether that's in code or not.

**Guest 2** (00:38:32)

I think what's really interesting is that we've tried to do a Figma for a long time is try to make design bigger the design, right? And say, it's not just about designers. It's like the people that we interact with as PMs, as researchers, as writers. And how do we build tools for that? And I think the same is true with AI. And the way these two things are connected is all these people can ask interesting questions that can make interesting artifacts, whether it's Figma, whether it's in codex, whether it's through Figma into codex and codex into Figma. What's important is like you feel comfortable just asking a question. And I think that's a really interesting place to start.

**Guest** (00:39:05)

Oh, I was going to say, yeah, I mean, I think that's a really great point. And one other, you know, maybe kind of thing I would kind of cherry add put on that cake is there's also, I think, a great way of thinking about these tools as well is thinking of them as a tutor or a kind of partner. And, you know, even if you don't know how to code and you start coding it you shouldn't kind of like i don't think the mental model should be i kind of like release control and like i don't need to know how to code and i can just build this thing i think it's like an amazing on-ramp right like you know if you're a designer working in a company you still work across the software development life cycle and there are still a lot of you know really important parts of software engineering hygiene that you're gonna have to go to you're gonna have to go through pr review you're gonna have to understand the code base you don't want to introduce you know foot guns in the code you want to like respect the data model And all of that actually requires knowing how to code.

**Guest** (00:39:57)

So it's a very empowering new technology to give people an on-ramp. But once you start going down this route, you can also just start asking questions. You're like, okay, I've built this React app. What is React? What do these different pages do? What is the difference between a layout page and a normal page? Okay, how does CSS interact? And it's this way of kind of Basically kind of getting over this initial hump, which I think can be a bit scary for folks. Like, you know, I've been to the same, you know, bootcamps probably that Guy has and like, you know, it was a lot of time and investment to go to these things. And frankly, a lot, quite scary for a lot of people, if your kind of background isn't in engineering. But now you can kind of have this on ramp and you can slowly ramp up because I do think like it's really important to understand the underlying systems that you're designing within.

**Guest** (00:40:47)

And none of this basically like obfuscates the need to do that. But it's a really great tool to basically bring more folks into the vault.

**Guest 2** (00:40:54)

I really do think that curiosity is going to be the defining skill of people that succeed in this kind of new era. Because A, it's changing so fast and you just need to have enough of it to ask, okay, what does that mean? for what I'm doing. And if you're already asking that, you're already in a good place. And then to Ed's point, what does that mean, this thing that I've just done? How can I find out a little bit more? And if you have that curiosity, you're adaptable and you're open to new information you're open to trying out new things and i think that's going to be the thing things are changing so drastically that if you think it's a small shift that you can adapt slightly you might miss like the actual bigger picture and so to be asking these questions to be trying these tools to be it's hard to keep up and there's a lot of uh sometimes i feel the anxiety of like oh my god there's too many things launching at the same time and i still have to do my daytime job But there is this kind of mindset.

**Guest 2** (00:41:52)

Let's ask questions and let's see. And now I have this incredibly patient tutor, like I said, that never gets tired, never clocks out. And I can just ping, but I don't get it, but I don't get it. Just explain it to me in simpler terms. And I can get it to work with me at whatever level that I need it to work in terms of abstraction. And so I think... if you can just develop that curiosity instinct, it's probably to your question, like, how do I get started? Just that, just like see yourself as a curious person and start asking questions is what I would say.

**Aakash Gupta** (00:42:23)

I saw this funny meme on Twitter that I'd rather hire a new grad that has been using these tools to their full extent than somebody with a ton of experience who hasn't tried them just because their company hasn't procured them. And I hope that you guys all get that message, which is like, even if you don't personally have your company paying for Figma MCP and Codex yet, If somehow they're not doing that and allowing you to do that yet, it's not a reason to not do it on your own. Ed gave the story of how him and his wife are building an app to go on their honeymoon. You can use personal use cases to explore some of these tools, and when your company finally gets on the bleeding edge, then you will be the first person to be able to take advantage of those tools.

**Aakash Gupta** (00:43:09)

One of the things that's talking to you guys is such a privilege is you guys are basically operating at the frontier. A lot of other companies are going to be operating at the way you guys are operating in a year, in two years. And we've been talking about how designers might be in a staging environment. Designers might even be shipping polish to production or Ed might even be shipping whole things to production. that he creates on his own. Where is the line now? These designer and engineer roles are clearly merging. And then there's always been this third leg of the trio, which

**Guest** (00:43:39)

is a lot of the people watching this podcast, which is

**Aakash Gupta** (00:43:41)

PMs. I would love to know not your guys' prediction of where these roles go, but actually just your description of what it looks like inside OpenAI and Figma today. How are those roles working together? Where are the lines drawn?

**Guest 2** (00:43:52)

I mean, the boundaries between these roles have been blurring for a minute, right? And I think AI has really accelerated that. And so for us, the way that we're thinking about this is that there are people with spikes, right? But there is no, like, kind of territory. There's things that people gravitate naturally to do, and that's now broadened. And so I have designers shipping code, PMs shipping stuff and prototyping stuff and working into design. designs and so one of the things that we found really interesting is with this advent of things like skills and that you're able to kind of guide models to do something you have this almost like pedagogic nature of writing kind of like how do I think about this thing and we have this kind of collective wealth of information that we're like some of it we're using to train our to add to our tools that you know that we've released but some of it we're using internally and so what you end up having is designers writing skills on how to coach AI to design well.

**Guest 2** (00:44:51)

You have PMs working through skills on how to make interesting product decisions and all this kind of stuff, which means that it accelerates that blurring even more. Because now as a designer, I can make use of a PM's mindset to work through some decision making, whereas a PM is trying to figure out how to debug something. And it creates this really interesting thing where I have a natural spike in design, not so much in engineering, but I now have the, I'm standing on the shoulders of giants of a bunch of engineers that have helped me kind of have guide, you know, codecs into a certain way of deploying or something. And so for us, we're now just becoming more, you know, in football, soccer, in Holland in the 70s, there was total football where every position played, every position you didn't have a specific thing. And now we're in this thing.

**Guest 2** (00:45:44)

When someone moves over here, you can cover over here and you have this thing where you don't know how to mark and you're a much kind of, you know, bigger threat as a team. And so for us, we're starting to move into that where teams, have a natural interest and spike in things, but they're able to internavigate and help each other in problems where sometimes someone goes out for a day or they're sick or whatever, and that's now no longer a bottleneck. You can start making progress here and there. It doesn't happen on every team yet, but we're starting to see the signs of this becoming a thing where you... the empowerment that has come from AI has meant that this idea of roles and, you know, rigid org structures is kind of slightly starting to diffuse a little bit.

**Guest** (00:46:28)

Yeah, I would agree with a lot of that. I think that, so, you know, first different roles can kind of, you know, blend a little more easily in terms of just like the day-to-day work that you're doing. But I think one counter perhaps I would provide is, you know, I think the role of a designer doesn't... go away. The role of a product manager doesn't go away. The role of an engineer doesn't go away because you actually play very different roles, right? Like, you know, if you're a product designer, you're, you know, arguably the voice of the user. You're trying to build products that people love and use, you know, same as product managers. If you're an engineer, you're perhaps, you know, more focused on systems and performance and, you know, designers care about these things as well. But you know, even though the different tools that you use are more accessible, or even if now, you know, an engineer can hand something off to Figma more easily, I don't think that, yeah, kind of impacts actually much of the day-to-day work that has happened, that kind of happens in terms of the you know, the different value, the different roles prefer.

**Guest** (00:47:33)

And I would actually kind of look more to the past than the future on this point. So, you know, one way of thinking about it is we look to the future and these roles converge. Another is kind of you look to the past and actually all of these roles have like very different roles within an organization. And, you know, you bring each other together and maybe your toolbox is the same, but, you know, the role of product managers and product is building great products. And, you know, the mandate of an engineer isn't necessarily that. So, you know, it is like great engineers are great, you know, great, great product folks as well. But, you know, I think bringing these different skills to bear at a more kind of like conceptual level, I think like is even more important than the kind of low level of implementation side of things.

**Aakash Gupta** (00:48:13)

So what I'm hearing from both of you is that we have always seen the roles converging, but you do see both of these three roles staying separate kind of conceptually or in spirit representing sort of different elements where the engineer represent more of the quality system and engineering. The design represents the voice of the user and a great user experience. And the product manager, it sounds like, is bringing that business angle to make sure that these are all driving the business goals. Is that roughly the mental framework I should have or how should I be thinking about, well, even if you can do some of the elements of somebody else's job, this is what a person stands for?

**Guest 2** (00:48:51)

Yeah, I'd say yes. I'd say to the point about spiking is that you have things that you naturally gravitate towards doing and that kind of has in a way informed the trajectory you took your career on. But there was moments there perhaps where you are arbitrarily siloed into that perspective because of the amount of time it took to become proficient in a tool. So if I wanted to learn a specific tool, that would kind of gate me in a specific thing unless I had so much time in the facility to also learn let's say code and design and then somehow spend a lot of time thinking about like the intricacies of you know SQL for like querying you know data sets etc and so you you kind of ended up funneling down one thing. And now that the tools are becoming easier and these abstraction layers are being built on it so that you can step into slightly other domains, you're able to do that.

**Guest 2** (00:49:47)

It doesn't mean I'm going to start becoming a designer, becoming a PM or become an engineer, but it means that I no longer am working with only like a third of the picture. And so what it means is I can start like, working into product decisions and into shaping strategy roadmaps and having a higher seat at the table, but also working much more in the implementation thing if I want to. But my role as a designer and how I would self-identify is still, as I'd said, I want to figure out as the voice of the consumer, what is the ergonomics of the thing? What are the ways that I want someone to work through this problem? And then, you know, I will put in enough of my energy into, you know, bringing some of that to life and also creating a narrative and a business narrative around it.

**Guest 2** (00:50:33)

But I have teams to help me do that. But sometimes I'm working on my own zero to one projects, etc. And I'm now able to step into that and write a much more coherent executive briefing, let's say, without having to have gone through the PM, the indoctrination of how do I think about these mental frameworks, mental models, and all that kind of stuff. A lot of that can be surfaced up for me to take advantage of. And I think that's kind of what I mean by People being able to kind of lean a little bit further into another one of the kind of the pillars to ship products. And so, yes, we've been, I don't think people are necessarily jumping ship from one into the other because they like what they like and they're good at what they're good, but they're now able to be better at more things.

**Guest** (00:51:18)

Yeah, I think similar, you know, I, I can only really speak for myself, but like, even though I'm spending most of my time coding, I was still self-identified as a designer and I don't think that has changed. It's just, you know, you're, you're still solving the same problems. You're still trying to, you know, uphold a you know high bar of craft and that just means that you you know work in this different medium and you can kind of collaborate more easily with folks and same with pms that i work with it's like you know a lot of a lot of pms you know still do write prds but there's this great phrase that i've heard a little bit which is like you know prototypes not prds and um you know many of the pms on our team i think are good examples of this and like they'll, you know, bring a working prototype that they're thinking about, or they'll, you know, ship a PR for a feature that they that they were thinking through to like stress test it with some engineers before maybe someone else kind of, you know, takes it on and takes it further.

**Guest** (00:52:12)

So I think it's about like, how can You know, how can code help you in your role, you know, better achieve the types of objectives that you're trying to do? And for product folks, like that's a little bit different often actually than engineers, but the medium that you use kind of, you know, might change.

**Aakash Gupta** (00:52:30)

I could probably ask you guys another hour of questions just on this topic, but we're going to leave it there. This has been a fascinating insight into how I think two of the most important companies shaping the future of product development, how they work in the inside. Gini, Ed, thank you so much.

**Guest 2** (00:52:46)

Thank you. Thank you for having me. All

<!-- sponsor -->
**Aakash Gupta** (00:52:48)

right, everyone. See you later. I hope you enjoyed that episode. If you could take a moment to double check that you have followed on Apple and Spotify podcasts, subscribed on YouTube, left a rating or review on Apple or Spotify and commented on YouTube, all these things will help the Finally, do check out my bundle at bundle.akashi. to get access to nine AI products for an entire year for free. This includes Dovetail, Mobbin, Linear, Reforge Build, Descript, and many other amazing tools that will help you as an AI product manager or builder succeed. I'll see you in the next episode.
