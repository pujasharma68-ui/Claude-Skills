**LinkedIn Algorithm Score**

A senior-growth-strategist scoring pass on a single LinkedIn post: how well it's likely to be read, ranked, and distributed under LinkedIn's current feed algorithm - not just whether it "sounds good."

**How to run this**

1. **Get the draft.** If the full post text isn't already in the conversation, ask for it (copy, plus any image/carousel text, plus any link that would be attached).
2. **Refresh on the algorithm before scoring.** Run 2-4 web searches for the latest LinkedIn algorithm / ranking behavior (e.g. "LinkedIn algorithm ranking signals \[current month year\]", "LinkedIn dwell time depth score", "LinkedIn engagement bait downranking", "LinkedIn 360Brew \[current month year\]"). Explicitly include 360Brew - LinkedIn's foundation-model ranking system - in this refresh, since it's the current core of how distribution decisions get made; don't score without checking for any recent update to how it behaves. Prioritize sources from the last 1-3 months over older ones - this platform moves fast and the person is explicitly asking you not to score from stale knowledge. If web access isn't available for some reason, say so plainly, and score against the baseline model in reference/algorithm-baseline.md instead - don't quietly fall back without flagging it.
3. **Score every category** in the table below (see reference/scoring-rubric.md for the full definition of what "good" looks like in each row, with current-algorithm reasoning).
4. **Apply the compliance gate** - see step 5 below - as a deduction, not a category.
5. **Deliver the full output** in the format specified at the end of this file.

