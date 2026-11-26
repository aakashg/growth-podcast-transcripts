---
title: "How to PM Production Changes with Devin: Tutorial From Gumroad CEO, Sahil Lavingia"
subtitle: "How Sahil Runs $10M ARR Company with 1 Employee Using AI."
date: "2025-10-19"
host: "Aakash Gupta"
guests: ["Sahil Lavingia"]
speaker_names: "substack"
substack_url: "https://www.news.aakashg.com/p/sahil-lavingia-podcast"
youtube_url: "https://www.youtube.com/watch?v=I_ue2vrTM9M"
duration: "00:28:05"
word_count: 6354
source: "Substack episode transcript (aired audio)"
sponsors:
  - name: "Vanta"
    url: "http://vanta.com/aakash"
  - name: "Testkube"
    url: "http://testkube.io/"
  - name: "Kameleoon"
    url: "http://www.kameleoon.com/"
  - name: "AI PM Certification"
    url: "https://maven.com/product-faculty/ai-product-management-certification?promoCode=AAKASH550C7"
---

**Sponsors:** This episode is brought to you by [Vanta](http://vanta.com/aakash), [Testkube](http://testkube.io/), [Kameleoon](http://www.kameleoon.com/) and [AI PM Certification](https://maven.com/product-faculty/ai-product-management-certification?promoCode=AAKASH550C7).

# How to PM Production Changes with Devin: Tutorial From Gumroad CEO, Sahil Lavingia

*How Sahil Runs $10M ARR Company with 1 Employee Using AI.*

**Aakash Gupta** (00:00:00)

Sam Altman said one person will be able to create a billion-dollar company.

**Sahil Lavingia** (00:00:04)

Such that one person could ship the entire product. The nice thing about Gumroad is it's basically just me. It's a dictatorship, right? That's kind of why we can move super fast.

**Aakash Gupta** (00:00:12)

Zahil Lavinia has one full-time employee, and he's taken Gumroad to a $10 million ARR and a $100 million valuation. From Slack to Code.

**Sahil Lavingia** (00:00:21)

It'll go and build this. And then you can actually see, based on your PRD, what did the designer think they were supposed to be designing. All of a sudden, this is now a feature in production without us having to really do anything.

**Aakash Gupta** (00:00:30)

That's crazy. Weeks of coordination. You guys just decided, we want to do this. Devon addresses.

**Sahil Lavingia** (00:00:35)

We are leaving CSS behind to migrate every single one of our CSS files and delete

**Aakash Gupta** (00:00:40)

them all.

**Sahil Lavingia** (00:00:40)

You can go straight from Slack to Devon. This is like the first step I tell everyone to do if they're moving to start to use AI more.

**Aakash Gupta** (00:00:47)

Oh, wow. Honestly, I think that's the new dream though. Everybody wants what you have now. And how many dividends have you paid yourself in the last year? Really quickly, I think a crazy stat is that more than 50% of you listening are not subscribed. If you can subscribe on YouTube, follow on Apple or Spotify podcasts, my commitment to you is that we'll continue to make this content better and better. And now on to today's episode. Sahil, welcome to the podcast. Hey, thanks for having me. I was telling you off screen that I have been fanboying about you for a while. I once saw you in person four years ago, but I was too shy to actually come up to you. So this is a dream come true to be recording with you.

**Sahil Lavingia** (00:01:30)

What are we going to do today? We are going to be cooking. We're going to be making three things, walking through how we use AI. I guess small, medium, and large. The first thing will just be kind of how we sort of use it to small like you know, to solve like a really small issue that comes up in Slack, where we have Devin just kind of take care of the issue so that we don't have to get bothered by some small fix, some small feature requests that normally an engineer and designer PM would have to tackle. The second one is going to be like sort of how we walk through building a feature, scoping out the PRD for an existing product of ours called Flexile. And then finally, we'll sort of try to build something totally from scratch, zero one, and see how that goes.

**Sahil Lavingia** (00:02:05)

We don't know what we'll build, I guess. So QB on that

**Aakash Gupta** (00:02:07)

track. Truly live, everybody. Awesome. So can you show us this first one? I was pretty mind blown when you even just told me about this. From Slack to code. Yeah,

**Sahil Lavingia** (00:02:16)

sure. This is an example of how we would use something like Devon to solve a problem. So, you know, we have Slack, like many companies who use Slack. We have an internal customer support tool that we've built called helper, helper.ai. And we had a feature request from somebody basically adding this kind of assign yourself button when something is not assigned. So if you use something like GitHub, it just basically instead of two clicks where you have to like first click on assign and then click your name, it's one click. So you save, you know, your customers one click, which is awesome. And so this was reported by one of our customer support staff and She explained exactly why. This is very great. This is like exactly like the perfect feature request, which is like what you want and why you want it. And so I just said, hey, Devin, solve this, address this.

**Sahil Lavingia** (00:02:57)

And Devin reads the Slack thread, sees the two images, and then sort of explains its planning and keeps you up to date. And then eventually opens a pull request and... Here you can read the code as you should. You should probably test it, make sure it did what you want it to do. Obviously, if you have tests, you should make sure the tests are up to date, all that kind of stuff. So Devon, this is kind of, you know, kind of goes through and creates this. And then I do it and review it. So this is a good example of something that like no one had to really spend too much time thinking about, but it was solved. It was deployed. It was at all the deployment and all that. It's a long bit automated. So all of a sudden, this is now a feature in production for people to use and benefit from without us having to really do anything.

**Sahil Lavingia** (00:03:35)

So yeah, that's one example.

**Aakash Gupta** (00:03:37)

That's crazy. So the original process at a larger company that most people are living through right now, they are going to get that request in Slack. The PM is going to take note of it. They're going to investigate it. They're going to see, oh, how many people is this affecting? Is this a big enough request? Then they're going to prioritize it. Once they prioritize it, there's going to be a request for create a PRD about this. They'll create the PRD about it. Then engineering is going to create their engineering spec about it. Then finally, it'll get prioritized in a sprint and an engineer will actually work on it. Weeks of coordination. You guys just decided we want to do this. Devin, address it.

**Sahil Lavingia** (00:04:11)

Yeah, well, you know, I have a big reason that companies like that are, they do that is because they need buy it from so many people, right? So the nice thing about Gumroad is it's basically just me. It's a dictatorship, right? So that's kind of why we can move super fast. You don't have to kind of like put together all this sort of work that's really just again like internal buy-in it has nothing to do with actually shipping the change the the hard part is like in aligning all the people to kind of get behind that specific decision uh one other reason i really like ai is because i think it sort of is quite good it's sort of like 99th percentile at many things um And so generally, the decisions it makes are pretty good ones. And actually, like things like design and code, we just kind of defer to the AI, right?

**Sahil Lavingia** (00:04:52)

And so it should come up in that sort of PRD. Something that's important should show up in the spec conversation itself. And if it doesn't, that's not that important. And AI can decide, however, to tackle the problem. You know, as long as it meets the criteria in the spec, it's going to, you know, it's correct, quote, quote.

**Aakash Gupta** (00:05:07)

But could bigger companies adopt this for features that are a little bit less contentious, that don't need buy-in? Like, I feel like there's going to be a future world where some companies are taking more of how you guys are working, maybe creating a bar for certain features and that way shipping much, much faster.

**Sahil Lavingia** (00:05:25)

Yeah, I mean, I think the way that a bigger company would probably do it, I don't have a lot of experience working at big companies, so I don't know, to be honest, like the mechanics of them. But basically, you would just do it on a team basis, right? So you would pick a specific project. You know, microservice architecture is quite popular in these big companies for this reason, right? Where you can sort of, people get frustrated that they have to move at the slowest pace of the large organization. And so they think that, oh, if they like factor off and they just have like a small API microservice that they can now all of a sudden move much faster. They can make different technical decisions. They can make different architectural choices. It's true to some degree, but that introduces like a lot of other complexity that you then have to think about.

**Sahil Lavingia** (00:06:01)

And I think my bias is to tend towards like what's the right approach such that one person could ship the entire product like so a lot of the way that big companies move faster makes it impossible to get smaller like their process actually is probably quite fast but requires like a number of people that you can't but you need a pm you need the designer you need the engineer like the way they work you can't without refactoring the process you're not going to be able to get and that's largely why these roles even exist people talk a a lot about automation and unemployment and stuff like that. But most of that unemployment, one, it will happen to these kinds of jobs. It'll be mostly these kind of producer-like jobs. But two, they're going to persist a lot longer than people think because the production process is quite rigid in most of these organizations.

**Sahil Lavingia** (00:06:45)

So you're not going to see companies all of a sudden decide to get rid of like three steps in their process. It's very difficult once you have process to get to unwind it unless you have some sort of like like what happened recently with was it EA, I think, which is when private they were acquired. So in the case of EA, EA is a good example. They probably have built up like a ton of bureaucracy over like the last 30 years that in the next five years is going to get chopped, right? Like the bureaucracy is going to get massively sliced. Better or worse, it's going to lead to a much higher volatility in what EA as a company is going to ship instead of just like FIFA 26, FIFA 27. You know, they're not doing much, right? Like they're really beholden to this bureaucracy, which basically exists because FIFA was such a successful game that they basically haven't had to do anything innovative for 30 years.

**Sahil Lavingia** (00:07:30)

That will now sort of start to happen, which I'm very, I think that's like sort of a, I'm actually more interested in that. Like how does AI, can you revitalize these existing businesses and brands not necessarily new businesses and new brands. I'm actually I was like zero interest, frankly, almost in like new things right now.

<!-- sponsor -->
**Aakash Gupta** (00:07:47)

So we saw the dictatorship workflow, maybe not portable to other companies. I think the second workflow might be portable, especially some of those microservices, those smaller teams who want to pilot it. Today's episode is brought to you by Vanta. As a founder, you're moving fast toward product market fit your next round or your first big enterprise deal. but with ai accelerating how quickly startups build and ship security expectations are higher earlier than ever getting security and compliance right can unlock growth or stall it if you wait too long with deep integrations and automated workflows built for fast moving teams vanta gets you audit ready fast and keeps you secure with continuous monitoring as your models infra and customers evolve Fast-growing startups like Langchain, Ryder, and Cursor trusted Vanta to build a scalable foundation from the start. So go to Vanta.com slash Akash, that's V-A-N-T-A dot com slash A-A-K-A-S-H, to save $1,000 and join over 10,000 ambitious companies already scaling with Vanta.

<!-- sponsor -->
**Aakash Gupta** (00:08:50)

AI is writing code faster than ever, but can your testing keep up? Testkube is the Kubernetes native platform that scales testing at the pace of AI accelerated development. One dashboard, all your tools, full oversight. Run functional and load tests in minutes, not hours, across any framework, any environment. No vendor lock-in, no bottlenecks, just confidence that your AI-driven releases are tested, reliable, and ready to ship. Testkube, scale testing for the AI era. see more at testcube.io akash that's t-e-s-t-k-u-b-e dot i-o slash a-a-k-a-s-h i want to talk a little bit about gumroad because it's just it's got to be one of the most fascinating companies out there tell us a little bit about how you guys are structured you have only one employee but you have contractors how did those contractors get work you pay them what is the structure for getting work done at gumroad

**Sahil Lavingia** (00:09:44)

Yeah, we've been through a lot. You know, we started out as like a sort of traditional venture-backed startup in 2011, up until 2015, when we failed to raise our CVSB. That's when I sort of did our first sort of major pivot as a, the products stayed the same, but as sort of operational pivot. So we downsized, we went to About three or so people got to profitable and sort of ran the business myself for a while, did customer support, product support, you know, fraud risk, customer support, fixing bugs. Not that many new feature shipments, but, you know, basically just try to kind of keep the site up and respond to customers and stuff. Then we started growing a little bit. COVID happened. That was a big boon. Crowdfunding round. So all of a sudden we had some more cash. We started growing the team again. But this time sort of differently.

**Sahil Lavingia** (00:10:24)

Primarily contractors, hourly, part-time, remote. And we have a core team now. That's like full-time. So me and Urshad. And we have maybe three or four people who work like 30 hours a week or so. And then we have the bounties that we do with the open source community now. So all of our code is open source, which means we don't actually need that many engineers on the team because you don't have to be on the team to work on the code. Right. So in theory, you need a lot less, less people. And that's kind of how we work now. So so it's sort of a small team and it's hard. We have an office that could fit 11 people, but it's just tough to, you know, our bar is really high and AI is so cool. And there's so many so much opportunity for everybody out there that's hard to find the right the right people.

**Sahil Lavingia** (00:11:04)

So.

**Aakash Gupta** (00:11:04)

So you aimed, it sounds like at one point, to build a billion dollar VC backed company. What is your current goal for Gumroad?

**Sahil Lavingia** (00:11:12)

I mean, very practically, very boring, but we're trying to get to 10 million in EBITDA. It's just nice to have a goal. Nice to have a short-term goal for the year where the team and everyone can align on what we're trying to do and the changes we're trying to make and the sort of order of magnitude changes we need to make to make that goal happen, which I think we'll get to. It'll be tight, but that's a good goal. I think pushes you at the very end to work a little bit harder. beyond that I haven't thought about it too much like open sourcing everything was a goal but to be honest like we don't have a lot of goals because like if we have if we want to do something we just do it you know like there's not like a long lead time to doing stuff so we just started doing more frequent on sites so you know try to sort of one week a month where we get together in person and build stuff together so you know well I think a lot of my focus over the next couple years will be like now I have a kid I have a five month old so balancing the two and structuring the company and the culture is such that I can be really productive and and I'd still do stuff with a team, but then also like not have it be as intense and as all-consuming as it can be sometimes.

**Sahil Lavingia** (00:12:10)

And so that's kind of like the sort of balance that I'm trying to strike. But yeah, nothing too crazy, to be honest. I feel like for the first time in a long time, which is the nice thing about having a profitable business doing dinner, is I'm not like looking at the future and the, like I get dividends every year. So I'm not, I'm actually, I'm trying to like operate the business, you know, slightly better, like, like almost like as a perfectionist, like, can we just perfect the current business instead of like do other stuff all the time? So we'll see. Flexstyle is fun to work on. It's growing, you know, chip away at that, you know, fix bugs, improve the product. I just want to like work on software, make the software better. have people use it, you know, and just like be proud of the work we do, have some cool people to do it with.

**Sahil Lavingia** (00:12:49)

So I have some structure in my life, you know, stuff like that.

**Aakash Gupta** (00:12:51)

Honestly, I think that's the new dream though. Everybody wants what you have now, like a business working towards 10 million and EBITDA. Where are you guys at so far in the progress towards that?

**Sahil Lavingia** (00:13:01)

Yeah, I think we're at like seven or eight million. So, you know, still work to do. Like, it's not going to be a walk in the park. That's

**Aakash Gupta** (00:13:09)

pretty amazing. I think

**Sahil Lavingia** (00:13:10)

we'll get there sometime next year.

<!-- sponsor -->
**Aakash Gupta** (00:13:12)

Today's episode is brought to you by the experimentation platform Chameleon. 9 out of 10 companies that see themselves as industry leaders and expect to grow this year say experimentation is critical to their business. But most companies still fail at it. Why? Because most experiments require too much developer involvement. Chameleon handles experimentation differently. It enables product and growth teams to create and test prototypes in minutes with prompt-based experimentation. You describe what you want, Chameleon builds a variation of your webpage, lets you target a cohort of users, choose KPIs, and runs the experiment for you. Prompt-based experimentation makes what used to take days of developer time turn into minutes. Try prompt-based experimentation on your own web apps. Visit chameleon.com slash prompt to join the waitlist. That's K-A-M-E-L-E-O-O-N dot com slash prompt. Today's episode is brought to you by the AI PM certification on Maven. Run by Mikdad Jaffer, who is a product leader at OpenAI, this is not your typical course.

<!-- sponsor -->
**Aakash Gupta** (00:14:14)

It's eight weeks of live cohort-based learning with the leader at one of the top companies in tech. As you know by now, the future of PM is AI. And this certificate will give you the learnings, plus the hardware to show you are ready for an AIPM role. I myself took the course and recommend it. Put on by the amazing team at product faculty, including Mo Ali and Pavel Hearn, it's worth it. Former students come from companies like OpenAI, Shopify, Stripe, Google, and Meta. The best part, your company can probably cover the cost. So if you want to get $550 off, use my code AKASH550C7. That's A-A-K-A-S-H 550C7. And head to maven.com slash product-faculty. That's M-A-V-E-N.com slash P-R-O-D-U-C-T dash F-A-C-U-L-T-Y. And how many dividends have you paid yourself in the last year? Last year, I got about $2 million. That's really the life, right? Living, building a profitable software business, having a five month old, controlling your schedule, paying yourself $2 million.

<!-- sponsor -->
**Aakash Gupta** (00:15:20)

I think a lot of people want to aspire to that. When you talk to people, you know, outside of when they're not in the VC backed realm and they're just hiring like crazy, but they are trying to stay bootstrap profitable. They are growing. They're trying to take on AI tools. What are the things getting in their way where I see you very freely just using AI tools? What are the unlocks those founders need to hear?

**Sahil Lavingia** (00:15:39)

yeah i mean maybe their businesses are just doing super well uh and so they don't need to reinvent themselves i think that's a big part of it you know like i think people underestimate like if you're doing fine like there's no reason to like investigate the future so yeah so i i would say that's the biggest one you know just like p zero right like there's only so many priorities you can actually have so you know if it's not your number one priority in the business like you have one more priority like let's say it's hiring someone you're gonna be spending all your time on that so that's kind of just like the way it goes

**Aakash Gupta** (00:16:05)

So you have some other things you're working on, like anti-work. You talked about flex style. I think you guys acquired like small bets. How does it all fit together, the picture for you?

**Sahil Lavingia** (00:16:13)

Yeah. How did it fit together? I don't know. Honestly, I just kind of did like a retrospective on like COVID and everything else like that and just felt like, Just felt like, why not make a bet? And what was like the best fit? It wasn't like, is this the right fit? It's just like, well, let's just make a bet on the best fit. So that's what we did. And now we're in, you know, nice to have a community, you know, nice to have a place that's kind of like our default, like community of small time creators. And so that's kind of like why we did it. And, you know, I was thinking a lot on like, okay, we built this like, you know, like last month, like 35,000 people sold at least one product on Gumroad. So there's like a huge number of people. But Gumroad has kind of plateaued and we sort of have what we want.

**Sahil Lavingia** (00:16:51)

We're incrementally making it better. But I don't think that's like more features isn't really what creators want. Like community advice, stuff like that, I think would be better. And so that's kind of like where we kind of decided to say, oh, maybe there's this like community and we can upsell. And so there's like the base Gumroad SaaS. And then there's like the community that can actually help you like with legal, finance, business, marketing, sales, tax, advice, hiring. That's where I think people, creators sort of tend to need to need help getting to the next level going from like one person to a team for example like even me you know I technically only have one employee or whatever like that's who cares right like what matters is like are you you know doing the things you want to do are you you know do you have a great the reason we don't have one billion dollar single person company is is not that we can't it's just that we don't want to Like Google has $3,000 billion companies in Google alone.

**Sahil Lavingia** (00:17:39)

It's like probably, I can't imagine how many PMs run a billion dollar company by themselves, you know? So it's probably pretty common. Within Fang, there's probably thousands of examples. It's just outside of Fang, if you're doing it on yourself, like I have to do the bookkeeping. I have to do the, you know, like it's just not. not what most people want to do. So it tends to be more of like a marketing gimmick, like, oh, one person, you know. So yeah, that's kind of how I, I mean, maybe that's different. Like we have true AGI where you really don't need any accounting, like all sort of tasks you can sort of have a robot do. But in my mind, if that's possible, then like the robot will automate you too. You'll kind of have a zero employee business. You won't have like a one person business, right?

**Sahil Lavingia** (00:18:16)

You'll just go straight to zero. You'll still own the business, but there will be no people working on it. You know, it'll be kind of like a four contract or something like that.

**Aakash Gupta** (00:18:23)

Yeah, I feel like that's what I discovered too, scaling my business. After a while, it's like, what was the point of being a solopreneur? Just so I could put the label solopreneur, I think I'm going to switch over to entrepreneur and hire somebody to help me with taxes, with sales, with all these different activities that you don't want to do. You don't have to stick to a solo business.

**Sahil Lavingia** (00:18:43)

Yeah, exactly. I think that's a big part of it. Like, I think there's just so much there's sort of like the pro VC anti, you know, like pro VC cult. And that sort of a lot of the indie hacking is kind of like a response to that. But I think it also is a cult in a way, right, where it's just like there's nothing wrong with having a team. There's nothing wrong with like working in person. There's nothing wrong with like being acquired. There's nothing wrong with having a job like there's like we're all basically trying to manage our time and money equation. And like the way that ends up looking for people is going to be different. And it is very dependent on like your personal background. For example, I don't invest in public stocks. Most people would say that you're insane. That's crazy. I just got $2 million in dividends.

**Sahil Lavingia** (00:19:18)

I just hold it in cash, 100% in cash. But the reason I do that is because I have access to deals that no one has access to. The public does not have access to startups. A lot of these things are dependent on that. Why would I invest in Figma as a public company if I could invest in Figma as a private company? so all this stuff matters when you're making decisions for yourself that you know that's just kind of part of thing so yeah i i think you don't want to be extreme like one person you know company is not necessarily the goal um it's sort of a vanity metric right it's kind of cool fun it definitely gets eyeballs so like if there's ever like a a time cover of me it'll be something along those lines just because that's kind of like what people read it click i think having a team is great like the one of the nicest things about having profitable business you can hire people right you oh i really want to work with this person boom i now can talk to this person for an hour every month because i hired them to do this task and i get to talk about talk to them about this specific thing and it's it's like kind of almost like a like a hiring a therapist or something you know to to some to some degree

**Aakash Gupta** (00:20:14)

yeah as soon as you build that one person company that is making like 500k or a million i think everybody will cross that point they'll realize it as well being a solo per business is kind of overrated But I don't think what's overrated is embracing AI in every part of your business and being at the front edge of how to use AI in your business. Like someone I was talking to, he has a huge consultancy. So what he's done is he's created a bunch of AI agents that take the notes, that take the advice he's given his prior mentees. and then simulates for him a draft of what he would want to say after a meeting. So there's all these different workflows, whether you're in a consulting business or a product business like we just demoed all day today, where I think being on the edge of AI is still really useful.

**Aakash Gupta** (00:20:58)

Totally.

**Sahil Lavingia** (00:20:58)

I mean, at the end of the day, it is like the technology of our time. So like I would have learned to drive in 1920s. Now you have to learn to use AI, right? So

**Aakash Gupta** (00:21:06)

if

**Sahil Lavingia** (00:21:06)

you want to be in tech, that's like what being in tech is, definitely.

**Aakash Gupta** (00:21:09)

So you have a legendary Twitter account. That's what made me a fanboy back in 2021, as we were talking about a lot of people. I think I've overturned 60,000 followers at this point on Twitter. So it sounds like that's helped you in a couple of different ways. Right. It's helped you with the deal flow. It sounds like for your angel investing, which is the major thing you're doing with those dividends. It's obviously helped you grow Gumroad and you probably get some creator monetization. Are those the three main areas of benefit or how else do you think about that?

**Sahil Lavingia** (00:21:38)

I think it's really good feedback. So I think most people don't have access to the number of people to give you feedback. So like imagine you have an idea. Your idea is going to be somewhat reasonable. But like if you have 100 people give you feedback on the idea, whether it's a book or a chapter or a web application or a product idea or a startup or a business or philosophy or politics or whatever, I just think my ideas are better because I just get so much more feedback about

**Aakash Gupta** (00:22:01)

them.

**Sahil Lavingia** (00:22:01)

So I think that it's sort of like market feedback in some kind of way. You just have a lot more of that. And so that's a really, really helpful thing. I think it's really helpful if I move to a new city, I sort of have like a built in social network, which is really nice. I generally a lot of really cool, smart, hardworking, successful people. I can sort of like pre-filter them just based on what they say on the Internet, like whether I would like to hang out with them or not. So that's cool. But to be honest, that's about it. Like, I actually think it's like never been less useful. It's actually really. And that's because the algorithms are really good these days, right? You can sort of think about it like the better the algorithms get, the like more useless your audience is because in theory, a really good algorithm means that like a new person with a really good piece of content, but no audience will get significant reach, which can happen.

**Sahil Lavingia** (00:22:43)

So I think now more than ever, like this sort of incumbent advantage is very low for content. for other things it's still high but like for like being like for example if you're a new musician today it's like the best time ever to be a new musician it's never never been a better time music filmmaker are you kidding me like a new filmmaker today the only problem is you have so much competition because so many people also have access to the same tools sort of just like the number of people but But most people, frankly, don't actually compete that seriously. So you're not really like the pool of people like doesn't grow as proportionally to the how much easier it is. Right. So even if it's a thousand times easier to build web applications today than like five years ago or 10 years ago or 20 years ago or whatever.

**Sahil Lavingia** (00:23:23)

You don't see that number of people doing it, right? Like roughly a similar number of engineers today than 10 years ago, even though it's much easier to deploy something to the internet today, like a lot easier. And that's because people just have personal preferences, what they want to do, what they want to work on, how they want to spend their time. So I think a lot about that too. Like how does AI like change things, but also how does AI not change things, right? Like if AI makes it incredibly easy to code, you're not going to see more software engineers. you may you're actually probably going to see a decline in software engineers because the people who wanted to become software engineers already did so like actually the hardness may be something that attracted them to it that like if it's no longer hard they may not be attracted to it uh so yeah fun stuff to think about

**Aakash Gupta** (00:24:03)

I was going to ask after that, and since we're at time, this is pretty much our last question here. Would you recommend people who are trying to create, you know, a really lean AI first team to be investing in building a personal brand and building in public?

**Sahil Lavingia** (00:24:15)

I mean, I think the most important thing is to get to know your customers, right? If your customers are there and that's a way to reach them, fine. If you're doing venture, fine, because your customer is the VC to some degree. So that's important. But I would say most people doing it like they're doing it because they want to. They're not doing it because there's like a business reason to do it. Right. Like I'm not tweeting because there's a business reason. I didn't like come up with my, you know, like some sort of strategy. Right. Like I was just having fun. I was like a young kid in high school and I wanted to talk to other people building stuff. And the only way to do that was Twitter at that time. And I was literally in Singapore. There's like no way to hang out with these people in Singapore.

**Sahil Lavingia** (00:24:49)

So, you know, I created a Twitter account and there's like a hundred people from Singapore on Twitter or something. And, uh, and maybe it's not Twitter today. Maybe it's something else. I mean, the most important thing is you want to get to, you want to build a reputation of someone who is helpful and smart, right? Like, like this person helped me in this way, right? Uh, that's generally, hopefully why I have followers. I don't have followers because I said something witty. Hopefully I said, I assume like people are like, oh, Sahil like wrote this essay and it helped me clarify my thinking in this way. And, and, I'm going to follow him. Maybe he has some other interesting stuff, right? Like, so I think it's sort of like, that's kind of how I think about follower counts generally. It's just like this person helped me. And so that's kind of how I think about it.

**Sahil Lavingia** (00:25:22)

It can be in-person help. It can be offline help. It can be parental help, friends. The goal should be just like to help people. And like if you help people, then you will have an audience. Like you may not have a follower count, right? Like you may not even have, but like more people will show up to your birthday, right? Like more people will show up to your book launch. Like I think people, you know, there's a big difference in like people, not followers and like genuine followers. like fanatics, you know, like, like if I walk down the street at Times Square, no one's going to notice, even though I may have a lot of followers. And then someone with very few followers, but is famous, you know, like will, you know, people will notice, right? Like George Clooney, I don't know if he has a Twitter account, but like he would probably be recognized on the street.

**Sahil Lavingia** (00:26:02)

And so I think, you know, sort of there's like fame. And I think people sort of proxy like followers on Twitter fame or something like that. But there's zero correlation, right? It's it's it's kind of a weird I think of it like you're kind of like on the other side of the Vegas trip. You're like on the productions line. You're not supposed to see, but there's like all the creators are hanging out and all the business owners and all the like grabbing a drink at the bar, all the cab drivers, like that's kind of like Twitter. It's like how many of those people know who you are, right? Like how many, it's sort of this like meta, the meta world. It's sort of like the, it's sort of the deep state almost. Like it's just the people on Twitter are the deep state basically. Yeah.

**Aakash Gupta** (00:26:40)

Or maybe they're all just really shy like me. And when they do see you in person, they just don't go home by the value.

**Sahil Lavingia** (00:26:48)

Yeah, that could be true to some degree. I do notice, like, if I wear a Gumroad shirt, I get recognized a lot more. But my guess is I get recognized somewhat similarly, but people feel comfortable because I'm wearing the Gumroad shirt that it's kind of like, it's okay to say you know me because I'm the one saying I'm okay with this sort of, you know, this identification. So, yeah.

**Aakash Gupta** (00:27:07)

Yeah, totally.

**Sahil Lavingia** (00:27:07)

That's funny.

**Aakash Gupta** (00:27:08)

We could talk for hours. Thank you so much for your time today, Sahil. You're welcome. I really appreciate it. Hopefully it's helpful to people. Alrighty. See y'all later. Bye. So if you want to learn more about how to shift to this way of working, check out our full conversation on Apple or Spotify podcasts. And if you want the actual documents that we showed, the tools and frameworks and public links, be sure to check out my newsletter post with all of the details. Finally, thank you so much for watching. It would really mean a lot if you could make sure you are subscribed on YouTube, following on Apple or Spotify podcasts, and leave us a review on those platforms that really helps grow the podcast and support our work so that we can do bigger and better productions i'll see you in the next one
