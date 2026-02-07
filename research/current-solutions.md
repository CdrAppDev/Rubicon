# AI due diligence tools are improving fast, but fundamental workflow gaps persist

**All six problem hypotheses find strong evidentiary support.** The current solutions landscape reveals that due diligence technology — from virtual data rooms to AI contract review — remains anchored in a paradigm of secure document storage rather than intelligent analysis. Despite billions invested in VDR infrastructure and a surge of AI-powered tools, practitioners still rely on Excel spreadsheets, email threads, and manual cross-referencing to perform the analytical core of due diligence. The deepest root cause beneath most of the hypothesized problems is that **VDRs were designed as secure repositories, not analytical platforms**, and AI tools have been layered on top without solving the underlying workflow fragmentation. This report documents the specific failure points, user complaints, and gaps across six categories of tools — with verbatim evidence from practitioners and review platforms.

---

## H1 is strongly validated: manual review under tight timelines remains the norm

The evidence overwhelmingly confirms that due diligence teams face an impossible throughput challenge. Deals closing in the first half of 2024 lasted **258 days on average — 32% longer than in 2020** — while document volumes continue to grow. Harvey AI's own blog describes the "familiar pain points: hundreds or thousands of agreements, inconsistent document sets, and a tight deadline. Associates spend hours combing through contracts to find key clauses, and then manually copy them into a spreadsheet or chart." Jurimesh puts it more bluntly: "Your junior associates spend days just figuring out what's in the data room. They're opening files, renaming documents, and building basic indexes before any real review can begin."

The result is systematic under-review. Traditional due diligence examines only **5–10% of the contract population** in a transaction involving 10,000+ active contracts, "missing material obligations and exposures by design," according to Sirion.ai. Thomson Reuters estimates AI can reduce document review time by up to 70%, which implicitly quantifies how much time is currently wasted. McKinsey reports that early AI adopters "spend only about one day summarizing the data, instead of one week" — yet **70% of M&A practitioners are not meaningfully using AI** in their deals, per McKinsey's own survey. Bain's latest data shows AI adoption in M&A roughly doubled to 45% of practitioners in 2025, up from 21% the prior year, but the majority still operate manually.

Multiple Datasite user reviews confirm the experience at the tool level. One G2 reviewer noted that "document review speed can be slow due to one-by-one file access, and search accuracy sometimes misses relevant text." Another requested "a more streamlined, preview-friendly interface [to] make it much easier to quickly scan and prioritize key files during due diligence." An Intralinks user on Capterra wrote that "managing Intralinks became a full-time job. Training others on how to use Intralinks took up so much time — again, this time should have been used for completing the due diligence process."

- **Verdict on H1:** Root problem, not symptom. The volume-timeline mismatch is structural.
- **Relevant data:** 66% of M&A practitioners say DD is the single most important success factor, yet 48% believe it could be most enhanced by technology (Datasite survey).

---

## H2 finds strong support: cross-referencing failures let anomalies slip through

The inability to systematically cross-reference information across large document sets is not merely hypothetical — it has produced documented deal failures. When Marriott acquired Starwood, it failed to detect a massive data breach affecting millions of customer records, including passport numbers, during due diligence. Verizon's more careful technology DD of Yahoo discovered that all three billion email accounts had been hacked, **saving $350 million** on the purchase price. These are the high-profile cases; the routine misses go unreported. As DealRoom notes, "Look for due diligence failures in the literature and the same 10 to 15 deals are mentioned over and over... nobody wants to admit their due diligence failure."

The scale of the sampling problem is striking. Academic research published in MDPI found that auditors pick "less than one percent of total" accounting data for manual assessment, "creating a sampling risk when financial misstatements dissolve in a much bigger non-sampled data group." McKinsey reports that AI-driven pattern recognition can reduce credit losses by **20–40%** by detecting "subtle, high-risk anomalies that manual reviews often miss" — a figure that quantifies the detection gap in current practice. V7 Labs describes how "AI noticing that the sales figures mentioned in the CEO's presentation don't match the numbers in the financial statements" represents cross-document analysis that "was practically impossible to do at scale manually."

Most current AI tools, however, analyze documents individually rather than across related documents. Gavel.io's review of AI contract tools found that "M&A review isn't single-document... Disclosure Schedules vs. the main APA... Most AI tools do not consider cross-document dependencies." Evisort's own documentation acknowledges that "AI cannot span interrelated contracts, and results are not 100% automatic." This gap means that even teams using AI still miss relationship-level signals.

