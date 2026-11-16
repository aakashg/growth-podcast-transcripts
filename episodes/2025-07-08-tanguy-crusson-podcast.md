---
title: "AI Product Discovery: Complete Course"
subtitle: "We're breaking down how to use AI across all 4 stages of Product Discovery: Wonder → Explore → Make → Impact with Jira Product Discovery's Head of Product"
date: "2025-07-08"
host: "Aakash Gupta"
guests: ["Tanguy Crusson"]
speaker_names: "substack"
substack_url: "https://www.news.aakashg.com/p/tanguy-crusson-podcast"
youtube_url: "https://www.youtube.com/watch?v=6oottgko7pQ"
duration: "01:28:28"
word_count: 15463
source: "Substack episode transcript (aired audio)"
---

# AI Product Discovery: Complete Course

*We're breaking down how to use AI across all 4 stages of Product Discovery: Wonder → Explore → Make → Impact with Jira Product Discovery's Head of Product*

**Aakash Gupta** (00:00:00)

Tanguy Coussaint is one of my favorite voices in product management. He worked at Atlassian for over 10 years, and for the last five years, he's been the head of product for Jira Product Discovery. Tanguy, welcome to the podcast.

**Tanguy Crusson** (00:00:16)

Thank you for having me. Super excited

**Aakash Gupta** (00:00:18)

to be here. There are a million things we could talk about together, but today I wanna go really deep on product discovery. And the topic on the top of everybody's minds is, how has AI changed product discovery?

**Tanguy Crusson** (00:00:34)

Yeah, so. I don't think AI has profoundly changed product discovery yet. However, it's got the potential to make it more accessible to a lot more people. So there's a lot of areas where we are currently experimenting or using AI. For example, in my team, I can talk a lot about what we do to make it concrete. But then I'll zoom back to look at this product discovery itself and what it means and how it may differ from how your listeners might be thinking about it. So there are a few areas where we use AI a lot in the job of the discovery team. Probably the most successful experiment we've had so far is with prototyping. So like everyone else, we've tried V0, Bolt, Lovable, and so on and so forth. And we use that to more easily create prototypes that we share with customers in Zoom calls to be able to get feedback faster than to have to spend days trying to create new figmas and iterate on solutions in prototypes that may not be yet fully thought through.

**Tanguy Crusson** (00:01:37)

So instead of doing a drawing on a napkin, we have the ability to create prototypes that are a bit closer to reality and test those with customers. That's probably the most revolutionary use case, let's say, today for AI in discovery, but there's a lot of time savers though. that you can have. So for us, what we save time is on competitor analysis. So instead of asking someone to go and spend a week to look at competitors and their messaging and how we compare to that and how users talk about them and so on and so forth, we can get that in minutes, especially with deep research. And it's usually pretty good for things like this. I use it personally a lot to identify customers to talk to by querying our user feedback we have a lot of it or to get data from customers before joining a call so you know we use Confluence internally the whole company so I might go in there and say hey rovo like what's the what can you tell me about this particular customer and the discussions we've had with them over in the past month And I would have a few seconds later a bit of a summary that helps me understand a bit more the context of this customer for the entire Atlassian product suite, not just Jira, but the discovery, which helps me a lot when joining these conversations.

**Tanguy Crusson** (00:02:56)

We use it to summarize user feedback, go through all the CSAT feedback that we get as well and kind of tell us what the top themes are. And so it's kind of a gut check. uh on the the data that we have ourselves because we spend a lot of time in individual bits of feedback we'll go over that in a moment and it may help with things like writing documents but personally i'm not a huge fan of that i like writing helps me think so if someone does it for me i'm not going to think and that's not good then we've seen a few areas where there's more potential, maybe in the future. And that's probably the part I'm most excited about. And it's about removing the need for intermediaries when talking with users and interpreting what they mean. So for example, we have a lot of salespeople, support, customer success, solution engineers, and they talk to customers and then they come to us to say, this is what we've been hearing from customers.

**Tanguy Crusson** (00:03:56)

And oftentimes, things get lost in translation by having too many intermediaries. And what I'd love to be able to do one day is just plug something on all the feedback, the raw feedback that we get from customers. So every video conversation, so on Zoom, directly there, whether that's a discussion with salespeople, maybe a Gong recording, or a conversation that a researcher has with a customer, another product manager across the company, and being able to go in there and query based on that and try to find moments to watch that could be interesting for us in Java product discovery based on things that we are exploring or things that we're not exploring yet. I wouldn't go as far as saying we could generate synthetic users to ask questions and validate solutions. Personally, I'm not a fan of that. I'm more of a fan of spending time as much as I can actually talking with customers.

**Tanguy Crusson** (00:04:55)

I don't need to be so much with people inside the doors of Atlassian. I need to be with our customers a lot. But if I can find the right people to talk to, and get exposed to as many contexts as I can. That's why we keep experimenting with AI to try and answer that. So that's new things that come with AI, but there's probably still the question on, okay, but what is product discovery that we're trying to help with there? And I've seen a lot of misconception out there as to what that is. So I'd like to cover that a bit. So it's not, yeah. Did you hear stuff about product discovery in all the interviews that you did? Never heard of it. All right, so the biggest misconception, it's not how do I specify the things before building it. It's not I do discovery, then I do delivery.

**Tanguy Crusson** (00:05:48)

It's not that at all. In fact, the term I think was cornered probably 15 years ago by Marty Kagan. It was probably even before that when he was saying, listen, tech people, 50% of the ideas you have will fail. So, and that's just a fact and there's a variety of reasons for that. And so what you need to do is to validate what you can much earlier and answer and address key risks for everything that you're trying to build and do that before committing to building something and keep doing this as you're building it because the most likely outcome is going to be failure. So you're trying to get to a success rate, which is higher and to stop the bite ideas earlier. And the way you are framing it is you need to validate value. So customers actually get value from what you're doing. It might be that, you know, you think it's going to be awesome.

**Tanguy Crusson** (00:06:43)

You give it to customers and they're like, meh, and they don't use it. It might be usability. Your stuff is awesome, but it's so buried somewhere in the app and it's so hard to use that no one ends up using it. It might be feasibility. It's an awesome idea. but let's say you're trying to do something that AI can enable today and you didn't have AI, say, well, five years ago, well, it might be an amazing idea, but without the tech to do it, it's not worthwhile and it should be valuable for your business. If you have a team of five and it's only possible for a team of 50, you might want to think twice. And so those are really key considerations and the job of product discovery is to make sure that at whatever stage you're in, you're trying to address these key risks And your focus is on that, not on when is X going to ship.

**Tanguy Crusson** (00:07:34)

So how that actually shows up in the way we do things, for us, product discovery happens throughout the whole life cycle of everything that we build. And it means talking to customers a lot. It means using prototypes instead of real production code to test stuff. It means working with 10 customers instead of a thousand to try and validate things because it's much faster. And it means testing early prototypes whenever we actually write a real feature with 10 users and telling them all the kind of cases that there is around them and we haven't fixed all the bugs, you know, basically just to make sure that the thing actually answers their problems before committing too far. So for us, it's really about matching the commitment that we give to things to our appetite and keeping iterating on that. Is our investment matching our appetite? And it might be at the beginning during the research, it's amazing, but then it turns out to be much longer to build and we're like, well, there's something else that's much more important that came through since then.

**Tanguy Crusson** (00:08:34)

So are we still okay to spend another quarter on this? Maybe not. And so this discipline of keeping validating, you're focusing on the right things and keeping questioning your assumptions is really what product discovery is about. And it doesn't mean, oh, I now have V0 or Lovable so I can quickly create an app and throw it out there and that's how I test stuff. No, that's still the most expensive way you can test stuff because now people have an app. They've got expectations. You need to maintain it. You need to keep doing iterations on it. And it might be the wrong app. And maybe you can validate that by just working with 10 people and letting them play with the prototype. So for me, the role of a PM is to drive the discovery process and make sure it's infused everywhere from product managers, to designers, to engineers, to working with customers, to educating sales teams about what that is as well.

**Tanguy Crusson** (00:09:28)

