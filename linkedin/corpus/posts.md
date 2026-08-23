1. Everyone is asking whether AI agents can write error free production code. I spent the last year on a narrower question: can they hold a standard over hundreds of hours without a human watching?

The common instinct is to write better prompts. I wanted to test something else, so I built an operating framework around the model instead: one Claude Code session acting as a CTO, orchestrating 12 specialist agents across 8 execution cycles, with enforcement moved out of prose and into code hooks that block an action until its gate is met.

Then I used it to build something real. TaskIt is a project and task management platform, built in-house at Fortes Investment, in the class of Asana or Monday.com. It is live in production: around 150 users onboarded through Microsoft accounts on the way to a 1,500+ person organisation, currently carrying 73 active projects and over 1,100 open tasks across 53 channels.

Three things I found:

→ Prompts do not hold. Rules written as instructions were followed roughly 14% of the time. The same rules enforced mechanically at the hook layer held at ~97%. Capable models make sharp judgments, but they do not self-prompt.

→ Review has to come from somewhere else. Every change is checked by a different agent than the one that wrote it, including live testing against the running application. Self-reported success is not evidence.

→ Incidents are the real specification. Each failure gets converted into an automated guardrail, so the same class of mistake cannot ship twice. The framework got stricter every time it was wrong.

The takeaway for anyone building with agents: spend on structure before you spend on model capability. The ceiling is rarely the model.

What I took away personally: the hard part was not orchestration, it was learning where LLMs go non-deterministic over long autonomous runs, and what it takes to pull them back. Design decisions and final verification still sit with me. I rule on every design, read every database change before production, and test each release myself. The framework earns autonomy inside those lines, not outside them.






2. I wanted to see if Claude Code could really run unsupervised for 18 hours straight on production code

Planned out the exact scope of work, exact execution cycle, exact feedback based loops

then incorporated my framework for building production code

imagine returning to an "API overload" message

ill build a timer to retry

Enjoy this picture of my Mini's lower control arm


3. Claude Ultra Code


Close followers of my Production Framework assumed Claude UltraCode just killed what im building

It didnt

UltraCode is real, by the way
It can deploy multi agent workflows on its own now
Thats a genuine step up from wiring your own agent system together by hand

But it solves a different problem than mine

UltraCode can build the agents and run them
It doesnt decide how a team of agents works together inside a company

Who owns what
Who checks who
How they hand off before something ships

Thats not a deployment problem
Thats an org problem

A CTO agent, QA, builders, researchers, all coordinating like a real team
Thats the layer ive been building for months

So im not competing with UltraCode
Im building on top of it

It runs the engine
My framework runs the team

Not a screenshot







4. What do you think?


Three words that have fixed more of my Claude Code sessions than any prompt trick

Heres the situation

The model writes something
Its wrong, or half nonsense, and it doesnt even notice
Correct it directly and it gets defensive, patches around the mistake, makes it worse

So I stopped correcting it

Now I just ask: what do you think?

And it stops
It reads its own output again like its seeing it fresh
Half the time it goes wait, this is wrong, and rewrites the whole thing itself
The other half it sharpens what was already there

Same model, same context, one question

Works way better on Opus 4.7 and 4.8
The self reflection is just stronger there

If you live in Claude Code like I do
Ask what do you think more often

Let it catch itself











5. This is exactly it.



as I have said before

AI is never replacing people not doing brain dead work

Its crazy how people can look at AI negatively

it makes sense, we've been trained to be labour from school, to college, to corporate offices where you punch in and punch out times like good boys to get paid

but now is the era we've dreamt of.

where AI takes over all the boring stuff and we do what's interesting

let it take over the boring stuff

do something interesting.









6. LLMs are like women....


Cant live with, cant live without.

Theyre the best thing thats happened to my life.

I'll talk about LLMs for now.

Stuff i thought would take lifetimes to build now takes me a month.

i never thought id be building enterprise grade apps for thousands of users, from scratch.

But here we are.

However....

LLMs drift.

You can start a session perfectly.

Clean output.

Tight reasoning.

