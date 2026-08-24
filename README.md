# Chronically Online — Incident Response Trainer

> **A lie is already 5 platforms deep.**
> **You just found out.**
> **The clock does not care if you're ready.**

Somebody screenshots it. Somebody forwards it. Somebody's group chat already has it.

You have **30 minutes.** No pause button. No do-overs mid-run. Every second you spend thinking is a second the story spreads *without you.*

You are the **Response Coordinator.** Not a bystander. Not a mod. The person who's supposed to know what happens next - and right now, you're the only one in the room.

**Go.**

---

## ⚠️ Read this before you play

This is a training simulation about **anti-Muslim hate and misinformation**, how a false claim spreads, and what it takes to slow it down.

The incident (**Cedar Falls**) is **100% fictional.** Every post, username, comment, and platform is synthetic for this scenario. No real people, real victims, real attackers, or real organizations are depicted.

This is not a game about hate speech for shock value. It's a rehearsal for the moment your instincts have to be faster than your fear. Play it seriously; that's the point.

---

## 🕵️ The case

At **T+0:00**, a claim drops on **Chirp** (the origin platform): mosque members allegedly attacked town hall attendees who opposed a mosque expansion. It's already got a video attached. It's already got comments. It's already got momentum.

You don't know yet if it's true.

**Neither does anyone else**, and that's exactly the problem. While you're reading this sentence, the claim is moving to the next platform. It doesn't wait for you to catch up.

Two meters run against each other:

| Meter | What it tracks |
|---|---|
| 🔥 **Harmful Reach** | How far the false claim and the backlash it drags with it has spread |
| 🧭 **Awareness** | How far *accurate* information has actually reached people |

**First one to 100% wins the run.** Get Awareness there first → contained. Let Harmful Reach win → not contained.

There is no pause. The clock ticks in real time, and it never waits for you to feel ready.

---

## 🎮 Play it - no install, no excuses
Open `first-30-minutes-dashboard.html` in any browser. That's the whole setup. No server, no account, no dependencies, nothing to configure.

---

## 🧩 Your moves, and why none of them are free

Every action costs real time off the clock. Most of them can only be used **once per run**. Wait/Monitor is the only repeatable one. Burn an action in the wrong moment and it's gone for the rest of the case.

| Action | Time cost | The catch |
|---|---|---|
| 🔎 **Verify with original poster** | 45s | Fast, but they're anonymous. Might go quiet. Might make it worse. |
| 📰 **Contact local news desk** | 90s | Slow, but a confirmed source hits different. Might come back empty. |
| 🧠 **Do your own research online** | 60s | A coin flip unless the news desk already left you a lead. |
| 📢 **Post public correction** | 60s | Verified facts land hard. Post it *unverified* and it reads as a bare denial and draws backlash accusing you of protecting your own. |
| 💬 **Reply directly to the post** | 30s | Only works on the platform hosting the original post. Might cool the thread. Might get quote-shared straight into a bigger audience. |
| 📣 **Post independent awareness message** | 60s | Same rule as public correction, your credibility decides whether it helps or backfires. |
| 🤝 **Escalate to trust & safety** | 75s | Too early and they won't even open a case. Wait too long and the report barely slows anything down. |
| ⏳ **Wait / monitor** | 60s | The only move you can repeat. Sometimes the smartest play, if your last verified post is still landing. Sometimes it's just handing the clock to the other side. |

**There's no "correct answer" button.** Verifying costs you time you don't have. Acting fast without facts can backfire on the community you're trying to protect. Every choice is a trade, and you don't see the trade-off until after you've made it.

---

## 🌊 It doesn't wait for you

New posts appear on their own, roughly every **20 seconds**, whether or not you've acted. Bigger accounts do outsized damage: a post from someone with 50K+ followers hits about **3x harder** than the same post from a nobody. Watch who's sharing what, not just what's being said.

Replying to a post doesn't make it disappear. Sometimes it cools the thread down. Sometimes it gets quote-shared straight into a much bigger audience. You don't get to pick which, you just decide if the risk is worth it.

The claim spreads across **six fictional platforms** — Chirp, Reelz, Facewall, GossipHole, WhisperLine, and Wireline — none of them real. New icons light up in the sidebar as the story reaches new places, with unread flags so you know exactly what you're behind on.

---

## 🏁 What "winning" actually looks like

When a meter hits 100%, the run ends and you get the full breakdown: time elapsed, final Harmful Reach %, final Awareness %, and if you win, your best time gets saved locally so you can try to beat it next run.

- **Contained** : Verified information outran the claim before real damage spread, including the hateful pile-on a careless correction can trigger.
- **Not contained** : The false claim won the race. By the time anything corrective broke through, the harmful narrative and everything it dragged out along the way had already reached everyone it was going to reach.

Neither outcome is scripted. It's entirely down to what you did with your 30 minutes.

---

## 🧩 The loop, broken down

Every strong response in this simulation or a real one comes down to four questions. Here's how this build answers them.

**Input: What does the user bring?**
Nothing but themselves and their doomscrolling skills. They open the file already knowing a false claim is spreading, the seed post is waiting on Chirp the moment they hit "Start the clock." No outside tools, no account, no prior context. The only thing they supply is the decision-making itself.

**Decision: What information shapes the decision?**
Two live meters (Harmful Reach vs. Awareness), a platform sidebar with unread flags showing where the story has spread, follower counts on who's posting what, and critically whether they've verified anything yet. That last one is the hinge: every action's outcome branches on whether the player is verified, so "do I have confirmed facts or not" is the single piece of information that determines whether posting helps or backfires.

