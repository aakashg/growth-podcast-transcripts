---
title: "How to Do AI-Powered Discovery (Step-by-Step with Live Demo) | Caitlin Sullivan"
subtitle: "The exact workflow a UXR expert uses to analyze surveys and interviews plus how to build agents that do it for you."
date: "2026-02-13"
host: "Aakash Gupta"
guests: ["Live Demo"]
speaker_names: "inferred"
substack_url: "https://www.news.aakashg.com/p/caitlin-sullivan-podcast"
youtube_url: "https://www.youtube.com/watch?v=rzAGo_XML1U"
duration: "01:12:40"
word_count: 13353
source: "Substack episode transcript (aired audio)"
---

# How to Do AI-Powered Discovery (Step-by-Step with Live Demo) | Caitlin Sullivan

*The exact workflow a UXR expert uses to analyze surveys and interviews plus how to build agents that do it for you.*

**Aakash Gupta** (00:00:00)

AI for user research is mess. It's unreliable. But what if I told you I know how to fix

**Live Demo** (00:00:05)

it? There's a real art to doing this right. But if you do it the right way, then AI actually isn't going to hallucinate on you. And you're going to cut your analysis time in half. The key is actually replicating the way that you would do things in a rigorous way as a human and just doing it like that and with AI.

**Aakash Gupta** (00:00:20)

This is Caitlin Sullivan, one of the world's leading experts in user research. And in today's episode, she's going to give you all the tools, the demos, the workflow, so that you can do amazing user discovery and customer research enabled with AI. These results genuinely shock. What does good AI customer research and analysis actually look like?

**Live Demo** (00:00:40)

So I think there's actually a really simple answer, which is it looks like replicating the way that we do rigorous analysis as humans. You've

**Aakash Gupta** (00:00:49)

chosen Claude. If people have the option to choose between all the AI models, why have you chosen Claude?

**Live Demo** (00:00:54)

I keep coming back to Claude because by default, it does a more thorough, more nuanced analysis than the other two platforms. And then

**Aakash Gupta** (00:01:03)

there's two big types of analysis that people tend to run, surveys and interviews. What are we going to do today on the surveys from?

**Live Demo** (00:01:10)

I'm gonna demo how you can use any of the large language models to run a few key steps that I just talked about to get really solid results. Wow, that's insane.

**Aakash Gupta** (00:01:22)

Before we go any further, do me a favor and check that you are subscribed on YouTube and following on Apple and Spotify podcasts. And if you want to get access to amazing AI tools, check out my bundle. where if you become an anal subscriber to my newsletter, you get a full year free of the paid plans of Mobbin, Arise, RelayApp, Dovetail, Linear, Magic Patterns, DeepSky, Reforge Build, Descript, and Speechify. So be sure to check that out at bundle.akashji.com. And now into today's episode. Quick note for my audio listeners, there are some things that we showed, which you can see on Spotify or YouTube, but we've edited this audio so that it's a really good listening experience nonetheless. Caitlin, welcome to the podcast.

**Live Demo** (00:02:06)

Hey, Akash. Thanks for having me.

**Aakash Gupta** (00:02:08)

What does good AI customer research and analysis actually look like?

**Live Demo** (00:02:14)

So I think there's actually a really simple answer, which is it looks like replicating the way that we do rigorous analysis as humans. I'm not reinventing the wheel with pretty much anything I do. I have just taken what I know to be true, doing really solid research as an individual contributor, as the head of user research, and replicating those processes with AI.

**Aakash Gupta** (00:02:41)

Amazing. So let's break this down for people in terms of what the actual tasks are and what the actual tools are.

**Live Demo** (00:02:50)

So analysis actually looks fairly similar, whether you're analyzing interview transcripts or survey responses or other kinds of short customer feedback. We're going to use a similar set of kind of phases of analysis across all of them. So good analysis, rigorous analysis with AI or as an individual, as a human doing it is going to involve analysis. Actual analysis where you dig through data and you pick it apart. You look at what's in there closely, put it back together in different ways and see what pops at you. And then verification or stress testing, basically seeing how the findings you have hold up under pressure and then finally synthesizing. But what most people do both as humans and also especially with AI is jumping straight ahead to synthesis. And that's exactly what we don't want to do.

**Aakash Gupta** (00:03:44)

And then there's two big types of analysis that people tend to run, surveys and interviews. What are we going to do today on the surveys, Frog?

**Live Demo** (00:03:53)

I'm going to demo how you can use any of the large language models to run a few kind of key steps that I just talked about to get really solid results out of any analysis that you do with surveys or short customer feedback. And I'm going to do that in Claude in the normal web UI, but you can replicate this process in Chachabuti or Gemini. I do that all the time as well.

**Aakash Gupta** (00:04:16)

Awesome. And then we're going to show you everything here in blue. So we're going to cover the cloud analysis process, but also show you the agentic version with the chat GPT codecs. You could use other tools like Zapier, N8N. And are people using those frequently in the fields? Yeah.

**Live Demo** (00:04:36)

So I'm going to do the agentic part in Claude code in my terminal, actually. But yeah, people are using the other tools. The agentic, the more advanced agentic tools, I would say, are not commonly used by most of my clients. But what a lot of people are already doing, because it's kind of a more familiar space, is automating a lot of these processes rather than making them fully agentic. So you can use N8N, Zapier, Make.com, Any of these automation tools to link up with your chosen large language model and sort of put some of these prompts in place to happen automatically for you.

**Aakash Gupta** (00:05:15)

Awesome. And then the other side, of course, everybody knows our interviews. And so there are the human moderated side of interviews. What are we going to cover for people there?

**Live Demo** (00:05:25)

I'm going to basically replicate the same sort of process across survey analysis and interview analysis. What's worth knowing for interview analysis is that things can get really complicated really fast. AI is built to understand structured information best. So with really long transcripts and sometimes messy transcripts where speaker labels aren't particularly good, We can run into a lot of problems with AI. So I want to show you how being systematic in terms of the sequence of prompts we use and the types of prompts we use can actually ensure that you get much better results, even when we're dealing with a tougher space like interview transcripts.

**Aakash Gupta** (00:06:07)

Awesome. So we're going to use transcripts for ChatGPT and Claude. If you had a video that is actually possible now with Gemini 3, we're not going to demo that, but that is something to keep in mind. And then the agentic version will show you guys how to do that in Claude code and do that in parallel with the survey analysis. Now, a lot of people have been talking about AI moderated surveys. So can you just talk to us about what these are, what the tools are, and how you might use these?

**Live Demo** (00:06:36)

So there are already a lot of AI moderation tools on the market. There's a huge list of them. They are tools that run sessions with customers for you. So the idea is sort of that you can scale your team's ability to talk to customers by having all of these sessions run when you're sleeping or making your coffee or spending time with your family instead of having to line up, you know, 15 people to talk to every day. So... As we've talked about before the recording started, there has been a little bit of discussion this past week where Claude, the team behind Claude, Anthropic, launched their own study where they're using an AI moderation tool of their own that has surprised some people in our space today. in terms of the quality of the questions that were being asked. So this space is a little bit tricky.

**Live Demo** (00:07:27)

There's a huge range of quality between the different AI moderation tools, to be honest. Some of them are asking really, really good questions and handling bias, not asking leading questions, and also doing decent analysis after collecting data. Some of them are not quite there yet. And I've seen the questions that Claude was asking in the Anthropic Team study, and I also wasn't particularly impressed.

**Aakash Gupta** (00:07:51)

