---
title: "Stop Using Frameworks: Lessons from Super-Senior IC PM Vineeth Madhusudanan (Microsoft, Meta, Statsig)"
subtitle: "From leading product teams at Microsoft and Facebook to scaling Statsig to $400M, Vineeth shares insights on breaking free from rigid frameworks and building user-focused products"
date: "2024-11-13"
host: "Aakash Gupta"
guests: ["Vineeth Madhusudanan"]
speaker_names: "inferred"
substack_url: "https://www.news.aakashg.com/p/stop-using-frameworks-lessons-from"
youtube_url: "https://www.youtube.com/watch?v=vZDTWn--zrc"
duration: "02:05:16"
word_count: 21668
source: "Substack episode transcript (aired audio)"
---

# Stop Using Frameworks: Lessons from Super-Senior IC PM Vineeth Madhusudanan (Microsoft, Meta, Statsig)

*From leading product teams at Microsoft and Facebook to scaling Statsig to $400M, Vineeth shares insights on breaking free from rigid frameworks and building user-focused products*

**Vineeth Madhusudanan** (00:00:00)

The best products are actually built by people that have a really strong mental model of who their users are, what their problems are, which of those problems are the most material to solve. Vineeth Manasuddin, a product leader at Statsig, brings experience from Facebook and Microsoft, where he helped shape video tech. Now he's making powerful data tools accessible to all product teams. Everything sounds good in theory, but sometimes it's not great in practice. And the quicker you can kind of get your ideas against real data, the faster you'll be able to kind of iterate. I think about it as dropping users into kind of a bit of success. It's not a mountain they have to climb to kind of hit success. Good PMs know how to bend the rules. And I feel like that is more important than being able to find the

**Aakash Gupta** (00:00:50)

perfect template. I'm so excited about today's episode of the Product Growth Podcast. We have a truly senior super IC, Vineet Madhusudan, who's been at Microsoft, he's been at Meta for years, and now he is a super IC at Statsing. Vineet, thank you so much for being here. Oh, glad to be here. So you've worked with so many PMs over the years. What are the things you do differently as a PM? There are probably three things that

**Vineeth Madhusudanan** (00:01:20)

people around me tell me that I do differently. I think one of them is I actually don't care about level-appropriate work. A lot of people kind of worry about, is their work level-appropriate? And it's kind of interesting, not worrying about that gives you a lot of freedom with kind of the solution space. You can be very attached to the problem. And there are times when you would do things like, you know, like literally writing docs for your product, literally sitting with customers and helping them onboard onto the product. And Just being able to do that sometimes kind of expands and gives you a lot more freedom than you have when you think about levels. The other two things are probably, you know, I feel like I've learned over time to kind of approach problems with a lot of curiosity. So even when somebody presents something that looks impossible, my favorite go-to is actually tell me more.

**Vineeth Madhusudanan** (00:02:07)

And that sometimes unlocks things that, you know, if you see something that's impossible, sometimes you kind of turn off your mind around what you could possibly do there. The last one is, I think I like to think of myself as, you know, there's thermostats and there's thermometers. So thermometers react to the temperature around. Thermostats help establish that temperature. And I think part of that being curiosity and being open is also like helping the team regulate for that when things go wrong, You're the person that's actually helping the team calm down and figure out what to do versus kind of reacting with the team and kind of, you know, feeding into that frenzy.

**Aakash Gupta** (00:02:47)

Can you tell us an example of, you know, when somebody came to you with an impossible idea and how you ended up using Tell Me More to build something that worked for customers? Sure. I

**Vineeth Madhusudanan** (00:02:59)

feel like many of our customer conversations in the first year of StatSig were exactly that. We were talking to customers that had more sophisticated needs than what we already had built in the product. And every time we engage with a large customer, like maybe a flip cart in India, for example, they were always asking us for things that were very far away on our roadmap. And for our teams, it was sometimes like, we're like, you know, it was hard to have those conversations because we realized how far out some of those things were. But the cool thing about being curious and trying to understand those problems, you sometimes realize that in the fullness of time, they wanted a solution that solved a bunch of things. But really, there were specific pain points that they had today that wouldn't necessarily be six months or 12 months out.

**Vineeth Madhusudanan** (00:03:52)

The other thing is, you know, I've been at StatSafe for about three and a half years and time passes. So being able to understand those things early on set us on, you know, helped us kind of figure out what we should be doing even a year later, even if it wasn't something we were going to do immediately. But that, you know, now it's three and a half years in and we're much better for those early conversations around tell me more.

**Aakash Gupta** (00:04:18)

Is your product team having trouble in capturing the true voice of customers? That's because user feedback is scattered across channels, making it nearly impossible to catch crucial conversations. It's time you're able to centralize your voice of customer from everything like your CRM, customer portals, call recordings, or even public reviews. That's where Zeta.io comes in, our podcast partner today. With Zeta's AI, you can plug your customer conversations in, and it will allow you to easily slice and dice these into actionable insights for your key product areas so that you can do more to improve NPS scores, analyze features, identify new features, or perhaps understand why you lost a few deals. This paves the way for planning the right features and channeling your efforts into actually planning and building your roadmap to finally close that loop 10 times faster. Product managers around the world use Zeta.io and use it to really improve their product discovery.

**Aakash Gupta** (00:05:21)

It's plug and play in just minutes. So visit zeta.io slash LPS slash Akash Gupta to get an extra 10% off. Got it. And how do you build conviction around the sequencing of features? And how did you do it in Statsyx case? What's an example of something they asked for two to three years ago, but you're shipping now this year?

**Vineeth Madhusudanan** (00:05:44)

Probably. A lot of it is making sure that you're solving problems well. So a great example of this is for people that run a lot of experiments, they often want to do what they call meta-analysis. The basic idea is you run a thousand experiments. You should be learning from each one of those experiments. But really you want to be able to look across the corpus of a thousand experiments and see what are the big learnings you can extract across them. So they might be things like you want to move revenue, but what are early indicators of that, that you could actually measure in a one week period instead of running like a six month long experiment, if you're actually wanting to measure LTV. A lot was that we've heard from our most sophisticated experimenters of one bank. And essentially what we chose very explicitly to do was not try and solve for that because that wasn't what the vast majority of our customers needed.

**Vineeth Madhusudanan** (00:06:39)

There were more pressing things to do. So the approach we took was, you know, if you were an open AI or an Atlassian, we essentially gave them APIs so they could solve these problems themselves and chose to kind of defer building any of these things out in the product. And it's only this summer that we're circling back to it, going back to some of these teams, learning what they built on top of the APIs we gave them and figuring out which of those things are generalizable. which of those things are hard for them to do themselves and kind of now building that into the product. Got it.

**Aakash Gupta** (00:07:13)

Very cool. So let's move into like being a super senior IC. And I think what the thing is, this has become a very trendy role. So what are the misconceptions people have about this? Probably two

**Vineeth Madhusudanan** (00:07:29)

misconceptions that I hear a lot of times. When I was at larger companies, I would often have people come to me and tell me that the number of super senior IC roles is actually very limited. And it sometimes seems like that because, you know, often career ladders and things like that are very sparse at the more senior levels. But the reality is, if you work for a successful business, there's always more problems that need to be solved than there are people able to solve them. So it's almost like if you're a leader in a successful company, there is a vacuum of people that can work on the super hard problems that have big impact. And so it's one of those interesting things where leaders want more super senior people, but when you're at the ground, it feels like there aren't enough roles. But that kind of leads to kind of the second misconception here.

**Vineeth Madhusudanan** (00:08:24)

People ask for, you know, what does the career ladder for a super senior IC look like? What does an IC8 look like? What does an IC9 look like? And the reality is across both companies like Microsoft and Facebook, I don't think they actually exist. Unlike for managers, where there is a rough playbook of, you know, here's what a D1 looks like, here's what a D2 looks like. For super senior ICs, a lot of these career ladders are, you have to make one for yourself. There isn't like a playbook that you can follow. And I've seen different people be very successful at it. You typically, you know, there's some people that essentially help the company move faster. And that is their magic skill. And that is what makes them a super effective IC. There are other people that have like just super deep industry expertise. And that is their playbook to kind of becoming super senior.

**Vineeth Madhusudanan** (00:09:17)

And I feel like part of being a super senior IC is kind of basically making up your own, you know, job definition of what it is. You're not going to find a playbook to kind of check things

**Aakash Gupta** (00:09:28)

off on. Yeah. In a lot of companies where I've gotten to see the pay of people, where I've been senior enough to see that, I think people would be surprised. There are a lot of super senior ICs making more than your directors of marketing, your senior directors of sales, even sometimes your VP of sales, even looking TC wise, because your super senior ICs, what I've noticed is that they'll be at like these big tech companies where they've acquired lots and lots of refreshes. And so these tend to be like, really highly qualified people. And there tend to be quite a few of those also. Like sometimes I think people will be surprised, but a lot of the core products, you know, like your big products at Google, your big products at Microsoft, they're helmed by these super senior ICs. How would you kind of describe the market.

**Aakash Gupta** (00:10:16)

If somebody is thinking, I really like being an IC. In fact, I bet a lot of listeners, they've been a manager for a while of PMs and then they were burned in this last cycle, you know, and they were put back to an IC and now they're like, yeah, I like this. How should they think about like, what is the market of roles of super senior ICs? Is it only at big tech or where, where can they get one of these types of roles? So I definitely don't work

**Vineeth Madhusudanan** (00:10:41)

at Big Tech. When I joined the company I met, that's it. I was employee number 10. We now have about 100 employees. And I still feel like I find very satisfying, fulfilling work here. I think in general, you know, both managers and super senior ICs do two things that are kind of in common. They help grow people around them and they help solve impactful problems. And really the difference is which of those you want to prioritize and which of those you want to spend more time on. Managers spend a lot more time kind of on the growing people and solving problems through them. ICs often have more time to be able to kind of essentially kind of wallow in problems and go really deep on them. But even as a super senior, I see you're not going to be very successful if you can't bring people along.

**Vineeth Madhusudanan** (00:11:32)

Like effectively, you're often, I feel like my job is sometimes like a little bit like a lobbyist where I can tell people what I think they should do, but if they don't believe it and if they don't understand it and agree with it, you know, it's going to be hard for me to actually march people along on things that I'm particularly excited about. And I think for people that aren't comfortable with a little bit of ambiguity around what your role is and are comfortable with, you know, not having a clear answer on what the job looks like, the super senior I see... a great way to actually work on interesting problems. That is what motivates me. And I feel like as an IC, there's a little more freedom to switch across problems than when you're attached to a team that you're supporting. And yeah, so it kind of depends on kind of which of those two things you want to lean more on.

**Aakash Gupta** (00:12:27)

So as we've alluded to, this role has become more and more trendy. You know, at Meta, they like compressed a lot of their M1s. They made them super senior ICs. That's like a very specific way that it's been enacted in the industry. And I think that trend has happened very broadly. I work with a lot of job seekers, job seeking VPs of product, directors of product. They're saying, yeah, companies want to talk to me as a staff PM or as a principal PM. What do you think has kind of driven... this super senior IC trend, I would probably call it the job market PM trend of 2023 and 2024. I think a

**Vineeth Madhusudanan** (00:13:04)

large part of it is you alluded to kind of just the fact that people have reduced or compressed a number of manager roles that are available, and that automatically forces people to kind of think about what are other ways to continue growing, you know, while having impact at scale. The other thing that's probably true is As more of these modern tech companies have gotten even bigger, there are more examples. When I used to work at Facebook, people used to seek me out and talk to me about You know, not even from the teams that I worked at to kind of understand what I did as a senior IC. And part of it was just having role models around kind of helped you see possibilities where earlier the default would have been, oh, I'm going to continue to grow as a manager. And suddenly you see more people doing it and you realize that you have optionality and it's actually a great option.

**Vineeth Madhusudanan** (00:13:59)

There's a different set of trade-offs you make and

