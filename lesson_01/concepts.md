# Lesson 1 — the concepts, written out

This is what was said in the session, as prose. It is here so you can look something up
without scrubbing through the recording.

**It is not a transcript.** The live demos are not in it, because a demo is something you
watch rather than read. Where the text says "let me show you", that is where a demo
happened; the files to try it yourself are in `data/`.

**Read it after the session, not instead of it.** The exercises in `lab_guide.md` are
where the learning actually happens.

---
<!--
  The spoken words. Read everything that is not in a blockquote.

  A line beginning ▶ RUN DEMO is a cue, not speech. The steps for every demo are in
  demos/demos.md, which is the only place they exist.
-->
<!--
  This file carries the spoken words AND the demo steps.

  Everything inside a blockquote marked DEMO is NOT spoken. It is what you do on the
  shared screen. Those steps are the same text as demos/demos.md. Edit that file, not
  this one, and rebuild.

  Consequence worth knowing: the demo blocks count as paragraphs, so this file is not a
  clean source for cutting into slides.
-->
<!--
  This file carries the spoken words AND the demo steps.

  Everything inside a blockquote marked DEMO is NOT spoken. It is what you do on the
  shared screen. Those steps are the same text as demos/demos.md. Edit that file, not
  this one, and rebuild.

  Consequence worth knowing: the demo blocks count as paragraphs, so this file is not a
  clean source for cutting into slides.
-->
Welcome to the Claude Expert Program. Over the next few months you will learn to use Claude properly, build with it, and design systems an organisation under real scrutiny can trust. Along the way we cover everything the 4 Claude certifications expect, so if your company is an Anthropic partner, you will be ready to sit them.

One thing before we start. You may write code every day, or you may never have written a line and never intend to. Either way you are in the right place, because what I am teaching is the judgement rather than the typing.

You type: write a mail to the client apologising for the delay. What comes back is polite, fluent, properly structured. And it does not know how late you are, or why it happened, or what you are offering instead. So you close it and write the mail yourself, and you think, well, that was no faster.

That is what this part is about. By the end of it you will write prompts that work the first time, and you will know exactly what to do when they do not.

Here is the thing I want you to understand before anything else. When that happened, you asked a one-line question. What came back was not Claude's answer. It was Claude's guess at what you meant. And you judged a tool on a guess.

This is not a beginner's mistake. The more experienced you are, the more exposed to it you are, and there is a good reason for that. You carry an enormous amount of context in your head. The delay is 11 days. The vendor missed a shipment. The client's operations director does not like surprises and she is already annoyed about something else. You know all of that so completely that you forget it is invisible. The more you carry, the more you leave out when you ask.

So we start with how to ask.

But before that, something simpler, and almost nobody teaches it because it looks too obvious to teach. Which Claude are you even in?

A chat is one conversation. It starts empty and it ends. A Project is work that comes back, with standing instructions and your documents attached to it. An artifact is a thing you are going to edit rather than read. Research mode is for when the answer is outside and has to be sourced and linked.

Here is why that matters. When somebody tells me Claude keeps forgetting their context, almost every time what they mean is that they are doing recurring work in a throwaway chat. The tool is not forgetting. They never gave it anywhere to remember.

Let me show you the difference live.

I am going to build a Project in front of you, for something real. I will give it standing instructions, the kind you would otherwise retype every Monday. Watch what goes in: who I am writing for, what good looks like, what the format is. Then I will upload one document that this work always needs. Now I ask a short question inside that Project, and none of that context had to be typed. Compare that with the chat we started in.

A chat is one conversation. A Project is work that comes back. If you take nothing else from this part, take that.

Now, the prompt itself.

Stop thinking of it as a search box and start thinking of it as a brief. Imagine a sharp graduate joined your team this morning. Very capable, knows nothing about your company, your client, or last Tuesday's call. If you walked up to that person and said "write a mail to the client apologising for the delay", what would they do? They would ask you a few questions before touching the keyboard.

A good prompt answers those questions before anyone has to ask them. There are 5.

The first is the simplest. What exactly do you want made? Not something about the delay. A mail, a table, a one-page note, a list of risks. Name the thing.