Mm-hmm. Even Anthropics interviewer couldn't do a good job, right? And so you want to think about this as a skill that you're going to continue to improve throughout your career. We could cover it all, but we don't think the AI interviewers are quite the most important thing for you to learn. So we're going to cover what's in blue for you guys, how to analyze surveys, how to analyze interviews. So without further ado, can you get us started, Caitlin?

**Live Demo** (00:08:33)

Yeah. Okay. So as I said, we have to go through multiple steps in the analysis process to get something really rigorous and reliable out. And I mentioned that we have to start with kind of picking apart the pieces of the data before we do synthesis, which is unfortunately what most people don't do. Most people jump straight to synthesis. Yeah. Another piece of the puzzle here is, of course, giving Claude or any of these large language models enough context that it can do a really good job for us. And I know that this metaphor is really overused at this point of saying that it's like your junior assistant or something. I prefer to think of these models at this point not as juniors, but like someone who's new to your team. So if someone new joined your team, they don't necessarily have no skill in this space, but they don't really have the expertise in the domain or about your customers that you have.

**Live Demo** (00:09:28)

They might not even know exactly what kind of feature functionality you have built in if they haven't been fully onboarded. So the first step that I use in a lot of, especially interview analysis, is just loading context. And I make this an individual prompt rather than building it into anything else, because large language models actually can be a little bit overloaded. If you try to paste a two-page long prompt in one go, a lot of the models will still have trouble handling that. And you'll see that they drop some of the instructions, even if you said, this is really important. So I'm just going to copy my first prompt here, which is only about context.

<!-- sponsor -->
**Aakash Gupta** (00:10:08)

If you're enjoying this masterclass in AI analysis, you will love Caitlin's cohort-based course. This runs for the month of March, where Caitlin will walk you through not just these first-level workflows that we've shown here, but the next layer deeper of complex workflows. The agent markdown files, everything you need. She will help you get to the next level of craft using AI for discovery and user research. For my money, it's one of the most important skills for PMs, but not just PMs, designers, engineers, go-to-market people, and obviously user researchers. So if you enjoy what she's saying now, take her course. You will learn even more. She'll walk through all of this in detail. And the best thing is you can get a discount on the course using my code, link in the show notes. So check her course out and back to today's episode. Today's podcast is brought to you by Pendo, the leading software experience management platform.

**Aakash Gupta** (00:10:56)

McKinsey found that 78% of companies are using Gen AI, but just as many have reported no bottom line improvements. So how do you know if your AI agents are actually working? Are they giving users the wrong answers, creating more work instead of less, improving retention, or hurting it? When your software data and AI data are disconnected, you can't answer these questions. But when you bring all your usage data together in one place, you can see what users do, before, during, and after they use AI. Showing you when agents work, how they help you grow, and when to prioritize on your roadmap. Pendo Agent Analytics is the only solution built to do this for product teams. Start measuring your AI's performance with Agent Analytics at pendo.io slash akash. That's p-e-n-d-o dot i-o slash a-a-k-a-s-h. And obviously you've chosen Claude. If people have the option to choose between all the AI models, why have you chosen Claude?

**Live Demo** (00:11:47)

I've chosen Claude. It's my favorite. It has been for a long time. And I keep checking myself on that, doing tests across the three major ones, meaning Gemini, Claude and Chachubiti. And I keep coming back to Claude because by default, it does a more thorough, more nuanced analysis than the other two platforms. I will say, though, I do like Gemini quite a lot because it's It seems to be fine-tuned a bit more for accuracy and focusing on frequency of findings. So you're more likely to get kind of a top five themes or patterns from Gemini really quickly that are solidly evidenced than you will in Claude or Chachupiti, just because that's kind of what it lifts up. But you'll have to push Gemini more than you have to push Claude to give you the complete picture and all of the smaller themes or the outliers and things like that.

**Aakash Gupta** (00:12:42)

Okay. Excited to see how Khan does.

**Live Demo** (00:12:44)

So I'm with my context prompt here. I'm just going to get all of my files ready here. I'm just dragging them over. And I want to quickly point out as I send this context prompt that I'm using Markdown files. And this is important because... In Claude, if you don't have a Max account like I'm using right now, if you have Pro even, you've probably experienced uploading a bunch of transcripts and hitting this token wall. Even though Claude's token limits have been expanding and expanding and, you know, it can handle a lot more at once now, you can kind of circumvent that issue by transforming your interview transcripts into Markdown files. But this is something that I teach in my course because you have to do it right. You have to do it in a way that really keeps, maintains all of the most important information from those transcripts and carries them over into Markdown files.

**Live Demo** (00:13:39)

But what you get out of a Markdown file instead of just using the transcript is you've turned it into a format that's more structured than the original transcript is, which means that it's not just better for file handling. It actually helps these models do a more accurate job as well.

**Aakash Gupta** (00:13:55)

Love it. And just the high level, like what is that transformation into Markdown look like? What do people need to focus on?

**Live Demo** (00:14:02)

You're basically telling it to take certain types of information and it's not going to take everything from the transcript. There's a lot of bloat in your transcripts. Not every conversation necessarily needs to be carried over. Some people will argue with that. But for especially for a lot of the sort of product research that I've done, you have a specific focus. You're not always doing exploratory research. So you can usually have a large language model with you comb through a transcript and extract. the right kinds of information that are most relevant to the topic areas you're exploring or the hypotheses you have and turn that into a document that already has tagging or groupings of conversations under certain headers and things like that, putting in metadata, a little bit of extra coding that makes it easier for the model to make sense of it.

**Aakash Gupta** (00:14:54)

And then how would you break down this context prompt? What are the key elements here?

**Live Demo** (00:14:58)

So it looks like a lot at first glance, I realize, because some people share a half of this or a third of this within a prompt with actual tasks. But I would call out what's most important here is I do have a bit of project context. I have a business goal, reduced churn. The percentage is kind of arguable here, though I would say in my experience saying 15% versus 50%, like 5-0, will make a difference. And then I have product context. So just like I was saying about onboarding this new team member, I want to make sure that it fully understands what kind of functionality is involved in the service that we offer, what the differences are between the product tiers so that in its context, reading through of people's experiences or comments about the product, what they're using, it fully understands what kind of functionality would actually be present and what they would be using when they have that experience.

**Live Demo** (00:15:54)

Otherwise, if we don't include something like this, I've seen huge, hugely wrong guesses, you know, gross... assumptions by large language models about what someone has as part of their account, kind of making things up or just trying to piece together bits of information it had that were entirely wrong.

**Aakash Gupta** (00:16:15)

Point it in the right direction of what your product is actually doing in that case. Exactly. Yeah.

**Live Demo** (00:16:21)

What's important here, though, is I said that for a context prompt, we actually are just loading context. So at the end, I said internalizes only do not run analysis yet. It's really important that you don't let it jump ahead and start doing tasks because I haven't given any instructions here for how to do analysis. So it hasn't done analysis yet. I'm just going to jump to the next prompt and send that now.

**Aakash Gupta** (00:16:44)

I think this is a really cool lesson for people. I don't think many people have done this two-step prompting, right? Yeah. First step. Context. Second step analysis. Most people try to shove it into one prompt.

**Live Demo** (00:17:00)

Exactly. But this will get you much better results. I mean, it will basically help the large language model focus on one thing at a time, which means that each individual step will be done more thoroughly.

**Aakash Gupta** (00:17:10)

Mm-hmm.

**Live Demo** (00:17:14)