**Aakash Gupta** (00:14:02)

it can be a lot of fun. Yeah, 100%. Do you think that it has better work-life balance than the manager track? I don't think

**Vineeth Madhusudanan** (00:14:12)

so. I would probably say there is a little more flexibility in that... You know, I don't have as many one-on-ones with people as some of my peers, but I have a lot of one-on-ones. So, you know, so there is a little more flexibility with choosing maybe which hours of the day you want to engage and work with, but I don't feel like... I have the optionality to like, in some ways I feel like I sometimes have to work harder because as a manager, you have the optionality to kind of sometimes shuffle things around and ask somebody else to lean in.

**Aakash Gupta** (00:14:51)

Whereas

**Vineeth Madhusudanan** (00:14:52)

here I have, I have the optionality to do that, but not maybe as the same, not as easily as when you're a manager.

**Aakash Gupta** (00:15:00)

Yeah. That's some feeling I got too. Um, So my favorite type of role, by the way, to hire when I was a VP and director of product was senior, super senior ICs because as a manager, they take so much off your plate. Usually you can entrust them to actually do pretty good product strategy work, which you can't entrust your average junior PM to do. Usually you can give them very ambiguous problem spaces. So I kind of want to get into those two areas of craft. strategy and ambiguous problem spaces. How have you kind of developed that skill set and grown into these kind of key senior IC skills over time? So

**Vineeth Madhusudanan** (00:15:40)

when I think about marketing, I think about it almost as my team can think about it in kind of three rough phases. The first phase was I was great at finding problems. You know, people around me would describe this is where we want to go. And I, you know, make a list of, oh, here's the 10 things that are going to be hard along that way. And that list of 10 things would become my to-do list. And that's what I would kind of go attack and solve. And somewhere along the way, I realized that, you know, like my job changed quite a bit and my job changed in the sense that it no longer became finding problems. It became finding value. When, you know, like I think Sakya once talked about this notion of he wanted people, you know, like if you have a pile of crap, anyone can smell that.

**Vineeth Madhusudanan** (00:16:29)

And he wanted people to be able to smell the roses even in the pile of crap. And that I felt like became what became valuable kind of somewhere in the middle of my career. Now I think about my role as a little different. A lot of what I do in my company is wallow in problems, spend a lot of time with customers, think about it, and help people around me with, you know, essentially giving them that context and that framing so that they can think about that problem similar to I would even when I'm not in the room. Because there are a lot of product decisions that actually get made where I am part of kind of the conversation, but there's many more product decisions that get made when I'm not in the room. And being able to kind of bring back to the team, whether it's an engineer, whether it's a data scientist, the context that I have and the way I think about a problem and building that together with a team is probably the most useful thing that I

**Aakash Gupta** (00:17:23)

do. Okay. How else has your craftsmanship evolved over time as you've matured as a PM? How have you approached... being a PM differently?

**Vineeth Madhusudanan** (00:17:35)

One was fairly early in my PM career. So I worked in Microsoft IT for many years before I joined the Office 365 team. And I remember one of the first banks that I wrote, it was a large PRD and it was kind of this notion of how do we take on-prem customers and connect them to the cloud Office 365 that we were building out then. And it was both our biggest opportunity, but also a fairly complex thing because we were cannibalizing a very successful business. There were both hard technical problems and hard business problems to solve. And I remember stressing a lot about business. you know, the big review that I was going to have for this document. And I worked like two months or something like that, you know, figuring out details, working with people, aligning stuff. And we finally had the review. And I remember it being a complete non-event.

**Vineeth Madhusudanan** (00:18:30)

We walked through it. People asked some questions. We talked about some trade-offs. And people were like, oh, great. And I was like, oh, wow. And I remember that distinctly, even though this was so long ago, because that is when I kind of realized, like, Like, you know, the whole thing that a PM does, like people sometimes think about it as creating a great PRD that the team executes on. But it's actually the process of kind of figuring out all those, you know, what problems to solve, how to solve them that are really the key part of what you do. And the actual document that you do is, like I said, almost like a non-event if you've done, you know, the core parts of kind of what you do as a PM really well.

**Aakash Gupta** (00:19:10)

Got it. And typically I would say like people lean on, you know, really, really good customer discovery skills, good data analysis skills, and general product sense is kind of like the three drivers of, I guess what we're talking about is like what PMs really do. Would you say those are the right three buckets of how you are getting even better at that? Or is there anything I'm missing? And if they are the right three buckets along those three, like how have you gotten better at those? One of the things that I work

**Vineeth Madhusudanan** (00:19:40)

with, I work with experimentation. I talk to a bunch of customers about how to use experimentation. And one of the challenges that people run into is like people think about notes. I run an experiment and I figure out what I'm going to ship. And I have very strong conviction that that's actually the wrong model. Like it's sort of like saying I run UXR and I figure out what to ship. Like the best products are actually built by people that have a really strong mental model of who their users are, what their problems are, which of those problems are the most material to solve. And that mental model is what you use to kind of build great products. And pretty much anything you do around user research or experimentation, I think also is just a way to kind of tune or improve the mental model that you have to build great product.

**Vineeth Madhusudanan** (00:20:33)

And how that happens is I spend, I want to say, quarter of my time doing something daily customer related, whether it is helping sell, whether it is helping customers kind of advance what they are trying to do. And a large part of that comes back into kind of refining my intuition about what is important for them. And that is a large part of how we've actually built successful products, you know, whether it's a big company or here at a small startup.

**Aakash Gupta** (00:21:14)

Okay, very cool. So we talked a little bit about that long PRD you spent two months on. What is your take now in 2024? How should PMs be writing PRDs and what does a good one look like versus a bad one? Very dramatically, depending on the kind of environment

**Vineeth Madhusudanan** (00:21:29)

that you're working on. I work at a small scrappy store and some of our best PRDs have actually been scribbles on a whiteboard. I, you know... Filling out a former document is sometimes useful because it helps you think about, oh, what are the things that you should have considered? At a small startup, it's often very easy to actually align people on pretty much everything you need to on a PRD literally around a whiteboard. The moment you move to a slightly larger company, it's incredible how many more people need to be brought along on that journey. And that is where, you know, having a more formal PRD becomes much more useful. I find this, you know, even here when I'm working with customers, like the most form of documentation that I create is when I'm actually working with a customer that is a really large bank or something like that.

**Vineeth Madhusudanan** (00:22:27)

And we're trying to align around the problem because, you know, it's not it's not five people huddled around. a whiteboard that you're trying to align. Sometimes it's dozens of people, some of whom are not going to have a direct conversation with you that you're trying to bring along for that journey. And that the needs around a PRD when you're doing something like that are slightly different. But it's really making sure that you've thought about the right problems, you've picked the right problems, and you've brought people along on that journey with you so

**Aakash Gupta** (00:22:59)

that they're aligned with you. So I think a lot of people listening may have never done this whiteboard PRD. I've basically only did them at one company, Epic Games. So can you walk us through what is the whiteboard PRD? What does it look like? How does it even come about that you guys are all at the whiteboard? What is put on there that is sufficient detail for then design and engineering to build? It is not appropriate for all teams, but

**Vineeth Madhusudanan** (00:23:23)

like when you have teams that actually have the same level of context as you do, You don't have to flesh out a level of detail that you would normally in a document. Usually, when we're building out... We were earlier talking about meta-analysis and this notion of being able to kind of answer questions across thousands of experiments that you've run. And when the very first version of something that we did around this... We literally huddled around, we had a bunch of customer conversations around trying to understand, you know, what they were trying to do, how they were hacking it together, what they did offline and things like that. But I still remember like coming together with a couple of data people, a couple of engineers and a designer in a room and essentially articulating you know, starting with kind of what questions did customers want to be able to answer?

**Vineeth Madhusudanan** (00:24:20)

And kind of, we literally whiteboarded a bunch of them and kind of picked five key questions that people want to be able to answer that we thought we should try and answer first. That was one part of it. The second part of it was, you know, just whiteboarding, how we might actually try and answer that. And literally on a whiteboard, we were creating some UX sketches for what it might look like, what you would look at, and what you would be able to answer from that. And in many ways, that was probably all we did for the PRD, for the first set of features that we bent around that. The couple of things that kind of allowed us to do that was the engineers had the engineers in the room also had context around what people do with experiments why these metrics matter why these questions matter like literally the fourth question that we picked was you know this team has done 100 experiments how many of these impacted a top line business metric versus just a team specific metric and super easy simple to understand problem that Like everyone in the room had context around why it mattered, how it mattered, what the underlying data sets were.

**Vineeth Madhusudanan** (00:25:38)

And a lot of the fleshing out that might happen around, you know, edge cases, use cases, how to filter, how to remove outliers and stuff like that happened after we had designed and built a very scrappy V1 and could actually look at real world data. Because sometimes you spend, you know, like anticipating what kind of problems will happen with something like this before you actually look at it with real data. And, you know, and that's part of the experimentation. Like, you know, everything sounds good in theory, but sometimes it's not great in practice. And the quicker you can kind of get your ideas against real data,

**Aakash Gupta** (00:26:20)

the faster you'll be able to kind of iterate. Yeah. So is that one of your core philosophies and product is like, try to get quickly to real data? Oh yeah. So

**Vineeth Madhusudanan** (00:26:31)

we, like one of the static values is notion of being very scrappy. And in the early days, one of the things that worked well for us with our speed was we sometimes work with really large customers. They would ask us for features that did not exist. on the platform, we would understand it. And by the time they actually had, you know, they got around to scheduling the next meeting because that sometimes took time in a large company, we would have actually built a version of this feature. And it was incredible because We could look at something real. We could look at something that, you know, they could test against real data on their side. And the amount of things that we'd make scrappy like that and have grown into bigger things is pretty amazing.

**Aakash Gupta** (00:27:22)

Yeah, it's like kind of an old concept, like build an MVP, get it out there, get data. But still to this day, very few product teams are actually living that. What do you think is kind of like... Resulting in this culture where people spend so much time de-risking, spend so much time on this large PRD, spend so much time on then large prototype testing, maybe a large alpha group before they're even willing to consider getting it out there to get a real experimental data.

**Vineeth Madhusudanan** (00:27:52)

Some of it. I think, comes from scale. So if you Google at Gemini and make some product calls wrong, the backlash you get is very different than if you're a small, scrappy startup and you do something and it isn't the great. The level of scrutiny that the big tech companies invite is very different. That is a reasonable... concern and I understand why that changes how people do things. The other thing is just the access to being able to move fast. So one of the things that I like about where I work right now, most of our revenue comes from large enterprise customers that we work with, but we actually have a free tier and a pro tier that has You know, sometimes like indie developers that are using us for some side project that they have. And one of the things that I find value with is when I build new interesting features, if it can be used by an indie developer, I almost prefer kind of working with them on these initial versions.

**Vineeth Madhusudanan** (00:29:02)

Because if a large company asks me for a feature and I build it, you know, by the time I actually tell them about it, you know, they think about using it in some quarterly planning cycle or something like that. And the distance between, you know, when I build something and they give me feedback on it can sometimes be a month, which, you know, like in that time, I'd lost context around what I was thinking about doing, what ideas I had. Whereas if I have access to kind of these immediate feedback cycles, which you get when you have, you know, like indie developers that move fast, if you have access to these fast feedback cycles, it is incredible how quickly you can kind of get early signal on whether you're solving the right problems, whether you've thought about it to the right way. Sometimes you, you know, you just realize you put the wrong thing and you're willing to kind of scrap it and start afresh.

**Vineeth Madhusudanan** (00:29:52)

That is very powerful.

**Aakash Gupta** (00:29:56)

Okay. So we talked a little bit about PRDs and we got into, you know, the essence of how to really do them. I think the other thing that PMs spend all their time on, which you just alluded to, is like these quarterly planning, annual planning processes. I'm curious, like how you approach planning and maybe like the lessons you've learned over time, just do a better job in these planning cycles. My general