But naming the thing is not enough, because the same mail reads differently depending on who is writing it. So the second question is, who is writing? Are you the project manager apologising, or the finance lead turning down a discount? Tell Claude which chair it is sitting in.

Now you know what to make and who is making it. The most important question is still missing. Who is reading it? A mail to your own team can say the build broke. The same mail to the client's director says we found a defect in testing, and here is the revised date. Same facts, completely different words, and only you know which reader it is for.

So you have the thing, the writer and the reader. And the answer can still be useless, because none of your actual facts are in there. The delay is 11 days. A vendor missed a delivery. The new date is the 18th. Without those, Claude invents something plausible, and plausible invented facts are the most dangerous output there is.

One more, and it is the one people skip. Say the shape you want. Under 150 words. No bullet points. One paragraph of apology, one with the new plan, one asking for a call. If you do not say the shape, you get whatever shape Claude picks, and then you spend 10 minutes reformatting it.

So, the recap. The task, the role, the reader, the facts, the shape. 5 things, 30 seconds of typing.

Of those 5, I want to single one out. The facts. The other 4 are things somebody can remind you to add, and once you have been reminded you will remember. The facts are different, because the problem is not that you forgot to include them. The problem is that you cannot feel yourself leaving them out. Your own context is invisible to you. That is the habit this whole part is really teaching: noticing what you left out.

Let me show you the difference live.

First I will type the vague version, the one we started with. Look at what comes back. Polite, fluent, and look at what is missing: no date, no reason, no plan. Now I will open a new chat beside it and type the full brief, with all 5 in. Put the 2 answers side by side. Every improvement you can see comes from one of the 5 questions. And the second one is close enough to send after a small edit.

Now, same facts, different reader.

I am going to take that second answer and ask for the same thing for my own delivery team. Read those 2. Same delay, same date, completely different words. Which one would you have written by default?

And format is a choice too, not something that happens to you. Let me ask for the same update as a table for a status report. And now as a document I can edit, open beside the conversation.

That last one is worth a sentence on its own. Anything you are going to edit should arrive as a document, not as text in a chat. If you find yourself copying an answer out of a conversation into Word, you asked for the wrong format.

So you can write a brief. Now, the way you ask should change with the kind of work, and there are 4 kinds.

First, analysis. You have 6 months of expenses and you want to know what is going on. The temptation is to type "analyse this". That gets you a description. Totals, averages, a paragraph of nothing. Analysis needs a question, not a subject. Ask which 3 cost lines grew fastest between April and September, and for each one whether it was price or quantity. Now the answer is useful, because you asked something that has an answer.

That distinction is worth more than it sounds, so let me show you both on the same data.

And while I do, notice the second thing analysis needs, which is the one almost nobody asks for. Tell it to say what it is unsure about. A table of numbers with no uncertainty in it is a table that has quietly guessed somewhere, and you will not know where.

Second, research. Research is about what is true in the outside world, so your prompt needs rules. Say what counts as a good source. Say how recent it has to be. Ask for every claim to carry its link so you can check it. And ask Claude to say plainly when it could not find something, rather than filling the gap. Then hold one rule firmly: anything you did not give it, you verify yourself. We go much deeper into that next.

Let me run a research prompt with those rules in it, and then do the thing almost nobody does, which is open one of the links.

I want you to watch your own reaction when I open it. If you feel a small reluctance, a sense that checking is a bit much, that feeling is the entire reason this is a skill and not a tip.

Third, drafting, which you have already seen with the mail. A draft is judged by a person with preferences, not by whether it is correct. That is why the role, the reader and the word limit matter more here than anywhere else.

Fourth, brainstorming. This is the odd one out, because you do not want the best answer. You want many answers, including bad ones, because the bad ones move your thinking. Ask for 15 ideas, ask for them to be different from each other, and say plainly that you do not want them filtered yet.

And that is where careful people get caught. If you ask for ideas in the same tight, well-shaped way you ask for a mail, you get 5 safe ideas you had already thought of. Precision is right for analysis and wrong for brainstorming.

Let me show you that trap.

Here is the tight prompt: 3 ideas to improve customer retention, under 50 words each. Read those. Safe, aren't they. Now I loosen it on purpose: 15 very different ideas, include unusual ones, do not filter them. Look at the range. There is an obviously bad one, and it has done its job, because it moved where I was looking. And now the second step, which is where the value is: from these 15, pick the 3 most practical for a small team and say why.