And it's not just, the PMs are not just left of code, they're basically throughout the whole journey and trying to make sure that the right investments are there at any point in time. And the role of the PM is to be able to navigate from the strategy questions all the way to the tiny details, all the way back up and to keep doing that gymnastic of going up and down. And I think, I've heard a lot of noise, especially around AI with the collapse of the talent stack, right? So now you've got PMs, you can do design, you can do delivery, but guess what? Most of the great PMs I've worked with, they already do it without AI. The thing is, in many ways, when I look at all these PMs, we're all overstretched, overworked, and work-life balance suffers a bit. And I think the potential I can see with everything that we've seen coming out of AI right now is ways to actually make it a job which is feasible because it's currently transitioning from tech teams to a lot of companies out there that are not in tech at all.

**Tanguy Crusson** (00:10:33)

And I think we need to be reasonable with expectations. And right now I'm loving a lot of things I'm seeing, especially on prototyping to help maybe less senior PMs actually adopt these practices and have to do a lot less of the heavy lifting that we oldies used to have. to do.

<!-- sponsor -->
**Aakash Gupta** (00:11:11)

Transcription by CastingWords That's A-T-L-A-S-S-I-A-N dot com slash product dash discovery. Jira Product Discovery. Build the right thing. Today's episode is brought to you by the AIPM certification on Maven. Run by Mikdad Jaffer, who is a product leader at OpenAI, this is not your typical course. It's eight weeks of live cohort-based learning with a leader at one of the top companies in tech. OpenAI just doesn't stop shipping, and this is your chance to learn how. Run along with product faculty and Mo Ali, the course has a 4.9 rating with 133 reviews. Former students come from companies like OpenAI, Shopify, Stripe, Google, and Meta. The best part? Your company can probably cover the cost. So if you want to get $500 off, use my code AAKASH25 and head to maven.com slash product dash faculty. That's M-A-V-E-N dot com slash P-R-O-D-U-C-T dash F-A-C-U-L-T-Y. It seems like every PM you talk to is just, oh, my calendar is slammed, my to-do list is slammed.

<!-- sponsor -->
**Aakash Gupta** (00:12:39)

And so AI is going to be one of those things that allows PMs to focus on these high leverage tasks, these discovery tasks to get out of the minutia, the details sometimes that can bog down people like status updates and things like that.

**Tanguy Crusson** (00:12:58)

Yeah, that's correct. It's got the potential to do all this. And you can already experiment with a lot of it today. You know, you throw your user feedback at it and you ask questions. But keep looking at the user feedback yourself, right? Because your brain is like a massive LLM engine. Your intuition, people talk a lot about product intuition, product sense. To me, that's bollocks. It's basically you put a lot of data in And then you let it, you know, simmer for a bit and good things will come out if you've been exposed to enough context and enough data. Your brain already is a great machine at doing stuff like that. That's where you'll get your best ideas from. Talk to as many customers as you can and so on and so forth. But like you said, the busy work that we do as PMs. A lot of PMs I talk to are very much trapped in the hamster wheel of having to focus on low leverage tasks, status updates, specific asks from specific stakeholders, having to defend their roadmap when they've already explained it 50 times, You know, all that stuff is taking time away from the stuff they should be doing, which is working with customers, finding problems, finding solutions, iterating on those, finding the right distribution models, testing those and all that stuff can also be helped with AI.

**Tanguy Crusson** (00:14:17)

But hopefully we get to a stage where for everyone, the busy work goes away. I can think of a few technological revolutions that were promising that, though, and people are still being people. So I don't know. I'm cautiously optimistic on that front.

**Aakash Gupta** (00:14:32)

Yeah, it's not a panacea. Before we go any further, guys, there is a wonderful screen share that Tangi does alongside the content you're about to listen to. And if you want to actually see the steps in action, be sure to check this out on YouTube or look at the video version of the podcast on Spotify to get even richer information. Now back to the episode. Can you walk us through, step-by-step, an ideal discovery process?

**Tanguy Crusson** (00:15:03)

Yeah, so ideal, no. But an example, definitely. And what I'll use is the example for how we do things in the JiraPoder discovery team. So it might be a bit meta how to do discovery to create JiraPoder discovery. But I think we're going to do fine. The quote-unquote process that we follow ourselves has four main... I'd call them stages. It looks like waterfall. It's not really waterfall. Things keep moving from one stage to the other based on what we learn. But generally speaking, whenever we tackle a new problem area, that's what we follow. When we created Jira product discovery, the product, the whole product, we followed stages in this process as well. So it applies for us at the macro level and it applies also at the micro level when we work on specific features. The reason we created this process was that it's very complicated to talk about the stages of things with everyone at Atlassian.

**Tanguy Crusson** (00:16:04)

So whenever we talk about an idea and this idea is super fuzzy, we're not even sure what problem area we're doing. We need to give it a name because people might assume it's further down the track otherwise. And maybe we'll come to them with a specific ask to help, depending on the stage. So, for example, if we are making something, we might come with an ask from a dependencies to help us build something. Versus if we're exploring solutions and we're just about to exit that stage, it means that we might be asking for funding and things like that, right? So we've kind of set those four stages as vocabulary across the whole of Atlassian, pretty much. Everyone knows at Atlassian what we're doing when we say we've got something in Wonder. So we've got wonder, explore, make and impact. Wonder is all about problem exploration. We're not exactly sure what we're doing but we've got a lot of customers currently that are talking about in their road mapping process how they should be working with dependencies and working with capacity and those things seem to be tied together for example.

**Tanguy Crusson** (00:17:11)

And so what we do is we get in and do about a dozen user interviews and to try and unpack that and to go with customers and try to understand how these things fit together. And the conversations will usually be about an hour long. And we do a few of them until we feel like, okay, the same themes are coming back and so on and so forth. Once we've got a good understanding of that, we go into solution explorations. And our goal here is not just to go into a room, create designs, and then only come out when the designs are finished. No, the goal is basically to quickly find ways to test stuff with users until they tell us, yes, this would actually solve my problem. I have a few examples of that. Then once we have enough validation that something is worth investing into that's when a team makes a pitch to go into make which is okay you know what we've got all the validation that we need here it's enough now we should really start working with a lot more customers so currently we've got 10 that are interested we'd like to get to 100 and progressively to a thousand for example and so that's what we call make which is we're committing to building something we've got enough validation we think for it And now it's really about making it happen.

**Tanguy Crusson** (00:18:22)

Maybe we just do a first version first. Maybe we'll do some more iterations later. So we try to shape that there. And there's a few iterations that go in make. And then impact is usually when the problem is translated into something that is in the product. And now we're measuring to see how well it performs. because it might be working well for a small number of users, but we need to make it work well with a super large number of users. And so we call that impact. There's usually a few months after we launch things, we sit down and we write down an impact page to go, this is actually how it's performing, we recommend just putting it on hold for now, it's doing fine, or doing one more iteration, or we actually need to have a roadmap over a longer period of time, to actually have it work to its full potential.

**Tanguy Crusson** (00:19:06)

What should we do? Should we retire it? Should we leave it to a small number of customers or should we invest more? So that's the process, problem, solution, building it for real and actually iterating on it until we've got, we hit the desired goals for it. So probably best that I go into, so that's Jira Product Discovery and that's our Jira Product Discovery project. So in there, we do everything from discussing feedback that we receive from customers, classifying them into, okay, those are big bets versus iterations on current experiences versus like small pebbles, which are tiny UX improvements that any engineer can come in and pick up whenever they've got some spare time and want to do something different. And it's also where we have our roadmaps, so going from the roadmap that we have at the highest level and that we share with our leadership, focused on bets and solutions, and then roadmaps from specific teams, for example, that would go more into solutions that ladder up to specific bets and specific iterations, right?

**Tanguy Crusson** (00:20:14)

So what we do in the job of the discovery team is we actually are on rotation, the PM team, to look at user feedback. So we have four PMs, meaning every week. There's one of us four that for the week looks at all the feedback and tags this feedback based on what we learned as insights to ideas. We discuss that every week altogether. I think next week is actually my turn. And then we sit down more or less every month to discuss, okay, so what's changed really, that means that we should revise, review our roadmaps. But let's assume that we have said, okay, you know what, that stuff came often enough, we need to look into it. What we do is we start a wonder stage, which is, let's look at, let's unpack the problem. So I've got here in product management jobs to be done, which is one of our bets.

**Tanguy Crusson** (00:21:08)