**Vineeth Madhusudanan** (00:30:19)

sense with planning is, you know, remembering that planning is just a tool. Really what you're trying to do is you think you're trying to, you know, you're playing to win at something and planning is in service of that. So if you keep that perspective, like my approach to planning is I like to start super early. I, you know, like we've gotten to the point where now we think about quarterly plans, but often two months before, like it's kind of funny, two months before my quarterly plan starts, I've already got a notepad that I'm jotting down ideas and wallowing in things to explore or conversations to have and things like that. And by the time other PMs are, you know, starting planning, what I often have is I think of it as a Shittycloth draft or what I think the plan is, because there's nothing that invites discussion and critique as much as somebody seeing something on a board and saying, oh, that is not right or that is wrong or you've missed something.

**Vineeth Madhusudanan** (00:31:25)

And I love planning cycles where you kind of have really early drafts that are very, like essentially you're building your plan in public so that whether it's your customers, whether it's internal stakeholders can actually critique you. So that by the time you get to a plan, you're comfortable. But the other thing is planning never really ends. Like I think about the best plans at both places that I've worked as kind of essentially a series of ideas. And when you're going down executing, what you're trying to do is you're trying to validate, I had this idea. Is there actually value shared? How can I prove or disprove it? And which kind of then guides you down this path of things that you keep investing in and things that sounded like a good idea, but like in the real world aren't naturally going to work out.

**Aakash Gupta** (00:32:17)

Okay. So it's always going on. And I think a word you used a couple times is wallowing. What is the process of wallowing for you look like? Wallowing for me

**Vineeth Madhusudanan** (00:32:29)

is really just... noodling or thinking about a problem for a while. Like often I will have a germ of a problem that I know I need to solve, but not necessarily the right framework for how to think about it. But if I've identified that, you know, like it will kind of like, I don't necessarily have to actively think about it, but when I'm having conversations with people, I will sometimes, you know, associate that with this problem that I have in the back of my head. I'll be showering and I'll think about like an idea or a next step that I can kind of, oh, I should talk to this person about it. And it's not so much a conscious, it's not, you know, there are some, there's obviously times when I start at my desk and I'm like, oh, okay, what should I do about it?

**Vineeth Madhusudanan** (00:33:20)

But just telling myself, oh, here's a problem. And I'm not happy with current state of how I'm able to kind of think about it. Oh, I, allows me to sometimes over a period of time kind of, you know, find three things that I can do to improve it or find, you know, like the germ of an idea that I probably wouldn't have had if I just sat on my desk and thought about, okay, how am I going to go follow this now?

**Aakash Gupta** (00:33:43)

Okay. So you think about the shower, you come out of the shower, you realize like, okay, I need to go talk to some of my enterprise customers about this problem. I want to go talk to my SMBs about this aspect of the product. What is your productivity system look like to organize all the things you need to be doing? Because these discovery tasks, you know, often execution just seems to get in the way. Like when I developed my Eisenhower matrix, that was my productivity system. They would never come in the urgent side. And so they would just never get done. How do you make sure that these things get done? I wish I had

**Vineeth Madhusudanan** (00:34:18)

a magic answer. Actually, I feel like I actually have a magic answer. I struggle with doing it consistently. What? Usually... What I try and do is at my desk, I have a little post-it doc. Usually it is like the top three or four things that I want to do for the next, you know, not short term. So usually it's a few months or something like that. And what I find super helpful, like the weeks that I'm the most productive are the weeks when I get in on a Monday morning, look at that list of three or four key things that I want to be doing. assess where I feel like, like how I am doing against those and figure out what are the next two or three things that I need to do on each of them. And, you know, from some weeks, it may be nothing on something, but like on other weeks, there might be a bunch of things on one of those things and kind of make a plan for the week.

**Vineeth Madhusudanan** (00:35:17)

One of the things I struggle with as a PM is my day is often a constant series of either meetings or interruptions. And having, you know, 20 or 30 minutes at the start of the day to be able to kind of figure out what it is that I want to do or move forward or put energy behind allows me to make sure that I make the space for that versus letting, showing up for my first meeting and that's when I start work and then kind of my day just at 6 p.m. or 7 p.m. and I'm like, wow, where

**Aakash Gupta** (00:35:52)

did the time

**Vineeth Madhusudanan** (00:35:52)

go? What did I do?

**Aakash Gupta** (00:35:54)

Yeah, I share that with you too. That's like the worst start to my days is when you just are rushing in like a minute late for the meeting and then you're like, okay, now my day is just going to be like this. Whatever meetings and Slack messages I'm getting, I'm just tackling.

**Vineeth Madhusudanan** (00:36:09)

Yeah, but it's amazing how much like 20 or 30 minutes of focus time without interruption helps you figure out where to put energy and how that changes how wildly different a week can feel.

**Aakash Gupta** (00:36:23)

Yeah, it's about getting like more time for those high leverage tasks versus like those neutral or overhead tasks to use like Trace's LNO framework. What do you feel like typically falls within that leveraged high leverage? What are like the things that you're doing, the two to three things per week to move forward, the three to four things you need to do over the next couple of months? Like are those tasks often talking to customers, digging into data? What are those tasks often look like?

**Vineeth Madhusudanan** (00:36:48)

Talk to customers are typically not in the... Like, talking to customers is something I end up doing, but it ends up being in service of something. So an example of that is we have... So we have an analytics product and we have a cloud version of that product. And one of the things that I'm trying to do is kind of advance, we have a warehouse native version of that same product, which is essentially the customer never sends us their data. We just like keep the data in place and we need to reason over it and offer them the same kind of insights that a PMIQ is to like Amplitude or something like that for. And so right now, one of the things on my list is definitely advancing kind of our warehouse native capability. And The specifics of what I do on a weekly basis might vary.

**Vineeth Madhusudanan** (00:37:40)

Often, like some weeks, it might be kind of understanding a class of problems that people use other tools for. Some weeks, it might be, you know, understanding what kinds of things current customers are cobbling together on their own that we don't support well. That, you know, like often a great signal, it do things to build it. where people are kind of doing something very clunky with your tool that, you know, they realized has value because they're willing to kind of jump through hoops and, you know, fit a square peg in a round hole despite you not having solved that problem. Some weeks, we're focused, making sure that, you know, we've figured out what the next thing to build is or how we're building it. for the daily dramatically, but usually it tends to be a theme around like advancing some product area or in some, some months it is addressing a new market or an opportunity or thinking about, you know, a different kind of competitor.

**Vineeth Madhusudanan** (00:38:46)

Because one of these things, like we're young enough that all of these things change dramatically.

**Aakash Gupta** (00:38:53)

Yeah, especially in the product analytics space. They're changing all the time. Okay. So one of the things that's clear is that you have like a, what I would say, like a very high executive presence communication style. How have you developed your communication style over time? And do you think about storytelling as an aspect of that? A little bit.

**Vineeth Madhusudanan** (00:39:14)

Like as a PM storytelling is easy. Super important because ultimately, like often I feel like people forget the details and they remember how they, how you made them feel. And as a PM, that is probably one of the most effective tools you can have. So we've been around for a while now, and we've bid out much more in the last three and a half years than we had in maybe the first six months. And now when I look back, you know, there were customers like Headspace or Notion that were willing to bet on us pretty much three years back. And a large part of that was... You know, like us being able to paint a story of what their organization would look like when we had solved problems that they had or used tools that we were bending. And a large part of that, yeah, was just pretty much storytelling.

**Vineeth Madhusudanan** (00:40:08)

And it's amazing how true that is externally, but also internally with being able to kind of move and motivate a team towards purpose.

**Aakash Gupta** (00:40:20)

Got it. And one of the hot areas I feel like recently, especially with, you know, like the rise of Figma and PMs not being given edit access on Figma and stuff like that is like this PM designer relationship. How have you kind of approached that relationship and how has that evolved over time?

**Vineeth Madhusudanan** (00:40:44)

It comes a little easier to me than for some. I am not very good at UX and UI design. And it's kind of funny because I'm the first person to kind of admit it. It isn't necessarily a strength of mine. But it works really well because my strength tends to be understanding things. the problem, the customer problem that they try to solve. And it allows me to actually have a really great relationship with people that work in design because I'm able to help the team articulate and understand kind of what the core problem to be solved is. And I almost lean a little more than I sometimes feel some of my dear PMs do on them for help with the design and designing kind of the visual architecture and figuring out how we're actually going to solve the specific problem at hand. But my understanding of the problem, you know, allows me to help kind of test the solution that we're looking at in a way that if I was part of the design, maybe I would not, if I was a little more closer to the design, I probably would not be able to kind of detach myself and sense.

**Vineeth Madhusudanan** (00:42:01)

And I feel like I really enjoyed that partnership that I have with the divine team

**Aakash Gupta** (00:42:06)

that I work with. Got it. Really triple clicking on the problem as kind of the lens for your evaluation. So that's our super deep dive on super senior IC. I want to talk about who should be a super senior IC. So first of all, why did you choose the path of senior IC versus management?

**Vineeth Madhusudanan** (00:42:27)

I kind of stumbled into it by accident. When I started at Microsoft, I became a manager maybe like a year and a half or two years into starting to work. And before I knew it, I was, you know, seven or eight years in, I had a team of, I think at that point of time, about 25 or something like that. And it wasn't something I'd done consciously. And I remember waking up one day and realizing, wow, my job has changed quite a bit because, you know, initially you start with a small team and you're still effectively an IC and you're just kind of coaching and bringing some people along with you. And as you switch to becoming a manager of managers, eventually I realized that my job was fundamentally a very different job than what it was or what I thought it was a little while back.

**Vineeth Madhusudanan** (00:43:20)

And what I chose to do then, I switched back to being an IC and my plan was to do that. for a year. And that was kind of my plan. Now that is, I feel like 15 years back or something like that. And I haven't looked back. And pretty much every job that I'd been at, I've had a manager or a few managers work with me and try and convince me that, you know, here's how you could help the organization by switching to being a manager. Here's the opportunities for you and so on. And What I've realized is I really love the freedom that kind of comes with being an IC and being able to kind of both choose with some constraints, like what problems I want to work with, the teams that I want to engage with, how much energy to give which people. And I can't imagine having it any other way.

**Aakash Gupta** (00:44:21)

Got it. So you've seen both sides of the coin. For somebody who is trying to figure out which side they should pursue if they haven't seen both sides, what would be kind of your advice? Who's a good fit for senior IC versus management track?

**Vineeth Madhusudanan** (00:44:38)

My general advice to people that are thinking about this is you should absolutely try both. I have my wife is a PM and like she has switched between being an IC and a manager multiple times and over time has decided that she really enjoys kind of the she gets joy working with people and helping them grow, then in addition to kind of being able to solve problems. And it's really kind of just that balance between growing people and solving problems. So as a manager, I feel like you get to do a little more of the growing people. As an IC, you get to do a little more of the solving problems. In either case, as a senior person, you should be doing a bit of both. But Yeah, for people that haven't done both, I think there's nothing like trying your hand at being a manager.

**Vineeth Madhusudanan** (00:45:25)

Most people start out with allergies, but definitely try your hand at being a manager before you decide that. And the other thing is, like my wife, you don't have to be attached to one of those. It's actually often possible to be reasonably steward across those. As long as you keep... You know, as long as you keep your ability to kind of dive into details, you maintain your product sense, which most good leaders often will. Oh, yeah. It should be fairly easy to sit

**Aakash Gupta** (00:45:55)

between the two, but once you've tried them, you can divide. I think some people might be nervous about that switching. How does it actually look? Maybe you can give this specific example on Microsoft. You're managing a team of 25. How does one go back to being an IC? How do you handle that conversation with your manager, HR, et cetera?

**Vineeth Madhusudanan** (00:46:14)

