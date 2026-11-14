# Try it yourself — every demo from the session

These are the same things I did on screen, written so you can do them.

Work down the list in order. Each one takes 5 to 10 minutes and they build on each other:
the Project you create in number 3 is used again in number 8.

**Model: Sonnet 5.5, Medium** unless a step says otherwise. Check the picker before you
start, because it does not reset when you open a new chat.

**Where there are 2 windows, use 2 browser windows side by side, not 2 tabs.** You need to
see both answers at once.

---

## 1. The vague prompt beside the full brief

1. New chat. Type exactly:

   ```
   Write a mail to the client apologising for the delay.
   ```

2. Read what comes back. Before you go on, write down what is missing.

3. Second chat. Type:

   ```
   You are a project manager writing to the client's operations director. Our delivery is 11 days late because our hardware vendor missed a shipment. The new date is the 18th. Write a mail under 150 words, in 3 short paragraphs, no bullet points, that states the delay, gives the new date, and asks for a 15-minute call this week.
   ```

4. Put them side by side and find each of the 5 in the second answer: the task, the role,
   the reader, the facts, the shape.

**What to notice.** Every improvement came from one of the 5. None came from a better
model.

---

## 2. Same facts, 3 readers, then an artifact

Stay in the second chat from number 1. Do not start a new one: the point is that the facts
are already there.

```
Same facts. Now write it as a 3-line Teams message to my own delivery team.
```

```
Now the same update as a table I can paste into a status report: what slipped, why, the new date, and what we need from the client.
```

```
Put that status report in a document I can edit.
```

**What to notice.** Same delay, same date, same vendor, and barely a shared phrase between
the versions. And the last one opens a document beside the chat rather than text inside it.

---

## 3. Build a real Project

**Do this one on your own work, not on mine.** It is the exercise that changes a working
week.

1. Left sidebar, **Projects**, then **New project**. Name it for something you do every
   week.

2. Right-hand panel, **Instructions**, then **Edit**. Write who you are writing for, what
   good looks like, and what you never want. Mine was:

   ```
   I write a weekly status report for the operations director at our largest client. She is not technical. She wants the decision first, then the reason, then what she needs to do.

   Always: lead with what changed since last week. Use plain English, no jargon, no bullet lists unless I ask. Keep it under 200 words.

   Never state a delivery date I have not given you. If a date is missing, ask me for it.
   ```

3. Same panel, **Context**, then **Add**. Upload 2 files: what you produced last time, and
   the reference the work always needs. To copy mine exactly, use
   `data/last_week_status_report.md` and `data/delivery_plan_reference.md`.

4. Start a chat **inside the Project** and give it only the new facts:

   ```
   Draft this week's update. The integration testing finished on Tuesday and found 2 defects, both fixed. The vendor shipment is still outstanding.
   ```

5. Now open a **normal chat**, outside the Project, and paste the identical message.

**What to notice.** Compare the two. One of them knows who the reader is, how long to be,
and what happened last week. The other asks you for the project name.

**Keep this Project.** Number 8 comes back to it.

---

## 4. The same question twice

1. Open `data/customer_feedback.csv`, select all, and **paste the rows** into a chat. Do
   not attach the file.

2. Underneath them, type:

   ```
   Summarise these, give me the top complaints, tell me what to fix first, and write a slide.
   ```

3. Do the identical thing in a second window. Same rows, same instruction, nothing changed.

4. **Compare the theme counts in the two answers.** Write them down.

**What to notice.** They will differ, and neither will tell you which counting rule it
used. Ask yourself which one you would put in front of your management.

5. Now a third chat. Paste the rows again, then:

   ```
   Here are customer feedback forms. Pull out every distinct complaint as a flat list. One complaint per line. Do not group them and do not rank them yet.
   ```

6. Scroll that list. Look for the same customer id appearing twice.

7. Then carry on, one step at a time, in the same chat:

   ```
   Group those complaints into themes. Count how many forms mention each theme.
   ```

   ```
   Rank the themes by how many customers they affect and how much money is at stake. Say which ones you are least sure about.
   ```

   ```
   Write 6 lines for a management slide from the top 3 themes.
   ```

**What to notice.** The first 2 answers gave you a conclusion. This one gives you the thing
the conclusion was made from, while checking it is still cheap.

---

## 5. Three named faults become 3 lines of prompt

Go back to the weak mail from number 1. Do not generate a new one.

Write down exactly what is wrong with it, as separate faults. Not "it is bad". Something
like: too long, too formal, no date.