And 4 hours later youre staring at nonsense.

Doesnt matter what you put in your prompts.

Doesnt matter how many sub prompts you stack.

im learning the trick is to cut it short.

Restart mid session.

Fresh window every time the model starts getting weird.

But im lazy.

Very.

So im just baking it into my production framework.

Ill let you know if it works 💀











7. Claude Code is sh*t.

The LLM is excellent.

The context management is the problem.

Give it a big task. It tries to do the whole thing by itself, all at once.

It overloads its own context window. The attention mechanism that separates signal from noise breaks down. Signal doesnt disappear. It gets diluted into the noise.

The output looks confident. Its wrong in ways that arent obvious.

Thats the kind of thing that gets screenshotted and sold.

So heres what im building instead.

A production framework. No name yet.

Think of it as a standalone company built around a single SaaS.

CTO. Product manager. Architect. Builders. QA. Researchers.

All agents. All coordinating.

The rule: nothing gets implemented unless theres a research-backed precedent. Open source tools. Competitor implementations. Real things that have already shipped.

No hallucinated architecture. QA on every implementation. UX testing directly through the browser via Playwright. Automated.

Im testing it by building with it.

A full multitenant SaaS for task management. AI integrations. Full automation engine. Competing with Asana and ClickUp. Solo build. Real users.

Also a vendor email scraping pipeline. Open source rules. Parses Outlook emails and pulls exactly what the user needs. No manual triage.

Both shipped.

Not a screenshot.











8. AI is too stupid to replace humans.

Unless we're talking about humans doing brain dead tasks.

There's a difference.

The ones panicking right now cant explain what they do beyond "i manage spreadsheets" or "i send emails" or "i update this one report every Friday."

If that's your answer, AI isnt your problem.

That answer was always the problem.

The MD pulling 14 hour days. The founder who knows every single customer by name.

They are not getting replaced.

They'll use AI and run circles around everyone who was doing brain dead work before AI even showed up.

A hammer didnt replace carpenters.

It replaced the people moving nails with their thumbs.

They said the hammer was a threat too.

ofcourse they did.

















9. Most AI agent demos are sh*t.



A working POC and a screenshot.

That's all they have.

They have not used it themselves. They have not run it for three months. They have not generated their own income with it. They just promise it'll change your life and ship the screenshot.

I despise these people.

The ones they sell to are MDs, founders, CEOs.

The hardest working people in any company.

They dont have the luxury of being nonchalant. Its their business on the line.

I work directly with one of them. Ajay Mankani. Hardest worker in our entire org, day in day out.

He doesnt deserve a screenshot.

So heres what im doing instead.

Two builds. Neither for sale yet.

One is a LinkedIn skill. Claude runs my LinkedIn against my own AI-tells research. Voice-aware. Approval-gated. It only talks about things i actually care about.

Two is the flagship. A production framework that lets Claude build enterprise software ground up. Multi-tenant. Real users.

How am i testing the framework?

Im building another product with it. Solo. Ground up. Real users, real data. Its called TaskIt.

ofcourse it has bugs.

Last week the framework caught one before it shipped. Would have shown one customer's tasks to another customer. Claude tried to ship the fix. The framework rejected it and pointed back to the original incident in its own catalog. Done.

Thats how you know if a framework works. Not a screenshot.

Im not selling either of these.

Ill start when ive been the first one bitten by everything wrong with them. Until then, the catalog grows.









9. Hot take: I dont think anyone wants to be rich.

Everyone wants to be operationally useless.

They want a money printing machine you set up once (with blood sweat and tears ofcourse)

But then pull back from it....

And keep getting paid

That's the business dream, right?

But if that's your goal from the start...

Maybe don't start just yet.

Why can this 23 year old punk talk about this?
 
Because he has been lucky.

Lucky enough to work with UHNWIs.

Including directly.......with a Billionaire.

There are about 3000 billionaires in the entire world.

Let that sink in.

So then how's this one like?

He's smart, very. He knows everything about everything while still calling himself the biggest idiot.