It feels like forever ago. I think the biggest thing with switching from being a manager to an IC is, you know, being able to kind of I wasn't very senior when I made that switch. I was probably like the fish level person. And I think the biggest challenge that people struggle with when I've seen people try to make that change is being able to articulate what you will do as a senior IC. Because sometimes that isn't always clear. But so you have to kind of walk in with the confidence that you're going to be able to do it. Because in more... Like most people that make that transition, they've often struggled a little bit with clearly articulating what value would look like when they're on the other side. But when they do it well, it's one of those, you know, when you like, I, you know, people will be like, oh, I have no idea what an IC8 does.

**Vineeth Madhusudanan** (00:47:14)

But when you see somebody doing it, you're like, oh, I get why they're a senior person and Yeah, so you have to kind of be willing to kind of make that leap of faith and be confident that you will find enough things of value. At the place that I am at, kind of changed roles. roughly about once a year in a very material way and when i switch from one role to the other role i often don't have a lot of clarity on what that new role is going to look like but part of going in and doing that is figuring it out and yeah just be comfortable that is probably the most beautiful bit.

**Aakash Gupta** (00:47:59)

All right. So before we close out our section on superceder ICs, what is your best advice for like an aspiring superceder IC?

**Vineeth Madhusudanan** (00:48:08)

This is going to sound simple, but it's really like Find a way to be useful? It sounds trite, but I talked about this earlier. Most teams have more problems than they have people stepping up to provide solutions or solve things. And just... Having a lens that allows you to see what are these unsolved problems that leaders either know about and care about or should know about and care about is probably the most impactful thing you can do when you think about pursuing a CIC role. If you're not comfortable with finding these problems to solve, you know, are different parts probably more comfortable? Yeah, that is probably the lens that I would, you know, for deaf people approach this through.

**Aakash Gupta** (00:49:12)

All right. So now I want to move into a topic that I think you're pretty well known in the product world about, which is world-class experimentation. You wrote a really popular Medium article, Five Features to 10x, Your Experiment Velocity. Can you walk us through it? The article has specific

**Vineeth Madhusudanan** (00:49:28)

features, but I actually want to take a quick step back and talk about a different transition and a different era. So like 100, 150 years back, A lot of the factories here in the U.S. actually used team as their power supply. And, you know, it was horribly inefficient. Things broke down all the time. It was hard to do stuff. And there was, you know, very, you know, there was a few companies that found this really cool innovative thing that they called electricity. And it was amazing how much more productive they could be. And it was a few companies that actually didn't. And back in the day when they did this, there was the grid you could connect into. You essentially had to build the captive power plant. And you literally had a vice president of electricity. But it was really cool. And if you did this, you were like leaps and bounds ahead of your competition.

**Vineeth Madhusudanan** (00:50:21)

And that's, you know, like it's kind of funny to think about factories with a VP of electricity. But that changed over time because as more factories realized what kind of advantage they had with that, they also hired VPs of electricity. And they quickly got to the point where, you know, everyone was doing it. And suddenly what was once a competitive advantage was not. And then this other thing happened, which was people invented the grid. And there was a time when the grid was, you know, maybe not as stable and reliable as your in-house power plant. But over time, that changed. You eventually got to the point where, you know, today, if you're setting up a factory, you never think about having a VP of electricity. You just plug it to the grid. And unless you're doing something very, very bespoke, if you're an aluminum smelter, then yes, you have your own capital power generation plant.

**Vineeth Madhusudanan** (00:51:13)

I guess if you're Microsoft and you have a large AI data center, you think about bringing back the three-mile island. But pretty much in all other cases, you kind of connect to the grid. And I feel like, you know, I tell the story because I've seen a similar transition happen with Microsoft and kind of Office 365 where, you know, everything was on-prem and there was a time when connecting to the cloud was like, oh, scary and risky. And now it's funny if somebody tells you that, you know, I want to set up my own email server, which was a thing. You know, that article was basically taking that same idea with experimentation, because I feel like we're in that same transition with experimentation. 15 years back, if you were building a product company, you didn't have experimentation tools that actually helped you measure the things that you cared about.

**Vineeth Madhusudanan** (00:51:59)

And if you were a Microsoft or a Google or an Amazon or a Uber, you had to build it in-house. Now, it is much more accepted that part of product building is being able to measure, being able to experiment. But incredibly, there's a lot of people that actually have roles where they're building the equivalent of captive electricity generation plant. by building their own experimentation tooling. And a lot of what I wrote about in that article was kind of what are the things that big tech companies are able to do with their experimentation tooling that you should be able to access to And why using a product, whether it's, you know, Static is clearly one of them, but like using a modern experimentation product is basically like connecting to the grid. You have instant access to, you know, best in cloth functionality versus spending, you know, Microsoft took three years to build out the tooling that they had.

**Vineeth Madhusudanan** (00:53:03)

And that's not dissimilar for many other companies that did the same thing. Got it. So what were the five features? The five features were, the first one was basically making it such that if you want to measure a feature, the marginal cost of doing that for your engineer is close to zero. So there's a set of features around basically making sure that even if you're shipping a bug fix, you can measure that as an experiment without actually doing any other work. The second one was the notion of being able to use holdouts. So holdouts are a really cool feature that actually allow you to quantify if you've shipped a bunch of goodness over six months, being able to actually measure the cumulative impact of that goodness related to kind of, you know, other things that might have changed your trajectory. So market conditions, the economy, other, you know, competition and so on.

**Vineeth Madhusudanan** (00:54:03)

The other one was being able to experiment on business metrics. Many of the A-B testing vendors that have kind of played in the face for a while, the legacy players, focus on measuring clickstream metrics and very shallow, like did the user proceed a funnel, when really most modern companies want to be able to measure outcome metrics. So you signed up a bunch of people for a trial, great. You draw trial conversions up, great. Really what you're looking for, how many engaged users did you get out of that? You're not looking for just, you know, how many people did you get to fill out a form? The first one is, Being able to, like, make it really easy to run mutually exclusive experiments. Most modern companies will run, like, hundreds, sometimes thousands of experiments at the same time. And sometimes those experiments don't work well with each other.

**Vineeth Madhusudanan** (00:55:01)

You're testing two kinds of onboarding promotions, and you don't want the same user to actually get both of them. And... Tools that make it super easy to do that are helpful. The other one is just being able to kind of self-service analysis. So part of what differentiates companies that do this at scale from smaller companies is just the fact that, you know, you want PMs to be able to look at experiment results, deep dive into that, and, you know, like slice it by pretty much any cohort they can think of themselves without being dependent on a data team doing that work for them. And that's a key part of kind of enabling that culture.

**Aakash Gupta** (00:55:44)

Got it. Say more about holdouts because I think it can be a somewhat of a controversial topic. What are the right cases and even right business models where you can do a holdout? I think like the big sort of area where people don't do a holdout is if they have to like market a feature to everybody, then they're like worried about it. But yeah. Is that enough of an objection? Should most people just be considering having a holdout for all their experiments over some time period? It comes

**Vineeth Madhusudanan** (00:56:14)

back to kind of what your goals

**Aakash Gupta** (00:56:16)

are.

**Vineeth Madhusudanan** (00:56:18)

So we work with probably the largest retailer in India, and they have an interesting setup where they are a tech company, but they have parallel organizations between what they think of as the business and the tech. So the business is responsible for marketing and, you know, brand and all of those kind of things and tech is responsible for the product. And they're actually far as competitive between the two teams on, you know, how to attribute growth. And like that is a case where they were one of the first few people that actually pushed us really hard on holdouts and wanted to do it because they had the strong motivation to kind of delineate when they had growth, how much of it happened because of product changes that can own the business. And there isn't a better way to quantify your product impact than a holdout. The flip side to holdouts are holdouts are not cheap.

**Vineeth Madhusudanan** (00:57:19)

Holdouts require all kinds of trade-offs. So there is an engineering cost with running a holdout over a long period of time because essentially you're allowing two versions of many features that you've shipped recently to kind of coexist and both of them need to kind of work and not have bugs. You often have, you alluded to, so there's companies like Ancestry in the US that do run holdouts and deal with support calls from people that say, hey, you've been advertising this feature or my cousin has this feature and I don't have this feature and kind of they have ways to kind of deal with that. The other thing with holdouts is also just kind of, you know, often you're running holdouts for a quarter or a six month. If you're not paying attention and something happens that allows you to beat your holdout, it is very expensive to find that out six months, you know, into your holdout.

**Vineeth Madhusudanan** (00:58:14)

So all that stuff is clear, of course. But for a team's way, you know, it is worthwhile to understand kind of the difference between product impact versus things that are happening external to them. They're probably the gold standard. And... for pretty much any find in consumer app i feel like holdouts are pretty much the primary way to do it about you go into things like anonymous apps or things that where the user is not signed in holdouts are much harder to do over a long period of time because now you're reliant on things like cookies that are not good signal over long periods of time but

**Aakash Gupta** (00:58:56)

Yeah. For logged out, it may not be as good a fit, but if you're logged in, um, it's probably makes sense. I think maybe the other skepticism people have around holdouts is like major evolutions in their product. Like we're going to add a new product line. Can we really just avoid giving that to 5% of users?

**Vineeth Madhusudanan** (00:59:18)

Probably not. So there are many... There are situations where hornouts are not a good idea. So like the ones that come to mind are, you know, like if you fix bugs... as the simplest example. Like it's the clearest example of where you probably don't want to hold that out. And you know, you want to give that to all your people. The moment you have network effects. So if you're doing a calling product, for example, within an existing app or a messaging product within an existing app, It doesn't work if, you know, you have the ability to message me and I'm in a holdout group where I don't have this feature. So there's a bunch of product use cases where holdouts aren't the answer. And often, like when I work with customers, we find other interesting things to do. So we do things like, Actually, at Facebook, we'd also think about this as rolling out by country.

**Vineeth Madhusudanan** (01:00:11)

So you'd find a group of markets where most of the connections are kind of local to that. And that's how you would roll out features where you had strong network effects. Yeah, so CoreNote, fantastic for a core set of scenarios. Not the perfect solution for everything, but like just understanding kind of what the costs and the benefits are helps you kind of reason over when to think about them.

<!-- sponsor -->
**Aakash Gupta** (01:00:36)

This episode is brought to you by Sprigg. Meet Sprigg, a product experience platform that generates AI-powered opportunities to continuously improve your product at scale. First, Sprigg captures your product experience in real-time through heat maps, replays, surveys, and feedback studies. Then, Sprigg's industry-leading AI instantly analyzes all of your product experience data to generate real-time insights. Sprigg AI goes even further with actionable product recommendations to drive revenue, retention, and user satisfaction. Join product teams at Figma and Notion by uncovering AI-powered product opportunities at scale. Visit sprig.com slash product growth podcast to book a demo and get a $75 gift card. Okay. And then I think the other sort of area where people might be skeptical is just experimentation in general, like around, for instance, like that new product. They might say, oh, it's better for alpha, beta, GA. What are like the guidelines for when you should A-B test?

<!-- sponsor -->
**Aakash Gupta** (01:01:53)

Probably some basic

**Vineeth Madhusudanan** (01:01:56)

table stakes needs. Like one of them is you need to have enough samples for it to be meaningful. If you have, you know, like I feel like if you have like a over, like once you have over 100,000 users or something like that, you begin to kind of enter the realm of where you can get meaningful signal from this. When you're smaller than that, there's sometimes value in A-B testing, but sometimes there's you know, even more value in just looking at other products around, you know, that have the benefit of KB testing and learning from, you know, what they have done. I worked with some application makers on things like signup flows and things like that. And often when I look at that test, The best advice I can give them is just go look at what Amazon does for their sign-up flow because they have the benefit of A-B testing this on literally millions of users.

**Vineeth Madhusudanan** (01:02:54)

