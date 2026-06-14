# COSS Contribution System — Build Momentum

Written 14.06.2026. 43 days left in the window — that's six weekly cycles,
plenty of room for the loop below to compound. The window is a forcing
function for shipping, not a countdown to a verdict.

You've already done the parts most people get stuck on. You picked a strategy
([context.md](../context.md)), cut the list from five to four after real
evidence came in (27.05 calls on Composio and Shannon), paid the onboarding
tax on Strix (sandbox model, type hints, LiteLLM mocking notes in
[Github_COSS/strix.md](../Github_COSS/strix.md)), and brought the mimicry
idea that most contributors never think of. The hard thinking is done. The
rest is showing up, shipping, and pouring fuel on whatever lights up.

The system has three jobs: (1) make starting trivial on a tired evening,
(2) make wins visible so the next evening starts easier, (3) keep your hours
flowing toward whatever is warming. The release valve in section 5 exists so
that effort spent on a cold target gets recycled into a hot one — not lost,
not a verdict on you.

---

## 1. Your portfolio — four shots, not one bet

Four parallel bets is the move. Picking one upfront is what made it feel like
a lottery; the portfolio turns it into a search where every week you learn
which target deserves more weight. The live set:

| Target  | Repo                  | Wedge (per 17.05)               | Why it's on the list |
|---------|-----------------------|---------------------------------|----------------------|
| Strix   | usestrix/strix        | CI/CD + issue-tracker plumbing for the scanner | Warmest — your setup notes already exist |
| OpenWork | different-ai/openwork | Slack/Jira/Linear integration edges | Big wedge, integration-heavy by design |
| Hive    | aden-hive/hive        | Observability/logging connectors | Big wedge, enterprise pain point |
| Shannon | KeygraphHQ/shannon    | API schema / cloud-auth ingestion | One-week look-see to confirm or flip the 27.05 read |

Opening hour split for weeks 1–2: **Strix 35 / OpenWork 30 / Hive 25 /
Shannon 10**. Strix is largest because friction is lowest — you already know
how to run it, so the cost of any given evening is the smallest there.
Shannon gets the smallest slot precisely so one calm week of data settles
the closed-shop question instead of leaving it as a low-grade nag.

The portfolio's real superpower: when one target is slow to reply, you don't
sit refreshing GitHub. You open the next folder in
[Github_COSS](../Github_COSS/) and keep moving. Forward motion across four
repos beats stuck deliberation on one.

---

## 2. The weekly loop — Sunday decides, weeknights ship

The point of the loop is to make weeknight-you stupid. Weeknight-you is
tired and will quit if asked to decide anything. Sunday-you, with coffee,
makes every decision in advance so weeknight-you just opens what's been
queued and ships.

**Sunday (45–60 min — the only thinking session).** Open this file and the
log. Five things, in order, none need to be perfect: (1) write down what
shipped this week (PRs opened, merged, comments answered) — this is the
momentum check and it'll surprise you how much it adds up; (2) score the
five signals in section 4 — flag any target that's heating up so you can
pour fuel on it; (3) for each target, queue **one leverage candidate** and
**two petty fallbacks** so weeknight-you always has three things to open
without thinking; (4) write the week's bet in one line — "if I ship X on
Y, signal Z should move"; (5) adjust the hour split based on what's
warming.

**Weeknight evenings (aim 60–90 min, floor 25 min).** No deciding. Open the
issue Sunday queued. Ship. On a tired night, 25 minutes of: pull latest,
re-read thread, leave one substantive comment — that's a real win. Your
handle just landed in a maintainer's notification feed, which is the whole
game in week one. Most contributors quit on tired nights; you don't have
to be heroic, just present.

**Saturday (15 min — pure logging).** PRs opened, merged, maintainer
replies and turnaround, anything surprising. No interpretation —
Sunday-you handles that.

Output of the loop: consistency. The Brian Douglas hire pattern in
[dailyPathA.md](../dailyPathA.md) — "junior dev grinds PRs for 30 days,
core dev DMs them" — is about visible consistency, not heroic single PRs.
The loop produces exactly that signal.

