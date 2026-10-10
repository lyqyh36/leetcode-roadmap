# leetcode roadmap: a week-by-week plan that takes you from arrays to DP without grinding 3,000 problems

You open the problem list, see 3,000+ questions, sort by acceptance rate, and solve three Easy problems that teach you nothing. Two weeks later you're back where you started, except now you own a notebook with seven half-finished attempts in it.

That's not a discipline problem. It's a sequencing problem. The search "leetcode roadmap" is really four questions bundled together: what order do I study things in, how many problems is enough, when do I move on from a topic, and how do I know I'm actually ready for a 45-minute interview. Everything below is an attempt to answer those four plainly, with a concrete schedule you can put on a calendar.

## What a leetcode roadmap has to cover (there are four layers, not one)

Most roadmaps online are just a list of topics in a vaguely sensible order. That's the easy part. The hard part is that interview performance sits on four separate skills, and each one needs a different kind of work:

1. **Data structure fluency.** You can write a hash map traversal, a linked list reverse, a BFS without looking anything up. If you're reaching for documentation mid-problem, you're not learning patterns yet, you're learning syntax slowly.
2. **Pattern recognition.** Given a problem you've never seen, you can tell in the first two minutes whether this is sliding window, binary search on the answer, or a graph traversal. This is the layer that decides interviews.
3. **Volume practice.** Speed and comfort come from reps. Not 3,000 reps, but more than the 40 you'll do while learning the patterns.
4. **Interview simulation.** Talking through your reasoning while your hands are typing, with a clock running and someone asking "what's the complexity if we stream the input instead?"

A lot of people spend three months on layer 3 and never touch layer 2. That's why they can solve the problem they practiced and freeze on the near-identical one they didn't.

## A 12-week leetcode roadmap

Twelve weeks assumes roughly 1–2 hours a day, six days a week. If your interview is six weeks out, take the same list and cut the DP block down to the two most common families, and start the company-specific work in week 3 instead of week 11.

| Weeks | Focus | What "done" looks like |
| --- | --- | --- |
| 1–2 | Arrays, strings, hash maps, two pointers, sliding window | You solve mediums in these families in 25 minutes without editorial help |
| 3–4 | Binary search (including search-on-answer), stacks, queues, linked lists, prefix sums | You write binary search without an off-by-one bug and can say which half you discard and why |
| 5–6 | Trees: DFS, BFS, recursion, then backtracking on small inputs | Recursion stopped feeling like magic; you can draw the call tree |
| 7–8 | Graphs: DFS/BFS on grids, topological sort, heaps for top-K and k-way merge | You can convert a word problem into a graph without hints |
| 9–10 | Dynamic programming: 1D, 2D, knapsack variants, LIS | You can state the recurrence out loud before writing code |
| 11–12 | Company-specific sets, timed mocks, revisiting your own old mistakes | Two full mock interviews per week, out loud, on a timer |

Two notes on this schedule. First, the order matters more than the topic list — recursion appears in week 5 because DP in week 9 is nearly impossible without it, and this is the same reasoning AlgoMonster's own roadmap page gives for finishing its sections in sequence rather than cherry-picking. Second, DP is the standard cut line when time is short. AlgoMonster's roadmap page says it outright: if you're not targeting the most selective companies, you can skip DP initially and focus on the more frequently tested patterns. That's a useful permission slip, because DP is where a lot of people lose two weeks and their confidence.

## How many problems is actually enough

The honest answer is that the number matters less than the ratio of patterns to problems. A rough benchmark that has held up for years: Yangshun Tay's Blind 75, a set of 75 problems grouped by pattern rather than by difficulty. The point of the list was never the number 75 — it was that each problem represents a technique you can reuse, so mastering the list means mastering the techniques rather than memorizing 75 answers. Tay later shipped Grind 75, an adjustable version of the same idea where you set your available hours and it reorders the list for you.