They've figured out the right patterns and you're better off not figuring it out from scratch for where you are. There are obviously... Once you have enough sample size, it is very useful to actually begin to understand your users because what works for one doesn't automatically translate to the other. Facebook has video, YouTube has video. The performance characteristics of both of those are very different because people go to YouTube with the intent of, I want to watch this video. And if it takes a second to start, as long as it plays right, you know, plays really well, they're fine with that. On Facebook, on the other hand, people don't often go to Facebook with the intent of watching video. They're scrolling through a feed. And if the video takes like even maybe 250 milliseconds to start playing, you know, Guess what? They've lost that video view because the user just quite paused.

**Vineeth Madhusudanan** (01:03:51)

And so intent really matter and context matter. So when you have scale, you know, the best way to learn about your users is to do the kind of tests when you don't have that scale. learn from others that maybe have. The other context is also, there's a big difference between B2B and B2C. So with B2B, you often have, like there's, I feel like about, One third of our enterprise customers on Statsig are actually B2B companies for companies like Sigma or Notion. And the types of problems that they have to solve are quite different from like a classic B2C. where, you know, now you end up with these lumpy organizations. You might have two enterprise customers that kind of are well. And when you're doing randomization, if both of them end up in your control group, your basic A-B test has kind of gone for a tux.

**Vineeth Madhusudanan** (01:04:56)

And so there's a class of very interesting problems that have to be solved for B2B when you care about adoption. In the old world, when you just solved B2B and you didn't care about adoption, A-B testing, the value of A-B testing was probably limited, but in the current world, even for us, it's not enough for us to sell Statsync to a company. We have to make sure that they're actually finding value and being successful with it. A-B testing becomes meaningful around how we can actually, I think about it as dropping users into kind of a bit of success. So it's not a mountain they have to climb to kind of hit success. If they, you know, just follow how we nudge them down, they, they should just fall into the spit of success. And testing is definitely a way I find like to learn about that.

**Aakash Gupta** (01:05:47)

Okay. So we talked a little bit about this in the terms of the five features, and now I want to return to it, which is this PM practice of being able to look at your experiment results yourself, not having to go ask an analyst and wait for a week or two, then to finally get your results, but to move a lot faster. What are your best practices for how to look at experiment results as a PM effectively?

**Vineeth Madhusudanan** (01:06:14)

Four. This is actually something that I have really strong conviction around. When I work with companies that are trying to scale experimentation or like kind of get to the next level, they will often come talk to us about how can I get training for my PMs? You know, how can we kind of set them up for success? And they often think about it as like a training problem. And I think more training in the workplace is is actually not very durable. You know, people go to a class, they're sometimes doing something else when they're in the class and then they forget about it when they leave. And I actually look at what companies did with management to kind of learn here. So when you ask people, you know, what is the most youthful manager training? They don't think about it, but it actually is often their performance review process and the calibration meetings they have around that.

**Vineeth Madhusudanan** (01:07:05)

Like, you know, managers go to some class and like, you know, piece from slides or whatever kind of thing. But it's when they're fitting in calibration that they actually learn and realize, oh, this is what this company values. This is what is rewarded. This is what is recognized. This is what, you know, like it's actually, you know, that is calibrating the managers more full than calibrating the employees that they're discussing. The same thing is actually true with experiments. The companies that actually have the strongest experimentation culture use experiment reviews to do the same thing. And the idea is as a PM, when you're designing your experiment, you actually are forced to write up, you know, here is kind of what I'm planning to do. Here is why I think this is a great idea. Here's how I'm going to measure success or not. And this is what success looks like.

**Vineeth Madhusudanan** (01:07:55)

And you write that and people on the larger team kind of look at it and critique it. Ditto when you're actually making a decision. You kind of capture, here is what I observed. Here is what I concluded based on that. And a set of peers around you can kind of look at that and give you feedback on, oh, do you also look at this? Do you miss a piece of context around something we've tried before? Ari, you didn't slice this the right way and you missed an effect that is actually material to the business. And when I joined Facebook, that's how I learned to run experiments. And the act of, you know, actually trying to do it, writing up what I thought about it and having the team around me provide me context was... Well, how I really learned to run experiments, and that is probably the strongest advice I have for people that are building experimentation culture and wanting to kind of set their PMs up for success with being able to do this.

**Aakash Gupta** (01:08:54)

Okay, so tactically what I'm hearing is like the PM before the experiment, like the scientific method is talking about, these are my primary secondary guardrail metrics. Here's how I expect them to move. We'll see whether the null hypothesis is accepted or rejected based on this experiment. And then it sounds like they, you know, use a tool like Statsig or Amplitude or whatever they have to pull those metrics, but then they don't just end there. It sounds like what's critical is that they have a meeting with some of the key people so we can actually talk about the results, think about things that we might not have... thought of or second-order effects that we might want to go look at, things we've learned since you wrote those hypotheses, and that's a really critical part of the process. Am I hearing that right? That is correct. It does, though, require

**Vineeth Madhusudanan** (01:09:44)

a meeting. It can sometimes be done async, like generally things that are low stakes or don't have a lot of contention. You just write up, you know, share in Slack or something like that, and it's just an offline review that happens, but things that are contentious. Because I think Bonifait is also... you know, like as a PM when you're building a feature, you have the strong bias to believe that your feature is good. You know, that is why you're building it. That's why you've convinced a bunch of people to kind of go spend parts of their life building it. And when you look at data, You know, we have so much data available. It's very easy to cherry pick things that support your conviction. Oh, if I slice users by this dimension and this sub dimension and look at data only on Tuesday, you know, I find a piece of data that says supports kind of the strong conviction that I have.

**Vineeth Madhusudanan** (01:10:34)

And that's why the scientific method is actually useful. Like a lot of what we do, like it's kind of funny. When I look at the literature around how to do this properly, a lot of what people talk about with online experimentation actually mirrors, you know, how people do vaccines or how people do like big clients, because it's basically the same thing. And part of that scientific method is critique. And yep.

**Aakash Gupta** (01:11:00)

Okay. What are the biggest, most common mistakes product teams make in experimentation?

**Vineeth Madhusudanan** (01:11:08)

Two biggest mistakes that people make. I alluded to this earlier, but it's kind of this... Sometimes people will draw this direct connection between experimentation and what gets shipped. And I think that is actually a terrible way to build Pranant. And generally, the way I think about experimentation is like, you know, you have this very strong mental model of your users and kind of what is important to them. And when you run an experiment, if something goes up and you don't expect that, You don't ship it. You try and understand why something went up. Because what you want to do is actually improve your mental model about your users and kind of use that to kind of guide what gets shit. So that's probably one misconception that I have about experimenting. I often see it on experimentation. The other one is... What I think of, like, what goals are around experimentation.

**Vineeth Madhusudanan** (01:12:08)

Like, often what I see in companies is, you know, you have a PM that's really excited about experiments. And what he will do is, I got this fantastic idea, and I'm not sure which of these three variants to kind of bend it around. So I'm going to run this as an experiment. But guess what? 80% of their roadmap is a bunch of other ideas that they have strong conviction about that they're just going to ship and run as an experiment. All of a sudden, not run an experiment around. And across a bunch of companies, whether it's Facebook, Microsoft, Google, Amazon, all these companies, For a reasonably well-optimized surface, you know, when they actually measure everything that gets shipped, the numbers are actually astounding. Like roughly about a third of their features that they ship end up being, I thought was good for the user. It is good for the user.

**Vineeth Madhusudanan** (01:12:56)

A third of them end up being, I thought it was good for the user, but I can't detect an uplist when I run an experiment. And this often requires iteration. Like you have to kind of dive into it and understand, oh, did the user not get the value? Did the user not see the prompt? Did the user, you know, get confused and think it was meant for something else? And kind of you have to iterate to kind of unlock that value. And there's roughly about a third of the features that you ship on your roadmap that are actually just bad for your user. Like if you knew the impact, you would unship them and turn them off. And I was talking to, I was at a conference last week and I've talked to someone that ran the experimentation program at booking.com for many years. And what he said was, it wasn't, You know, these fancy ideas we tested and found that allowed us to kind of win when they did.

**Vineeth Madhusudanan** (01:13:47)

It was basically 15 years of unshipping bad ideas. And just that allowed them to kind of beat a lot of their competition. And so I think people think about experimentation as like, let me try these three ideas and ship the best one. But it's really... Like, can you actually, it's not an experimentation, it's just measuring. Can you measure the impact of each feature for that you know, you know, like, oh, that was good. Or in this case, you know, let's unship that.

**Aakash Gupta** (01:14:19)

Yeah. If you look at the data from people like Ronnie Kohavi, who published like the success rate of experiments, I think he published like Airbnb, Microsoft and Amazon. They were all less than 50 percent successful. Like you were saying, kind of like anywhere from a third to 50 percent. So why is that that we producting through this work and less than 50 percent of experiments are successful? Are there things we can do to increase that percentage?

**Vineeth Madhusudanan** (01:14:50)

There's a couple of things to keep in mind. One of them is that we're often trying to do hard things. That is like at its core, that is why, you know, all these percentages that we talk about, like, you know, only a third succeed or less than 50%. It makes the assumption that you're working on a surface that is not very, sorry, you've already kind of a little optimized. So if you're starting with a green slate, I start with a brand new app and I magically have distribution. It's actually often possible to ship a bunch of really good ideas because, you know, you're starting from scratch. You don't have a well-optimized... surface, but often the hardest things that we're working on are surfaces that we've already kind of spent a lot of thought about. And so for Google to find, you know, like a half a percentage point win on their homepage is actually like hugely, wildly successful.

**Vineeth Madhusudanan** (01:15:46)

And they're probably willing to spend like, you know, try a hundred ideas to get one of those things. And, but it comes back to kind of this notion of, you know, you're often trying to do really hard things. all. But the things that you can use to increase your success rate, you know, come back to kind of like the basics of being a good PM. Like there isn't a magic thing around experimentation. It is, you know, having a really strong mental model of your users. And the more you do that, the better productivity, you know, the more the more you do that, you know, the more success you'd likely to kind of end up with. But the other thing is also just realizing that there's no substitute for, you know, shots on goal. So, like, the best thing that I've seen people do is find ways to kind of try a lot of ideas to figure which ones actually have value.

**Vineeth Madhusudanan** (01:16:43)

And sometimes that means like constraining dramatically. I'm only going to follow it for iOS in the US on this surface and validate that it's actually a great idea or people care about this. And when I do, then I go invest and ship it to the whole world and figure out how to support all the platforms and so on. Yeah.

**Aakash Gupta** (01:17:04)

All right. So before we close our section on experimentation, if somebody feels like they're just, you know, average at experimentation, but they want to become world-class, what's your best advice for kind of improving your experimentation culture?

**Vineeth Madhusudanan** (01:17:19)

When you're starting out, probably the number one thing is just increasing your velocity. And the idea behind increasing your velocity is two things happen out of it. When people don't run experiments, there's a lot of friction with running experiments. It's expensive to run experiments. you really want to get to the point where, you know, for your engineer to ship a new feature as an experiment is like literally 15 minutes of work over building the actual feature. And when you get to that point, you know, like then you don't debate and argue and wonder whether you should run the experiment and like the data kind of leads you further. The other thing that happens with velocity is with more turns of the crank, you refine your mental model around what works, what doesn't work, what is important to pay attention, what you should have thought about before, what you should have thought about after.

**Vineeth Madhusudanan** (01:18:15)

And, you know, later you can worry about, you know, more interesting kind of experiments and stuff like that. But the number one thing that I suggest to people is just kind of initially just focus on velocity so that the cost of doing so is like close to zero. And, you know, you get those turns of the

**Aakash Gupta** (01:18:31)

crank. Okay. I love that advice. Let's move over to some PM hot topics. And I love your take here. You said frameworks and processes are meant to lift the average. They're not designed for your top performers. I think that's really profound. Can you explain? A lot of that is around,

**Vineeth Madhusudanan** (01:18:50)

