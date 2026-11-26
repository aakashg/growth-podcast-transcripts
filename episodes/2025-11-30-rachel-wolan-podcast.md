---
title: "How Product Leaders Should Use AI, with Webflow CPO Rachel Wolan"
subtitle: "We have a special episode on how Rachel Wolan built an agentic chief of staff and set up her entire $4B product org to work this way."
date: "2025-11-30"
host: "Aakash Gupta"
guests: ["Rachel Wolan"]
speaker_names: "substack"
substack_url: "https://www.news.aakashg.com/p/rachel-wolan-podcast"
youtube_url: "https://www.youtube.com/watch?v=82zF4BUqxkA"
duration: "00:21:36"
word_count: 4080
source: "Substack episode transcript (aired audio)"
sponsors:
  - name: "Linear"
    url: "https://linear.app/partners/aakash"
---

**Sponsors:** This episode is brought to you by [Linear](https://linear.app/partners/aakash).

# How Product Leaders Should Use AI, with Webflow CPO Rachel Wolan

*We have a special episode on how Rachel Wolan built an agentic chief of staff and set up her entire $4B product org to work this way.*

**Aakash Gupta** (00:00:00)

I run my whole day out of cloud code and cursor. These are my AI superpowers, and I'm encouraging my entire team to use them.

**Rachel Wolan** (00:00:07)

This is Rachel Woolen, the chief product officer at Webflow, the $4 billion web giant used by companies like TED Talks, SoundCloud, and even Reddit.

**Aakash Gupta** (00:00:17)

So it's almost like having a data scientist in my pocket.

**Rachel Wolan** (00:00:19)

I think this is the art of building amazing AI-native product. It

**Aakash Gupta** (00:00:23)

gets rid of a lot of the junk in my inbox first, and then it will actually create drafts for a few people that it thinks they need to actually send emails to. And I think that's the one thing I would say about a lot of building an agent is trying it out and then going and adjusting what you want the agent to do.

**Rachel Wolan** (00:00:38)

This is the roadmap to becoming a great product leader. There are tons of tutorials about Cloud Code and Cursor for ICPMs, but what about product leaders? Today's episode is a masterclass. What is this concept and how can CPOs effectively do IC work?

**Aakash Gupta** (00:00:54)

To me, IC CPO means as a leader, you are able to get your own answers to practically any question.

**Rachel Wolan** (00:01:01)

We've just showed all these amazing workflows. How do you set up your organization to work this way? I

**Aakash Gupta** (00:01:07)

think one of the things I would first assume is that

**Rachel Wolan** (00:01:13)

Really quickly, I think a crazy stat is that more than 50% of you listening are not subscribed. If you can subscribe on YouTube, follow on Apple or Spotify podcasts, my commitment to you is that we'll continue to make this content better and better. And now on to today's episode. A quick note for all you audio listeners, most of this episode was a video demo, but we have edited that video demo so it's still a good listening experience. If you actually wanna go see the video demo, we upload the video to YouTube and Spotify and you can find it there. Otherwise, let's get back into the audio version of how to build multi-agent systems. Welcome to the podcast.

**Aakash Gupta** (00:01:51)

Thanks, Akash. Great to be here.

**Rachel Wolan** (00:01:53)

What are we going to do today?

**Aakash Gupta** (00:01:54)

We are going to go through some of my workflows, my agentic chief of staff, and a bunch of different ways that I use Cloud Code and Cursor. And then I'm going to walk you through what it's like to actually build AI native products. in the wild. And we're in the middle of getting a product, a new code gen product ready to go. And so I will walk you through the good, the bad, and the ugly of trying to get a new AI native product out into the wild and into our customers' hands.

**Rachel Wolan** (00:02:21)

Awesome. So as you alluded to there, there's really two sides to AI product leadership. There's being a productive AI product leader, and then there's shipping AI native features. So in the productivity bucket, Let's start here at this concept of IC CPO. What is this concept and how can CPOs effectively do IC work?

**Aakash Gupta** (00:02:40)

Yeah, so to me, ICCPO means that as a leader, you are able to get your own answers to practically any question. And if you stated that as a goal, then you kind of have to work backwards and look at how do I make sure my data is in shape, where I, as well as anybody else on my team, could go and self-serve answers. And that is a large task to undertake, I can tell you that from experience, and we're still in the middle of that. I think the second is making sure your team has the right tools for what they're trying to accomplish and then can even stair step their way up. And then I think the third is really figuring out how and when to model for your team, not because you expect them to copy your workflows, but you want them to be inspired.

**Aakash Gupta** (00:03:26)

I think that part of, you know, being a great leader today is also being a great, I see, and getting your hands as dirty as you can, carving out time to experiment and showing your team that it's okay to experiment. And for sometimes it works, sometimes it doesn't, but that's part of, you know, like building today.

**Rachel Wolan** (00:03:44)

Amazing. So let's start with Claude and Cursor. Can you walk us through how you're doing some of this ICCPO activity through them?

**Aakash Gupta** (00:03:51)

Yeah, absolutely. So what I've done is I've built out what I call my agentic chief of staff. And this is a combination of a set of Claude code agents, rather, as well as an app that I'm building that I use on a day-to-day basis. So first I'll kind of walk you through how I use cloud code. And this is by the way, in cursor, you could do this in any IDE. I also, depending on what my task is, sometimes I will use cursor and the cursor agent. A lot of times if I'm like trying to start something, a project from scratch, I will install from cursor. I will also sometimes use a codex, especially if it's like a complex type of task where I'm trying to understand content from our monorepo. And so I basically am running out of terminal for a bunch of different tasks.

**Aakash Gupta** (00:04:39)

And so what I've done is I've created a set of agents And I'm constantly adding to those agents. So I'll just show you what an agent looks like. And this was generated by Claude. And we'll go through how to actually generate an agent. But this one is understanding the priority of a calendar event and trying to decide if it is truly important. And so what I'll show you is, I actually was running this earlier today. And you're trying to decide, is this part of my priorities? And then trying to filter out noise and then looking for different types of meetings that are very important. And then also really like this is all generated by Claude, by the way. And then what I'm doing. So I ran this earlier today. Let's see. Hopefully it doesn't have anything too crazy in here. And what I, you know, I think I looked at this before I got in here.

**Aakash Gupta** (00:05:36)

And so what I did was first, I asked it earlier today. I ran it because it takes a little bit of time. I asked to look the last two weeks, and I said, can you analyze my calendar, how I spent my time? So analyze my calendar for the week. How did I spend my time? Where could I have been more effective at delegating? So this is something that I do usually like once a week, but I also will run this once a day as well. And then first it kind of gave me like, here are delegation opportunities. These are actually right. I ended up not attending this meeting because I needed to get ready for this podcast. Funny enough, this is a meeting that usually I do send one of my directs to that is our growth lead. This is spot on, right? This is a demo lab that we run called Alpha Arcade, and I usually don't end up attending that one.

**Aakash Gupta** (00:06:28)

Merge Council is something that I have somebody on my direct team. So this is all completely correct. And then it also identified like red flags, like where I'm like double and triple booked. You know, like said, hey, you're not like your context switching too much. I mean, this is this is correct. Right. And this is something that I give to my EA and I'm telling her, hey, like this is this is kind of what I'm seeing. And we'll start with this at the beginning of the week. And then I also like to look forward at the following week and be like, hey, what can we do to improve things? And a lot of it is like, what do you recommend I should cut for next week? I'm not sure. I agree with everything in there, but a lot of this is like a first pass and it's organizing it in a way that makes a ton of sense to me.

**Aakash Gupta** (00:07:17)

And this was just from basically running the agent and giving it that one line.

**Rachel Wolan** (00:07:22)

That's cool. So you've got one of your chief of staff agents. What else are you building around the chief of staff space?

**Aakash Gupta** (00:07:28)

Yeah. So I do the same thing in email. So it has complete access to my email triage and this is spot on. So basically I asked it to triage my email and I think I ran it a couple of times accidentally. What it does is it gets rid of a lot of the junk in my inbox first. but it will first go through and run it. It runs a triage first and then I tell it what to archive. So I don't want like calendar notifications or marketing or systems messages. Then it like pins the messages that are kept and then it will actually create drafts for a few people that it thinks I need to actually send emails to. Right. I don't want it sending emails on my behalf. That's not the point. But I do think that there are like opportunities to where it's like an email that's been sitting in my inbox and sees me.

**Aakash Gupta** (00:08:12)

It kind of is actually like watching the behavior in my inbox. And then, you know, ultimately I'll get into a much, much healthier state. The other thing that was like funny, I ran it this morning and I had a meeting with someone that it didn't have a meeting link and it called it out. So it's like kind of little things like that where maybe there are mistakes and it's not typically acting on my behalf. It's just running the triage for me. So it recommends it would archive 40 emails, right? It would keep it in the inbox. And then I basically say yes or no to go and run those actions.

**Rachel Wolan** (00:08:44)

This is epic. So how would somebody set this up? How do they connect their email and calendar to Cloud Code and give it access?

**Aakash Gupta** (00:08:51)

Yeah, so I basically set up a token in Google. I'm not going to show you my exact ENV setup, but I basically generated a token on Google Cloud and then I store that in my .env file, which is, I'm not going to show you the actual file because it has all of my tokens and regenerate them. But basically I have like an env file and then the reason why it has a, this is basically ignored by cursor, right? This is also ignored by a git. So I have this as like a GitHub repo that I maintain, but it doesn't, this particular file does not get synced. And so there are variables that are in that file and Cloud Code like generates it for you. So it's not, I basically tell it, hey, generate a variable for Gmail, right? And it'll say, okay, it's in this file.

**Aakash Gupta** (00:09:44)

And then I go and I generate it on Google in the console.

**Rachel Wolan** (00:09:50)

Awesome. So we got the high level overview. You're getting your full chief of staff agents This episode is brought to you by Linear. You know what's broken about product development right now? It's not the coding. We've got AI helping with that. It's everything else. The planning, the feedback synthesis, the endless context switching between tools. You're drowning in PM busywork while the actual product work suffers. Linear started as that issue tracker engineers actually wanted to use, which, let's be honest, is pretty rare. But it's evolved into something way more powerful, your entire product development hub. Their new AI features are a game changer for product managers. Product intelligence automatically surfaces insights from customer feedback and support tickets. No more manually combing through hundreds of reports. And their AI agents help draft PRDs, scope projects, and handle all those status updates nobody wants to write. Product teams from OpenAI to Vercel use Linear to build complex products at speed.

**Rachel Wolan** (00:10:42)

There's a reason they call it magical. So visit linear.app slash partners slash Akash. That's linear.app slash partners slash A-A-K-A-S-H. As you talked about, as a leader, we have to motivate others and inspire others. How do you set up your organization to work this way? Obviously, you need to get everybody a cloud code license. You need to allow people to access the MCPs for Snowflake and whatever else that might be needed. But beyond that, how do you really build a product organization that is at the bleeding edge of AI?

**Aakash Gupta** (00:11:16)

This is a great question. So I think one of the things I would first assume is that your organization is going to be like every other adoption curve known to man. So you will have people in your organization that are the early adopters. You'll have the early majority, but you will also have the late adopters and the laggards and then kind of everyone in the middle. And you wanna really figure out how to cater to all of those different people in your organization so that they can start to ascend the ladder themselves. So whereas I might be, I would probably put myself more in early majority, at least if it's hardware, but maybe with software I'm more in the early adopter. I think that I have people in my team where I'm like, hey, I only wanna see prototypes, for example, when you're gonna have meetings with me.

**Aakash Gupta** (00:12:03)

And that's kind of created a dynamic where we spend a lot of time looking at the prototype and they spend a lot of time investing in what that prototype, like what that experience is like. It doesn't mean we don't have a PRD, but we've kind of like shifted away from a PRD in a lot of cases and maybe it's like a more evolving document, right? And so then when I kind of think about how do we train our team, we have, everybody has like access to Figma Make, for example. There's a very, like a much easier tool to sort of learn. And we've taken our design system and made that accessible in Figma Make. We also have a repo that is our design system that is accessible through cursor. We just did a cursor training. We did a Figma Make training. And we've done a couple of these builder days where we have people that are like the champions on our team who are maybe at the bleeding edge, but they are really there to help walk people through getting over the technical hurdles.

**Aakash Gupta** (00:13:04)

And so we're going to do a builder day where everybody has to demo something. And it can be in any of those tools, but you do have to go a little bit outside of what you're comfortable with right now. And ideally, what we saw when we went through that exercise was the first time we did it, we just did it in design. And we basically went from nobody in design using cursor to about 30% of the team using cursor weekly. Now that's kind of crept up a little bit because once you have a base of people using it in an organization, you start to see more and more people leveling up. And then we're about to go do a second builder day and it's going to be for product design and insights, which is like user research and data science. Data science is a different set of use cases for cursor than product managers, than design.

**Aakash Gupta** (00:13:55)

And so a lot of this is like trying to both have people who are champions that are like kind of bottoms up showing things off. And then also saying, here are some of the behavior changes that we expect. We are actually rewriting our career ladder. to incorporate this as an expectation. We're thinking about... So it's like you want people to be supported, but also you want to create the right incentives inside of your team. And then you also want to make sure that you're thinking through like, well, are you just inserting AI for AI's sake? Are you going to get... At the end of the day, you want to get to a better outcome. So I'll give an example that happened to me yesterday. I was in a meeting, this is hilarious, where this designer had put together an amazing prototype. It was awesome. It was really very future forward.

**Aakash Gupta** (00:14:44)

It incorporated a lot of new elements around our answer engine optimization workflow. Uh, this is kind of the new AEO is the new SEO and what we, but somebody, another, like one of the directors of design in my team was like, Hey, I was in this design review where somebody else had a prototype. It looked a lot, you know, like some of the workflows you are building and I want you to, to go and like harmonize your two prototypes. There's a lot easier to do now than like being like you're, you know, so far down the product development life cycle and you're building something. And then you're like, Oh crap. these two workflows don't work with each other. So I think it's really productive, but it's definitely a different way of building.

**Rachel Wolan** (00:15:27)

So many insights packed in there. If I were to synthesize for everybody, at the base of the pyramid, start with access. So we talked about cursor access, cloud code access, Figma make access, then giving the MCP access for those tools. The second layer, supporting your team, whether that's training, builder days, bringing the people who are at the bleeding edge and helping others. And then we talked about getting the incentive structures right. So even changing your career ladder, that's how you actually create these AI native product organizations. So once we conquer the productivity side, the other side is shipping AI native features. And I think you have a really interesting story about eval. So can you tell us that?

**Aakash Gupta** (00:16:07)

Yeah, so one of the things that I think is really fun about building AI native products is so much is changing.

**Rachel Wolan** (00:16:14)

Yeah, I think this is extremely powerful. As a product leader, you need to be leveraging the latest technology. You can't see a trend like all this stuff we just demoed with Cloud Code and not think about how could this be brought to my product. And I love the thinking framework you've given us here of, well, what are my strengths? In Webflow's case, building production apps, having an incredibly large enterprise backing of users, being able to do it on your hosting. Being integrated with the CMS for people who don't understand CMS content management system. This is like where you're actually publishing all your blogs and your pages and the content on them and then leveraging that to build a product. I think this is the art of building amazing AI native products. The final lesson is you need to think about distribution. How do you build products with a distribution first mindset?

**Aakash Gupta** (00:16:59)

Yeah, it's a great question. So I think that if you think about the different waves of innovation that happened, you know, each of those waves has had a different distribution mechanism that product managers have had to learn. And so if you think about the first wave, that was really the internet, and then you needed a way to find websites. So people learned how to optimize search engines. Search engine optimization, there's a lot of dark art to optimizing your website for keywords and keyword stuffing back in the day. It still works. It still works sometimes. And so that was kind of like phase one. Phase two was you were like, okay, I also want to launch a mobile app. And mobile apps also have app engine optimization, right? So people had very similar tactics to get to the top of the iOS store, right? And so that again was a very specific set of tactics to get distribution for your product.

**Aakash Gupta** (00:17:59)

Wave three was social. So you're building for virality. You're trying to get people to discover your product, to come back to your product, to share your product, and on and on and on. That, you know, worked on, it still works on many different platforms. And so these are all still viable distribution paths for some segment. But the next wave is really going to be around how do you get listed in answer engines? How do you get your brand recognized in answer engines? How do you get your, you know, if you make a product change, it's like a major product moment. How do you get that answer engine knowledge to swap out? And so a big part of that is going to come through your website, understanding that you need to feed, you know, a FAQ to your website. and get that updated and that is something that needs to be part of your product process in order to get that information updated or you can use a platform like webflow that does it automatically you need to really think about how are you going to create apps that showcase or maybe highlight part of your experience as you know chat gpt apps start getting adopted and Inevitably, there's going to be all kinds of agentic experiences around these agentic browsers that will also want to interact with your app or with your website or with your e-commerce store, etc.

**Aakash Gupta** (00:19:20)

So really thinking about, I mean, and that's going to be a huge opportunity for growth. right? That's going to be an unseating of how people discover things. And so the more you can understand how people's discovery is shifting, the more you can actually drive growth to your product.

**Rachel Wolan** (00:19:38)

Yes. I think that this is the final thing that so many PMs, they maybe outsource to product marketing or outsource to their execs, but it's actually worth thinking about from the very beginning so that you make it a part of all your plans. So that concludes our masterclass in AI product leadership. We started with AI productivity. We walked you through how to be an ICCPO, how to use cloud code and cursor, how to build agents, what agents Rachel is building, including her amazing chief of staff team of agents, and how to set up your organization. Then we talked to you through the three most important lessons on shipping AI native features, having great evals in place, continually iterating on them, playing off your strength, and thinking about distribution first. This is the roadmap to becoming a great product leader, a top 1% product manager. You have to embrace these tools.

**Rachel Wolan** (00:20:24)

Rachel, thank you so much for dropping all the sauce.

**Aakash Gupta** (00:20:26)

Thank you so much, Akash. It was great to come on and just really appreciate it. Thanks for letting me share.

**Rachel Wolan** (00:20:32)

And if you guys didn't know, I write a paid newsletter of which Rachel has been a subscriber for a really long time, which is really, really special. I only found that out in our pre-call recording. Check that out as well if you want. Check out Webflow for their amazing new app builder and we'll see you in the next one. Bye. So if you want to learn more about how to shift to this way of working, check out our full conversation on Apple or Spotify podcasts. And if you want the actual documents that we showed, the tools and frameworks and public links, be sure to check out my newsletter post with all of the details. Finally, thank you so much for watching. It would really mean a lot if you could make sure you are subscribed on YouTube, following on Apple or Spotify podcasts, and leave us a review on those platforms.

**Rachel Wolan** (00:21:18)

That really helps grow the podcast and support our work so that we can do bigger and better productions. I'll see you

**Aakash Gupta** (00:21:26)

in the next one.
