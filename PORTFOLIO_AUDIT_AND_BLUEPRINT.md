# Portfolio Audit & Professional Blueprint

**Repository audited:** `Risper-Nyawira/risper-nyawira-portfolio`  
**Default branch:** `main`  
**Audit date:** 6 November 2026  
**Purpose:** Upgrade the existing portfolio for broad agricultural research, data analytics and development opportunities.

## 1. Executive assessment

The portfolio has a credible and distinctive professional direction: agricultural economics, applied research, data analysis, agricultural markets, policy and sustainable food systems. It already has a custom website, a profile README, several analytical repositories, charts, project documentation and a separate ideas register.

The main weakness is not lack of subject matter. It is the uneven presentation of evidence. Some strong work is not visible on the homepage; some work is described only as experience; some projects overlap; and some claims need more precise status labels or stronger supporting outputs.

The upgrade should preserve the existing site and repositories while improving the evidence architecture, project case studies, navigation, technical proof and consistency of claims.

This audit is based on repository files and directory listings inspected on 6 November 2026. It is a source-level review, not a browser-based visual or accessibility test of the deployed website. Some linked binary files and private programme datasets have not been independently inspected.

## 2. Current portfolio assets

### Main portfolio repository

The root contains:
- `index.html` — single-page portfolio website.
- `styles.css` — custom responsive styling, including mobile breakpoints.
- `script.js` — mobile navigation toggle.
- `README.md` — professional profile, selected projects and skills.
- `IDEAS_BANK.md` — four innovation and enterprise concepts with explicit concept-stage disclaimers.
- Three homepage chart/dashboard image assets and a portrait image.
- `projects/sichei-soil-health-analysis/` — a documented exploratory soil and land-health analysis.

### Separate public GitHub repositories discovered

1. `kenya-agricultural-policy-impact-tracker`
2. `Tomato-value-chain-challenges`
3. `kenya-food-security-analysis`
4. `food-producing-communities-food-security`
5. `kenya-agricultural-market-intelligence.` (repository name currently ends with a period)
6. `Risper-Nyawira` (GitHub profile repository)

A private `agri-career-radar` repository also exists, but it is not part of the public agricultural research portfolio by default. Decide separately whether it should be shown as a software/product side project.

## 3. Project inventory and publication status

| Project / work | Evidence located | Recommended portfolio treatment |
|---|---|---|
| Kenya Agricultural Policy Impact Tracker (INT-01–INT-10) | Public repository, methodology, ten intervention summaries, limitations note and master Excel workbook | **Flagship case study.** Describe as ten preliminary evidence assessments, not ten completed impact evaluations. |
| Tomato Marketing Channels / Tomato Value Chain Challenges, Murang'a | Public repository contains proposal, project documents, correction document, presentation slides, SPSS output and Tobit results workbook | **Flagship field-research case study.** Explain the user's lead role, five-person team and approximately 200 farmer surveys. Verify final study title, objectives, statistical model, results and permissions before publishing detailed findings. |
| Kenya Agricultural Market Intelligence | Public repository contains analytical design, data-audit and pipeline scripts, SQL, SQLite database and findings documentation | **Flagship data case study.** First analytical slice is tomato wholesale prices. Explain source coverage and limits; do not imply local climate or production causality. |
| Kenya Food Security Analysis | Public repository contains structured folders, SQLite/SQL objects, Python notebook, Power BI file and output/documentation folders | **Flagship data case study.** Show end-to-end workflow, dashboard and conclusions; verify notebook reproducibility and source/indicator definitions. |
| Food-Producing Communities and Food Security in Kenya | Separate repository contains a Python notebook, processed data references, charts/tables and conclusion/data-inventory documents | **Consolidate with the Kenya Food Security work unless a distinct research question and dataset can be demonstrated.** The two projects currently overlap materially in maize production, climate/market context and food insecurity. Avoid presenting duplicate work as two unrelated flagship projects. |
| Sichei Soil Health: Land Use, Management Practices and Recorded Erosion | Portfolio subfolder includes README, Excel procedure, findings/limitations, selected data dictionary and citation notes | **Flagship exploratory research case study.** Current documentation describes 160 Sichei-only plot records and 131 fields. Present as descriptive analysis; only two records are positive in selected erosion indicators, so robust erosion-group inference is not supported. Confirm codebook definitions before stronger interpretation. |
| Kenya ASAL Sustainable Water and Soil Management evidence synthesis | A report draft exists in the user's project materials; structured evidence synthesis with preliminary findings and policy implications | **Research-in-progress case study.** Do not call it a completed systematic/scoping review: reproducible searching, deduplication, formal screening, PRISMA flow counts, full-text checks and final reference verification remain outstanding. |
| SNV CASHA Data Quality Assessment | A process record and cleaning log exist in project materials. Four sheets were reviewed: Participants, Activity Tracking, Attendants/Attendance and Other Value Chain Income. Work includes standardisation, cross-checking verifiable missing information, using 888 as a Value ID placeholder, structuring tables and filtering PivotTables to SNV. | **Applied MEAL/DQA case study after close-out verification.** The available record says final workbook validation, unresolved-gap review, file close-out and supervisor sign-off are not confirmed. Do not claim a fully signed-off DQA or a dataset with no missing values. Never publish confidential programme records. |
| Effects of Middlemen on Maize Farmers' Income, Ololulunga, Narok South | Listed on the current website and in CV material; detailed public repository/report not located in this audit | **Research experience now; standalone case study after outputs are located and verified.** Confirm sample, method, findings and the user's exact role. |
| Agricultural Finance and Smallholder Farmer Productivity | Research direction/protocol work exists in conversation history; no completed empirical dataset or results verified in this audit | **Proposal / research-in-progress.** Label it as a Kenya-focused mixed-methods proposal with African comparative evidence, not a completed study. |
| CASHA value-chain mapping and market analysis | Internship activities and familiarisation are documented in profile/context; no independent finished mapping deliverable verified here | **Experience and programme exposure**, not a separate completed project until a deliverable can be shown and approved for sharing. |
| SHEP market survey and agricultural enumeration | Field experience described in profile/CV material | **Experience highlights**, unless a distinct public research output is available. |