He's an EXCELLENT communicator, if he explains something to you, you can't not understand it. (I can not stress how deviously good he is with this).

He's the most humble person AND commands insane respect all at the same time.

I could go on and on, he's not normal.

Not your normal topper, hardworker, genius.

But everything I mentioned above?

I have somehow met 2 more just like that. (I'll be buying lottery tickets)

Super impressive people ofcourse, but their net worth?

💀 

Middle class 

So then, whats the difference between being worth $300k and making $300k a day?

What creates the $999,757,773 difference?

Ill tell you.

This guy set the bar for the most insane work ethic I have ever seen.

He is voraciously obsessively hard working.

When you watch him in a moment of crisis...

He looks like he's almost enjoying it.

Another puzzle to solve, another demon to slay.

As if he has decided that life looking any other way, specially as a retired 60+ person on a beach mansion is the real bore.

ofcourse he has dedicated staff and heads of departments with their own visions and capabilities to lead growth.

They work their shoulders off, each one

But no one can confidently ever say....

"I worked harder than Ajay today"

So is being operationally useless possible?

Yeah.

Does he look like he wants to be?

Only for the boring stuff.

The repetitive stuff that should be a system.

But the real problems? The messy ones? The “oh sh*t” moments?
He’s there.

The constant growth leader?
It's him.

And that’s what I learned:

If you’re in business, some part of you has to actually enjoy the fight.

Not the cars.

Not the vacations.

Not the “money printing machine” fantasy.

Because the machine only prints…

after you become the kind of person, who thrives when it breaks.










10. Can AI be too smart?

We built an AI system that was exactly that

The idea sounded perfect

Automatically ingest any database
Turn every table into vector context
Make the entire company’s data queryable in plain English

Automatic reports
World-class data science

Any DB
Any Table
Any Schema

We ran LLMs on headers and data samples, inferred relationships, predicted what each table could answer, and stored that as metadata in a Qdrant vector store

Inspired by Neo4j
The prototype worked beautifully

I was ready to scale

Then I spoke to someone who builds AI systems for large enterprises

He asked one question:

“What happens when multiple tables have the same headers, random names, and completely different purposes?”

With 2,000+ tables, that’s not an edge case
That’s just reality

I asked if we just manually add context for every table

He said: “How many different queries do you think people will actually run?”

In the first month, everyone experiments.
Everything feels magical

But over time?

Those queries collapse into a few patterns: fetch, summarize, compare, identify

That’s when it clicked.

Why I failed, and why 97% of AI startups fail

Real AI systems don’t fail because they aren’t intelligent enough

They fail because they assume the world is clean

The solution wasn’t more intelligence
It was constraint

Collect the most common queries
Make them explicit

Let the LLM choose between validated intents

Minimum viable system
Maximum reliability

If your AI needs perfect data to work, it’s already broken

And if it's really 'elegant', you might need to rethink















11. If you walk into an AI interview without using AI… you’ve already failed the test.

I’ve given 5 AI engineering interviews this month.

On the day of the first interview, I woke up at 5 A.M.
Meditated, fasted.

Quietly prepared for the typical AI technical interview:
• Python fundamentals
 • DSA
 • Maybe a small LeetCode-style test
 • Agentic frameworks, deployment, CI/CD

I was confident, expecting the usual.

2 P.M, I am outside office.

Calmly, I walk in and sit infront of this CEO with deep blue eyes and no time.

"How familiar are you with cursor?"

I froze for a second.
 Wasn’t that supposed to be engineering cheating?

"A little bit, not too much"

I thought that was the proud, hardworking answer.
The “real engineer” answer.

But he leans forward.
"I have seen your projects, but you'll have to prove to me you can use cursor for this job."

from there, he was super specific:
“Which LLM do you use within cursor? Why?”
“Which MCPs are you most productive with?”

He then asked me to build something end-to-end, right there.

That’s when it clicked.
It’s no longer: Show us you can code.
It’s now: How fast can can you produce?

ofcourse they want you to use autocoders.

Because to companies today:

A great engineer isn’t just the one who writes clean Python…
but the one who ships fast.

You bet after that interview, I dove deep.

If you write any code.....ever, this is your new toolkit:

1️⃣ Context7 - Keeps Cursor aware of latest packages + docs so dependency hell disappears
2️⃣ Browser / BrowserBase - Lets Cursor search docs + web in real time for better reasoning
3️⃣ Project context tools (NPX etc.) - Give AI full structure awareness to avoid wrong links
4️⃣ Claude Code (Sonnet 3.5/4.5) - Best auto-coding engine right now (Cursor paid tier)

And the wild part?

Every interview after that…
Cursor, MCPs, and how fast you can ship always had a part

ofcourse you can't go in completely reliant on AI, your project wouldn't handle 2 edge cases.

It is a fine balance.

The new skill, as Mr Big Brain Basil Fateen made it clear to me:
 Adaptive learning. Good judgement at high velocity.
 Knowing when to build, and when to let AI build with you.

So if you’re still treating Cursor like cheating…
you’re already behind.








12. Yesterday taught me that you grow fastest when you walk into rooms you don’t know yet.

I went to Hub71s event alone.
Took a taxi to ADGM at noon, no agenda except to learn and meet a few people.

First person I met was Jobin Johnson, a data scientist.
We just started talking in the elevator and somehow, we were already deep in a discussion about safe AI pipelines.

He shared how you can maintain low latencies even when you run constant input-output checks.

One cool thing, how giving less context sometimes makes LLMs hallucinate less.

Wild, all they tell you nowadays is to give as much as you can, and it made sense.

Then on stage came Karim Davis Dib, the most goated mentor in the world.

He spoke about how founders should be a problem looking for a solution, not the other way around.

Simple, but it hit hard.

After that, Baris Yesugey, Google’s Startup Accelerator Lead, shared how Google helps founders go from A to Z kind if like walking in the sun for 60 minutes vs an AC taxi. Super knowledgable.

Basil Fateen, Tech Evangelist at AWS, was next and his energy filled the room.

He spoke about how we’re finally entering the age of enlightenment for GenAI
The phase where we’re learning its limitations, not just chasing its potential.

He said something that stuck with me:

“Adaptive learning and good judgment at high velocity — that’s the most important skill for founders today.”



After the talk, I went to meet both Baris and Basil.

Baris gave me direct feedback on my secure AI idea, helping me see where:

1. The real problem lies
2. A real use case
3. And I am going to be reaching out to him many many times.

And Basil… well, that turned into 3 guys discussing context, tech, shared memory, strands, and having the time of our lives.

It was me, Basil, and Moudjahid Moussa, a very cool young inmovator working on very innovative edtech, and we ended up somehow concluding nobody knows sh*t, experiment and learn.

Later, I even got to see Daymond John from Shark Tank speak live.

But honestly?
The highlight was the people.

I ended the evening in the Apple Store next door, talking for an hour with Andrés Campos, one of the smartest and most passionate tech minds I’ve met working on the most innovative product idea i have heard.

an automated netflix style series on you

Didn’t eat much even though there was food.

Too many conversations, too much to take in.

Walked in alone.
Walked out with ideas, mentors, and friends.

Not bad for a Tuesday afternoon.

And I am going to be meeting all of them again.








12. I Think I Finally Get It.
People are the most valuable currency you own.

I’ve heard that before, but only recently did I feel it.
Lately, I’ve seen how fast you grow when you’re surrounded by the right people.

Even the smallest efforts start to catch fire.

And on the flip side, how being around the wrong ones can water down your energy, your ideas, and even your momentum.

It’s strange, because nothing else changes.
Same work ethic. Same ambitions. Just better company.

I’ve started to notice it in everything, friendships, partnerships, even random conversations.

The right people make things move. The wrong ones make things heavy.

It’s made me realize it’s worth putting in extra effort to find, and keep those few people who bring out your best.

Even if that means disconnecting from a hundred who don’t.
Because even just one good person beside you can change your entire pace.

I’m genuinely grateful for the few who’ve done that for me lately.
They’re rare

they make all the difference.

And I hope I can do the same for them.


















