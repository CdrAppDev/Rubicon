# Why AI adoption in due diligence remains stubbornly low

**The 16% adoption rate for AI in M&A due diligence is not a single-barrier problem — it is a cascading "trust stack" failure where accuracy deficits, security risks, regulatory exposure, workflow friction, and economic misalignment compound to make adoption rationally unattractive for most deal teams.** This matters for Rubicon because addressing any one layer in isolation will not move adoption; the platform must dismantle the entire stack simultaneously. The research below synthesizes findings from 40+ sources across management consulting surveys, legal technology evaluations, regulatory guidance, and practitioner accounts to map every documented barrier and identify the precise conditions under which deal professionals would adopt.

---

## The rank-ordered barrier hierarchy shows data security, not cost, is the real blocker

Cross-referencing six major surveys from 2024–2025 reveals a consistent hierarchy of barriers — and several surprises about what does *not* matter.

**Deloitte's 2025 M&A Generative AI Study** (1,000 senior corporate and PE leaders) produced the most DD-relevant rank ordering: **data security at 67%**, data quality/availability at 65%, model reliability at 64%, ethical considerations at 62%, and regulatory/compliance uncertainty at 61%. These figures cluster tightly, suggesting deal professionals see these as interconnected rather than distinct. The **KPMG Q3 2025 AI Quarterly Pulse Survey** reinforced this with even higher numbers in an enterprise context: data quality at **82%** (up from 56% the prior quarter), cybersecurity at **78%** (up from 68%), and data privacy at 62%.

The **ABA TechReport 2024** (512 attorneys) surfaced a different hierarchy specific to lawyers: accuracy/hallucination concerns dominated at **75%** (up sharply from 58% the prior year), followed by reliability at 56.3% and data privacy/security at 47.2%. Three-quarters of surveyed lawyers said hallucination risk was the primary reason they hesitate to implement AI. The **ILTA 2024 Technology Survey** (536 firms, 138,000+ attorneys) found **54% cited resistance to change** as the biggest hurdle to emerging technology adoption.

What the data consistently shows is that **budget and leadership buy-in are not the real barriers**. KPMG found budget constraints cited by only **14%** and leadership buy-in by only **8%** — the lowest factors every quarter. A Ropes & Gray/Corporate Counsel survey found only 7% cited budgetary constraints. Basic legal AI tools cost $50–$200/month per user. The barriers are trust-based, not resource-based. PwC's 2025 AI Agent Survey made this explicit: cybersecurity (34%) and cost (34%) topped the self-reported list, but PwC argued these are "safe excuses" masking the real barriers — organizational change (17%) and employee adoption (14%) — which respondents underreport because they're harder to admit.

---

## Deal data is MNPI by definition, and that changes everything about security

The security barrier in DD is qualitatively different from general enterprise AI security concerns because **due diligence data constitutes Material Non-Public Information (MNPI)**, creating insider-trading-level regulatory exposure. Inputting MNPI into unsecured or unapproved AI systems is **expressly prohibited** for investment advisers. The SEC has imposed penalties exceeding $10 million for MNPI-related violations, and a public company employee uploading MNPI into a consumer AI tool could violate Regulation Fair Disclosure.

EY Switzerland's analysis identified the fundamental structural barrier: "Data in virtual data rooms is usually well protected and the sell side is often not willing to have their confidential information used for AI training. Also, the VDR provider is generally mandated by the seller. Hence, developing and training algorithms for M&A due diligence may be very limited 'on the fly' in running transactions." This creates a triple lock: the seller controls VDR access, resists AI model training on deal data, and mandates the VDR provider — meaning buyer-side AI tools face structural access limitations.

The specific security concerns, as documented across National Law Review interviews with legal tech executives and law firm policy frameworks, center on five questions firms ask vendors: (1) Do you employ encryption? (2) Do you train on data I submit? (3) Do you mask PII before LLM processing? (4) Can I control data retention duration? (5) Where is the data processed geographically? The minimum certification stack firms require is **SOC 2 Type II plus ISO 27001**, with best-in-class vendors adding ISO 27701 (privacy) and ISO 42001 (AI governance). Encryption must be **AES-256 at rest and TLS 1.2+ in transit**. Zero model training on client data is a non-negotiable contractual commitment.

A Zscaler 2025 threat report analyzing roughly one trillion AI transactions found that **72% of corporate environments had a critical vulnerability discovered on the first test** of their AI system. This validates the caution. Meanwhile, Stanford Law School research found that **88% of AI vendors impose liability caps** and only 17% explicitly commit to complying with all applicable laws (versus 36% in broader SaaS), forcing firms using AI DD tools to assume compliance responsibility themselves.

