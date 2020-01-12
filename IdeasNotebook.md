---
layout: page
title: Ideas Notebook
---

<p class="message">
  <b>A notebook of quick ideas, thoughts, mental models and reminders.</b> <br>
  Any time you read something interesting or useful that you might want to explore in the future, take note of it here. Otherwise, you'll end up forgetting it. Compound and structure your ideas here. 
  <br>
  <b>Possible topics:</b> ethics/behaviour, philosophy, neuroscience, risk, probability + statistics + ML, investing, startups + VC, thoughts on careers + work...etc
  <br>
  Even if you only write down 1 interesting technique/idea/thought a week, by the end of the year you should have at least 50 decent paragraphs to think about. 
</p>

--- 

#### --. Information Loss as a framework for your research interests: the 'Procrustean Bed' of Statistics, Probability and Information Theory
* **Probability Theory**
  * Given a random/uncertain/stochastic process, what sort of outcomes can it possibly generate?
  * Over a long time-span, what will these outcomes look like? 
  * Maybe that's why NNT says the one of the best ways to learn probability theory is to do 1000s of Monte Carlo simulations: you see different outcomes being generated, and the behaviour of these generated outcomes.
  * Also: ergodicity problem: 1 data-generator going through 1000 time-steps is NOT always the same as 1000-data generators going through 1 time-step each. Their statistical properties are different when incorporating the possibility of the gambler's ruin.
  * Ergodicity and iid: The outcomes of Russian roulette is technically *i.i.d.*. But if you don't survive a round, then you dont get to play again - the outcomes of all the sequential turns are VERY dependent on your last turn. (literally your *last* turn. sorry....). So the exposure to an iid variable isn't necessarily iid --- is this just respresented as a transformation of random variables??
* **Information Theory**
  * Given a *restricted* channel that transmits information/data, what can you tell about the source, if you receive a signal at the end of the channel?
  * How much information can the channel even transmit? How can you *lose* valuable information if the channel isn't very good? Can you choose to lose redundant/useless information to save space/time? 
  * Sometimes, in the case of data-science/statistics, the lossy/noisy channel is actually just your data collection technique! You collect data from a data-generating-process in an ineffective way, due to resource constraints (time, money, sensors...etc), and so you *lose* some of the information along this data-collection 'channel'. Or there are external variables that you haven't considered to collect, so it seems like there is 'noise' in the data that you collected. 
  * Regardless, data collection is usually an act of forcing a real-life phenomenon through a noisy and lossy channel, where the output is just your collected dataset. And sometimes, there's even some sort of 'bandpass'-like filter in this channel: e.g. collecting data from a fat-tailed/heavy-tailed variable, but not over enough of a time-span, so the lowest frequency data-points might be under-represented. (see: The Statistical Consequence of Fat-Tails - NNT). Similarly, you can have other types of filters, through data-collection biases like: survivorship bias, selection bias - leading to things like Berkson's paradox...
* **Inference!!!!!**
  * How do you further 'compress' or 'filter' your collected data into a more compact *statistical model*?  Or in other words, how do you *bias* the data towards your chosen model? 
* ------------------------------------------------------
*  **\[ 1 \] \-\-> \[ 2 \] \-\-> \[ 3 \]**
  * 1 = data-generating process; can theoretically generate 10000s of outcomes, across many parallel universes (Monte Carlo sim...).
  * 2 = collected data; only managed to collect 1 of the 'parallel universe' outcomes though. Already, you see there is some loss of information. In fact, the whole idea of cross-validation is to pretend like you collected multiple sets of data from parallel universes, and use one of those as the testing-set...
  * 3 = selected model; you further had to lose some of the information in the data-set into a simple model. A lot of the time, you'll use some big assumptions for this process... 'statistical modelling' and 'machine learning', they call it... 
* ----------------------------------------------------------
* **What ways can you 'compress' and lose information along the 3-step process?**
  * D.Freedman: Statistical Models - different assumptions used to do statistical modelling (need to go through the book...)
  * N.Taleb - Gaussian Assumption (lose info about fat-tails), Ergodic assumption (lose info about path-dependence), ...etc
  * Statistical Learning Theory - 'compress' and intentionally lose information so that data is 'biased' to a chosen model.
  * Polyadic vs Dyadic relationships - Shannon-information measures, like Entropy and Mutual Information, fail to capture multivariate dependencies (dyadic relationships! - e.g. XOR gate and conditional entropy - dissertation is related to this and the consequences in gambling)
  * J.Pearl - causal information is usually lost in most statistical models, so how can you extract that using things like probabilistic graphical structures?
* ----------------------------------------------------------
* **And finally, the whole reason for these topics: GAMBLING**
  * Given that you have all this information loss in your statistical modelling process, how can you best predict the behaviour of the data-generating process?
  * And more importantly, even with possibly incorrect/inaccurate information, how should you bet on the outcomes? How do you transform probabilistic behaviour of a random variable into a real exposure to your life? 
  * Different ways of managing exposure: bet-sizing and capital allocation, contracts and options ('clipping the tails of the distribution', or more commonly known as insurance).


---

