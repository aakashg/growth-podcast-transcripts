---
title: "Claude PM Masterclass from Former FAANG AI PM Jyothi Nookula"
subtitle: "She's been an AI PM at Meta, Amazon, and Netflix. Here's her breakdown of everything Claude"
date: "2026-07-13"
host: "Aakash Gupta"
guests: ["Jyothi Nookula"]
speaker_names: "substack"
substack_url: "https://www.news.aakashg.com/p/the-complete-claude-stack-for-pms"
youtube_url: "https://www.youtube.com/watch?v=uEK9ONplfRk"
duration: "01:33:20"
word_count: 14685
source: "Substack episode transcript (aired audio)"
---

# Claude PM Masterclass from Former FAANG AI PM Jyothi Nookula

*She's been an AI PM at Meta, Amazon, and Netflix. Here's her breakdown of everything Claude*

**Jyothi Nookula** (00:00:00)

understanding which surface to reach for which use case becomes one of the core pm skills that will help you become 10x more effective

**Aakash Gupta** (00:00:15)

on LinkedIn and it caught my eye. You said that you won your internal hackathon against 30 engineering teams and you used this concept of adversarial agents.

**Jyothi Nookula** (00:00:23)

Anthropic had just released a blog post around partners and long-running agents. So I looked into the blog post and they had the concept of adversarial agents that was what got me the hackathon right

**Aakash Gupta** (00:00:34)

where does the product manager line end and developer line begin in 2026

**Jyothi Nookula** (00:00:39)

get comfortable with web building get comfortable with say flawed code with all the flawed ecosystem that we how do you

**Aakash Gupta** (00:00:49)

use cloud design how do you build a knowledge base mcp server for all of your pm contacts to make cloud 10x more productive that is what we're going to answer in today's episode

**Jyothi Nookula** (00:00:59)

now there's this new rule coming up called ai builder anthropics adopted it open ai's adopted it making and building is easy now taste is what is important for us to develop

**Aakash Gupta** (00:01:10)

can you do the big reveal now and help us get that set up going in cloud code before we go any further do me a favor and check that you are subscribed on youtube and following on apple and spotify podcasts and if you want to get access to amazing ai tools check out my bundle where if you become an anal subscriber to my newsletter you get a full year free of the paid plans of mobbin arise relay app dovetail linear magic patterns deep sky reforge build descript and speechify so be sure to check that out at bundle.akashg.com and now into today's episode so i've been thinking about something we've had advanced tutorials on claude code with analytics on pmos setup but how do you actually take the entire claude ecosystem and make the most out of it from scratch i keep getting dms from people who say this episode is too complex or i'm not at this level yet i'm still stuck on chad gpt if you're one of those pms this episode is going to build you from zero to 80 we can't get you from zero to 100 in a single podcast but we're going to get you the 80 you need to know in 20 of the time i have brought back jyoti nukla you guys loved her last episode and specifically the feedback i got was that her structured communication was amazing for beginners so she is going to break down for all the beginners how to make the most out of claude today jyoti welcome back to the podcast

**Jyothi Nookula** (00:02:43)

super excited to be back thank you for having me

**Aakash Gupta** (00:02:47)

jyoti you posted this on linkedin and it caught my eye you said that you won your internal hackathon against 30 engineering teams and you use this concept of adversarial agents can you break down exactly how you won the hackathon

**Jyothi Nookula** (00:03:01)

yes so a few days before the hackathon i was trying to see what i could build and anthropic had just released a blog post around harnesses and long-running agents so i looked into the blog post and they had this concept of adversarial agents where you build an agent and then you set up configurations in another agent telling it what matters most to your company in a way not like evals but more around capabilities that you want your um agent to test and so i set up i started with that idea and then i said let me take this idea i went into plot code and i was jamming with it for almost a day uh with different configurations and there we go i had an adversarial agent evaluator running sricharangovindolla product growth aakashgupta company code and integrated that into an actual production running code and that was what got me and my team the hackathon prize

**Aakash Gupta** (00:04:17)

so that's the promise for you guys we are going to help you get to that level where do we start jyothi how can we break this down in a structured way so that people can get to this level at the end of the episode

**Jyothi Nookula** (00:04:30)

great we'll tackle it today so we'll start with understanding the clod stack first and then getting into some of the basics like how do you use co-work and then getting into plot code itself so let's get started on the clod stack so at the bottom of the stack is your models so clod has haiku sonnet and opus they're all different intelligence profiles and which one you need to use when um they have different cause profiles different intelligence profiles so that's the decision framework we'll get to in a second so this is your layer one on top of your models are what's built your surfaces which use to access these models so your surfaces could be like cloud.ai which is on your browser it could be a desktop app it could be a mobile app it could be your chrome plugin these are all the interfaces that you use to interact with cloud now these are not the same product with just different uis they have completely different capabilities and understanding which surface to reach for which use case becomes one of the core pm skills that will help you become 10x more effective

**Aakash Gupta** (00:05:49)

so this is our

**Jyothi Nookula** (00:05:49)

second layer on top of this layer is your knowledge base now this is where your institutional knowledge lives your projects your skills your memory your custom instructions now this is the layer that i think most pms under invest in it's this layer that makes claude go from being a generic chatbot to actually knowing your context

**Aakash Gupta** (00:06:19)

on

**Jyothi Nookula** (00:06:20)

that stack is your layer four which is your integration fabric for example your mcps now mcp connects cloud to every external system that your organization uses like your slack your google drive your jira your salesforce your internal databases or your own local files skills are what extends what your cloud knows how to do and what to do with that data so this is your layer four and now on top of that is your agents and orchestration this

**Aakash Gupta** (00:06:55)

is where your cloud code

**Jyothi Nookula** (00:06:58)

co-work design channels got it that's how i think about the cloud stack

**Aakash Gupta** (00:07:09)

what do people need to know about layers one and two in order to make the most out of the top layers

**Jyothi Nookula** (00:07:14)

yeah so let's get into the models now haiku is your speed machine it's the fastest cost efficient and it's really great for tasks where you need volume over depth so let's say you are trying to generate a large number of variants of something or triaging like a pile of documents or you're doing some quick classification or maybe even some tagging haiku handles this really well now the output won't have the reasoning depth of like your sonnet or your opus but for tasks where depth isn't needed much haiku is sufficient for your use case there sonnet is where 90% of my work lives it has the best quality to cost ratio so when i'm drafting prds or i'm synthesizing user research or i'm doing competitive analysis or i'm doing stakeholder briefs or i'm thinking about roadmap i use sonnet sonnet handles all of this extremely well so opus is for your high stakes high complexity reasoning tasks so let's say if you're doing some complex trade-off analysis or you're synthesizing genuinely contradictory research or you're doing some long horizon planning where you need the model like work through second and third order implication opus is really good it has really strong reasoning capabilities but i've also noticed from my day-to-day working with opus that it also tends to get into this um hallucinated stuck mode a little bit quickly then sonnet where i would use opus and it would get into like one reasoning decision point and it and it would keep revolving in that local maxima and i would have to like literally turn off the chat and move to a new chat and then start all over again to get it out of that thinking mode for example and that's when i sometimes move back to sonnet because even though it may not have as high a reasoning it's generally a very efficient model to work with and it's also more cost efficient than opus

**Aakash Gupta** (00:09:36)

got it so bring the right model to the right task it sounds like for 90 percent of the tasks for pms you'd recommend sonnet

**Jyothi Nookula** (00:09:43)

yeah i think that's a good place to start with and then if sonnet doesn't work for the depth that you want you can always like have open up a chat with opus and start there

**Aakash Gupta** (00:09:53)

what do we need to know about the next layer