So let me start working on it on this step so that I can talk through it at the same time because it will take a minute. What's really important here is I've started analysis, but I'm not saying, hey, go find me some themes and patterns. So what I said earlier about starting rigorous analysis means doing actual analysis and not synthesis. It actually means that we need to tell it to go look at every single file that I just uploaded. I'm basically asking it to pull out for each participant value anchors. And I'm telling it that means what's keeping them subscribed. And then fragile points here. The formatting is a little wonky. What frustrations exist despite subscription. And I'm spelling things out in detail. So where I say I want it to give ratings, right, like how strong, how big a deal is this? How how strong a fragile point is this?

**Live Demo** (00:18:05)

I'm explaining what a high fragile point means, like what is a high rating? So I'm not letting it make any assumptions here. I'm trying to be pretty explicit in every case about how I would rate things. I've also started this prompt with quote selection rules, which seems a little funny because I think most people just assume large language models know what a quote looks like. But if you prompt in Gemini and then you prompt in Claude, you will see that they interpret quotes completely differently. So Gemini will give you much shorter snippets. Gemini will give you much shorter snippets of customer statements. And Claude will give you, you know, a longer sentence or even a short passage. So I like to, you know, avoid making the assumption that Claude in this case has the same understanding of quotes that I do. And I spell out what a quote looks like to me.

**Aakash Gupta** (00:18:58)

Very interesting. Yeah, I've also noticed that sometimes the AI will... like you've had here, take away some of the hedges and qualifiers. It'll try to like clean up the quote as if it were cleaning it up for a news article. But in user research case, we don't want to clean up the quote. So we're giving that instruction to the AI.

**Live Demo** (00:19:17)

Yeah. And in that case, you could even line, add a line here that says something like leave ums, uhs, pauses, um, you know, fumbled language, things like that. I sometimes include that in here too, to keep things exactly as they are with the customer's voice.

**Aakash Gupta** (00:19:33)

And can you define some of these words for me? Because I'm not totally familiar with them. Or I can imagine a lot of the audience is trying to guess at exactly what they mean. Value anchors, fragile points, stability rating. What are those? Those seem like cool terms of art in the user research discipline people could benefit from learning.

**Live Demo** (00:19:49)

Let me give you a background quickly about the data I'm using here, too. So I have eight interview transcripts from a synthetic user study that I created based on a study that I actually ran. And it's all about improving retention and decreasing churn. So these are all people who had a premium tier account on a fictional app called Flow that is a meditation and anxiety management app that also has on-demand therapy. And so what I'm doing here is I'm trying to figure out, I'm doing a bit of a retention analysis where I'm trying to figure out what's keeping people subscribed, and then what's likely to break their experience. So what frustrations exist despite subscription basically means the flip side of the things they're finding really valuable about the service, what could actually push them to cancel anyway. And I want to collect both sides of that because I'm not assuming that when someone is super happy, they're just happy.

**Live Demo** (00:20:50)

No one is so one dimensional as that as a customer or as a human being. So I want to know, OK, if they're happy about using the service and they continue to pay, that's great. But what would cause them to turn anyway if it continued or increased over time?

**Aakash Gupta** (00:21:05)

Makes sense.

**Live Demo** (00:21:06)

So we have some results here and I've told it to put this into a table. So it followed my instructions really well. Basically, this looks like, you know, the value anchors are in a table here for participant one. This is by participants. So this is the first participant here. Value anchors, then fragile points. And then I also ask for a stability rating. So overall, how risky or how much risk is there that this person will churn? And then I have a few key themes that I asked it to call out to. And then we start participant two. And it just looks like that for every participant. So what I said earlier about making sure we actually pick through the data and kind of look at it closely first is what I've forced the large language model to do here. But if you jump to asking for themes, patterns, pain points, whatever it is, you're actually forcing it to jump into like synthesis mode instead of real analysis picking through the data mode.

**Live Demo** (00:22:03)

So I usually start with something like this where I force it to look at every file and kind of look for specific pieces of information so that it actually comes through properly.

**Aakash Gupta** (00:22:13)

And that's replicating the human process. That was the high level advice you knew this at the beginning, which is we are always going to analyze the specific interviews. So let's not have the AI jump that step. Let's have it analyze those first.

**Live Demo** (00:22:25)

Exactly. So as a very experienced user researcher, you always comb through, you know, we used to just sit with one interview transcript and look through it manually, every line, copying, pasting into Miro or sticky notes or whatever. And so I'm basically replicating that process here.

**Aakash Gupta** (00:22:44)

Awesome.

**Live Demo** (00:22:46)

So the kind of information that we get here is going to be much more granular, much more specific. It hasn't really, other than this bottom section here, it's not mapping things into themes. It's really just picking up the foundational elements that a really good analysis will be built on. So we have things like this full passage passage. about someone who is doing breathing exercises with this app every day, usually between meetings and so on, all of the things that she's using. And so the strength of this in terms of stickiness with the product is strong because there is daily integration into the work routine, multiple features used regularly, and so on. Let me see what else is there. It's... maybe more than what she expected because she thought it would just be meditation, but it's become this whole system for managing my new role. So dealing with stress at work is kind of now dependent on this app.

**Live Demo** (00:23:39)

That's a good sign. And then the therapy sessions can be booked spontaneously. I don't love that this means I won't always talk to the same person. So there's something interesting there. It's labeled this as moderate. I would almost say, okay, well, the You know, this is where my perspective comes in because I don't just have AI do analysis without thinking about it myself. But this seems very positive and the rest is starting to get a little bit more into the fragile points. So this is the sort of thing that I want to be pulled out because if I were doing this as a researcher, I would be pulling out all of these quotes myself and then trying to categorize them, label them, give them ratings and so on. So this is really what it looks like to do good analysis, whether you're doing it with AI or not, but it's doing it much faster for me.

**Aakash Gupta** (00:24:22)

And there are a lot of tools that I think help with this. When I was at a firm, we used a tool called Dovetail. What is your take on some of those tools and which ones do you like?

**Live Demo** (00:24:32)

So I use a few that are less talked about. The two that I've continued to return to because I think they're doing a particularly good job are Breda.ai. I can send you that for the show notes. And Reveal, they have completely different approaches. And I think there's so many different tools out there that really do things just very differently than each other. So it's hard to compare them all kind of apples to apples. But Breda is... Getting to a pretty good nuanced level of analysis fast because they have really good prompting in the back end and reveal maps the customer comments in a bit of a grid and does a bit of hypothesis testing for you. So it lays things out in a way that you, you know, kind of like this. I'm almost mimicking what they do as well. being able to see things yourself and make your own comparisons in Reveal versus just having a finished analysis for you.

**Live Demo** (00:25:30)

Dovetail, I honestly hear mixed reviews about from researchers especially, and I have had mixed experiences with it. So I haven't tested it in about five months, so I wouldn't dare to kind of give it a final rating right now. But a tool like that is really meant to get you to insights as fast as possible. But you don't have control in any of these platforms over exactly what you're looking for and exactly the type of analysis that you want it to do. So I tend to stick to the large language models for the most part, unless the time to insight is so extreme that I, you know, feel better uploading things into a platform and having it do that for me. But it's rare.

**Aakash Gupta** (00:26:14)

So the platform is going to take some of this control that we're getting from these prompts, from this step-by-step prompting process out of your hands. Yeah. That's the power of this workflow. We're kind of showing you guys the advanced. This is what an advanced user researcher would do. Yeah.

**Live Demo** (00:26:29)

And obviously, the teams behind all of those tools have worked tirelessly on those prompts. They've also worked with the team at Maze to kind of develop the prompts behind their AI analysis and AI moderation. So I know what it looks like behind the scenes, and they're all working very hard to kind of figure out the right prompting sequences to do this for you. But I prefer as someone who's used to doing research, especially I prefer to have more control over the granularity in the analysis or focusing it on a retention analysis in a certain way and so on over using a tool to do it for me.