The timeline mismatch compounds the problem: SOC 2 Type II certification takes 6–12 months, law firm AI tool vetting involves policy committees, security audits, and pilot phases, and EY describes a process of "small-scale pilots, developer feedback, certification for compliance and data security, then scaled testing." **Deals close in 4–6 weeks; security vetting takes 6–12 months.** By the time an AI tool is approved, the deal that motivated procurement is long closed.

---

## The accuracy gap is 5–19 percentage points below what lawyers require

The most rigorous independent accuracy benchmarks reveal a persistent gap between what AI delivers and what DD demands. **Stanford's RegLab study** (published in the Journal of Empirical Legal Studies, 2025) found that leading RAG-based legal AI tools hallucinate between **17% and 34%** of the time — Lexis+ AI at 17%+, Westlaw AI-Assisted Research at 34%+, and general-purpose GPT-4 at 58–82% on legal queries. This despite vendor marketing claiming "hallucination-free" results.

The accuracy threshold professionals require is stark: the **Thomson Reuters 2025 Future of Professionals Report** found that **41% of legal professionals said AI outputs would need to be 100% accurate** before they could be used without human review, and 9 out of 10 said computers should be held to higher accuracy standards than humans. For high-stakes legal data extraction (renewal dates, payment terms, termination clauses), Sirion's enterprise framework specifies a minimum of **95%+ accuracy with human validation**. Current tools deliver 80–93% on structured tasks with clean data, creating a **5–19 percentage point gap**.

Kira Systems, the market-leading DD tool, claims "90%+ accuracy with hybrid AI across 1,400+ proprietary AI fields." But Artificial Lawyer's independent review (24 firms surveyed) found that custom Quick Study models start at roughly **80% accuracy** and require extensive training. Users reported: "We need a lot of examples to train it and also that the more variety you give the system the less accurate it becomes." The CUAD benchmark (Contract Understanding Atticus Dataset) found transformer models achieved only **72% F1** on contract clause extraction tasks.

The error asymmetry makes this especially dangerous for DD. **False negatives — missing a hidden liability — are catastrophically more costly than false positives.** Koley Jessen law firm documented a case where AI summarized a supplier contract as "low-risk" but missed a critical change-of-control clause requiring supplier consent for M&A. In another case, an AI hallucinated a non-existent tax declaration document, leading to discovery of a **$1.5 million tax liability post-deal**, reducing deal value by 10%. When UBS acquired Credit Suisse under compressed DD timelines, it set aside approximately **$4 billion** for legal and regulatory fallout from inadequate diligence.

Trust in AI tools is also asymmetrically fragile. As SpotDraft's analysis in Artificial Lawyer noted: "It only requires a couple of inaccurate results for legal teams to lose faith in a new tool entirely." Many correct results build trust slowly; a single error destroys it fast.

---

## A regulatory and liability landscape that punishes both use and non-use of AI

The regulatory environment creates what practitioners describe as a "damned if you do, damned if you don't" dynamic. **ABA Formal Opinion 512** (July 29, 2024) established that all existing Model Rules of Professional Conduct apply to AI use, specifically naming "due diligence" and "document review" as tasks where generative AI may assist — but with substantial guardrails. Under **Model Rule 1.1 (Competence)**, lawyers must have "a reasonable understanding of the capabilities and limitations" of any AI tool. The NCBE Bar Examiner's analysis was blunt: "Lawyers' uncritical reliance on content created by a GAI tool is risky — and **almost certainly malpractice**."

Under **Model Rule 1.6 (Confidentiality)**, before inputting client information into self-learning AI tools, lawyers must obtain **informed client consent** — and boilerplate waivers are explicitly deemed insufficient. The client must receive the lawyer's "best judgment about why the GAI tool is being used, the extent of and specific information about the risk, including particulars about the kinds of client information that will be disclosed." For DD platforms processing deal data from multiple clients, this is an enormous consent burden.

The liability exposure is personal and uninsured. No profession allows reliance on AI as a complete defense against malpractice liability. As the ABA Journal reported in February 2025, **many lawyers may be surprised to learn that malpractice policies do not explicitly cover AI-related claims** — AI tool use may not satisfy the definition of "professional service," and sanctions flowing from AI tool use may not be covered. Comprehensive AI insurance policies for lawyers do not yet exist, though Munich Re's aiSure product and Orbital Witness's insurance-backed guarantees represent early market entrants.

Simultaneously, a growing legal argument holds that **failure to use AI may itself constitute malpractice**. If AI tools can perform a research task in seconds, charging eight hours of manual research time may violate Rule 1.5 (reasonable fees) and Rules 1.1/1.3 (competence/diligence). This creates a regulatory trap: use AI without sufficient oversight and face malpractice for reliance errors; decline to use AI and face malpractice for inefficiency.