Loose first, tight second.

So, the 4 together. Analysis needs a sharp question. Research needs source rules and your own checking. Drafting needs the reader and the format. Brainstorming needs volume and no filter. Same tool, 4 different ways of asking.

Now, what happens when the job is too big?

Say you have 40 customer feedback forms. You need a summary for Monday's management meeting, the top complaints, what to fix first, and a slide-ready version. So you paste everything and ask for all of it in one message.

And what comes back is good. That is the part I want you to sit with, because it is not what you were expecting me to say. It is well organised, it has a table of themes with counts, a ranked list of what to fix, and a slide at the end. If I showed you only that, you would send it.

So let me do something simple. I am going to ask that same question in 2 windows at once. Same data, same wording, side by side, so you can see nothing is different between them.

And the numbers will not match.

Not wildly. One theme will be 7 in one answer and 8 in the other. One of them will count a customer who complained about 2 things under both themes, and the other will pick one. Neither of them will tell you which rule it used unless you read the small print under the table.

Now, which one goes in the board pack?

You cannot answer that. I cannot answer that. Both are confident, both are tidy, and nothing on either screen tells you which is the right count. And notice what is not the problem here. Neither answer is lazy. Neither is thin. The problem is that you asked for a conclusion and got one, and the working was thrown away before you saw it.

The fix is to cut it into steps and run them one after another, each step using the previous step's output. First, read the forms and pull out every distinct complaint. Next, group them into themes and count them. Then rank the themes by how many customers and how much money each one affects. Finally, write 6 lines for the slide.

Let me run that live, and watch for one specific moment.

So here is the same job done as steps. Step 1 does one thing only: pull out every distinct complaint, one per line, no grouping and no ranking.

Look at what comes back. The same customer appears twice. One person complained about being logged out and about a wrong invoice in a single sentence, and now those are 2 lines. A dozen customers did the same thing.

40 comments went in. More than 40 complaints came out, and you can count them, because they are sitting there one per line.

That is the difference, and it is not that this answer is prettier. It is that this one has working you can see. The first 2 gave you a conclusion. This gives you the thing the conclusion was made from, at the one moment when checking it is still cheap.

Step 2, group and count. Step 3, rank. Step 4, the slide.

Now put this slide beside the first one. They will look similar, and this time you know where the numbers came from.

How small should a step be? There is no formula. Here is a working rule: if you cannot say in one sentence what a step should produce, it is still 2 steps.

So you can write a brief and you can break a big job into steps. Both will still sometimes give you answers that are not right. And how you handle that is what separates people who get real value from people who stay annoyed.

You wrote a careful prompt and the answer came back too long and too formal. What happens next decides whether you get better at this or stay annoyed by it.

Most people ask again, maybe adding "no, shorter". Sometimes it works, so it feels like a method. It is not. It is a coin toss, and 3 tosses later you have 4 answers and no idea which prompt produced the good one.

Iterating means something specific. You read the answer, you name exactly what is wrong with it, and you change the prompt so that fault cannot happen again. Then you run the new prompt. The prompt improves. Repeating does not.

So the real skill is in the naming. "It is bad" is not a diagnosis. "It is 400 words and I need 120, it uses words my client will not know, and it never mentions the new date" is 3 faults, and each one turns straight into a line in your prompt. Too long becomes a word limit. Too formal becomes "write it the way you would speak to a colleague you know well". Missing the date becomes putting the date in the prompt, because it was never there.

Let me show you. Here is that weak answer from earlier. I will name the 3 faults out loud. Now watch me turn each one into a line of prompt. A word limit, a tone instruction, and the date itself. And I am going to run this in a fresh chat, not as a reply, because I am not asking again. I am asking better. All 3 faults gone, and I did not have to negotiate.

Now the part I care most about in this whole session.

When an answer comes back wrong, it is one of 3 things, and they have 3 different fixes. Guessing wrong here is expensive, because the usual guess is "use a better model", and that is almost always the wrong answer and the one that costs money.

The first is a prompt failure. You never said it. The date was missing because the date was never in the prompt. Fix the prompt. This is most of them.