**Aakash Gupta** (00:27:02)

Makes sense. So is there a step three now? There

**Live Demo** (00:27:06)

is

**Aakash Gupta** (00:27:06)

a step

**Live Demo** (00:27:06)

three.

**Aakash Gupta** (00:27:07)

So I had said two step before, but it's actually a three step prompting process.

**Live Demo** (00:27:11)

It's three step here, and I would say it's four if synthesis is added. So the context is almost like a step zero, I would say. You kind of just load the background information. So I would call this three steps in this workflow, which is condensed compared to what I usually do. So for the most rigorous possible version of this, you have more steps because you need more feedback loops with AI. But you'll see one version of this here. Let me just space this out so people can see this more easily. Just going to let it do its thing while I talk. So this is what I referred to earlier as a stress testing or verification step. We need this because even if you think everything looks really good, which, you know, most people go, oh, AI did this analysis for me and it looks really solid.

**Live Demo** (00:28:06)

It's usually not as solid as you think it is. And what happens down the line is then a product manager or a designer or researcher presents some findings in a meeting and then can't trace them back or realizes there are actually lots of holes in this insight or set of insights. But if you push your model through an additional step for verification, or I usually call this some kind of audit step, then it very often catches its own mistakes. And I get questions all the time from people who are really rigorous or kind of know that these models have a lot of bias built in. They ask me, yeah, but how is it going to critique its own work, you know, its bias toward its own work? The truth is they do find mistakes. They find mistakes all the time. And I've tried this kind of splitting the process between tools too, but this actually using it in the same model that you're doing analysis in does find issues.

**Live Demo** (00:29:04)

So let's see if it found some things. So yeah. Yeah. So in this particular prompt, actually, let me bring this back up again. This version of a verification check, I'm asking for contradictions in user statements. So it's very common that one person in a transcript will be telling a story one way, like they say, well, first I got my shopping cart when I was going grocery shopping, and then I looked for the apples or whatever, in a certain order. The second time around, in a different part of the conversation, they tell the story of the user journey in a completely different order. Or they contradict whatever they said earlier in some way. Well, you know, I use this every day. The equivalent of like, I go to the gym every day or five times a week and then, well, when was the last time you went to the gym?

**Live Demo** (00:29:52)

Oh, well, it was probably Saturday and it's Wednesday today, right? So... Very often, if you're doing a good interview, you find some contradictions in what someone does and says or what someone said the first time around and then what they said the second time around. But AI is very likely to blur that, kind of cherry pick the stories that it likes or that match what you asked for most closely and forget about or ignore the second thing they said that is actually the opposite. Yeah. So I'm putting it through this pass where I'm checking for contradictions, and that will make the full analysis in the end much more bulletproof, kind of preventing the cherry picking of the story that best aligns and getting the full picture. So to spare you the details, I think people can look at this on the screen, stop the video if they want to.

**Live Demo** (00:30:42)

But I'm basically asking for contradictions and I'm defining what contradictions look like to me. I've even spelled out what is not a contradiction and a few examples. So I'm consistently giving examples, definitions, and then what that looks like to me to be really, really clear. And just so you see a few contradictions here. So something was revised. The rating was revised from, let's see, original. No, this is confirmed. Sorry. This one is moderate risk in the first place, like at risk of churning. And then it was revised to high risk. So upgraded because it double checked what the person was saying, the stories they were telling and actually realized that there's more risk involved. So this is the sort of correction that I'm looking for. I want to make sure that it has combed through the data again, made sure that the claims, the statements that it made were actually

**Aakash Gupta** (00:31:38)

verified. You know what kills momentum? Spending 30 minutes on a brainstorm with Claude and then copy pasting it into a slide tool to create the slides. That loop is dead. Gamma now works inside Claude through Claude Connectors. So you can go from thinking to a finished presentation without ever leaving the conversation. Here's what that actually looks like. You're brainstorming a product strategy in Claude. Mid conversation, you say, turn this into a deck. Gamma generates it right there. You keep refining your thinking and the presentation updates with you. No copying, no pasting, no starting over in another tool. And it gets better. Connect Gmail, Notion, or GitHub alongside Gamma, and Claude will use those connections to pull live data straight into your slides. Weekly business reviews, feature PRDs, all generated from the data you're already using. Your deck finally keeps up with your ideas. Try it now.

<!-- sponsor -->
**Aakash Gupta** (00:32:23)

Connect Gamma to Claude at gamma.app. Go from thinking to presenting in one flow. Claude helps you think, Gamma helps you show it. Today's episode is brought to you by the experimentation platform Chameleon. 9 out of 10 companies that see themselves as industry leaders and expect to grow this year say experimentation is critical to their business. But most companies still fail at it. Why? Because most experiments require too much developer involvement. Chameleon handles experimentation differently. It enables product and growth teams to create and test prototypes in minutes with prompt-based experimentation. You describe what you want, Chameleon builds a variation of your webpage, lets you target a cohort of users, choose KPIs, and runs the experiment for you. Prompt-based experimentation makes what used to take days of developer time turn into minutes. Try prompt-based experimentation on your own web apps. Visit chameleon.com slash prompt to join the waitlist.

<!-- sponsor -->
**Aakash Gupta** (00:33:16)

That's K-A-M-E-L-E-O-O-N dot com slash prompt. today's episode is brought to you by amplitude replays of mobile user engagement are critical to building better products and experiences but many session replay tools don't capture the full picture some tools take screenshots every second leading to choppy replays and high storage costs from enormous capture sizes others use wireframes but key moments go missing creating gaps in your understanding Neither approach gives you a truly mobile experience. Amplitude does things differently. Their mobile replays capture the full experience. Every tap, every scroll, and every gesture with no lag and no performance hit. It's the most accurate way to understand mobile behavior. See the full story with Amplitude. So this is how we increase the certainty that it hasn't hallucinated and it's giving us the right analysis based on the quotes.

**Live Demo** (00:34:08)

Exactly. So it's a bit of an analysis check in the first place. It's also an exaggeration check in some cases. You can run an audit to make sure that you're staying as close to the data as possible, that no statements were made by AI in the process that are a bit over or under exaggerated. So you can use it for lots of different things. This is just one version of it.

**Aakash Gupta** (00:34:32)

Excited to see where we go from here.

**Live Demo** (00:34:34)

So I would end this process for this kind of very condensed workflow version with synthesis. I think if it's okay with you, I would just skip a synthesis step because I think most people know how to do synthesis. Most people would just say, summarize this or give me the key themes, the top three action items, that sort of thing. And I would hop into survey analysis. Does that work? Let's do it. Okay. Okay. So let me open a new window.

**Aakash Gupta** (00:35:02)

The key takeaway here, what we did is we didn't jump into synthesis. We did this, whatever you want to call it, two, three, four step process to make sure that we increase the certainty in the results, in the quality of the analysis and replicate the human process.

**Live Demo** (00:35:15)

Exactly. So this is what I'm dealing with here. This is a very basic churn survey, but pretty similar to what I've ended up working with in the past. We've got some automatically logged information. We've got a call in like reason text where the The customer chose a category from a dropdown and these are a lot of other categories. So this isn't particularly well organized in the first place. Then we have reasoned detailed text. And this was an open text field where people could just say something about why they were canceling. Pretty basic. And then we have what tier of service they were on at the end. So that's the file that I will be uploading now.

**Aakash Gupta** (00:35:55)

Like what all of you guys have.

**Live Demo** (00:35:56)