#### --. Ancestrally Lost Emotions
There are a few 'ancestral' emotions that, historically, our ancestors have always felt and lived with, that nowadays most of us don't feel. Maybe it would be a good idea to design your life so that you actually experience some of these emotions.
* *Being needed by your team* - when was the last time that you felt *needed* within your 'tribe'? Not just *"it would be nice to have you tag along, but if you dont turn up we'll still survive"*, but more like *"we need you on our team and without you this mission has a real chance of failure, so get your sh\*\t together and stop whining"*. As harsh as that sounds to hear, there's something strangely warm there.
* *Loyalty* - when was the last time you actually had to live with a sense of loyalty towards a group? A sense that you should sacrifice some of your own selfish interests for the good of the whole group? Or are you working for a team you don't respect, full of obedient cowards who've never taken any risks in their entire lives, but you 'need the money' so you tolerate it? How can you ever be loyal to a group that you don't respect? And how can you be loyal to a boss who you never voted into power? 
* *Craftsmanship* - when was the last time you felt a sense of pride and craftsmanship regarding your work? Can you take pride in the quality and elegance of the work that you create? Can you move towards a sense of mastery? Or are you shuffling papers around and sending emails for a living: the kind of job that takes a new grad only 2 or 3 months to learn how to do?
* *Risk and Adventure* - are you working on something where you could fail? Are you chasing a goal that makes your life into a bit of an adventure? Or are you obediently doing what you're supposed to do all the time, and your sense of adventure is derived purely from travel/holidays and planned experiences? See, that's not adventure - that's just expensive consumerism. But since it's expensive and more exclusive than, say, watching Netflix, it becomes prestigious. The same way that powdered cocaine is almost the 'prestigious' version of smoking crack, but in both cases you're still an addict.

Maybe the solution is to work in small selective teams with autonomy and shared values (like Startups, small Hedge Funds and elite R&D groups) and chase high-risk-high-reward opportunities as a team. Maybe that's the more ancestrally suited way to work.

---

#### --. Generating Process vs Realized Outcome
* There's a difficult tension between focusing on the generating process vs focusing on the realized outcome.
* When you focus on the process, and perfecting your 'craft' and on becoming ["So Good They Can't Ignore You"](https://commoncog.com/blog/so-good-they-cant-ignore-you/), you enjoy the day-to-day aspects of work much more, and you improve at a much faster rate.
* But the whole point of being good at the process is so that you can eventually generate good outcomes. But focusing too much on the outcome makes you sacrifice energy optimising for something quite fleeting: after you generate the outcome, often you are left only with the skills that you picked up. 
* **From a Skill + Craftsmanship perspective**: should you focus on being the best musician you can be, or do you focus on playing a specific song as perfectly as you can? Because focusing too much on playing a specific song may distract you from spending time actually improving your real skill.
* **From a Statistical perspective**: "The basic problem that we study in probability is: *Given a data generating process, what are the properties of the outcomes?* ... The basic problem of statistical inference is the inverse of probability: *Given the outcomes, what can we say about the process that generated the data?"* - All of Statistics, L.Wasserman
* **From an Ethical perspective**: The honor and 'sacredness' of living up to certain virtues (the generating process) is more important than the outcome (winning). That's why sometimes it's better, and more elegant, to lose ethically than win unethically. 
* **From an Academic perspective**: Should you focus on being the student with the most knowledge, curiosity and depth of understanding? Or should you focus on optimising your grades like an obedient f\*\*\*ing nerd? I guess that phrasing gives some indication about my opinion on the matter ;) 
* **From a Motivation perspective**: Focusing too much on the outcome makes you feel too much pressure. Enough pressure and stress to make you put things off for later, for when '*you're more prepared*'. Unfortunately, that's one of the surest ways to waste your life away, one day at a time. Instead, if you give yourself permission to screw up, you feel suprisingly free and motivated to do your best work. Intentionally ignoring the outcome makes you enjoy and master the process which, paradoxically, leads to a better outcome. I think the idea of *Memento Mori*, or the reminder of inevitable death, has a similar effect: *You're going to die anyways, so it's actually OK to fail today - it's not a big deal. So why not just do what you want to do, make a sincere effort at trying your best, enjoy the process, and see what happens? Leave the rest up to fate. Considering that you're going to die one day anyways, whatever happens will be a good thing.* A lot of the ideas from Stoicism are similar to this. (TODO: link to convexity, and having nothing to lose - next idea)

Judgement of process over outcome: "Heroes are heroes because they are heroic in behavior, not because they won or lost. Patrocles does not strike us as a hero because of his accomplishments (he was rapidly killed) but because he preferred to die than see Achilles sulking into inaction. Clearly, the epic poets understood invisible histories. Also later thinkers and poets had more elaborate methods for dealing with randomness, as we will see with stoicism." - NNT, Fooled By Randomness

---