**Jyothi Nookula** (00:09:55)

so next is your surfaces now plot.ai your which is your web or browser i think this needs no introduction everyone's pretty familiar with this this is where you can use to chat with it the downside is that it doesn't have access to your local system so if you have some files that you want to access cloud.ai may not be able to like directly go and change of course you can have like an mcp server but still it's it's i don't prefer it for um for anything that that needs local access that's when i use desktop so my cloud co-work runs here it's able to access my files it's able to access all the other systems that i have integrate and and run some scheduled runs which i'll show you um in a second

**Aakash Gupta** (00:10:50)

i built a podcast guest prep agent in hybrid the job is simple before every interview give me the guest's recent appearances strongest arguments company context sharp question angles and stuff i should avoid asking because everyone else has already asked for this run i pointed it at howie lu ceo and founder of airtable the useful part is it can actually go do the research it's browsed pulled sources worked across files and integrations and then turned the whole thing into a brief i can use before i hit record here's the output recent appearances public arguments company context question angles and what not to ask this is the kind of prep doc i actually want not a generic summary it shows what they believe where their thinking has changed which questions are obvious and where the thinking tension might be then i saved it as an agent the output is useful but the saved agent is the real goal i don't have to rebuild the whole thing i point the same agent at a new name and

**Jyothi Nookula** (00:11:48)

it already

**Aakash Gupta** (00:11:49)

knows the format i like the sections i care about and the kind of question framings i come back to podcast prep is one example the bigger idea is recurring work becoming reusable agents hyper agent is built by the team behind air table but it's a separate product they're offering one thousand dollars in credits to the first one thousand subscribers who use my link claim yours at hyperagent.com product growth

**Jyothi Nookula** (00:12:14)

i also use mobile for when i have a run kicking off and i can just go for a walk and i can come back and while i'm still doing my walk i can look into my phone and see if any of the tasks need my attention so this has been really helpful that way i also use claude for chrome plugins especially it's very helpful if you want to do computer use so for example when i'm launching an ad and i want to do some competitive research i'll kick it off for through my claude plugin and it'll use browser use and it will open up a browser it will do the analysis it will click through things and say here is what you need to know on how your ad should be against competitors for example

**Aakash Gupta** (00:13:10)

good for getting into like data that ai agents can't otherwise like linkedin or other things like that

**Jyothi Nookula** (00:13:16)

and also good for user testing where you can put up your product up and have um give an instruction to claude saying go find check check out this item and you can see how it goes and finds things to see how well your product can be understood by agents and where does it fall and it also gives you a really good user summary as well if you say behave like a real user and try it and so it'll tell you here are all the things that were confusing and so you can use it for user testing your products too

**Aakash Gupta** (00:13:55)

and are you using cloud code in the desktop app or using it in terminal where does that fit in

**Jyothi Nookula** (00:14:00)

oh yeah that's a good one i use cloud code in ide because i use cloud code to build and so i use cursor or or vs code and today i'll show you with vs code because it's really beginner friendly so i use cloud code extension in vs code

**Aakash Gupta** (00:14:18)

is there anything else people need to know about layer two or should we move on to layer three

**Jyothi Nookula** (00:14:21)

let's move on to layer three and before we move on to layer three i'll come back to show you the knowledge base on how to create but first let me show you how you you as a pm can 100x your productivity by running a few skills and scheduled runs in co-work

**Aakash Gupta** (00:14:42)

awesome

**Jyothi Nookula** (00:14:43)

because that will bring us all together on like building your own chief of staff and then i'll show you in plot code how you can you can do something much more fun

**Aakash Gupta** (00:14:52)

so should people be using chat at all or should they always be using co-work

**Jyothi Nookula** (00:14:57)

so chat is to get you like i have a question what does this versus that or tell me about a little bit about this information so it's it's more like a place where you go to search instead of going to google search no i just find myself going to plot in chat and asking it some questions i use co-work for automations and i'll show you a few today that i use like i have a morning i have my jira connected so i get my stand-up brief so every day it kicks off and tells me here are all the jira tickets that need your attention and here is how your project is progressing here are four blogs here are three things that have changed so it gives me my uh brief even before i go to the stand up and end of day summary so there are a lot of things you could do in co-work um in terms of automations to just make your um work life much more easier so you're focusing on things that need the most attention

**Aakash Gupta** (00:16:03)

awesome so can you show us how these work

**Jyothi Nookula** (00:16:05)

sure so co-work is there on your desktop app so you need to have your desktop app and you also need to be at least a pro member which is like about 20 dollars per month so with co-work i can schedule my automations so you can see i have a few that have scheduled like end of day daily briefing day stand-up briefing chief of staff and i'll walk you through each one um right now so every day at 9 a.m this runs for me where i can say and i'll show you a few as well right now so you can see my instructions i'm saying you're my chief of staff generate my morning brief for today here are your data sources and i connected it to google calendar gmail google drive and jira how did i do that let me show that to you in a second so go to customize go to connectors and click on the plus right now you can see i have connected to atlassian robo gmail calendar and drive but there's plenty other connectors that you can connect to like canva figma notion wherever your data lives you can connect to it all that you have to do is just hit a plus and that brings it in and you'll have to authenticate it and beyond that that's all you need to do so i said here are my data sources i need you to go into google calendar gmail google drive and jira pull today's calendar events for each meeting capture the title the time the attendees the description and any attached docs for each meeting with external attendees or something that looks important search the google drive for any attached doc or recent docs with the meeting title or attendee names read enough to know the agenda and search gmail for recent threads pull jira items needing my attention scan gmail you can also add slack to it and have specific channels that you wanted to review and send it to you as a morning brief and i said here's my output format i want a morning brief top three things that i need to focus on today calendar today here are the things from inbox that need my attention here are the things from jira that need my attention and here are some rules and this is important is i said keep it under 400 words because i don't want to be reading a coffee table edition the first thing in the morning so keep it under 400 words so it's very easy for me to skim through and understand what i need to focus on what needs my attention immediately claude can sometimes pump you up so i said just give me facts no like great news so don't hype me up never invent deadlines or action items so this is like a guard ray i've put in there and i've asked it to filter aggressively so that i don't have to read anything um or everything all the time and if it's a light day just write a three-line brief and stop so this is

**Aakash Gupta** (00:19:03)

my use my markdown formatting in order to help it with the headings as well

**Jyothi Nookula** (00:19:09)

yes that makes it easy for cloth to read

**Aakash Gupta** (00:19:12)

cool

**Jyothi Nookula** (00:19:12)

and so you can see there are a few things that have run previously so one thing to remember is these automation tasks run only when your laptop is turned on if you close your laptop it doesn't run until your laptop turns back on again so when you choose the timings just remember that and so have it at a time when you think your laptop will be on but otherwise when you turn it on the first time it will last you and will run that automation at that time so like for example let me show you something that ran so i ran something that that um that's from may 8 so it captured a few in box things that needs my attention and i can run something now and see how that works there's a run that started now so it'll go and collect things and you can see the whole process of how it's thinking and if you notice i'm using hyco for this i didn't go and use opus just to like save um some tokens it asks you for permission it'll go and pull up things it'll search email threads and while that's happening let me show you the next briefing so that was my chief of staff morning brief i also have an end of day which wraps up my day which runs at 5 pm every day now my end of day instructions are very similar the data sources are similar but the steps are different so i said read the morning's brief and that's what i had planned to do well what actually happened today like which meetings happen which were cancelled and pull tomorrow's calendar as a preview and so the output format is like tell me what's shipped what slipped and what's new from today and show me tomorrow at a glance again i have some rules so this is my instruction for end of day

**Aakash Gupta** (00:21:15)