The second is a hallucination. You did say it, or it was checkable, and the answer invented something anyway. That is not fixed by rewording. That is fixed by verification, and we spend a whole part on it later.

The third is a model mismatch. Your prompt was right, the facts were there, and the job is simply harder than the tier you chose. That is fixed by changing the model. It is the rarest of the 3.

Let me show you all 3, because telling them apart on a screen is a skill.

Here is the prompt failure, the mail with no date. Ask yourself what is wrong with the model. Nothing. It was never told.

Now a hallucination. I am going to ask for a specific subsection of a regulation, quoted. Look at that. Confident, precise, carries a number. Now I am going to open the actual regulation and check that subsection. Whatever we find, notice what just happened: I had to look. That is the fix, and no amount of rewriting the prompt would have been.

And now a model mismatch. Here is a genuinely hard reasoning task on the cheapest model. Watch it go wrong in a way that is not a missing instruction. Same prompt, unchanged, on the top tier. The fix was the model.

Before you blame anything, ask whether you ever told it. Most of the time, you did not.

Now I want to do something different, because you have watched me for an hour and watching is not the same as knowing.

I am going to put 3 real prompts on screen. All 3 are weak, all 3 are the kind somebody types at 5 in the afternoon. For each one I want you to work out what is missing, and I will take your answer and type it. If you are wrong we will see it on screen together, and that is more useful than being right.

You are looking for the same 5 things every time: the task, the role, the reader, the facts, the shape. And the question underneath all of them: what does this person know that they have not said?

One last habit at this level, and it costs nothing. When you finally get the answer you want after 5 rounds of correction, go back and write the one clean prompt that would have produced it, and save that. That is the prompt you reuse next Monday. Five rounds of "no, not like that" leaves you a conversation nobody can reuse.

Everything so far is what you do in the product. Now I want to show you the same ideas from 3 more directions, because the same skill looks different depending on where you are standing. If you do not write code, stay with me: you are not going to be asked to type anything, and the last 2 of these are decisions, not keyboards.

Start with code.

When you call Claude from your own program, the prompt stops being one message. It has parts, and where you put things matters.

Standing instructions, the role, the constraints and the format go in the system prompt. The material for this one request goes in the user turn. If you put the role in every user message instead, you get 2 developers producing 2 behaviours from one feature, and nobody can say which is correct.

When the request carries a long document, the document goes above and your question below. That is a real effect and it is free.

When a prompt mixes different kinds of material, label each one. Wrap it, tag it, make the boundary explicit. It looks fussy on screen and it stops your instructions being confused with your pasted text.

Now the serious one. Any text that arrived from outside is untrusted. A customer mail, an uploaded PDF, a scraped page. It is sitting inside your prompt, and it can contain instructions. So you fence it, you label it, and you say in the prompt that nothing inside the fence is an instruction. We go at that properly later in the course. The habit starts now.

If code downstream is going to read the answer, state the shape and then check what came back. Never assume.

And one piece of vocabulary you will meet everywhere. Zero-shot means no examples. Single-shot means one. Multi-shot, usually called few-shot, means several. About 3 works well. Past 5 it stops helping. And the useful version of that: examples beat adjectives. 2 real examples of the mail your team already sends will outperform a paragraph describing the tone you want.

Now 2 things that are easy to say and surprisingly hard to do.

The first is instruction clarity, and it has a precise meaning that is not "write clearly". It means an instruction that can only be read one way. Here is the test I use. Read your own instruction and ask whether a careful person could follow it correctly and still give you something you did not want. "Summarise this briefly" passes as English and fails that test: brief is 3 lines to me and a page to you. "Summarise this in under 80 words, as 3 bullet points, for somebody who has not read the document" cannot be misread. Every ambiguity you leave is a decision you have handed over without meaning to.

The second is where the instruction goes, and this one catches people who have been building for months. You are not writing one prompt any more. You are writing instructions that live in several places at once, and they do not all behave the same way.

In a chat, everything is one conversation and the newest instruction tends to win. In a Project, the standing instructions sit above every conversation in it. In Claude Code, there is a file of rules that applies to a repository, and rules that apply only inside certain folders. Through the API, you have a system prompt that is separate from the message. And a Skill carries its own instructions that arrive only when it is invoked.