### Important project-status distinctions

- A complete workbook or tracker is not the same as a completed impact evaluation.
- A structured evidence synthesis draft is not a completed systematic/scoping review.
- Documented DQA actions are not the same as final data validation and supervisor sign-off.
- A proposal or concept is valid portfolio material when labelled accurately.
- The two food-security repositories should be reviewed for consolidation or clearly differentiated modules before both are promoted as separate flagship projects.

## 4. Professional positioning

### Recommended headline

**Agricultural Research & Data Analytics | Agricultural Economics | Policy & Market Systems | Sustainable Food Systems | MEAL**

### Recommended profile statement

Agricultural Economics and Rural Development graduate combining applied agricultural research, farmer-level field experience, data management and analytical work, and development-programme exposure. Interested in turning agricultural, market and programme evidence into practical insights for stronger farmer livelihoods, more effective development interventions and sustainable food systems.

### Target opportunity families

- Agricultural research and research assistant roles
- Agricultural data and market intelligence roles
- Agricultural economics and policy research
- Value-chain and market systems research
- Food security and rural development analysis
- MEAL, programme data quality and learning support
- Sustainable agriculture and climate-resilience research

This broad positioning should have one central identity—agricultural research and data analytics—rather than presenting unrelated job titles as equal specialisms.

## 5. Skills architecture and evidence rules

| Skill group | Skills to show | Evidence / proficiency treatment |
|---|---|---|
| Agricultural economics and sector knowledge | Agricultural markets, production economics, value chains, food security, rural livelihoods, agricultural policy | Ground in degree, research and documented project work. |
| Research and fieldwork | Literature/desk review, structured farmer surveys, questionnaire administration, field data collection, research coordination, descriptive analysis, research writing | Show actual roles and outputs; distinguish leading, supporting and participating. |
| Data management and quality | Excel, Google Sheets, data cleaning, standardisation, cross-checking, DQA, cleaning logs, KoboToolbox/KoboCollect | Excel: intermediate as stated. Kobo: describe workflow familiarity. Do not claim full MEAL system ownership. |
| Data analysis and visualisation | SQL, SQLite, Python, pandas, Matplotlib, Power BI | Demonstrate with code, notebooks, queries, dashboard and outputs. Use working/developing labels where independent proficiency is still growing. |
| Programme and development practice | MEAL foundations, participant/activity tracking, GESI/YEE awareness, programme reporting, value-chain mapping exposure | Attribute to SNV/CASHA internship and training; avoid implying independent programme leadership. |
| Sustainable agriculture | Soil/land health, agroforestry, regenerative agriculture, climate adaptation, circular bioeconomy | Distinguish subject interests, learning and concepts from implementation experience. |
| Developing areas | GIS/QGIS, spatial analysis, advanced Python/SQL, advanced Power BI | Place under current learning, not established core skills until demonstrated. |