and i guess you could even enhance these if you're interested right you could probably connect up your analytics you could add in more context from other systems like your crm the limit is just your imagination here

**Jyothi Nookula** (00:21:27)

absolutely you you can connect it to as many data sources as you want um beat even sometimes your um facebook ad systems or your crms or even your youtube um and you could get an end-of-day summary um that captures and you could also say create a nice dashboard which i'll show you um that i did for jira where i said the the results uh print it up in a nice dashboard that i can view and it does that for you

**Aakash Gupta** (00:21:56)

and so this is basically taking over a lot of what people would have hired a relay or a lindy last year or a gumloop or a even make.com and now you can just build it in claude

**Jyothi Nookula** (00:22:08)

yes and one thing it's different from all of those other ones is you would have to like paint box by box think about how the interaction works connect each of those and if one thing fails your entire loop fails that was like how you used to do it before in like say innate n or lindy or gumloop or other things that you want but here you see i'm just giving natural language instruction i can even convert that into a skill so it's pretty robust where it's very easy for me I don't have to think about the architecture I don't have to think how it's connected which box flows into which where is a conditional formatting I don't have to think of any of those

**Aakash Gupta** (00:22:52)

so end of day chief of staff what are the other two scheduled tasks doing for you

**Jyothi Nookula** (00:22:57)

so this one is my stand-up briefing this is the one that's connected to Atlassian that is my JIRA jira board and so i said use this atlassian connector to fetch all issues in the active sprint and here's the brief i wanted done since yesterday which are the issues moved to done in the last 24 hours in progress issues blocked or at risk new since yesterday and what's the sprint held and i said keep the total under 250 words and show you an example of this this it's asking me for some approval i approve it and it's actually rendered it to me really nicely for me to view and because i asked it to create a dashboard it's running that

**Aakash Gupta** (00:23:44)

i think what people don't realize is how much better these systems got around december of last year what really happened that enabled all this to work so much better now

**Jyothi Nookula** (00:23:52)

improvements in the llm reasoning capabilities where previously if it and previously as well it was much better than what it was two years ago so we're constantly improving but compared to last year the new word now is hardness so the memory the reasoning capabilities the tools that it can access all of the underlying systems have improved and so the latest improvement is this hardness engineering that is adding so much value into how your systems behave now

**Aakash Gupta** (00:24:31)

now we have your stand-up brief how would you rate this is this a good stand-up brief or is this just okay i

**Jyothi Nookula** (00:24:36)

think this this is a mocked up one so therefore it's showing me a few things which is still a lot better than what i would have had to like go and listen in a call um but there's definitely ways i could improve this much more like for example um it's telling me like there's no progress in 24 hours um this i could look at which are which are those ones that have not moved at all and see who is the assignee on those and set up an automation for a claude to go reach out like ping them on slack and ask them for an update for example so you could set up nested more more automations as well so it's it's really helpful to keep away your busy work so you're focusing on actually going and solving your customer problems

**Aakash Gupta** (00:25:29)

so if these are the four scheduled tasks are there any other scheduled tasks that you recommend pms invest the time in building

**Jyothi Nookula** (00:25:36)

so what i have here is some examples but there are lots more you could do so here's an example so let's say if there is a ticket a jira ticket or even a customer support uh ticket that's come from your um from your customers it could automatically be you could create a jira ticket from it you could point your cloud code to get activated so that it can actually go and implement that and cut a pr and so there's a pr waiting for review

**Aakash Gupta** (00:26:07)

very cool so if that's scheduled tasks i think the next thing you had mentioned this section were skills what do we need to know about skills what skills should we have how do we create them

**Jyothi Nookula** (00:26:17)

yes so if you go to customize again and you can see skills this is where you can add different skills i'll show you some examples of some skills so here's my skill on synthesizing customer interviews so as pms we have we sit through a lot of customer interviews or at least we get a lot of customer interviews for research for feedback for focus group testing for beta testing we do lots of that

**Aakash Gupta** (00:26:43)

and i wanted an easy way

**Jyothi Nookula** (00:26:45)

for me to have or understand what's key what's important and then generate insights from it so this is my skill that does that which is synthesizing customer interviews it has like when do you use this skill and what's the checklist so it has step by step like inventory the inputs extract observations with citations now that's important i'm not asking to just extract observations i wanted to cite so that it hallucinates less use the speaker's own words do not interpret yet and separate behavioral observations from stated preferences i also have additional .md files listed in here linked so that it could leverage those if needed now that's the beauty of skill is skill is not just a markdown file you also can add functions into it you can have it link to other skills for example so what used to happen before a skill was that the whole tool would be loaded into the context and now imagine if you have like 40 tools all of those are loaded into the context it eats into your context memory so by default your your LLM or your model would have very limited memory for even before you even began asking it anything what skill does is similar to like progressive disclosure where it just loads up 50 words of just like the name and the description into the context now you can imagine the load is so much lower when the model decides during orchestration based on the question you have asked it goes through the list of tools to see is there a tool that i need to use or is there a skill that i need to use if it decides that this skill is valuable based on the description then it will load the next set of instructions into memory so that's why skills are powerful because it doesn't eat up or clog your context window for your models and it progressively disclosures and the third is you can link it to more files or more uh skills or functions even like you can have a function where it needs to go run and do something

**Aakash Gupta** (00:29:16)

so yeah i think it was around february of this year when they made skills not just a single markdown file but you could have multiple files and if you aren't using multiple files and your main one isn't less than 500 lines you're really missing out i feel

**Jyothi Nookula** (00:29:30)

yeah and so for example i have this evidence underscore rules dot md which i'll show it to you in a second um so that's in step two so if step two is invoked then it will go and see evidence underscore rules to identify to understand selection criteria or how to handle ambiguity then step three is like cluster into candidate patterns and look i'm here again linking it to another one called jobs to be done framework then i said then apply the pattern threshold and then surface the contradictions and then draft hypothesis and then validate every claim against the source codes and that's when i said assemble the final output but i want it in this template and this template is output underscore template so i'd give it my template so if it gets to step eight is when it will load the output template.md

**Aakash Gupta** (00:30:26)

and right now we're paying a lot of attention to what is actually in the skill file how important is that for pms versus just letting claude kind of handle what's in the skill file

**Jyothi Nookula** (00:30:38)

so a lot of times we do use claude to write the skill file too but it's also shown research has shown that AI generated skill file is less effective than human written skill files so that doesn't mean you don't use AI there what the way I interpret this is put in your human domain knowledge in there to make it work for what you need versus just taking it and automating it from Claude and putting it in there so I have used Claude a lot to help my skill files write my skill files but then i go in and i add my own tweaks like what's the template that you want how do you want it structured and i work with plot to keep making that changes and from there um add and tweak furthermore to get to the skill file that i want

**Aakash Gupta** (00:31:36)

and how often should we be updating our skill files

**Jyothi Nookula** (00:31:39)

as often as things change for you so the way to think about skill skills is this is um kind of like a a guidebook or a playbook for your cloud to know how to do a task for you so let's say for example prds now if your company doesn't change the template of how a prd is maybe that's fine but but your domain may change or your understanding of your domain may continue to change and you do want to like come back and review your skill files um maybe say once every quarter depending on how often things change so the parameters for you to decide is how often does things change in your domain how frequently do you use that task for and the third primary thing is how is the output currently because if you're not satisfied and you're like it was good but now it doesn't seem to be as good maybe go back to a skill file and say you need to update it so it's like that drift as well that you that gives you a cue that you need to go and update it

**Aakash Gupta** (00:32:47)

and what are the most important skill files for pms to create

**Jyothi Nookula** (00:32:50)