---

## 3. Petty + leverage — both ship, in that order

Your worry about "only fixing petty issues" is half right, but the fix
isn't to stop petty PRs. Petty PRs are how you buy attention cheaply in
week one. They get merged fast, your name lands in commit history,
maintainers learn your handle, and you're inside the file the leverage PR
will touch. They're the warm-up, not the goal.

Target mix per target per week: **one leverage PR + however many petty PRs
naturally fall out** of being in the codebase. Don't force the ratio.

A **petty** issue: mechanical fix the maintainer could do in 10 minutes if
they cared. Broken link, dep bump, README typo, missing CONTRIBUTING
section, a flaky test. Ship freely, no second-guessing.

A **leverage** issue meets three tests: (a) the maintainer would have
hated doing it themselves — usually a third-party integration, auth edge
case, or a connector to something they don't run; (b) a real user is
asking for it in issues or Discord, so the merge benefits a customer;
(c) the fix needs judgement (API surface, naming, failure mode), not
just typing. Strix's sandbox boundary notes in
[Github_COSS/strix.md](../Github_COSS/strix.md) are an example of context
you need *before* leverage work is possible — that prep counts as
progress.

When you sit down tired and unsure which issue is "real contribution,"
remember: shipping anything beats shipping nothing. Petty PR shipped
tonight > leverage PR you'll start "tomorrow."

---

## 4. The five signals — what to look for, and celebrate

These are the things that mean it's working. Score each target on Sunday
as warming / flat / cooling vs last week. Direction matters more than
absolute level — cold-going-warm is a stronger bet than warm-but-flat.
When any of these moves the right way, the response is the same: pour
more hours into that target this week.

**(1) PR turnaround.** Time from your PR open to the first substantive
maintainer comment. Watch it drop over weeks. Same-day responses mean
you're on the radar — celebrate, double down.

**(2) Comment register shift.** Maintainer comments move from "thanks,
please rebase" to "what do you think about X?" This is the single
strongest leading indicator of conversion. It means they're starting to
use your judgement, not just your labour. When this fires, you've
arrived — that target gets the lion's share next week.

**(3) Cross-issue tagging.** They @-mention you on issues you didn't
open, asking if you've seen it or want it. Rare and significant. One of
these = double down.

**(4) Channel graduation.** Invited from public Discord to a
contributors-only channel, or a maintainer DMs you unprompted. Closest
public proxy to "they're considering you." Treat as green light.

**(5) Wedge issue density.** Count open issues matching your wedge
(column 3, section 1). Growing = the angle is getting more valuable on
its own. Shrinking to near-zero = pivot the wedge within the target,
not necessarily the target itself.

"Is X PRs/week enough?" dissolves into these. PR count is the input.
Signals 1–4 are the output, and they're what get you hired. Three PRs
that move signal 2 > ten PRs that don't.

---

## 5. Release valve — redirecting hours toward what's working

Not about cutting losses. About not leaving hours stranded on a cold
target when another one is warming. Pre-committed now, on a calm Sunday,
so future-tired-you doesn't have to negotiate with themselves at 11pm.

**Double down** (absorb hours from a quieter target) the moment **any**
of signals (2), (3), or (4) fires on another target. Don't wait for
confirmation — these are rare enough that one is enough. This is the
move that turns the system from "trying things" into "compounding on a
winner."

**Redirect** a quieter target's hours (cut to 5h/week, hold the slot
open) when, after two full weeks: PR turnaround on a merged PR is still
48h+, **and** no comments have crossed into the consultative register
(signal 2), **and** an open PR has sat 10+ days while maintainers were
visibly active elsewhere in the repo. All three together — not any one
alone — is the threshold. Those hours go straight to whichever target is
warmest.

**Pause** a target entirely only when maintainers visibly enter crisis
mode and lock down community contribution (Composio's May breach in
[dailyPathA.md](../dailyPathA.md) is the template). Recognise within a
week, recycle the hours.