The failure mode is always the same, and it is worth recognising from a long way off. Somebody puts a rule in one of those places, sees it ignored, and concludes the model does not follow instructions. The model followed instructions. It followed a different one, from a place the person had forgotten was also speaking.

So when something behaves strangely, before you rewrite anything, list every place an instruction could be coming from. Let me show you what that looks like.

Now the third direction, and the question changes.

As an architect, you are not asking whether this prompt is good. You are asking whether a system can depend on it. One prompt, running unattended, thousands of times, with something downstream trusting the answer.

That changes what you write. "Flag anything suspicious" produces a flood nobody reads. So you state what counts, what does not, and what the edge cases are. And now you have something you could not have before: a number. The false positive rate, before and after. That is the first time in this part that a prompt has evidence attached to it rather than an opinion.

Few-shot changes meaning here too. For you, examples made one answer better. For an architect, examples stop 10,000 answers drifting in shape. Same technique, completely different reason.

So if you are ever asked to show that you improved a prompt, 3 things: the criteria written down, the false positive rate before and after, and the examples that pin the shape. Without those, "I improved the prompt" is a claim with nothing behind it.

And the fourth direction, which is about money and about the organisation.

As an owner, the question is not whether one prompt works. It is whether your organisation has one prompt or 40.

The system prompt is where the house voice lives. What you always refuse, what format you always use, who you write for. Let me show you what that looks like.

I am going back to the Project we built at the start. These instructions here are a system prompt. Not a message you send, standing behaviour. I am going to add one rule to it: never state a delivery date I have not given you, ask for it instead. Now I will make a request and deliberately leave the date out. Watch it ask instead of inventing.

Now I want to be careful here, because this is where people get a wrong idea. That is a guardrail shaping behaviour. It is not enforcing anything. A determined input can still get round it. Real enforcement is a separate subject later in the course, and confusing the two is how people end up trusting a sentence to do a security job.

Three things make a prompt an asset rather than a message. Modular prompts, assembled from parts, so one house style exists instead of 40 private ones. Caching, so a long unchanging prefix, like a policy document in front of every question, is not paid for every single time. And Skills, so a capability is defined once and invoked rather than pasted.

And one more that sounds boring and is not. Prompts belong in source control with an owner, treated like a code change. If somebody complains about something you sent last month, and you cannot say which version of the prompt produced it, you cannot investigate.

Last thing on this. Deciding how precise to make your criteria is yours. Deciding what false positive rate is acceptable is not: that is a business decision about who reads the flags and what it costs them when they are wrong. Put a number in front of that decision rather than making it quietly.

So, where you have got to.

You can write a prompt that names the task, the role, the reader, the facts and the shape, and get something usable first time. You can pick the right surface instead of doing everything in a chat. You can take a big job that used to be one hopeless paste and run it as steps you can check. You can look at a disappointing answer, say exactly what is wrong with it, and change the prompt so the fault cannot recur. And you can tell a prompt problem from a hallucination from a model mismatch, which is the one that saves you money.

One thing to take away and do. Pick a task you do every week and write down what a good version of it looks like. Not the steps. The test. How you would know the finished thing was right.

Almost nobody has ever written that down, and that is exactly why prompting feels like luck. If you cannot say what good looks like, you cannot put it in a prompt, and you cannot tell whether the answer is any good.

So here is the whole session on one card, and if you remember nothing else, remember this.

Name 5 things: the task, the role, the reader, the facts, the shape. The facts are the one you will forget, because your own context is invisible to you.

Match the asking to the work: a question for analysis, source rules for research, a reader for drafting, volume and no filter for ideas.

When it is too big, cut it into steps and check each step before it spoils the next.

When it is wrong, name the fault and change the prompt. Do not ask again. And before you blame the model, work out which of the 3 it is: you never said it, it invented something, or the job is harder than the tier.

And when you finally get the answer you wanted, save the prompt that produced it.

The lab guide has 10 exercises and they are all on your own real work, not toy examples. If you only do one, do the Project. It is the one that changes a working week.

And coming up, one of the most important skills for real work. You will get Claude to quote a regulation confidently, right down to a subsection number, and then you will check whether that subsection even exists. So bring a little suspicion.