backlog triaging give it context and i'll show you in a second how to do that from a context point of view but give it context so backlog writing prds customer interviews even your support tickets how do you take a support ticket and how do you put it into a jira that could be an automation but it could also like it could be a skill that is scheduled to run every time there is a trigger now in that case your trigger won't be something that runs time-based because there's no like one particular time you're going to get a support ticket but it could be a trigger when whenever there is a support ticket added in your service now or zendesk or wherever your support forums are

**Aakash Gupta** (00:33:46)

so is it fair to say you're going to have more skills than scheduled automations some of your scheduled automations might reference a skill

**Jyothi Nookula** (00:33:53)

that's true and the way to think about it is most of your scheduled automations are time-based so things that are more personal productivity based that happen at some sequence like I know I meet my manager once every week so I know the meeting is always on Wednesday so I run my automation on Friday evening and it maps out saying here are the things that you need to talk to your manager from all these other meetings that you have sat through

**Aakash Gupta** (00:34:22)

makes sense the last layer you talked to or i think you're going to show us how to do context in this skill

**Jyothi Nookula** (00:34:28)

so here's the thing so until now what you have done is you've connected it to sources it can go read all of those sources and go and do the task for you but it doesn't learn the people around you it doesn't learn your connection to people it doesn't learn it doesn't have that knowledge graph or the knowledge base for what you're working on and so i wanted to build a chief of staff that understands and is grounded in the knowledge base that i have and so i went to cloud code and i said let me spin this up so i'm going to show you what i'm going to do there so i'm on vs code now for those who are looking at this ide for the first time explorer is the place where you can open up your folders and for you to find clod just go into extensions and search for clod code for vs code and you'll find it there'll be an install just like how you see something else that i haven't installed there'll be an install button that you'll have to click on and that's it it'll install and then it'll ask you for your login and everything when you install it so that way you're logged in and ready to go always and it'll show up here as an icon that you can click any and ask whether it's a new session or existing session i'll click on new session and you you'll see how it makes it so much better now that i can just talk to it right here of course i can open the terminal too and it'll i can see if if i need to like run some commands but right now i can just talk to it right here in natural language so here's my chief of staff um template that i have written where let's say i've joined some company i'm the senior director there um i want to build this personal agent that helps me navigate strategy execution people politics so the agent should learn from my meeting trans transcripts and i use granola for my meeting transcripts so it should learn from my meeting transcripts in just documents like strategy docs or charts prds emails and build a knowledge base over time about people dynamics topics company context and so i said this is my architecture overview of inputs here's my context and my agent and i said here's my documentation and

**Aakash Gupta** (00:37:08)

claude wrote this right

**Jyothi Nookula** (00:37:10)

yes claude wrote this yeah cool um i told it in natural language like i want xyz here are all the things and it kind of created this whole um .md file that i could use now with claude again um to build it so let's say i joined a company as whichever role and i say i want to build a personal ai agent that helps me navigate my work like my strategy execution people and politics so the agent should like learn from my meeting transcripts i use granola you could use zoom you could use team you could use whatever you use for transcripts you just have to like mention that here ingest documents and build a knowledge base over time about people dynamics topics company context and here's the architecture overview now i gave my use case to claude and it wrote this up for me and put this architecture overview that i could use it then give it back to claud again to code it up and so for part one there's uh here's my document ingestion pipeline so i have like strategy docs what to extract like i want to extract goals priorities metrics timelines and as pms we are so cross-function it's not just our docs we read 50 docs in a week so this is like really helpful for me to like just feed that in and it'll read it up it will store it into a knowledge base and i'll show you that in a second and it's really cool where the other day i was i was in a meeting this person was showing me a few things and after the meeting got over and we record transcripts in google meet and so when the transcript came through my chief of staff reviewed it and then it said you know what you should make this person your ally because this person is good at x which you're trying to like get into and so i'm like oh okay that's great and then there was something else that i needed to convey to somebody and my chief of staff said hey this is extremely sensitive have you thought about xyz people that you have to inform first before you convey to this person and that's so thoughtful because now it's it understands my org it understands who is doing what it understands their personalities so it's like really powerful it's like really i have this chief of staff that's telling me always what i need to do so here are all the supported documents i wanted to ingest and here's the document extraction prompt so i'm saying you're helping me build a knowledge base about my workplace i'll share a document extract relevant information and so i said for strategy or planning docs extract this way for orgs and org charts extract these for prds extract this

**Aakash Gupta** (00:40:10)

more

**Jyothi Nookula** (00:40:11)

for emails or communication extract these capabilities so i have this for each of the ones that i need and i said format the output in this wave for it to store in my knowledge base and here's a knowledge base structure it has its context it has people topics meetings documents company and my context like what are my priorities my okrs my preferences notes questions insights like political landscape and patterns that it identifies or extracts it can save it here and these are like patterns observed over time you can add more as well like to do for example it could be a running to do that your chief of staff could be maintaining for you and here are the templates for the different types i said extract this for it to like save it into the knowledge base any document that i give extract the metadata the summary the key points involved what's the relevance to me and my vertical what are the action items and some raw notes and for people profile again extract these metadata how they operate the communication style making behavior what works or doesn't work what they care about what are their motivations so and what's the relationship to me and then over time keep reviewing the relationship quality whether they're a strong ally friendly neutral cautious friction

**Aakash Gupta** (00:41:53)

by the way guys if you want the exact information that jothi is sharing you can get all of those in the github link in description

**Jyothi Nookula** (00:42:03)

organizational dynamics the observation log company strategy templates so when you have your companies sharing you the strategy saying here's what we're going to do in 2026 here are the key things i wanted to extract org structure template and meeting transcript extraction so when i give it a meeting transcript what i needed to extract the agent system prompt and this is my prompt for the agent on you have access to my context kb your job is to help me ramp up fast give me strategic advice grounded in context help me prepare for meetings coach me on people of politics help me think through decisions connect dots across documents and meetings and keep me focused on my priorities again style is like my style what i like don't sugarcoat politics when i share a document extract key information update relevant kb sections and so i've given it all of this information right so this is all about like what it needs to do so i have this now i'm just going to point my cloud code to it and say now can you build this knowledge kb and can you put this behind an mcp server so that i can use my cloud desktop to access my knowledge base so i have an implementation you can see my implementation i'm saying cloud desktop plus mcp so build mcp servers for kb read and write chat with cloud desktop can also connect to google drive slack directly and so i said create the context kb folder structure write my goals initial priorities in just any onboarding docs and after your next meeting run the transcripts for extraction and the kb compounds over time so i'm just going to go to plot code and i'm going to say can you implement so

**Aakash Gupta** (00:44:02)

you're using the at command to pull up that specific file and reference it

**Jyothi Nookula** (00:44:07)

yes so that way it's effective it just knows which one i'm referring to but even if you don't do it if you tell a chief of staff agent design it can go and search through your repository um and find uh the right one for you so you can implement

**Aakash Gupta** (00:44:24)

now here i'm if

**Jyothi Nookula** (00:44:26)

you see what i'm doing um there are there's one thing i want to like show um you is shift tab i can go into plan mode which i can use it for planning again if i do shift tab going to auto mode i can go shift tab ask before edit mode i can go into shift tab again edit automatically where it gets into like actually coding and doing so if you're planning like for example how i planned with it to create that .md file i was all in the plan mode where i was like let's just plan don't start coding anything let's just talk

**Aakash Gupta** (00:45:05)

um and

**Jyothi Nookula** (00:45:06)

now once i'm ready um i can shift tab again and go into edit automatically and it will set it off to go do a few things

**Aakash Gupta** (00:45:18)

and why do we want this as an mcp server

**Jyothi Nookula** (00:45:22)