- **Verdict on H2:** Root problem. Even AI tools haven't fully solved cross-document analysis.
- **Unanticipated finding:** The problem is compounded by OCR quality. Best OCR achieves only 98–99% accuracy, meaning **200+ errors per 10,000 characters** — and scanned, handwritten, or watermarked documents perform far worse.

---

## H3 is validated at every level of the tool stack: search remains primitive

Datasite's own survey captured the problem precisely: "Trying to locate a specific piece of information among all those documents is very difficult and time consuming, requiring Buyers to read through pages and pages to get the data they need." This isn't a marginal inconvenience — **65% of survey respondents** said new technologies should enable greater analytical capability in the DD process.

Current VDR search is limited to keyword matching. As one analysis noted, teams are "using basic search methods like Ctrl+F to look for specific terms, which frequently miss synonyms and the meaning of the phrases." Firmex was specifically criticized for offering "no search by filters and labels, which makes finding specific documents time-consuming and inefficient." A Firmex user complained that "the tree structure of the files could be better... it is also difficult to understand where in the folders structure are located files found by searching." Datasite users wished they could "search by Doc IDs/location numbers in addition to just searching for document contents or titles."

Datasite and Ansarada have begun adding AI-powered search features — Datasite offers "Summarize" and "Explain This" generative AI features, while Ansarada offers an AI Intelligent Data Assistant. But these are nascent additions to platforms built around secure storage, not analytical intelligence. The most advanced search capabilities come from standalone AI tools like AlphaSense (which offers Smart Synonyms™ and generative search across 500M+ premium documents) but AlphaSense is designed for market intelligence research, not data room document analysis. Its users still complain that "even though they have query expansion, their search quality still sucks."

The gap is clearest in Jurimesh's description of what AI-enabled search can do but VDRs currently cannot: "The system detects cross-references between documents. If board meeting minutes mention a 'Management Incentive Plan' but that plan isn't in the data room, you'll get an alert. What used to require careful human cross-checking across thousands of files happens automatically." No major VDR offers this capability natively.

- **Verdict on H3:** Symptom of the deeper problem that VDRs are storage tools, not analytical platforms. Solving search alone is insufficient without cross-document intelligence.

---

## H4's fragmentation problem runs deeper than expected: it is the default operating model

The evidence suggests that workflow fragmentation isn't a failure mode — it's the standard operating procedure. **60% of executives say deals fail due to poor due diligence**, with communication silos identified as a primary cause: "Due diligence teams risk not cooperating enough to see the whole picture. Due to poor communication, DD professionals may miss critical interdependencies between findings."

The fragmentation is both inter-team and inter-tool. Spellbook's analysis found that "most due diligence contract work does not happen in a data room or CLM dashboard. It occurs in Word, line by line, before any contract is escalated, priced, or signed." CENTRL documented how "in most due diligence workflows, email adversely affects productivity and efficiency. Often due diligence professionals must chase investment managers through numerous emails and track responses... they must also check and re-check the accuracy and validity of information by looking at multiple Excel spreadsheets, Word documents, and PDF files." Datasite explicitly acknowledges the persistence of this problem: "Generally, this request list takes the form of an Excel spreadsheet, sent by email. When the seller uploads files from the list, the advisor manually updates the checklist. It's a laborious process. And ripe for errors."

A telling complaint from a Datasite reviewer reveals a gap no VDR has closed: "Allocation of documents could be possible within the tool. For example, I should be able to mark the documents I intend to / have reviewed. It should be possible to both allocate and see who has been allocated documents on the site." No major VDR was found to offer robust document assignment and review tracking within the platform itself. Teams build parallel tracking systems in Excel, creating the version confusion and duplication the VDR was supposed to eliminate.

Q&A workflows — the "central nervous system of the due diligence process" — have their own critical gaps. A Datasite user reported that linking Q&A questions to specific files "was all manual (e.g., writing out where a file is located)." An Ansarada user described having to "make a fake account on behalf of a 3rd party to process questions" because the platform didn't support asking on behalf of external parties.

- **Verdict on H4:** Root problem, and arguably the deepest structural issue. The entire DD tool ecosystem is built around individual tools (VDR for storage, Excel for tracking, email for communication, Word for analysis) with no integrated workflow layer.

---

## H5 is validated with vivid specificity: the "ingestion gap" defines portfolio monitoring