So let me get my file in here. Just dragging it over. And what most people would do here is similar to what I said before, kind of toss in a CSV file, say, show me the biggest pain points from the column with the open responses or count all response types in this other column where, you know, we had the type of cancellation logged. But that's actually not what I want to do here. Because a lot can go wrong if you start there. Similarly to the interviews, just jumping into pattern finding, a lot can go wrong, a lot can be missed, and a lot can be miscategorized. So when we're working with survey responses or short customer feedback, we want to code first.

**Aakash Gupta** (00:36:42)

And for people who don't know, what does coding mean? It's not software engineering.

**Live Demo** (00:36:46)

No, definitely not. I'm not a particularly technical person, so definitely not that type of coding. We're talking about applying labels to things, putting things in buckets that help us make sense of them. So normally, if you're doing data analysis, you're looking at all of these responses and there is an open text response field like... customer feedback form or feature request form, that sort of thing. You have to kind of make sense of what people are talking about in those message fields, in those message responses, and label them with something before you can start grouping and saying, well, most people complain about this or most people are requesting this. That coding needs to have an approach, right? You need a bit of a methodology for the coding in the first place. You can do inductive coding where you look at the data available and you try to make sense of it from what's there.

**Live Demo** (00:37:38)

Or you can do deductive coding when you already have a taxonomy. you already have parts of the product and you want to, you know, label all of your data with those features or customer types or things like that. So you might already have something that you like to use as labeling. But in this case, I'm using inductive open coding, where I'm saying let themes emerge from the data rather than forcing preset categories. And what's important about this, I very often use inductive coding, at least at first, Because I let AI try to see what I may not have noticed about the data and apply codes from a more open perspective first. If you just apply your own tags and say, here's the list of tags I want you to code this with, what very often happens is it will start force fitting things. It will take the quotes that it sees and try to make them make sense in the set of kind of required buckets that you gave it.

**Live Demo** (00:38:37)

And that doesn't lead to the most accurate coding and analysis.

**Aakash Gupta** (00:38:42)

Makes sense. This goes back to that craftsmanship of research that you want to be applying. And so we have this first step here where we code.

**Live Demo** (00:38:49)

And I'm going to let it start working because it will take a couple of minutes on this. But I also have rules here. So I'm not just saying go ahead and code this however you want, you know, be open, find some interesting things for me. I'm also saying each response needs one primary code. They need to be mutually exclusive, not overlapping. I want really tidy little boxes. I want all of the quotes to be in one box categorized, right, in a way that I can make sense of later, not having too many kind of messy overlapping things. This is really up to the person doing the analysis with AI. You could, you know, anyone watching could decide you would take a completely different approach and that's fine. But what's most important here is just that there are rules, that there are criteria, that there are kind of lines that we need AI to paint within.

**Live Demo** (00:39:35)

We don't just kind of let it run this however it feels like running it.

**Aakash Gupta** (00:39:38)

Yeah.

**Live Demo** (00:39:39)

And one last thing while it's still working on this, most likely, yep. I finish with a line that is maybe becoming obsolete, but not quite yet. I've always included this as a bit of a fail safe. In the past, all of the models have made mistakes with math calculations. And a lot of the time, the calculations on a data set like this come from sometimes running tasks with math in text instead of in code. which is a really goofy thing because we know that all of these tools have been coding for many, many months at this point. But if, you know, they are originally text-based machines. And so I've seen so many cases in my students' projects that they've submitted and in my own work of saying, you know, calculate how many people said this and then seeing that the answer is different if you prompt it three times because it doesn't do it in an actual math equation.

**Aakash Gupta** (00:40:30)

Mm-hmm. Yeah, it's they're notoriously bad at math unless you tell them code, use coding for.

**Live Demo** (00:40:36)

Yeah. So I'm hoping I can remove that in my latest tests with all the models. I, you know, got really consistent results without having that in as well. But I still am a little anxious about taking it out. So I just leave it in all of my prompts. It's better, better safe than sorry.

**Aakash Gupta** (00:40:52)

Good takeaway for anybody watching. If you want to be safe on your math, tell it to code it. What I love about Quad these days is how much of the thinking is exposed and how much planning it's doing and how much step-by-step and how you can even click into some of those and just watch it work. I find myself just like getting fascinated with this and getting better at coding and stuff like that by doing that.

**Live Demo** (00:41:12)

Yeah. And you don't really need to be a Python expert here to just see, you know, how it's thinking through things like team specific issues. It's already kind of providing an overarching code group here, invoice reimbursement, primary, primarily a team issue. And then, you know, logging, if you find any of these terms, then code it like that, right? So this is how it's thinking through, I found these topics, and this is how I'm going to start coding them.

**Aakash Gupta** (00:41:38)

seem to have brought a lot of the cloud code functionality into the cloud user interface so if people have just been stuck in cloud code the user interface version has gotten quite a bit better in the last couple months people are curious it's almost always going to import pandas which is like a really common data science library so you as you watch this think and learn you get to learn a little bit more deeply too yeah exactly and so if you were doing this as a human what would have been the process

**Live Demo** (00:42:02)

More or less the same. I mean, again, what I'm showing you is a bit of a condensed process compared to what I would usually do. I have more steps involved. So one way I might have done this as a human or with AI as well is actually to break this prompt into multiple steps. So human-wise, right, I would be reading all of the responses. If we didn't have a code book already, if we didn't have a taxonomy or a set of tags that we wanted to apply, and we really were doing this... from inductive open coding. I would read through all the data or, you know, a sample of it at least and start coming up with the labels that I think most apply from what I see. So that's this creating a code book. Like, what are the labels that I'm identifying the codes? Why do I think that they should exist?

**Live Demo** (00:42:47)

What's the definition of them? How would we know if something else should fit into this group or not? Giving some examples. And then applying that code to other responses. You could even say in between these two, there's a step of testing it, like taking another sample from the data set and checking do these codes that I just came up with actually apply to this new sample or am I missing something, right? Mm-hmm. You're doing this kind of chunk, look at it, create codes, apply it to the next chunk. Did that fit? Yes or no? Okay, iterate, keep going. And this is really how I would have done things manually as well. So I've just laid out the steps that I would follow and I've given them to Claude. But here then is where things do get a little bit better if you have a slightly more complex, stretched out process where...

**Live Demo** (00:43:34)

You separate these steps into individual prompts, like first going through the data and thinking about what the codebook might be. And then I could give it another set of data and say, do they still fit for this, for example, and so on.

**Aakash Gupta** (00:43:48)

Nice. Okay. And it looks like it's got a response for us.

**Live Demo** (00:43:50)

It's got a response. I'm going to close this version because it has things down here, hopefully. Yeah, it's still generating. So dominant turn driver is clear, 23.5%. What I actually am more interested in is this. So there's some quantification. I want to see the code. Let me see. Usually it gets me a code book.

**Aakash Gupta** (00:44:10)

This is already so much more than I would have done as a PM. This is cool.

**Live Demo** (00:44:14)

So you've got a bit of the code book in here. And what's funny is it didn't give me a code book. Usually it gives me a code book. But it has basically coded everything again. So I have a downloadable version of my CSV file with all of the codes applied to it. So every single line, every row is now coded. And then I have my code book here. I think this is the code book. Usually from this sort of prompt, it gives me a code book. It gives me the recoded CSV file. And then it also gives me its kind of summary of the analysis. So that's what this is. What I actually don't need yet from my perspective is this full analysis, but I want the quantification. I want to see how it, like first, how it coded things, the codes that it came up with to see, do I agree or do I feel like it coded things in a funny way that I want it to iterate on?