We help product operations teams and administration teams roll out JPD, job with discovery at scale. And it's part of the jobs to be done theme, where we focus on specific personas, PMs, product operations, administration. So in there, there's something called global fields. It was not called global fields before. It was a messy area, which was called global entities, which was we were finding, people kept talking to us about having many gyropodic discovery spaces, projects, and needing to be able to work with all of them at scale. And it was initially, we had discussed a bunch of solutions and we were like, you know what, it's super easy, AirMoss. Emma Sandunga, one of the product managers in Japan for the discovery. Why don't you go and actually figure out what that all means? And she went to run a wonder stage. And this is a typical outcome from a wonder stage, which is a page.

**Tanguy Crusson** (00:22:08)

that tries to find basically who we're trying to help and the types of problems that they face. So she had decided for this particular exploration to focus on specific personas, so product ops, program management, VPs, stakeholders, and PMs. And then what we do for all of them, what I ask the PMs is, all right, I don't care about big lengthy pages that explain to me how big a problem is. Instead, give me all up less than 10 minutes of videos of customers talking about their problems. And I want to see the different facets of it. So it has to be probably at least 10 customers. And they have to be talking about their problems in ways that makes us understand the different facets of these problems. And so that's what Hermos does really, really well. She starts and runs a little bit of research. It lasts for a couple of weeks.

**Tanguy Crusson** (00:23:03)

And she comes back with a page like this where you see there's one problem area here. There's a second problem area here. And there's a third one there. And then that's it. and literally we have a meeting with all the product managers and we watch this together silent reading and watching videos for 10 minutes and then we discuss and usually within half an hour after that we're like oh yeah yeah that sounds important or it needs a bit more exploration and whatnot but that's really for us what wonder means it doesn't have to be something which is a Like we've surveyed thousands of users, we've done this comprehensive, super scientific approach to all this. It's really no. Like we've got a few customers that have been voicing this. Let's go in there and understand how they're feeling that pain. And we bring that to the rest of the team so they understand where the pain comes from.

**Tanguy Crusson** (00:23:57)

So that for us is wonder. Any questions you'd have before we go into explore? It seems a

**Aakash Gupta** (00:24:02)

lot like ethnographic research where instead of just doing a large survey, you're trying to go really deep and add texture to the problem, really understand how does that affect their jobs to be done.

**Tanguy Crusson** (00:24:15)

Yeah, that's correct. And we try to do as much as we can in plain English, raw emotions for those users. It's like, okay, so, you know, Let's explain it to the team in the customer's own words how the pain is coming out, removing all the varnish there is around it. Let's try not to make it sound too smart. Let's try not to make it so compelling with a lot of superlative and objectives to describe it. Instead, let's just hear it from them. And what we found is people resonate a lot with that. They'll be convinced in an abstract sense by reading a page that's beautifully written and they'll be like, wow, that's smart. but it doesn't trigger the urgency and the need for action that watching a video from a customer does. And it's even better when we invite, for example, engineers with us on some of these conversations And the engineers hear it firsthand from the customers.

**Tanguy Crusson** (00:25:13)

The response from them is like, okay, there's an innovation week next week. I'm going to try a solution for that. And they really go all in. And that's exactly the energy that we want around these problems, right? So are there any

**Aakash Gupta** (00:25:26)

tips for how to conduct this conversation as a PM?

**Tanguy Crusson** (00:25:32)

Yeah. Honestly, if there's one investment you could make that would change your life as a PM is... find a real user researcher, someone who does that as a trade and ask them for training. I used to think I was amazing at user interviews. I was saying a lot of smart things and people would concur with a lot of them. And then I had a researcher, Georgie Bottomley, she was at Atlassian and she watched about 20 user interviews and she said, yeah, I know you're very proud of those 50 user interviews you did. Dude, I can tell you, you didn't learn a thing. You're leading all these conversations. You're pushing users in directions that they would not have taken on their own. So you're not really learning anything. And what she did is to basically give me a simple interview script with a lot of silence to follow, which is basically just, you know, ask them to introduce themselves, ask them to describe what they do in their company.

**Tanguy Crusson** (00:26:40)

And from then on, you don't have an interview script, you rebound on what they say, and you might be poke in one direction if they are going there, but you do not ask leading questions to take them somewhere. And so if you're trying to validate if product managers struggle with dealing with feedback, you don't never bring the word feedback in the conversation. Instead, you let them, you try to see if they go there. And if they go there, then you can start to poke. And the other feedback she gave me is never interrupt a user who is talking. So I took all her feedback on board and started doing more interviews and she's like, wow, I'm proud of you. Three minutes, you didn't say a thing. And there's a few other tips like this, like never give options. It might be uncomfortable, but if you ask someone, for example, what's the first thing that you do in the morning?

**Tanguy Crusson** (00:27:30)

We're humans, we're trying to make the other person feel comfortable. We're gonna give options. What's the first thing you do in the morning? Do you drink coffee? Do you have a shower? Do you brush your teeth? When you try to interview users and you're trying to learn from them, the way you'd ask that is, what's the first thing that you do in the morning? And you just sit on your hands and you just wait and there's an uncomfortable silence and it's just there with you. You feel like it's forever. and then they start talking, but the way they start talking is based on, it's from their perspective. You didn't give them options they can just latch onto and reply yes to, because they just want to please you by default. So things like this are just, Tips and tricks. I'm not trying to tell you that's exactly what would work for you.

**Tanguy Crusson** (00:28:18)

More like get training from a researcher. It will drastically change everything that you do afterwards. Otherwise, I can promise you that you are going to have many conversations and it's going to prove what you think is right.

<!-- sponsor -->
**Aakash Gupta** (00:28:30)

Trust isn't just earned, it's demanded. Whether you're a startup founder navigating your first audit or a seasoned professional scaling your GRC program, proving your commitment to security has never been more critical or more complex. That's where Vanta comes in. Businesses use Vanta to establish trust by automating compliance needs across over 35 frameworks like SOC 2 and ISO 27001. centralized security workflows, complete questionnaires up to five times faster, and proactively manage vendor risk. Vanta can help you start or scale your security program by connecting you with auditors and experts to conduct your audit and set up your security program quickly. Plus, with automation and AI throughout the platform, Vanta gives you time back so you can focus on building your company. Join over 9,000 global companies like Atlassian, Kuora, and Factory who use Vanta to manage risk and prove security in real time. For a limited time, my listeners get $1,000 off Vanta at Vanta.com slash Akash.

<!-- sponsor -->
**Aakash Gupta** (00:29:28)

That's V-A-N-T-A dot com slash A-A-K-A-S-H for $1,000 off. AI evals are one of the most important skills for PMs. And I know you know they matter. The question is, are you doing them right? Most teams are winging it with basic metrics and hoping for the best. Meanwhile, the teams that actually ship reliable AI, they've cracked the code on systematic evaluation. Today's episode is brought to you by the AI evals for engineers and PMs course by Hamil Hussain and Shreya Shankar. This live Maven course will teach you the battle-tested frameworks from Hamil and Shreya, who are the engineers behind GitHub Copilot's evaluation system and 25-plus production AI implementations. Four weeks, live instruction. Next cohort starts July 21st. Start shipping AI that actually works. Enroll at maven.com with my code ag-product-growth for over $800 off. That's ag-p-r-o-d-u-c-t-g-r-o-w-t-h. And this document seems really well written. What is the right way to sit down and put a document like this together?

**Tanguy Crusson** (00:30:44)

I think mostly like the way Hermos does it is the text doesn't matter. The only thing that matters is the videos. I barely glance at the text. I watch the videos and what she's doing is to find ways to tell a story by selecting snippets of in the video that progressively ladder up to give me the feeling that I've looked at this via all the different facets. She's got basically 10 minutes to summarize probably about 10 to 15 hours of conversations. And so typically what happens is it's a lot of the work that you do interviewing users and immediately after those conversations, like finding the highlights that you think like really took you to an aha moment. So I wouldn't focus so much time in the writing of the document. but a lot more time in making sure that as you go through the customer conversations, you take the moments that gave you this aha moment to see if you can reproduce that with the people you're going to share the video with, right?

**Tanguy Crusson** (00:31:45)

And making sure that it tells a story when you put all of them together is quite important. So you basically are taking people with you. By the end of reading these documents, I was telling Hermann, oh, okay, I see. You would like to build this. And she was like, yes. But it was so clear by watching this video. And it might be a trick to convince me, but she was convinced that it was the right thing to do after doing all these interviews. So that's why it should be a no-brainer to the people watching this. It should be really clear. There's a moment when you start those conversations where you just don't know It can last for a long time. You're navigating and you feel like you're going backwards some days, like some things you were thinking. Some customers went that way. Some customers went completely another way.