there is a lot of context around the problems that we're trying to solve. And Frameworks and processes sometimes try and abstract that out. One of my experiences when I worked at Facebook was I went over from Microsoft, you know, it took me, I don't know, seven, eight months to get to the point where I felt like I was really comfortable and I was doing well at Facebook. And I noticed this interesting thing that happened to me. Managers of other teams would bring some of their directs to me and say, can you have the Microsoft conversation with them? And really what they wanted me to do was talk to them about, you know, the problem was these people would sometimes see a problem at Facebook and explain to people, when I was at Microsoft, here's how we solved it. And what used to happen at Facebook was instantly when he said those words, people would, you know, like not hear the rest of what he was saying because in their heads, they're hearing, oh, that is Microsoft, that doesn't apply here or whatever kind of thing.

**Vineeth Madhusudanan** (01:19:46)

And sometimes these people actually, you know, like the reason we hired them was because they're smart people and had, you know, like good experience, found specific things that were relevant. And often, you know, my conversation with them would be just leave out at Microsoft part. you know, talk to people at Facebook about here is the problem and here is what, you know, the shape of the solution and why it addresses that. And it can be something that you did at Microsoft and was successful, but leave out that part because then people kind of evaluate it not as a, you know, is this a process that we want to inherit from Microsoft or not? And people kind of look at, here's the core problem and here's the solution and here's, there's either a match or there isn't. And I feel like That the same thing is true, like working at a startup, I've definitely learned this time and again where people, you know, sometimes will say, oh, here's what this other B2B company did.

**Vineeth Madhusudanan** (01:20:41)

Here's what this other SaaS company did. And a lot of those things don't automatically translate to the context that we have, the buyers that we're trying to sell to. And processes sometimes get in the way of kind of figuring out what, or if you're using a template from somewhere else, kind of gets in the way of figuring out what truly matters here. Once you're scaling, you know, these things are amazing. This is how you kind of make sure that things become repeatable, things, you know, that you can do a bunch more of what you initially kind of hand-crossed it and did. But that is the distinction I make between the two. Good PMs know how to bend the rules, and I feel like that is more important than being able to find the perfect template or something like that to use anywhere.

**Aakash Gupta** (01:21:33)

Yeah, I think whether you're in startup or big tech, good BIMs need to know how to bend the rules. What are like the type of rules that are bendable and what are some examples where you've done that? There's probably two

**Vineeth Madhusudanan** (01:21:42)

examples that I can think about with bending rules. One of them is with just, you know, often we have plans around what we're going to build in product and there is a reasonable sequencing we've already figured out. But when you're working with customers, it is important to be able to kind of think about when to disrupt that. Like there are times, there are many a times when I'm working with, you know, some larger customer or something, and I find something that they're asking for that, you know, only they have asked for. When I understand the problem that they try to solve, I realize that, oh, it's not a them problem. It's actually everyone's problem. They're just smart enough to have kind of honed in on it and realized that... It is a material issue for them. And even though nobody else has asked for it, I have the sense that, oh, this would matter to other people.

**Vineeth Madhusudanan** (01:22:35)

And when they find something like that, I am actually very willing to kind of disrupt the set upon, agreed upon plans that we have with the product and quickly find out what can I do to kind of actually validate that This is something that is material for everyone. Because sometimes I think those are the best roadmap ideas that you can actually do where nobody's actually asked for it. Someone smart has thought about it. And, you know, you're like, wow, I can, you know, because you seem, you come across as like a super smart person to all the other people if you land it right. Just because, you know, there was somebody that was smart enough to kind of give you that insight that, you nobody else had thought about. That's an example of one place that basically disrupting your current plans when you find something that is particularly useful to.

**Vineeth Madhusudanan** (01:23:31)

Another example of that is probably just when working with customers, we often have like commercial contractual relationships with customers and things like that. And there are some times when you realize with a particular kind of customer that there's a different kind of value exchange that you can have. So maybe they're giving you enough interesting insight that it's actually worthwhile for you to like dramatically discount the product and make them use a feature that maybe they wouldn't have bought on their own. Or like we use design partners all the time on new things that we're building out. And for when we're doing that, we're willing to kind of bend ourselves backwards. towards doing things that would never scale with those design partners, doing very well that it's not something that we can keep doing. It's not something that we can keep scaling, but like unlock sufficient value for us.

**Aakash Gupta** (01:24:25)

Okay. Another hot topic is just around availability. And I noticed that like compared to the average PM, like you've written like deep content on this. So how can companies and PMs design for failure? I have two thoughts on this.

**Vineeth Madhusudanan** (01:24:44)

One of them is specifically answering a question. When I worked at Microsoft, I spent some time working on the Substripe, which is kind of the code infrastructure that has all the user-level data that Office 365 uses. And the biggest thing that I learned working with that team was the notion of making sure that Any failure you wanted to protect against needed to be a very common failure. You couldn't have failures that only happened once a year because you'd be terrible at dealing with it. And so their approach to building things was they would literally, you know, if they wanted to kill a server, they would literally unplug the server and make sure that the system around it was designed that it could tolerate that. And once you did that, that is how you did deployment. Like we pretty much do that here at StatSig where, you know, when we do deployments, which we do every day, we essentially take down forms and fail over to the other pod for effectively testing kind of what would normally be an outage literally every day.

**Vineeth Madhusudanan** (01:25:48)

And because it is a common pattern, our systems have evolved around it. But the other piece of advice I might have for people that think about this is also kind of reframing problems around reliability as business problems. I spent a year working at Facebook on making video infrastructure better in emerging markets, so in countries like India and places like Africa. And it's kind of funny because it also helps me when I'm here in the U.S. because when I'm inside a big concrete building, you know, my connectivity is as variable as it can be, you know, somewhere far out. But the thing that was kind of interesting to me after spending a year doing that was like roughly our efforts were, you know, about half the work was doing really cool, interesting stuff. Literally half the work across like many teams because, you know, you had people on the mobile apps, you had people on the servers, you had people on the network layer, you had people at CDN worrying about this.

**Vineeth Madhusudanan** (01:26:45)

Half the work was fixing bugs. And it's really hard to go to like a broad set of people and say, hey, we're going to fix a bunch of reliability bugs. Because, you know, it's not uplifting. It's not motivational. It's like, I don't want to spend the next six months of my life working on bugs. But... Like, it's amazing if you're able to kind of frame that problem as, hey, we're going to make video better for, you know, about 2 billion people. And here's, you know, here's the breakdown. Here's how it matters. And here's the thing. It's amazing how much you can rally people towards a goal like that. And that was kind of just a very cool experience to be part of. And like, just that insight was like, yep, this is how we should do reliability programs.

**Aakash Gupta** (01:27:29)

Okay, so now I wanna shift to some of your career lessons. You were a big tech lifer as we've reflected on essentially. Then you moved to a startup, why?

**Vineeth Madhusudanan** (01:27:40)

So, you know, I went to Microsoft Travel and it's funny, the day I decided to leave Microsoft was funnily enough, the day I got a promotion I was not expecting. And it's kind of an odd thing to say, but the thing, you know, the fact that I was not expecting it, I remember realizing, oh my God, I am so comfortable here. Like if I spent another 10 years here, I'd go on to like maybe retire. And I was like, I was curious about what the world was like outside. And I was also curious, like, would my skills transfer? And that's how I ended up at Facebook. When I went to Facebook, I really just looked at where did clusters of people that I'd really enjoyed working with, where had they collected? And that's how I went to Facebook. I had no plans to leave Facebook when I actually joined StatsAid.

**Vineeth Madhusudanan** (01:28:30)

I was doing really well. And when I When I started talking to some of the people at Statsig, I was pretty much like my, I remember telling my wife, like, oh, I should be nice to them because, you know, Vijay, the CEO of, like, senior executive Facebook, and I was like, in startup I was forwarded, he might come back to Facebook, and I might still work with him, so I should be on his good side. And when I started talking to him, the thing I realized was I'd never really thought about startups because I often worked on like large scale infrastructure problems that only big tech worries about. And kind of ruled out like I were working in a startup because I felt like, oh, they now have you for kind of the skill sets that I typically booked. When I started talking to Bijan Statsig, I realized that I was actually not right.

**Vineeth Madhusudanan** (01:29:14)

Like, there were skills that I could bring over and you, and I felt like, It went well. I would unlock a whole new set of capabilities and things that I push myself on, like a whole set of new problems that I've never thought about. And that was kind of my bet for literally when I joined, I was like, oh, I should try for six months. Walscape, I could go back to some big tech thing. But here I am three and a half years later, and I can't imagine, yeah, my world if I had not

**Aakash Gupta** (01:29:48)

made that

**Vineeth Madhusudanan** (01:29:48)

jump.

**Aakash Gupta** (01:29:49)

What are the big changes between working at a fast-moving startup like Statsig versus Big Tech for PMs?

**Vineeth Madhusudanan** (01:29:58)

I think probably the biggest difference for me is the idea of not building for scale. So at pretty much the larger companies, anything that you build will often get way more scale than the scale that we have today after three and a half years. And so that becomes ingrained in kind of how you think about solving problems. Whereas at Statsik, a lot of our discovery has been about what problems are actually worth solving. And often how we do that is by literally building a shitty first version, putting it out and kind of seeing what people's reaction to it is, which parts of it had value, which areas should be fleshed out and which all. And a lot of that is actually, frankly, You know, like I would never ship something like that at some of the big tech companies that I've worked at. And our blast radius is dramatically smaller, so it kind of makes it easier to do that.

**Vineeth Madhusudanan** (01:30:56)

Our feedback loops are also much tighter. So that allows us freedoms that, you know, I would have never had big tech. We actually have a sub stack that we write called Scaling Down. And a bunch of people on the team have written about it because many of us used to work at Facebook before we actually came here, some at Uber, some at other big tech companies. And it was a collection of these learnings around that. I think the other thing for me personally was I feel like when I worked at Big Tech, I actually took some of my excellent partners for granted in the sense that I superficially knew what they did and how they were used. But if I had to go back in time, I wish I'd spent more time kind of understanding how they did what they did. Because like at Big Tech, it was magic and it just happened.

**Vineeth Madhusudanan** (01:31:46)

And now, you know, working at a small startup, particularly in the early days, I was like, oh, I wish I knew how marketing thought about this type of problem. I wish I knew, you know, even simple things like content design. Like when you have a bunch of engineers and PMs writing stuff, you're like, wow. You're like, you know, you suddenly grow to appreciate like what your XFN partners did at Big Tech. And yeah, so like, and probably the last one was probably Oh, yeah, just kind of the learning around building products and selling products. I think at large companies, I never thought about the selling part or didn't spend any kind of related to the last one. Whereas here, it's very much something that I think about as a core part of kind of,

**Aakash Gupta** (01:32:34)

you

**Vineeth Madhusudanan** (01:32:34)

know, building.

**Aakash Gupta** (01:32:36)

Okay. And I think we covered this earlier, but also just the way you do the craft, it seems like there's a lot less focus on documentation. It's a dirty. I think like as a big tech PM, like you're just like your life, at least as I perceive it, like revolves around like product reviews, like eventually getting experiment results and PRDs versus like as a startup, it seems like it's much more like you're almost talking about like core product strategy stuff. Like what problems should we be solving? How are we going to go to market with the solutions? That's probably one of

**Vineeth Madhusudanan** (01:33:13)

my favorite things now that I've worked in a startup for a little bit about kind of working at a start, where I feel like when I worked at big tech, there are some things that you end up doing that are, you know, Maybe performative? Like you do them because the organization expects it of you. Whereas at a startup, there's very little of it that is like that. Like, you know, like many things that would be a meeting at Big Tech aren't a meeting here because they literally are a five-minute hallway conversation and that's good enough. It is also really cool because pretty much everyone sees a direct connection between like some value to the company they understand and the task that is at hand. Whereas the big tech, like that connection between the two is awesome, you know, has so many layers of abstraction. It's sometimes actually hard to tell, oh, here's something that's actually useful versus here's something that, you know, was useful maybe at some part of time, but now it's just enmeshed in a process that is pushed out.

