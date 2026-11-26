---
title: "How to Build AI products in FinTech | $100B Lessons from Robinhood VP PM"
subtitle: "The VP behind Robinhood's explosive growth reveals how they ship products"
date: "2025-09-11"
host: "Aakash Gupta"
guests: ["Abhishek Fatehpuria"]
speaker_names: "substack"
substack_url: "https://www.news.aakashg.com/p/abhishek-fatehpuria-podcast"
youtube_url: "https://www.youtube.com/watch?v=pc04_TW7Z3U"
duration: "01:18:57"
word_count: 11794
source: "Substack episode transcript (aired audio)"
sponsors:
  - name: "Kameleoon"
    url: "http://www.kameleoon.com/"
  - name: "Mobbin"
    url: "http://mobbin.com/aakash"
  - name: "The AI Evals Course for PMs & Engineers"
    url: "https://maven.com/parlance-labs/evals?promoCode=ag-evlas"
---

**Sponsors:** This episode is brought to you by [Kameleoon](http://www.kameleoon.com/), [Mobbin](http://mobbin.com/aakash) and [The AI Evals Course for PMs & Engineers](https://maven.com/parlance-labs/evals?promoCode=ag-evlas).

# How to Build AI products in FinTech | $100B Lessons from Robinhood VP PM

*The VP behind Robinhood's explosive growth reveals how they ship products*

**Aakash Gupta** (00:00:00)

Robinhood has just crossed $100 billion market cap. It 5.5xed its stock in the last year. It is one of the hottest companies in fintech, and I sat down with the VP of product behind it all, Abhishek Fatapuria.

**Abhishek Fatehpuria** (00:00:12)

Robinhood Cortex is an AI assistant. We bring together news, research reports, how trading is happening on Robinhood, and SEC filings to help customers make sense of it. U.S. stocks are still a lot of the envy of investors around the world. You ask your average person in an international country what company they want to invest in, very, very frequently they're going to say Apple, Tesla, NVIDIA, and those are all U.S.

**Aakash Gupta** (00:00:39)

companies. There have been tons of other amazing IPOs that it's pretty much the only way for the retail investor to get access. And I believe that's one of your products. So tell me the story about that.

**Abhishek Fatehpuria** (00:00:49)

The mission's very broad to democratize finance for all. And that to a lot of us means like everything. We're expanding into credit cards and banking. Vlad wants to be in every country in the world over time. Wow. We're starting to roll it out for stocks. We've got some pretty cool stuff coming up as well for it.

**Aakash Gupta** (00:01:09)

Really quickly, I think a crazy stat is that more than 50% of you listening are not subscribed. If you can subscribe on YouTube, follow on Apple or Spotify podcasts, my commitment to you is that we'll continue to make this content better and better. And now on to today's episode. Abhishek, welcome to the podcast. Thank you for having me.

**Abhishek Fatehpuria** (00:01:32)

Yeah,

**Aakash Gupta** (00:01:32)

I'm excited. So your latest launch, an AI assistant. Tell me about this. What can it do?

**Abhishek Fatehpuria** (00:01:39)

Yeah. So Robinhood Cortex is an AI assistant designed to help with your investing. So we started with a few things. So the first thing we started with was what we call Stock Digest. So one thing we really wanted to do when we took a step back is fit the AI into the customer's existing workflows. And one thing we learned when we talked to customers, it's a very universal problem, is you get this push notification from Robinhood, stocks move like 5% up or down, you open the stock, you see the chart, and the first question you have is like, why did it move? And the first goal of the feature is just to help customers figure out why it's moving. So we bring together news, research reports, how trading is happening on Robinhood, and SEC filings to help customers make sense of it. So we're starting to roll it out for stocks.

**Abhishek Fatehpuria** (00:02:42)

We're bringing it to crypto pretty soon. But the idea is to just help customers invest in their existing workflows. And we've got some pretty cool stuff coming up as well for

**Aakash Gupta** (00:02:57)

it. So building products with AI in fintech, it seems like a hazy area, an area where you want to

**Abhishek Fatehpuria** (00:03:03)

be

**Aakash Gupta** (00:03:03)

really sensitive. What were the key things you guys thought about as like guardrails or like these are some restrictions around building this product?

**Abhishek Fatehpuria** (00:03:11)

Yeah, I mean, it's hard in fintech. You have a lot of regulatory constraints. You're dealing with people's actual money, so you need a high degree of trust. So I think the first thing that we started is what data do we want going into the AI? So we curate almost all of the data that's going in. We secure licenses with the news providers we're using. We're getting research reports. We're using our own market data on the pricing we're getting directly from the exchanges. And so we're spending a lot of time curating upstream what data is going into the AI. And then we're spending a lot of time figuring out how to prompt it and how to coach it to not make mistakes and to not make recommendations and really be an informational tool for investors. But I think the thing I'm excited about is we're figuring out how to make it work in a regulated landscape, which should help us do a lot more in the future.

**Aakash Gupta** (00:04:18)

So it sounds like you were very careful to point out that it doesn't make recommendations. Is that one of the important elements, being a brokerage and those kind

**Abhishek Fatehpuria** (00:04:25)

of

**Aakash Gupta** (00:04:25)

things?

**Abhishek Fatehpuria** (00:04:26)

Right now, yes. In the future, we want to be able to do stuff like advisory and recommendations, potentially with AI. But right now, it's really a tool designed to help customers make their own investment decisions. And how did you guys decide this sequencing? The bar's a lot higher for recommendations. You have to be really, really careful. You have to consider their existing portfolios. You have to consider all sorts of other data. So where we thought it would be best to start is most of our customers come to Robinhood to make their own investment decisions. So how do we aid that process? And the early feedback's been awesome.

**Aakash Gupta** (00:05:13)

Okay. So is it safe to say that I can make more money if I start to use more AI tools like this to improve my information digest?

**Abhishek Fatehpuria** (00:05:24)

Um, I don't think that's necessarily true. I mean, ultimately you have to do your own research and make your own decisions. Our goal is to sort of optimize your workflow. So the thing that we notice a lot of people do is they read a lot of news or they read news and then they read research and then they look at analyst upgrades. So how do we condense that process and optimize it and make it faster?

**Aakash Gupta** (00:05:54)

And what did it look like in terms of the product development steps for building this AI feature? Like, how long have you guys been working on this? What type of discovery did you do? What type of solutions did you explore?

**Abhishek Fatehpuria** (00:06:05)

Yeah. I mean, so back in March, we announced Robinhood Cortex. We sort of demo two features. So one was the digest I told you about. And the second was a trade builder that helps you sort of understand potential price targets for a stock, different types of analyses, and then helps you screen the market for potential trades based off of your hypothesis. So I think our approach was generally like, we don't want to build AI products for the sake of building AI products. We want it to fit into problems we know customers already have. So, I mean, so the first, so we basically look through all of our research and we're like, what are the problems that people have that AI could help solve? So the first one was help me understand why a stock is moving up or down. It's a really, really fundamental question that almost every investor has.

**Abhishek Fatehpuria** (00:07:10)

And actually funny enough, even in internal meetings, sometimes we're like looking at a stock and someone's just like, what's Cortex say today about it? So it's honestly like been useful to us as well. And the second one was helping customers construct trades. So a customer will come into the app and they'll be like, hey, I think this stock's gonna go up or gonna go down. But then they don't know how to turn that hypothesis of theirs into like an actual trade or they don't know like hey i could buy the stock but what if i wanted to trade options how would my opinion map to a trade so those were two problems we identified pretty early and we designed the products around those

**Aakash Gupta** (00:08:00)

okay okay if you had to generalize advice for fintech pms building ai products what would it be

**Abhishek Fatehpuria** (00:08:08)

Um, oh man, that's a tough one. Um, I think the first thing is like you have to, I think you have to understand what's like possible given the technology and then you need to like really understand the regulatory landscape you're working in. Because if you don't understand that landscape, you're going to go to your legal partners or whoever else, and they're going to think you're kind of crazy. So I think you have to really understand what can be done with the tech and then also become a reasonable expert in what's possible from a regulatory perspective. And then I think the third thing is be patient. It's okay if you have this large vision that will manifest over a couple of years, which we do, but it's okay to start small and build comfort. One thing that we learned a lot from customers too is that They don't always trust an AI when it comes to their money.

**Abhishek Fatehpuria** (00:09:20)

So even for them, doing little steps and incrementing all the way there, it's best for you as the product team, it's best for your legal counterparts explaining this to regulators, and sometimes it's best for customers.

**Aakash Gupta** (00:09:37)

I want to move on to another product of yours that's pretty exciting, which is, well, I want you to explain it, actually, because all of us have seen these images of Vlad Tenev, your CEO, presenting at Cance. What is it that he presented?

**Abhishek Fatehpuria** (00:09:53)

Well, it's not my product. I think the crypto team has done an incredible job with it. But we announced tokenization earlier this summer in Cannes and basically announced two products with it. First was stock tokens, which is basically taking sort of what the stable coins did for the US dollar, but doing that for US stocks. So making building the rails to tokenize stocks outside of the U.S. Ultimately, you know, stocks, U.S. stocks are still a lot of the envy of investors around the world. You ask your average person in an international country what company they want to invest in more often than not. They'll either mention a local company, but very, very frequently they're going to say the companies you and I love like Apple, Tesla, Nvidia or whatever. And those are all US companies and it's actually pretty hard for them to access it. So if you think about what the stablecoins did for the US dollar, which is make it really accessible to get dollars overseas, these stock tokens sort of make US stocks much more accessible overseas.

**Abhishek Fatehpuria** (00:11:16)

The second thing we talked a lot about was private stocks and tokenizing them. and i think to a certain degree it's almost i think the reason why so many people were talking about them is sort of independent of the tokenized aspect of it it's that so many of the valuable companies nowadays choose to stay private for longer so retail investors can't get in they can't participate and i think We really like tapped into this like latent demand for like, I want to invest in these private companies. Like I'm using chat GPT every day. Why can't I invest in open AI? So I think that the private company aspect, I think we actually almost tapped into something else, which was people really want to invest in these private companies. Yeah.

**Aakash Gupta** (00:12:11)

So the other product talking about giving access to retail investors that you guys are really well known for is IPO access, right? Most recently, you guys let thousands, I don't know if you've disclosed the number, but many, many people of

**Abhishek Fatehpuria** (00:12:24)

my

**Aakash Gupta** (00:12:24)

friends in my network, so I know it's thousands of people

**Abhishek Fatehpuria** (00:12:27)

get

**Aakash Gupta** (00:12:27)

access to the Figma IPO. There have been tons of other amazing IPOs that... It's pretty much the only way for the real deal investor to get access. And I believe that's one of your products. So tell me the story about that.

**Abhishek Fatehpuria** (00:12:38)

Yeah, we launched IPO access in 2021, in May of 2021. We started working on it in late 2021. and it was sort of around the time we started thinking about going public ourselves and we i think part of the place where it started was like how do we we're really the home of retail investing how do we give our customers access to our own ipo and we sort of turn that into a product So we've done a lot of IPOs since then, but basically the way that it works is we're part of what's called the selling group as part of the IPO. We can collect demand after a company submits a prospectus. So we're collecting orders. So while the company is doing the roadshow and the bankers are collecting institutional orders, we're collecting orders from retail customers and we're sharing the demand data with the bankers for that stock or the underwriters.

**Abhishek Fatehpuria** (00:13:51)

And then the night of the IPO, they basically tell us how many shares does the Robinhood retail base get? And then we allocate that to our customers who requested stock. Now, very frequently, we don't get access to as many shares that customers requested. So we do our best, but, you know, It's something that a lot of people didn't have access to before. And even other brokerages that did, they tended to reserve this product for like high net worth customers or their most valuable customers. So it was really hard for the average retail customer to get access.

<!-- sponsor -->
**Aakash Gupta** (00:14:37)

Today's episode is brought to you by the experimentation platform Chameleon. Nine out of 10 companies that see themselves as industry leaders and expect to grow this year say experimentation is critical to their business. But most companies still fail at it. Why? Because most experiments require too much developer involvement. Chameleon handles experimentation differently. It enables product and growth teams to create and test prototypes in minutes with prompt based experimentation. You describe what you want, Chameleon builds a variation of your webpage, lets you target a cohort of users, choose KPIs, and runs the experiment for you. Prompt-based experimentation makes what used to take days of developer time turn into minutes. Try prompt-based experimentation on your own web apps. Visit chameleon.com slash prompt to join the waitlist. That's K-A-M-E-L-E-O-O-N dot com slash prompt. Before we dive deeper, let's talk about something every PM faces, getting alignment on product decisions.

<!-- sponsor -->
**Aakash Gupta** (00:15:35)

You know that feeling when you're trying to explain a user flow to engineering or justify a design choice to leadership and you're just describing it with your hands? That's where Mobbin comes in. Mobin is the world's largest library of real-world mobile and web app designs from industry-leading apps like Airbnb, Uber, and Pinterest. Instead of spending hours taking screenshots or hunting for inspiration, you can instantly find exactly how successful products handle onboarding, paywalls, checkout flows, whatever you're facing over 1.7 million product builders use mobbin to benchmark against best-in-class products and show their team's proven solutions whether you need to convince stakeholders there's a better way to handle user activation or research a top app's approach future discovery mobbin gives you the visual proof to back up your product decisions check out mobbin.com akash that's m-o-b-b-i-n dot com slash a-a-k-a-s-h and get 20 off your first year And I think you guys are just an engine of products like these, whether it was fractionalized stocks before that, or even just giving buyers with the initial inception of the app an easy way to sell in one click.

<!-- sponsor -->
**Aakash Gupta** (00:16:41)

If you try to sell at your big bank, if you're keeping your stocks there, it's like 20 clicks

**Abhishek Fatehpuria** (00:16:46)

just to

**Aakash Gupta** (00:16:46)

sell. So that's like then the history of Robinhood. What is it about you guys? How can somebody else who's trying to reverse engineer

**Abhishek Fatehpuria** (00:16:54)

it from

**Aakash Gupta** (00:16:54)

the outside kind of understand that DNA of building these innovative products in a regulated industry?

**Abhishek Fatehpuria** (00:17:01)

Yeah, I think our general approach to any new product is we want to give the most value back to customers and we want to have the best experience. And that's kind of our recipe. You can't have, we don't, we rarely ship a product that only has one of those. So whenever we're talking about like a net new product, it's like, how do we give the most value back to customers still in a profitable way for us, but in a way that really, really benefits customers? And then how do we build a delightful experience? And that recipe has worked really well for us. One thing that I like to do when we start new products is one thing that's unique about the financial space is that it's very rare to invent a new product. I use this example with retirement accounts all the time. Robinhood didn't invent IRAs or Roth IRAs.

**Abhishek Fatehpuria** (00:18:07)

They kind of are what they are. It's a regulatory thing. It's legislated. So the challenge that we put in front of RPMs and our team is like, okay, so we're building IRAs. You can't really change the rules of the road behind an IRA, but what are like three or four things that our IRA is going to do infinitely better? than any other Aira out there. So we have these like constraints by default because the products are what they are, uh, regulatory. And then we have to sort of push the boundaries from within. So one exercise I love is we have, whenever we launch a new product in the app, we have these things called swipeys. They're like these little four screens that tell the customer what the product is. And I love just writing, what are the swipeys for this product going to be before we build anything?

**Abhishek Fatehpuria** (00:19:10)

Because it forces you to like succinctly summarize the product to a customer in like four small sentences. So I think that exercise has worked well for us.

**Aakash Gupta** (00:19:24)

The Swipeys are the full screen takeovers, right? They have like an animation and a little text. Yeah,

**Abhishek Fatehpuria** (00:19:28)

it's usually like an animation, gorgeous illustration that our design team does. Like a little bit of text explaining the product and you can like swipe through them. And there's usually like three or four for any given product. So it's

**Aakash Gupta** (00:19:45)

kind of like Amazon's working backwards, but from a swipey point

**Abhishek Fatehpuria** (00:19:49)

of view. Yeah. I mean, we were a mobile first company. So like we think and like mobile screens. Yeah. So it's like, if you can't convince a customer to hit the get started button in like one sentence, we don't have a great product. Yeah. That's kind of the bar we try to hold.

**Aakash Gupta** (00:20:09)

So IPO access, like let's break that down in detail even further, right? We got the timeline, we got the high level.

**Abhishek Fatehpuria** (00:20:15)

What were

**Aakash Gupta** (00:20:16)

the evolutions of the product along the way before the final version that people got to see?

**Abhishek Fatehpuria** (00:20:21)

Yeah. I, you know, it comes back to the, the few things, which was like the swipeys, like how do we talk about this product? It feels so obvious now, but like we took so long to get to the tag phrase, like get in at the IPO price. Cause people like investors weren't really used to participating in the IPOs. So like, they didn't fully understand what like IPO access like meant so we had to like succinctly and like five lines explain like what is it that this product is gonna give you and one pain that we felt customers always express with this is like they see the chart they're like the stock seems to have opened at 20 but it seems like it started trading at like 50 Like, who got access at this, like, $20 mark? So the tag phrase we sort of landed on at the time was get in at the IPO price.

**Abhishek Fatehpuria** (00:21:28)

It, like, spoke to the pain people felt versus, like, speaking to, like, this... It was like the classic like painkiller versus like vitamin phrasing of the product. And then the second thing was like, how do we make like getting a share part of this IPO, like a really memorable experience, like something that you emotionally connect to. And the team put together this gorgeous like animation of every time when you receive these shares, like this hot air balloon, goes in the sky and you get like the stock certificate that shows you like you were the nth investor in whatever company so we like really just dialed in the details of the experience

**Aakash Gupta** (00:22:17)

and those things like those animations why isn't every other brokerage doing things like that

**Abhishek Fatehpuria** (00:22:23)

I think it comes down to like what you value. You know, I think ever since day one, we pay so close attention to the pixels and like to the experience and just not a lot of other brokerages do. And it's infused in the DNA of the company. Like Vlad spends a lot of time with the pixels. Like I spend a lot of time with the pixels. It's not just like the design team is making these beautiful designs. It's like a lot of the entire company really thinking about how do we craft the best experience. I haven't worked at other brokers, but I would imagine that the CEO of the company or like the leaders of the companies at other brokerages aren't spending a large share of their time thinking about How are we going to make this experience feel great? What's the animation going to be?

**Abhishek Fatehpuria** (00:23:24)

You know, so I think it's like it's infused into the DNA of the company in a lot of ways.

**Aakash Gupta** (00:23:31)

And then I guess your harshest critics, they would say, well, that's actually a good thing that those other companies, you know, are putting up walls because. You shouldn't really trade often. People who trade a lot lose a lot of money. The average retail investor is not beating the S&P 500. How do you guys kind of grapple with that?

**Abhishek Fatehpuria** (00:23:51)

Um, yeah, I mean, for IPO access, for example, I would argue that getting having the ability and having the option to invest in an IPO for a company that you've personally been using for such a long time is a really valuable like option to have. So I think our general principle is like people should have access and great design, like You shouldn't use bad design as a way to like keep people out or like high guardrails or high walls. Like we like as a company, like deeply believe that people should have access to the financial tools. That they need to be successful. And I think historically, you know, people have said like, you need like this much money to participate. And in a lot of ways, I don't, especially with the internet and people having more access to information. I don't know if like net worth is like necessarily correlated with like sophistication.

**Abhishek Fatehpuria** (00:24:58)

Yeah. So I think some of the old constructs around like how do you how do people like qualify for certain products or how are they eligible for certain products don't make that much sense anymore. Yeah.

**Aakash Gupta** (00:25:10)

And I think having been a PM in fintech myself, sometimes, you know, the PMs on my team, sure, we're coming up with great ideas that do remove friction. But then what ends up happening is like death by a thousand departments. You know, the legal team comes in and they say, oh, we need to add this line here and it needs to be visible right under the CTA. And then that... privacy team comes in and says oh we need to add this step and then you know the kyc legal team another legal team comes and all of a sudden after 25 departments have it you know your product is a total frankenstein but ramen hood's products somehow they don't fall into that trap is

**Abhishek Fatehpuria** (00:25:45)

it

**Aakash Gupta** (00:25:45)

something like is it vlad at the top just pushing all the teams is it a culture where the type of people you're hiring in those departments aren't putting up those roadblocks how do we dissect that

**Abhishek Fatehpuria** (00:25:54)

Yeah, I think we've got an incredible legal team and compliance team. And I think a lot of it starts at like they are so they're so deeply like experts in the space, like a number of them worked at the SEC. A number of them have worked as regulators or they've worked in the space before. They've worked at other BDs or broker dealers. So they're so familiar and they're such deep domain experts in these problems that they're actually like... they're actually very effective at solving the problem and getting to a really, really good product solution. So, I mean, so many, I love our legal partners. So, so many of them, like they get excited about the product and they want to find ways to like build the best experience for customers. So I think some of it comes down to culture. Sometimes when there's disagreements, I mean, obviously we escalate And sometimes, you know, they're the ones pushing like, how do we make this a better product?

**Abhishek Fatehpuria** (00:27:03)

So it's like infused into the culture and who you hire. And, you know, our chief legal officers done an incredible job building like a really, really like expert team there. ai evals are one of the

<!-- sponsor -->
**Aakash Gupta** (00:27:16)

most important skills for pms and i know you know they matter the question is are you doing them right most teams are winging it with basic metrics and hoping for the best meanwhile the teams that actually ship reliable ai they've cracked the code on systematic evaluation today's episode is brought to you by the ai evals for engineers and pms course by Hamal Hussain and Shreya Shankar. This live Maven course will teach you the battle-tested frameworks from Hamal and Shreya, who are the engineers behind GitHub Copilot's evaluation system and 25-plus production AI implementations. Four weeks, live instruction, next cohort starts July 21st. Start shipping AI that actually works. Enroll at maven.com with my code ag-product-growth for over $800 off. That's ag-p-r-o-d-u-c-t-g-r-o-w-t-h. today's episode is brought to you by amplitude replays of mobile user engagement are critical to building better products and experiences but many session replay tools don't capture the full picture some tools take screenshots every second leading to choppy replays and high storage costs from enormous capture sizes others use wireframes but key moments go missing creating gaps in your understanding When you're coaching your own PMs about working with legal, what do you tell them?

**Abhishek Fatehpuria** (00:28:59)

I tell them, I think the biggest thing is you have to assume good intent. They're not there to make the product worse. They have a role to play. Their job is to make sure that we are safely shipping the products we want to ship in accordance with the regulations. So it's like you have to start with good intent. I think the second thing is you want to make everyone on the team better. regardless of what function they're in, buy-in to the vision of the product. When you have a legal partner or a compliance partner who's bought into the vision of the product, the outcomes of that product are so much better than if they don't believe in the product in the first place. So in the same way that you get buy-in from the engineers or the designers, you got to get buy-in from the legal team.

**Abhishek Fatehpuria** (00:29:56)

that the thing you're building is going to be awesome. And that leads to great outcomes. And I think the third is to actually deeply understand the issues that the legal team is bringing to you. And actually understand like, what's the rule? Like, what is the issue that we're trying to solve? If you become an expert in it, and you empathize with it, you'll find that most of the time there's a reasonable solution to it. And, you know, it's like 10% of the time it's like black and white. And then like 90% of the time you're dealing in gray areas. So you want to like empathize. You want them to buy into the vision. And then you find usually a good solution.

**Aakash Gupta** (00:30:48)

So you joined Robinhood in 2016. Quite a long time. What stands out to you? You know, revenue, people, culture. How has this company scaled?

**Abhishek Fatehpuria** (00:31:00)

I think the thing that convinced me to join was the people. I mean, the talent density at the company, even when it was at the stage of post-product market fit, but pre-serious revenue was insane. And I felt like I was learning all the time. And I felt like that was the type of environment I really wanted to be in. So that's what attracted me in a lot of ways. That's like what's kept me. I think the second thing is this like laser focus on building like the best product. I think Robinhood is a great example of like great products tend to win in the market. great products with great distribution win in the market. And it's not just about like being first or like being first to market doesn't always matter. Like we spend a lot of time crafting the product, paying attention to the details, and that makes a huge difference.

**Abhishek Fatehpuria** (00:32:06)

And that's the type of place I wanted to work. And then the last thing is, I mean, the ambitions of the company are insane. The mission's very broad to democratize finance for all. And that to a lot of us means like everything we're expanding into credit cards and banking. You know, Vlad wants to be in every country in the world over time. So I think like the mission is so broad and there's like no end to the types of things we can do. So the one thing that I reflect on is after nine months, it always feels like my job is somewhat different. So it keeps it fresh.

**Aakash Gupta** (00:32:52)

That's

**Abhishek Fatehpuria** (00:32:52)

crazy. So what are all those products? I mean, you have stock trading, you have options, you have crypto, you've got margin, securities lending. um what else um i actually robin hood gold maybe robin hood gold yeah that's a good one so we're not

**Aakash Gupta** (00:33:15)

stock market experts this is not financial advice but how would you break down the elements of why your guys's stock has had this phenomenal five and a half xing the past year

**Abhishek Fatehpuria** (00:33:27)

Oh, I mean, I don't want to speculate on that. And I'm not sure I'm supposed to speculate on that. But I mean, you see the metrics online, the same that we have when we publish quarterlies. The revenue has been really strong. I think we have figured out how to sustainably really grow assets on the platform ever since we launched retirement. with the match, that's been a very effective strategy for us. And then I think the thing that I'm most proud of and that we love to talk a lot about is product velocity. I think that's the hardest thing to think about when you're just analyzing a stock. Robinhood, like our teams are so focused. It seems like we ship some stuff every week at this point. So I think the product velocity to me is like the most impressive thing when I look back at it.

**Aakash Gupta** (00:34:30)

Yeah, I think that's exactly right. I think it's that combination of you're proving it in the metrics. Yeah. But then there's all this potential we see with what you're shipping just regularly, and it's always coming out faster and faster. And so that's a really incredible. How does it feel to pass 100 billion in market cap?

**Abhishek Fatehpuria** (00:34:48)

You know, um, I don't really think about it. I'm like, I'm like, so, so we have this, uh, we have our next keynote coming up in a month. So I'm like, so focused on that, that I'm not, I haven't really even been thinking about the stock price and the market cap, you know, to me, those are like, those are like, it's a little bit, I mean, I check it and stuff, but I don't really process it as much. Um, yeah it's just

**Aakash Gupta** (00:35:19)

a distraction i

**Abhishek Fatehpuria** (00:35:20)

mean it's hard to ignore because our our app is literally about stocks and the thing i test every day is literally about stocks so it's hard to ignore but i try to ignore it as much as possible and especially right now while we're like um focused on Hood Summit in a month. I'm like so laser focused on that. Life as a product leader, right? It's

**Aakash Gupta** (00:35:49)

like the next big release.

**Abhishek Fatehpuria** (00:35:51)

Yeah. I think the events have been like also game changing. I think so. Yeah. Have you watched them?

**Aakash Gupta** (00:35:58)

They're just I'm just watching how much social attention they're getting

**Abhishek Fatehpuria** (00:36:01)

over

**Aakash Gupta** (00:36:02)

time You know, I think like four or five years ago I wouldn't have heard about a product launch from you guys

**Abhishek Fatehpuria** (00:36:06)

now It's like

**Aakash Gupta** (00:36:07)

every two or three months you guys dominate my ex

**Abhishek Fatehpuria** (00:36:09)

timeline. That's actually something I was very Surprised by that worked really really well for us, which was these like product. Yeah events and We started in March of last year. That was our first one. Nice. We did the gold event, the first gold event. Okay. And we've done, like, a few since then. And if

**Aakash Gupta** (00:36:35)

people don't know, that's Robinhood gold, which gives you, like, I think 3% cash back, which is more than, like, any other

**Abhishek Fatehpuria** (00:36:40)

card, right? So that's the credit card. Yeah. 3% cash back. Yeah. It's a great card. Yeah. I use it personally, so. But... Yeah, that's the one thing that I think has been really effective for product growth has been these events. And it's actually also been amazing for the organization because having an event to point an entire team towards where it's like we are shipping and delivering these four or five things. It's clarifying. It creates a lot of focus. Yeah.

**Aakash Gupta** (00:37:19)

So you smashed 100 billion. You went through another really emotional moment when you guys IPO'd. What was that like?

**Abhishek Fatehpuria** (00:37:25)

Oh, that was one of the most memorable moments of my life. Yeah. Yeah, it was really fun. I mean, we were I was in New York for most of that week. And, you know, we got to go to the NASDAQ. We did like an event there in the morning, went out to Times Square. It was like one of those. It was like a big milestone moment for the company. And, um, it was like very, it was just awesome. Like so many of the team came out despite it sort of being COVID lockdown, still a lot of people made it out. So it was great. It was very, very like rewarding to be a part of that.

**Aakash Gupta** (00:38:13)

It must have been crazy, like after

**Abhishek Fatehpuria** (00:38:14)

all

**Aakash Gupta** (00:38:15)

those hard years of work, seeing that outcome.

**Abhishek Fatehpuria** (00:38:18)

Yeah, especially like 2020 and 2021 was particularly crazy for us. So that was like a great bookend to all of that.

**Aakash Gupta** (00:38:28)

Yeah, you guys were in the news all the time, whether it was meme stocks or GameStop or so many things. That's crazy. Speaking about that, I think at that period, that's when there was the most controversy

**Abhishek Fatehpuria** (00:38:42)

about

**Aakash Gupta** (00:38:43)

Robin Hood. What's one thing outsiders completely misunderstand about Robin Hood's success? In that period or in

**Abhishek Fatehpuria** (00:38:50)

general? In general. Oh, misunderstand about Robinhood's success. I don't know. I think we went through like a big low point in our brand in 2021 and everyone thought we were like not like we had like bad intentions and stuff. And I think that was a particularly tough period to be like an employee because like, you know, we were all there. I mean, we have... like to think we have good intentions um we are trying to make access to products that have historically been gated away from people so i think that period was particularly tough but very rewarding to like make it out the other end

**Aakash Gupta** (00:39:40)

And did Robinhood have to go through one of those tech shrinkages? Did you guys have a layoff? I think

**Abhishek Fatehpuria** (00:39:46)

I heard about that. We

**Aakash Gupta** (00:39:47)

did in 2022.

**Abhishek Fatehpuria** (00:39:48)

Those are also very tough. Yeah, that

**Aakash Gupta** (00:39:50)

whole period was a really tough

**Abhishek Fatehpuria** (00:39:52)

time at the company. But, you know, I think so many learnings from that whole like COVID plus 2022 experience. Yeah. I feel like I grew a lot.

**Aakash Gupta** (00:40:12)

Yeah. So now we've come to the topic that all my listeners, when I told them I was interviewing you, they said I had to ask you about, which is... how you guys build products. Because I don't think there has been any information on the internet anywhere. This is going to be new information for everyone. What does the Robinhood product team look like? How is it structured to start?

**Abhishek Fatehpuria** (00:40:36)

So we are in GMs, so we're sort of structure into like three big business units, call it brokerage, crypto, money, which is the credit card and banking and stuff. I hope I'm not missing something. And then within those, sometimes we have like sub-businesses like the futures business or international and stuff. And sort of each business unit has a product team. So I work on the product team for brokerage. So that's sort of how we're structured today at a high level. And then, you know, we have design and engineering. We made the switch to GMs from like functional actually around the time that we did our reduction in force in 2022. Yeah. And, you know, I think it was just amazing for the company because, I mean, you were asking about like working with legal and stuff, but it brought a lot of functions like product, engineering, operations, compliance, all under the same like org, not legal, legal, still separate, but it brought all of those functions under the same org for each business.

**Abhishek Fatehpuria** (00:42:02)

Gave them like some shared goals and some shared purpose. And that made a big difference. Suddenly felt like everyone was rowing in the same direction.

**Aakash Gupta** (00:42:13)

What was the implication for life as a PM? Did it mean that you might be working on more of a wider platform team and now all of a sudden you're working on a very specific product? Did it mean that the nature of your metrics changed? How did it change your job?

**Abhishek Fatehpuria** (00:42:28)

For me personally or for the team? For PMs at large. Yeah. I don't think so. I think the biggest impact was probably more on the like cultural side of the PM team. Like when we were one big PM team, there was a really tight unit. People hung out a lot and people spent a lot of time together and there was a lot more like product team, call it like camaraderie. And when you split it to product team for brokerage, product team for crypto, etc., we definitely lost some of that connectivity of one single big product team. As for the day-to-day work, I think the other big shift was... And I think a lot of our PMs already did this, but really not just thinking about the product, but also thinking about the business and connecting it to the business. And in a lot of ways, sort of starting to push a lot of our PMs to think more like GMs for their businesses.

**Abhishek Fatehpuria** (00:43:41)

um and for the products that they work on which i thought was a great change personally um so i think those were probably the two big changes i don't think the day-to-day changed that much apart from that

**Aakash Gupta** (00:43:58)

so how big is the pm team today how big is the engineering team um

**Abhishek Fatehpuria** (00:44:05)

So brokerage all in is around, I want to say around 25 to 30 p.m. to about maybe a little bit less to about 250 engineers in brokerage. um i want to say okay and that probably kind of like scales appropriately brokerage is the largest like org in the company so that's sort of where we are okay so it's like

**Aakash Gupta** (00:44:37)

a one to ten

**Abhishek Fatehpuria** (00:44:39)

Yeah, a little bit. I think it depends on the function. So like something like options, much more niche, much more like complex domain, a little bit lower. Some of the domains that are more complicated, probably closer to 10.

**Aakash Gupta** (00:44:55)

Okay.

**Abhishek Fatehpuria** (00:44:55)

Okay. Yeah. How do you guys handle planning? Oh man, we change planning every year, but it gets better. I think What we try to do is, and there's no perfect way to do planning, as I'm sure you know. We try to align on, I think, so first starting at a leadership level, we try to align on like what are our big bets for next year. And water some like ideal targets for metrics. So say like last year, it was like, we want to ship this desktop web product. And then we also want to grow this mature business by like X percent. So we'll try to align on that at a leadership level. One tweak I'm trying to make now with our team and the company at large we're trying to make is now that we do these product keynotes, instead of just being like, what are our big bets?

**Abhishek Fatehpuria** (00:45:57)

It's more like what's going to be in the, what's going to be in the keynote? Like let's plan the tentative keynote like now. And that sort of substitutes for like the big bets. after that um after we have the big bets and rough metrics targets sort of let the individual teams cook on plans for to achieve those goals for the big bets it's typically a conversation around like what is it going to take do we need to add more people to the team do we like reorient some of the org to make it happen For stuff like grow this mature business by X percent, it's like the team comes back with a plan for it and then we review it together. So I think it depends a little bit. I think the big change I'm hoping to make is let's just plan these keynotes like 9 to 12 months in advance so we know what we're trying to deliver.

**Aakash Gupta** (00:47:02)

And some companies... Actually, every company I've worked at planning, they have like certain units that they really care about. So at a firm, it was like GMV, like that's the unit that we're looking at almost everything through

**Abhishek Fatehpuria** (00:47:16)

the

**Aakash Gupta** (00:47:16)

lens of how is it driving GMV? Or when I was at Apollo.io, it's like incremental ARR is what

**Aakash Gupta** (00:47:22)

we

**Aakash Gupta** (00:47:22)

really cared about or net revenue retention, depending on the phase that we were talking about. So do you guys do something like that? Like, how do you guys think about what are the things you pay most attention to in this planning process?

**Abhishek Fatehpuria** (00:47:34)

yeah so we um sort of have three like strategic arcs to the business so the first is to be number one for active traders so the key metrics we look at for that are like market share uh along our key businesses and One challenge that we have is that our business is very dependent on the market. So it's very hard to be like, hey, we want to set these like volume goals because something happens in the market. You're not you may just blow past it. You may not hit it. So we look at market share. Mm hmm. The second strategic arc is number one in wallet share for millennials or the next generation. Millennials and Gen Z and soon to be Gen Alpha, hopefully. For that, we tend to look at like net deposits, like are people... depositing more money into the platform and we look at gold subscriptions the last is global financial ecosystem which is sort of international where we sort of look at how many international customers do we have that is at its most nascent stage and number one in active traders is probably the most mature of those three so we have a fairly diverse business so that means sort of looking at a lot of metrics but it's worked for us so far

**Aakash Gupta** (00:49:18)

and then where does like responsibility allocation go do you guys use okrs for that how do you handle that

**Abhishek Fatehpuria** (00:49:26)

yeah we don't use okrs necessarily we have like goals they're like functionally okrs they're just like simpler typically like either a goal will be qualitative like ship xyz by this event and that's typically for like the big projects or you'll have grow net deposits by like this much so they're not as like complicated as okrs we had okrs at some point and sometimes we just ended up debating the difference between an objective and a key result always and it was just like why are we doing this like the goal is the the goal is the goal so we just simplified it yeah and

**Aakash Gupta** (00:50:15)

sometimes you don't always have a key result and in that case are you going to formulate and fabricate one or like and

**Abhishek Fatehpuria** (00:50:22)

so

**Aakash Gupta** (00:50:22)

just goals okay

**Abhishek Fatehpuria** (00:50:24)

yeah it's just goals it's really simple we like grade them every we like trend them we grade them we see how we're doing we hold ourselves accountable to them and then we like refresh them quarterly

**Aakash Gupta** (00:50:41)

how are you asking your pms and other people in the epd trio to use ai at work

**Abhishek Fatehpuria** (00:50:47)

Yeah, we're still, I think for PM, the thing I, and we're still pushing this a lot more, I think are two things. One is like, almost like ideation and discovery and research. Like I personally use it all the time to be like, Here's a product problem we're trying to solve. Here are like two or three ideas I have. Can you hit me with like 10 more ideas? Usually pretty high noise, but sometimes you'll find like a gem in there. And it's pretty low cost sort of trial and error. There's that. The second thing that we use it a lot for is like when we're evaluating a new opportunity to like learn about the space. So let's say hypothetically... Before IPO access, we were like, Hey, I want to like learn all about IPOs. Like that's a great tool to have. So I think it's really helpful in like the early stages of product development.

**Abhishek Fatehpuria** (00:51:57)

um and ideation that's where i've personally and the team has found the most value sometimes and then i think the second category is like automating and reducing the toil of like some of the like manual administrative work around pm um like Sometimes you're just writing content for something and you need to like replicate 10 different messages. You just make that fast. Yep. You know, so I think early stage product development, it's a super helpful tool, late stage, you know, or like day to day operations, just helping with your own efficiency. Um, I'm not sure it's quite there yet in helping write a whole PRD or something. I don't think you're going to get keen insight from it.

**Aakash Gupta** (00:52:54)

And what's your take on the PRD, actually? These days, a lot of people are talking about how AI prototypes should just replace the PRD.

**Abhishek Fatehpuria** (00:53:01)

So I think in fintech, it's hard because sometimes the PRD covers so much of the like detail behind a product, you know, like here are the rules and the regs and here are the edge cases we need to capture. So I don't think you can ever effectively like get rid of it. But I will say, and for a long time, I don't like personally doing product reviews with like PRDs. I find them to be not that like high signal on like, are we going to build a good product? So I typically try to avoid doing like a live product review with someone on my team until we have some semblance of either the swipeys to talk about like value props or we have an actual mock or prototype because ultimately it's like I'm going to experience the product. Like our customers are not going to get to read your beautiful...

**Abhishek Fatehpuria** (00:54:06)

PRD yeah to understand what why and why they should use this thing yeah so why should I as the reviewer get that assistance you know so are

**Aakash Gupta** (00:54:19)

you guys using AI prototyping tools

**Abhishek Fatehpuria** (00:54:22)

Not that much, honestly, right now. I mean, we're using it a lot in engineering and stuff. The engineering team uses all the AI tools, but not as much in prototyping. I'm excited to see what we can do with early stage design and stuff.

**Aakash Gupta** (00:54:40)

Mm-hmm.

**Aakash Gupta** (00:54:42)

So you've hired a lot of PMs who haven't worked at Robinhood, even though you've worked entirely at Robinhood. What do you find as like those things that they're finding? Oh, this is different about how Robinhood builds product.

**Abhishek Fatehpuria** (00:54:53)

Yeah. Oh, I've had a lot of conversations about this. I think the attention to detail in the pixels that is expected by a PM at Robinhood is very, very high. Yeah. like i've had people join my team and they're doing super well now but like going from outside to inside and being like oh like i have to like pay attention to like these level of pixels in the product and make and push the team to get to this degree of polish is typically a pretty big shock to people. And it's an adjustment that people have to make. But that's what makes our product special. So it's something we've really tried to protect. But I've also heard that everyone loves it after some time. Like it's very painful at the beginning. You might have something like get delayed because you didn't like pick up on something. And then someone went in was like, this doesn't feel right.

**Abhishek Fatehpuria** (00:56:02)

We're not shipping like fix it first. So it's like painful at first, maybe for new people. But I've never really had someone on my team come to me like a year down the road and be like, I'm like frustrated at the level of detail that is expected of me in the product. Because ultimately, I feel like they feel prouder of what they're shipping because of it. So that's usually, I think, the biggest adjustment.

**Aakash Gupta** (00:56:33)

And all the PMs are going to be raising their finger and saying, but, but, but, Abhishek, what if I don't work at a company where design is so open to me just being in the pixels? What is the right way to work with design?

**Abhishek Fatehpuria** (00:56:47)

I think you need to establish trust. I mean, I think it's... And what I mean in the pixels, it's not just in like Figma. It's like also like once it's been built, like... using it tearing it down making sure think the product feels great like ultimately what i hold the product team accountable to is like did we ship a great product that had impact so if it's not good or it doesn't feel polished or it doesn't feel like it's up to the bar um they should feel accountable for that. And I think on the design stuff, it just comes to a high degree of trust between the teams. And it's like, it's like asking questions. It's like, hey, is this the right way to do it? Or did we miss something? It's not like going in there and editing it yourself.

**Aakash Gupta** (00:57:42)

Yeah. So it's about collaborating in the right way also and not stepping over their line that that's their responsibility. But like you said at the beginning, first inspiring them with the vision and then giving them the feedback after they give that

**Abhishek Fatehpuria** (00:57:55)

first draft. Yeah. It's typically more like I've got the product in hand, I'm using it, but it just like it feels off or like certain things aren't fully right yet. And it just comes down to like intensely using it and being like what feels wrong. And sometimes it's like we just didn't catch this thing when we were designing it.

**Aakash Gupta** (00:58:25)

So do you guys have a pretty long period? Like I can remember times that I've never even as a PM touched the final version of the product because maybe there were some build issues getting me the production version of the app and how it looks outside of a sandbox environment. Do you guys make sure that like everybody internally is using the product for some period of time before you ship it?

**Abhishek Fatehpuria** (00:58:46)

We tend to dog food a good amount internally. I mean, the length depends on the product.

**Aakash Gupta** (00:58:53)

Yeah.

**Abhishek Fatehpuria** (00:58:55)

So for something huge like retirement, we were using that for longer internally. For something smaller, the internal time isn't that long. But it's not unusual for, you know... stuff to hit internal and then we're like, hey, this isn't quite ready yet. Let's take an extra one to two weeks and make it feel really dialed in. And I think the best part is a lot of our company are actually users of our product. They use it all the time. So you kind of get to a naturally high bar just with internal feedback.

**Aakash Gupta** (00:59:37)

Yeah,

**Abhishek Fatehpuria** (00:59:38)

yeah.

**Aakash Gupta** (00:59:39)

So within the product team, you guys launched an APM program. Yeah. How's that going?

**Abhishek Fatehpuria** (00:59:44)

It's new. I mean, they joined like, I want to say like a month ago now. So it might be too early to say. But I'm really excited about it. I mean, we have two APMs on my team. Mm-hmm. They both seem awesome. And they're both... They're kind of working on, like, very different things, which is going to be interesting. It's almost like an A-B test for, like, what is the right type of project to have an APM work on. One of them is working on, like... smaller scale, but like rapid product improvements to like our desktop product. Um, and then one of them's working on like, uh, working with another one of our PMs on like a larger scale, like nine month project, um, So we'll see which one works better. But I'm really optimistic about it. I mean, I joined Robinhood as a new grad.

**Abhishek Fatehpuria** (01:00:54)

The early hiring philosophy was a lot of new grads at that company. So I feel like it's kind of going back to our roots. Yeah, it's like the DNA of the company. Yeah. So I'm really excited. I'm really pumped about it. What was your story of breaking into Robin Hood? So I interned as an engineering intern and then converted full time. I just love the team, learned a lot. How did you crack that internship? So I actually had so my old my like freshman year college floor mate had interned the summer before me. So it was through him that I network that I got the interview. And he very interestingly, he had also joined full time. So he referred me. It was great. I loved it. Had a lot of fun with the team. Decided to stay back. I was on the engineering team. I mean, the company was so small, like the line between engineering and product was blurry for quite a bit of time.

**Abhishek Fatehpuria** (01:02:12)

But started doing some product work, like right after I joined full time, worked on growth, built our referral program. That was sort of my first career. that was

**Aakash Gupta** (01:02:25)

huge back in the day

**Abhishek Fatehpuria** (01:02:26)

yeah yeah that was uh that was a that was one of the big unlocks for us like the free stock because it was a variable reward right the free random stock yeah that was a big one so that was my first like big product as a product manager also did the a lot of the engineering for that

**Aakash Gupta** (01:02:46)

did you guys know variable reward worked like did you hit that off the

**Abhishek Fatehpuria** (01:02:48)

back or did you have to unlock that over testing um We tested so much with that product. Nice. Um, we kind of had an intuition that free stock was going to be the best, but there were a lot of weird learnings along the way. So we started with cash, um, like 10 bucks. Um, it, it worked, but it didn't work great. Like the conversion numbers weren't, we're like, okay, not good enough. Then we were like, okay, let's try variable cash. And in this whole meantime, we were trying to figure out how to like mechanically do stocks because it was more operationally complicated. So we did variable cash. So things improved with variable cash, but still wasn't great. Then we launched variable stocks. And it worked really, really well. But the thing that we learned was it still wasn't converting well enough to actually make the program work.

**Abhishek Fatehpuria** (01:03:52)

So the unique thing that we actually learned at the time was the first version of variable stocks. And so many people talk about this product, but they don't talk about this part. We just put the stock in someone's account. But then we were like, the conversion's not good enough. They're not actually activating. So we added this step to make customers affirmatively claim their stock. So they actually have to go in and say, I want my stock. It was more delightful than that. And that completely changed the trajectory of the conversion because they were doing an action to take that. And then we did all sorts of other things, like now that you owned a stock, we would send you a price movement notification a week later, or we would send you a news notification about the stock that you got. To kind of get you like in the ownership mentality and all that stuff made a big difference.

**Abhishek Fatehpuria** (01:05:05)

And then the last sort of very unique finding was with variable rewards, you sort of control the expected value of the outcome. So customers actually weren't that sensitive to the expected value. What they really cared about was twofold, that they were getting a stock and that they had some chance of getting a really valuable stock. So we were able to experiment for a long time with that and it was huge for us.

**Aakash Gupta** (01:05:38)

Yeah. Yeah. That's a great example of, I think, why you guys succeed, going back to the very beginning, right? It's like this crazy amount of iteration and testing on these growth levers. Why are most fintech PMs not doing that? Why are most fintech PMs failing at that? Are they? I think so, yeah. Oh,

**Abhishek Fatehpuria** (01:06:00)

really? I don't know. I mean, I think we're fairly successful at it. So I didn't know that people are failing. Why do you say that?

**Aakash Gupta** (01:06:12)

I don't think many people are doing it. I mean, most people, they launch a referral program. They do 2020 because that's what Amazon or Uber did. And that's

**Abhishek Fatehpuria** (01:06:20)

like

**Aakash Gupta** (01:06:20)

the end of it, you know? They're not like... You just talked about a series of like 10 different successful tests, which tells me there's probably 50 failed tests as

**Abhishek Fatehpuria** (01:06:29)

well. So

**Aakash Gupta** (01:06:29)

you did like 60 tests on the program and you were able to think of very unique hypotheses and kept iterating. That's just your product velocity that you guys have that very few fintechs have.

**Abhishek Fatehpuria** (01:06:40)

Yeah, I don't I don't know. I think one thing is like you have to take inspiration from like other companies and like what's working. But you have to like think about what's going to work for your product and you have to like. You also have to take whatever someone else is doing with like some grain of salt because like you can't assume they did everything like perfectly. You know, it's like the same laziness that you have inside the company probably existed. at amazon or uber too yeah so i and i think specifically with the referral program our thing was like we want to give you a unit of this service like the insight from amazon or uber especially is not that they give you 10 bucks it's that they give you a ride

**Aakash Gupta** (01:07:32)

yeah

**Abhishek Fatehpuria** (01:07:33)

so it's like okay so you stretch that further it's like what is the ride equivalent of robin hood it was a stock it wasn't 10 bucks

**Aakash Gupta** (01:07:42)

yep

**Abhishek Fatehpuria** (01:07:43)

so i i think you have to dig a little bit deeper than like just what the surface tells you

**Aakash Gupta** (01:07:51)

yeah so you probably hired some pms from other fintech companies what advice are you giving them to succeed in fintech

**Abhishek Fatehpuria** (01:08:00)

Um, I think FinTech's really unique. Um, you have a broad set of cross-functional partners, probably larger than most other companies or most other like traditional tech companies. So I, I think the biggest thing is you have to like. The same way you would treat like engineering or design, you have to treat like all your partners because they are essential to getting the product out and it being successful. So it's the first thing is you have to recognize that you have a broader set of partners and they're not there. to be like blockers. They're there to be a part of the team. They're there to be effective. And that mindset shift is like a really big one. It's not just like engineering product and design. There's a lot more involved. in shipping product in financial services. And I think that's why you also tend to see some of the ratios of ENG to PM a little bit lower in fintech because there's just so much more for the PM to do.

**Abhishek Fatehpuria** (01:09:16)

So I think that's the first thing. I think specifically at Robin Hood, it's like pay attention to the design and care deeply about the experience. That's something like everyone resonates with. And then... I think for fintech, those are like probably the big things.

**Aakash Gupta** (01:09:39)

Yeah. Yeah. Really getting good at working with these different cross-functional teams. And like you were saying earlier, becoming a little bit of someone who can learn fast. Like what is the actual core of a legal issue means you need to be able to either with AI as your sparring partner or legal as your sparring partner, get pretty deep into a topic quickly. Yeah.

**Abhishek Fatehpuria** (01:10:00)

Yeah, I mean, that's absolutely true. And you have to build intuition for these things. Like it's never black and white. Oh, it's rarely black and white. Sometimes it's black and white and then it's really easy to make decisions. But in order to make the best product decision, you got to like understand like your legal partner needs to understand what you're trying to achieve in the product. And in the same way, you need to understand, like, what is the legal issue that you are trying to deal with? Yeah. Or what's the operational issue that you're trying to deal with? Without having that understanding, you'll just talk past each other.

**Aakash Gupta** (01:10:46)

Yeah.

**Abhishek Fatehpuria** (01:10:48)

And how do you deal

**Aakash Gupta** (01:10:49)

with like building a product? Like what's the philosophy you have of building a product that has real money, real risk, real emotions behind it?

**Abhishek Fatehpuria** (01:10:57)

Yeah. I mean, I think the first thing is you have to like really understand like what is it that your product is? Like, what is it that your product is going to do better than other products out there? So, I mean, a lot of the first steps that we do, which I'm sure others do, is like, you're building IRAs. Go understand all the other retirement accounts on the market. Like, what do they do well? What do they not do well? one thing we have to like think about early is like what do we want someone to like feel when they use this product like what emotions do we like want to elicit and I think for I'll use retirement as an example like we were like hey we want to make the act of saving for retirement feel like really really special So it feels like a moment that you connect with, it's a moment you want to do over and over again.

**Abhishek Fatehpuria** (01:12:00)

And it's something that a lot of people are proud of when they save for retirement. So I think you need to connect to a certain degree on a human level of what are the objectives people are going to associate with your product with. Like with buying a stock, a lot of people remember the first time they bought a stock. They remember what platform they bought it on. It's a really meaningful moment for a lot of people. So you really want to like pinpoint like, what is it that we want you to like feel in that moment? And to me, for like saving for retirement or buying your first stock, I think we want people to feel like happy. We want them to feel like they're doing something like positive and good for themselves. So I think there's like that emotional aspect of it that you have to understand.

**Abhishek Fatehpuria** (01:12:57)

What is it you want people to feel?

**Aakash Gupta** (01:12:59)

Mm-hmm.

**Abhishek Fatehpuria** (01:13:01)

So we've walked through

**Aakash Gupta** (01:13:02)

your career story from intern to VP in less than nine years. What do you think are some of the career habits or the ways you treat your career that's different from others that has enabled you that really rapid success?

**Abhishek Fatehpuria** (01:13:18)

Um, yeah, I think Robin Hood was, I think there's a little bit of luck. Actually, there's probably a lot of luck, like right place, right time. Um, I think there is like I think the biggest thing is like not being afraid of like the like the like work you made like not like the detail oriented like grunt work. I think that's like the thing I've always like never shied away from. And I think it builds a really strong degree of trust with people. When a product manager or a product leader digs in and is like, okay, great, we've got this issue. Let's deeply understand what's going on and really digs in to empathize with the other person. Or if there's an engineering problem, the PM or the product leader is there and even if they're just there for like moral support, like those things make a big difference.

**Abhishek Fatehpuria** (01:14:23)

So it's like always asking how you can help. I mean, obviously having an impact on the business and then, you know, being like treating not just, I think the one thing that I like to do is like my team is like more than just like the product managers. It's like everyone who works on the brokerage product. They're all like, In a lot of ways, like I like to think of them as my team. And that like, I think builds like, it just like points you to think in a different way, which builds trust with people.

**Aakash Gupta** (01:15:02)

Especially over the long term, right? Because then you're making, I guess, like decisions that to use Adam Grant's language is more like giver than taker.

**Abhishek Fatehpuria** (01:15:11)

Yeah, hopefully. I mean, I'd like other people to say that about me. Makes

**Aakash Gupta** (01:15:17)

sense. Let's say you have your cousin and he's trying to become you. He's in college. He's saying, Abhishek, I need to find this next company like Robinhood because you just told me right place, right time was a really important part of it. How do they go about doing that?

**Abhishek Fatehpuria** (01:15:35)

I think it's hard, and I got lucky. I think the thing with Robinhood, and I think it's increasingly true with companies today, was it was post-product market fit. Yeah. So even when I was interning, it just felt like, I mean, I definitely drank the Kool-Aid, but it felt like there was some sort of inevitability to the company because customers loved the product. Yeah. So I think that you've got to find a company that's at product market fit or like you are confident you can help it find product market fit. And in that case, you're probably joining really early anyways. Yeah. I think that and then ideally the company is like responsible. I think one thing that Beju and Vlad did really, really well early on was was the company was like lean from day one. And I think they bet on, like their whole philosophy on talent was betting on people over and over again.

**Abhishek Fatehpuria** (01:16:45)

So, I mean, we definitely hired a lot of experienced folks, people in the brokerage industry, people from across the industry, but especially early on, they wanted to bet on the talent that was at the company. So that plus like the company's trajectory was like a great recipe.

**Aakash Gupta** (01:17:06)

So look for a company that has product market fit defined as customers just insatiably love it so that you can feel like it has some inevitability of success. And then

**Abhishek Fatehpuria** (01:17:15)

look

**Aakash Gupta** (01:17:15)

for founders that are running it well. They're running

**Abhishek Fatehpuria** (01:17:17)

it

**Aakash Gupta** (01:17:18)

lean and are willing to bet on people.

**Abhishek Fatehpuria** (01:17:20)

Yeah. I think the last part's really important. Okay. You want to be at a place that's going to invest in you. Yep.

**Aakash Gupta** (01:17:29)

Yeah. When I look back, like some of the places I worked, ThredUp, that's where the company I went through that IPO'd, the founders were just always there investing in

**Abhishek Fatehpuria** (01:17:36)

their

**Aakash Gupta** (01:17:36)

people. Which

**Abhishek Fatehpuria** (01:17:37)

one

**Aakash Gupta** (01:17:37)

was that? ThredUp. ThredUp. Yeah. Yeah. So it was a similar era as Robinhood,

**Abhishek Fatehpuria** (01:17:43)

I

**Aakash Gupta** (01:17:43)

think 2021 IPO. Yeah. Well, I'll be shaking. We could do another 90 minutes. That is our time. If people want to get in touch or learn more,

**Abhishek Fatehpuria** (01:17:54)

how can they do that? Yeah. I mean, feel free to reach out. I've got my Twitter account. I've got my LinkedIn account. Feel free to reach out.

**Aakash Gupta** (01:18:03)

All right. Twitter or LinkedIn. There you go, guys. That's how to get in touch with him. Thank you so, so much. Yeah. Thank you. All right. Bye everyone.

**Abhishek Fatehpuria** (01:18:09)

So

**Aakash Gupta** (01:18:09)

if you want to learn more about how to shift to this way of working, check out our full conversation on Apple or Spotify podcasts. And if you want the actual documents that we showed, the tools and frameworks and public links, be sure to check out my newsletter post with all of the details. Finally, thank you so much for watching. It would really mean a lot if you could make sure you are subscribed on YouTube, following on Apple or Spotify podcasts and leave us a review on those platforms. That really helps grow the podcast and support our work so that we can do bigger and better productions. I'll see you

**Aakash Gupta** (01:18:47)

in the next one.