**Tanguy Crusson** (00:32:34)

That's completely normal. And my advice here for people is just embrace that messiness. It's fine. It's actually... those things that if you let it sit for a while, eventually you're going to see through. It's like if you take a bottle of water and you put sand in it and you shake everything. That's what we do when we do a lot of user interviews. And then you put it on the table and you wait. And eventually the sand will settle and you're going to see through. It's exactly the type of things that I ask the PMs, wait till you've hit that clarity. like you have another conversation and you're like, oh, I feel like I'm having the same conversation again. Good, that's the moment where you actually write this page. It should not take you more than two, three hours all up to write that page, basically, because you're already clear.

**Aakash Gupta** (00:33:23)

So you stop the interviews once you're converging on insights, once that sand is starting to settle. And I think one thing that might get in people's way is just the tools itself, because they'll say, I've never clipped a video and put a video together, several clips together. How do you guys do that?

**Tanguy Crusson** (00:33:41)

Oh, it's really simple these days. I don't know how many tools there is out there. For us, we've tried many. We use Loom for putting them together and we also use Dovetail. So Dovetail is where a lot of our, most of our user interviews go and then it creates a transcript and then we can query it for, you know, We can query transcript for specific themes, but also we can create snippets and then we put them in what I think they call that an insight, which would have a bunch of video reels put one after the other. My advice to every PM as well is to, when you join a team and there's no, people don't talk to customers a lot. and they don't know how to do stuff like that, your first job is to put that in place, right? So the finding, like recruiting, identifying, recruiting, setting time with customers, extracting, like running the interviews, extracting video clips from it should be something that takes you no thinking whatsoever.

**Tanguy Crusson** (00:34:49)

So for us, for example, I go in Pendo, I run a little segment. I know which customer I'd like to talk to for specific behaviors, if it's data related about a specific feature. If not, I will go into Dovetail or I would go into our Jira Service Management Cube where we'll receive more feedback. I'd run a little query and within a few minutes, I've got a few names of people I can talk to. I also have tooling to be able to send them emails with a quick intro that's as little fluff as possible. Hey, you've been using JiraPoder Discovery a lot lately. I'm part of the team, would love to chat about how we can make it better for you. That kind of stuff, make it human, simple, two-liners tops with a Calendly link. They click on it, they book time. It's connected with my calendar.

**Tanguy Crusson** (00:35:34)

I don't have to send three options. They reply, we reply. No, that stuff is gone. Then whenever I join this meeting, I know that it's going to go to Dovetail. I've got my recorder coming with me on the call as well. So I know it's all going to be recorded so I can extract snippets after the call. All that stuff, all that mechanics is really something that you should put in place because As a PM, AI or no AI, you're going to beat every other competitor if you learn faster than them and if you know more about your customers. And it's worth a lot, like 10 times more than any automatic insights you can get from any model today. which, and so use the AI to get you in the right conversations is the way I would say it. Use the AI to extract snippets from videos, watch as many of them as you can.

**Tanguy Crusson** (00:36:29)

So for example, sometimes I go in Gong and say, I mentioned you're up with the discovery, say premium because we just launched it. And I see where it's mentioned and boom, I watch all the video clips, that kind of stuff, right? That's a lot, that's what will give you an unfair advantage because you're gonna keep learning and it's gonna keep giving you perspectives that you didn't have. So that's, that tooling really important. And so for us, we've got DovTay here, we've got a community group where users can come in and they can ask questions. We receive maybe 10 questions a day here sometimes. And they ask questions, like it can be as simple as something like this, where like someone was saying, oh, there's a bug. I used to be able to filter on this and I can't. And I just took an example, it happened yesterday.

**Tanguy Crusson** (00:37:17)

And today I was like, oh shit, yes, we're looking into it. And then a few hours later, okay, we fixed it for you. That kind of stuff gets users engaged and then they come back, they ask more questions. So that we can then let them know when, for example, we're experimenting with new features. So I, for example, posted this feature, which is now part of the JRPOD Discovery premium plan, but basically it started just with the Loom, where I was like, hey, we're thinking of this, what do you think? And so you can see here, there was like 2000 views on it, lots of comments and reactions, and even at the bottom of the post, like either excitement or questions, I've got four pages of comments for it. Right? So we use it for that, for answering people's questions, for addressing their bugs. So it's quite useful at the scale that we're at, which is 18,000 customers today.

**Tanguy Crusson** (00:38:12)

We still are able to stay on top of that with a PM team of four with a weekly rotation. We do have Pendo where we basically can in-app ask questions to users. We use that for CSAT, but we also use that for things like we're looking at option A versus B. What do you think? And sometimes it can help settle an argument. We get like, I don't know, 100 answers and we're like, eh, see? And we look at that, but we often look at the commentary. We always ask them like, tell us more. And they give us commentary. So whenever we hesitate between two things, we just ask and then we get something back. That's pretty useful. Needs that. need to implement this tooling, but once you have it, it's really amazing. We do talk with customers in Slack. So I've got probably about 20 customers that I'm I have on speed dial.

**Tanguy Crusson** (00:39:05)

So they're all in this folder right here, which is collapsed. And Medibank is one example. You can see here, 5th of May, it's like what, two weeks ago. They had an issue using JavaScript discovery with Miro. With a new feature we built, we helped them with that. And since then there's been other questions, answers, questions, answers, and then stuff that we asked them to do as well sometimes. So basically as close to the ground as possible is what I would recommend for things like this. And we've got this thing where, so you arrange your product discovery and you might have feedback for us. You click that, you just give us your feedback. This feedback goes into Azure Service Management Queue and we can triage all this and we tag the new things that we haven't thought about to ideas as insights. And we can also use rovo here to give us like, okay, so in the last six months for the people say, which is a way to use the AI to help us like look at things at the macro level sometimes.

**Tanguy Crusson** (00:40:03)

Anytime I start in the new team, that's the first thing we set up, which is all these touch points to make it so customers just literally have to pick up the phone and they can talk to us. Every PM that first joins the team say, it's never going to scale. And I'm like, I don't care because we're meant to be swamped with this stuff. That's what will make us think. Not if we're comfortable and we have little summaries that our research team gives us and it's all very well organized and we should do just A and B and C. It doesn't work like that. What we know is we ship products, there's existing features, but they also want new things. And there's also reliability things we need to worry about. And there's some customer segments it works for them, some it doesn't. Some would care about specific details, others just don't care.

**Tanguy Crusson** (00:40:54)

And it's just like this diversity and this is how I progressively get an understanding of what our users need. The reason I can say I think I've got some credibility in talking about this is as we scale from zero to 18,000 customers, our CSAT has stayed at above 85 the whole way. And that's really hard to reach a score like this. It's the first time in my career I actually get that. And that's where a lot of our growth comes from too.

**Aakash Gupta** (00:41:24)

I think just implementing this system will be a revolutionary way to work for 75% of people listening, but I cannot vouch for this more. It's about seeping the customer knowledge into your own LLM brain, right? And this is how you do it. You're getting as close to the feedback as possible.

**Tanguy Crusson** (00:41:45)

Yeah, and always try to frame it from the lens of the customer with their own words and vocabulary and so on and so forth, which actually takes me, we've been spending a lot of time in that first stage, wonder. Explore. Explore, how do people, how do I see a lot of our customers do this? Often for the less mature PM teams, what happens is a long process of designing the solution, followed by a spec, followed by a long process of building it. And in that long process of building it, they use Sprint. And yes, that makes sense. But Agile was actually meant to cover both of these things together, which is you actually iterate on the solution and you iterate on making it at the same time. And you might be uncomfortable for a super long time as this thing is shaping up. And that's exactly what it's meant to help you achieve.

**Tanguy Crusson** (00:42:48)

But let's start with Explore. So what do we mean by prototypes? and validation here. So what I ask the PMs is create, like you can work on prototypes, expose them to the, you know, you've got 10 customers here in your wonder page, great. Get the same 10 people in a video after you've presented your solutions and get them to explain how that's solving it for them. That's what I want for you to be able to exit Explore with enough confidence that we should invest a lot in it. So it's basically Hermos going back with his customers, iterating on potential solutions. And then she's like, you know what? We're really onto something here. Here's the proof. And it can be things that are very lo-fi and simple. For example, I'm going to zoom back to five years ago, we were exploring concepts for what turned out to be JiraPoder Discovery.

