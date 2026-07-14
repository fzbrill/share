# Mapping the Governance of Frontier AI — The US Federal Lens

*Written notes, July 2026. Organizing lens: **governance layer**, restricted to the **US federal government**. Layers run from the softest and most operationally powerful (what actually shapes model behavior day to day) down to the hardest and most legally binding (what can actually compel or forbid). The map's central claim is that these two properties run in **opposite directions** — see "The inversion" below.*

**Abbreviation used throughout:** **CBRN** = chemical, biological, radiological, and nuclear (weapons). CBRN is the standard umbrella category across essentially all frontier safety frameworks — it appears as a first-class, named threshold in the labs' own policies (e.g. CBRN-3 / CBRN-4 capability levels; CBRN Low/Medium/High/Critical tiers), as catalogued in METR's [Common Elements of Frontier AI Safety Policies](https://metr.org/common-elements). Alongside CBRN, the other recurring frontier-risk categories are **offensive cyber**, **loss of control**, and **automated AI R&D**.

---

## The one-paragraph version

Frontier AI in the US is governed mostly by the companies themselves, lightly supervised by a voluntary federal testing body ([CAISI](https://www.nist.gov/caisi)), steered by a stack of reversible executive orders, and hard-constrained at only one point: export controls. Congress has passed no comprehensive frontier-AI statute. The binding action is happening in two places the federal government does *not* fully control on its own — export law (which it does control, and used for the first time in June 2026 to pull a deployed model offline) and **state** law (which it is actively trying to preempt without yet replacing). The result is a system with a great deal of process and very little enforceable safety floor.

---

## Layer 1 — Corporate self-governance *(softest bindingness, most operational power)*

Where almost all real decisions about frontier-model safety are actually made.

- **Actors:** the frontier labs — Anthropic, OpenAI, Google DeepMind, xAI, Meta — and their internal safety/policy teams and boards.
- **Mechanisms:** each lab's own risk framework — Anthropic's [Responsible Scaling Policy](https://www.anthropic.com/rsp) (ASL tiers), OpenAI's [Preparedness Framework](https://openai.com/preparedness/) (tracks CBRN, cybersecurity, persuasion, model autonomy), Google DeepMind's [Frontier Safety Framework](https://deepmind.google/) — plus internal red-teaming and public **system cards**. Labs define their own thresholds, run their own evaluations, and set their own release terms.
- **Bindingness:** none external. Labs write, interpret, and enforce these rules on themselves and can revise or waive them.
- **Illustration from the Mythos work:** the Mythos Preview system card *is* this layer — a lab voluntarily withholding a model, running its own alignment/CBRN/cyber evaluations, and publishing results on its own terms. Nothing external required it.

## Layer 2 — Voluntary government–industry engagement *(soft law)*

The federal government's main hands-on contact with frontier models, built almost entirely on voluntary cooperation.

- **[CAISI](https://www.nist.gov/caisi) (Center for AI Standards and Innovation)** — inside NIST/Commerce; the renamed successor to the US AI Safety Institute. Holds **voluntary pre-deployment testing agreements** with five labs (OpenAI, Anthropic, Google DeepMind, Microsoft, xAI); has run 40+ evaluations (including of unreleased models) on cyber, bio, and chemical risk; also evaluates foreign models (e.g. [DeepSeek V4 Pro](https://www.nist.gov/news-events/news/2026/05/caisi-evaluation-deepseek-v4-pro)) for backdoors. Some classified work runs through the interagency **[TRAINS Taskforce](https://www.nist.gov/news-events/news/2024/11/us-ai-safety-institute-establishes-new-us-government-taskforce-collaborate)** — *Testing Risks of AI for National Security*, NIST-led, now 10+ agencies (DoD, including its Chief Digital and AI Office and the NSA; DOE and its national labs; DHS/CISA; NIH). It runs joint evaluations, risk assessments, and red-teaming across the **full CBRN spectrum — including radiological and nuclear** — plus cyber, critical infrastructure, and conventional military capabilities.
- **[NIST AI Risk Management Framework](https://www.nist.gov/itl/ai-risk-management-framework) (AI RMF)** — a voluntary standards/vocabulary framework that much of industry and government treats as the reference point.
- **[June 2, 2026 EO — "Promoting Advanced AI Innovation and Security"](https://www.whitehouse.gov/presidential-actions/2026/06/promoting-advanced-artificial-intelligence-innovation-and-security/)** — creates a *voluntary* framework for developers to give the government **early access to frontier models (up to ~30 days) before wider release**. Explicitly not a license or pre-clearance regime.
- **Bindingness:** low. Participation is optional; leverage comes from labs wanting government goodwill, procurement, and influence over standards.
- **Key dependency:** the government's ability to *see* frontier models depends on labs volunteering them, and its evaluations lean on the labs' own system cards and tooling. The watchdog is largely dependent on the watched.

### What "standards table"? (concretely)

There is an actual forum structure, and it is where the soft-law leverage lives:

- **Domestic:** NIST/CAISI is literally a *standards* body (the "S"), and the [NIST AI RMF](https://www.nist.gov/itl/ai-risk-management-framework) is the de facto US reference standard.
- **International standards:** [ISO/IEC JTC 1/SC 42](https://www.iso.org/committee/6794475.html) is the joint ISO/IEC committee writing AI standards — and its secretariat is held by [ANSI](https://www.ansi.org/) (US), giving American actors an outsized hand.
- **Cross-government evaluation:** the [International Network of AI Safety Institutes](https://cfg.eu/the-ai-safety-institute-network-who-what-and-how/) (launched Seoul, 2024; UK AI Security Institute as coordinator; US among members) runs a shared **Joint Evaluation Protocol**; CAISI and the [UK AI Security Institute](https://www.aisi.gov.uk/) have run [joint evaluations of frontier models](https://blogs.microsoft.com/on-the-issues/2026/05/05/advancing-ai-evaluation-with-the-center-for-ai-standards-us-and-innovation-and-the-ai-security-institute-uk/).

So "a seat at the table" concretely means influence over the RMF, over ISO/IEC SC 42 texts, and over the international evaluation protocols — none binding, but agenda-setting.

## Layer 3 — Executive & administrative action *(the dominant federal instrument today)*

With Congress stalled, the executive branch is where federal AI policy is actually being made — via orders that are fast, wide-ranging, and reversible.

- **[Jan 23, 2025 — EO 14179, "Removing Barriers to American Leadership in AI"](https://www.federalregister.gov/documents/2025/01/31/2025-02172/removing-barriers-to-american-leadership-in-artificial-intelligence)** — revoked Biden's EO 14110 and reset federal posture toward deregulation and AI "dominance"; ordered the Action Plan.
- **[July 23, 2025 — "Winning the Race: America's AI Action Plan"](https://www.whitehouse.gov/wp-content/uploads/2025/07/Americas-AI-Action-Plan.pdf)** — 90+ policy actions across three pillars (accelerate innovation, build AI infrastructure, lead international diplomacy/security), issued with three EOs: promoting the American AI export stack, fast-tracking data-center permitting, and "preventing woke AI" in federal procurement.
- **[Dec 11, 2025 — "Ensuring a National Policy Framework for AI"](https://www.whitehouse.gov/presidential-actions/2025/12/eliminating-state-law-obstruction-of-national-artificial-intelligence-policy/)** — the **preemption push**: directs the Attorney General to stand up an **AI Litigation Task Force** to challenge state AI laws (Commerce Clause / federal-preemption theories) and directs Commerce to flag vulnerable state laws.
- **[June 2, 2026 EO](https://www.whitehouse.gov/presidential-actions/2026/06/promoting-advanced-artificial-intelligence-innovation-and-security/)** — frontier-model security + the voluntary early-access framework (Layer 2) + directs the AG to prioritize prosecuting AI-enabled cybercrime under existing statutes.
- **Existing agency authority pointed at AI:** [FTC](https://www.ftc.gov/) (deceptive/unfair practices), [DOJ](https://www.justice.gov/) (fraud, cybercrime), sector regulators, the [Copyright Office](https://www.copyright.gov/ai/), [FCC](https://www.fcc.gov/). No new frontier-specific powers — old tools on a new target.

### Are the EOs conflicting? If so, what binds?

Mostly **cumulative and consistent**, not conflicting. All four share the same throughline: AI dominance, deregulation, security pursued through *voluntary* means, and hostility to state regulation. The one real tension is between the deregulatory Jan-2025 order and the June-2026 "security" overlay — reconciled by keeping the security measures voluntary so they don't reimpose the burden the first order stripped.

On hierarchy, three rules decide what binds:

1. **Later controls earlier.** Where two EOs conflict, the most recent expression of presidential will governs, and EOs typically state what they revoke or amend (EO 14179 expressly revoked Biden's EO 14110).
2. **EOs are subordinate to statute and the Constitution.** An EO only directs the executive branch within existing authority; it cannot override a law or create obligations Congress hasn't authorized.
3. **That subordination is why the preemption EO has weak teeth.** An executive order *cannot itself preempt* state law — only Congress (or the courts, reading the Constitution) can. That is precisely why the Dec-2025 order has to work *indirectly*: a DOJ litigation task force plus a request that Congress pass a preemption statute. The EO signals intent; it does not bind states.

- **Bindingness:** medium but brittle. EOs move fast and bind agencies, but the next administration can reverse them, and most of this stack directs *voluntary* engagement rather than mandates.

## Layer 4 — Hard law *(hardest bindingness, narrowest scope)*

### 4a. Export controls — the one genuinely binding lever

- **Actors:** Commerce / [Bureau of Industry and Security (BIS)](https://www.bis.gov/).
- **Mechanisms:** controls that have climbed the stack from chips → equipment → compute/cloud → **model weights**. The [AI Diffusion Framework](https://www.federalregister.gov/documents/2025/01/15/2025-00636/framework-for-artificial-intelligence-diffusion) created ECCN **4E091** for frontier model weights trained above **10²⁶ operations** (BIS estimates fewer than five models qualify); exports to non-allied countries are presumptively denied.
- **The precedent that touches the Mythos work:** in June 2026, Commerce Secretary Lutnick's letter forced Anthropic to **disable Fable 5 and Mythos 5 worldwide** — the first time the US directly controlled access to a specific *deployed model version*, restricting it by user nationality under the [EAR](https://www.bis.gov/regulations)'s deemed-export doctrine. The hardest, most enforceable federal action to date — and notably justified on **national-security / export** grounds, not a safety statute.
- **Bindingness:** high. Real penalties, real enforcement — but aimed at *who can access* models (geopolitics), not at *whether a model is safe to deploy* domestically.

### 4b. The legislative frontier — proposed, not enacted

No comprehensive federal AI statute exists. Congress has **twice rejected** a moratorium on state AI laws (the Senate stripped a 10-year moratorium 99–1 in July 2025). What's live:

- **[Great American AI Act (GAAIA)](https://obernolte.house.gov/media/press-releases/obernolte-trahan-release-discussion-draft-great-american-ai-act)** — bipartisan *discussion draft* (Obernolte R-CA / Trahan D-MA, June 4, 2026; **not yet formally introduced**). Would require frontier developers to disclose model information (§111), obtain **independent third-party audits** (§112), and protect whistleblowers (§113), with critical-incident reporting and penalties for noncompliance. Includes a **3-year preemption** of state laws "specifically regulating the development" of AI, while preserving generally-applicable state laws and post-deployment authority ([Roll Call](https://rollcall.com/2026/06/04/bipartisan-ai-draft-proposes-three-year-preemption-of-state-laws/), [TechPolicy.Press](https://www.techpolicy.press/unpacking-the-great-american-artificial-intelligence-act-of-2026/)). *Notably: no authority to block a dangerous deployment.*
- **[Anthropic's Advanced AI Framework](https://www.anthropic.com/policy-on-the-ai-exponential)** (with Dario Amodei's [*Policy on the AI Exponential*](https://darioamodei.com/post/policy-on-the-ai-exponential)) — proposes mandatory testing keyed to a **10²⁵ FLOP** threshold and companies over $500M revenue / $1B R&D, across four risk categories (cybersecurity, biological weapons, loss of AI control, automated R&D), plus authority to **block** deployments that fail. Anthropic **opposes preemption unless federal law is at least as strong as its framework** — a direct shot at GAAIA's clause.
- **Export-control bills:** [AI OVERWATCH Act (H.R. 6875, Mast)](https://www.congress.gov/bill/119th-congress/house-bill/6875/text) — licenses + congressional review for advanced-chip exports (passed House Foreign Affairs 42–2, Jan 2026); [MATCH Act (H.R. 8170, Baumgartner)](https://www.govtrack.us/congress/bills/119/hr8170) — gives allied toolmakers 150 days to match US chip-equipment controls.
- **Bindingness:** zero today (all pending), but the highest *potential* — statute is the only layer that could set a durable safety floor.

## The federal–state axis *(cuts across all layers)*

### Why "100+ state laws" but only ~3 operative obligations *on frontier developers*

The 100+ figure counts **all** state AI laws — the vast majority govern *AI applications and uses* (election deepfakes, hiring/employment tools, insurance, healthcare, chatbot-disclosure, consumer protection). Those bind *deployers and users*, not frontier model *developers*, so they sit outside a frontier-governance map.

Only a handful impose obligations **specifically on frontier model developers** — publish a safety framework, submit to audits, report incidents:

- **[California SB 53 — Transparency in Frontier AI Act (TFAIA)](https://leginfo.legislature.ca.gov/faces/billNavClient.xhtml?bill_id=202520260SB53)** (signed Sept 29, 2025): framework publication, catastrophic-risk reporting to the Office of Emergency Services, critical-incident reporting, whistleblower protection, AG civil penalties.
- **[Illinois SB 315 — AI Safety Measures Act](https://www.crowell.com/en/insights/client-alerts/illinois-imposes-transparency-and-safety-obligations-on-frontier-ai-systems)** (signed July 6, 2026; effective Jan 1, 2027): **first state to mandate independent third-party audits** of frontier models; AG fines up to $1M (first) / $3M (subsequent).
- **[New York RAISE Act — Responsible AI Safety and Education Act](https://www.governor.ny.gov/news/governor-hochul-signs-nation-leading-legislation-require-ai-frameworks-ai-frontier-models)** (final amendment Mar 27, 2026; effective Jan 1, 2027): safety-protocol publication, **72-hour incident reporting**, applies to models trained above 10²⁶ FLOPs / >$100M compute, AG penalties $1M / $3M; modeled on California's "trust but verify."

So for frontier developers, **the real operative obligations in the US today are three state laws** — which is exactly what the federal preemption push (Dec-2025 EO + GAAIA's 3-year clause) aims to clear away.

---

## The wiring — dependencies to notice

- **Government sight depends on corporate consent.** CAISI evaluations, the June-2026 early-access framework, and much of Congress's information rely on labs volunteering models and on the labs' own system cards. Federal capacity to evaluate frontier models is downstream of the companies being evaluated.
- **Soft law leans on hard law for teeth.** Voluntary engagement (Layer 2) and EOs (Layer 3) have leverage largely because the government holds the export-control hammer (4a) and the threat of legislation (4b).
- **Export controls substitute for a safety regime.** With no domestic safety statute, export law does double duty — the Fable/Mythos suspension was a *safety-flavored* action executed through a *national-security* instrument.
- **Preemption is load-bearing.** If federal preemption succeeds before a strong federal statute passes, the binding state layer disappears and the actual safety floor drops, not rises.
- **Reversibility runs through everything executive.** The entire EO stack — and CAISI's posture — can be rewritten by the next administration. Only statute and, to a degree, export regulation are sticky.
- **Thresholds don't line up.** BIS uses 10²⁶ operations; NY uses 10²⁶ FLOPs + $100M; Anthropic's framework uses 10²⁵ FLOPs; Illinois uses compute + $500M revenue. Four "frontier" definitions, four cut-lines — a verification problem in its own right.

---

## The inversion *(is "paradox" the right word?)*

Short answer: **no — "inversion" (or "mismatch") is more accurate than "paradox."** A paradox is an *apparent self-contradiction*; there's nothing self-contradictory here. What the map shows is a real, explicable **inverse relationship**: as you move down the layers, legal bindingness rises while day-to-day operational influence over models falls, and vice versa. The layer that most shapes what models actually do (corporate self-governance) is the least binding; the layer that binds hardest (export control) touches models least and only from the side of *access*. That crossing is a **structural mismatch between where the power is and where the accountability is** — concerning, but not paradoxical. I'll use "the inversion" for the crossing arrows and reserve "paradox" for genuine contradictions.

## Analytical read *(incorporating my prior view — see ["A Race to the Bottom on Safety," June 16, 2026](https://fzbrill.substack.com/p/a-race-to-the-bottom-on-safety-what))*

The inversion makes the "race to the bottom" concrete: **there is no binding federal safety floor**, so competition among labs is checked only by each lab's own discretion (Layer 1) and by a national-security lever aimed at foreign access (4a) — neither of which stops a US lab from deploying a domestically risky model. My position:

1. **The GAAIA is the viable vehicle, but weak as drafted** — real transparency and audits, but *no deployment-blocking authority* (accountability without consequence), plus a 3-year preemption clause.
2. **Passing it as-is could be worse than passing nothing**, because it would let Congress declare victory while wiping out the stronger California/Illinois/New York protections and putting nothing comparable in their place. Anthropic's own anti-preemption stance (preempt only if federal law is *at least as strong*) is effectively a warning to the sponsors.
3. **Two amendments matter most:** (a) strip or narrow preemption (or condition it on the federal standard matching the strongest state / Anthropic-framework benchmark), and (b) add authority to **block or delay** deployments that fail verified tests in the four risk categories, with safeguards against political abuse.
4. **The compute threshold is a leaky proxy.** A 10²⁵–10²⁶ line was meant to track dangerous capability, but DeepSeek showed capability and compute decoupling — so the threshold **systematically captures American labs and misses efficient Chinese ones**. Fixes: lower the threshold over time, add a capability-based trigger, or (most realistically) lean on **export controls** to constrain what can't be verified. *You can't regulate what you can't verify* — which is why the one binding lever we have (4a) keeps ending up at the center of the story.

**Bottom line:** the US federal system today is heavy on voluntary process and executive signaling, light on enforceable safety obligations. Its only hard edge — export control — points outward at adversaries, not inward at the race among domestic labs. Closing that gap requires statute, and the fight over the GAAIA (deployment authority vs. preemption) is where it will be won or lost.

---

## Companion visual

This map has an accompanying diagram (see `US Federal AI Governance Map.svg` / `.png`, and the fully clickable `.html` version). It renders the same structure visually:
- a vertical stack of the four layers, widest-but-lightest at top (corporate) narrowing to hardest-but-narrowest at bottom (export control);
- a right-hand pair of block arrows showing **operational influence increasing upward** and **legal bindingness increasing downward** (the inversion);
- the **federal–state axis** as a side box (California SB 53, Illinois SB 315, New York RAISE Act) level with Layer 4, with a horizontal **preemption** arrow pointing at it;
- **Mythos/Fable** traced as a dotted line touching every layer (system card → CAISI eval / early-access EO → export-control suspension).

---

### Sources
- **Labs:** Anthropic [RSP](https://www.anthropic.com/rsp); OpenAI [Preparedness Framework](https://openai.com/preparedness/); Google DeepMind [Frontier Safety Framework](https://deepmind.google/); Mythos Preview system card + prior research on the Fable 5 export-control suspension.
- **Executive:** [EO 14179](https://www.federalregister.gov/documents/2025/01/31/2025-02172/removing-barriers-to-american-leadership-in-artificial-intelligence) (Jan 2025); [America's AI Action Plan](https://www.whitehouse.gov/wp-content/uploads/2025/07/Americas-AI-Action-Plan.pdf) + 3 EOs (July 2025); [National Policy Framework EO](https://www.whitehouse.gov/presidential-actions/2025/12/eliminating-state-law-obstruction-of-national-artificial-intelligence-policy/) (Dec 2025); [Advanced AI Innovation and Security EO](https://www.whitehouse.gov/presidential-actions/2026/06/promoting-advanced-artificial-intelligence-innovation-and-security/) (June 2026).
- **Testing/standards:** [CAISI](https://www.nist.gov/caisi); [DeepSeek V4 Pro evaluation](https://www.nist.gov/news-events/news/2026/05/caisi-evaluation-deepseek-v4-pro); [NIST AI RMF](https://www.nist.gov/itl/ai-risk-management-framework); [ISO/IEC JTC 1/SC 42](https://www.iso.org/committee/6794475.html); [International Network of AI Safety Institutes](https://cfg.eu/the-ai-safety-institute-network-who-what-and-how/); [UK AI Security Institute](https://www.aisi.gov.uk/); [TRAINS Taskforce](https://www.nist.gov/news-events/news/2024/11/us-ai-safety-institute-establishes-new-us-government-taskforce-collaborate); METR, [Common Elements of Frontier AI Safety Policies](https://metr.org/common-elements).
- **Export controls:** [BIS](https://www.bis.gov/); [AI Diffusion Framework](https://www.federalregister.gov/documents/2025/01/15/2025-00636/framework-for-artificial-intelligence-diffusion) (ECCN 4E091).
- **Legislation:** [GAAIA discussion draft](https://obernolte.house.gov/media/press-releases/obernolte-trahan-release-discussion-draft-great-american-ai-act) ([analysis](https://www.techpolicy.press/unpacking-the-great-american-artificial-intelligence-act-of-2026/)); [AI OVERWATCH Act H.R. 6875](https://www.congress.gov/bill/119th-congress/house-bill/6875/text); [MATCH Act H.R. 8170](https://www.govtrack.us/congress/bills/119/hr8170).
- **State:** [California SB 53 / TFAIA](https://leginfo.legislature.ca.gov/faces/billNavClient.xhtml?bill_id=202520260SB53); [Illinois SB 315](https://www.crowell.com/en/insights/client-alerts/illinois-imposes-transparency-and-safety-obligations-on-frontier-ai-systems); [New York RAISE Act](https://www.governor.ny.gov/news/governor-hochul-signs-nation-leading-legislation-require-ai-frameworks-ai-frontier-models).
- **Opinion:** Frank Z. Brill, ["A Race to the Bottom on Safety"](https://fzbrill.substack.com/p/a-race-to-the-bottom-on-safety-what) (June 16, 2026); Dario Amodei, [*Policy on the AI Exponential*](https://darioamodei.com/post/policy-on-the-ai-exponential).