it's a good call so if you want your knowledge base and say obsidian you can connect it that way and and put it behind an mcp server and capture it and here at that point you just have to say do you put this in obsidian at that point but i'm using local i'm showing it on my local file system because it has a few interesting things when you're working at a company you don't want such really personal private data living in some cloud and you wanted for example to live on your laptop so the day when you walk out of the company the laptop goes to them anyway so you walk out with no data on your hand and so i prefer because this is just so much of knowledge base and very private and personal i keep it on my um laptop but you can keep it on obsidian or notion or whichever one you want to use for your knowledge base you just have to change the system prompt at that point

**Aakash Gupta** (00:46:28)

and what does putting the mcp server on top of the knowledge base help with why can't it just be like a set of markdown files and folders

**Jyothi Nookula** (00:46:36)

yes so what what it allows it to do is your you can talk to your knowledge base from your desktop app because otherwise where is the knowledge graph sitting it's sitting in some place and if it's sitting on your computer then it can read and it can write to it so all those things that we said extract this extract that it will actually go and write it on into your knowledge base automatically

**Aakash Gupta** (00:47:06)

okay so it makes it a little bit more portable than a cloud code web session

**Jyothi Nookula** (00:47:10)

yes and so you can go back and even look at all the .md files to see like what it extracted from which um meeting but over a period of time like right now i have my knowledge base is like really huge um and so i um i don't even go look into the .md files i just ask desktop um claude saying hey i'm going to meet my manager one-on-one tomorrow what should i know and it will go and dig up all the context in the knowledge base and say here are all the things you need to know because it has my to-do there it knows the style of my manager it was really interesting it said this person is a no first person and so you should just get to it versus preambling a lot around it because it's capturing across various conversations patterns too

**Aakash Gupta** (00:48:03)

quality of the data going in is the most important thing what is the data a pm needs to make sure is hitting their knowledge base

**Jyothi Nookula** (00:48:09)

your meeting transcripts for sure because the number of meetings that we attend there's a lot of data there's a lot more richer context there around people their body language when do they push back how do they react um so it's there's a lot of like understanding of context that happens there so definitely your meeting transcripts your um key documents that you receive like say strategy docs that i write i i say push this into kb so that it uh remembers so the next time i say i'm working on this project it knows it has context directly um and any other um documents that you review you can push that um to your knowledge base too and then your slack your slack threads that's the other place which is super rich uh beyond meeting transcripts

**Aakash Gupta** (00:49:02)

and so do you need to like update your kb somehow or do you set a scheduled task to update your kb or how do you make sure that it's kind of no so

**Jyothi Nookula** (00:49:10)

every time every time you have a meeting transcript it writes to the kb

**Aakash Gupta** (00:49:16)

and how do you set that up

**Jyothi Nookula** (00:49:17)

yeah i'll just show that once this is done so uh it's again your mcp so if it is let's say you have granola so every time or you have google meet and every time there is a new meet recording that hits or a transcript that hits your inbox you could set up a co-work automation to say use this and update kb for example

**Aakash Gupta** (00:49:42)

so set up some sort of automation to make your kb updating make your kb an mcp server so that you can access it from regular cloud chats not just cloud code web sessions and then you're really putting everything together within layer three you've got skills you've got memory is there anything people need to know around projects

**Jyothi Nookula** (00:50:03)

yes um in a quick second once this is done it'll actually ask me to create a project and put the instructions in there

**Aakash Gupta** (00:50:12)

okay and what are the projects pms should be creating

**Jyothi Nookula** (00:50:16)

the way to think about it is organize it like your folders which have unique information related to it so let's say you have you work on say three projects at company like say you're you're pming three swim lanes and and each swim lane could be a project and you can have the necessary context that you need in there in as project instructions that you could then use for your cloud to understand that a little better got it

**Aakash Gupta** (00:50:51)

let's do it

**Jyothi Nookula** (00:50:51)

so here it's done there's a knowledge base at context kb full structure so i'll just show that to you and it's also mcp server is at the server.py installed here it exposes these tools and it appended chief of staff server alongside my existing file system server and so to activate i just need to fully quit my desktop and reopen the cloud desktop and reopen and then chat start a new chat insert the chief of staff system prompt from the slash menu and then try list everything in my kb or paste granola transcript and run extract meeting and it also added details and troubleshooting in a readme as well so let me quickly pull up my context kb and just show you how that looks and let's say i don't know where that is for example i could also ask it where is it but in this case i will pull it up and show you can see created two folders context kb and my mcp server i hit on context kb it has created these folders in a nice way company documents insights meetings all of the things that i asked it to like capture it has ready folders and so you can see this md file set up for everything so as and how it's extracting it will write into these .md files and this is the mcp server so let's see what it has asked me to do from the slash menu okay so let me first quit my desktop app quit is just command q so i quit it and then i reopen so i have reopened now if i go into customize and connectors let's see you can see it has installed my chief of staff local mcp server

**Aakash Gupta** (00:52:51)

this is so cool we've done a lot of cloud guides and nobody has really shown this feature before

**Jyothi Nookula** (00:52:56)

this has saved me so much of time like it's literally my productivity booster and it tells me things and nuances that i might have forgotten otherwise okay so we restarted um insert the chief of staff system prompt from slash menu now i could say or let me say where is it where is the system from let's say i don't know right you just ask it so look it's given me the system prong lifts inside the mcp server here it's the chief of staff system okay how to use it so after you restart i can in a new chat type slash and you will see the system prompts okay so let's go here so after i restarted i'll create a new chat and i will say what did it ask me to do or it's saying you can use this in cloud project custom instructions feed so i will go create a project and put that as instruction so let's say i'm going to say this is i'm going to create a project and i'm just going to use um say i'm working on a product called meal planner and all my meetings or it could also be company x at like uber level if you just want it to be like one i can just put company x and here's where i i can give um my instructions let me first like create the project and then i can add my instructions here from so i can go into my file system and my so let's say i'm not able to find it i'll say can you create the system prompt as a .md file that i can paste into project instructions so it's writing the prompt so there you go here's my prompt i can just copy it and i'll show you what it has so i'm going back to my project instructions i'm just going to paste this so it's saying here you're my personal chief of staff an AI advisor who helps me navigate I'm so and so I just started you have MCP access use these tools your job is to wrap me up fast here's my style when I share a document when I share a meeting transcript so we do you can modify this more and refine this more but for now I'm fine with this so I save that instruction now if i give it a meeting transcript let's see what it does let's say i have this interview that i got i'm going to add this

**Aakash Gupta** (00:56:00)

here and

**Jyothi Nookula** (00:56:02)

i will say log it into kb let's see what it does i log this interview into a kb

**Aakash Gupta** (00:56:14)

so ideally it should be using kind of the right tool in our kb mcp server

**Jyothi Nookula** (00:56:19)

so it wants to use my kb so it'll ask for permission once because it's the first time we have set up it's asking all the permissions but after that it's pretty smooth

**Aakash Gupta** (00:56:29)

is there like an always allow permissions mode on the app like there is dangerously skip permissions in cloud code

**Jyothi Nookula** (00:56:36)

there is but the thing is the first time it will still ask for it because it's accessing your tools and I do give it always allow so then it'll run the next time I send it something it doesn't ask for permission it'll just go directly read so you can see it's loaded a bunch of um mcp tools um and so it's going and saving that in meetings underscore template dot md and then it'll give you some something around one discipline note as this is a single interview so there's no pattern yet but if i add like a few more um it'll generate some patterns and i and you can actually just have like a co-work either so there are a couple of options right so you can every meeting transcript you can just paste into this and it will automatically extract and fill your knowledge base or you can have a co-work automation that every time there is a meeting transcript in your email and look for what how the meeting transcript lands like google meet has like a google meet meet recordings or some some transcript word so use that and say every time this lands in my inbox automatically log this into my kb and it will do this all this thing automatically for you and if you're an email heavy company you could say every email that i get just log it into my kb it will do that too