For PE firms, the SEC's 2019 fiduciary duty interpretation confirms that private fund managers have a non-waivable duty to "perform adequate due diligence on the fund's investments." Black-box AI models directly conflict with this duty because advisers cannot comprehend or explain the AI's methods. The **EU AI Act** (effective August 2, 2026 for high-risk rules) classifies customer due diligence systems, credit scoring, and AML monitoring as high-risk, imposing strict requirements for risk management, data quality, technical documentation, audit logging, human oversight, and transparency. Non-compliance fines reach **up to 7% of global annual turnover or €35 million**. FINRA's 2026 Annual Regulatory Oversight Report dedicates a significant section to GenAI, emphasizing that supervisory rules "continue to apply when firms use GenAI" and flagging auditability, transparency, and scope of AI agent authority as key concerns. Across jurisdictions, the state bar landscape is a patchwork — dozens of states have issued individual AI guidance with no uniformity, while the UK SRA has offered "no substantive guidance" at all, creating a regulatory grey area.

---

## Nearly every first-wave legal AI company failed, and pilots die at 95%

The implementation evidence is sobering. MIT research confirms that **95% of AI pilots across industries fail** to deliver measurable business impact. Axiom Law documented its own failures: "We piloted a general-purpose legal AI tool to a subset of our lawyer bench. We assumed our lawyers, who are smart, tech-forward professionals, would figure out how to extract value from it. We were wrong. Adoption stalled within weeks." Their Microsoft Copilot evaluation followed the same pattern: "impressive technology, enthusiastic launch, then crickets." The failure mode: "Your team opens the tool, stares at a blank prompt, and has no idea what to do with it."

**Bloomberg Law's 2025 analysis** quantified the expectations-versus-reality gap: in 2024, 75% of law firm lawyers predicted AI would increase automated processes. In 2025, only **37%** reported this actually happened. The explanation: "Transitioning from legacy systems, getting security credentials in place, setting up training programs, and handling a host of other integration challenges may be making implementation more complex than anticipated."

Perhaps most telling is the fate of the first-wave legal AI pioneers. **Virtually every one has been acquired, shut down, or consolidated**: RAVN (sold to iManage), eBrevia (sold to Donnelly Financial), Kira Systems (sold to Litera), Seal Software (sold to DocuSign), Leverton (sold to MRI, "had a bumpy journey"), RFRNZ (closed — "lack of demand from lawyers"), ROSS Intelligence (shut down after Thomson Reuters lawsuit), Evisort (sold to Workday), Eigen Technologies (sold to Sirion), Casetext (sold to Thomson Reuters). The standalone AI DD tool model has not survived independently. When Kira was sold to Litera, Luminance publicly offered a "rescue package" for concerned Kira clients, illustrating the platform risk firms face when their custom clause training is locked into a vendor that changes ownership.

The workflow integration barriers compound these failures. Data preparation is a critical bottleneck: "Organizing the data to be effectively engaged with by legal tech is a very time-consuming process in itself — at times organizing the data to be analysed by the legal tech could take up more time than the analysis itself." AI tools assume structured input; DD data rooms contain decades-old faxed contracts, handwritten amendments, mislabeled files, and documents in multiple languages. Kira's own users report persistent issues with OCR not handling handwriting, watermarks causing problems, large tables presenting "serious limitations," and party name confusion. The "last mile" problem means that even when AI generates findings, **100% human verification is still required** for high-stakes DD — potentially negating the time savings that justify adoption. And AI output formats (dashboards, JSON) do not match deal team deliverables (Word DD reports, PowerPoint presentations, Excel checklists).

---

## The 10x firm-size gap is driven by innovation teams and deal volume, not budget

The adoption chasm between large and small firms is dramatic and consistent across sources. ILTA 2024 found **20% GenAI adoption at firms under 50 lawyers versus 74% at firms with 700+**. For Copilot specifically, 4% of small firms are piloting versus 50% of the largest firms, and 37% of small firms have zero Copilot plans versus 0% of the largest firms. ABA data shows a gradient from 17.7% for solo practitioners to 47.8% for firms with 500+ lawyers.

The evidence consistently shows this gap is **not primarily about budget**. The real drivers are:

- **Dedicated innovation infrastructure**: Large firms have in-house AI task forces (ILTA 2025 found half of all firms now have them), innovation officers, and IT support teams. Small firms lack this entirely.
- **Deal volume amortization**: Large firms and PE shops process enough deals to justify AI investment and amortize the learning curve. A small firm doing 2–5 deals per year cannot justify dedicated AI infrastructure for DD.
- **Governance capacity**: 34% of law firms have no official GenAI policy; 33% of PE/VC firms lack formal AI policies. Large firms have compliance teams to build governance frameworks; small firms don't.
- **Talent availability**: Bain found **75% of companies struggle to find in-house GenAI expertise**. Large firms hire specialized AI talent; small firms rely on partners who may lack technical literacy.
- **Risk asymmetry**: Small firms can't afford a mistake on any given deal; their risk aversion is proportionally higher because each deal represents a larger share of revenue.

