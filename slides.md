---
marp: true
theme: default
paginate: true
backgroundColor: #0d1117
color: #e6edf3
style: |
  section {
    font-family: 'Segoe UI', Arial, sans-serif;
    padding: 48px 60px;
  }
  h1 {
    color: #58a6ff;
    font-size: 2.2em;
    border-bottom: 2px solid #21262d;
    padding-bottom: 12px;
  }
  h2 {
    color: #79c0ff;
    font-size: 1.6em;
  }
  h3 {
    color: #d2a8ff;
    font-size: 1.2em;
  }
  strong {
    color: #ffa657;
  }
  em {
    color: #a5d6ff;
  }
  blockquote {
    border-left: 4px solid #58a6ff;
    color: #8b949e;
    padding-left: 16px;
    font-style: italic;
    font-size: 1.1em;
  }
  ul li, ol li {
    margin-bottom: 10px;
    line-height: 1.6;
  }
  .columns {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 32px;
  }
  section.lead h1 {
    font-size: 2.8em;
    border: none;
  }
  section.center {
    text-align: center;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
  .pill {
    display: inline-block;
    background: #21262d;
    border: 1px solid #30363d;
    border-radius: 20px;
    padding: 4px 14px;
    font-size: 0.85em;
    margin: 4px;
  }
---

<!-- _class: lead center -->

# Trustworthy AI
## Keeping Humans at the Heart of Intelligent Systems

<br>

**SlashNew Conf · 2026**

---

<!-- _class: center -->

# The question is no longer *whether* machines will assist us.

<br>

> "The question is how we ensure they do so **responsibly**."

---

## A Tale of Two Futures

<div class="columns">

<div>

### 🤖 AI Without Trust

- Opaque decisions nobody can explain
- Bias baked silently into outcomes
- Human judgment replaced, not amplified
- Accountability gaps at every level
- Erosion of user confidence

</div>

<div>

### 🤝 AI With Trust

- Transparent reasoning, auditable trails
- Fairness built in from the start
- Human oversight at every critical loop
- Clear accountability chains
- Technology people actually *believe in*

</div>

</div>

---

## About Me

<div class="columns">

<div>

**[Speaker Name]**
*[Title · Organisation]*

- AI practitioner & advocate for human-centred design
- Working at the intersection of responsible AI and software engineering
- Passionate about building systems that earn trust

</div>

<div>

**What I've seen in the wild:**

- AI systems that optimised for the metric, not the mission
- Teams shipping "magic" they couldn't explain to users
- And teams that got it beautifully right

</div>

</div>

---

<!-- _class: center -->

## Today's Journey

<br>

**1 · Human-in-the-Loop Design**
Why oversight isn't optional

**2 · Principles of Trustworthy AI**
Explainability · Reliability · Inclusivity

**3 · Real-world Practices**
Governance + empathy, without slowing down

<br>

*45 minutes · actionable takeaways · no hype*

---

## Three Waves of AI-Assisted Development

<div class="columns">

<div>

### 🌊 Wave 1 — Pair Programmer
*Inline suggestions and autocomplete*
**Coding what you were going to code anyway, just faster.**

<br>

### 🌊 Wave 2 — Peer Programmer
*Synchronous agent mode*
**The agent takes a bounded task while you code together in real time.**

</div>

<div>

### 🌊 Wave 3 — Asynchronous Agentic SDLC
*Multi-agent workflows · autonomous task execution*
**Agents execute work across the delivery lifecycle while humans orchestrate, review, and own outcomes.**

<br>

> **Key message:** Each wave expands scope —
> from *code tokens* → to *tasks* → to *end-to-end outcomes*.

</div>

</div>

---

## Wave 3 Changes the Operating Model

- **Wave 1** helped me *type* faster.
- **Wave 2** helped me *think and build* in parallel.
- **Wave 3** changes the *operating model*: agents execute work while we **orchestrate, review, and own outcomes**.

<br>

### This is why *humans at the heart* matters more now than ever.

- As autonomy rises, **accountability doesn't disappear — it concentrates.**
- **Rule Zero:** *You own the code.*

<br>

> In Wave 3, human-in-the-loop is no longer a nice-to-have UX pattern —
> it is the **control system** for safe, scalable delivery.

---

<!-- Divider slide -->
<!-- _class: lead center -->

# Part 1
## Human-in-the-Loop Design

*Why human oversight is critical for mitigating bias and ensuring ethical outcomes*

---

## What Is Human-in-the-Loop?

A design pattern where **human judgment is embedded** in the AI decision pipeline — not bolted on at the end.

<br>

| Mode | Description | When to use |
|---|---|---|
| **Human-in-the-loop** | Human approves each decision | High-stakes, low-volume |
| **Human-on-the-loop** | Human monitors, can intervene | Medium-stakes, real-time |
| **Human-in-command** | Human sets goals & constraints | High-volume automation |

<br>

> The right level of oversight depends on **stakes × reversibility**.

---

## Why Machines Still Need Us

- **Distributional shift** — the world changes; training data doesn't update itself
- **Edge cases** — models fail silently on inputs they've never seen
- **Values** — fairness, dignity, and ethics are *not* loss functions
- **Accountability** — "the model decided" is not a legal or moral defence
- **Context** — humans carry cultural, emotional, and situational nuance no dataset fully captures

---

## The Bias Amplification Problem

```
Biased data  →  Trained model  →  Biased predictions
     ↑                                    |
     |___________ feedback loop __________|
```

<br>

**Without human checkpoints:**
- A hiring model trained on historical data under-ranks qualified candidates from underrepresented groups
- A medical triage model deprioritises patients whose symptoms were historically underdocumented
- Each new batch of data *reinforces* the original skew

**Human oversight breaks the loop.**

---

## Designing Effective Human Checkpoints

✅ **Define decision boundaries upfront** — which outputs require human sign-off?

✅ **Surface uncertainty explicitly** — show confidence scores, not just answers

✅ **Make override easy and logged** — if overriding is painful, people skip it

✅ **Avoid automation bias** — design UI so humans genuinely deliberate, not just rubber-stamp

✅ **Close the feedback loop** — human corrections should retrain the model

---

## Case Study: AI-Assisted Code Review

<div class="columns">

<div>

**Without HITL**
- AI auto-merges PRs below a risk threshold
- A subtle logic error passes silently
- Production incident; no audit trail
- "The AI approved it" — *whose fault?*

</div>

<div>

**With HITL**
- AI flags risk areas with reasoning
- Developer reviews flagged sections
- Decision logged with rationale
- Continuous improvement from corrections

</div>

</div>

<br>

> The developer's intuition caught what the model missed. **That's the point.**

---

<!-- Divider slide -->
<!-- _class: lead center -->

# Part 2
## Principles of Trustworthy AI

*Explainability · Reliability · Inclusivity as non-negotiables*

---

## The Trust Triangle

```
           EXPLAINABILITY
               /\
              /  \
             /    \
            /      \
           /________\
    RELIABILITY    INCLUSIVITY
```

<br>

Remove any corner and the triangle collapses. **All three must hold simultaneously.**

---

## Explainability — "Show Your Work"

**Why it matters:**
- Users won't trust what they can't understand
- Regulators increasingly *require* it (EU AI Act, GDPR Art. 22)
- Developers can't improve what they can't inspect

**Practical techniques:**

| Technique | Best for |
|---|---|
| LIME / SHAP | Feature importance per prediction |
| Attention visualisation | NLP & vision models |
| Counterfactual explanations | "What would have changed the outcome?" |
| Model cards | Communicating capability & limitations |
| Natural language rationales | End-user-facing explanations |

---

## Explainability — What Good Looks Like

<br>

❌ **"The loan application was denied."**

<br>

✅ **"The loan application was declined primarily because the debt-to-income ratio (42%) exceeded our threshold of 35%, and the credit history length (14 months) is below our 24-month minimum. Improving either factor would significantly change this outcome."**

<br>

> Explanation is an act of **respect** towards the person affected.

---

## Reliability — Trustworthy Enough to Depend On

**Reliability ≠ accuracy.** A model can be accurate *on average* and still fail catastrophically for specific subgroups.

<br>

**What reliability requires:**

- **Robustness testing** — adversarial inputs, out-of-distribution data
- **Uncertainty quantification** — the model knows what it doesn't know
- **Graceful degradation** — fail safely, not silently
- **Monitoring in production** — drift detection, anomaly alerting
- **Rollback plans** — because production surprises are inevitable

---

## Reliability — The SRE Mindset Applied to AI

| Traditional SRE | AI Reliability |
|---|---|
| SLOs / error budgets | Model performance budgets per segment |
| Incident response | Model degradation runbooks |
| Chaos engineering | Adversarial & perturbation testing |
| Observability (logs, traces, metrics) | Prediction logging, explanation logging |
| Canary deployments | Shadow mode & staged model rollouts |

<br>

> **Treat your model like a production service.** Because it is one.

---

## Inclusivity — Building for Everyone

**The diversity problem in AI:**

- Models trained predominantly on data from specific demographics
- Evaluation benchmarks that don't represent global users
- Teams that lack diversity in lived experience

<br>

**Inclusivity as engineering practice:**

- Disaggregate metrics by demographic subgroups — don't hide behind averages
- Conduct bias audits *before* and *after* deployment
- Involve impacted communities in requirements, testing, and feedback
- Apply inclusive design principles: if it works for the margins, it works for everyone

---

## Inclusivity — The 1 Billion User Test

> If your AI system were used by 1 billion people globally — across age, gender, language, ability, and economic background — **who would it fail?**

<br>

- Does it work in low-bandwidth environments?
- Does it handle non-English text with equal quality?
- Is the UI accessible to screen readers?
- Are the training labels free of cultural assumptions?
- Were marginalised communities consulted, or just considered?

---

<!-- Divider slide -->
<!-- _class: lead center -->

# Part 3
## Real-world Practices

*Integrating governance and empathy into AI workflows without slowing innovation*

---

## The False Dilemma

<br>

<!-- _class: center -->

> "We can move fast **OR** we can be responsible."

<br>

### This is wrong.

<br>

**Responsible AI practices reduce rework, incidents, and reputational damage. They make you faster in the long run.**

---

## Responsible AI Doesn't Have to Be Bureaucracy

**It starts with three habits:**

<br>

**1. Ethics by Design** — raise the questions *before* the first line of code
- What decisions will this system make?
- Who is affected, and how?
- What's the worst plausible failure mode?

**2. Continuous Evaluation** — treat fairness like you treat test coverage
- Not a one-time audit; a living metric

**3. Graduated Autonomy** — earn trust incrementally; don't deploy full autonomy on day one

---

## The Responsible AI Workflow

```
  DISCOVER        DESIGN          DEVELOP         DEPLOY          MONITOR
─────────────────────────────────────────────────────────────────────────────
  Stakeholder    Risk             Fairness        Model card      Drift
  mapping        assessment       testing         published       detection

  Impact         Explainability   Bias audit      Human          Performance
  assessment     requirements     by subgroup     review gate    disaggregation

  Data           HITL             Adversarial     Staged         Incident
  provenance     touchpoints      testing         rollout        playbook
```

---

## Practical Tooling for Responsible AI

<div class="columns">

<div>

**Fairness & Bias**
- Fairlearn (Microsoft)
- AI Fairness 360 (IBM)
- What-If Tool (Google)
- Aequitas

**Explainability**
- SHAP
- LIME
- InterpretML
- Alibi Explain

</div>

<div>

**Governance & Docs**
- Model Cards Toolkit
- Datasheets for Datasets
- Responsible AI Tracker (GitHub)

**Monitoring**
- Evidently AI
- Arize AI
- WhyLabs

**Red-teaming**
- PyRIT (Microsoft)
- Garak

</div>

</div>

---

## Empathy as an Engineering Skill

**Empathy isn't soft — it's a requirement for correct systems.**

<br>

- **User research before training** — understand the humans your data represents
- **Persona-driven red-teaming** — who is most likely to be harmed by an error?
- **Affected community feedback loops** — not just user testing, but *community* testing
- **Ethics champions on the team** — someone whose job includes asking uncomfortable questions
- **Retrospectives on AI failures** — blameless, learning-focused, systemic

---

## Governance Without Gridlock

**Common failure modes:**

| Pattern | Problem | Fix |
|---|---|---|
| Ethics review as final gate | Caught too late to change anything | Shift left — review at design |
| Checklist compliance | Tick-box mentality, no real scrutiny | Outcome-based criteria |
| Siloed AI safety team | Not embedded in delivery | Ethics champions in squads |
| "We'll fix it after launch" | Harm is already done | Staged, monitored rollouts |
| No rollback plan | Irreversible harm | Reversibility as a design constraint |

---

## What Developers Can Do Right Now

🔍 **Ask the hard question early:** "What's the worst this could do?"

📊 **Disaggregate your metrics** — overall accuracy hides subgroup failures

📝 **Write a model card** — even a one-pager forces you to be honest

🔁 **Build feedback loops** — user corrections should reach the model

🛑 **Define your kill switch** — what triggers a rollback, and who can pull it?

🤝 **Include impacted communities** — before launch, not after the incident

🧪 **Red-team your own system** — find the failures before adversaries do

---

## Trust Is an Emergent Property

You cannot install trust as a feature. It **emerges** from:

<br>

<div class="columns">

<div>

- Consistent, explainable behaviour
- Honest communication about limitations
- Rapid, transparent response to failures
- Demonstrable fairness across groups
- Human oversight that *actually* works

</div>

<div>

- Accountability that goes beyond PR statements
- Continuous improvement, publicly tracked
- Communities feeling heard, not just studied
- Engineers who feel safe raising concerns
- Leadership that rewards the right incentives

</div>

</div>

---

## The Stakes Are Real

- **Healthcare:** AI triage that systematically underserves certain populations
- **Criminal justice:** Risk-scoring tools that encode historical bias
- **Hiring:** Resume screeners that replicate past discrimination
- **Credit:** Loan models with proxy variables for protected characteristics
- **Content moderation:** Systems that suppress marginalised voices disproportionately

<br>

> These aren't hypotheticals. They are documented cases. **What we build has consequences.**

---

## The Opportunity

<div class="columns">

<div>

**AI systems that earn trust:**

- Are used, not abandoned
- Scale without causing harm at scale
- Survive regulatory scrutiny
- Attract users *and* talent
- Create genuine, lasting value

</div>

<div>

**Developers who build them:**

- Sleep better at night
- Build longer-lasting careers
- Contribute to a healthier ecosystem
- Demonstrate that *engineering ethics* is not an oxymoron

</div>

</div>

---

<!-- _class: lead center -->

# Trust Is the Ultimate Feature

<br>

*Not a toggle you flip before shipping.*
*A property you earn through every decision.*

---

## Your Actionable Checklist

- [ ] Map stakeholders and affected communities *before* design
- [ ] Define HITL touchpoints and decision boundaries
- [ ] Require explainability at the interface — for users *and* operators
- [ ] Disaggregate evaluation metrics by demographic subgroup
- [ ] Publish a model card (even a draft is better than nothing)
- [ ] Build a staged rollout with monitoring and rollback criteria
- [ ] Schedule bias audits on a cadence, not just at launch
- [ ] Create a safe channel for raising ethical concerns on your team
- [ ] Red-team with diverse personas before deployment
- [ ] Close the feedback loop — corrections should reach the model

---

## Further Reading & Resources

**Frameworks & Guidelines**
- Microsoft Responsible AI Standard
- EU AI Act (2024)
- NIST AI Risk Management Framework
- Google People + AI Research (PAIR) Guidebook

**Communities**
- Partnership on AI
- AlgorithmWatch
- Distributed AI Research Institute (DAIR)

**Essential Reading**
- *Weapons of Math Destruction* — Cathy O'Neil
- *Atlas of AI* — Kate Crawford
- *The Alignment Problem* — Brian Christian

---

<!-- _class: lead center -->

## Thank You

<br>

**[Speaker Name]**
*[Email · LinkedIn · GitHub · Social handle]*

<br>

> *"In the age of AI, trust is the ultimate feature."*

<br>

**Slides & resources:** [link]

---

<!-- _class: center -->

# Q & A

<br>

*What questions do you have?*

<br>

> The best AI systems are built by people who keep asking:
> **"Who might this harm, and what are we doing about it?"**