**Tanguy Crusson** (00:43:42)

And the first prototype we put in front of users was actually that one. which is nothing more but a slide. And because we were hearing them talk about all these problems and we were like, there's a lot there, like PMs are having a tough time. What should we help with? And so we tried. I don't know, countless iterations of that slide where we had different pillars, we put them in different orders. This was probably the last one where everything we realized was centered on prioritization and everything else was in service of it. But there were key components we needed to get right that integrate well with it. But what we did is we would create a slide like this and we would join a call with a PM who would explain their life and what they were struggling with and then we'd show that slide and go, so what do you think?

**Tanguy Crusson** (00:44:40)

This is a solution we're building, how would it help you? And we'd get them to engage with this and give us feedback, oh, that's interesting because this bit is... This bit is quite important for us, but really the stuff I'm struggling with is that, for example, which is where we landed in a lot of conversations. And we found a lot of users to work with there who were able to very crisply define what their problems were. And so one of them, Brent, which is one of our Lighthouse customers, we can come back to that later, was saying, you know, this is really what it boils down to. I work in a sales driven organization and I need to get people rallied behind my priorities. And it's really hard, but I really enjoy when we get to the end of this process and this clarity into what we're building for everyone.

**Tanguy Crusson** (00:45:30)

It's really joyful when we get there. And we're like, you know what? We want to help Brent. And Brent validated this one. And then we found other customers and eventually we narrowed down on that. But that was the prototype. That was the first one. So we're like, okay, cool. We need to focus on prioritization. How are we going to help them focus on prioritization? Initially, we were like, you know what? We need to help them with prioritization because they're struggling with working with all these other teams. So we're going to give them a place where they can have all the feedback going in and they can prioritize this feedback. And look, it looks like Gmail, I guess. It's basically an inbox of feedback. We presented that to a few customers. So this one was probably a week spent in Figma discussing potential options. And then we presented that to users and they were like, oh yeah, that's interesting.

**Tanguy Crusson** (00:46:19)

Yeah, I could use something like that. Brent was saying the same stuff. And I was like, that's not quite the response I was expecting. Okay. We explored a few other concepts. We went back to Brent and we presented that. Again, very simple. It's just like capture, prioritize, deliver, which are the pillars we described in the slide. And then we were centering on ideas here with uh lettering up to goals user impact strategic value and with a some kind of of a priority score we presented that to brent and a bunch of other users and they were like when can i get this i'm struggling right now i've got this conversation coming up with my cpo we're trying to present our roadmap the cpo keeps arguing for us to build a particular feature we keep thinking we need them to step up Focus on goals, let us do the work of defining what should be in the product.

**Tanguy Crusson** (00:47:12)

I need this. That's when we knew we were onto something. We didn't write a single line of code there. The main reason is there's no technical complexity in building something like this in Jira. We've got all the assets that we need there. So it was basically one PM, two PMs, one designer. We were iterating on this concept. We built a full prototype at some point and we validated a lot of stuff this way. That was before we wrote a single line of code. Today, the way we do this is we're going lovable. We upload a screenshot from Figma and we turn it into a prototype and then we get users in course playing with it. Trying to make it lo-fi still in... in Lovable because we still want people to understand it's not a final product and get them to think. But basically that is the step which for me is super important, which is not jumping straight into building, thinking that you can validate by getting your customers to use something.

**Tanguy Crusson** (00:48:13)

Because by the time you get there, you're months later and you haven't learned anything and you might be wrong. And it happened to us a few times to be wrong. So that's Explore for us, which is really focusing on this and not going all in until we've got enough validation from customers, from their mouth, that it solves the problems they've stated before. It's a bit unnerving for the new product managers who joined the JiraPoder discovery team because they, like we all like to take shortcuts and it's fine to do it on something small, but not with something is big. And so some initially think it's a waste of time to do all this, but then they realize actually that they don't waste as many cycles on things that in the end are not used by anyone.

**Aakash Gupta** (00:48:59)

Love it.

**Tanguy Crusson** (00:49:02)

So that's the explore phase. I mean, this one, you'd know what it is, right? You'll know what you're building, so you're making it. And this one is about measuring impact. But there's one key thing about this make bit here, which is that one. It's a slide I found from a Reforge course. And it's about the growth funnel versus the safety funnel. That was a key way for us, again, to make sure that we don't go too far ahead of ourselves too early. So whenever we've got a concept, let's say the concept is the one I was showing just before for the prioritization. We don't immediately give it to thousands of customers saying, that's it, go and try. It might not fit their environment and we don't know yet. It might not be ready for them. If it's an early product, maybe they want more compliance controls and like enterprise controls and so on and so forth.

**Tanguy Crusson** (00:49:59)

The problem is if we get them something which is not good, they're going to come once, they're going to have a look at it, and then they're going to be like, it's not for me, move on, and it's going to be an uphill battle to win them back. So instead, I'd rather think of it as a queue in front of the nightclub, right? And we let people in, as we know they're going to have a good time, not before. That's what in this slide they talked about as the safety funnel. You minimize the number of people who have a bad experience. And then once you know, you know what? All the users that we have on this solution, now they're really enjoying it. CSAT is really high and so on and so forth. Let's lift the limit. Let's let everyone in. Everyone thought initially in Japan, the discovery was way too conservative when we were doing this because we said we would work with 10 customers, then a hundred, and then progressively with a thousand.

**Tanguy Crusson** (00:50:50)

But that really worked for us. By the time we lifted that, we went from 1000 companies playing with it, not paying to 18,000 paying for it, uh, in less than, uh, two years. Right. So that's, that recipe works. The only reasons I'm giving these stats is like, it works. Trust me. Like there's, there's really something to play with here. Uh, Yeah, so that's basically one key thing for when you're between wonder and make, which is be patient, get it right, and then progressively stuff. I know that's a lot of, we watch some of these companies that manage to grow extremely fast, extremely quickly. At the moment, I'm thinking of the lovables like VZERO, bolts of this world. Most businesses are not like that. And it's easier to crash and burn by taking this approach than by being a little bit more methodical in making sure that your users will only get the thing when it's ready for them and they're going to have a good time with it and they're going to want to take out their credit card.

**Tanguy Crusson** (00:51:56)

And we could have said, you know what, we've already got competitors in this space and so we have to go fast. The thing is, like one of those competitors at 6,000 customers when we started, we went triple in two years. So it's like the growth can hockey stick from there. It's just that the product needs to be ready at that point. So as long as you're able to buy the time to get there, right, you should absolutely do it from my perspective.

**Aakash Gupta** (00:52:24)

So is the advice to quickly release things to the market and get feedback from the market a little bit overrated?

**Tanguy Crusson** (00:52:32)

I'm not sure. So it's every question in PM is always, it depends, the answer, right? I know enough now to know that I don't know a lot, but basically you should try to answer the most important questions. What was the most important question when we started your product discovery? It was not, can we get this the right solution? Because we had answered it with this with a small number of customers. So we didn't need so much to validate that. but it was more, will people buy it if we have it? So what we did is instead of releasing it and having them buy it, is we started with things like this, which is from one day to the next on the Atlassian website, there was an ad for dear product managers, your job is hard because of various reasons. Are you proud to ship? We'd like to help you join us on the journey, put your email.

**Tanguy Crusson** (00:53:35)

And so for us, it was even without talking about particular solutions was that do people connect with this? And is there enough PMs who actually care? Can we reach them? Can we potentially sell things to them? Within two weeks, we had 3000 companies who had put their email down on it. And we did some scrubbing from what we had in Salesforce, what we had in our customer base, licensing and so on and so forth. And we were like, whoa, Okay, there is something there. That gave us two things. One is validation that Yes, there is a there there and people connect with the thing that they connect with the problems. We had after those 3000 emails, we had 50 user interviews from there and people really confirmed all of that. So we're like, okay, there's a real thing. There's a real problem. And then it's just about, okay, so it looks like we have to like, we can reach these people and these people connect with the problems.

**Tanguy Crusson** (00:54:32)

We just need to get them the right solution. So then our, you know, our focus is doing the right solution, working on it up until we can give it to those companies right there, which we had segmented into early adopters, not early adopters, enterprise SMB, all of that stuff. We did the homework there. But basically from there, what we did is progressively give it to more customers based on their appetite to try early stage stuff. So I wouldn't say you should completely ignore that part, which is get it out there, because distribution is probably the hardest nut to crack. But you need to make sure people don't land with something that's not ready for them, because winning them back is going to be much harder than waiting until you give it to them. So for us, this playbook works because we built a product by cross-flowing from an existing one So it really depends as well on your distribution potential and so on and so forth.