**Aakash Gupta** (01:34:17)

Very cool. So when you made the shift from Microsoft to Facebook, you've said in a couple different places, you learned a new way to build product. Can you explain? There were

**Vineeth Madhusudanan** (01:34:29)

two things that were very different about my Facebook experience related to kind of my context to Microsoft. I think one of them was... Microsoft, you know, a lot of the history around how we build products was steeped at a time when, you know, you had a three-year cycle around building a product. And when you were done with building the product, it got stamped on this special thing that they called a golden CD and taken to a factory where... You know, they then made thousands of copies of it to sell to customers. And so a lot of the process and systems that were engineered were engineered and optimized around kind of this three-year cycle where, you know, if you're an ICPM, you don't actually have a feedback loop outside of your manager telling you whether you're doing the right things or not until three years go by and you ship your product.

**Vineeth Madhusudanan** (01:35:20)

But even then, you know, it's like another two years before people have actually deployed your software. Yeah. And so the Microsoft that I left obviously had changed dramatically from then, but like the roots came from there. When I joined Facebook, on the other hand, I think most people that join Facebook from Microsoft feel like it has barely controlled chaos. And their instinctive reaction is, oh my God, everything is going to, you know. hit the fan like next week. And usually it takes a little bit of time to actually settle in and realize, nope, this is how it is. This is normal. And their success has not come despite this. Their success has come because of this. And I think that was... this notion of kind of barely controlled chaos and, you know, like was an interesting thing to kind of get used to. And one of my learnings there was, you know, like my instinct would be to kind of, oh, let's stop the chaos and let's kind of fix it.

**Vineeth Madhusudanan** (01:36:25)

And really what I learned to do at Facebook was kind of ignore or suppress that reaction and instead focus on this is chaos, this is beautiful. What are the one or two things that I can do to make it better? And kind of stay very focused on that and finding the next things to make better. And that was how, that was one part of kind of the product-based culture. The art part of it was kind of just testing. At Microsoft, when I left, We used to run experiment, but they were not cheap to run, so we were thoughtful about them, and it was a very small subset of things that we actually shipped that we ran experiment for. When I went to Facebook, Facebook had amazing infrastructure such that literally even a bug fix that you were rolling out would get shipped as an A-B test.

**Vineeth Madhusudanan** (01:37:14)

You wouldn't write a hypothesis and stuff like that, but you just do a slow rollout. You roll it out to 2% of your audience, And effectively, you can compare stats for these 2% relative to the rest of the group. And that's what the tools did for you. And it was humbling to do that because, like, you know, we talked about, like, you know, you bid ideas because, or you bid features because you think they're a great idea. And when you can actually measure the impact of it, suddenly you realize that so many of your ideas... either don't have the value you expected or need something else to unlock it. And that was humbling because, yeah, you sometimes shipped what you thought was a great idea and then had to spend time iterating on it to kind of unlock the value there. Or in some cases, realize that the value you had there wasn't something that was real.

**Vineeth Madhusudanan** (01:38:08)

And yeah, that was... It was both humbling, but also probably the biggest change around how I thought about building software.

**Aakash Gupta** (01:38:21)

Okay, very cool. And it's cool and makes sense then that you would go to Statsync to like help other people also live, like what that's like to be able to roll out bugs progressively. I feel like that's something I never got to experience. Now I'm feeling really jealous. So let's move into big tech recruiting. And let's obviously start with Microsoft. So you were there for a while. Maybe can you share some stories or kind of like the inner workings of like how PMs are hired there?

**Vineeth Madhusudanan** (01:38:55)

It's been a little while since I've worked at Microsoft. So the Microsoft that I left, I guess, seven, eight years back is a different Microsoft than now. But the Microsoft that I grew up in, a lot of our PMs were actually grown from within the company. And I feel like when I think about my peer group, like it was probably... less than 10%-ish of my peer group that I worked with that were often, you know, people that had spent a lot of time outside of Microsoft and were relatively newer to Microsoft. And that was both an advantage and a disadvantage. Like the advantage was everyone kind of knew the Microsoft way of doing things and they had a common style around how to approach problems and things like that. and you knew how to get things done with them, which at a large company is often like half the battle.

**Vineeth Madhusudanan** (01:39:52)

Like Hustrick is kind of figuring out what to do and Hustrick is actually getting things done. But I feel like the Microsoft of now is... You have a different Microsoft where like the PM distribution of people that have grown up at Microsoft, life was at Microsoft versus not is very different than that. And so some days I, you know, when I talk to friends there, I'm like, oh, wow, like I feel like going back to Microsoft will feel like a very different Microsoft than the Microsoft I left. And that's kind of exciting.

**Aakash Gupta** (01:40:21)

Yeah, it does feel like even for me, like having advised people about getting jobs at Microsoft, where before it was like everybody was a lifer at Microsoft, basically. And the people you'd see move into program management or product management, whatever their title was, like they might have been in different parts of Microsoft and they really learned that industry or that domain. And then they became the program manager or product manager. So it seems like things have changed dramatically. Now, if some friend came to you and they asked you for help, like, I want to break into Microsoft product management, what would be your tips for them? I think

**Vineeth Madhusudanan** (01:40:56)

A lot of my advice is probably could be similar to other places, but I think, you know, Microsoft, back in the days when they, like, Microsoft invented what they used to call the program management function, which is a predecessor to the current function, or, like, probably back in the 80s or something like that. And they have these documents that were maybe refreshed every 20 years about what it meant to be an OPM, and... I think there's one bit that I remember reading in one of these that kind of stuck with me. And it talked about how, you know, the PM is the person that actually finds what is of value to build and then works with the team to kind of realize that value. And I think that, irrespective of all the places I've worked, is kind of the essence of PM to some extent. And so if you like Microsoft, I think being able to kind of articulate how you have helped find value and how you've helped your team kind of realize a product that realizes that value is probably the biggest thing that I can think about.

**Vineeth Madhusudanan** (01:42:02)

The rest of it is like, you know, like Microsoft focuses definitely on a lot of behavioral interviews and they love being able to kind of talk to examples in your past. And, you know, the usual things that you do around prep around that is actually pretty helpful.

**Aakash Gupta** (01:42:17)

Yeah, usable things being like have a good backlog of stories that you remember the details of, be able to tell them in like a situation, task, action, result format. And the framework that you like, like

**Vineeth Madhusudanan** (01:42:27)

Star or something like that. Like use the place where frameworks are actually useful because they kind of jog you on, oh, like these are the five things to kind of

**Aakash Gupta** (01:42:35)

do right.

**Vineeth Madhusudanan** (01:42:35)

Yep.

**Aakash Gupta** (01:42:37)

Okay. And then shifting over to meta Facebook, whatever you want to call it, what does their process look like? How do they like to hire PMs?

**Vineeth Madhusudanan** (01:42:49)

Probably the biggest difference between Microsoft and Facebook around hiring is like Facebook focus on kind of more key study like examples where it's, you know, they absolutely talk to you about things that you've done in the past, but like they're much more focused about giving you a problem and then seeing you work with them to kind of solve it. And that key study style approach works really well to kind of you know, show how you can understand the problem, how you can work with them to kind of flesh it out a little bit, how you can kind of both form a high level view of what the problem spaces and quickly narrow down kind of, and like, here's how you would prioritize, here's the first set of problems that you would pick on and kind of go almost all the way down to kind of, you know, the nitty gritty of designing that.

**Aakash Gupta** (01:43:40)

Yeah, that's what I've noticed as well, is like Microsoft has a much higher percentage of behavioral. Facebook meta, they'll tell you at the beginning of your process, okay, you have product sense, and then you have product execution, then you have leadership and drive, and they seem to have kind of very specific rubrics for what they're looking for in each of those interviews as well. I noticed the old days when they

**Vineeth Madhusudanan** (01:44:03)

had funner names for those things. So literally like, actually on the engineering side, like you would have a pirate interview, which was literally, you know, like how scrappy can you be? Can you take a problem that you haven't worked with and come up with something that is scrappy and then figure out how to scale that? For across these disciplines, the Jedi used to be the name for kind of the behavioral thing where we were trying to figure out, oh, are you a good... Like, how do you work? Will you work while here? And, yeah. I don't think the Bergson's one did have a cool name.

**Aakash Gupta** (01:44:48)

Okay, so same sort of question. Your friend comes to you and they're like, okay, Vineeth, how do I break into Facebook PM? What would be your tips? The general

**Vineeth Madhusudanan** (01:44:57)

option that I would make is, like, you have a... Everything you've done up until now has been prepped for this. So like, I'm assuming that's already a given. Probably the most useful thing with the case style thing is if you haven't done that type of interview, just find people that you can do mocks with. Case interviewing is definitely something that with practice you become much more comfortable with and getting reps on that is sometimes, like it's really hard to do. prep for that on your own in a room. And just, you know, the actual exercise of going through a mock with a friend or a phone that's worked there or something like that is

**Aakash Gupta** (01:45:35)

helpful. So now you're part of stats saying that's obviously pretty different from big tech recruiting. What are your tips for startup job searching? Outside of things that

**Vineeth Madhusudanan** (01:45:48)

demonstrate your competence, The two things that are particularly helpful I've realized when you're applying for a startup is you know, like being able to show how much you want to be there actually matters a lot. And it's kind of fun. And this expresses itself in, you know, like how much do you understand about the space? Is there some unique motivation or interest that makes you kind of want to be here? And I, you know, like it's funny how much of a difference that makes when we're talking to candidates. I, the other thing that, we hire a lot from big tech, so like pretty much I feel like half of product and engineering, well over half of product and engineering literally worked at Facebook and quite a bit of the rest worked at Uber or Airbnb or a similar company. And one of the things that we kind of worry a lot about is kind of, will they work well in our culture of being really scrappy, of, you know, having this environment where the PRD is sometimes a document, sometimes a literally whiteboard.

**Vineeth Madhusudanan** (01:47:03)

And so being able to show... You know, like, I think it's a combination of being scrappy and being able to make a way, even if there isn't a way, like showing that, you know, you push through things and you can make things happen. Because in addition to kind of the raw skills, that is probably one of the things that we value the most and is critical at like a small startup like a, and being able to kind of, you know, convey clearly that oh this is something that you're good at and it's not just being able to convey but it's like that's also like the rubric that you might use when you're thinking about like a small startup or big tech like are you willing to kind of make a way because at a small startup that is what you'll also be expected to make to

**Aakash Gupta** (01:47:48)

Yeah, that's exactly what I found with startups is like, number one, research the space, actually use the product, understand what they're doing. If you don't have that basics, like people who do, they really shine through. And then being able to demonstrate that if you are in a bigger environment, you can be in the smaller environment. Very, very important. Sort of orthogonal to, you know, type of company job search is like where you're coming from. If you're an engineer and you're wanting to become a PM, how should you approach it?

**Vineeth Madhusudanan** (01:48:19)

So I talk to quite a few people that sometimes want to change across disciplines and become a PM. And the thing that I've realized is when people look at, if you're an engineer and you see a PM, I often think you see things that I think of as product tasks. And I think of product costs as things like, oh, like the person talks to the customer. The person, you know, writes down and makes a list of things the customer cares about. The person comes up with a list of ideas or, you know, works with the team on a list of ideas that we could have picked. And they break them down and kind of figure out sequencing and things like that. And I think when people say they want to dabble with PM or consider PM, they often think about this class of things that is visible.

**Vineeth Madhusudanan** (01:49:05)

There's a whole class of things that I think of as more product thinking, and it's not and visible. So this is, you know, like... gaining insight into, great, the customer cares about this problem, but is this the problem the customer cares the most about or are there other problems the customer cares even more about? Because, you know, it's very, in B2B, it's like crazy. You can go to a practical customer and they will spend 30 minutes telling you about this problem. And if you built a solution for that and go back and ask them, hey, are you going to use it? They're like, yes, maybe, but like, you know, this is really problem number nine on my list of 10 things. And I'm probably not going to get past my first three. And so being able to benefit, like product thinking is not as visible when you're looking at what your PM does, but it's probably the most useful skill that you can build.