Every skill shown prominently should link to at least one project, work example, certificate or verifiable output. Avoid unsupported proficiency labels.

## 6. Website audit: strengths and gaps

### Strengths to preserve

- Distinctive visual identity and strong headline: “Better agricultural decisions through better evidence.”
- Clear interdisciplinary connection between agriculture, economics, research, data, markets and development.
- Custom CSS and mobile breakpoints are already present.
- Existing chart images make the work more tangible than a text-only profile.
- Research/field experience is visible, not hidden behind technical projects.
- The ideas register explicitly distinguishes concepts from implemented or validated work.

### Priority improvements

1. **Make the first screen more recruiter-oriented.** Add a precise role headline, concise value proposition, core capabilities and clear actions to view projects, download a CV and contact.
2. **Feature the strongest evidence.** Add policy tracking, tomato field research and Sichei soil-health work; promote CASHA DQA after validation.
3. **Resolve food-security overlap.** Consolidate or distinguish the two repositories and their analytical questions.
4. **Improve project navigation.** Add filters such as Research, Data Analytics, Policy & MEAL, Sustainable Agriculture, and Research in Progress.
5. **Create dedicated case-study pages.** Homepage cards should lead to pages with question, role, data, methods, findings, interpretation, limitations, outputs and links.
6. **Make outputs easy to inspect.** Add executive summaries, selected charts, dashboard previews, reproducible notebooks/queries and reports where permitted.
7. **Make skills evidence-led.** Use proficiency/status labels and connect skills to examples.
8. **Clarify experience versus projects.** Tomato research may appear as both a case study and a role, but the wording should not double-count the same work as two separate projects.
9. **Improve professional learning presentation.** List exact course/certificate names and providers only after checking the credential; separate completed certificates from training and informal learning.
10. **Add accessibility and metadata checks.** Include a skip link, visible keyboard focus, meaningful heading order, descriptive image alt text, reduced-motion support where needed, page title/description and social-sharing metadata. Test deployed mobile behaviour and all links.
11. **Review public contact details.** Keep professional email and LinkedIn easy to find; decide whether a personal phone number should remain public.
12. **Fix repository naming and links.** The market-intelligence repository name currently ends in a period. Rename it to a clean slug if the user approves; update every website and README link afterward.

### Existing homepage claims to tighten

- “200+ farmers reached through lead research” should be revised to the more precise “approximately 200 farmers surveyed” if the underlying study records confirm this.
- “3 data and research projects documented” does not match the four projects in the README and three project cards on the homepage. Replace with a defined count or remove the metric.
- “Power BI Data Analyst” may be read as a formal professional certification. Use the exact verified course/training title instead.
- GIS/QGIS, spatial analysis, precision agriculture and AI applications should remain in a clearly labelled learning/developing area unless supported by demonstrated work.
- Do not publish causal claims from descriptive food-security, market-price or soil-health analysis.

## 7. Recommended flagship project set

Build six to eight substantial project pages, not a large gallery of shallow entries.

### Tier 1 — flagship case studies

1. **Kenya Agricultural Policy Impact Tracker:** ten intervention-level preliminary evidence assessments; evidence hierarchy, 18-step framework, workbook and limitations.
2. **Tomato Marketing Channels and Value-Chain Research:** primary farmer research, team coordination, research design, SPSS/Tobit outputs and practical market insights, subject to final-output verification.
3. **Kenya Agricultural Market Intelligence:** data audit, SQL/SQLite, Python pipeline, tomato market price panel, market comparisons and limitations.
4. **Kenya Food Security Analysis:** consolidated food-security project with a clear distinction between the overall analytical workflow and the food-producing communities question.
5. **Sichei Soil Health and Land-Use Analysis:** 160-record Sichei subset, data dictionary, Excel workflow, descriptive findings and limitations.
6. **SNV CASHA DQA:** applied programme-data quality case study, pending validation and supervisor close-out.