**Live Demo** (00:45:03)

And then I want to see the, how, you know, how many, responses it coded as each of those codes. So missing favorites or save functionality because this fictional app didn't have a way to kind of save your favorite meditation sessions so you can return to them. This was a big chunk. So 23.5%. And yeah, that's like a clear that rises to the top. And then we have some other things like switch to competitor, content gaps didn't resonate. But to be clear, what's really important about the way that I structured this prompt is is actually the order of things i'm forcing it to go through the coding and the analysis in this order i'm not saying hey provide frequency counts i'm saying first look at the data then create the codes then apply them and then decide what the frequency counts are because if you jump to give me some patterns it hasn't coded anything or made sense of it in a way that you know we would agree with or make sense to us before it starts counting things and that doesn't make sense

**Aakash Gupta** (00:46:04)

I think this is a more generalized advice for anybody watching. This step-by-step prompting is how you get the AI to follow your human process. And that's our North Star here.

**Live Demo** (00:46:12)

So let me jump into the next step. You can keep asking me questions about that if you want to, but just to keep things moving. Copy-pasting

**Aakash Gupta** (00:46:22)

prompts. If the last step was coding.

**Live Demo** (00:46:26)

So this, I'm actually adding a little bit of a... of a step here for the survey analysis, because I want to compare this a little bit with, for example, sentiment analysis. For a lot of people, sentiment analysis is a natural thing to do on survey responses like NPS or CHURN. The problem with sentiment analysis is, and even a prompt like this, is that we're assuming that a large language model will understand sentiment and rate things in the way that we would. So first of all, with any Rating task like does this fit into, you know, negative, positive or neutral sentiment or, you know, which buckets do customer statements fit into? We need to explain what we would rate things at or how we would label them. So that's what I'm doing here. But also with a turn survey, for example, there is a pretty strong likelihood that a large language model will decide that everything is negative and that doesn't really help us.

**Live Demo** (00:47:25)

So instead of saying, hey, categorize or group things by sentiment, I'm having it add intensity ratings so that we can make more sense of which of the problems that are causing turn are actually most worth us working on as a product team. So if people are having a soft exit where they're circumstantial, like things in my life just changed, like there's no hard feelings. I'll come back if things change back again. Well, this isn't necessarily something that we're probably going to want to fix. Whereas if something is really frustrated, if it's, you know, a group of people who very much fit in our ICP group or they are high value customers and they're frustrated or angry, then these are probably the things we want to focus on.

**Aakash Gupta** (00:48:10)

And what's happening in this calibration example?

**Live Demo** (00:48:12)

So all of this is about how to rate things. What do we call a soft exit versus an angry exit versus, you know, a vocal detractor? What's the difference between frustrated and angry? It would be making a mistake if we assume that Claude or any of the large language models know the difference or interpret the difference the same way that we would. And this is where it gets a little bit subjective. But, you know, as someone doing a lot of research, I have beliefs about some of these things or I have an idea about what an angry customer looks like from my domain. Right. Like from this flow app or whatever I've been working on. I know the difference between angry and frustrated or you could kind of come up with your own definition. So I want it to follow my lead or the way that I've grouped people in the past so that I have comparable results.

**Live Demo** (00:49:01)

Something like that. So it's really important to me that it doesn't just kind of come up with its own rating scales or ways of labeling things, but that it kind of follows my lead and way of thinking.

**Aakash Gupta** (00:49:12)

So when you're defining something, put some few shot examples so that it's very explicit and clear what that means for the LLM. That's what I'm taking away here. Is that right?

**Live Demo** (00:49:21)

Yeah. Yeah. And what's actually really important about few shot is reasoning, not just showing what the example looks like, but why as well.

**Aakash Gupta** (00:49:32)

Okay. So giving it that reasoning so it can replicate you.

**Live Demo** (00:49:35)

So here today, it's putting things into TXT files, which is really funny because usually it outputs everything in the normal view. But here we have analysis here. But we see most people are clustered in these like level two, three, and four here. There are far fewer angry exits than neutral and frustrated, which at least is a good thing. But we want to see how they line up, how they stack up with these different codes as well, right? So this is kind of a stacking of prompts, getting more specific or more detailed in our analysis or adding a layer to the analysis. So we did coding. And now we're determining the emotional strength of these different codes. So this is the point here. What I wanted to see was... Okay, how frustrated are people who are missing favorites or save functionality, for example? Pretty frustrated. I mean, it's in the middle, level three, but there are more level threes than anything else.

**Live Demo** (00:50:31)

So that means they're pretty frustrated. And that would say to me, hey, this is something we need to work on. Makes sense. But we have all of the codes ranked by intensity. We have a little bit of a visualization because Claude decided to go a little bit beyond the brief here. I didn't ask for any visualization, but hey, I'll take it.

**Aakash Gupta** (00:50:49)

So overall, you're happy with these results?

**Live Demo** (00:50:51)

I am happy with these results because I can also check them. So because I had that exportable CSV that was recoded for me, I always ask for these kind of outputs at the end where I can double check, first of all, that from the interview analysis that the quotes are real. If it gives me, hey, this quote came from this participant on this page or it was quote number, whatever, in my Markdown file, then I can go back and I can make sure that that quote exists, that it came from the participant it said it did. And in this case, when it quantifies things, but it's already given me the full set of coded, recoded responses, I can go do my own math there too if I want to. Awesome. Where do we go from here? So... We still need an audit, that verification step. Just like we did with the interview analysis, we need to check or we need AI to check its own work here.

**Aakash Gupta** (00:51:48)

So it's going to select random responses, check for code consistency.

**Live Demo** (00:51:52)

Yeah.

**Aakash Gupta** (00:51:53)

Okay.

**Live Demo** (00:51:53)

What's really important here is simply, first of all, simply that you do a step like this, like I said before, we just need to force it to kind of do another pass through its own work. And it will usually find something that's a little off. Sometimes what it finds is some big calculation errors and It's rare if you have really good prompts and you push it through this step by step process. It's rare to find big calculation errors. Sometimes they're small, though. Sometimes it goes, hey, I would change the coding a little bit here because I think there's another group that deserves another code that I kind of mixed up in some other groups. And then, you know, the quantification changes a little bit. So that's the sort of thing I want to see here because I want to stay as close to the data as possible.

**Live Demo** (00:52:36)

I don't want to exaggerate things. I don't want to blow up responses to super angry exits from the previous step. If they weren't super angry exits, I want to be as realistic as possible.

**Aakash Gupta** (00:52:50)

Mm-hmm.

**Live Demo** (00:52:51)

So it's, for example, here it's rechecking level four because I asked it to specifically check level here. For the intensity rating audit, recheck all responses rated four or five. We don't want to go kind of running around saying, oh, people are super, super angry and we have to fix this thing right away because they're all level four or five. We want to know, is that true? Like, should this actually be priority number one? Are they actually really angry or did we over exaggerate a little bit?

**Aakash Gupta** (00:53:18)

I think this is a really interesting way to use AI. I'll call this the CYA, the way to use AI, cover your ass. What is anything that could come back to bite you when you're using AI in the project? Have AI check that out. I love this lesson.

**Live Demo** (00:53:32)

Yeah, that's a good name for it. I've heard so many people, it's less common with researchers because I think they're feeling more cautious with AI and a bit more protective of this work naturally. But I've heard a lot of product managers I've worked with and friends and designers as well. Kind of say like, yeah, I came up with all of these really nice sounding insights. And then when I went digging into the data myself or I presented it and someone asked questions I couldn't answer. And, you know, they didn't do a step like this. And if they had, I bet you that a few of the issues, a few of the holes that could be poked in the insights would have been highlighted here.