Portfolio monitoring tools face a problem so fundamental that V7 Labs calls it "the dirty secret of the asset management industry": despite billions spent on portfolio management systems, "the industry's backbone remains a fragile mesh of spreadsheet workbooks." The reason is what V7 Labs terms the **"ingestion gap"** — private market data arrives as unstructured PDFs, slide decks, emails, and spreadsheets in wildly different formats, and "highly paid analysts, trained to value assets and structure deals, spend an estimated **40–60% of their time acting as data entry clerks**, re-keying numbers from PDFs into the PMS."

The consequence is severe data lag. "Because ingestion is manual, the data in the PMS is often **30–45 days old** by the time it is reconciled. Investment committees are forced to make real-time decisions based on last quarter's numbers." BDO's 2025 Private Equity Survey found that "many fund managers lack real-time oversight of their portcos, primarily relying on quarterly reports and meetings" — and that 84% report longer holding periods, intensifying the monitoring burden. A VC analyst quoted by PortfolioIQ described the reality: "The way we do our portfolio review one-pagers is mostly last-minute. We're like looking at two different screens, one of the PDF of the board deck, and then we're plugging in the numbers manually... it is cumbersome."

Every major portfolio monitoring tool — Visible, Carta, Chronograph, eFront, Cobalt, iLevel, Addepar — operates on a fundamentally **periodic** data collection model. Even the most advanced (Chronograph's Chrono AI, eFront's ML automation) improve the speed of processing quarterly data but don't change the underlying cadence. None provide continuous monitoring of external signals — news, litigation, regulatory actions, executive departures — that could indicate portfolio company distress between reporting periods. A Cobalt client captured the pain of the status quo: "We've been held hostage by our own data due to an over-reliance on spreadsheets and maintaining disparate databases."

Data collection also depends on voluntary compliance from portfolio companies. Visible reports that "investors struggle to monitor their portfolio companies effectively because if they hear from companies at all, it's in a format that is unstructured and in a frequency that is unpredictable." The result is that VCs burn an estimated **500+ hours yearly** just collecting and cleaning data.

- **Verdict on H5:** Root problem. The periodic reporting model is structural, not fixable by better tools alone. The deeper issue is that portfolio monitoring tools were built to organize data that arrives on schedule — they have no mechanism for continuous intelligence.

---

## H6 is supported but the burden may be more systemic than founder-specific

Evidence confirms that DD preparation is painful for founders. DocSend's own blog quotes a founder experience: "Most would rather give birth, have to run into a burning building to save a kitten, or have all of their teeth pulled. At least the pain would be over much faster." The process takes **2–8 weeks minimum** and can extend to months if documentation is disorganized. Sophia Parvizi-Wayne, founder of Kanjo, warned that DD "will take way longer than you think" and cautioned founders to "be aware when people are dragging you around in circles, because it will mess up your round."

The tool landscape for startup DD preparation is fragmented across a cost-capability spectrum. Google Drive is free but offers no analytics, no watermarking, and no audit trails. DocSend (Dropbox) provides engagement tracking but lacks Q&A functionality, redaction tools, and document-level permissions — and users report a "confusing UI" that "did not significantly change in the last 10 years." Notion is gaining traction for data rooms (endorsed by VCs like Eniac Ventures) but lacks engagement analytics, granular security, and audit trails. Proper VDRs cost $150–500+/month, and startups often can't justify the expense pre-revenue.

The core pain, however, may be less about tools and more about the fundamental asymmetry of the DD process. Dr. Anas Nader, CEO of Patchwork Health, "appointed an existing member of the team as a project manager who was in charge of preparing the data room" for his Series B — effectively dedicating a full headcount to the process. Westaway Law recommends founders "choose a single person to lead the due diligence process" and "make due diligence their primary job during the process." Capbase warns that "you may find yourself paying lawyers to gather and organize documents" if records weren't maintained.