Don't skip categories because a post is short or simple - score all 22 and note "N/A, minimal impact" only where a category genuinely doesn't apply (e.g. no hashtags used at all → still score hashtag strategy as low/missed opportunity, don't skip it).

**The 22 scoring categories and their weights**

Weights reflect what actually moves distribution under the current algorithm (comment depth and dwell time carry more weight than hashtags or emoji-hook tricks; see reference/algorithm-baseline.md for why each weight is set where it is). They sum to 100.

| **#** | **Category**                                                                      | **Weight** |
| ----- | --------------------------------------------------------------------------------- | ---------- |
| 1     | Hook strength (opening line / scroll-stop)                                        | 6          |
| 2     | First 2-3 lines effectiveness (pre-"…see more" performance)                       | 5          |
| 3     | Readability                                                                       | 4          |
| 4     | Storytelling quality                                                              | 5          |
| 5     | Value delivered                                                                   | 8          |
| 6     | Originality                                                                       | 4          |
| 7     | Engagement potential                                                              | 6          |
| 8     | Comment generation potential                                                      | 6          |
| 9     | Shareability                                                                      | 4          |
| 10    | Save potential                                                                    | 4          |
| 11    | Credibility and authority                                                         | 6          |
| 12    | Emotional impact                                                                  | 4          |
| 13    | Audience relevance                                                                | 6          |
| 14    | Formatting and whitespace                                                         | 4          |
| 15    | Sentence length variation                                                         | 3          |
| 16    | CTA effectiveness                                                                 | 4          |
| 17    | Keyword optimization                                                              | 3          |
| 18    | Hashtag strategy                                                                  | 2          |
| 19    | Personal branding consistency                                                     | 4          |
| 20    | LinkedIn SEO optimization                                                         | 3          |
| 21    | LinkedIn algorithm friendliness (native format, link handling, dwell-time design) | 6          |
| 22    | Virality potential                                                                | 3          |
|       | **Subtotal**                                                                      | **100**    |

**Compliance gate (deduction, not a weighted category)**

After scoring the 100 points above, check for current-best-practice violations and subtract from the subtotal:

- Engagement bait ("comment YES if...", "tag someone who...", vote-bait) → **−10**
- Banned/red-flag phrasing for this account: "delve," "in today's fast-paced world," "game-changer," "unlock," or other generic filler → **−3 per instance**
- AI-sounding, templated phrasing patterns (LinkedIn's ranking has gotten better at flagging these) → **−5**
- Misleading hook (opening promises something the post doesn't deliver) → **−5**
- Naked external link with no framing/context before it → **−3**

State each deduction explicitly with the line that triggered it. Final score = subtotal − deductions, floored at 0.

**Output format (always use this structure)**

**1\. Overall LinkedIn Algorithm Score: NN/100** One line verdict (e.g. "Strong - minor tightening before posting" / "Needs a rewrite of the hook and CTA before this earns real reach").

**2\. Category-wise scoring table** Table with columns: Category | Score (as fraction of weight, e.g. 5/6) | Why. Keep the "Why" column to one sharp sentence grounded in current algorithm behavior, not generic advice.

**3\. Strengths** 3-5 bullets, each naming the exact line/element that works and why it helps distribution.

**4\. Weaknesses** 3-5 bullets, each naming the exact line/element that's holding it back.

**5\. Factors reducing reach** Call out specifically anything from the compliance gate, plus any structural issue (post too long before the fold, no native format, external link with no context, weak first-2-lines, generic hook) with the deduction/impact stated.

**6\. Actionable improvements** Concrete, copy-pasteable rewrites - not just directions. For a weak hook, write the replacement hook. For a weak CTA, write the replacement CTA. Each fix should say _why_ it helps (e.g. "moves the stat into the first line so it survives the 'see more' cutoff, which raises pre-expansion click-through").

End with: **"Score after fixes (estimated): NN/100"** if the person applies the changes above.

**Notes for applying this well**

- Ground every score and every piece of advice in either (a) something you just found via search, cited by source name, or (b) something explicitly labeled "established best practice, not confirmed by a recent source" - never state a specific algorithm mechanic with confidence unless it's backed by one or the other.
- This person's posts are usually for the home-based care / healthcare-AI B2B space (AutomationEdge / CareFlo AI) - when relevant, weigh "Audience relevance" and "Personal branding consistency" against that space's norms (compassion-led framing for clinical audiences, stats-forward urgency where appropriate) rather than generic B2B SaaS norms. Don't assume this if the draft is clearly for a different audience or a personal account - check first if unclear.
- Comments and dwell time currently outweigh raw like-counts in distribution - when scoring "Engagement potential" and "Comment generation potential," reward posts that invite a real opinion or experience ("What's your team's take on X?" beats "Like if you agree").
- **Score with 360Brew's behavior specifically in mind**, not just generic "the algorithm." 360Brew is LinkedIn's foundation-model ranking system, and it changes how several categories should be judged: it reads a post's actual meaning rather than counting signals, so (a) it can tell a specific, expertise-inviting question from a generic one - reward "What's the one edge case in X that breaks Y?" over "What do you think?" when scoring "Comment generation potential"; (b) it weighs saves and thoughtful reshares-with-commentary well above likes and blind reshares, which should raise the bar for "Save potential" and "Shareability"; (c) it evaluates a post's topic against the whole profile (headline, About, recent post history) for authority, not the post in isolation - factor this into "Credibility and authority" and "Personal branding consistency," and note explicitly if a post's topic looks like a departure from the account's established few content pillars; (d) it can detect generic, low-substance comment threads ("Great post!" pile-ons) as noise rather than signal, and it can detect AI-templated writing patterns - both feed into the compliance-gate deductions above. Treat "360Brew" as the named mechanism behind these effects when you cite it, rather than a vague "the algorithm."
- Some reporting disagrees on exactly how confirmed/deployed 360Brew is for feed ranking specifically (versus other ranking/recommendation surfaces) - if search results conflict on this point, say so plainly rather than asserting a firm rollout date, and default to treating its behavior patterns as current best-practice guidance either way.
- Native, kept-on-platform content (text, carousels/documents, in-feed video) currently gets a distribution edge over posts leading with an external link - factor this into "LinkedIn algorithm friendliness," and if a link is present, check whether enough context appears before it that the post could stand alone even if the link were removed.
- Hashtags currently carry much less ranking weight than they used to (topic/semantic matching does more of that work) - don't over-penalize a post for using few, well-chosen hashtags, and don't reward a post just for hitting a specific hashtag count.
- If the post is an event-promo post for AutomationEdge/CareFlo (webinar, summit, booth), this algorithm score is a complement to - not a replacement for - the dedicated event-post checklist skill; mention that skill exists if the post looks like an event promo and hasn't been run through it yet.
- If the person pastes multiple drafts/variants at once, score each one separately with its own full output, then a one-line recommendation on which to publish.

**Reference files**

- reference/algorithm-baseline.md - fallback scoring model and reasoning for each category weight, to use only when web search is unavailable or comes back thin. Read this if search results are sparse, to make sure you're not scoring from bare guesswork.

**LinkedIn Algorithm Baseline (fallback reference)**

Use this file only when web search is unavailable, or returns thin/low-quality results. Otherwise, prefer fresh search results - this reference will go stale, and LinkedIn has been changing its ranking system fast through 2025-2026.

**Last grounded:** July 2026, from a mix of LinkedIn's own creator-facing guidance and independent industry analysis of the platform's ranking shifts. Treat anything below as "best practice as of mid-2026," not as LinkedIn's official permanent policy - re-verify with search whenever you can.

**360Brew: the foundation model behind current ranking**

360Brew is LinkedIn's large (reportedly ~150-billion-parameter), decoder-only foundation model for personalized ranking and recommendation, built by LinkedIn's Foundation AI Technologies (FAIT) team and first detailed in a research paper (arXiv, Jan 2025). Reporting through 2026 describes LinkedIn folding feed ranking, search surfacing, and recommendation into this single unified model rather than the older setup of many separate task-specific models. Treat the _exact_ deployment status (fully live in feed ranking vs. still partial) as unconfirmed by any single authoritative source as of this writing - some coverage cites an official LinkedIn Engineering announcement, other coverage frames the feed-ranking link as inferred. Score using its described behavior patterns either way, since those patterns show up consistently across independent sources:

- **Reads meaning, not just signal counts.** Because it's a language model, it can tell a specific, expertise-inviting question from a generic engagement-bait one, and can identify a comment thread that's substantive versus a pile of "Great post!" replies from the same small circle.
- **Profile and content are evaluated as one unit** - described as a "contextual content ecosystem." A post's topic gets checked against the poster's headline, About section, and recent post history; a post that's a sharp departure from an account's established few content pillars (topic consistency, roughly 3-4 recurring themes) can get suppressed even if the post itself is well written.
- **Saves and reshares-with-commentary are weighted well above likes and blind reshares.** A reshare with a few sentences of the resharer's own take is treated as a stronger cross-network endorsement than a bare reshare; likes alone are a weak signal in this model.
- **Specialized, topic-specific questions outperform generic ones** for drawing the kind of comment 360Brew rewards (e.g. "What's one edge case in home health referral intake that breaks a standard automation workflow?" over "What do you think?").
- **Detects AI-templated writing patterns** at the text level, separate from any single banned phrase - formulaic structure and generic phrasing can suppress reach even without an obvious red flag.

**The core framework LinkedIn itself describes**

LinkedIn has publicly framed its feed ranking around three signals:

- **Relevance** - how closely the post matches the interests of a specific, definable audience (not "everyone").
- **Expertise** - whether the post demonstrates real subject-matter knowledge, cross-referenced against the poster's own profile (headline, About, experience).
- **Engagement** - whether the post sparks _meaningful_ comments from people who genuinely engage with that topic, not just quick reactions.

**360Brew: the foundation model behind current ranking**

360Brew is LinkedIn's large (reported ~150-billion-parameter), decoder-only foundation model for personalized ranking and recommendation, built by LinkedIn's Foundation AI Technologies (FAIT) team and detailed in an arXiv paper (Firooz et al., submitted January 2025). Industry reporting through 2026 describes LinkedIn deploying it as the unified engine behind feed ranking, search, and recommendations - replacing what was previously a set of separate, task-specific ranking models with one model that reasons over content the way a person would, rather than just tallying likes/comments/shares as separate counted signals. Some sources note this deployment-for-feed-ranking specifically isn't 100% officially confirmed by LinkedIn in the same breath as the paper itself - treat the mechanism as credible current best-practice guidance, but don't state a specific rollout date as hard fact without a fresh source backing it.

What this means in practice for scoring a post:

- **Meaning over metrics**: because it reads content semantically rather than just counting actions, a comment like "Great post!" is treated as low-value noise even if the comment count looks healthy - score "Comment generation potential" on whether a post invites a _specific, substantive_ answer, not just any reply.
- **Saves and reshares-with-commentary > likes and blind reshares**: a reshare with three-plus sentences of the resharer's own take is read as a stronger endorsement signal than a bare reshare or a like. Weight "Save potential" and "Shareability" accordingly - a post that gives someone something worth bookmarking or restating in their own words outperforms one that's just agreeable.
- **Profile-content coherence as a unified signal**: 360Brew is described as evaluating a poster's profile (headline, About, experience) and their body of content together as one "contextual ecosystem," rather than judging each post in isolation. A post whose topic doesn't match the account's established few content pillars can get suppressed even if the post itself is well written - factor this into "Credibility and authority" and "Personal branding consistency," and flag if a draft looks like a topic departure from the account's normal focus.
- **AI-generated/templated detection**: reporting describes this system as specifically able to detect and deprioritize generic AI-sounding content, reinforcing the existing compliance-gate deduction for templated phrasing.
- **Semantic relevance over broad reach**: distribution is described as "precision delivery" to the specific people likely to care about a topic, rather than maximum broadcast - a very generic, broadly-worded post can underperform a narrower, sharper one aimed at a defined audience, even though the narrower one looks like it has a smaller addressable audience on paper.

**What's changed through 2025-2026 (why the weights above are set where they are)**

- **Dwell time / "Depth Score"**: how long a person actually reads or watches before scrolling away has become a headline ranking input - posts holding attention for real time outperform posts that only rack up quick likes. This is why "Value delivered," "Storytelling quality," and "Readability" carry meaningful weight in the rubric - they're the levers that actually produce dwell time.
- **"See more" expansion rate**: whether people bother to expand a truncated post is tracked and rewarded, which is why the first ~200 characters (before truncation) matter so much - this is the basis for weighting "Hook strength" and "First 2-3 lines effectiveness" together at 11 of the 100 points.
- **Comment quality over comment count**: the algorithm can distinguish a substantive reply from "Great post!" or emoji-only comments from the same small circle. Comment-bait ("comment YES if...") is actively suppressed. This is reflected in the compliance-gate deduction and in how "Comment generation potential" should be scored - reward posts that invite an actual opinion, not a reflex reaction.
- **Profile-post cross-referencing**: LinkedIn increasingly checks a claim in a post against the poster's own profile (headline/About/experience) to judge credibility before amplifying it. This underlies "Credibility and authority" and "Personal branding consistency."
- **Native format preference**: text posts, carousels/documents, and native video that keep people on-platform tend to get a distribution edge over posts that lead with an external link. A link isn't disqualifying, but the post should stand on its own and give enough context before the link that a reader isn't required to leave the platform to understand the point. This is folded into "LinkedIn algorithm friendliness."
- **Hashtags de-emphasized**: topic/semantic matching (the platform reading the actual text) has taken over much of what hashtags used to do for categorization. A handful of specific, well-chosen hashtags is still fine; stuffing more in doesn't help and can look noisy. This is why "Hashtag strategy" carries only 2 of the 100 points.
- **AI-sounding / templated content flagged**: generic, formulaic phrasing patterns (stock hooks, stock CTAs, obviously-templated structure) are increasingly detected and can suppress reach even without any other red flag. Factor this into "Originality" and the compliance gate.
- **Engagement bait actively suppressed**: explicit asks like "like if you agree," "tag 3 people," or "comment YES" reduce rather than help distribution - treat any of these as an automatic compliance-gate deduction, not a stylistic nitpick.
- **Evergreen posts have a short shelf life**: most organic posts see the bulk of their distribution within roughly the first 1-3 weeks, with an initial small "test" audience (sometimes called the "golden hour") determining whether a post gets pushed further. Early, genuine engagement in that window matters more than post age or general topic evergreen-ness.

**Using this baseline responsibly**

- Never present anything in this file as if it were a live, just-verified fact about LinkedIn's current system - frame it as "established best practice as of mid-2026" when you're relying on this file instead of a fresh search.
- If the person is scoring several posts in a row in the same conversation, only re-run the search refresh once near the start, not before every single post - reuse what you found unless a lot of time has passed in the conversation or the topic clearly requires a fresh check.