**Aakash Gupta** (00:54:13)

So if we review the three prompts so far, the first prompt was coding, the second prompt was quantification, and the third prompt is verification. Is that the right summary?

**Live Demo** (00:54:21)

So the first prompt was coding and quantification in one. The second one was rating the emotional intensity, you could say. And the third is auditing the results of everything so far. So here you can see it's corrected things. It says survey final corrected at the top. So it's recoded potentially the primary codes and also the intensity levels here. Let me see. So corrections made the coding eight corrections. So some things were missing. Oh, missing favorites was the old code and the new code is actually lack of control over selection. So it's gotten more specific about the code that it feels should be applied there. And because it's lifting this up and because it had recoded the whole thing originally, I can go through this myself and I would in a normal workflow scenario. I would go through and I would double check, do I agree with these?

**Live Demo** (00:55:13)

Like based on my understanding of the data, do I agree with these and would I kind of label them the same way?

**Aakash Gupta** (00:55:17)

And I think this is a really important step because it gave us a preview of the synthesis, even though we didn't ask. And its synthesis was like missing favorites is like driving all the churn. And I was like, wow, like if that's true, then you can really quickly solve a lot of your churn problems. But going back and coding it, I realized, oh, there's some nuance here beyond just favorites.

**Live Demo** (00:55:35)

And here, exactly as I expected, the intensity rating for at least two things was redone. So it kind of over exaggerated the frustration, right? It dropped things down from some from angry to frustrated, which could be meaningful, especially if it found more issues like that. So now we have

**Aakash Gupta** (00:55:53)

got it to check its work. What is the next step?

**Live Demo** (00:55:55)

So from here, same as with interviews, I would just do a synthesis. Like I said, I would say wrap up the top issues that are worth fixing. I would maybe ask for things per tier, like per segment based on the service tiers that they were using, like the people on individual premium accounts versus team accounts and things like that. because those might be a little bit different. We see things like billing account admin issues or technical issues, right? That might be across both of them, but billing an account would only be with team account users, for example, or proper invoice issues, things like that. So I might do a synthesis like that. But I think, again, most people are decent enough at asking for a wrap-up of the insights and not as good at pushing through this. So I would... Jump to the mega version of this, I would say, which is, if it's okay with you that I skip synthesis again, I

**Aakash Gupta** (00:56:50)

would jump. Yeah, no, I think people can imagine it on their own, right? And I'd say like how a PM and a user researcher do it might be different too. And so that's, build it to your own use case. Like as a PM, I'd probably be saying like, you know, okay, draft up, my first version of my product strategy document based on this, like what are the key problems we need to solve? Across those, please put one or two quotes from the specific survey and make it link backable so that I can go trace it if needed. But a user researcher might have some different goals. And so build the synthesis prompt for your goals.

**Live Demo** (00:57:24)

Exactly. Yeah. And all of these prompts can be modified for your goals. Right. I've done this in a particular way with, you know, retention and churn as the focus. But this can be used for any kind of analysis you're doing, any kind of data sets. It's really it's supposed to be a flexible model. That's kind of why I developed it this way. But I developed it, like I said, based on the way that people like me have been doing analysis for decades anyway. So it's not not reinventing the wheel here.

**Aakash Gupta** (00:57:51)

Awesome. So what does the agentic parallelized mega version of this look? This somewhat scary but awesome cloud code is here. Or you just install it with like a simple command. It's like npm something something. You might need to install npm. In this case, it'll have you use homebrew to install that. So it can feel a little bit intimidating to install this. But once you have it installed, you just type in the word cloud and you're here.

**Live Demo** (00:58:14)

Yeah. So I'm not using anything like a special code review or like VS Code or anything. I usually use the terminal exactly as it is, especially for demo videos, because most people who aren't used to using the terminal will download it and look at it like this. So I want to kind of keep it consistent. What's worth knowing in the first place is you have slash commands and... Agents is what I'm going to be working with right now. So if I just look at my agents, I have a bunch set up already. I kind of add new ones, delete them and reiterate them all the time. But what I'm going to be using right now are my survey analyzer light and my interview analyzer light. And this is exactly what you just saw. I've pretty much set up the same workflows or mostly, but just to work a little bit more on autopilot.

**Live Demo** (00:59:03)

So I set up those agents beforehand. The only difference between that or the biggest difference between what you've seen me do step by step in the web UI versus this is I have programmed those agents with system prompts that refer to and retrieve information from more files. Wow. So instead of being in the web UI and just uploading things every time and having an individual prompt for everything, I actually have a context document that it's going to retrieve from instead of me prompting, hey, here's my context. And I can change that context over time so I can kind of... use this agent for different things and update the context when our team information, project information, customer information, whatever it is, feature set changes, I can keep that updated. But it's kind of doing things a bit more automatically than my step-by-step process in the web UI.

**Aakash Gupta** (01:00:02)

So just to summarize for folks, I heard three inputs. Your context document, which is similar to the context prompt we saw. Your agent markdown file. In this case, she's got two. She's got a survey and an interviewer-like agent markdown file. And then your actual data or responses.

**Live Demo** (01:00:20)

Yeah. And for some reason, my pasted prompt wasn't showing for you. I really want you to see it. Give me a second. There we go. Okay. So what I'm saying here, this prompt, what you see is really simple compared to the other things, right? So what I just said was I'm basically loading all of the steps automatically in the system prompt. I built in a little bit of extra kind of feedback loop type stuff in there as well. And then it's pulling from documents. So I don't need to break this up into individual prompts. I just send it one prompt to kick off using my pre-programmed agents. I'm calling the interview analyzer light here. It's not a slash command. I just write it in and the survey analyzer light. And I'm just basically telling it to refer to the Markdown files here. And I can hit enter and it will just in a moment tell me, OK, it's starting that.

**Live Demo** (01:01:22)

So it's reading the markdown files that I just referred to for each agent. Oh, it's searching for them. This happens all the time. If my paths, if I didn't give a file path here and I just name the markdown file, then it has to go hunting for them. Sometimes I write the full path wrong too, and then it has to go hunting for them. But the great thing about Claude is it will troubleshoot that on its own. So you don't normally have to go, oh, wait, go look over here. It's there. Instead, it will just go find it in your files for you. So it found them.

**Aakash Gupta** (01:01:55)

Sometimes it might ask you for like a permission or something. You usually just hit like two, I think, and then it'll just keep going forward.

**Live Demo** (01:02:01)

Yeah, I have something I don't necessarily recommend to everyone, but you can see at the bottom this red text bypass permissions on so you can actually type in a command to remove that request, which means, unfortunately, if I were to go beyond this prompt, it can kind of do anything it wants on my computer and destroy all of my files. So I don't recommend that you do that every time. But for a demo like this, it's really helpful because it won't ask me every five seconds whether I really want it to do the next action or not.

**Aakash Gupta** (01:02:28)

And I think it's called YOLO mode, right? You can just type in like slash YOLO.

**Live Demo** (01:02:33)

So you can see it's hunting through my files in my Dropbox projects, AI tests, live demos, Akash, right? I have these files set up here so you can see the paths. And it's reading everything it needs to based on what I told it to do in those system prompts that you didn't see. And it says now I have the paths here for interviews and it's reading all of the files with the names here so I can make sure that it has read the right interview files. What's really cool about this, I mean, the reason I'm showing this in the first place is you just saw me do these analysis processes where, you know, if I weren't talking so much in between the survey analysis and the interview analysis processes individually for that amount of data and that number of prompts took about 20 minutes each. But that means you would spend 40 minutes on that.