**Aakash Gupta** (00:58:05)

oh man you might burn some tokens that way

**Jyothi Nookula** (00:58:08)

you will but you have such a rich knowledge base at that point in time where it will connect all the pieces together so you can see now both files are now in kb here's the things that's logged um a couple of judgment calls so you see this is the first time so it's not like it's going to give you the best of insight but you can see it's giving me things worth my attention so i'm a senior director um the AI coach is part of Lumen in your lane and it's the weakest thing in this interview Maya whoever is this user ignores it and two times it showed up that she bounced off it I just wanted a yes or a no and so that's a clean agent ux signal where and it's this kind of thread worth watching as more interviews come in so you see how it's just one interview in but it's giving you insights and things that you need to watch for

**Aakash Gupta** (00:59:02)

love it okay shall we move on to layer four i feel like we've already a little bit talked about layer four with people because we've showed them an mcp and layer four's integrations but you had this really cool linkedin post which maybe you can teach us a little bit about right now um what what exactly do people need to know about mcps

**Jyothi Nookula** (00:59:24)

yes so mcp is the way that allows you to connect to different capabilities like your gmail slack i think we connected to a bunch uh in our co-work um and so i didn't i showed you two things i showed you remote mcp i also showed you local mcp like your knowledge kbe is your local mcp that uh you're accessing

**Aakash Gupta** (00:59:49)

what integrations or mcps do pms need to make sure that they have

**Jyothi Nookula** (00:59:56)

so look at the tools that you use more often so like gmail uh for example assuming your company uses gmail for emails you want to connect that calendar you want to connect that you want to connect your slack you want to connect your meeting transcripts wherever they are stored like if that's granola or if that's google meet or zoom recordings you want to connect those you want to connect your crms your dashboards your jira boards your maybe you're using amplitude for analytics connect that there maybe you're using some other tool like radar for observability to monitor your the performance of your application connect it you it's the the possibilities are really endless so for example one of the tool that i had connected at work is nvidia bionemo model to help show and do drug prediction based on a few component libraries so it's like really like it's you're only limited by what you can imagine but that doesn't mean you go you just go on MCP shopping spree so I would say start off with like connecting what works for you and what use cases you're trying to solve and so if you're a beginner try to follow through this video and do some of the initial automations that I showed you in co-work to just get started get your hands wet and then go build this chief of staff for yourself and you could ask your chief of staff what else should i connect to and it will tell you here are the list of servers that you need to connect to because i'm seeing this being mentioned in meetings and you don't have the access to that

**Aakash Gupta** (01:01:44)

love it so you can actually progressively build on your connections with your chief of staff start with that meeting transcript let's move into layer five shall we

**Jyothi Nookula** (01:01:53)

yeah

**Aakash Gupta** (01:01:54)

lovely perfect

**Jyothi Nookula** (01:01:55)

okay

**Aakash Gupta** (01:01:56)

all right so that covers layer four we've now done layer one two three four the next is five what do people need to know about agents and agent harnesses

**Jyothi Nookula** (01:02:05)

so we have built cloud we have used cloud code for building our capabilities we have used co-work which are all sitting in your five layer five now i want to show you design cloud design

**Aakash Gupta** (01:02:18)

so

**Jyothi Nookula** (01:02:19)

the thing with cloud design is you have to do cloud.ai slash design um so let me show you that cloud.ai slash design it is not integrated directly in your cloud.ai yet you have to go through plot dot oh

**Aakash Gupta** (01:02:35)

there we go

**Jyothi Nookula** (01:02:36)

and so you can see it's in research preview now you can as pms we do a lot of design work we prototype we create slide decks we create mock applications and plot design really works with a lot of those things so for example you can i'll show you a few things here so prototype i can give it a name you can see there is wireframe and high fidelity so you can choose which type you want on slide deck you can give the project name and you can even attach your speaker notes and it'll create a deck again you can use an animation based template to create something and you have another now on your right you'll see you have recent any designs that you have worked there are examples that you can use to get inspiration and you can use as templates and there's something called design systems now design system is something interesting now if you if you have a brand color like for example companies that have a design guide you want your slides or your wireframes or your markups to look similar to what your console is or what your company's colors are and then you can use this design guide here you can just click on create you can link you can either give it a link on github or you can upload a figma file or you can add all your assets here and create a design system i'll show you an example of a linkedin post i did i just gave it my post and i said can you create visuals for it um and and so it created this carousal that i wanted in the colors of my product next gen product manager um so um it created this eight card caruso based on the uh text i gave it so i gave it my post my linkedin post i said here is what my linkedin post is about can you create this and created this for me now here's some cool things i want to show you now it's built this now let's say i want to mark it up i want to tell claude to change something so maybe say i wanted to tell uh make layers and use orange highlight color and claude can go and change just this one piece

**Aakash Gupta** (01:05:24)

so it's got that visual editor built in now

**Jyothi Nookula** (01:05:27)

yeah and you can also draw up things that's pretty interesting for editing so you can edit I can give it instructions right here and say edit this I can leave comments yeah I can change I can do comments like

**Aakash Gupta** (01:05:48)

oh like we used to do in Figma but now I will execute the edit

**Jyothi Nookula** (01:05:52)

yeah so I can give it comments right here and send it to cloud um and i can um even drag uh and i can like just draw and say make it counterclockwise

**Aakash Gupta** (01:06:08)

wow so this is a carousel but should pms basically be creating all their presentations in cloud design now

**Jyothi Nookula** (01:06:14)

i used to be a big gamma fan and now i just use cloud design for everything it well it consumes more tokens the token budget is different but it's being very rewarding where i don't have to sit and create slide decks anymore and does it in my brand guide and so it just doesn't even look any different so it was funny I had a meeting with my CEO and one hour before I have my content I pushed it to Claude I made it create a slide deck it's like looks so professional doesn't look like it was just done like a few minutes before it looks like I spent several hours to sit and create it

**Aakash Gupta** (01:07:00)

wow so it created a ceo level presentation for you in an hour that looked like it took hours very cool should pms be making prototypes in cloud design

**Jyothi Nookula** (01:07:11)

so here's the thing so you there are different types when you need different uh levels of uh prototypes so for something quick and dirty where you're like is this how i want this to be um use cloud design if you need but i am more a cloud code user because i'm like i'll just spin up and go create that app really quickly and i had a it's something like an app so people could like click on it and see how it works and you get really good feedback that way but you also could use this to create your slide decks to make presentations to your company about what's the feedback from that user interview you could use this to create quick uh design patterns um that you want to like share because your app may be like easy for user testing but maybe you you want this to like um uh create some marketing content to share with your uh marketing team or you want to create training uh playbooks for your sales and accounts team to tell how to go use this product and these are like really quick designs you can generate uh without having which looks polished and professional for them to like just go put it into the um into wherever your uh knowledge base is

**Aakash Gupta** (01:08:37)

awesome you mentioned you use cloud code for prototyping and that's where i wanted to take it next so we started this episode with adversarial agents and your cloud code setup to win the hackathon can you do the big reveal now and help us get that setup going in cloud code

**Jyothi Nookula** (01:08:53)

so here's the thing i have to create that whole thing here

**Aakash Gupta** (01:08:56)

all right let's do it

**Jyothi Nookula** (01:08:58)

what do you have we have the time

**Aakash Gupta** (01:09:00)

let's do it