- **Verdict on H6:** Supported, but this may be a less acute market opportunity than H1–H5. The pain is real but episodic (fundraising rounds), and simpler solutions (templates, better record-keeping habits, lower-cost VDRs like Papermark or Carta's free data rooms) may adequately address it. The larger structural problems in H1–H4 affect high-frequency, high-value professional workflows.

---

## Where existing AI tools actually fail: the gap between demos and reality

The AI due diligence tool market includes several established players — **Kira Systems** (Litera), **Luminance**, **Evisort** (Workday), **DiligenceVault**, **Daloopa**, and **AlphaSense** — plus newer entrants like Dili (YC-backed), Zuva (Kira spinout), LEGALFLY, Gavel Exec, Imprima AI, and DealRoom AI. Their capabilities are real but narrower than marketing suggests.

**Kira Systems** offers 1,400+ pre-trained smart fields and claims 50% time savings in contract review. But users report that accuracy "has not been good enough to trust 90+%, which means that it is currently just a review aide and still costs lawyer time." Training new provisions is "extremely time consuming," and Kira "is less helpful when the diligence is composed of many different types of agreements, none of which are similar."

**Luminance** claims to process 3,600 documents per hour versus 79 manually, but an independent Nevada State Bar review rated its usability **1.5 out of 5**, citing "big problems with fitting it into existing workflows and the constant need for manual tagging." Users report that "it looks amazing in the sales demo but struggles with the messy reality of their own documents."

**Evisort** (now Workday Contract Intelligence) was rated a Gartner "Visionary" and processes up to 450,000 contracts daily, but users flag that it "struggles with low-quality PDFs and has limited OCR capabilities" and that "AI cannot span interrelated contracts." One G2 reviewer warned that "the pre-implementation sales team is more focused on selling the software than understanding the problems potential clients are trying to solve."

**AlphaSense** is the highest-rated tool (G2: 4.6/5, TrustRadius: 9.5/10) but serves market intelligence rather than data room analysis. Users still complain it is "cost prohibitive" and that "there is a lot of repetition in the data it picks up, making it tedious for the research team."

A law firm article from Koley Jessen documented a specific AI failure: "The summary flagged the contract as low-risk, but it missed a critical change-of-control clause requiring supplier consent for M&A. The AI's training data lacked examples of such non-standard provisions." This exemplifies the central limitation: AI tools trained on standard templates miss the unusual provisions that matter most in DD. They summarize but they don't interpret.

- **Adoption remains low:** Only **3% of small and mid-sized firms** actively use AI for due diligence, versus 29% of large firms.
- **Pricing is universally opaque:** Kira, Luminance, Evisort, DiligenceVault, Daloopa, and AlphaSense all require sales conversations for pricing, creating barriers to comparison and adoption.

---

## Three findings that no hypothesis anticipated

**First, the "lifecycle gap" is the deepest structural problem.** No single tool covers the full due diligence lifecycle — document ingestion, contract analysis, financial modeling, cross-document risk synthesis, collaboration, and deal memo generation. Teams currently stitch together 4–6 disconnected tools (VDR + Excel + email + Word + PDF reader + sometimes an AI tool), and the seams between tools are where errors, inconsistencies, and blind spots accumulate. This isn't captured by any individual hypothesis but underlies H1, H3, and H4 simultaneously.

**Second, Q&A workflows are a hidden bottleneck that none of the hypotheses address.** The Q&A module in VDRs is described as "the central nervous system of the due diligence process," yet it has critical gaps: inability to link questions to specific documents (Datasite), inability to ask questions on behalf of third parties (Ansarada), confusing question ordering with bulk uploads, and limited team-based routing. These gaps force workarounds that slow deals and create confusion.

**Third, the demo-to-reality gap in AI tools suggests the market is ripe for disruption but also ripe for disappointment.** Luminance's 1.5/5 usability score from an independent bar review, Kira's admission that accuracy isn't trustworthy enough for automation, and Evisort's overselling during pre-sales all point to a pattern where AI tools overpromise and underdeliver in production. The winning solution will need to manage expectations carefully while delivering reliability on messy, real-world documents — not just clean demo data.

---

## Conclusion: what a winning solution would need to address

The evidence validates all six hypotheses with varying degrees of strength. H1 through H5 represent deep, structural problems that current tools fail to solve. H6 is real but may be addressable with lighter solutions. The most important insight cutting across all findings is that **the due diligence technology stack was designed for document security, not document intelligence** — and layering AI features onto storage platforms hasn't bridged the gap.

The competitive white space for Rubicon (or any challenger) sits at the intersection of three unmet needs: cross-document analytical intelligence (not just single-document extraction), integrated workflow that eliminates the Excel-email-VDR fragmentation, and continuous portfolio monitoring that breaks the quarterly reporting cycle. Current leaders like Datasite and Intralinks are adding AI features incrementally, but their architecture is fundamentally storage-first. AI-native tools like Kira and Luminance are powerful but narrow — focused on contract clause extraction rather than holistic deal analysis.

The strongest competitive signal is that **70% of M&A practitioners still don't meaningfully use AI**, yet those who do report 20–50% improvements in speed and cost. The gap between potential and adoption suggests the market is waiting not for better AI models but for better-integrated, more reliable, and more transparent products that work on messy real-world documents without requiring extensive training or configuration. The team that closes the demo-to-reality gap while spanning the full DD lifecycle will capture significant value.