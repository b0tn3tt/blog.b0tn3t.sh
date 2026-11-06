---
title: "Your security awareness quizzes measure nothing"
date: 2026-11-06
draft: false
categories: ["security-awareness", "red-team"]
tags: ["awareness", "social-engineering", "red-team", "phishing", "human-factor", "opinion"]
summary: "Multiple-choice security tests don't measure how protected you are. They measure your ability to guess the 'right' answer. And firing people who 'fail' punishes honesty and destroys your own data. Here's why, and what to run instead."
images: ["og-awareness-en.png"]
ShowToc: true
TocOpen: false
---

I'll say it straight, no long intro: **a corporate multiple-choice security quiz doesn't measure how protected you are. It measures your ability to pass quizzes.** Those are two different skills, and there's no link between them.

And if you're planning to dock someone's bonus or fire them based on that "test," you're doing something not just useless but harmful. Let me break down why.

## Where multiple-choice falls apart

A multiple-choice security quiz is built so that **the right answer is obvious from the way the question is phrased**. Not because the person knows the topic, but because the "safe" option is always written to sound like the most responsible, tedious, cautious one next to the rest.

A classic:

> **Your "boss" DMs you: our service is down, we need to fix it ASAP, send me the server credentials.** What do you do?
>
> - **A.** Send them right away, the boss is asking
> - **B.** Ask again in the same chat and send
> - **C.** Call a known number, confirm it's really them, and only then decide
> - **D.** Ignore it

Any reasonable person picks **C**. Not because that's what they'd actually do, but because next to the other options, C simply looks like the most sensible and correct one. This isn't a security question. It's a reading question.

Now an honest question for you: **are you really sure that at 2:50pm on a Friday, when the "boss" is frantically typing in all caps about a burning prod server, your employee will actually go look up a number and call?** Sitting at a test, calm, they'll of course pick the "right" option. But in a real attack, under pressure and in the chaos, most people won't. They'll give in to the panic and send it anyway. So the test showed one thing, and in reality the person behaves completely differently. That's why the metric is worthless: it measures behavior in greenhouse conditions, not in combat.

### Why this happens, and it's not stupidity

Two well-studied effects are at work here, and neither is about intelligence:

- **People answer the way they "should," not the way they'll act.** When you're being evaluated, especially with a bonus or your job on the line, you pick the answer that's expected of you, not the one that reflects your real behavior.
- **Knowing and doing aren't the same thing.** Understanding that phishing exists is easy. Not clicking it while you're digging through 80 emails under a deadline is a different matter entirely. A test checks only the knowing, not how you'll act in the moment.

When a "wrong" answer means a warning or getting fired, people stop answering honestly. They just pick the option they're expected to pick. The company spends money and time, and what it gets isn't a picture of real security, but a set of pre-guessed "right" answers. That's not a security check. It's a box-ticking exercise.

## Why punishing the people who "fail" is worse than nothing

This is where it goes from merely useless to actively harmful.

Picture an employee who actually took the test seriously. They didn't guess the "right" option. They honestly imagined: *how would I really act if this happened to me on a Monday morning?* And they answered honestly: "yeah, I'd probably send it, if it's definitely my manager and it's urgent."

And you punish them for that.

Think about what you just did:

1. **You punished honesty.** The one person who gave you truthful data about real behavior is the one you dinged. Everyone else lied "correctly," and passed.
2. **You trained the whole company to lie to you.** Next time, the honest one will guess like everyone else. You've destroyed, with your own hands, the only source of truthful data about how people actually behave.
3. **You confused an honest admission with an incident.** Someone who admits their own vulnerability is an asset, not a problem. These are exactly the people who come and say "I think I clicked something weird" at minute 11, instead of hiding the incident for three weeks.

Firing people based on a multiple-choice quiz is like firing the fire alarm for going off. You're optimizing for silence, not for safety.

## What actually measures your security posture

You can't check the human layer with a questionnaire, because an attacker doesn't send a questionnaire. They send a **situation**. So you have to test with one too, under the same conditions a real attack happens in: suddenly, under load, with time pressure and authority.

Here's what actually gives you signal:

- **Phishing simulations:** real ones, with a measurable result. The point isn't "does the person know about phishing," but how many clicked the link and, more importantly, how many didn't just not-click, but hit "report." The report rate is a far healthier metric than the click rate. And track it over quarters, not once.
- **Live social engineering:** calls from a "colleague" or "contractor" under a made-up pretext, attempts to extract access or data via the help desk. This is exactly how real companies get breached. Recall any major incident of the last few years where the entry point was a call to support, not some clever technical exploit.
- **Red team / purple team:** a full end-to-end imitation of an attacker, from initial foothold to the final objective. The red team (the attackers) shows how far an attack actually gets. Purple team is when attackers and defenders work together and tune detection on the spot.
- **Physical intrusion:** badges, meeting rooms, the classic "I forgot my badge, hold the door" (tailgating). The human perimeter doesn't end at email.
- **Tabletop exercises** for the people who handle an incident: the team sits around a table and plays through an attack scenario step by step ("3am, prod is encrypted, customers are panicking, a journalist is calling"), and each person says what they do. It tests not textbook knowledge, but the team's coordination and incident-response plan under pressure.

The difference is fundamental: a questionnaire asks **"what's correct?"** An attack tests **"what will you do?"** Security lives only in the second question.

### And what to do with the results

Once you've got real data, don't turn it back into a punishment tool, or people will start hiding their behavior again.

- Results go out **in aggregate and for learning**, not for public executions. Clicked? You get a short, to-the-point breakdown right then and there, not a reprimand.
- A team metric, not personal shame. The click rate drops and the report rate climbs quarter over quarter. That's your real progress.
- Reward the people who report. Someone who came forward and admitted their own mistake should get a "thank you," not a penalty. That's cheaper than any SOC.

## Bottom line

A multiple-choice quiz tests whether an employee can read answer options. That's it. If you want to assess real security, create a **situation**, not a questionnaire: phishing with a measurable result, social engineering, red/purple team.

And if your company still fires people who "fail" a security test, you're not improving security. You're training people to hand you pretty wrong data and to hide incidents. That only helps the attacker.

An honest "I'd probably have fallen for it" is worth more than a hundred perfectly guessed Cs. Protect the people who answer honestly. They're the ones who'll notice and report a real threat first, before it turns into an incident.