**Jyothi Nookula** (01:09:01)

so create a new session let me actually open up a new project so you can see i'm opening up a new window so my previous one doesn't interfere with this and i'll go create a folder for this so i can open it up so now let me open and you see it's a clean folder i'm just going to start a new session here and i'm going to say let's build an adversarial evaluator

**Aakash Gupta** (01:09:31)

and what is gain

**Jyothi Nookula** (01:09:33)

so generative um adversarial networks were very popular before llms uh came into the picture and that was primarily how first uh generative ai industry even started mostly applied to images where there are two networks there is a generator and there's a differentiator the generator generates and the differentiator tries to predict is this image real or fake and the optimization loop is that the generator should get so good at generating images that the differentiator gets confused whether it's real or bad

**Aakash Gupta** (01:10:14)

interesting i've never seen this built before

**Jyothi Nookula** (01:10:18)

theme architecture let's kick it off and we we massage it along the way noodle it and figure out what how we want it to work

**Aakash Gupta** (01:10:29)

so what are while this is building what are the keys to winning a hackathon outside of creating this gan inspired adversarial agent

**Jyothi Nookula** (01:10:37)

so here's the thing it's not about um writing code has become so easy now right so building is easy it is thinking about the new capabilities and how you want to go solve the problems that your customers have so it's more imperative now to put on your product hat and see where are the problems today how where where are the most friction points so that pain and problem first mindset or first or design principles that we have as product managers should continue to stay here so you can see now it has asked me for a few questions around agent interface how will i call your agents on the test so let's say for simplicity it's just cloud system prompt which model should power the adversary and the evaluator so let's just keep sonnet how should the results be presented you can go really like even a web ui you could build a streamlet application i'm just going to go cli and json

**Aakash Gupta** (01:11:46)

what are the pros and cons of those various options web versus cli and json

**Jyothi Nookula** (01:11:50)

so cli and json json shows you right in the terminal it may not be pretty and not and may sometimes overwhelm people as well streamlet gives you a really nice web ui and a dashboard makes it really presentable now that's where you have to think through who are your users if your users let's say it's a developer who is going to like use this application which is what i had built for they're very comfortable staying in their terminal reviewing things in their terminal and so i don't have to complicate my life further by going and creating the streamlet but if i was building it for like say my mom she's not comfortable looking at things on a terminal so i would want to present it in a way that's easier to look understand and access information so you have to think about the kind of users and where do they see this and what's their use case to think about these options

**Aakash Gupta** (01:12:52)

you've been a senior product manager at amazon a lead product manager at meta director of product at netflix now you're a senior director of product at a startup how do you think about the future of the product role here the pm is basically doing coding work this traditionally would have been in the developer sandbox or set of tools where does the product manager line end and developer line begin in 2026

**Jyothi Nookula** (01:13:21)

different companies are trying it in different ways now there's this new role coming up called ai builder or you can see it as a member of technical staff anthropics adopted it open ai's adopted it this this less of like engineer product manager designer these roles are all combining into being a member of technical staff and the ratios are also changing previously if you see one product manager works with eight engineers now it's like two product managers one engineer so the roles are also like collapsing quickly where your engineering is helping you guide in terms of how do we scale the systems how do we harden the systems whereas you as a product manager you're like well enabled to go and tackle those PR issues yourself to tackle the user feedback yourself along with plot code

**Aakash Gupta** (01:14:32)

so if you're a pm and you've watched this video and you want to become a builder pm nab one of these ai builder pm roles at a startup like yours join your team let's say hypothetically what's the roadmap to get there

**Jyothi Nookula** (01:14:47)

get comfortable with building get super comfortable with say cloud code with all the cloud ecosystem that we learned today and get comfortable building and putting your ideas out there i think now is a time where building speaks a lot more and this is what i tell even my students when i teach aipm and agentic ai cohorts at next gen product manager where i tell them the way to transition now is by building and talking about the challenges that you have learned how you went about navigating those challenges and why did you choose this approach versus this other approach and what happened as a result and you can see a lot of companies now start putting even um uh cursor or cloud code prototype uh as part of the interview process itself

**Aakash Gupta** (01:15:43)

you just recently went through a very senior level aipm job search what was your experience on the job search what are the like if you were to try to describe as a pie chart the interviews you faced in the various categories what were they

**Jyothi Nookula** (01:15:58)

so broadly they're still around product sense like you saw here it's even more imperative now in this world of ai to have product sense to understand how do we want to tackle a problem how do we want to scope a problem which use a to go attempt how do you want approach it so the product principles stay true even now um and really strong product managers or an ai are actually really strong in their fundamentals as a pm so you have product sense, product analytics, behavioral interview but you also have an ai round as well now where you're asked to code your idea so like in product sense whatever idea i would have come up with they're like could you pull up cursor or your favorite ide and let's start coding and through the coding they are able to see how i think through like why did i choose this option versus this other option how am i navigating am I just taking the first thing that the AI tells me as like this is great and wrapping it up or am I looking through things to say okay this is good but what about this edge case this works well but what about this other instance how am I corralling and shepherding my AI to work with me to get it to where I want these are all the things that they are looking into in addition i also had a technical round where they test you on your ai knowledge like do you understand basic terminologies because you'll be working with machine learning researchers and scientists and you just don't want you you won't be able to communicate to them so you you are tested on fundamentals of ai as well not from a coding or engineering system design perspective but more around do you understand what that means as a pm and how does that impact your product for example

**Aakash Gupta** (01:18:02)

got it so how are adversarial agents looking

**Jyothi Nookula** (01:18:05)

so let's see it's built and here's the gan inspired architecture uh let's go and see you can see it's built a bunch of things um and so you can see it's went and built my red teamer designer it's built an agent.py my evaluator so here's where i can like give it my rubric okay so it's done a few things so let's see um as soon as i build so you can see i i wanted to kick off as soon as i build an agent i wanted to automatically go and do a red teaming and adversarial example on it so as soon as i build an agent i want to kick off my adversarial agent until end the feedback from my adversarial agent is passed back to my generator agent until it passes the criteria of my adversarial agent

**Aakash Gupta** (01:19:23)

so you're gonna send it off on essentially its own red teaming improvement loop

**Jyothi Nookula** (01:19:26)

yes yes

**Aakash Gupta** (01:19:28)

so is this the secret sauce

**Jyothi Nookula** (01:19:30)

yes um there's the the secret sauce is how the system has built and the second aspect is what am i asking it to test for what what are my configuration parameters and that's where domain knowledge becomes very important where you've got to say what is important or this what about these edge cases what about these use cases you can work with it and say here are three are there anything more but it's like making and building is easy now taste is what is important for us to develop what should that was real feedback iterate on something okay there are a couple of options for now i'm saying just iterate on the system prompt because that's the easiest uh right now and what's counts as passing and i'll say mean score of greater than eight on all criteria and how many iterations before giving up i'll say five iterations so let it do this and then we can test it out with a simple agent and see how it works

**Aakash Gupta** (01:20:27)

awesome and one of the cool features i guess is we could queue messages here so should we queue up our message for the test

**Jyothi Nookula** (01:20:34)

sure we can queue it up but i i want to see what it comes back with because sometimes if

**Aakash Gupta** (01:20:39)

i might have some questions for us that's the one downside of queuing okay

**Jyothi Nookula** (01:20:43)

and the other times as it would go and implement it in a way and you're like oh no no no no i don't want it that way i want it this way and

**Aakash Gupta** (01:20:50)

so we were talking about those ai rounds i think i heard like almost two different ai rounds that you encountered in the job search one was more like i want you to vibe code or prototype in this round and another was ai fundamentals for both of these how do you succeed and prepare in those interviews

