# The First 30 Minutes

**A false claim about a Muslim community spreads in minutes. The correction usually arrives in hours. This is the gap where real harm happens — and where we built.**

> In July 2024, a false claim about an attacker's identity spread across UK social platforms within hours of a real tragedy. By the time it was corrected, the story had already hardened — and mosques and Muslim communities were attacked as a result. *(Source: ISD, "From rumours to riots," 2024)*

That single fact — **correction always arrives after the story has hardened** — is the entire premise of this project.

---

## Play it

Open `first-30-minutes-dashboard.html` in any browser. No install, no server, no account.

You are the volunteer Response Coordinator for a fictional town. A false claim just started spreading across five platforms. You have **30 minutes of action-time** before it settles — one way or another.

- 🐦 Watch the sidebar light up as the story reaches new platforms
- 📊 Every action costs real minutes — verifying is slower than reacting, and reacting badly can make things worse
- 🔥 Watch the reach meter. It doesn't wait for you.
- 📋 Walk away with an after-action report scored on the same four factors real incident postmortems use

---

## Why this exists

Most anti-hate hackathon projects build a **detector**. Ours is a **rehearsal**.

Detection tools answer "is this hateful?" — a question ChatGPT can already answer reasonably well. The much harder, much less-built question is: **when a false or coded claim starts moving, does the person responding actually know what to do in the first half hour — before it's too late to matter?**

That's not a classifier problem. It's a training problem. So we built a training tool.

## The four factors

Every decision in this simulation is scored against the same framework used to analyze real incidents where correction failed to keep pace with spread:

| Factor | What it means | What fails without it |
|---|---|---|
| **Speed** | Acting while the window is still open | Correction arrives after the story has hardened |
| **Context** | Verifying before you speak | A premature correction gets picked apart and spreads the claim further |
| **Handover** | Escalating with enough information to act on | The next person starts from zero, re-doing work already done |
| **Feedback** | Closing the loop with whoever raised the flag | People stop bothering to report anything at all |

There is no single "correct" playthrough. Verifying with a news contact is more reliable than reaching the original poster — and takes twice as long. Replying directly is fast — and feeds the post to more feeds regardless of what you say. Every choice is a real trade-off, not a trap with one right answer.

---

## What's actually happening under the hood

- A **fictional, invented incident** (Cedar Falls — no real event, person, or organization depicted)
- **Five parody platforms**, not real ones, each spreading at a different rate — mirroring how a claim moves from a fast public feed to algorithmic video to closed groups to private forwarding
- A **live reach meter** driven by real mechanics: organic spread compounds every minute you don't act, replying feeds the algorithm regardless of tone, and a correction posted without verification measurably backfires
- **No AI model** runs any of this — it's fully deterministic branching logic, which means nothing here can hallucinate, misrepresent a real event, or behave unpredictably in a live demo
- **Nothing is stored or transmitted.** Session best score lives in memory only and resets on reload.

## Built for, not despite, the rules

- No real hateful content anywhere — every post, comment, and username is synthetic, written for this scenario only
- No real event is depicted — Cedar Falls is fictional; the four-factor framework it's built on is drawn from published analysis of a real incident, cited above, not reenacted
- No personal data, no accounts, no tracking, no network calls

---

## Known limitations (stated plainly, not hidden)

- Only the **false-claim** scenario is fully built. A true-but-decontextualized version and a genuinely-unverifiable-in-the-moment version are designed but not implemented — see `/docs` for the full sketches. This matters: training only on false claims teaches "always deny fast," which is the wrong lesson for the many real cases that aren't clearly false.
- Scoring constants (time costs, spread multipliers, mistake penalties) are a first pass, tuned by hand-simulation, not real playtest data.
- This is a rehearsal tool, not a live monitoring system — it doesn't detect or respond to anything happening on real platforms.

## Roadmap

- Second and third scenario types (true/decontextualized, unverifiable)
- Multiplayer mode — one player manages the narrative, a second plays the response, same scoring
- A shared, growing library of scenarios usable by real community organizations for volunteer training

---

## Run it locally

```
git clone <this-repo>
cd <this-repo>
open first-30-minutes-dashboard.html   # or just double-click it
```

That's it. No dependencies, no build step.

---

*Built for the Harvest Anti-Muslim Hate Hackathon, hosted by the Global Network on Combatting Islamophobia (GNCI).*