### Tier 2 — supporting research and development work

7. **Sustainable Water and Soil Management in Kenya's ASALs:** structured evidence synthesis in progress; upgrade to a completed review only after the protocol and screening workflow are completed.
8. **Middlemen and Maize Farmer Income Research:** promote after source files, methods and findings are verified.
9. **Agricultural Finance and Farmer Productivity:** publish as a proposal/protocol until primary data collection and analysis occur.

### Separate innovation and concepts section

Keep `IDEAS_BANK.md` and create a concise innovation section for:
- RegeneraSense — concept development; pitch deck prepared.
- Afya Verified — integrated farmer services/platform concept.
- Kabukuru Farm — integrated regenerative farm concept.
- Limuru Herbs and Spices Farm — early feasibility/planning concept.

Do not present these as operational businesses, implemented platforms or validated pilots.

## 8. Standard case-study template

Every flagship project page should use the same structure:

1. Project title, status and date
2. Executive summary (3–5 sentences)
3. Research/problem statement
4. Objectives and research questions
5. User's role and exact contribution
6. Data sources, coverage, sample and permissions
7. Methods and analytical workflow
8. Results with labelled charts/tables
9. Interpretation and practical implications
10. Limitations, uncertainty and evidence gaps
11. Reproducibility: code, workbook, database or notebook
12. Downloadable report / executive brief, where appropriate
13. References, data attribution and confidentiality note

A case study is not ready for flagship placement until its claims, sources, methods, outputs and limitations have been checked.

## 9. Proposed website information architecture

- **Home:** professional headline, concise summary, proof points, featured case studies, CV/contact actions.
- **About:** education, professional narrative and research interests.
- **Skills:** grouped capabilities with proficiency/status and evidence links.
- **Portfolio:** filterable project collection.
- **Case studies:** dedicated project pages.
- **Research & writing:** reports, policy briefs, protocols and public articles.
- **Experience:** SNV CASHA, tomato research leadership, Fair Trade Enterprise, CloudFactory and other verified roles.
- **Learning:** certificates and professional development with exact names.
- **Innovation:** concept-stage projects clearly labelled.
- **Contact:** email, LinkedIn and optional phone.

## 10. Execution roadmap

### Phase 1 — evidence and content audit
- Verify the final outputs for each flagship project.
- Reconcile project titles, dates, roles, samples, findings and tools.
- Resolve food-security project overlap.
- Confirm DQA close-out and safe public disclosure.
- Verify certificates and exact skill levels.

### Phase 2 — project case studies
- Develop the policy tracker and tomato research case studies first.
- Complete market intelligence and food-security case studies.
- Strengthen Sichei documentation and charts.
- Add DQA only after final validation and approval for a sanitised public example.

### Phase 3 — website redesign
- Retain the current brand identity, but simplify the homepage.
- Add a filterable portfolio, case-study pages and clear recruiter actions.
- Improve accessibility, mobile usability, SEO and metadata.
- Add project status labels and downloadable outputs.

### Phase 4 — quality assurance
- Test all links, mobile layouts, images and downloads.
- Re-run project calculations and notebook workflows where feasible.
- Verify all displayed numbers against their source outputs.
- Review privacy, licensing, attribution and confidentiality.
- Ensure the profile README, website and CV tell the same professional story.

## 11. Definition of a portfolio-ready project

A project is flagship-ready only when:
- The project question and purpose are clear.
- The user's contribution is specific and defensible.
- Sources, sample and coverage are documented.
- Methods can be explained and, where possible, reproduced.
- Findings are checked against the underlying output.
- Limitations and uncertainty are explicit.
- A recruiter can inspect a useful output without needing private access.
- Confidentiality, licensing and attribution requirements are respected.

## 12. Immediate next actions

1. Build the final evidence matrix from the actual reports, notebooks, workbooks and presentations.
2. Prioritise the policy tracker and tomato research as the first two full case studies.
3. Consolidate the food-security projects and define one clear project architecture.
4. Complete DQA close-out checks before publicising the work as a completed quality-assurance exercise.
5. Prepare a new homepage and case-study design only after the evidence and project statuses are settled.

**Guiding principle:** present the strongest real evidence, explain it clearly, and never inflate a skill, result, role or project status.