**Tanguy Crusson** (00:55:31)

If I was starting in a startup right now and I had zero customers, I'd probably be talking to the world about it, but I'd still have a wait list. because I'd want to drum up interest into a waitlist and then progressively take people off the waitlist bit by bit to get the right references and then to get to prove that we've solved the right problems, get the right quotes, get the right messaging validated and progressively get something that I can launch and open to everyone.

**Aakash Gupta** (00:56:00)

And is there any risk when people are using the product for free that you're not going to get the right type of feedback? Sometimes people bring that up if they're only if they're paying, are you going to get the right type?

**Tanguy Crusson** (00:56:13)

Yeah, we really like this one was the biggest gamble we made in JPD. At some point, I was uncomfortable with how far we went without having people having to take out the credit card. It probably depends on which market you're playing in. For us, teams had to invest a lot of time to configure their processes and their workflows in the product. There's no JiraPoder Discovery project that looks the same. This is the way we do things in the JiraPoder Discovery team, which is very different to how Medibank does things and to many of our other customers. So the fact that they had to spend that time, and then what we realized is that more product managers were active like 30%, I think, of product managers were active every month, were also active every day in the product. So we were getting, like, they were basically putting a lot of time in there.

**Tanguy Crusson** (00:57:06)

We were also tracking, like, how much time do they spend? What are the actions that they're performing? And we were doing regular conversations with them to understand the value that we're getting from it. Where it was like, well, you know what? If they have to stop using this, once we make it paid, it's gonna be a major pain. But it was still an assumption. And to validate this assumption, we did content surveys and we did a whole bunch of research. We've got a strategy and business operations team focusing on that. We validated, no, no, you really have basically people willing to pay here. But for me, I was very uneasy up until I actually saw people taking out the credit card, which is why when I first tried, I think the first one I tried was like Bolt. And I had to, I put five prompts and the sixth one, I had to give my credit card.

**Tanguy Crusson** (00:57:53)

I was like, yeah, that's pretty good. Would I pay 20 bucks for that? Yeah, okay, I want to continue. I was a bit worried for them in that, yeah, I'm putting my credit card now, but I'm probably going to cancel because I don't have an immediate project to use it. So their churn is probably going to be something and so on. But anyway, it really depends on what market you're playing in and the dynamics for how people adopt your tool. For us in the collaboration space, it's mainly B2B and people have to really put effort into adopting the tool. It's not cheap, it's not free. Once you adopt it, it gives a lot of value, but removing it is harder. We're in a special circumstance. If I was working on a B2C app, I would probably not do this like that. It's always, any question is back to first principles, like what's your biggest risk?

**Tanguy Crusson** (00:58:43)

And how do you validate that your gut feel is right?

**Aakash Gupta** (00:58:48)

And here, I think the key insight is if you're in a market where people are investing a lot of time to change their processes, that already is a significant investment. That kind of mirrors pulling out your credit card in a B2C environment.

**Tanguy Crusson** (00:59:03)

It depends also. Yeah, you're completely right. That one is like there's a certain resistance to change. So it's really hard to get people to change their way of working. I mean, how many apps do you use every day if you introduce a new one? Like, it's painful to have to change stuff, right? But also, like, how critical is the process that you're tapping with? So it might be that people have spent time and they use it often, but it's not that critical. If it's not that critical, then, you know, the churn, like, they might not end the pain. If they really sped it out to you how hard their life was before and you solved it, It also validates that they have the budget because they might also be in a team that doesn't have the budget to pay for stuff like that. So once you put all this stuff together, you should be able to have a better answer for how do I, like when do I ask people to pay?

**Tanguy Crusson** (00:59:59)

It's never as simple as do it early or do it late. It really depends on the special circumstances of where you play.

**Aakash Gupta** (01:00:06)

Makes sense. One of the things you said at the beginning was it's not just about discovery, then delivery. How do you infuse this process into the make and impact stages?

**Tanguy Crusson** (01:00:20)

Yeah, so for whenever we enter make, What we basically have is kind of a prototype that has validation with customers. Sometimes we wrote what we call a technical spike, which would prove whether we can actually technically do it. So we did it recently, for example, for this feature right here where we can have ideas that are of different types and these ideas can be connected to other things like solutions iterations, customers, those kinds of stuff, and then visualize those in views that make it look like a hierarchy or where you can see what are the iterations for something or what customers ask for this particular solution, that kind of stuff. We're not quite sure whether that would work technically, so as part of Explore, we actually had a team who for two weeks tried to spike it, meaning go in the code, try to make it work, and anytime they hit a roadblock, just document it somewhere saying we need to solve this, we need to solve that, to get some understanding as to the technical complexity for what we want to solve, and then inform how much how much appetite we've got to actually build it based on that, right?

**Tanguy Crusson** (01:01:39)

But when we exit explore, we go into make and basically the start of make is always, okay, so how quickly can we get something in the hands of customers? And so what we tend to do is we usually reset the design. So whatever we show to customers then we reset and we start iterating again on solutions, this time with engineers. designers and PMs in the same room, right? And so, you know, like, for example, you see, if you, when we start make, like you, every Figma design that we've got in the team, you have a tangy tab or a few tangy tabs where I take something from the designer and I refund it based on conversations we had with the designer, with the engineers, and we basically go through this daily, but here we land somewhere where we're like, okay, cool. Now that's the target. Now, what would a version zero look like?

**Tanguy Crusson** (01:02:30)

And then we go into that and we strip everything away to get to what's the minimum we could give to 10 customers for it. And so we iterate on that with the engineers, with the designers. And from there, we usually get to a stage where we have something like this, which is, okay, so based on this, it looks like we've got, for this feature, we've got to do these three things. And then we've got three parallel streams of work that can converge back to milestone zero or milestone 0.5, which is every time I tell them, I don't care, just tell me whenever I can start playing with it myself. And then one we can give to Atlassians and then one we can give to customers. And we keep iterating on that weekly, right? So weekly we have a demo and then we look at it ourselves and we see how far we've progressed and we discuss what can we catch or what can we add to make something, like to give something, usually we give it three months maximum for a very meaty feature.

**Tanguy Crusson** (01:03:32)

What would it take to get there? And so the scope has this tendency to expand and contract and expand and contract as we go through it. The more we understand something, the more the scope expands. And then after we feel like we understand everything, we cut things back up until we get to something minimal. And so it's a bit of a process of shaping. I think there's this methodology as well. I love the name ShapeUp, created by Basecamp, I believe.

**Aakash Gupta** (01:04:00)

Yes.

**Tanguy Crusson** (01:04:01)

And for us, that's really the process of we don't just shape a feature that we design. The design was here to inform where we want to get to. but then we pair it back 50 clicks into what we're going to ship first. And we go through whiteboards like this to discuss how we're going to do it. And we spend all our time in Figma. There's lots of comments there and whatnot. We have this thing called a live feature document where we define our V0s. So as we go through it, we're like, okay, so what are the key flows we want to work and where are they currently? And as we discover more stuff, we add more lines here. And then as we progress, we're like, you know what? This stuff can go to later. And so we keep doing this. We don't do this in Jira.

**Tanguy Crusson** (01:04:44)

We do this as the whole team, product manager, designer, and engineers. And it's a living document that we update weekly. Like at the very beginning, it's like almost every day. And then it's like once a week. And then at some point, we've got a first version that we can give to users. So we give it to 10 users. work with them and sometimes it can take a while. And then eventually we get to the stage where we want to invite more. But what's quite important here is to have the right tooling to be able to reiterate fast. So let me see if I've got this here. Okay, so there's, I do have here a shortcut for all the branches in Bitbucket where we write code and anything that starts with poll, is Polaris for JiraPoder Discovery. And in there, we've got all the stuff that the team is currently working on.

**Tanguy Crusson** (01:05:39)

So you see all our branches and some branches were dated 30 minutes ago and some were like a couple of hours ago, some were yesterday and whatnot, right? That's what we're currently working on. The worst thing that could happen is that as a PM, I can only work with that when the team is done. So instead is I tell them, whenever you create a branch, just, and there's something for me to look at, just send me a branch. it might be a micro change we change the button we change an interaction and whatnot but i can go in jira for the discovery i can open that uh chrome extension and i can for example oh yeah that one was pretty cool so i can reload jira for the discovery with that bridge so it's not on master it's not something that's integrated into our test environment.