#### --. Having Nothing to Lose, Stoicism, Antifragility and Underdogs 
* I think Stoicism and the idea behind a 'Memento Mori' can be summed up in this one line: "If I have 'nothing to lose' then it is all gain and I am antifragile" - NNT, Antifragile. 
* A few interesting ways to feel like you have nothing to lose (or feel like it's OK to fail):
  * 'Fear-Setting', and clearly defining the worst-case scenarios (Tim Ferriss)
  * 'Finally after years of frustration, I had a breakthrough. A very wise person suggested that I give myself permission to never publish the book. I felt an immediate sense of relief' - R.G. Ignore the outcome - Give yourself permission to fail. Give yourself permission to screw up and make mistakes. Give yourself permission to get rejected. Now that you've stopped caring about perfectionism and success, you can focus on doing good work and enjoying the process/attempt.
  * 'All I’m allowed to do is absolutely nothing, or write.' - [Neil Gaiman](https://tim.blog/2019/03/30/the-tim-ferriss-show-transcripts-neil-gaiman-366/)
  * 'Actually almost everything I've written that has survived was written when I didn't try to get anything done.' - N.N.Taleb 
  * The whole idea of being an underdog is that it's actually somewhat OK for you to lose. Nothing else is expected from you anyways. But that's what's so freeing and motivating for you to win.
  * Countersignalling - downplaying your traits and being humble allows you to feel OK with failing; much more freeing than having the pressure of having to live up to expectations. In a way, countersignalling makes you feel like an underdog. 
  * Epistemic Humility - Reminding yourself that you're *mostly* an idiot and you're nowhere as smart as you pretend to be is freeing. It lets you ask dumb questions, look underneath deeply held assumptions, and ask questions that are usually overlooked. Honestly, it's also quite fun being the 'surprisingly smart, not as dumb as he looks' guy in the room (rather than the other way round). 
  * Trash - something very personal; remind yourself that you're *mostly* an arrogant, abrasive, disagreeable trash who doesn't really deserve special treatment or acceptance. Now that you really don't care if you get rejected, in fact maybe you even feel like you actually *deserve* it, it frees you up to be authentic and sincere and humble; no pretending or trying hard to impress. And look at the consequences of that - more people like you than ever before ;) 
  * 'It is only when you don't care about your reputation that you tend to have a good one' - N.N.Taleb
  * 2am Productivity - maybe you're most productive at 2am (like right now...) because you already feel like the day is gone. There's no expectations anymore. You can go sleep or you can do some work, it doesn't matter. Feels freeing enough for you to enjoy working with no expectations. (or it might just be your Cortisol rising at about 2am and this bullet point is dumb a.f. .....)
  * gambling away time - (expanded in another paragraph) - gambling 2 hours feels kind of freeing too, like I have nothing to lose. There's some acceptance of the 2 hours being totally unproductive and profit-less - hence the term 'gamble'. If I get something interesting done in those 2 hours, then I'd be really happy but there's no pressure. Same with the 2-week experiments (Tim Ferriss) and 6-week-bets (Basecamp).
  * Past experience at Nomura - waited until after a deadline to do some work... Mostly to p\*ss off the right people, but also because now there's nothing to lose. I'm already technically past the deadline. No pressure now that I know that I can do it at my own pace without having anything to lose. What are they gonna do - be more disappointed in me? ;)
  * Gratitude - for some reason, cultivating a sense of gratitude also makes me feel like I have nothing to lose. Maybe because, implicitly, gratitude suggests that what I'm grateful for isn't supposed to be mine by default. It's not normal to have such things, and life could be *much* worse. Gratitude makes those things feel like an undeserved reward from a benevolent god or universe. Gratitude feels freeing, even if it's indirectly. 
  * k.o.d.m.y.h.&.c. - d.d.

I think the reason this idea is so freeing is because you have 2 types of stress. Eustress (positive stress), the kind of good stress you feel when chasing (or hunting) a goal. And Distress (negative stress), the bad stress you feel when avoiding (or running away from) a punishment. Most situations in life probably contain both types of stress. **But what if you can get yourself into a state where you are ONLY chasing, but not running away?** That way, you ONLY feel Eustress, and almost no Distress. 

Feeling like you have nothing to lose might invoke this state. If you have nothing to lose, you have nothing to run away from.

---

#### --. Eustress vs Distress; Predator vs Prey Brain Chemistry...

* Look up later: is eustress just an optimal ratio of cortisol/adrenaline/dopamine? And is distress just a 'bad' balance of those hormones? If so, is the feeling of 'having nothing to lose' just a way of tricking your body into releasing less cortisol (?) so the hormone balance is more optimal? 
* What's the equivalent neuroscience for predatory and prey animals? Predatory animals (Tigers, Wolves, Lions... all the cool ones, really...) have nothing to lose when they hunt. They're already in a default state of 'not having much to eat', so anything they hunt is a positive reward. So maybe their actions are mostly dopamine-motivated?(simplistically speaking) 
* But prey animals *always* have something to lose: by default they have food (grass and leaves usually) everywhere. When they have to actually do something, it's always some sort of running-away-from-danger activity, to avoid losing their life. So are they more (adrenaline/cortisol/distress)-motivated? 
* What does that imply about people and employment? Are you chasing and 'hunting' your own targets, with a sense of eustress and excitement? Or are you dodging bullets, trying to balance a bunch of work being thrown at you by a moron you don't respect? Are you avoiding getting into trouble with a sense of distress and just rying to keep up? 
* TODO: read up a bit more on: Agency and freedom of choice + immune system health + endocrinology stuff (Status Syndrome by M.Marmot, Why Zebras Don't Get Ulcers by R.Sapolsky)    

---

#### --. Writing and Expression: Forcing-Functions for Procedural Knowledge
* Something interesting that I've learnt over the last term -  Writing and Expression expose your knowledge to a very useful constraint: the constraint of actually making sense.
* Sometimes an idea can hibernate in your brain without it necessarily being examined thoroughly. Maybe you believe something because it sounds good, or because everyone else believes it. But the moment you commit to actually explaining the idea on paper, it gets 'exposed'.
* Without a true understanding of the topic, you won't be able to write anything interesting or coherent. The act of explicitly writing down and exploring an idea on paper *exposes the gaps* in your thinking.
* Writing, like programming, forces you to explicitly articulate and organise **procedural knowledge**. It almost forces you to construct the idea from scratch and walk through the idea, step by step. (Similarly, doing exercises in a textbook forces you to run throught the **procedure** of actually using the techniques that you were supposed to learn.)
* The only problem with writing is that words are so linear - it's hard to capture non-linear interactions and complexity in a single sentence. But I think the act of constraining non-linear, complex network/tree-like knowledge into linear combinations of sentences and ideas is what makes writing so useful and clarifying. 
* Part of what makes someone a good writer, or a good poet or even speaker, is the ability to evoke complex, non-linear imagery using a linear string of words. 
* Most importantly, from a personal perspective, is that writing makes you - if only temporarily - into a maker, a creator, and an expressive thinker, rather than just some passive information-consumer. It's almost like the idea of ['make before you manage'](https://tim.blog/2019/12/18/make-before-you-manage/); writing helps you 'create while you consume'.

---

##### --. Writing: Daily Target
* Apparently Ernest Hemingway used to write about 500 to 1000 words per day. Steinbeck aimed for at least 1 page per day. And one of Tolstoy's diary entries: "I must write each day without fail,not so much for the success of the work, as in order not to get out of my routine." Many of the greatest writers all had a habit of **creating + writing, every single day**. 
* And I'm willing to bet that some of the greatest software engineers do the same: write and re-write their code, every single day.
* So maybe that's a good target for personal productivity: write roughly 600 words (~4 pages, with equations and all) of technical content per day.

---

#### --. Writing: Verbal Explanations vs. Mathematical Proofs; finding the 'Verbal Threads'
* Interestingly, if you look at your memory and understanding of a technical topic *months* after you learn it, the mathematical proofs aren't necessarily what you remember. In fact, what you remember is actually very verbal and/or spatial - you rely heavily on diagrams and verbal explanations. The equations are just representations of the ideas, but compressed into symbols to save space. 
* And similarly, when you listen to a lecturer, you don't focus on the maths symbols - you focus on the sentences that talk *about* those symbols, and *how* they're connected to each other. 
* So maybe the best way to learn technical material is to articulate the content in sentences, and *only then* are you allowed to compact/compress the ideas into symbols. 
* In a way, the words and the explanations are the dynamic, procedural 'life' of the knowledge; they actually explain how you jump from step to step. The mathematical symbols and the diagrams are mosty just snapshots of the knowledge - they show the state of your variables and their relationships in a static manner, but they never explain how to get to the next step.  
* In other words, your job when you read a research paper or a textbook chapter is to *seek out the verbal threads in the text*. The verbal, articulatable knowledge will be hidden behind lots of complicated symbols. They're not important. The underlying thread is the important part. Reading papers written by guys like Richard Feynman, Ed Thorp and E.T.Jaynes seems to re-inforce this concept. They're very verbal and speak almost in a conversational tone. They don't dilute their sentences with useless words, and they don't use unnecessary maths - you can see the 'verbal thread' very clearly.

---

#### --. Rate maximisation of X/Y (Should you maximise the numerator, or minimise the denominator?)
* You want to maximise the rate of X per Y. Trying to increase the rate of X is numerically, but not practically, equivalent to decreasing Y. 
* Real life example 1: Returns/Risk in finance. Maximising returns and finding alpha might be a very different activity to finding sources of risk and minimising them. But both actions lead to a higer ratio of returns to risk. Sounds very obvious, but maybe it gets forgotten in practice.
* 'The essence of investment management is the management of risks, not the management of returns.' - Benjamin Graham

---

#### --. Asymmetries between Losses and Gains...
* *Magnitude Asymmetry*: a 10% loss can only be 'evened out' with an 11.1% profit. Similarly, 50% loss can only be evened out with a 100% profit. ('volatility tax' M.Spitznagel)
* *Time Asymmetry*: losses are usually quick (crashes, days), profits are much slower to accumulate (months, years).
* *Psychological Asymmetry*: if you screw up and lose money at the start of the year on a single day, you'll effectively spend the rest of the year just playing catch-up to break even. How much stress that entails... I dont know... But if you spend the whole year making money and then lose it all on the last day, and break even, it won't be anywhere near as psychologically or physiologically stressful... 
* Maybe these asymmetries are why Warren Buffet's rules are: 'Rule No. 1: Never lose money. Rule No. 2: Don’t forget rule No. 1'.

---

#### --. The Equation for Wisdom, and aging well...
* The guys who I respect and whose 'wisdom' I take seriously all have something in common: they have the courage to stand up for what they believe in, and they say what's on their mind. They're willing to take risks and pay the price for their opinions. They're definitely not wimpy conflict-averse conformists, to put it lightly.
* I still don't know what came first though: did their courage allow them to become wise and interesting, or did their internal wisdom tell them to be courageous? 
* Something that I've personally experienced: Every time I took a risk for something that I believed in, but scared me, I always ended up with some extra sense of self-respect afterwards, even if I failed. 
* So maybe this is a good test: Sum up (or *integrate*) the number of courageous actions you took last year. That's probably proportional to the amount of wisdom, experience and self-respect you gained. If it wasn't scary, then you probably didn't learn sh\*\*. 
* And an extra note: Curiosity helps too. If you're actually curious about something, you learn much faster and in more depth.
* So, in a very nerdy way, it's something like: **d(Wisdom)/dt = c*(Courage) + k*(Curiosity)**. 
* Maybe this is harsh, but it seems there are some old men that have no wisdom and command absollutely no respect. They've only aged in biology, but not really in spirit. I wonder if that's because they never take risks for what they believe in, and so they have no personal wisdom? "Often a very old man has no other proof of his long life than his age." - Seneca

---

#### --. Gatekeepers and Rejection
* I've noticed that rejection feels refreshingly fair when it seems like I've been judged on my actual qualities. Sure, it hurts a little bit - but there's no 'salty' leftover resentment: I feel perfectly fine afterwards, and if anything it motivates me to improve my skills. 
* But when a rejection feels like it was based on surface level inaccurate information, and was made by someone who couldn't make a proper judgement, there's leftover resentment - it feels almost unethical. Most commonly,'unfair' rejections seem to come from gatekeepers: or those who don't have the skills to judge quality, but are in the position to do so. In other words, skillless recruiters and HR leeches with disproportionate power and influence. The types who are impressed by buzzwords and judge you based on the presence of those buzzwords, while the only tangible skill they themselves have is 'sending emails'. (But credit where credit is due: some of the recruiters thrive in a risky career where their income depends on their performance; I think that's quite respectable.)
* This leads to a more interesting and deeper problem: information symmetry, signalling and honest representation. 

---

#### --. Countersignalling and Pretending
* Anyone would tell you how repulsive it is when someone pretends to be better than they actually are. Someone trying hard to look smart, interesting, strong, or any other positive trait, will always look stupid when they're found out. Bluffing is only (temporarily) impressive when it works.
* The ethics of information-sharing, and spotting the pretenders, is kept deep in the memories of our DNA. Spotting a pretender brings out an instinctive, strong sense of repulsion and mistrust. 
* But something interesting that I noticed about guys that I respect is that they actually do the opposite of pretending: they **countersignal**. They actually try to downplay some of their impressive traits in a humble way. 
* Sometimes, the smartest guy in the room is the most willing to look like an idiot by asking stupid questions and joking around with people (while the less sharp guys sit their with a boring, serious look and an unnecessary fondness for jargon and beating around the bush). Sometimes, the strongest guy in the room is the most willing to de-escalate a tense situation, at the risk of looking 'scared'. And sometimes, it's the billionaire who walks into the room with flip-flops while the rest of the room tries hard to look like they have money.
* Comedians, for some reason, seem to do a LOT of countersignalling. In a way, a good stand-up comedian is most likely the wittiest and bravest in a crowded room, and yet they countersignal by saying a lot of hilariously stupid stuff, along with self-depreciating jokes. 

---

#### --. Focus on the Jugular; Spot the Pulse
* Or, more elegantly said: "If they don't go for the jugular, they don't know where it is." [(link)](https://startupbros.com/antifragile-act-cant-know-much/) 
* And, "Nitpicking is the unmistakable mark of cluelessness" - N.N.Taleb 
* In other words, in any conversation, don't be the clueless idiot who has no idea where the jugular is. 
* And if you don't know where it is, don't pretend like you do know. As we've established with the previous idea on 'Countersignalling and Pretending', pretending is repulsive and unethical. Just admit that you don't understand what the core principles and ideas are, and work forwards from there. Epistemic humility and honesty are more impressive than temporarily looking smart. 
* You're aiming for clarity of thought and the ability to spot the jugular: that's what lets you ask the real questions and make the biggest impact. And maybe a lot of this skill is actually just the ability to ignore the unessential: the ability to filter out noise.

---

#### --. Noise Detection
* (todo)
* (knowing what to ignore, negative knowledge)...
* Now, the idea of detecting which rules, conventions and people to ignore: unruliness, disagreeableness. 

---

#### -. High Agency; Unruliness; Disagreeableness
* Something important to remember and 'unlearn' after all those years of schooling and credential-gathering: **Listening to instructions is NOT the same thing as playing to win.** Breaking conventions and ignoring what you're 'supposed' to do, and aggressively chasing your own interests, is sometimes the best option. Seeking the approval or permission of an institution or a system designed by an obedient nerd isn't really winning. Some of your favourite writers all have their unique takes on this idea.
* Eric Weinstein: ['High Agency'](https://tim.blog/wp-content/uploads/2018/08/131-eric-weinstein.pdf)
* Paul Graham: ['Relentlessly Resourceful'](http://www.paulgraham.com/relres.html), ['The Lesson to Unlearn'](http://paulgraham.com/lesson.html) 
* Jocko Willink: 'Default: Aggressive', 'Extreme Ownership'
* Nassim Taleb: 'Aggressive Tinkering', "The doer wins by doing, not convincing. Entire fields (say economics and other social sciences) become themselves charlatanic because of the absence of skin in the game connecting them back to earth."
* "Agreeables play games where judges award points to determine the winner. Disagreeables play games where you win by scoring goals." [link](https://hackernoon.com/nassim-taleb-and-the-disagreeables-35d1f9cfad90)
* Tim Ferriss: "If the potential damage is moderate or in any way reversible, don't give people the chance to say no. Most people are fast to stop you before you get started, but hesitant to get in the way if you're moving. Get good at being a troublemaker and saying sorry when you really screw up."
* Jack Donovan: "No one respects a man who is always asking for permission. No one respects a man who won't stand up for himself or fight for his own interests. No one wants to cheer for a team that stopped playing to win. Most people would agree that men who don't play to win deserve to lose."
* But now you encounter a new problem: Too much disagreeableness, self-interest and unruliness isn't sustainable for long-term relationships. You need something else: risk + sacrifice for others.

---

#### --. Sacrifice + Risk
* (todo)

---

#### --. The 99/1 Barbell Personality; Directed Intensity; 10am/12pm/*2pm*/4pm
* The Personality Barbell: Probably the greatest idea that I've picked up over the past year, and something I've noticed about the guys that I respect: they have the capacity for aggression and power, but they don't overuse it. 99% of the time, they show a combination of humility, hospitality, gratitude, kindness and a general sense of relaxed playfulness. In other words, most of the time, they're very chill, down to earth and don't take themselves seriously. But in that rare 1% of the time when it's needed, they can 'activate' the aggression, conviction and disagreeableness that makes them respectable to begin with. They go straight for the jugular when it's time, so to speak. 10/01/20 - Watched the acceptance speech by Dave Chappelle, for the Mark Twain award. Apparently his mum used to say something to him when he was younger: 'Sometimes you have to be a lion so you can be the lamb you really are.'
* The Craftsmanship Barbell: Similarly for technical and creative disciplines/crafts, world-class performers claim to apply a similar idea with their craft. Most of the time is spent in a relaxed, low-effort mode. And when it's time to start working, they turn up their intensity and aggression to the max, in an almost disagreeable and antagonistic way: absolutely nothing should stand in the way of their craft, and they have no time for time-wasting distractions or empty words. Eric Weinstein, Tim Ferriss, Jocko Willink, Nassim Taleb, Josh Waitzkin, Cal Newport, Naval Ravikant, Paul Graham... etc all talk about variations on this idea. 'Deep Work' seems to be the current popular term for it, but it doesn't quite linguistically capture the aggression and harsh intensity behind the work.
* I've found that this on/off intensity idea is the most helpful for learning fast and enjoying the process. Every day, at 10am,12pm and 4pm, dedicate 2-hour blocks to aggressively chase down anything you want to work on. Each block should consist of: 90-mins of pure focus and disagreeable intensity on mastering your craft or subject. No talking, no planning, no brainstorming. Just pure action and relentless movement. And then 30mins of just relaxing and doing nothing. 3 of these productive blocks (at 10,12 and 4) means you'll do roughly 4.5hrs of intense work every single day. And then from 6pm+, you can reflect on what you've learnt, cook some steak, drink with friends, daydream, or do whatever you want really... A consistent routine of 3-intense-blocks-per-day will get you further than most other schedules. And, because of Jensen's Inequality and Convexity, you'll probably do better with short intense sprints and long rests, rather than long stretches of medium intensity.
* ALso, interestingly, that disagreeable mindset seems to help you ignore the noise and filter through to the signal when you read papers and books. It sort of gives you 'permission' to skip paragraphs if they're boring or not clear, and that seems to help you piece things together faster (compared to getting stuck on a paragraph or line and wasting time).

---

#### --. Divergence of Intelligence and Aggression over History
* "The society that separates scholars from its warriors will have its thinking done by cowards and its fighting done by fools."
* Historically, in hunter-gatherer times, I think it would be a decent bet to say that the smartest men were probably also amongst the strongest. There was probably some sort of link between Intelligence/Mastery/Skill and Strength/Aggression. I think this is partly because the real 'intelligence' of a man was measured by his ability to fight and hunt and work well within a tribe/coalition.
* Nowadays, there seems to be an anti-correlation here. Some of the 'smartest' nerds seem to have the weakest physiques, while some of the biggest, brawniest and most aggressive seem to lack intelligence and skill.
* Hilariously, if you were to imagine the average PhD candidate with a growing mastery of their field, you wouldn't imagine a lean, muscle-bound warrior with aggression and conviction. And if you were to imagine the average gym-rat, you wouldn't expect them to be much of a poet/writer/thinker.
* Yet if you look at the etymology of 'prowess' and the idea of a martial 'art', warrior cultures have ALWAYS had an emphasis on technical skill mastery. Warrior cultures in the past, ranging from Bushido (Japan) to chivalry in Medieval Europe, never ignored the value of technical skill and mastery and philosophy. In order to be a good warrior, you HAD to have mastered the technical aspects - being a dumb knucklehead wasn't really an option.
* I think it's only recently that the idea of being a 'warrior' (and having strength and agression) has become anticorrelated with skill and intelligence.
* Maybe it's because, nowadays, the majority of intellectual work doesn't seem to need aggression, and the majority of physical work doesnt need intelligence. Special Forces and Professional Sports seem to be the 2 big exceptions that I can think of right now. And maybe being a contrarian thinker or a mafia boss lets you be quite 'aggressive' in your field of work...

---

#### --. Gambling Away Time
* A recent recurring idea that I've seen being used by multiple people is the idea of betting your time.
    * Tim Ferriss - 2 week experiments
    * Basecamp/37 Signals - 6-week bets (from Shape Up)
    * The whole idea of 'experimenting' in your 20s to find the right lifestyle for you is similar to this.
* And another recurring idea that I've seen is to focus on the most important/interesting problem you could be working on, and ONLY focus on that. Everything else should be treated as a distraction.
    * Gary Keller - The ONE Thing: “My life is better when I’m spontaneous after I’ve done my most important thing. Being spontaneous before that, that’s where it becomes a distraction and does me harm.”
    * Marc Andreessen - Pmarca Guide to Personal Productivity: if you don't keep a schedule, you can instead "work on whatever is most important or most interesting, at any time."
    * Paul Graham - Maker's Schedule - this idea implies that a maker focuses on one overarching technical/creative problem, rather than multitasking and focusing on many different, unrelated problems.

So maybe a good approach might be to bet 2-hour-blocks of time to work on the most interesting problem you could work on, every day. 3 or 4 blocks of these per day and you'll probably get more done than usual.

---

#### --. Enjoyment is Time-Dependent and Path-Dependent
* Why is it that the same activity, done under different conditions, can feel entirely different? That's something you should keep in mind when it comes to structuring your work.
* **Time-Dependence**: Something that you enjoy doing for 4 hours might become boring if you are compelled to do it for 8 hours a day. Worse, it might become truly unbearable if you have to *pretend* to do it for 8 hours a day ;)
* **Path-Dependence**: Sometimes, you can only start enjoying working on something *after* you've taken care of the problem on your mind. Until then, you will be distracted and any work you do will feel forced. And sometimes you just need to [do something creative](https://tim.blog/2019/12/18/make-before-you-manage/) *before* you start doing the non-creative work.
* **Intensity-Dependence**: Your enjoyment of something will depend heavily on your intensity of focus. Some things are more fun when you give them your full attention. And sometimes, you can't give something the full attention it deserves unless you *know* your [schedule](http://www.paulgraham.com/makersschedule.html) is free.
* **SITG-Dependence**: And your biggest weakness is that an activity becomes unbearably painful if you have no ownership or skin-in-the-game (SITG) in the outcome. If you're just told to do something, and the quality of the outcome has no real direct impact on your life, there is no way you'll enjoy the process. So aim to work on projects where you have a stake in the outcome, rather than projects that you were told to do in return for a constant salary.

---

#### Violence, Law and the Outsourcing Problem
* Without capacity for violence, or the threat of violence, there would be no way to enforce the law. "A rule not ultimately backed by the threat of violence is merely a suggestion."
* So in a way, the police is just our outsourced 'violence department', through taxes. And we rely on their capacity for violence to maintain any semblance of what we call 'law' and 'ethics'.
* But the problem with outsourcing is that you lose your independence and become overly reliant on others.
* And worse, what happens if the government, the very organisation who you entrusted to carry out violence in your favour, decides to unfairly carry it out against you? Sounds unlikely and unrealistic until you hear the words 'Gulag', 'Communism', 'Fascism' amongst others.
* Now suddently the 2nd Amendent and the American obsession with guns doesn't seem so unreasonable, especially considering the revolutionary roots of the country.

---

---

---

##### --. Intervention vs Post-hoc Analysis
Within fields like Medicine, how much extra data can you collect and 'exploit' through measuring the effectiveness of small actions and interventions, rather than doing one large snapshot statistical analysis after all the treatment is done? How much data granularity do you lose by viewing a complex sequence of events as a single outcome *after* the ordeal? What examples can you find irl?

##### --. 'Universe selection' in statistical modelling
Obvious reminder: if a model doesnt have any predictive power for 100 stocks of various types, maybe the model would start to get more useful if you split the 100 into groups by industry or sector or some other criteria. 

##### --. Entropy in the brain, immune system, ..etc
Is the novelty or unexpectedness of a piece of information related to the amount of entropy it introduces into the neural connections in your brain? If a new piece of information 'affects' you and makes you re-think something that you initially believed to be true, did it introduce a large amount of entropy in your nerve connections? The feeling you get when things just 'click' and make sense - is that related to minimising entropy, or at least reaching some local minima? Maybe dopamine acts as a network strengthening agent, to reduce entropy, in a way...? What about the immune system? Are there any interesting ways entropy and your immune system are linked? Is the novelty of pathogen protein structure somehow related to how seriously your immune system takes it initially? What other biological systems (might) 'respond' to entropy? 

##### --. Temporary Correlations
Consider this situation: the correlation between variables A and B are not always be constant, and fluctuate over time. But if you knew they *did* correlate heavily under certain circumstances, can you *force* them to become temporarily correlated through manipulating the circumstances? What can you do to *temporarily 'crystallise' the correlation between A and B*? And more interestingly, how can you profit from it, before the correlation dissolves away? Is the risk/return ratio worth it? (interesting quote about RenTec that I read on some random answer on Quora: "Someone has to create the correlations in the markets." Don't know how legit it is though.) More importantly though... is correlation even the right tool?...(pls study).

##### --. Monopolistic Poaching of Brains?
If you were a company that was dominating the market in a certain technical field through propietary knowledge(e.g. Deep learning, quantitative trading, search engines...etc) but you didn't want to apply for a patent, and a *very* smart PhD seems to be publishing papers that are scarily close to your trade secrets, would it be profitable to hire them with an outrageous offer? Say, £300k+ starting? The cost of leaving them alone to publish research close to your 'edge' might be much more than the 300k you pay the researcher. Plus, you now have another researcher working with you, AND they probably signed a non-compete to join you anyways, AND they can still be profitable. And they can no longer join one of your main competitors. If Ed Thorp hired Black, Scholes and Merton before they published their formulae, wouldn't he have been able to keep that knowledge propietary for much longer? 

##### --. Information Theory and Quants
Jim Simons, Elwyn Berlekamp, Ed Thorp, Leonard Baum (Baum-Welch algorithm...) and a few other guys - a lot of quants have an Information-Theory background, or at least were closely linked to the subject. Simons was a code-breaker during the Cold War. Ed Thorp worked with ***Claude Shannon*** (!!!) and J.L.Kelly  (Kelly criterion...)for various gambling techniques and tools. Lots of connections to information theory, computational linguistics, code breaking...etc. But when I look at online quant resources, there's hardly any mention of information theory. Instead, a bunch of guys write shitty tutorials on 'Markowitz Portfolio Optimisation' and 'Value at Risk'... strange... Either Information Theory is useless so it doesn't get mentioned often, or it's very useful, so people actively avoid mentioning it. Or more realistically, the quants who are actually making money don't need to write crappy posts and websites like this one (and worse: blogs mentioning anything like 'Efficient Market Hypothesis'). Plus, they're probably not allowed to disclose much information... Also, quite recently, N.N.Taleb has spoken about entropy, mutual information and 'Elements of Information Theory' a few times on Twitter.  So studying Information Theory might be a good bet this year...

##### --. Corruption Questions
* A few questions on institutions and practices that look corrupt. Are they really corrupt? Are they just incompetent? Or am I an idiot and missing something important? 
* Academic Publishing - how comes academic publications get to charge for research behind paywalls when almost all the research was publicly funded through taxpayer money? Shouldn't they be obliged to also publish the pre-prints? 
* Pharmaceuticals, Agriculture and the carb problem; sugar lobbying
* Too Big to Fail problem with Banks...
* 

##### --. (todo) Sleep position and cerebrospinal fluid movement
Learnt something interesting: apparently your sleep position affects how well your cerebrospinal fluid cleans out your brain. Sleeping on your side is most efficient apparently. (brain needs to be cleaned of all its metabolic waste at night). (also: apparently Dolphins can tell one hemisphere to go to sleep, while the other stays awake... Do both sides of the brain get cleared of toxins at the same time? Or only the sleeping side?)

##### --. (todo) Checklists as outsourced intelligence. (a bit like this page... meta..)
Use checklists compiled over months or even years to remind you of the small details that you might forget when making decisions. But careful not to let too many small details overwhelm you though. Maybe checklists should primarily be used for risk-management, to check if you've successfully avoided all the pitfalls? (I think this is what Atul Gawande's 'The Checklist Manifesto' talks about, but still need to read it...). 

##### --. (todo) Dynamics and movement of ideas: a quicker way to learn things?
For some reason I learn faster when thinking visually and spatially, with movement and dyanmics between my ideas. Is that because visually imagining the movement and placement of 'blocks' of ideas activates more parts of my brain at the same time? Or maybe because we're wired to work well with real-world, dynamic objects? 

##### --. (todo) Fragility, Compression, Redundancy and the Levenshtein Distance
In information theory and compression, if you compress a message too much and remove all redundancy, it makes the message that much more fragile and prone to being permanently unreadable after damage. (e.g. the word 'because' can change a letter or two and you can still guess what word it is, since it's long and has quite a few redundant letters. Its 'Levenshtein distance' to the cloesst word is quite large.  But you can't do the same with the word 'cat'. A single letter-change might change the entire meaning.) Similarly, is there redundant code in DNA to make sure mutations aren't too catastrophic? Also: maybe that's a sneaky marketing (or phishing) technique. Make your company or domain name very close to a common typo, and maybe you get more visits? free advertising.

##### --. (todo) Flow of electricity in the brain: Is it deterministic?
Electricity flows down the path of least resistance. Your brain (and maybe consciousness) works because of electrical signals. So does that mean that your mind just thinks of thoughts that sparked through the *path of least electrical resistance*? And so when you form neural connections through learning  (or addiction), is that just an act of carving low-resistance pathways in your brain? And how do you *choose* to take the more electrically resistant path? If electrical flow is deterministic...

##### --. (todo) Writing with blood (Nietzsche).
'Of all that is written, I love only what a person hath written with his blood' - from Thus Spoke Zarathustra. How many of your ideas are actually yours? Are you writing with your own blood? Or, are you mostly regurgitating stuff that you've read? And if so, how can you take ownership of that knowledge? Will you test it in real life - under risk and uncertainty?   

##### --. (todo) Trading and investing ideas: look at mathematical derivatives and integrals, maybe. Instead of absolute values (y), what happens if you look at dy/dt? Or what about dy/dx? Or integrate y w.r.t. t or x, but with limited windows? ...etc

##### --. (todo) Inhibitory wisdom: Risk management and what NOT to do.

##### --. (todo) Inhibitory neurons: the 'corpus callosum' and modulation of neural signals. 

##### --. (todo) Investing in monopolistic businesses - Lesson from both Peter Thiel and Warren Buffet

##### --. (todo) Taleb's Barbell Strategy

##### --. (todo) What to learn: Knowledge vs Trivia

##### --. (todo) Uncertainty in limited doses: curiosity, serendipity, adventure...

##### --. (todo) Motivation and unearned dopamine in the morning; why you shouldn't listen to music until the evening.

##### --. (todo) Productivity Trick: Listen to the same song on repeat. What's the possible neuroscience behind that??

##### --. (todo) A set of highly related traits to work on: 'High Agency' (Eric Weinstein), 'Relentlessly Resourceful' (Paul Graham), 'Extreme Ownership' and 'Default:aggressive' (Jocko Willink), 'Aggressive Tinkering' (Nassim Taleb)

##### --. (todo) Procrastination as wisdom: Is your psyche trying to tell you something? 

##### --. (todo) Filtration mechanisms through opinions: The risks and rewards for being a polarising s.o.b. 

##### --. (todo) Measuring fragility of career choice: How many clients do you have? Sources of demand? Intensity of demand?

##### --. (todo) The Kelly Criterion: Bet sizes for gambling and investing.

##### --. (todo) Lying with Correlation: how can I lie with the simple, well-known measure of correlation?

##### --. (todo) Ethics and virtue as self-imposed constraints: If its not self-imposed out of a sense of self-respect, then is it cheap obedience out of fear?



##### 10. (todo) Evolutionary attractiveness of the 'shadow': Why do people like Anti-Heroes and Femme Fatales?

##### --. (todo) A genuine question about p-values and disconfirmation of knowledge...

##### -. (todo) Disconfirmatory research papers - are there papers like that? 
i.e. 'We couldn't find any results that are definitely 'positively' true, but we managed to show that all these other possibilities are definitely NOT true'. Are there research papers like that? 

##### 7. (todo) The Need to be Activated: Brain regions and a framework for viewing emotions that come from 'lack of something' (e.g. boredom from lack of stimulation, loneliness from lack of connection, agitation from lack of action).
Just like your circadian rhythm cycles through states once a day or so, are there similar cyclical activation requirements in many parts of your brain? Are there parts of your brain that need to be activated once every few hours, or days? Is that the neural basis for emotions like boredom and loneliness - not enough activation of certain regions? Is there an activation requirement for the neural regions associated with aggression and competition? Do we all occasionally need something to fight against - an opportunity to commit acts of heroism or sacrifice? Or are we perfectly fine with comfort, cushy office jobs and mindless consumerism in the evenings? I wonder if this is linked to the accelerating depression rates and mental health issues. If Rafiki (and Mufasa's ghost) didn't remind Simba to heroically take his place in the kingdom, would he have spent the rest of his days feeling existentially anxious, playing video games, uploading social media posts, and watching videos on netflix (or other *less conventional* websites)? 

##### 8. (todo) Viewing psychology through the lens of 'sub-personalities', and being 'possessed' by ancient neural forces that are much older and deeper than you. 
'You don't get angry. *Anger gets you*.' - JBP (Also: you don't get interested. Interesting things *capture* you. It's not your *choice* - you barely have any control over your curiosity. If you had full control of your interest, then procrastination wouldn't exist... You'd just control your emotions to become interested and focused...)

##### 6. (todo) Brain Hemispheres: Structural differences and consequences (esp. for processing novelty + uncertainty)

##### 5. (todo) Dopamine, Play and Hunting: Why do we respect wolves more than rabbits?
(The evolutionary basis of admiration and respect in social hunting animals. e.g. Wolves, Chimpanzees.)

##### 4. (todo) Interconnectivity and Systemic Risk: Pandemics, War and Economic Shocks

##### 3. (todo) The Idiocy of 'Hard Work': Why people who claim to 'work hard' are admitting slavery

##### 2. (todo) The Occasional Virtue of Arrogance: how else can you aim to be creative and contrarian?

##### 1. (todo) The Cheap 'Virtue' of Obedience: roots of totalitarianism and fascism.  