**Live Demo** (01:03:22)

which is still remarkably fast if you felt that that was complete with a short synthesis prompt afterward. And usually it takes me a little longer than that because I have an even more rigorous process with more steps and feedback loops built in, but that's still just really fast. This allows us to do both of those things in parallel. So because the interview analysis and the survey analysis here don't build on each other, they don't need to be sequential. So instead of saying, I have one hour to analyze all of this stuff, will I have enough time? Well, yes, you have enough time if you do it like this, because you just let your agents with a pretty solid process do both things at once. And then you can triangulate on your own at the end, or you can put that into AI and triangulate for you.

**Live Demo** (01:04:07)

But you're cutting out half the time by parallelizing this. And how did we

**Aakash Gupta** (01:04:12)

parallelize

**Live Demo** (01:04:12)

it? So simply because I have agents set up that run the processes I went through manually in Claude in the web UI, I can call them both here. So in this prompt where I say, number one, use interview analyzer light. This has all my prompts that I just showed you in Claude, plus a few extra feedback loops. And so it's basically saying, do that, what I did in Claude's web UI, and then also do the survey version, but do them at the same time.

**Aakash Gupta** (01:04:43)

Nice. Yeah, sometimes I did this, like I would open this in cursor and I'd have multiple terminal windows, but I think this is actually an even cleaner way.

**Live Demo** (01:04:51)

It is really clean. You can just follow the whole thing here too. There will be sections of the process where it says expand with command O or something like that. So you can really look at the whole process it's going through just like you would in the web UI and make sure that it's kind of following the instructions, doing things properly properly. And I've told it to output everything, like output the final analysis to Markdown files as well. So I'll be able to see them in my files and kind of review them there. I also kind of like seeing how many tokens.

**Aakash Gupta** (01:05:23)

Yeah, you always want to know how many tokens you're running. While this is running, could we look into one of those agent Markdown files maybe and start to teach people about what those look like?

**Live Demo** (01:05:31)

Yeah. Got to stop sharing now. So this is I mean, this should look familiar if anyone really stops and looks at the prompts that I've used. So this is the interview methodology markdown. I've got the product, the project context and the product context and everything that was already done. in those prompts before right so i'm just feeding it all of that background information in this file and then also the definitions of contradiction types things like that so all of those pieces of information where i'm trying to teach it to analyze or identify information or label it the way that i would that's basically built in here as a sort of context load that it can retrieve from and does an

**Aakash Gupta** (01:06:10)

agent marked on file need any special formatting or instructions

**Live Demo** (01:06:14)

I mean, it depends on what you're trying to do. There are ways of getting a little bit trickier about it. But generally, it's still all grounded in being specific, being clear and specific, just the way that you would be in prompting. And for markdown files specifically, it's about structure, right? So the reason we use Markdown files is really to help the large language model retrieve information in structured, organized ways that will make it easier for it to do the processes faster and more accurately as well.

**Aakash Gupta** (01:06:50)

Okay. And Claude can help you create these agent files. If you guys are nervous about them, you can put in some of these prompts and say, hey, create me a nice interview analyzer light and it'll work with you on it.

**Live Demo** (01:07:00)

Exactly. So let's see how Claude is doing over here. Still working. You can see it's running interview analyzer light here. So it says both agents are still analyzing the data. Let me wait for them to complete.

**Aakash Gupta** (01:07:14)

Generally, do you find yourself using Claude code more or the UI more for this these days?

**Live Demo** (01:07:19)

It really depends on what I'm trying to do. But if I have everything based in my files, then I find cloud code in the terminal to just be a sort of more efficient way of doing things. I'm, like I said earlier, I don't consider myself a super technical person. I have a marketing and then design and then research background. So I'm not coming from coding. And I, once I got used to this, like the whole interface, not being particularly, you know, designy. I started really appreciating just being able to use slash commands to kind of call things, start tasks with a couple of keystrokes. I think it's really interesting to automate these processes that I would normally do step by step manually, but just learn how to make it call the right information from different documents. Or the fact that it can find the right information within my documents without me having to go, oh, where did I put that?

**Live Demo** (01:08:19)

Or even saying, do we have, you know, for repository cases where someone's saying, what do we already know about X? Well, if you have Cloud Code and it's actually synced to all of your company files, your project files, then it can just go figure that out for you. You need to know how to prompt really well. You need to be clear and explicit and you need to know how to... structure documents in a way that makes it easier for your large language model to call all of them. But if you figure that out, then a process like this goes really, really fast and much easier. So interview analysis is complete here. Survey analysis is complete. And it has a few quick findings. But what's more important is that it has output things to a file. So I'm going to stop the screen share here. And I'm going to go over to where I hope it saved it.

**Live Demo** (01:09:11)

So here's our meditation app premium user retention analysis. There's an executive summary in here because of my instructions. So we have how many stable subscribers, moderate risk subscribers there are, and so on from the interview analysis, right? So this is my interview analysis results markdown file. Phase one, data confirmation. Phase two, individual retention analysis. So there's a little bit more in here, but it's basically doing the same thing. We have the value anchors analysis and the results here. This particular therapy chat feature directly addresses a gap that traditional therapy couldn't fill and so on. We've got quotes and timestamps from this participant. So it's done exactly what it did when I was doing this step-by-step in the browser UI per participant, pulling out everything. Then we've got p2, participant 02, and all of the value anchors from this person. It's all of this, the output you've already seen, but just now in a markdown file.

**Live Demo** (01:10:11)

So what I usually do from here is I kind of format this differently, put it in pages or Google Docs or something and make it look a little bit nicer. And then I'll pluck out things that kind of stood out to me. It has, you know, that executive summary of the top. So most of the time that's pretty ready, I can kind of copy paste that and share it with someone else. But it has all of the details that I would need if I want to review this on my own as well, like you saw in the browser and even some tables.

**Aakash Gupta** (01:10:39)

Epic. I mean, this is a sick workflow.

**Live Demo** (01:10:43)

And I have another. Sorry. Oh, go ahead. I have another file like this for the survey analysis, too, just to be clear.

**Aakash Gupta** (01:10:50)

Cool. So if I were to summarize for you guys what we covered today, we gave you a masterclass in how to do discovery with AI. Discovery is the most important skill for building great products. And we've covered examples for how to do that, both for surveys and for interviews. And we've showed you how to do that with Cloud step-by-step using multi-step product sharing or to use Cloud Code and build an agent to do it. Now you have all the tools. It's up to you to go apply this. See where you get stuck. Drop in a comment below on this video or find Caitlin online on LinkedIn or somewhere else. Maybe take her course to learn deeper and really embrace this new way because the best products are built with the best user understanding. And this is your roadmap. Caitlin, thank you so much for sharing all these valuable insights for free.

**Live Demo** (01:11:41)

It was my pleasure. Thanks for having me.

**Aakash Gupta** (01:11:43)

See you later, everyone. I hope you enjoyed that episode. If you could take a moment to double check that you have followed on Apple and Spotify podcasts, subscribed on YouTube, left a rating or review on Apple or Spotify and commented on YouTube, all these things will help the algorithm distribute the show to more and more people. As we distribute the show to more people, we can grow the show, improve the quality of the content and the production to get you better insights to stay ahead in your career. Finally, do check out my bundle at bundle.akashg.com to get access to nine AI products for an entire year for free. This includes Dovetail, Mobbin, Linear, Reforge Build, Descript, and many other amazing tools that will help you as an AI product manager or builder succeed. I'll see you in the next

**Live Demo** (01:12:29)

episode.