**Tanguy Crusson** (01:06:28)

So like, I mean, it's not ready. It's not in the pipeline to go to production. It's just a branch. It might be throw away, but that's how we can test a lot of stuff. And so this one, for example, was, hey, what would it look like if we had whiteboards in Jira for the discovery, which we don't yet, but we were like, all right, let's integrate whiteboards from Confluence. And now I'm actually in a branch. and I can work with my ideas here in whiteboards and drag and drop them and stuff like that. That was a concept that was built in three days by one of our engineers in an innovation week by using the components we've got internally like whiteboards and confluence. But that tooling, you see here, the thing is purple. It means that there's a branch active and it's that branch is what we use to iterate fast internally as we test this.

**Tanguy Crusson** (01:07:17)

And then eventually we're like, you know what? We're getting close. We should be giving it to 10 customers. And usually we're about halfway. Because then there's like the polishing and the making sure that, okay, have we thought about how it's going to impact this part of the code, that part of the code? Do we have minimum test coverage at least to make sure that we're not breaking important things? We're building a complex app. It looks simple, but it's pretty complex in the in the backend. And so that's the kind of stuff that we do. So when we're 80% done, we're about halfway through. We polish that, we give it to 10 customers. And then we keep iterating from there. And we're with them on Slack. We get into Zoom calls with them. We look at their feedback. We keep addressing it. And at some point, we're like, it looks like it's good enough.

**Tanguy Crusson** (01:08:12)

We'll make it available to 100 customers. and the cycle repeats and then eventually we give it to everyone. But in between, we make sure that whatever we thought would happen actually happens or we learn from it and we change the app. So that's, in a nutshell, basically how we work with, during the make phase, to make it so that it's not just, here's a spec, build it, ship it, but instead we keep iterating and we keep infusing user feedback into what we did. So it's, We love to get something to customers in one month. Now we're at the stage where it's more like three months before we get something, but the feature might take six plus months to be fully ready. But as early as possible, we're trying to get users to actually play with this. It seems like you're

**Aakash Gupta** (01:09:02)

very, very focused on craft and high quality product where a lot of product environments that I've worked in and a lot of product managers I talked to, you know, some executive comes up with a feature and they want to see it in production the next day. How do you handle those communications and set the right expectations?

**Tanguy Crusson** (01:09:23)

Yeah, okay, that is super familiar, and that is a topic for discussions with our customers that comes up super frequently, as you can imagine. At some point in my career, I realized it's not because my stakeholders are higher in the org chart that they know more about the problems I'm working on. They have different, they're looking at things from a different strategic layer. But if I'm working on a product, I have the biggest subject matter expertise there. And so I have to be able to represent that. And what I have to be able to do is to manage their expectation, to do the things that we believe in the team are right based on everything that we've learned. And so a lot of what I focus on whenever, for example, I've got a new manager, which happened actually just a couple of months ago after a reorg in Atlassian, is I spend the first few months really trying to set the tone for the conversation, and explain, like basically get to a moment where the leader trusts what we do so much that they are trying to help instead of jumping in and suggesting stuff.

**Tanguy Crusson** (01:10:53)

Because there's nothing that is more demoralizing to a product team than if a stakeholder comes in and says, yeah, your ideas are nice, but I want you to build that. Often the stakeholder really, like they don't, know that they should not be doing that. They really believe that they're doing the right thing. At least if you work in one of those environments, which I wouldn't work in any other. And so it's really on, I think it's really on me to start by as politely as possible, say no to everything and then progressively explain what I'm saying yes to and give them the sense for where we're going and how fast we're going there. So this concept that works pretty well, which is to find ways to give bite-sized information that gives this sense of velocity that makes you look like a fast moving train. And this train goes really, really, really fast.

**Tanguy Crusson** (01:11:48)

It's a French train, the TGV, like a train a grande vitesse, high speed train. No one will fuck with a high speed train. They're not going to get in front of it. They're not going to get under it. They're not going to jump in it when it's running full steam. They let it go and they go, let us know when you need something. That's where I want to get to. So what do I do? Every week, we send at Atlassian all of us bite-sized updates onto the things that we're working on. I use this moment to basically highlight key learnings that we've got and everything that shows that we are progressing. It might be a user snippet of a user interview. It might be a demo for a feature that we just recently started and we've already got something to show for. It might be a chart focusing on one key part of the onboarding funnel.

**Tanguy Crusson** (01:12:37)

And so what I do is I keep sending those every week and I've been doing this for as long as I've been working on your app or the discovery. So you probably have around 250 of these updates somewhere where we send these updates and people are following those and they receive a digest every morning that shows them that. So I do that. Then there's a monthly explanation as to remember our top strategies and how we're going after them and see how we're progressing towards each of them. When we get wins, I make sure to communicate them. When we get not wins, so losses or something that's not working quite right, I also share it. So basically I try to make it so that the stakeholders can progressively get a picture for where we're trying to go and all the things that we're doing to get there, to really get the sense of, wow, they really know what they're doing, I should not interfere.

**Tanguy Crusson** (01:13:33)

And so I don't know, like for our customers, every company is different, but I don't know a single recipe that works other than frequent bite-sized comms that focus on the story that you want to tell to be able to continue investing in the things you believe are important. When we were in the super early stages of the JPD, it was all snippets of user interviews. Yes, you'd like us to build that. Please listen to this customer for like, one minute explaining their problem you still think we should be doing that that kind of stuff and then later on we progressively became uh much more comprehensive in terms of the metrics we look at and share and so on and so forth but i see it as my job as the head of product to basically shield the job or the discovery team from the rest of atlassian not because atlassian is a bad place but because atlassian might not be like acutely aware of based on the stage that we're in as a new product, what it is that we need to do at our stage to be able to be successful.

**Tanguy Crusson** (01:14:36)

And so that's basically my role and it's mainly via comms and sharing super frequently.

**Aakash Gupta** (01:14:41)

I think that the basis of that, building that trust in those comms, is making sure that you are the subject matter expert. A lot of people really struggle with that because there might be a founder or somebody who's been there eight years longer. There might be a customer success person who spends even more time talking to customers or a salesperson who thinks that they talked even more time to potential customers. It goes back to the very beginning of that wander and explore phase where you are the one who has done those 10 interviews on that specific problem area, and you have those video proof to back it up.

**Tanguy Crusson** (01:15:22)

Yeah, that is correct. It only gets easier with time because people, you know, you promise something, you deliver it. You promise something, you deliver it. You said no to something, but you said yes to something more important. and people can see the results. Like the winds compound and eventually people pretty much leave you alone, which is what happened for us. But it means that initially you need to do a lot of education based on everything that you learned. You can't just say no, you need to educate. There are a few recipes that can help you. Fair. The one that's been the most successful for us when it became really tricky with stakeholders was to play a little $10 game, which is okay. You're the leader of this area. I mean, we're one of the 10 things that you manage. You think we should be building X.

**Tanguy Crusson** (01:16:17)

What we're going to do is we're going to explain the things that we currently have on the roadmap. And you're going to put your stuff in there as well. And we're going to play a $10 game. I want you to spread this $10 across all the initiatives that you've got there to tell us how much we should invest in each. And you're basically forcing them to think through your lens as a PM where you have to worry about everything, always, all the time and forever. And currently they wake up and they have maybe an idea for a new thing and they're really excited about it. And then they need to think, okay, how important is it compared to all these other stuff. So if you frame the exercise correctly, where first you do a little session where you go through the data, you go through user interviews, you go through the strategic thinking and the rationale with them, and then you let it sit for a few days, and then you do a $10 game, it's very rare that they're gonna come back with, I want you to spend $10 in this.

**Tanguy Crusson** (01:17:17)

in this new idea I've got. They're most likely going to be like, well, okay, so is there any way you could do that part faster and maybe describe some of these because of, like you're gonna get into actual conversations around why are you doing the things that you're doing, which ones are important, are they right sized? And that's probably why you want their input as opposed to, I want you to build X. So make it your job to turn your stakeholders into servant leaders, basically.

**Aakash Gupta** (01:17:46)