**Vineeth Madhusudanan** (01:50:01)

And you can actually build that even in other disciplines. I work with people that, you know, my data science lead is not a PM, but I think of them as a product leader because they actually have this product thinking. And like for people that are wanting to switch, I think being able to find ways to grow their product, thinking is probably the most useful thing that they can do, irrespective of whether they want, you know, completely to come a PM or just be seen as a product leader. That is... The thing people sometimes gravitate towards is, you know, the tasks part of it, which is actually relatively not, you know, it matters, but it's not the hard

**Aakash Gupta** (01:50:46)

part. Yeah, that's the more easily learned part of it. So now we got to shift to the, you know, the hot topic in product management, which is AI. So where I want to start is like, how do you or don't you use AI tools like Zoom's meeting notes, ChatGPT, et cetera, in your day job as a PM?

**Vineeth Madhusudanan** (01:51:05)

So I definitely, actually, we use Gong, which same type of thing. It is incredible how useful AI is at summarization. So like our large enterprise customers, it's amazing. Like it was a game changer to be able to go and say, ask them, oh, what does customer X do with, you know, what warehouse do they use? Or what is the current platform they use? And it can search through like eons of, you know, meeting notes from meetings across maybe three months and like, that was a game changer. The other thing that I do a fair amount of is using ChatGPT for Inspiration. And inspiration not in the sense of getting an idea for what to do directly, but often when I start with a black slate problem, I will go into Chachapiti and ask it to suggest something. And I often find it easier to start thinking about a problem when I see...

**Vineeth Madhusudanan** (01:52:03)

something bad that I can critique. And it's not necessarily that censorship is always bad, but like it's often like, you know, when I see what it puts out, I'm like, oh, it's not right because this is the wrong way to think about it or something. And that sparks how I think about a problem. I definitely use it with You know, if you want to write a product update and you want to fit it within, like, make it really short, ChatGPT is amazing at, like, summarizing maybe my blog post into something that isn't the final version, but, like, is a really good starting point to kind of critique. Same thing, like, G2 reviews. You want to look at a competitor, you want to look at your own, like, just the ability to kind of pipe that into ChatGPT and have it summarized, like, game changer. The thing that we've actually done a hackathon with some, with like HelloFresh or Kustomer, is kind of interesting is, you know, we talk about experiment reviews and experiment reviews often have two parts to it.

**Vineeth Madhusudanan** (01:53:05)

One part is a mechanical part, which is, did you write a hypothesis? Does it match your metrics and things like that? And then there's part of it that is more business context. Are these the right metrics? Are you thinking of like, what should your guardrails be and stuff like that? The lantern is maybe a little harder to automate, but what we did literally in our hackathon was we took their experiment review training, put it into an LLM, and used it to kind of critique experiment designs that people were configuring in Statsing. And I was amazed at how useful it was when... at you know kind of handling kind of the basic newbie things so more the mechanical things but like you know now if you're an experimenter that's just getting started you hit a button and you can kind of see what you would otherwise have to make a slack post wait for people to kind of to take and it's not a replacement for experiment review but like it's amazing how it can complement for the more mechanical parts of it

**Aakash Gupta** (01:54:02)

Tired of spending your days and nights managing all your paperwork processes with multiple tools? Good news. Today's podcast partner, Anvil, is a document AI that helps you build software for your paperwork processes at ludicrous speed. Turn your PDFs into templates in seconds. Anvil document AI identifies input fields, assigns labels, and even prepares your document for signature. What if you could transform your templates into web forms in the blink of an eye and embed them into your application for a seamless user experience? The best part? Anvil separates your structured data from your PDFs so you can power your business with data, not documents. Making it fully operational. The next time you're stuck processing PDFs, creating web forms, or gathering e-signatures, remember you can do it faster with Anvil Document AI. So visit anvil.com slash akash. That's U-S-E-A-N-V-I-L dot com slash A-A-K-A-S-H. Don't get PDF'd. Love those use cases.

**Aakash Gupta** (01:55:15)

Yeah, Gong, if people don't know, is a conversational intelligence tool mainly bought by sales teams, but it sounds like you're using that sales data for your product insights, which is super cool. How do you think AI is going to shape the future of PM in a world of, you know, GPT-7? We've seen like GPT-3 pass the Turing test. GPT-4 can suddenly give itself tasks and go after it and is, you know, much more readable and writes much better. What do the roles of designer, engineer, and PM even look like in, like, a GPT-7 world? I wish I knew.

**Vineeth Madhusudanan** (01:55:47)

We're probably going to find out together, but, like, I suspect there is still value in there's hopefully some kind of insight that... Actually, the honest truth is I don't know. Like, my hope is that, you know, there's still a role for, like, people that understand, you know, the customers, the problems, the trade-offs, and want to do something like that. But there's a lot of, like... prd part of what a pm does that perhaps with that insight becomes you know like instead of the same amount of time i spend creating something on a whiteboard i'm actually able to generate a reasonably well fleshed out prd in the same amount of time i i'd be surprised if you know the core of what you do which is kind of like like find the insights that have the most value and make a bet using kind of intuition if that gets replaced but

**Aakash Gupta** (01:56:52)

It is hard to tell. 100%. Personal question. What's the craziest thing you've ever done? Probably, my wife and me like to do

**Vineeth Madhusudanan** (01:57:03)

things that might be scared of. Often not digital, but like, you know, that scare us a little bit. So we've done random things like gone kayaking for a week in Alaska where we saw probably a hundred times more bears than we saw a human during the week. But probably the scariest thing that I've done is actually out here in Western Washington, where there are these people that allow you to wing walk, which essentially you take off on a small prop plane. And while it is in the air, you sort of tethered, but you climb out of your feet, walk onto the top of your plane and strap into something before they start with acrobatics. And if you enjoy roller coasters, I think it is like the ultimate roller coaster when they're doing barrel rolls and loops and stuff like that with you strapped to the plane outside.

**Vineeth Madhusudanan** (01:57:57)

But that's probably the wildest thing that I can imagine. I sent my parents pictures of it the day I did it. You know, they didn't react. They assumed it was some AI-generated pain because, you know, even when I was trying to explain to them that it was real, they were like, you know, it was just so far outside of their realm of what they thought, you know, is reasonable to consider doing that they were like, they were convinced because an AI stunt.

**Aakash Gupta** (01:58:26)

Yeah, that sounds insane. It takes plane diving to a new level. Okay. So now we're on to the lightning round. The potpourri of questions we ask almost every guest. What's your favorite interview question of product management candidates?

**Vineeth Madhusudanan** (01:58:42)

Usually I love giving the candidate a problem that they are not familiar with. And because part of what I want to do is kind of have them work with me to understand the problem a little better, learn a little bit about it, and usually involves fairly complicated trade-offs. Because what I want to do is kind of get a sense of how they think about trade-offs. And I love kind of working with that together on them.

**Aakash Gupta** (01:59:07)

Okay, all about trade-offs. What's your favorite book with lessons for product and growth people? There's a bunch of books that, you

**Vineeth Madhusudanan** (01:59:15)

know, you learn specific skills from. But one of my favorite books that stuck with me for a while is a book I read a long time back. It's actually almost a parable. And it's called The Perfect Snowball. And it's about this kid that builds, like, the perfect snowball with a group of his friends. And as he's rolling the ball down the hill... the ball gets larger and larger and eventually requires other people to lean in and help kind of roll the ball. And at some point, you know, like there's so many other people helping with the ball that he's no longer running with the ball and able to keep up and kind of steps back. And it's kind of a, I read this book a long time back and it's kind of stuck with me for a while because different people see different things in it.

**Vineeth Madhusudanan** (01:59:57)

You know, parents see, oh, that's what like growing a kid is like. But to some extent, building successful products feels a little bit like that, where you start with the color of an idea with you and, you know, your friends are doing something. And when it picks up momentum, part of allowing it to grow is realizing that you know, you're not going to be the only people working on that. And part of that is kind of, yeah, it's kind of a cool parallel to working on something

**Aakash Gupta** (02:00:25)

that's fun and that grow. Love that parallel. What's a newsletter you anticipate hitting your inbox? Puffy strategy. Oh, it's kind of funny. Like, I can, like,

**Vineeth Madhusudanan** (02:00:38)

Much of what I want to do to keep up with big tech and the big things that are happening in that space, it's like everything you need to go talk to at a party, I feel like Strat Cherry has for you. And I love the level of insight that he actually has around

**Aakash Gupta** (02:00:58)

the

**Vineeth Madhusudanan** (02:00:58)

things that he exposed at.

**Aakash Gupta** (02:01:01)

Yes, case study and like one of the best paid newsletters of all time. Okay. What's a new product you've started using and enjoy? Offslate,

**Vineeth Madhusudanan** (02:01:11)

it is this company called Sunoo.com. Oh, it's actually a very cool product where they... allow you to kind of create your own music. It's like if ChatGPT and Spotify had a baby, like that's what you would have. And they did some really cool things with being able to kind of explore what other people around are creating. And just the creativity that you see there is incredible, where people are putting together, you know, Bangla beat with Dalkan beat for like just, yeah,

**Aakash Gupta** (02:01:43)

it is amazing. Sounds cool. Yeah, I used it when it first came out and made a splash. I'll have to check out the tool again. What product feature or product are you most proud of shipping? There's definitely a recency bias

**Vineeth Madhusudanan** (02:01:56)

here, but like all. From the experimentation at Statsig, when I joined Statsig, the company was like two months forward and we had absolutely no customers. Like when I say no customers, it wasn't even like a free tier person getting and using us. And we, you know, we had no idea whether anyone would buy. And sitting here today where, you know, companies like OpenAI and Anthropic and Notion and Preq are using us is like, Pretty

**Aakash Gupta** (02:02:22)

cool. For sure. And Figma, too, I believe, right? So basically, like, the entire wave of sexy companies right now. What's one particularly memorable product failure that you learned from? I won't have faith, though.

**Vineeth Madhusudanan** (02:02:40)

Wait... Pretty much anything that we were building, if you said it was going to fail, 9, 10 out of 10, you'd probably be right. What is the last few things that I worked on at Facebook was actually we built a live audio product. And this was right when Clubhouse was at its peak. And we tried to do a Me Too thing. And it was kind of cool because it was a blast because... We worked on it for probably about 60 days from, you know, when we started talking about whether we should do it to when we actually did it, got to the point where we had a few million users and stuff like that, and quickly did it afterwards. But in some ways, you know, I had friends that, like, I told you the thing about, like, you know, nine times out of tens, it probably is going to be It probably will fail.

**Vineeth Madhusudanan** (02:03:25)

And it did, but it was still amazing because of all the things we learned. I worked on video for a few years at Facebook and I'd never thought about audio as much as I did in those 60 days. And if I'd seen Facebook, I probably would have, you know, like there's a bunch of things that I would have been better off just for having spent those 60 days working on something that actually didn't go anywhere.

**Aakash Gupta** (02:03:51)

Sometimes our best learnings. All right. Thank you for this in-depth, super deep dive on super senior ICs. We could use the word super 200 times probably in this episode, but it was super hearing from you to make it 201. Where can people find you online and how can they help?

**Vineeth Madhusudanan** (02:04:10)

Layton is probably the easiest place to find me. And barita at, or email vm at statsig.com. That might actually be easy. You don't have to spell out. And I think the thing I've realized over the last couple of years is I'm an experimentation nerd at heart. So I love chatting with anyone that cares about it. So you have a fun story. You have a fun problem. You don't have to be using Statsig. I love to chat about it.

**Aakash Gupta** (02:04:39)

All right. Send Vinith some messages about your experimentation horror stories and learnings, and we'll see you in the next episode, everybody. Bye. See you in the next episode.