**Jyothi Nookula** (01:21:07)

so it comes down to you understanding the basics um vibe coding is building right there's no shortcut to it just build um and i always say this don't build them as projects treat them as products like find problems in your area find problems that are finicky enough for you to want to go build a solution go build solution and see who else wants something like this have them come and use your product you have real users you have feedback coming and saying oh i don't like this i don't like that so that's like real user experience of iterating on your own product that you have built and that really gives you a lot of confidence when you talk about your projects to interviewers because you're not just like building something in an hour and calling it a project you've actually had to think through how the user experience should be you have real users giving you feedback you are you are parsing that through to figure out how you want to prioritize which one you want to tackle first which one you don't want to all the things that you do as a product manager in real world so i always say this don't build projects try to make your projects as products that tackles the wipe coding part

**Aakash Gupta** (01:22:27)

now preparing for your

**Jyothi Nookula** (01:22:30)

knowledge you can depends on how structured you want it and how you thrive so if you're really structured and you can do it everything by yourself there's tons of like very good information on your newsletter on youtube videos so go read them up and gain that knowledge or if you want something structured like like saying five weeks i want to like understand every um fundamental aspect of ai then come take a course where you have five weeks or cohort based courses i offer one too through next gen product manager so you can come sit and it's structured you know with someone teaching you week by week you know what's coming and by the end of five weeks you understand the concepts without you having to get overwhelmed so it really depends on your style how much time you have and how much you can dedicate

**Aakash Gupta** (01:23:32)

all right looks like the next round of gan output is here from cloud code

**Jyothi Nookula** (01:23:36)

yes so now it's good um you can see it's run it added a few examples here okay great so now i could literally say um it i could start or i let's say i don't know what i should do i could ask what is my next step here how do i test it okay so i have to set my api key and i could run a mini tiny smoke test first uh with the example and then i can i can inspect the output all right so yes so let me just set my api key for a second and stop sharing and then i'll share it okay so i added my api key and now i can um run a tiny smoke test so it's given me what I could run so I'm just going to copy this and actually just copy and if you notice I have a terminal that I use so you can just go to terminal and click on the terminal and open up a terminal for you so now I can run this command so you can see it is iterating you have it's using haiku clots on it it's going in the so you can see the first round it's tempting the bot into breaking.

**Jyothi Nookula** (01:24:54)

So this is like a simple bot that had built, so we could test. So you can say adversary is generating three attacks and here was the score trajectory there's a mean of mean scores 9 .13 years the final hardened system prompt so it's gone and edited the system this is your final system prompt but you could also like see examples where um i can say show me an example of where it will underperform so that i can see the iterator working

**Aakash Gupta** (01:25:47)

and

**Jyothi Nookula** (01:25:47)

improving the system prompt so in this case it passed in the first iteration but we can see if it can generate an example where we can try it to do it across multiple iterations let's create an agent which is a weak support bot let's see how it will do it there

**Aakash Gupta** (01:26:08)

so it's improving itself

**Jyothi Nookula** (01:26:10)

how do i run it give me the exact code as well that i can use to run so you can also run run it automatically for you by default so i can say run it for me so i don't even have to go to the terminal it can directly execute bash commands

**Aakash Gupta** (01:26:27)

so is this your preferred way to use it the cloud code extension in vs code is that the best way to use cloud code

**Jyothi Nookula** (01:26:33)

it's the least overwhelming way for folks so i really like to show this cursor is also another good one but if you have never used cursor there's lots going on that it could make you feel overwhelmed so i prefer to show vs code because it's like a really gentle introduction and doesn't overwhelm you much once you know how and where it is which i have already walked our users through so hopefully they are not overwhelmed

**Aakash Gupta** (01:26:59)

so we've been doing the cloud ecosystem and you mentioned like learning the cloud ecosystem is one of the most important things to becoming a builder pm compare and contrast the cloud ecosystem the open ai ecosystem i keep hearing like codex might be better than opus now at coding and the gemini google ecosystem

**Jyothi Nookula** (01:27:17)

so here's the thing the flavor of the month keeps changing um because all these models are getting really better um what i have found is rather than chasing behind the next big one i'm what i'm trying to improve is improving my productivity that's what if coming back to like first principles what's my goal is to improve my productivity and i have all the systems and connections right here for me to go leverage all the hooks and harnesses oh harness is a word i've used a couple of times i want to like break it down so previously you would have orchestration where your agent orchestrates across tools across different capabilities now being a being able to um provide the right capabilities like the memory or these uh evaluators or the various systems that your agent or your LLM orchestrator brain can interact with to enhance the experience and the output you receive is what is hardness engineering that's that's become very popular now especially as models have become better the context windows have improved are fairly large and so hardness engineering becomes more important what's something interesting that you have seen and how um your folks on your podcasts use um cloud how do you how do you use cloud

**Aakash Gupta** (01:29:07)

oh wow big question i mean i use it all day every day so one of the most interesting things that i've seen people do is set up their entire system as a self-improving product loop so they will have support tickets and bugs come in they have the pm agent that is triaging and understanding those then they have the pm agent understanding okay this is the future we want to build it even goes and does user research and creates the prototype itself that comes up with the prototype that works then they have their coding agents set up by their engineering team that code the feature then they have their analytics team agent that creates the right telemetry all of that goes to an engineer who reviews it once they pr review it actually ships and they have their own analytics agent that automatically is analyzing it and so they have like the entire product development life cycle built into clod and automated improving loop especially on like support related easy front-end changes that to me is probably been the most powerful thing i've seen recently

**Jyothi Nookula** (01:30:13)

yeah it's it just empowers you so much uh than before

**Aakash Gupta** (01:30:17)

yeah it's crazy it's not just like writing documents or you know doing analysis at this point it's like closing the loop with actually building

**Jyothi Nookula** (01:30:26)

this is where it takes time where it goes and tries to think through and comes back um so this is the piece with uh plot code that takes time whatever it comes with we can end with it and be like okay here's an example of how it iterated

**Aakash Gupta** (01:30:39)

perfect

**Jyothi Nookula** (01:30:40)

okay so it's come up it's done a few iterations so you see in first iteration it was it scored an 8.52 but the agent caved on some format conflict attacks so it didn't pass it went back to the generator agent to improve the prompt and then second iteration it scored a nine and in the third iteration is code 9.08 at which point it passed our threshold and so you can see for each iteration it went back and improved the system prompt until it passed the threshold and that's when the agent got a pass sign and so this is where you're not just building an agent you're actually building another evaluator to go break this agent in different ways that's important for you to know about or for your users that you care about and and this loop can continue until the agent that's built is not strong enough and that's the beauty of this technique age-old technique being applied for how agents will be evaluated

**Aakash Gupta** (01:31:57)

what a masterclass jyothi thank you so so much for walking us from layer one through layer five we have ended on self-improving agents for you guys as we promised we were going to take you from zero to eighty now the remaining eighty to one hundred you could spend 10 hours we just spent two hours a little less than two hours here today on it to go learn the later next 80 to 100 and that's on you so no more watching we have the github repo down in the description below go check that out go fork the repo start to use some of these skills and go win your hackathon i hope you enjoyed that episode if you could take a moment to double check that you have followed on apple and spotify podcasts subscribed on youtube left a rating a review on apple or spotify and commented on youtube all these things will help the algorithm distribute the show to more and more people as we distribute the show to more people we can grow the show improve the quality of the content and the production to get you better insights to stay ahead in your career finally do check out my bundle at bundled .akashg .com to get access to nine ai products for an entire year for free this includes dovetail mobbin linear reforge build descript and many other amazing tools that will help you as an ai product manager or builder succeed i'll see you in the next episode