In practice, 150–250 well-chosen problems with a revisit schedule beats 800 random ones. If you've solved 200 problems and still can't classify a new problem type in two minutes, you don't have a volume problem.

## The practice loop that makes problems stick

The loop matters more than the list. A version that works:

1. **Attempt with a timer.** 25 minutes for a medium, 15 for an easy. No editorial, no autocomplete suggestions.
2. **Escalate hints in stages.** Stuck? Get a nudge about the technique, not the code. Still stuck after another 10 minutes? Read the approach, close the tab, and re-implement from an empty file.
3. **Do one variation immediately.** Same pattern, different surface. If you learned sliding window on "longest substring without repeating characters," solve a fixed-window problem next. This is the step almost everyone skips, and it's the one that builds recognition.
4. **Revisit on a schedule.** Roughly 1 day, 1 week, 1 month later. If you can't solve it cold, reset the clock. A problem you solved once is a problem you'll forget in four days.
5. **Write down the invariant, not the code.** For binary search: "I'm searching in [L, R]; if mid < target, everything left of mid is dead." That sentence transfers to the next problem. The code doesn't.

If your study log only records "solved / didn't solve," you're throwing away the most useful data, which is the reason you got stuck.

## Where a structured course fits into the plan

The weak point of self-directed roadmaps is layer 2 — pattern recognition. You can only recognize patterns you already have names for, and most people's names for them are vague ("it looked like a two-pointer thing"). A course that ships an explicit, ordered pattern list removes a lot of that guesswork.

AlgoMonster is built around that idea. It's a paid prep platform whose own learning path lives at its roadmap page, and it's structured as a sequence rather than a problem bank. A few things about it are worth knowing before you spend anything:

- **It has a real order, and it says so.** Start with the Foundation Course if you can't yet solve easies comfortably; go straight to Core Patterns if you can. Then finish sections in sequence, because later sections assume earlier templates.
- **The learning loop is concept → quiz → practice → Speedrun.** Speedrun is the interesting part: instead of writing code, you answer multiple-choice questions about *which technique and template the problem needs*. That directly trains the recognition skill, and AlgoMonster's reasoning is that half of a real interview is spent identifying the algorithm and explaining it anyway.
- **Decision flowcharts.** For "I have no idea what this problem is," the platform walks you through questions like *is the input sorted?*, *is the subarray contiguous?*, *is it a graph?*
- **Company-specific sets and a 50-problem list** for the final sprint, plus short 3-minute breakdown videos on their YouTube channel if you want something to watch on a commute.
- **The short-on-time path is documented:** learn each pattern's core technique, then jump to company-specific questions. Their own framing is that a text-and-diagram curriculum is meant to be something a textbook-averse candidate can finish in weeks rather than months.

What it isn't: a 3,000-problem bank. Third-party reviews put it around 48 patterns and roughly 230 lessons and problems, against LeetCode's thousands. The core lessons are text and interactive diagrams rather than video walkthroughs. System design coverage is introductory, and there are no live mock interviews with real engineers. If your gap is volume or senior-level system design, this is a supplement, not the whole answer.