Shadow AI use complicates the picture. ILTA notes that "tracking of 'stealth' Gen AI use can be elusive" — solo and small firm lawyers may use ChatGPT without firm knowledge or approval, meaning actual usage is higher than formal adoption surveys suggest. Axiom's survey found **83% of in-house lawyers use AI tools not provided by their company**, and 81% use unapproved tools.

---

## What would tip adoption: integration, explainability, and insurance-backed guarantees

The research identifies specific conditions and features that would move deal professionals from reluctance to adoption. The **2025 Legal Industry Report** (2,800+ respondents) found that **43% adopted legal-specific AI because tools were integrated with software they already use** — making workflow integration the single strongest adoption driver. Another 33% said provider understanding of firm workflows was key, and 29% expressed greater trust in legal-specific tools versus consumer AI.

The requirements that emerge from synthesizing all sources form a clear product specification:

First, **near-perfect accuracy with full source traceability**. Not just confidence scores — tools must show which specific document, page, and clause informed each finding. As Artificial Lawyer reported: "Ask 'Why did the AI flag this clause as problematic?' If you hear 'proprietary algorithms' or just 'confidence scores,' you're looking at a black box lawyers won't trust." Thomson Reuters data shows professionals hold AI to superhuman standards, demanding 100% accuracy even though human DD has 15–25% error rates.

Second, **contractual and architectural security guarantees**. Zero model training on client data, private or on-premise deployment options, in-region data processing for cross-border deals, and information barrier enforcement for multi-deal environments. The tool must be certifiable as SOC 2 Type II and ISO 27001 at minimum, with a path to ISO 42001 (AI governance).

Third, **human-in-the-loop by design**. KPMG found **61% require human oversight for autonomous agents** and 63% won't allow AI access to sensitive data without human control. The platform must be architected around human validation, not around replacing humans.

Fourth, **insurance-backed output guarantees**. Munich Re's aiSure product and Orbital Witness's insurance-backed AI guarantee in real estate DD demonstrate the model. An AI DD platform that offers financial backing for its accuracy claims would address the malpractice insurance gap directly.

Fifth, **out-of-the-box readiness with deal-timeline-compatible onboarding**. Axiom's failure analysis showed that complex tools requiring months of configuration become shelfware. As one legal operations director put it: "It needs to be out-of-the-box. Ready to go." With DD timelines of 4–6 weeks, the tool must deliver value on the first deal, not the fifth.

Sixth, **client pressure as an external catalyst**. Thomson Reuters reports that some clients have already started requiring AI use "in certain situations," and "AI discounts" are appearing in legal RFPs. Organizations with visible, defined AI strategies are **3.5x more likely to experience critical AI benefits** (Thomson Reuters 2025). The most powerful adoption driver may not be solving barriers but creating external market pressure.

---

## Conclusion

The 16% DD adoption rate is rational, not irrational. Deal teams face a genuine trust stack where each barrier amplifies the next: AI accuracy in the 80–93% range feeds security concerns about unverified outputs, which feed regulatory uncertainty about liability for AI errors, which feeds cultural resistance from risk-averse professionals, which feeds implementation failure when pilots lack organizational commitment. The barriers are not independent — they are load-bearing layers in a structure of professional caution.

Three insights change the conventional framing. First, **the billable hour conflict is an underappreciated structural barrier**: 90% of legal spend flows through hourly billing, meaning AI that makes DD faster directly reduces law firm revenue. PE firms and corporate acquirers doing DD in-house don't face this conflict, making them more natural early adopters than law firms. Second, **the "non-use malpractice" argument is emerging as a potential tipping point** — the legal profession may soon face more risk from *not* using AI than from using it, creating urgency where fear currently dominates. Third, **vendor consolidation has eliminated nearly every independent AI DD tool**, meaning the market is resetting rather than maturing — new entrants face less established competition than conventional wisdom suggests, but must overcome the scar tissue left by failed predecessors.

For Rubicon, the implication is architectural: the platform must be secure enough for MNPI (zero-training, private deployment, information barriers), accurate enough for professional reliance (95%+ with full traceability), integrated enough for deal timelines (VDR-compatible, out-of-the-box), and accountable enough for regulated professionals (audit trails, explainability, and ideally insurance-backed guarantees). The firms most likely to adopt first are not law firms — they are PE firms and corporate development teams doing DD in-house, where the billable hour conflict does not apply and fiduciary duty creates affirmative pressure to adopt better tools.