Now open a **fresh chat**, not a reply, and turn each fault into a line:

```
You are a project manager writing to the client's operations director. Our delivery is 11 days late and the new date is the 18th. Write a mail under 120 words. Write it the way you would speak to a colleague you know well, not formally. Include the new date.
```

**What to notice.** You did not negotiate. You asked better once.

---

## 6. The brainstorming trap

```
Give me 3 ideas to improve customer retention, under 50 words each.
```

Now a new chat, loosened on purpose:

```
Give me 15 very different ideas to improve customer retention. Include unusual ones, ones most companies reject, and doing nothing. Do not filter them.
```

Then, same chat:

```
From these 15, pick the 3 most practical for a team of 4 with no budget, and explain why.
```

**What to notice.** Compare those final 3 against the first answer's 3. In the session,
none of them had appeared in the first list at all.

---

## 7. Three wrong answers, three different causes

**This is the most useful one on the list.** When an answer is wrong it is one of 3 things,
and they have 3 different fixes.

**A prompt failure.** Look again at the weak mail from number 1. Nothing is wrong with the
model. It was never told the date.

**A hallucination.** Ask for something specific you can check:

```
Which subsection of the DPDP Act sets out the consent requirements for processing a child's personal data? Quote the exact wording.
```

Then **open the actual Act at indiacode.nic.in and look.** Whatever you find, notice that
you had no way of knowing without looking.

Then ask the question that works:

```
What did you not check?
```

Not "how confident are you". A confidence score is another fluent sentence from the same
process. "What did you not check" gets you a list you can act on.

**A model mismatch.** Switch the picker to **Haiku 5.5**, paste the puzzle from
`data/hard_reasoning_task.md`, and read what comes back. Then switch to **Opus 5.5** and
paste the identical prompt.

**Set the picker back to Sonnet 5.5 afterwards.** It does not reset itself.

---

## 8. A prompt becomes an asset

Go back to the Project from number 3. Open its **Instructions**.

That is a system prompt. Not a message you send, standing behaviour.

Find the line you wrote about never stating a date you have not given. Now start a chat in
the Project and deliberately leave the date out:

```
Draft an update for the client about the vendor delay.
```

**What to notice.** It asks instead of inventing. And be clear about what that is: a
guardrail shaping behaviour, not enforcing it. A determined input can still get round it.

---

## 9. One instruction, 3 places

In a chat, mid-conversation:

```
From now on, never use the word "leverage".
```

```
Write 2 short paragraphs about getting more value from our existing tools.
```

Then change the subject entirely and come back to it later in the same chat.

Now put the same rule in a Project's instructions and start a fresh chat inside it. You did
not have to say it.

**What to notice.** When a rule seems ignored, the model usually followed a different
instruction from a place you forgot was speaking: this message, earlier in the
conversation, the Project, a repository file, a system prompt, a Skill.

---

## 10. "Analyse this" beside a question that has an answer

Paste `data/monthly_costs.csv` into a chat, then:

```
Analyse this.
```

Read it, then ask yourself: **what question did it decide to answer?** It picked one,
because you did not. Is it the one you needed?

Now a new chat, same data:

```
Which 3 lines grew fastest between April and September? For each one, say whether the growth came from price or from volume. Tell me which of the 3 you are least confident about and why.
```

**What to notice.** The last sentence of that prompt is the part almost nobody adds. A
table of numbers with no uncertainty in it has guessed somewhere and not told you.

---

## 11. Research with rules, then open the link

```
What has changed in India's rules for processing children's personal data in the last 12 months? Use only official sources or established legal publications. Give every claim its own link and the date of the source. If you cannot find something, say so plainly rather than filling the gap.
```

**Now open one of the links.** Do not choose the one that looks safest.

**What to notice.** If you felt a flicker of reluctance about opening it, that feeling is
the thing the next session is about.

---

## 12. Fix these 3 prompts

For each one, work out what is missing, rewrite it, and run both versions.

```
Write a job description for a data analyst.
```

```
Summarise this meeting transcript.
```

```
Make this email more professional.
```

**The third one is the interesting one.** Ask 4 colleagues what "more professional" means
and you will get 4 answers: shorter, less apologetic, no slang, a more formal greeting. If
4 people mean 4 things, the model had no chance.

---

## When you are done

The exercises in `lab_guide.md` are the ones that matter most, because they are on your own
work rather than mine. This list is for replaying what you saw; that list is for building
the habit.