And then the other obstacle that I think PMs constantly find in their way of this way of working, even if they know it's the right way of working, is they feel this pressure. Oh, we have a 1 to 12 PM to engineer ratio at this company, and I need to keep the engineers busy. How do you handle that?

**Tanguy Crusson** (01:18:08)

Oh yeah, that's a topic that... You've got really good questions, mate. This one comes up so often, even inside Atlassian. A new team is formed, there's a product manager there, there's a designer, there's seven engineers, and they're like, go. And the PM is like, but I'm new. I need to keep the engineers busy. And I'm like, no, you don't. That's not your job. Your job is to make sure they're focused on the right thing to actually make an impact. What do you know today? And what are the questions you all need to answer? And usually the PM comes back with, yeah, but my engineering manager tells me they need a roadmap. I'm like, cool, have them write spikes, technical. You know, you do little technical prototypes that prove, that try to tease out solution A versus solution B. What about this technology we plan to use?

**Tanguy Crusson** (01:19:01)

Right now, any team out there, if you're like, I don't know what my engineer should do, I'd be like, just write a spike on AI stuff. See how it could improve your product. Like that's not... That's not time that's going to be wasted because this technology is coming and it's going to evolve super quickly and you need to get started as early as you can to see how it's going to impact your product. But basically, you're trying to bring the engineers with you in all this. While they write these technical spikes, you actually talk to customers. When you talk to customers, you invite some of them. There's a rotation in the engineering team. Some of them join you like, for example, one in each call or something like this. They get a bit of understanding for all this. You have two hour blocks, three times a week, where you start on potential solutions, which will again inform more spikes.

**Tanguy Crusson** (01:19:49)

and they will work with the designer and they will work with you. And eventually you'll build this collective brain into what the problem is, what the potential solutions are, and you'll start to speak the same language and you'll start to build some shared understanding on the priorities as well and the sequencing and what are the quick wins we could get versus what are longer-term bets. And so my advice there is always bring them with you on the journey and get them to trust that the process is going to work for them. The engineers naturally, when they start, I find, will ask for clarity when you don't have it. And I think the worst thing you can do is to pretend you have it and send them down the wrong path because then you're going to break that trust. Instead, whenever I start with a new engineering team, I explain to them it's going to be messy.

**Tanguy Crusson** (01:20:44)

For about a month, you're gonna be like, what the fuck are we doing? But after a while, you're gonna understand the customers as well as I do for this problem area. You can understand all the different solution paths that we're exploring, and you're gonna be able to then come and propose alternate solutions and so on and so forth. And all of them do. And I remember Kostya on my team, engineer, he works in a squad I work with currently, and when he joined, he was like, dude, I need a one pager. I need a PRD. I need a spec. What the fuck are you doing? You're the PM. You're supposed to give me a spec. I'm freaking out here. And he was very emotional about all this. And I was like, dude, you need to relax, right? You're not going to be judged. based on what's happening right now.

**Tanguy Crusson** (01:21:33)

We are literally storming and norming that we need to do all this. And you'll see that the solutions we're gonna come up with are going to be better because you're going to be part of them. And you'll see that after all this, after we do that a couple of times, you're not going to ask for PRDs anymore. I haven't written a PRD in five years.

**Aakash Gupta** (01:21:50)

Wow.

**Tanguy Crusson** (01:21:51)

And that's exactly what happened. We work on Figma. We have these little documents I showed, like the live feature document. Everything is basically oral tradition. We talk about it a lot and we get on the same page. and we spar, we ideate on solutions together, and we critique each other's solution. And now Kostya would be the engineer who comes back and says, you know what, that feature you're designing, I don't think it's going to work like that. I think we should approach it more like that from a different way of approaching the UX, for example. And Ketelin, the designer, and I would be like, oh, you know what, I think you're right. And then we would, you know, continue the conversation from there. And that's... so much more efficient and so much faster than to try and keep the engineers busy while you're still trying to figure things out.

**Tanguy Crusson** (01:22:40)

Bring them with you on the journey. You don't have clarity, they don't have clarity. We're in the same boat.

**Aakash Gupta** (01:22:46)

I wish I had talked to you 10 years ago. I specifically remember scenarios, for instance, when I was a director of product at a firm and my product area got changed where I had to fake that certainty and then a month later when I learned stuff, I had to change course. This seems like a much, much better way to work. I love how you've described it and I think a lot of it is in the tooling. You need to empower your PMs to actually have a Figma editor license so that they can get into the pixels. You need to empower your PMs with Dovetail, with Jira Product Discovery, with Penda, with these tools so that they can actually go out and do this, not just say, oh, write up a document for the UXR team and the UX researchers are going to do it. PMs have to get really close to the designs, really close to the user research to enable this way of working.

**Tanguy Crusson** (01:23:40)

Yeah, they really need to get close to the research, close to the design, close to the engineers. They need to understand the technical constraints that basically inform how the designs can evolve. They need to understand the technical depth. so that they can see as well, we can't just keep piling stuff on top of each other in terms of features, we need to address our debt, whether that's UX debt or that's technical debt and how should we prioritize it. The PMs have the impossible job of really needing to be in tune with everything from the GTM all the way down to the code and back. I mean, I'm not coding, but I understand when we talk with engineers, like if they talk about an API that's not performing well, I understand the impact it can have to the different components of the app. So then we can discuss like how should we improve that?

**Tanguy Crusson** (01:24:33)

Should we post a new product work to focus on reliability work for like a month or two? Or should we start a team around reliability? As a PM, I have to be comfortable navigating these different aspects and being able to represent them with the others. When I'm talking with engineers, I'm representing the customer. When I'm talking with a customer, I'm kind of taking, like bringing the team with me in my head. When I'm talking with a stakeholder, I represent the team. So I always represent the people who are not in the room, but then I can actually keep receiving feedback, perspectives, and all this from all these other people to inform the direction we should take. And so it's the same as well as to how we organize the Jira product discovery PM team. It's not like we have PMs specifically working on one part of the app.

**Tanguy Crusson** (01:25:27)

The PMs are Jira product discovery PMs. And they are Jira for the discovery PMs because I need everyone to be able to think of this as a system holistically. And for their teams to think of the system holistically, currently we're focusing on this bit. Later we'll focus on that bit. We can understand how these things fit with each other. And that's how we create better user experiences. But it really starts with really blurring the lines between the crafts. Because I've seen that too often where the product managers do product manager stuff, the designers do designer stuff, the engineer's code. And that makes me so sad when I see it, because I'm like, you're missing 90% of the magic of creation in product. And you really should embrace that. The PM jumps in design and the engineer shits on the PM's idea. It really works.

**Aakash Gupta** (01:26:24)

It really does. And

**Tanguy Crusson** (01:26:26)

I'm sorry for my French. Pardon my French. I think it's how you say it in English. I keep swearing. I should stop.

**Aakash Gupta** (01:26:31)

Love it. Love it. I could definitely go another 90 minutes, but we are at time. If people want to get in touch with you or learn more, where should they go?

**Tanguy Crusson** (01:26:42)

Yeah, the easiest is you can find me on LinkedIn. I'm not super active, but definitely you can reach out, send me a message, that kind of stuff. If you're a user of Jira Porter Discovery, LinkedIn, the Jira Porter Discovery community group, you know you can find me there. I mean, you've probably seen my face already in a thousand looms, but I'm always happy to have a chat, especially if you've got a story that you think we should listen to for how to evolve the product.

**Aakash Gupta** (01:27:10)

And almost everyone listening is probably a Jira customer. Is there any specific way they can reach out to you if they are that?

**Tanguy Crusson** (01:27:18)

Yeah, the Jira Planet Discovery community group. You just Google Jira Planet Discovery community. We are there. And listening. Like... The one I shared today was literally from today. So proof that we actually watched this. Yeah. And again, LinkedIn as well. That works.

**Aakash Gupta** (01:27:36)

Amazing. I hope more of you guys listening adopt this way of working or at least take some baby steps. We will be sharing some of the resources that you included in the newsletter. If you have any additional questions or follow-ups and we'll see you in the next one. Thank

**Tanguy Crusson** (01:27:53)

you, everyone. Thank

**Aakash Gupta** (01:27:53)

you. Thank you so much for listening to that episode. If you enjoyed it, it would mean a ton if you could please leave a rating and review on Apple and Spotify podcasts, leave a comment on YouTube, like it on YouTube and check that you're subscribed. All those things really help support the show and help us to create bigger and better productions. I'll see you in the next episode.
