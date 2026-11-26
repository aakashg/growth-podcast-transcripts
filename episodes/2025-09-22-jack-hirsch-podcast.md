---
title: "The AI PM's Guide to Security - with Okta's VP of PM & AI, Jack Hirsch"
subtitle: "How AI is making your product a target and what to do about it"
date: "2025-09-22"
host: "Aakash Gupta"
guests: ["Jack Hirsch"]
speaker_names: "substack"
substack_url: "https://www.news.aakashg.com/p/jack-hirsch-podcast"
youtube_url: "https://www.youtube.com/watch?v=4dWbwGCPjUY"
duration: "01:30:22"
word_count: 15817
source: "Substack episode transcript (aired audio)"
sponsors:
  - name: "The AI Evals Course for PMs & Engineers"
    url: "https://maven.com/parlance-labs/evals?promoCode=ag-evlas"
  - name: "AI PM Certification"
    url: "https://maven.com/product-faculty/ai-product-management-certification?promoCode=AAKASH550C7"
  - name: "Kameleoon"
    url: "http://www.kameleoon.com/"
---

**Sponsors:** This episode is brought to you by [The AI Evals Course for PMs & Engineers](https://maven.com/parlance-labs/evals?promoCode=ag-evlas), [AI PM Certification](https://maven.com/product-faculty/ai-product-management-certification?promoCode=AAKASH550C7) and [Kameleoon](http://www.kameleoon.com/).

# The AI PM's Guide to Security - with Okta's VP of PM & AI, Jack Hirsch

*How AI is making your product a target and what to do about it*

**Aakash Gupta** (00:00:00)

Okta has been making huge waves. You guys probably get one of the best views into what is happening in cybersecurity out there. What are the wildest AI cybersecurity threats you've seen?

**Jack Hirsch** (00:00:12)

The DPRK is basically planting workers into many of the organizations that you might be familiar with, going through full interview loops, virtual backgrounds, ship laptops, and then there are inside Yeah, there's another one around help desk scenarios. People calling in saying, I need to reset my password. I no longer have access to my corporate email. And then suddenly you've got someone that's come in through a help desk. But ultimately it all comes down to the human element, which is always the weakest link.

**Aakash Gupta** (00:00:39)

Some reports are saying cybersecurity threats are up 40% compared to last year. AI is really enabling these hackers to do more.

**Jack Hirsch** (00:00:47)

Yes, I think 40% is probably a low estimate. Identity actually has become the primary threat vector. Before it was devices, networks, now they're going after the

**Aakash Gupta** (00:00:56)

identity. I

**Jack Hirsch** (00:01:01)

wrote myself a little phishing kit based on the Okta SDKs. That's when I realized if we're not careful, the wheels are going to come off the bus.

**Aakash Gupta** (00:01:09)

Okta is one of the world's largest cybersecurity companies with a market cap of $15 billion. Jack Hirsch is the product leader behind it. He leads all of Okta's core products, including their AI products. Today, we're going to break down what you need to know about AI cybersecurity threats, how to secure yourself against them, and how to build products in this AI age. If you're somebody who's building AI products or building products, there's going to be something for you. Jack, welcome to the podcast. Thanks for having me. Great to be here. Okta has been making huge waves. You guys probably get one of the best views into what is happening in cybersecurity out there. What are the wildest AI cybersecurity threats you have seen?

**Jack Hirsch** (00:01:59)

That's a great place to start. I will say that the threat landscape has changed quite a bit in the past few years. I think just jumping straight to the wildest, I think that the DPRK is basically planting workers into many of the organizations that you might be familiar with. And so what they're doing is going through full interview loops They will have virtual backgrounds. They will be using AI interview tools. They will get onboarded. They will mail their devices to device farms somewhere in whatever country, whether it be the United States, places in Europe. places where they receive laptops and they'll ship them over to DPRK. And then there are inside threats inside. So I think that's one very, very scary threat vector we're seeing across the industry. Yeah, there's another one that's also just as fun, not quite as nefarious, but really needs, or I guess not quite as creative, but really needs focus is around help desk.

**Jack Hirsch** (00:03:07)

So things like MFA resets, right? So people calling in saying, you know, hi, I'm Akash. I need to reset my password. Can you just go ahead and reset my password? Oh, I don't have I no longer have access to my corporate email address. Sign me in, you know, like reset my MFA reset my password and then suddenly you've got someone that's come in through a help desk Oftentimes those get really sophisticated. They will impersonate voices They will go in via slack You know, there'll be threat actors that move laterally and again use all the tools in the like We're all talking about VO for generating small clips of video. There are some really sophisticated threat vectors when you're combining all these like audio and video generation tools, voice changers, et cetera. So yeah, but ultimately it all comes down to, often it comes down to the human element, which is always the weakest link.

**Jack Hirsch** (00:04:05)

So yeah, exciting times in the world of cybersecurity.

**Aakash Gupta** (00:04:08)

Yeah, I think some reports are saying that this year cybersecurity threats are up 40% compared to last year. So it seems like AI is really enabling these hackers to do more.

**Jack Hirsch** (00:04:19)

Yes, I think 40% is probably a low estimate by what we're seeing at Okta. But I will say that one of the things that is most interesting for us at Okta is that identity is actually becoming, has become over the past few years, the primary threat vector. So before it was devices, networks, and people who are attacking systems, right? Poor coding practices. now they're going after the identity, whether that be the physical identity in a DPRK cases or digital identities. So yeah, identity really is the center of modern cybersecurity. So very interesting times, exciting times to be at Okta, exciting times to be working in identity security.

**Aakash Gupta** (00:05:03)

So what was the first moment you realized AI is going to change security forever?

**Jack Hirsch** (00:05:08)

Um, I, uh, I pulled up, uh, a vibe coding, a vibe coding tool. That's not one of the big ones. It was one of the, uh, you know, one of the sort of early movers. And, uh, I wrote myself a little fishing kit based on the Okta SDKs. So look like Okta felt like Okta. And since then, uh, we actually just published a report, um, that sure enough, threat actors have figured this out themselves. Um, but yeah, that's when I realized, uh, if we're not careful, the wheels are going to come off the bus.

**Aakash Gupta** (00:05:40)

Because the vibe coding tools are crazy good at replicating any design.

**Jack Hirsch** (00:05:44)

Absolutely. I mean, especially when the designs themselves, they're SDKs, right? They don't necessarily have to be that good. You just pick a domain name that's one or two letters off of what your target is. You assume they're using insert your identity provider, insert your SSO provider, grab those SDKs and start building. And then it's all about finding your targets and doing the last mile of social engineering to get there. But yeah, it's pretty wild out there.

**Aakash Gupta** (00:06:13)

Being an employee is like scarier than ever. Like those little phishing tests that companies send you, they could just easily catch you now. Why can't traditional cybersecurity stop AI attacks?

**Jack Hirsch** (00:06:28)

Yeah, the reality is traditional cybersecurity, and I think, well, traditional cybersecurity typically focuses on defense in depth strategy, right? There's some combination of device security, network security, and of course, identity security. Identity used to be considered like an IT thing. Like, oh, it's SSO, it's MFA. The IT folks will take care of that. It is very much a security game as of the past five, 10 years. And so the thing that needs to change is that we need to start thinking about identity as the final frontier and the first frontier in terms of stopping cyber threats. So I think that's probably the biggest thing to keep in mind.

**Aakash Gupta** (00:07:13)

How do AI agents change the security equation?

**Jack Hirsch** (00:07:17)

AI agents change the security equation in a couple of different ways. One is they present a threat vector in and of themselves and their capabilities. But I think more interestingly and sort of more nefariously and kind of flying under the radar is that we're deploying AI agents en masse in every single modern organization. And we're not thinking about them as identities that we need to manage that are being granted access to critical resources inside of the organization. And so it was just a couple months ago, the CISO, Chief Information Security Officer of JPMorgan Chase, put out an open letter to the SaaS ecosystem, basically calling out SaaS vendors for not taking this seriously. And there was a hint that AI agents were just making this worse. This idea that we're collapsing authentication and authorization, we're taking these AI agents, we're bringing them into our corporate boundaries, we're giving them unfettered access to our customer data, our user data, and frankly, with little control, little visibility, little oversight, little security.

**Jack Hirsch** (00:08:22)

And so I think That is probably the most clear and present danger today. There's obviously external AI agent threats to modern organizations, but I think the real scariest thing is the fact that security teams and IT teams don't want to be hindering their organization's adoption of AI tools, so they have to let them in. The business always wins and security is always playing catch up, frankly. And so the unfortunate thing there is that oftentimes those things are potentially doing nefarious things, whether the users like them to or not. So that's probably the biggest issue.

**Aakash Gupta** (00:08:59)

AI agents and MCP, I feel like people have been at least talking about security in the circles I come to. What are the underrated things? What are the security threats that nobody is talking about within AI that they should be?

**Jack Hirsch** (00:09:10)

AI, MCP, normal security threats. What else is there outside, but still AI adjacent security threats?

**Aakash Gupta** (00:09:17)

Exactly. Nobody's talking about, but they should be.

**Jack Hirsch** (00:09:20)

Great. Well, I think as context windows are getting bigger and bigger, you can just slurp in an entire API surface and look for various combinations of access patterns and look to go in, you know, what used to be the hard way used to be someone had to be very, very smart, keep a lot of context in their head, understand how different access functions at an API surface fundamentally function. And then now you can just jam that all in an LLM, tell it that you want in, tell the agent to go and they will go. And so I think if you think about how APIs get built at large organizations and API security, There are dozens, hundreds of teams that are building various bits and pieces of API surface. How often are they actually cross-checking different access patterns across those teams, right? Everyone is so siloed. AI is not siloed.

**Jack Hirsch** (00:10:25)

AI will take it all in. AI will find the vulnerabilities and we'll go after them very, very easily. So, uh, and that you do not have to be a sophisticated actor to go after those. So I think, uh, especially a lot of the vibe coded tools that are out there, uh, on the market, this is, uh, I would recommend you build some sort of, um, uh, you know, red teaming concept LLM and turn it loose on whatever application you're vibe coding, especially if you're bringing any sort of sensitive information into it.

**Aakash Gupta** (00:10:55)

I like that. So is the state of the art then to basically train an LLM to red team against you and act as that agent so that you can follow those threat vectors?

**Jack Hirsch** (00:11:07)

I mean, I don't know about state of the art necessarily, but I feel like I would be remiss if I didn't recommend people do that. Right. I mean, you think about a really robust software development lifecycle. You're definitely having security review things before they go out the door. if you don't have a security team what are you going to do right we all talk about having these ai board of advisors right well think about your software development life cycle who are the what are the personas that you want involved in that life cycle you might have a legal review i don't know uh but you definitely want a security review and so training an llm to review the code that you're publishing there's so many like every second day every second hour i should say there's a story about some vibe coded app getting hacked

**Aakash Gupta** (00:11:50)

yeah

**Jack Hirsch** (00:11:51)

um and frankly all of that much of that could have been dealt with if you just would have you know thought adversarially for a beat before you pushed it out

**Aakash Gupta** (00:12:02)

nice I like that so as you're pushing these things out Add that adversarial beat in just like you would have if you weren't vibe coding it. So there's so many other AI threat vectors we haven't even talked about yet, right? AI generated identities, deepfakes, synthetic fraud. What are these are the most dangerous and why?

**Jack Hirsch** (00:12:24)

Um, deep fakes are very, very dangerous. I think on a human level, I think we're seeing, um, I saw Pennsylvania state Senator, I think speaking about how his physical identity was compromised, um, because of a deep fake, right?

**Aakash Gupta** (00:12:38)

Um,

**Jack Hirsch** (00:12:39)

people are, and this is, this is pretty calm. I mean, not pretty common, but I think this, this has made out of the sort of technosphere and into the general news cycle where you'll have, I think the person in question I'm thinking about, their son had some YouTube recordings up, and so they scraped the son's YouTube, grabbed a bunch of their audio, faked their audio, called their dad, who happened to be a Pennsylvania, I believe a Pennsylvania state senator, we should check this afterwards, um and basically said hey i'm in jail uh help me get out i need you know need money and it was a real-time conversation that they had with their son and so i think those things when you extrapolate them out into the software world like Yeah, I might if I were a help desk representative and I got a call from the CEO, I might reset the CEO's password if the CEO called me and said, hey, I need you to reset my password.

**Jack Hirsch** (00:13:37)

I'm locked out. Yeah, that's a really easy way into an organization, unfortunately. And so in the security in security circles, locking down those critical access flows from support desks, that's also a major area of focus.

**Aakash Gupta** (00:13:54)

Crazy. So hopefully people got the picture, right? AI, cybersecurity. If you haven't been hearing about it on the news yet, you should be because it's a serious, serious issue. You guys are at the center of this all. You need to secure your own systems from these types of crazy attacks that you've just been talking about. What is your own AI threat detection system? Walk us through it.

**Jack Hirsch** (00:14:17)

So actually, I'll maybe take this in two angles. One is the same threat vectors of, you know, credential stuffing, like push bombing MFA. So like basically sending MFA pushes through some phishing site over and over and over again until a user relents and just says, like, we need to guard against that. And so at Okta, we have bot detection, fraud detection built into the standard auth flows. And that's evolved quite a bit. It's taking in a bunch of new signal types. But that is sort of business as usual, I would say. It's just evolving with the times. The second part, which I think is actually more interesting, frankly, is the assumption now that identities are effectively compromised. Everyone's identity is compromised. I think the stat that I last saw was somewhere between two and four billion credentials and session tokens and cookies were stolen just in the past year.

**Aakash Gupta** (00:15:13)

wow

**Jack Hirsch** (00:15:14)

and i think that was just from the fortune 1000 alone which is where they were able to get the data so if you think about this the front door is wide open right so you need to ready your defenses so we used to say you know in an enterprise context oh it's all about sso and mfa and securing the point of access well we've all had that experience where you're mfaing over and over and over again it's exhausting right you're getting like oh if you're at work you're okay single sign on into slack single sign on to the team single sign on to this single sign on to that That's exhausting. And then over time, over those like mission critical systems, if you're in a finance system, they might force you to re-auth every few hours or once a day, it's exhausting. So how do you maintain that session security over time?

**Jack Hirsch** (00:15:57)

Because that session security naturally degrades over time, right? You create the session, you cut the cookie, create the token, just by the very fact that that thing exists out in the wild means that there's more likelihood that someone's going to compromise that, right? And so a huge area of focus for us at Okta has been how do we maintain session security over time while keeping the user experience as good or better than pushing MFA all the time.

**Aakash Gupta** (00:16:27)

Yeah.

**Jack Hirsch** (00:16:28)

And so we've taken an approach of, so Okta, you know, this is not about Okta, but I think in general, the open ecosystem approach, which we're huge fans of, we have an open ecosystem approach using open standards like shared signals framework, which is effectively security vendors will share risk signals with each other. So for example, CrowdStrike or Zscaler or Palo Alto networks will share risk signal on behalf of Akash and say like, hey, your identity may have been compromised, but CrowdStrike may have detected it. So what remediations can we take on the identity side to be complementary to device or network security, right? And so I think how we do that in a seamless way, that's been really, really exciting. So maintaining that session security over time and as an end user, i think we don't we don't think about it because ideally the the ideal experience is you're not mfaing all the time you're just seeing continuous access and what's happening in the background is we're continuously re-verifying all of the signal that we have about you has your device posture changed has your network environment changed have you immediately magically traveled around the world to azerbaijan you know in one step like and did we recognize that we would we have first party detections did a third party recognize that and how we orchestrate remediation around the security ecosystem that's been a probably the second area of focus and i think that's new as of the past couple years

<!-- sponsor -->
**Aakash Gupta** (00:17:52)

Today's episode is brought to you by Amplitude. Replays of mobile user engagement are critical to building better products and experiences, but many session replay tools don't capture the full picture. Some tools take screenshots every second, leading to choppy replays and high storage costs from enormous capture sizes. Others use wireframes, but key moments go missing, creating gaps in your understanding. Neither approach gives you a truly mobile experience. Amplitude does things differently. Their mobile replays capture the full experience, every tap, every scroll, and every gesture, with no lag and no performance hit. It's the most accurate way to understand mobile behavior. See the full story with Amplitude. AI evals are one of the most important skills for PMs. And I know you know they matter. The question is, are you doing them right? Most teams are winging it with basic metrics and hoping for the best. Meanwhile, the teams that actually ship reliable AI, they've cracked the code on systematic evaluation.

<!-- sponsor -->
**Aakash Gupta** (00:18:50)

Today's episode is brought to you by the AI evals for engineers and PM's course by Hamil Hussain and Shreya Shankar. This live Maven course will teach you the battle-tested frameworks from Hamil and Shreya. We're the engineers behind GitHub Copilot's evaluation system and 25-plus production AI implementations. Four weeks, live instruction. Next cohort starts July 21st. Start shipping AI that actually works. Enroll at maven.com with my code AG-product-growth for over $800 off. That's AG-PRODUCT-GROWTH. So for customers, what's in Okta's AI security playbook? Give us the secret sauce.

**Jack Hirsch** (00:19:37)

Oh, that is actually really exciting. So we've got some some new things in the works that we have not yet officially unveiled, but I would love to share with you. So we are in the month, so early in August, we announced a new technology with the open ID, basically as part of our, the OAuth standard that we call cross app access. So what this is is a way to allow an AI agent to request access to a resource inside the organization through the central identity provider.

**Aakash Gupta** (00:20:16)

So what

**Jack Hirsch** (00:20:16)

this means is practically imagine like the the Claude 4.1 launch video. had someone asking a question of Claude and it reaching out to Gmail, Google Calendar, Asana, all of those things. Imagine starting your workday as an employee of Acme Corp. And you're day one, right? Employee of Acme Corp. And you sign into Claude, your AI agent companion. and it immediately has access to all of your Google Workspace, your Asana, your Slack, your Salesforce, all of the things that you need to be productive, it's all wired in immediately. That should be the end user experience. Now, the difference is today, if you were to do that, you're doing an OAuth dance. Every user is doing an OAuth dance. You say, oh, you wanna connect Claude to Gmail? Sure, do an OAuth dance. Oh, you want to connect Claude to Asana? Do an OAuth dance. Imagine spraying that out to thousands of employees or tens of thousands of employees at the largest organizations in the world.

**Jack Hirsch** (00:21:23)

So we don't want our customers to go through that. We want our customers to have that elegant experience where all their users just sign in and they start using their AI agents and they're augmented immediately. So that's what we're going for. And so I think from our customers at Okta, generally security and IT practitioners. So for them, the benefit they get is they get visibility into all the agents that are deployed in their enterprise. They get the ability to control with a very granular access. These users might be able to connect Claude just to these applications over here. But these other users, they might be privileged. They can connect Claude to a bunch of other services over here. So they get that granular level of control. They get to manage the life cycle of those AI agents. So I think that's a huge area of investment for us at Okta right now.

**Aakash Gupta** (00:22:13)

So in June of this year, you spoke with Gartner. You broke down T-shaped identity strategies, which I think are deep AI for threats and broad for security. Can you break this down?

**Jack Hirsch** (00:22:22)

Yeah. So this is part of one of the sort of mega trends in identity security these days. We used to think again about identity as being the point of auth, right? secure auth. Well, it turns out that there's a whole user life cycle. So the top of the T is before auth, what do we do to make sure that you're going to have the right level of access to the right things at the right time, no more, no less. And that's it. And that all that happens before you ever hit a sign in box. And then when you go to auth, how can we make it phishing resistant? How can we guarantee that phishing resistance, regardless of what device you're using, whether it be a Mac or PC, iOS, Android, whether you're a managed device, unmanaged device, all of that needs to be phishing resistant. and controlled by the organization.

**Jack Hirsch** (00:23:12)

And then again, the last part of the T is how you maintain that session security over time. So again, as we talked about, session security degrades over time. So how do we maintain that session security without dropping the dreaded MFA, MFA, MFA continuously? and then the the sort of base of the t is about not just having uh so identity used to be thought of as again sso

**Aakash Gupta** (00:23:39)

yeah

**Jack Hirsch** (00:23:40)

now it's so much more it's managing the user's life cycle so joiners and movers and levers like you know jack changed teams Does he have access to the right tools when he changed teams? All of those types of integrations, those are lifecycle management integrations. There's an open standard called SCIM that manages those lifecycle changes. Then it's how do you share risk signals, for example, with other security vendors or tooling. There is actually tooling on both of our devices right now that will share risk signals back with Okta using an open standard. So not just SSO and MFA and lifecycle management, risk signal sharing, but then session termination is another one. So it's how deep you go in those integrations. So session termination would be like, let's say we discover that your identity has been compromised. Oh no. Someone stole a credential off of your device and is replaying it.

**Jack Hirsch** (00:24:37)

I don't know why I want to pick on Azerbaijan, but it's

**Aakash Gupta** (00:24:39)

fun to say and so I'll pick on

**Jack Hirsch** (00:24:40)

them. But say like there's someone else, there's a threat actor replaying your session elsewhere. How do we terminate your session? Not just at the IDP, not just at Okta or on Entra or on Ping or wherever. but in all the downstream applications so that you get signed out of Slack and Zoom and Salesforce and then your device logs you out as well. So how do we shut down access all at once? So that's way more than just the moment of auth. It's maintaining security through that entire end user's lifecycle and having a depth of integration that goes way beyond SSO and MFA.

**Aakash Gupta** (00:25:21)

And

**Jack Hirsch** (00:25:21)

so that's fundamentally what's needed. And that means that you can detect risks. You can respond to them in an automated way. You can mediate them. And so again, you know, the moment we discover that I'm not actually sitting across from you and it's actually a DPRK threat actor, you know, we can terminate this interview immediately. So that's, yeah, maybe the analogy.

**Aakash Gupta** (00:25:43)

So before we close this Okta section here, how many AI-powered attacks do you reckon Okta is stopping per day in your success rate?

**Jack Hirsch** (00:25:50)

Oh, goodness. This, I'd actually want to check with our security team on this. I'm worried about drastically undershooting

**Aakash Gupta** (00:25:59)

because I'm

**Jack Hirsch** (00:25:59)

going to use an M in front of the Iliant and not a B. Oh. But it's of that scale.

**Aakash Gupta** (00:26:05)

Wow.

**Jack Hirsch** (00:26:06)

And so when you think about it, Okta is doing tens of millions of logins a month, right? Okta is so big, and this is actually one of the things that we can talk about if we get into product management as a discipline and sort of the ecosystem. We see macroeconomic trends in our data, right? We are so big that we see those sort of moves, right? And so, yes, absolutely. We're seeing a significant amount of AI powered attacks across the Okta product suite.

**Aakash Gupta** (00:26:33)

Crazy. So let's move into the playbook for any company.

**Jack Hirsch** (00:26:37)

Sure.

**Aakash Gupta** (00:26:37)

What's one thing every company should do this year to protect themselves from AI enabled threats?

**Jack Hirsch** (00:26:44)

number one you cannot get security right without getting identity right um this is not about this is not a pitch or a plea for okta this is uh i guess a plea for every organization to make sure that their users are protected um again threat actors today the vast majority over 80 percent of threat of uh breaches stem from some form of attack on identity yeah And so what that means is every organization needs to get their identity security in order. Um, it's no longer just enough to have SSO. It's definitely not, it's not enough to just have MFA. It's not just enough to have phishing resistant MFA. It's not enough to have, you know, you need to have that continuous session security or else you're going to continue to have those, uh, you know, long lived, uh, session threats. We need, you know, you need to close down support desk and make sure that all of those acts are the, those actions that the support folks can take is logged and controlled.

**Jack Hirsch** (00:27:42)

So all of that is to say is you can't get security, right? Uh, if you don't get identity, right? Um, that's, that's the number one thing.

**Aakash Gupta** (00:27:51)

What are the biggest mistakes companies are making when trying to AI proof their security?

**Jack Hirsch** (00:27:56)

I think assuming that there's going to be a singular solution, frankly. And I think that we've been, you know, we're trained to think about, and when I say singular solution, there are these like monolithic, let's call it microlithic platforms up in Washington, based in Washington that will say, oh, they'll keep you secure. But they'll keep you secure when you're using products in their ecosystem. Right. That's their commercial incentive,

**Aakash Gupta** (00:28:28)

is

**Jack Hirsch** (00:28:28)

to keep their customers safe. And they want to say, oh, if you use something outside of our ecosystem, that's scary. You don't want to do that. And then at the same time, the best of breed world has had a bit of a reckoning too. So if you say, oh, well, I'll take, again, the identity space. Identity and access management used to be thought of as a totally different market than identity governance. Totally different market than privileged access management. all of those markets are converging. And so there's the platformification around all these security vendors. So I think another big area of focus here needs to be on making sure that you're investing in your primary security clouds wisely. And I think identity definitely deserves to be in there. I also think, frankly, network, you need a defense in depth, device strategy, all of these things need to be thought through.

**Aakash Gupta** (00:29:24)

what's the right stage to really just take, like, when do you need to take a really close look at how AI proofed your security is? Is that any stage company? Is there a certain stage you need to reach?

**Jack Hirsch** (00:29:40)

I think anytime you have something to lose. So I'll, uh, This was not so many, many years ago, I worked for a company called Evernote. Evernote famously had a breach where a bunch of usernames and password, salted hash passwords were released. that really that was a huge catalyst for the uh i wouldn't say demise but definitely like they're not considered a winner by any you know by silicon valley standards at this point

**Aakash Gupta** (00:30:16)

yeah

**Jack Hirsch** (00:30:16)

and so they had a lot to lose um and the threat vector there that i i don't know if it's been disclosed but years later i'm pretty sure statute of limitations has expired but like that was related to very similar to a help desk attack, right? That was an identity based attack that eventually got a threat actor in and was able to push code to production to exfiltrate that data. And so, yeah, I mean, I think, you know, in terms of to answer your question very directly, as soon as you have something to lose, if users are using normal credentials to get access to production systems, and they're just using a username and password, that should be a huge red flag. They need to be using phishing-resistant authentication. Every single system that that user uses, they're now a privileged user, every single system that that user uses needs to be phishing-resistant, needs to have risk signal sharing on, needs to have continuous session monitoring.

**Jack Hirsch** (00:31:12)

Yeah, because it is way too easy to hit one of those missteps and lose it all.

<!-- sponsor -->
**Aakash Gupta** (00:31:19)

Today's episode is brought to you by the AIPM certification on Maven. Run by Mikdad Jaffer, who is a product leader at OpenAI, this is not your typical course. It's eight weeks of live cohort-based learning with a leader at one of the top companies in tech. OpenAI just doesn't stop shipping, and this is your chance to learn how. Run along with product faculty and Mo Ali, the course has a 4.9 rating with 133 reviews. Former students come from companies like OpenAI, Shopify, Stripe, Google, and Meta. The best part? Your company can probably cover the cost. So if you want to get $500 off, use my code AAKASH25 and head to maven.com slash product dash faculty. That's M-A-V-E-N dot com slash P-R-O-D-U-C-T dash F-A-C-U-L-T-Y. Today's episode is brought to you by the experimentation platform Chameleon. 9 out of 10 companies that see themselves as industry leaders and expect to grow this year say experimentation is critical to their business.

<!-- sponsor -->
**Aakash Gupta** (00:32:17)

But most companies still fail at it. Why? Because most experiments require too much developer involvement. Chameleon handles experimentation differently. It enables product and growth teams to create and test prototypes in minutes with prompt based experimentation. You describe what you want, Chameleon builds a variation of your webpage, lets you target a cohort of users, choose KPIs, and runs the experiment for you. Prompt-based experimentation makes what used to take days of developer time turn into minutes. Try prompt-based experimentation on your own web apps. Visit chameleon.com slash prompt to join the waitlist. That's K-A-M-E-L-E-O-O-N dot com slash prompt. So everybody needs to do it. So then walk us through your playbook that like for those companies that don't have security professionals, how should they be evaluating if their current security can handle AI threats?

**Jack Hirsch** (00:33:08)

I think so. First off, AI threats in general, it's there's any number of different market segments and categories, right? Are you trying to secure your software, the software that you're actually building? Are you trying to secure your network perimeter, your boundary if you're running a physical operation? uh are you trying to secure your devices so really it's going to depend on the type of organization that you're you're running

**Aakash Gupta** (00:33:34)

yeah

**Jack Hirsch** (00:33:34)

but i think all of that diversity of of types of organizations means that there's only one constant it's identity and i hate to say this coming from okta as the world's leading independent neutral identity vendor but like fundamentally identity is central to security and so you can't get it right uh you cannot get security right without getting identity right so the The way that I would start, frankly, is making sure that identity security is locked down. I think it's at this point, we no longer, most organizations, most startups, I would imagine most of your viewers, they're not going to be working from a skiff, you know, for the DoD, right? They're going to be sitting in a room like this, maybe not with the microphones and lights, but they're going to be working together on something that they think is going to be cool and change the world.

**Jack Hirsch** (00:34:19)

And that's awesome. And they should do that. But as soon as you have something to lose, get that identity security down, right? Because then you're going to have other people. You might have contractors. You might be using, you know, you might be using contracting platforms. to give other people access to various parts of your ecosystem. How do you secure their access? How do you make sure that they have access to the right things only, right? So maybe it's really easy if you have Google Workspace and you're just giving them access to one or two docs and they have their own domain. But as soon as you need to bring them into your trusted boundary, say they're labeling your data for AI, they're working in your code base, they're working in your design base, they're a guest member in your Google workspace, that's when it starts to get very, very real.

**Jack Hirsch** (00:35:09)

And those things happen very quickly as you're scaling. You're going to end up bringing contractors, consultants, business partners, they come in very, very quickly and making sure that they have the right access fundamentally is an identity challenge.

**Aakash Gupta** (00:35:23)

And for people who don't truly grok what you're saying here, basically you're saying that you should have the login for these systems go through an identity portal like Okta, which is identifying, do they actually have access to this? Are they getting the right access? Did I understand that correctly?

**Jack Hirsch** (00:35:39)

That's exactly right. So, you know, fundamentally people think about Okta, it's like, oh, it's a single sign on, right? You sign on once with one set of credentials and I get access to all my work tools. That's sort of where Okta started 10, 15 years ago. And now, sorry, 15, 17 years ago. But now identity is so much more than that. It can't just be that. It can't just be that login box. So that's a simple enabler of IT productivity. But then it's all the security stuff that we were talking about. That's the key driver right now. So as soon as you start exposing any part of your ecosystem and bringing users into your safe boundary, That's when identity becomes critical because ultimately I might be using a device. If you're starting a company and I'm a contractor, I might be using a device that you give me.

**Jack Hirsch** (00:36:29)

Chances are I'm using my device. Do you know if I have malware on my device? Do you know if I'm a malicious actor? How are you logging what's happening in your ecosystem? Identity is that the first and last fence when you don't have network control. If you go work at any of the largest organizations in the world, you're going to be using a VPN on your device. So they know that you're going to be inside a trusted network boundary. You can't do that as a startup, right? You're not going to do that as a startup. Same thing like, oh, there's going to be device management on your device. That means they're going to put a binary on your device and they're going to be monitoring everything that you're doing. They're going to be controlling what websites you go to so that you're not going to download that malware that's going to expose all of their corporate systems.

**Jack Hirsch** (00:37:14)

As you're building, you don't have that

**Aakash Gupta** (00:37:16)

yeah

**Jack Hirsch** (00:37:17)

right and so fundamentally all you have is making sure the right users get access to the right thing at the right time and that's it so uh yeah if i had one easy button for someone starting up or thinking about their security posture and their step one it's identity identity identity that's it

**Aakash Gupta** (00:37:38)

what ai security threat is coming the next few years that companies aren't preparing for

**Jack Hirsch** (00:37:44)

Pass. Um, no, legitimately. I, I honestly, There is so much in flux right now that it is, it is hard to see around the bend. I think we are, so that message of, uh, you know, and you choose to use this or not for the podcast, but fundamentally most organizations have not done the basics and that's not to like shame most of it. Like every, every organization of any consequence has breaches. Spoiler alert, everyone gets breached. Now, it's how you detect it, how fast you respond, what your internal and public responses are to that that separate. Again, I don't want to pick on competitors here or pick on anyone in the security space because everyone gets punched in the nose. Heck, Okta got punched in the nose a couple of years ago. And so you just have to assume that that is going to happen and there are going to be new vectors that come up.

**Jack Hirsch** (00:38:44)

And so securing things like discovering your service accounts. So if you have like standing credentials, you know, and you're building an app, you're using N8N internally and you're orchestrating a bunch of things, but you grab those credentials to your Salesforce. And that's where all your customer data, your CRM, where all your user data is. and you hand that off to N8N and it's just sitting there as a static credential, that's a breach vector. That means that there's a static credential that probably no one is watching. And so you're not putting that in a system where it's locked, where it's being rotated automatically so that if it does get leaked, that it won't be actually be used for nefarious purposes. So there's all these like basics that need to be done in most organizations where like, yeah, the threat vectors will continue to evolve. But if we're as, you know, if we are not evolving our security posture as modern organizations, The basics are going to be the thing that trip us up, not the novel AI driven, you know, threat vector.

**Jack Hirsch** (00:39:44)

It's all identity, identity, identity. Again, 80% today was 80% last year. It was 80% the year before. So again, security, identity, everything else, everything can be secondary after that. And I think that will be a really good way to future-proof yourself.

**Aakash Gupta** (00:40:01)

Okay. So we talked a lot about security. We have one last angle on security, which is building AI secure products. How has AI changed how you build products at Okta and what are your AI security principles?

**Jack Hirsch** (00:40:13)

There's sort of two ways to answer this. One is the products that we're building and delivering for our customers. And the other one is how we build products in the age of AI. And I will start with how we're delivering AI products to our customers. I think we basically made the determination that there are two categories of AI products for our customers. The first are essential AI services. This is what we were talking about earlier, blocking bot attacks, right? Catching credential stuffing, catching MFA bombing. Those sorts of things, we don't want to turn that off. We can't turn that off and keep the system up. It's like turning off DDoS protection. We're not going to do it, right? And so that is just part of keeping our service healthy. We run multi-tenant SaaS. If you get taken down, there might be collateral damage. If someone is DDoSing you, they might have collateral damage on other tenants in that environment.

**Jack Hirsch** (00:41:08)

So we don't want to shut that down. And that keeps us safe. That keeps all of our customers safe. And those are essential AI services. Now, there's the other tier, which are discretionary. Those are things like, hey, we're using an LLM to summarize. How did you get access to the thing you had access to when your identity was compromised? or when we're doing an access review to make sure that, oh, you have access to the super secret Asana Finance workflow. How did you get access to that? Well, we probably want an LLM to summarize that because there's probably umpteen checkpoints that you went through, and I don't know, I'm just making the access mechanism up. We want to summarize how you got access with an LLM. That's discretionary. We can give you the raw log output and you can have at it if you don't want any part of your data processed by an LLM.

**Jack Hirsch** (00:42:05)

So we give our customers the control to either opt in or opt out. So if they're buying and it can be either opt in or opt out, frankly. So like if you're buying a product or a SKU from us, we assume you're opting in. If you don't want that functionality, you don't have to buy the product. Um, but if it comes by default out of the, you know, it comes by default out of the, uh, out of the box, we're going to let our customers turn that off. So for those discretionary services, we want to make sure we give ultimate control to our customers. Uh, we want to make sure, I mean, we work in, you know, global supply chain logistics, trust us with FedEx, the department of defense trust Okta. So we are working, there are healthcare systems that are running on Okta. And so we need to make sure that in whatever regulatory environment, whatever security environment, we're doing the best we can to protect our customers and make sure that they're operating like they want to.

**Jack Hirsch** (00:43:00)

So we got to give that control to our customers.

**Aakash Gupta** (00:43:03)

I just wanted to cover like some people want to build like we just hyped up AI so much, AI threats. So as a PM or as a product builder, what are the things you need to be thinking about to make sure that your product's AI secure?

**Jack Hirsch** (00:43:17)

oh uh well then i think the first thing i would do uh is look into the new oauth standard that's coming out which is cross-app access yeah and so i would imagine that a significant portion of your audience is building b2b sas all right 100 okay 50 great okay 150 or above 50 percent either way excellent excellent so uh if you are trying to deploy software inside of a modern enterprise use the security capabilities that are available to you to become enterprise ready.

**Aakash Gupta** (00:43:48)

Yeah.

**Jack Hirsch** (00:43:49)

So a year ago, we announced a standard with the OpenID Foundation we called Ipsy, the Interoperability Profile for Secure Identity in the Enterprise. But no one cares about that. The acronym is what matters. And it's literally just make sure your app supports SSO. Make sure your app supports lifecycle management so users can be deprovisioned on day one, deprovisioned on their last day. So you don't have random user accounts floating around in your critical systems. It's very, very, very basic things like that. And then with cross app access, make sure that when you're deploying into an enterprise, especially if you're building an AI agent, you should not be tapping all of those users for OAuth grants to every single downstream app they want. Right. So I'll, uh, actually let's, let's use N8N as an example. So let's say that you are deploying N8N into an enterprise, right?

**Jack Hirsch** (00:44:43)

There are two different ways you could go about doing that. One is like min bar access where you say N8N has access to just like the corporate help desk content, right? So I want to use this as like a help desk deflection tool. Well, that's not super secure content. Everyone in the organization is gonna have the same level of access. There's nothing novel that's gonna differ between your access and my access. But that's not gonna change the world. That's not gonna change how people work. What you really want is something, especially when you think about MCP and agent to agent access and agent to resource access, you want something that is gonna know, like if you're deploying an AI agent, that is gonna know that you're you and I'm me, and we each have different levels of access. And so that's what cross app access does is it gives the enterprise the ability to say, hey, the security admins get access to all of these applications here and your AI agent or your application that you're building gets access to those.

**Jack Hirsch** (00:45:41)

So this works for AI agents. It works for to do apps, wiki apps, knowledge management apps. And so the same way that you want to just like basically provision access by using that OAuth standard of cross app access. that is going to give the enterprise visibility and control over those OAuth grants so that your users don't have to do it. And it's going to smooth out the delivery into any modern enterprise going forward. So there's an adoption game there. Don't get me wrong. It's going to take a year or two for that to get adopted. But if you go to websites like enterprise ready and you're looking at like the spec sheet of stuff They have where it's like sock to and you know, oh you must support us So obviously you want to support us. So you definitely want to support provisioning But I think getting the security story straight It will be a an incredible unblocker to get you into any business small or big

**Aakash Gupta** (00:46:37)

Security we talked about it. It was the whole first half of the podcast now I want to move into building products.

**Jack Hirsch** (00:46:42)

Sure. I

**Aakash Gupta** (00:46:43)

So you lead the AI products that are being built at Okta. What are the fundamental principles you guys are following? How are you guys building AI product at Okta?

**Jack Hirsch** (00:46:52)

Maybe I'll just talk about how we build using AI and some principles there. I think that's actually almost more interesting, the AI products. We talked a lot about identity. I think it's sort of how we build, which is interesting and

**Aakash Gupta** (00:47:06)

kind of the

**Jack Hirsch** (00:47:06)

secret sauce. There are three principles or a few principles, and I'll just name three of them. The first one is just use AI to accelerate, not abdicate responsibility. So acceleration over abdication. I think that's one. um two is don't forget your pm fundamentals jumping to prototypes oftentimes leads us to solution, like jumping to solutions without really deeply understanding the problem. And so I think that's two. And then three is like, be aware that we're in an AI hype cycle and don't fall victim to it, right? Really focus on problems, really focus on customer problems, on user pain points, and that will always lead the way to great products. So we can go through this, so like, On the acceleration, not abdication, everyone should be using AI to be better at their job, regardless of their function. Today, if you're not using AI, you are being left behind full stop.

**Jack Hirsch** (00:48:03)

But that doesn't mean that you want to abdicate 100% of your responsibility. Like I imagine that many of the people that are watching, watching this or listening to this, they are looking for ways to be better. And there's a temptation to effectively outsource your entire role to the best prompt you've ever created and the best conversation in your million token context window don't do that that's terrible like that's not why that's not why you were hired right we were hired because you know maybe use ai to get you 80 of the way there

**Aakash Gupta** (00:48:32)

yep

**Jack Hirsch** (00:48:32)

but use your own intellect and your own creativity to hone the last 20 because that's the difference between like you know, original LLM output that's super anodyne and magical content that really helps you, you know, visualize the outcome you want. It feels like you've already had the sparring partner. I've had really wonderful examples of when we didn't do that. We abdicated too much responsibility, and I won't call those PMs out here, obviously, but I was reading a spec once that had a bunch of competitive intelligence in it, and it looked... it looked bland in the way that if you look at a bunch of ai written text you sort of know you're like you don't know but you know without you know without sniffing it

**Aakash Gupta** (00:49:20)

right

**Jack Hirsch** (00:49:20)

yeah yeah you smell it you know and i saw it and i was like just out of curiosity i'll put an ai check and like sure enough 100 ai generated i was like damn it okay i'll just we'll we'll go with it because i assumed that they must have checked it and just use that to sort of rewrite it this particular spec had a bunch of competitive positioning in it And when I brought that to the field, when we brought that to the field, our sales, there was someone who had worked at that competitor and they were like, that is factually incorrect. And all of the assumptions that you've been using to build that product are wrong. And so that was horrible, like change costs for us. We had to like effectively go back to the drawing board. So please use it to accelerate, not abdicate your responsibility.

**Jack Hirsch** (00:50:08)

We hired you because you're brilliant and you're passionate. Use that brilliance and that passion to deliver the last bit.

**Aakash Gupta** (00:50:16)

It hallucinates a lot though. So you really have to check the facts.

**Jack Hirsch** (00:50:19)

Absolutely. And even if you're using, I mean, it doesn't matter which, you know, whether it be, you know, ChatGPT or Grok or Gemini, whatever, like doesn't matter how good you think you've gotten your prompt. There's always going to be hallucination. There's always going to be, I mean, it's like using Wikipedia for your reports, you know, way back when, like you got to check the, check the original sources, right?

**Aakash Gupta** (00:50:42)

Yeah. So that's principle one. Principle two was...

**Jack Hirsch** (00:50:48)

Don't miss solving the real problem. And there's that temptation with prototyping that you want to just... Prototyping is cool, right? We're like, oh, we had this idea and we can go from idea to reality and we can just get customer feedback immediately. That's amazing. And I've seen this so many times where we'll get customer feedback. Yeah, wait a second. What are we solving again? What are we doing again? Why are we here? Oh, wait, we didn't. And then you'll get masked user or customer feedback where they'll say, oh, well, that's really cool. And you're like, yeah, I got positive validation. But cool doesn't mean they're going to buy. Cool doesn't mean it's solving the problem. And so going back to first principles thinking, understanding the problem deeply, that is absolutely mission critical. So I think jumping straight to prototypes definitely risks missing the problem statement. I do think that there's a little bit of a nuance here.

**Jack Hirsch** (00:51:40)

If you're a pre-product market fit or post-product market fit, I think pre-product market fit, you'll probably have a bunch of ideas that might be very problem informed. And you do want to prototype very quickly. Amazing. Absolutely amazing. Post-product market fit, doing that last mile iteration, I've seen it just fall off the rails too many times. So I think don't forget those foundational product management principles. Don't lose them. Go back to go back to basics. Keep the problem in mind.

**Aakash Gupta** (00:52:12)

So what does a PRD look like in a world of AI prototyping?

**Jack Hirsch** (00:52:16)

It always starts with context. I think PMs are ultimately keepers of context, right? We're responsible for what we're building and why, not how we're building it. And so AI has this temptation to just be like, oh, well, we're going to build it. How we're building it? Oh, we're going to vibe code it. We're just going to feel our way into it. The spec still remains very, very problem and customer focused, right? There's going to be business context. There's going to be customer context. There's going to be, depending on the market, there might be competitor context. There might be analytical, you know, there might be qualitative data, quantitative data. I think that's actually something that's a little bit unique about Okta. We have a pretty heavyweight spec process. And it's there effectively to ensure comprehensive thinking, right? Make sure that we're hitting all the angles. So I think there's this temptation to use AI to write specs.

**Jack Hirsch** (00:53:08)

And I saw, depending on the organization, there's a shift in need to go from, you know, we're always like developer constraint, right? Engineering constraint. There's always engineering constraints in every organization. And I've heard in some organizations that they're shifting back, and we felt this a little bit, to product constrained. And so that shift, there's a temptation, again, to abdicate the responsibility of defining a great product, having taste, having sense, having intuition. to ai and that's where it just goes completely wrong so i think specs are still if if done right still focus on user-centered problems customer-centered problems uh market-centered opportunities not uh whatever you know drivel ai will produce on an even

**Aakash Gupta** (00:53:59)

day Because there's that's been the hottest thing right now in product. I think it was Madhu Guru over at Google He's had a product at Gemini. He said we're moving from a writing first culture to a prototype first culture But you think there's still a place for writing?

**Jack Hirsch** (00:54:13)

Oh, absolutely. I mean, I think, you know It doesn't matter where any number of brilliant people smarter than I have Basically said that like writing is the best way to clarify your thoughts. I mean, I think about it In terms of, you know, computing, right? Writing is how I refactor my thoughts, right? And so I need to get my thoughts out on paper. I will use AI to be a sparring partner, which I think is a great use of AI. But again, jumping straight to those prototypes without having that deep understanding and going through the various facets of what it means to be successful and truly understanding, are we solving a need? Are we solving a pain point? And again, deeply understanding that need and living it, wallowing in it, spending time just exploring it, talking to people about that problem without bringing a solution. So again, when you bring the solution, you start overfitting to that solution.

**Jack Hirsch** (00:55:12)

You start forgetting edges of the problem. And you end up with partial solutions. So, um, I think it's, you know, maybe a little bit of a contrarian contrarian take, but frankly prototyping is helpful. Um, but it's too easy to abdicate the deep thinking about the problem that you're actually trying to solve.

**Aakash Gupta** (00:55:32)

So use AI prototyping tools, but once you have conviction on the problem space.

**Jack Hirsch** (00:55:38)

Absolutely. And iteration then can go much faster, right? Iteration can go much faster. But the reality is so many people now are living in a digital native world where like you can pretty quickly spin up. I mean, if you spin up a very, very basic prototype, everyone like we, there used to be so much focus on design principles and understanding, you know, like UX principles. It is so easy now to build incredibly elegant user experiences. that that last prototyping should be like a validation not a testing not you know you should have that taste that intuition to get you 90 95 the way there there's a reason why in general you don't need to user test with more than three to five people right you get you get the you converge at some point yeah exactly and it converges fairly quickly and so if you've been around the block a little bit in product management design user experience you know the patterns and the anti-patterns right out of the gate and you can tell when something is probably going to work more than more often than not

**Aakash Gupta** (00:56:37)

in principle three was

**Jack Hirsch** (00:56:40)

uh there there is an ai hype cycle yeah and so we're in it right the the gartner hype cycle you know you've got your peak of inflated expectations your trough of disillusionment your slope of enlightenment and we are very much in the peak of inflated expectations mode

**Aakash Gupta** (00:56:55)

very

**Jack Hirsch** (00:56:55)

much right and so uh i mean even in your intro you're like oh jack's responsible for ai stuff everyone at octa is responsible for ai stuff And the reality is we need to, again, stay centered on our customers' problems. If AI is the right tool, great, let's solve it with AI. But if a standard linear thought process is the best answer or linear UX flow that has developed the old fashioned way is the right answer, that's also the right answer. We don't have to AI-fi everything.

**Aakash Gupta** (00:57:26)

And it's going to be a lot more reliable and cheaper if it doesn't have AI, right?

**Jack Hirsch** (00:57:30)

Exactly. Well, it depends. There's some efficiencies to be gained with AI. But that whole idea that AI is going to solve everything. I'll take a great example. Building security tool. Let's leave Okta aside. If you're a security professional, you want deterministic steps. to be taken in an incident. You do not want... LLMs, by their nature, are non-deterministic. You do not want to outsource that to a non-deterministic system. And so you need something that is going to operate linearly. You need to define that linear pattern. You are going to be in control of it. There are going to be stage gates along the way. So there are use cases where AI is not quite the best fit. And so I think two years ago, I'd say probably immediately after, and this is after Transformers, but immediately when ChatGPT was announced, the next year, maybe 18 months, everyone was asking, what's your AI strategy?

**Jack Hirsch** (00:58:34)

What's your AI strategy? What's your AI strategy? And the answer is like, well, for Okta, what's our product strategy? And can AI accelerate it? Can AI augment it? Can AI provide new ways to deliver those solutions to our customers? That's the answer. And so AI is fundamentally a tool. It's like, oh, well, we discovered relational databases. What's your relational database strategy? Well, you know, it's a really, really valuable tool. And so, again, we had a wonderful product that we had, we called Log Investigator. And it was this idea that, you know, to decode security logs, you need the decoder ring, right? If you're going to look at security logs, there's all sorts of esoteric context in there. You not only have to be a security professional, in our case, you need to know what's going on in Okta. And we're like, oh, well, we're going to take that.

**Jack Hirsch** (00:59:24)

We're going to feed all the context into an LLM and it's going to explain exactly what's happening. Now, the reality when we actually went and tested this is in those situations, our customers don't want or didn't want non-deterministic output. They wanted deterministic output. They needed the decoder ring, but they didn't want it from an LLM. And so things like, you know, automating configuration. That's a really tough thing to fully hand off to a non-deterministic system. When you know exactly what the acceptance criteria are, maybe there's a lossy path to get there if there are appropriate guardrails. But again, this AI for AI's sake, we have to be really, really careful. And I think there are also like business fundamentals that we tend to forget, right? There's competitive dynamics, there are market forces, there are network effects that we need to be paying attention to as product development professionals, right?

**Jack Hirsch** (01:00:21)

So again, the AI hype is very, very real. The reality is not quite there. Don't get me wrong, is it gonna be transformative? Yes, absolutely. But you know, it's that, that adage that we overestimate what's going to happen in the near term and underestimate what's going to happen in the longterm. Absolutely. We've overestimated what's happening in the near term. Um, and we've forgotten, you know, the basics.

**Aakash Gupta** (01:00:47)

Yeah, AI sprinkles, it hasn't worked for anybody. You have to

**Jack Hirsch** (01:00:50)

actually bake it

**Aakash Gupta** (01:00:51)

into the cake, right? It has to be solving some of the core problems that you were solving. It has to be solving it in a way that other technology, deterministic technology that's usually more reliable, couldn't have solved. So that's the fundamental. I'm curious, AI agents, you didn't talk too much about those. How should PMs be using AI agents? So

**Jack Hirsch** (01:01:12)

first off, even AI agents, there's like, I don't know, they're a nebulous term. How would you define them out of curiosity?

**Aakash Gupta** (01:01:18)

I would say it's an LLM that plans, takes action and reflects. Okay. Think plan, act, reflect, I think is the loop. Yeah.

**Jack Hirsch** (01:01:28)

Okay. That's a, that's a good. Okay. So great. Um, is ChatGPT on its own an agent?

**Aakash Gupta** (01:01:35)

If you turn on the agent mode, it can browse something. I guess it's one step, but the agents that I think PMs should use, if I were to recommend, is a lot of the no-code agent builders out there. Sure. Like Lindy or N8N, we talked a

**Aakash Gupta** (01:01:50)

little bit

**Aakash Gupta** (01:01:50)

about. It's deploying those for your more repetitive work. use cases like an example like in security we just talked about the threats in ai they're changing every single day just to keep up with that it could take you an hour a day so why not create an agent that's summarizing for you hey in the past seven days these were the most important new cyber security ai threats out there here are links to three articles like that type of thing you can create really reliably now

**Jack Hirsch** (01:02:18)

Oh, absolutely. So, so that to me, that to me is a really, uh, I think that's sort of short term, right? This whole idea of, so, but yes, that is an agent. I would actually take a more expansive view of what an agent is, right? I think that Claude in a simple chat interface with MCP is an agent, right? You can tell it to go do a bunch of things and it will go do a bunch of things. even not in necessarily agent mode. I think we're using terms like agent mode to sort of create some differentiation between something that's like goal seek over a longer period of time or goal seek that might have access to a desktop or browser interface. Or it could be something that's like a no code, low code flow builder type thing. I think all of those are derivatives of AI agents, even the very, very basic text box and text response.

**Jack Hirsch** (01:03:15)

So I guess, okay, so back to your question. So yeah, where were we? Let's start with like the expansive view.

**Aakash Gupta** (01:03:22)

Like how should you be using those at work?

**Jack Hirsch** (01:03:25)

Um, I think number one, uh, be pragmatic, um, use the right tool for the job. I think that means we all, okay. So I'll, I'll speak to PMs specifically. Uh, so PMs need to be experimenting with absolutely everything, everything out there. If you're not spending your nights and weekends playing with various AI tools, um, you are going to get left behind. Unfortunately, everything is changing very, very quickly. And that means that you'll be able to use specific tools for specific jobs. And so that means that, you know, you can create your AI board of directors and it's up to you whether you want to use that in Claude or Gemini or ChatGPT or Grok or whatever. or you want to build it in, you know, on some homegrown system, you know, in bedrock, build your AI board of directors. If you want to build automated workflows, you know, and you want to call those agentic workflows, you can, you know, grab N8N, grab the cloud version, you know, or grab the open source version, deploy locally, whatever you want to do, go play with it, go experiment with it.

**Jack Hirsch** (01:04:29)

If you go vibe code some things, go play with it and see what they're good for. And just be wary of that AI hype, right? So

**Aakash Gupta** (01:04:36)

don't

**Jack Hirsch** (01:04:36)

abdicate your responsibility. So I think number one is just be a pragmatic tool user. Yeah. I think second, I would say, and I want to go into, I really want to double down on that AI as a thought partner. Again, fundamentally, you're the knowledge worker, right? You're the one that should be coming up with these ideas. Granted, you can use AI to help you generate those ideas, but fundamentally it's your taste. It's your life. It's your interest. And so if they're, you know, I think one of the things that I learned that was probably most valuable for me from my startup journey is build something you're really passionate about because you're going to be spending every waking hour and minute, seven days a week working on this thing. And so if you outsource that to AI, you're not going to be fulfilled. And so I think really, really use AI as that thought partner.

**Jack Hirsch** (01:05:30)

Think about the types of advice you want, the types of consult you want. Hey, I would love to have you and your entire knowledge base and conversation base as a sparring partner for me as I'm thinking about product management in the era of AI. I would love to ingest all of that and take that all in and build a, build a thought partner out of that. Oh, Hey, I want to build financial excellence. So I need to build financial projections because I'm going to go raise money from a VC. What pitch decks work with pitch deck didn't their databases of pitch decks. Give me all the best, you know, the best tips and tricks. Um, so creating that board of directors, super, super valuable.

**Aakash Gupta** (01:06:12)

And then it sounds like engineering that board of directors with the right context.

**Jack Hirsch** (01:06:16)

Absolutely.

**Aakash Gupta** (01:06:17)

So you just mentioned your startup and that's exactly where I wanted to go next was a little bit about your background. You created an AI startup well before it was cool. So tell us the story of butter.ai. How did it come about?

**Jack Hirsch** (01:06:32)

So first off, the name Butter is really, really important to it. I don't know if you know why it was called Butter. You familiar, you know the show Rick and Morty? Yes. Okay, so you know the Butterbot in Rick and Morty?

**Aakash Gupta** (01:06:44)

Oh, I

**Jack Hirsch** (01:06:45)

don't. Okay, so there's a scene in Rick and Morty where they're sitting around the dining room table, they're having a conversation, and Rick, who's the sort of mad scientist character, fiddling with a robot, and it comes to life on the table. And it rolls over to him and says, what is my purpose? And he says, oh, pass the butter. And the robot comes, you know, passes butter. And he says, thank you. And swipes a piece of butter, you know, on the toast. Conversation keeps going. The butter bot interrupts. And he says, what is my purpose? And he says, oh, you pass butter. And the robot looks down at his little robot hand says, oh my God. And it's like, yeah, welcome to the club, pal. And so it's this whole moment of you realize that your purpose is just to pass butter. And you're sort of this bot, this agent, this AI thing is feigning self-awareness, but is it self-aware?

**Jack Hirsch** (01:07:36)

Is it just feigning self-awareness? We don't know. It's never really discussed in the show. And so we created butter.ai as a way of just passing the information. It was the whole idea is like, you're just going to say, hey, where are the Q3 financials? How did we do last quarter? It's going to find the information. It's going to find the right document. If you don't have the right access to the right document, it'll way find its way through the organization. Ask permission on your behalf if you wanted to grab that information and surface it up to you. So that was the whole. So initially we wanted to call it DocuBot. I thought that was lame. And so we went with butter.

**Aakash Gupta** (01:08:11)

And why did you build an AI startup? What was this, 2017? This

**Jack Hirsch** (01:08:14)

was 2015. Wow. 2015. So timing is everything. And startup folks, don't forget that. Timing is everything. Being too early doesn't always pay. So yeah, I think we overshot it a little bit in terms of timing. This is like just pre-LLM, LLM world. The value of it, I mean, so frankly, we were at Evernote and we had this, we kept having this problem of like, where's that document? Where's that document? We need like a docu bot. We need an enterprise search sucks. It's terrible. And so we need something that's smarter. Search has gotten better. Let's just build that. And so this was one of like a handful of, of, uh, product ideas we were batting around back in 2015. Um, and yeah, we, we test, we did a bunch of, you know, we again, tested a bunch of prototypes. It turns out search is a Sisyphean challenge.

**Jack Hirsch** (01:09:08)

Um, you're never going to get it exactly quite right. And the cost of missing is really hard in enterprise search. So enterprise search is a really hard market to, to play in. It's very, very tempting, especially with LLMs. But it's a difficult market to be in. I

**Aakash Gupta** (01:09:21)

think Glean is kind of in that market

**Jack Hirsch** (01:09:23)

now. Oh, absolutely. And Glean, if you're out there, a huge fan. They actually, I think the enterprise, I don't even know if I would call them enterprise search anymore, but it's sort of where they started. But yeah, this has been going for a long time. We keep trying to solve very similar problems. There was Coveo way back in the day. So like enterprise search is a well-established place. And what's great is we have these technology leaps that create new opportunities to remake whole industries. And Glean is taking a really clever approach now where obviously it's not just about, you know, click through rate and mean reciprocal rank and where in the search results, those things are that you're finding and making sure that it's the top one, two or three. It's about grabbing that information, surfacing the right context out of those documents with LLMs, creating agentic workflows that are sort of like content aware, really cool space to be in really, really hard market.

**Aakash Gupta** (01:10:21)

It sounds like you didn't build, didn't succeed as much as you want to do with butter. Did LLM unlock something specifically for Glean that wasn't there when you were working

**Jack Hirsch** (01:10:31)

on butter? Oh, absolutely. Absolutely. I think we spent, we spent a lot of sort of organizational calories on things like text summarization, NLP. Remember that? Remember natural language processing, understanding. So this is, you know, the first, the first iteration of this was a Slack bot where you could just You could add it to a bunch of channels, you can at mention it, you do whatever, and it would just go find you the bot. And so Slack was the original interface. We also did, we built a Chrome extension so that if you're searching like Google, but your result happened to be in Dropbox, it would say, actually, the thing I think you're looking for is in Dropbox or the thing that you're looking for is in Notion or somewhere else. So the interface, there were a few interfaces to it. But yeah, I wish we had the technology of LLMs.

**Jack Hirsch** (01:11:18)

I think it might have changed some things, but fundamentally, it's a knowledge management challenge. It's really, really hard to get right. And I think that from a business perspective, it's... it's a difficult place to be in i much rather be in the path of revenue i'd much rather be helping customers or users make money save money be more secure there are some like core value props that i think are much more attractive from a business standpoint and i think that you know enterprise like productivity on a personal level so anchored to it, so gravitated. I love the idea of augmenting myself as a human. I felt like Evernote, when I was using it in grad school, gave me superpowers because I could dump everything in there. I could search through case studies and documentation and notes and everything. I just had it all at my fingertips, and I felt superhuman as I was doing that.

**Jack Hirsch** (01:12:15)

That, I think, is enhancing personal productivity as a virtuous cause. I love it. But it's always considered discretionary spending.

**Aakash Gupta** (01:12:22)

Yeah.

**Jack Hirsch** (01:12:22)

And so it was very, very subject to, you know, uh, economic dips, um, and, uh, you know, in a business context, especially in the past few years with everything been being so topsy turvy, that discretionary spending is the first thing to get cut. Um, and so I'd much rather be in those mission critical industries, um, and delivering mission critical outcomes to customers or users.

**Aakash Gupta** (01:12:47)

you're living the dream you're a founder you get acquired and now for the last i guess seven or eight years you've been a product leader what has that transition been like what's kept you in product leadership

**Jack Hirsch** (01:12:59)

the well i will say this and this is uh i love box uh love box love all my former colleagues at box love my current uh people that are still there uh still a huge fan of the people there but i described it to the now cto at box that i felt like i was a bullet hitting jello Just full stop, right? It's just like it took all of this like passion and energy and just ground it to a halt And so I I definitely had a bit of like a crisis while I was at box Because everything was moving slowly I felt like I couldn't like move fast and break things and you know that's sort of the what I wanted and then I realized that I hey, look, this isn't a dinghy that I was used to in startup land. This is a tanker.

**Jack Hirsch** (01:13:46)

This thing, if it turns two degrees northeast, we're moving millions of gallons of water. This is, you're gonna feel the reverberations miles away. right and so the impact of the scale of something like box unparalleled i became addicted to that like that idea of like you know for me it's around like solving hard problems at scale that i really fell in love with um and at okta it's the same thing i mean i mentioned earlier i work at an organization you know where we see macroeconomic trends play out in our data that is wild to me and so that's something that we have to keep in mind in our spec writing process as an example right and so i think i fell in love with you know operating at scale some people do get frustrated with the pace i think the pace is still really really fast um it's just different you know but you but the scale of impact that you have is just otherworldly Um, so, you know, it's a balance, right?

**Jack Hirsch** (01:14:53)

Move fast and break things, but you know, you maybe break a few users versus, uh, move slowly, cautiously, trust, be trustworthy along the way and impact, you know, again, we have to do tens of billions of monthly auths a month at, at Okta. So it's a massive scale. Um, and I found that really, really personally motivating, um, yeah and it's kept me kept me going i also had had a bit of crisis of conscience when i chose product management versus engineering

**Aakash Gupta** (01:15:23)

yeah

**Jack Hirsch** (01:15:23)

that's when i actually had to make this the the choice is uh 2018 during the acquisition they were like which way are you going to go um and so yeah very very glad i went into product management

**Aakash Gupta** (01:15:34)

Okay. So there's a lot of product managers, product leaders, maybe VPs of product and angelic you were at Overnote who are thinking about becoming a founder and they're saying, oh, well his didn't go as well as he dreamed. Like, would you recommend that people just go for it and become founders?

**Jack Hirsch** (01:15:51)

Um, I think there are a few, so blanket statement. Yes. If you have that passion, if you have that, like, I, I can't go to sleep without like thinking about this. I wake up and I'm thinking about it. I'm on a run. I'm thinking about it. I'm exercising. I'm thinking about it. I'm hanging out with my friends and I'm like thinking about it. I want to talk about it. I want to get their opinions on it. Like if you have that fire go, right? Like you're just going to regret it. Um, so I would just say like, if you, if you want to go do that, you should absolutely go do that. I think, you know, in retrospect, I think that it's, it is definitely more calculus than linear algebra. Like there's your optimizing for a set of variables, right? What do I want out of my one precious life?

**Jack Hirsch** (01:16:35)

What do I want to be doing? Do I feel so strongly about this problem that I am ready to spend nights, weekends, every waking hour and more on this problem? I mean, if the answer is yes, then you know your answer already and you should just go do it. but i think there are a lot of people that feel like they should start a company and it's kind of for the wrong reasons they get frustrated because of lack of autonomy right

**Aakash Gupta** (01:17:03)

it's like an

**Jack Hirsch** (01:17:03)

externalized problem right it's lack of autonomy lack of empowerment lack of ability to experiment and they think they have like you know a better a better way of doing something a better process Maybe there's a feature that they wish they could build and they can't and they can't get it off the ground at whatever organization they're at and That's probably not the right set of reasons to go off and found a company. Yeah And so I think there's a and I obviously like in Silicon Valley and tech in general we glorify founders and But the reality is, you know, there's also like the mental health toll on founders that isn't really often talked about. I was surprised to find out that there are like support circles for CEOs.

**Aakash Gupta** (01:17:48)

I was

**Jack Hirsch** (01:17:48)

like, whoa, wait a second. CEOs wear the crown, but also heavy as the head, right? And so I think you don't hear about those stories, right? You don't hear the stories of founders that have significant, you know, real, real emotional health issues, the family issues. Not everyone gets their spot blown up at a Coldplay concert that are, you know, CEOs that, you

**Aakash Gupta** (01:18:12)

know, sorry, I'll leave

**Jack Hirsch** (01:18:13)

that aside. But like, I think, I think reality is we glorify it um we glorify the successes but we all know the stats right the vast majority will fail pretty you know and they'll go quietly no one talks about the failures um and you know i failed back in 2008 right but like that's not what we're talking about here right there's like oh there was an acquisition oh that was a success was it as big a success as i wanted absolutely not i wanted to go much much bigger but we should also like put that into the calculus right if you know that there's a 90 plus percent chance that you're going to go quietly into into the ether are you still are you going to regret not doing it yeah right so if you stare down those odds and go just go do it

**Aakash Gupta** (01:18:58)

So you mentioned Evernote and we have to talk about it because it was like the king of the world where I operate in the productivity space, building a second brain that was like everything. And like you said, that aha moment when you start searching your Evernote database, your notes, you're making connections you didn't think about. It was wonderful back in 2017. Why did it all fall apart?

**Jack Hirsch** (01:19:20)

Oh my gosh, it was still wonderful in 2017. I think so. Yeah, so I guess where do you want to start?

**Aakash Gupta** (01:19:28)

Why is it not one of the big Silicon Valley success stories?

**Jack Hirsch** (01:19:34)

Okay, that's a good question. I'd say probably, let's see, I'll give it three reasons. One is personal productivity just has a limited TAM. Okay, so that's one. I'd say two is Evernote was inherently single player. When Evernote was born, I think it was 2008, 2007, 2008, it was the era of social media where when everything belonged to the world, right? And Evernote was yours. It was your private thoughts. And so everything from the ground up was architected to be single player. And to graduate to the next level, Evernote needed to go multiplayer. And so that was probably two. And then three, so I think we raised too much money, frankly. And we got out over our skis. And so I think there are other like compounding factors there. I think, you know, there was a breach that really that like data wise that set us back between six and 12 months, which in VC funded world, especially late stage, that is an absolute killer.

**Jack Hirsch** (01:20:36)

Right. So I think there's there's other other factors there, but I'd say those three are probably the biggest ones. So, yeah, TAM, inability to transition from single to multiplayer and just raising too much money.

**Aakash Gupta** (01:20:48)

So you had a really interesting story about how you hustled your way into PM at Evernote. How did that happen?

**Jack Hirsch** (01:20:53)

That was actually really funny. It started here in San Francisco. I was sitting in Dolores with a good friend of mine. And he asked me, where do you want to go? What do you want to work on after you graduate from your MBA? Do you want to work at a place like Google? And I said, oh, as much as I love Google, I want to work for something I'm deeply passionate about, something I love. I want to work on a product that I love, something like Evernote. And he was like, oh, my dad works at Evernote. And I was like, oh, interesting. Okay, so I went home. I was going to school in Baltimore at the time, so I went all the way back across the country. On Evernote's website at the time, they had a bunch of coding challenges, so they didn't have any PM roles posted.

**Jack Hirsch** (01:21:32)

They had a bunch of coding challenges for engineers, and I solved all of the coding challenges. I printed them out on paper. I mailed them to my friend and I said, hey, put these on your dad's desk. And on the cover sheet was put on Phil Constantino, the then VP of products desk. And so I got a call a few days later from the then VP of product. And he basically asked, why am I talking to you? And this was like, you know, second year. This is post summer internship of a two year MBA program. And this is like maybe November, December of that year. And he was like, why am I talking to you? And I was like, a winter internship.

**Aakash Gupta** (01:22:14)

oh

**Jack Hirsch** (01:22:14)

and he said oh how much time do you get off your winter internship i don't know three four weeks he's like can you do something in three four weeks i was like absolutely i can do a lot in three to four weeks put me in coach

**Aakash Gupta** (01:22:26)

and

**Jack Hirsch** (01:22:26)

he's like how often are you in california and i was like oh i'm in california all the time i'm actually going to be there next week i literally opened up southwest.com as we're on that call i flew myself like the next day across the country and i showed up at their office like everything was cool and i was meant to be there Wow. And, you know, I had basically three weeks to prove myself. And then the CEO, Phil Libin, was like, hey, you want to join? You got to join now. We're not going to wait six months.

**Aakash Gupta** (01:22:56)

Oh, wow.

**Jack Hirsch** (01:22:57)

And I called my school and I said, hey, how many classes can I miss? They gave me the exact number. And that is exactly the number that I missed. And I was basically flying my way back and forth across the country. And I mean, at the time, like the team that I joined, like they had just been on the cover of Inc. magazine, like they were flying high. This was pre billion dollar, you know, billion plus valuation. But it was like the start of this idea of like, you know, bettering yourself. Right. It was it really was that. iconic personal productivity brand that was blooming and just like crossing the chasm into mainstream. And I just, I wanted to find my seat on that rocket ship and I wouldn't trade it for the world. But yeah, that was my, my intro to PM was starting, starting effectively as an intern.

**Aakash Gupta** (01:23:44)

That's insane hustle, though. So how can people reverse engineer that? I think I guess some of the lessons, right? Network and location. You being in SF and talking to a friend in SF helped because his dad was at Evernote. Number two, like thinking super creatively, I guess, about how to get in, right? Doing coding challenges for a PM interview, very rare. And then I think third thing, taking a lot of initiative to just Yeah, I'll do an internship for three to four weeks, right? Nobody does that. Are there any other elements people should focus on?

**Jack Hirsch** (01:24:18)

I mean, I think so when hunting for roles, I think it's really natural for people to treat it like, I don't know, online dating. Just like swipe left, swipe right. I mean, there are tools now, right? Like, oh, you swipe right on a job and an LLM will apply for you. Yep. cool if you want to play the numbers game great that works i since now it's 2010 i've never i have not played in my career the numbers game at all um and a lot of the people that have grown very rapidly in their career are not playing the numbers game And so find a set of targets that you want to go after and work your way in really hard. I mean, it's really funny. At Evernote, because it was like an IT company, and I'm sure, gosh, you ask any of the late-stage VC-funded IT companies of any era what they saw in the recruiting pipeline.

**Jack Hirsch** (01:25:11)

I've seen people write songs to get in, like play songs on the guitar, send YouTube videos, receive gifts and books from candidates. People are very, very creative to get in, but... again you can't it's not a numbers game you have to know exactly what you want you have to go for it um and so you can call that networking you can call that any number of things but again it's just avoiding the numbers game and being focused i think that's that's really really key i had three to five target companies that i wanted to go at and i effectively didn't want to take no for an answer i mean actually i would have taken no had they turned me down

**Aakash Gupta** (01:25:53)

yeah

**Jack Hirsch** (01:25:54)

actually turn me down but i'm not going to fire something into the void and assume that that is them turning me down that means that i wasn't given the appropriate consideration so like how do i get the appropriate consideration and so doing something that stands out to get you that appropriate consideration you obviously have to earn it after that right the person who wrote a song uh i won't name the employer it won't name the person uh they're a very talented musician they did not get the role because you know that that's step one in the process right it's a it's a funnel Yeah. Um, but I think, I think being much more targeted in the search mission critical, like absolutely have to do that.

**Aakash Gupta** (01:26:28)

I want to circle back to our topic right at the beginning. As we've told people, AI cybersecurity attacks, they're crazy, and they're going to continue to get more and more sophisticated. We walked through the playbook companies must have. Let's end on the personal angle. Let's say my identity gets breached tomorrow by some AI cybersecurity threat. What's the one thing I can do to save myself?

**Jack Hirsch** (01:26:54)

Number one, so your physical identity, your social security number, your credit score, all of that is very, very easy to breach, like trivial, trivial to breach. lock your security reports. Like, it's so easy. Just go to the major credit bureaus, TransUnion, Equif- like, just go to them. There's online fluids. They'll try to get you to pay for them. You don't have to pay. Go lock your credit reports.

**Aakash Gupta** (01:27:21)

Oh.

**Jack Hirsch** (01:27:22)

That means that anytime someone tries to open a checking account in your name, a credit card, sign up for a phone, file an insurance claim, or sign up for an insurance, sign up for insurance, file an insurance claim against your current insurance, all of that stuff, effectively gets blocked while your credit report is frozen. So I think your physical identity is this horrible vestige that we need to be securing. So I think that is number one. And it can be absolutely ruinous if you have had this happen to you. I have actually had my physical identity compromised when I was buying a house.

**Aakash Gupta** (01:27:59)

So I

**Jack Hirsch** (01:27:59)

had to I unlocked my credit report. There was paper that I got mail stolen. I hadn't locked. I didn't know that I had mail stolen. And then I found out that people had used someone had used my social security number. So locking your credit report is number one. Then there's like digital security. So I think physical security. So easy to breach. Lock it down. Digital security. Goodness gracious, please, please, please, please use a password manager. Use strong passwords. Use different passwords for every site. Use passkeys. If you haven't used a passkey, it's magical. Pass keys, actually we can get into why they're so magical and why they're so awesome and why they're so secure. You're not using a password. You are just using a biometric, some sort of biometric marker for yourself. And that's a multi-factor in and of itself because you're using a possession factor and an inheritance factor.

**Jack Hirsch** (01:28:57)

Your possession of your device and something that is inherent to you like your fingerprint or your face ID. So password manager, pass keys, please. And then last one, last bonus, lock your phone number. So oftentimes you will get, you know, probably if you don't use a super modern bank, you'll get MFA codes via SMS. SMS is really, really easy to breach. And so make sure that your phone number is locked with your provider. So I can speak confidently in the United States. Every single phone provider gives you the option to give you some sort of a pin code or secondary security lock that makes it so that you can't steal the phone number and transfer it to another third party SIM. So stealing someone's effectively, their phone number means that if they do happen to get your password, your MFA is compromised, right? Yeah. So SMS is a really bad second factor, it turns out.

**Aakash Gupta** (01:29:54)

So it's

**Jack Hirsch** (01:29:54)

not phishing resistant. And so, yeah, I would say that's probably good. So physical identity with your credit reports, use a password manager, use pass keys. Yeah, that's probably a great start.

**Aakash Gupta** (01:30:09)

This was a masterclass, not just in security, but building AI products, using AI to build products. Thank you so much, Jack.

**Jack Hirsch** (01:30:18)

Thanks for having me.

**Aakash Gupta** (01:30:20)

All right. Bye everybody.