**Action: What happens next?**
They pick from eight one-time-use moves (verify with poster, contact news desk, do their own research, post a correction, reply directly, post independent awareness, escalate to trust & safety) or the repeatable Wait/Monitor. Each action burns real seconds off the clock and immediately triggers a scripted outcome, a coin-flip verification result, a backlash reply, a cooled thread, a trust & safety response, logged live in the Incident Log sidebar.

**Result: What changes, and how do you show it?**
The two meters move. Harmful Reach and Awareness shift in response to that single action, the run either continues or ends the moment one hits 100%, and the end screen shows the receipt: elapsed time, final percentages on both meters, a plain-language outcome ("Contained" or "Not contained"), and if they won, a saved best time to beat next run. Nothing is hidden after the fact; the score bars and the log are the proof of what that specific decision cost or earned.

---

## 🧪 What's actually running this

No AI making decisions. No live data. No network calls, ever.

The whole thing is **one self-contained HTML file** - HTML, CSS, and vanilla JavaScript, zero frameworks, zero build step, zero external libraries or CDN calls. Every spread mechanic, meter shift, and branching outcome is deterministic logic written directly into the code - nothing is generated live, nothing is pulled from the internet, nothing you do is stored or transmitted anywhere except your own device (used only to save your best clear time).

Reload the page and the run resets. What you see is exactly what the code says will happen.

---

## 🛡️ Why it's built this way

Because the subject is real communities and real harm, we drew hard lines:

- 🚫 **No real hateful content**: every post, comment, and username is synthetic, written for this training scenario only.
- 🚫 **No real incident**: Cedar Falls never happened. It's a composite built to teach a pattern, not report an event.
- 🚫 **No real people**: no victims, attackers, organizations, or community members are depicted, ever.
- 🚫 **No personal data**: no accounts, no profiles, no trackers, no data collection.
- 🚫 **No live monitoring**: this does not watch real Muslim communities or real platforms. It never will.
- ✅ **Real research, fictional execution**: the mechanics are informed by documented analysis of real incidents, without recreating any of them.

---

## 🎯 Our why: Southport, 2024

This isn't a hypothetical. In 2024, a false claim about the identity of an attacker in Southport, UK, appeared within hours of a real tragedy. It spread through recommenders and forwards across multiple platforms. It reached real-world disorder, attacks on Muslim communities and mosques. And the correction, when it came, arrived after the story had already hardened.

Researchers who studied it (ISD, *From Rumours to Riots*, 2024) came away with four things builders can improve: **speed**: the right update has to land while choices are still open; **context**: source, uncertainty, and the full conversation need to travel together, not get stripped at each handoff; **handover**: evidence has to become a short, safe escalation to someone who can actually act; and **feedback**: the people who raised the alarm need to see what happened next.

Those four things are not abstractions to us. **They are the exact four dimensions this simulation scores**- Speed, Context, Handover, Feedback. Southport is why those four exist as meters instead of just being "act fast and be right." A volunteer who's fast but has no context can make it worse. One with context but no handover collapses the moment they step away. One who does everything right but never closes the loop teaches people to stop reporting. Southport (and several other such tragedies) is the proof that all four have to hold at once, in real time, or the correction arrives too late to matter.

That's the why. Everything else in this repo is the how.

---

## ❤️ Why the first 30 minutes matter

Misinformation doesn't stay information for long. It becomes:

**fear → suspicion → blame → harassment → violence.**

And when the target is a community that's already vulnerable, the damage doesn't stop when the original post gets deleted.

One volunteer can't fix online hate. That's not the claim here. But the person who shows up in the first 30 minutes, the one who verifies before they post, who hands off context instead of hoarding it, who closes the loop with whoever raised the alarm, that person changes what the next hour looks like.

This is a rehearsal for being that person.

---

## ⚠️ What this doesn't solve - yet

This build simulates exactly one kind of claim: **false.** That's a real limitation, and we're not going to pretend otherwise.

Real claims are messier. Sometimes they're:

- True, but missing context
- Partially true
- Impossible to verify in the moment
- Still developing
- Built on incomplete information

Training people to reflexively yell "FALSE!" at everything would be its own kind of harm. The harder scenarios are next. 

---

## 🗺️ Roadmap

**01 - More scenarios**
- [ ] False claim *(current)*
- [ ] True but decontextualized claim
- [ ] Unverifiable-in-the-moment claim

**02 - Multiplayer**
- [ ] One person manages the narrative
- [ ] One person manages the response
- [ ] Shared incident timeline
- [ ] Team-based scoring

**03 - Scenario library**
- [ ] Reusable training scenarios
- [ ] Community-organization workflows
- [ ] Configurable incident parameters
- [ ] After-action review library

---

## 🔬 Limitations & methodology

This is a first-pass model. Time costs, spread multipliers, and backlash mechanics were hand-tuned through manual simulation, not empirical playtesting on real platform data. The numbers aren't predictions of how real social platforms behave, they're built to create a consistent environment for practicing the underlying decision problem. Parameters will get refined as we playtest.

---

## 📚 Research

The framework draws on published analysis of real-world misinformation and anti-Muslim violence, including:

- Institute for Strategic Dialogue (ISD) - *From Rumours to Riots* (2024)

The research is why this exists. The simulation itself is fiction, start to finish.

---

## 🛠️ Built with

- **HTML, CSS, and vanilla JavaScript** - a single self-contained file, no frameworks, no build tools, no external dependencies.
- **Claude AI** - used for idea generation, narrative and UX framing, and coding assistance throughout development.

---

## 👩‍💻 Built by

Oyonti Nasir, Proshun Doza, Subaita Mamun

Built for the **Harvest Anti-Muslim Hate Hackathon**, hosted by the **Global Network on Combatting Islamophobia (GNCI)**.

<div align="center">

**The claim already has a head start.**
**You have 30 minutes to close the gap.**

⏱️ The clock starts the second you open the file.

</div>