If the sequencing problem is the one that's actually blocking you, 👉 [there's a free tier you can poke at before paying anything](https://algo.monster?fpr=li69).

## AlgoMonster plans and pricing

Here's what the subscribe page shows. There's no monthly option — you're choosing between a year and forever.

| Plan | Price | Billing | What you get | Buy |
| --- | --- | --- | --- | --- |
| Free | $0 | — | Limited access to a subset of patterns and problems | [Start on the free tier](https://algo.monster?fpr=li69) |
| Pro — Yearly | $99/year ($8.25/mo), list price $198 | Billed annually, cancel or upgrade anytime | Everything below, 12 months of access | [Get Pro Yearly](https://algo.monster?fpr=li69) |
| Pro — Lifetime | $189 one-time, list price $378 | Billed once | All Pro content, lifetime updates, everything in the annual plan | [Get Pro Lifetime](https://algo.monster?fpr=li69) |

What Pro unlocks, per the official page: all patterns, lessons and problems; unlimited AI assistant usage; unlimited Speedrun; real questions from top tech companies updated monthly; 500+ lessons across 6 courses; 1,000+ illustrations; 3,000+ editorials; and a member discount on their live bootcamps. Two bonus courses come with the subscription — a Foundation Course covering data structures from scratch, and a Build an LLM course that goes past API usage into tokenization, attention, and training. Content the site says is crafted by Google engineers and competitive programmers. Quant Interview Prep, developed with an external partner, is sold separately.

One thing to keep in mind while researching: a few review sites list very different numbers — $119 to $299 a year, or a $459 lifetime price with a $918 list price. Those figures don't match what the official subscribe page currently shows, and they also contradict each other. The subscribe page is the only number that matters, and since the $99/$189 pricing is itself a sale against a $198/$378 list, it can move. Discount codes from partner blogs circulate on top of it; they rotate and some stop working without warning, so the checkout page is the only place you can confirm one.

## Which plan makes sense

If you're interviewing in the next three months, the annual plan is the obvious pick — it costs less than a month of most bootcamps and less than LeetCode Premium's $159/year, and the content doesn't change meaningfully within a year. The lifetime plan is worth it if you expect to change jobs more than once. At a $90/year gap between the two, you're effectively betting you'll still want the material in two years, which is a reasonable bet for anyone who plans to interview again for a promotion or a better offer.

The free tier is the actual try-before-you-buy mechanism. There's no formal free trial, so use it for a few days to test whether you can learn from text and diagrams. If you need a person on video walking you through every solution, this format will frustrate you no matter how good the roadmap is.

## Mistakes that derail most leetcode roadmaps

- **Grinding by acceptance rate.** Sorting the problem list by "% accepted" gives you a random tour of topics, which is the opposite of a roadmap.
- **Learning a topic from a single problem.** One problem per pattern means you'll recognize nothing the following week.
- **Never simulating pressure.** Solving untimed problems at home is not the same skill as explaining your approach at minute 30 of a 45-minute round. Two timed mocks a week in the last month is the minimum.
- **Collecting resources instead of finishing one.** A course, two playlists, a Reddit list, and a spreadsheet of "to do" problems is not a plan. Pick one spine, use the others as references.
- **Treating system design and behavioral rounds as free.** They aren't. If you're targeting L5 or above, plan 20–40 hours of dedicated system design work, because a DSA curriculum won't cover it at the depth that round requires.

## FAQ

**How long does a leetcode roadmap take?** For most people with working coding fluency, 8–12 weeks at 1–2 hours a day gets them to the point where mediums are solvable and explainable under time. A 4–8 week sprint is realistic if you already know the basics and have an interview booked.

**Do I need LeetCode Premium?** It buys you company-tagged frequency data and the full bank. It's useful in the final two weeks for targeting a specific company. It's not a curriculum, and it doesn't teach you the patterns — that's the gap the roadmap above is trying to fill.

**Blind 75 or NeetCode 150 or a structured course?** Blind 75 for benchmarking where you stand, Grind 75 for a list that adapts to your available hours, a pattern-based course for the recognition layer underneath both. They're not competing ideas; they're different layers.

**Is using an AI assistant on problems cheating?** Not if you use it the way you'd use an interviewer's hint — ask for the technique, not the solution. Copying a solution and moving on is the failure mode, whether it comes from an AI or an editorial.

**Can I do this entirely for free?** Yes. NeetCode's videos, the LeetCode discussion section, and free pattern lists cover most of it. What free resources don't give you is a fixed order and an endpoint, which is exactly the thing people pay to stop having to decide.

The short version: pick an order, name your patterns, cap your volume, and rehearse out loud. If the "what do I study next" question is what's been stopping you, 👉 [AlgoMonster's roadmap-based curriculum](https://algo.monster?fpr=li69) is one way to outsource that decision and get on with the actual practice.