By Sunday **17.07.2026** (10 days before window close), check whether
signals (3) or (4) have fired anywhere. **If yes** — full throttle on
that target for the final stretch, that's where the conversion comes
from. **If no** — the loop has given you something most devs trying
this path never get: a clear read on which COSS targets actually
engage outside contributors. Use the last 10 days to convert merged PRs
into LinkedIn/resume artefacts and apply to remote YC roles in
[SloppyJobsOrganize.md](../SloppyJobsOrganize.md) with real public
proof of work — a much stronger application than 43 days ago. Either
branch is a real result. Neither is a wasted window.

---

## 6. The mimicry protocol — your highest-leverage move

This is the idea you brought today and it's the strongest single move in
the system. Most contributors write PRs in their own voice and hope
maintainers like it. You're going to write in the maintainers' register,
so your PRs read like they came from inside the team.

This is **fun work, not draining work** — closer to detective reading
than to grinding. It's the thing to do on an evening when you have a
little energy and want to feel like you're making real progress without
the cognitive load of writing code.

Per target, on the first Sunday you touch it (or tonight on Strix while
the idea is hot):

Find the top 3 contributors by recent commit count in each cloned repo
under [Github_COSS](../Github_COSS/): `git shortlog -sne --since="12
months ago" | head -10`. Cross-reference with whoever's actively
reviewing PRs on GitHub right now (often a smaller, more relevant set).
Two to four humans — that's your audience.

For each, pull their voice: `git log --author="<name>" --since="6 months
ago" --pretty=format:"%h %s%n%b%n---" | head -400`, plus skim their
last ~20 merged PRs on GitHub. Extract four things into a small note
per contributor (e.g.
`Github_COSS/strix/_contributor_notes.md`): PR title style (length,
prefix, tense), PR body structure (problem/approach/test, freeform, or
none), what they flag in review (types, tests, naming, perf — pick one
and you see their priority), and how they handle disagreement
(terse/explanatory/Socratic).

Then write your PRs in their shape. Not parody — match the form, keep
your substance. Good shape gets your PR read faster, which moves signal
1 and primes signal 2. This is the only piece that compounds across all
four targets simultaneously, because you're learning what "well-written"
looks like in the funded-COSS subculture as a whole.

Bonus: doing the mimicry pass also surfaces the next leverage issue for
free, because issues matching the top contributor's priorities jump out
as you read.

**Tonight, if any energy is left: do the Strix mimicry pass.** 30
minutes, interesting work, and you'll walk into the first Sunday already
armed.

---

## 7. What you have going for you

Re-read on tired days when the doubt comes back:

- **UTC+7 timezone arbitrage** ([context.md](../context.md)) — you can
  be the person who replied while the US team slept. This is a
  structural advantage funded US-based contributors don't have.
- **Infinite AI usage** (your 06.06 note) — the friction of reading
  unfamiliar codebases is the lowest it's ever been for any contributor
  in any window in history. Use it.
- **Four cloned repos, written context per target, a working Strix
  setup** — you're not at zero, you're at week three of prep work most
  people skip.
- **A system** — weeknight-you doesn't have to be smart, just present.
  The thinking is already done by Sunday-you.

---

## 8. First week, concrete

So Sunday **15.06.2026** isn't a blank page:

- **Tonight (14.06):** if any energy — run the mimicry pass on Strix
  (~30 min). Save into `Github_COSS/strix/_contributor_notes.md`. If no
  energy — close the laptop, you've already done the strategy work for
  today.
- **Sun 15.06:** first Sunday session. Queue three issues per target
  (1 leverage + 2 petty). Write the first week's bet line.
- **Mon–Fri:** ship from the queue. 25-min floor, 60–90 aim.
- **Sat 20.06:** 15 min logging.
- **Sun 21.06:** first real review session. Score signals. Adjust
  weights. Decide on Shannon based on its one week of data. The system
  itself is also on probation here — if a piece creates more friction
  than it removes, trim it. Trim, don't abandon. Showing up is the
  whole game.
