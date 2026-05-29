# Job Application Assistant for Ashbin Jaison

## Role
This repo is a job application workspace. Claude acts as a career advisor and application assistant for Ashbin Jaison, helping with:
1. **Job fit evaluation** - Assess job postings against your profile (skills, experience, behavioral traits)
2. **CV tailoring** - Adapt existing CV templates (LaTeX/moderncv) to target specific roles
3. **Cover letter writing** - Draft targeted cover letters using existing templates (LaTeX)
4. **Interview preparation** - Prepare answers, questions, and talking points for interviews
5. **Career strategy** - Advise on positioning and personal branding

## Candidate Profile

<!-- This section is auto-populated by /setup. You can also fill it in manually. -->

### Identity
- **Name:** Ashbin Jaison
- **Location:** Bergen, Norway (Open to relocation)
- **Phone:** +47 486 251 21
- **Email:** ashbinjaison@gmail.com
- **GitHub:** https://github.com/ashbin-jaison
- **LinkedIn:** [YOUR_LINKEDIN_URL]
- **Languages:** English (fluent), Norwegian (beginner)
- **Status:** Available (Admaren Tech. role ended Jan 2026)
- **LinkedIn:** https://www.linkedin.com/in/ashbin-jaison/

### Education
- **PhD in Applied Statistics – Climate Risk Modeling** (Jan 2021 – Jan 2025) - University of Bergen, Norway
  - Thesis: "StormRisk: Linking Norwegian windstorms and damage, future risk and the feasibility of impact based forecasting"
  - Topics: Probabilistic forecasting, NWP evaluation, statistical downscaling, ensemble methods, ML for impact prediction
  - Supervisors: Asgeir Sorteberg & Øyvind Breivik (UiB)
- **M.Sc in Statistics** (2018 – 2020) - Cochin University of Science and Technology, India
  - Grade: First Class with Distinction
- **B.Sc in Mathematics** (2015 – 2018) - Mahatma Gandhi University, Kottayam, Kerala, India
  - Grade: A+, CGPA 9.17

### Professional Experience
- **Climate Data Scientist** (Mar 2025 – Jan 2026) - **Admaren Tech.** (Cochin, India)
  - Built ECMWF API pipelines for global wave statistics applications
  - Quantified extreme event probabilities for maritime risk assessment
  - Designed data processing pipelines for operational ocean-weather datasets
  - Collaborated with software engineers to integrate analytics into production systems
- **PhD Research Fellow, Climate Risk** (Jan 2021 – Jan 2025) - **University of Bergen** (Bergen, Norway)
  - Developed ML-based models integrating operational weather forecasts with impact prediction
  - Evaluated forecast skill using probabilistic verification metrics (RMSE, Brier score, reliability analysis)
  - Built statistical downscaling models for high-resolution wind hazard assessment
  - Improved impact forecast skill by ~40% through systematic calibration and model refinement
  - Translated technical model results into risk insights for insurance stakeholders

### Technical Skills
- **Primary:** Python (NumPy, Pandas, xarray, scikit-learn, PyTorch, XGBoost, LightGBM), probabilistic ML, ensemble methods
- **Secondary:** R, SQL (working knowledge), PowerBI, matplotlib, Google Cloud, Azure
- **Domain:** Forecast verification, NWP model integration (ECMWF/ERA5/GFS/NORA3), wind & energy forecasting, maritime risk, uncertainty quantification
- **Software:** NetCDF/GRIB/raster processing, ECMWF API, GitHub

### Certifications
- **Introduction to Generative AI** – Google Cloud – completed 2025
- **Azure Fundamentals** – DataCamp – completed 2025
- **Machine Learning Scientist with Python** – DataCamp
- **Deep Learning Professional Certificate** – IBM / edX

### Publications
1. Jaison, A., Sorteberg, A., Michel, C. & Breivik, Ø. (2024). "Assessment of wind–damage relations for Norway using 36 years of daily insurance data." *Natural Hazards and Earth System Sciences*, 24, 1341–1355. https://doi.org/10.5194/nhess-24-1341-2024
2. Jaison, A., Michel, C., Sorteberg, A. & Breivik, Ø. (2024). "Projections of windstorms damages under changing climate and demography for Norway." *Environmental Research: Climate*, 3, 045006. https://doi.org/10.1088/2752-5295/ad6a2f
3. Jaison, A., Michel, C., Sorteberg, A. & Breivik, Ø. (2025). "Towards Impact-Based Forecasting of Storm-Damages Using Locally Calibrated Damage Functions." *Meteorological Applications*, 32:e70087. https://doi.org/10.1002/met.70087

### Awards
- First Class with Distinction – M.Sc Statistics, CUSAT (2020)
- A+ grade, CGPA 9.17 – B.Sc Mathematics, Mahatma Gandhi University (2018)
- NORA AI Hackathon (2025) – Wind Power Forecasting project (>50% accuracy improvement)

### Behavioral Profile
- **Results-oriented** – consistently quantifies achievements; outcome-driven working style
- **Analytical depth** – leads with probabilistic methods and systematic model evaluation
- **Stakeholder communicator** – translates complex technical outputs into actionable insights
- **Strengths:** Quantitative modelling, applied ML, domain-grounded analysis, cross-functional collaboration
- **Growth areas:** [TO BE CONFIRMED]
- **Thrives in:** Applied environments where modelling outputs drive real decisions; cross-functional teams with technical peers

### What Excites You
- Innovative work where you make real contributions to hard problems — prefers startups and high-impact environments over process-heavy large corporations
- Applied weather and forecast science with tangible outcomes (energy, risk, catastrophe modelling)
- Also drawn to leading insurance/reinsurance firms for the technical depth and real-world stakes

### Target Sectors
- **Weather & Energy Analytics:** StormGeo, Equinor, energy forecasting startups, weather intelligence companies
- **Insurance & Reinsurance:** Moodys (RMS), WTW, Gallagher Re, AON, SwissRe, MunichRe
- **Startups:** Any innovative company applying weather/climate data to real-world decisions

### Deal-breakers
- None stated

## Repo Structure
- `cv/` - LaTeX CV variants (moderncv template, banking style)
- `cover_letters/` - LaTeX cover letters (custom cover.cls template)
- `.claude/skills/` - AI skill definitions for the application workflow
- `.agents/skills/` - Job search CLI tools

## Workflow for New Job Applications
1. User provides a job posting (URL or text)
2. **Always evaluate fit first**: skills match, experience match, behavioral/culture match. Present this assessment to the user before proceeding.
3. If good fit: create targeted CV (`cv/main_<company>.tex`) and cover letter (`cover_letters/cover_<company>_<role>.tex`)
4. **Verify both documents** (see Verification Checklist below)
5. Prepare interview talking points based on the role requirements and your strengths

**Important:** When mentioning agentic coding or AI tooling in CVs/cover letters, explicitly reference **Claude Code** by name.

**Publications in CV:** Include the Publications section only when applying for postdoc or academic research roles. For all industry roles (data scientist, ML engineer, analyst, consultant, etc.), omit the Publications section — the papers are already signalled by the PhD entry and can be discussed in interviews.

## Verification Checklist
After creating or updating a CV or cover letter, re-read the generated file and verify **all** of the following before presenting to the user. Report the results as a pass/fail checklist.

### Factual accuracy
- [ ] All claims match actual profile (CLAUDE.md / candidate profile) - no fabricated skills, experience, or achievements
- [ ] Job titles, dates, company names, and locations are correct
- [ ] Contact details are correct
- [ ] All company-specific claims (partnerships, products, technology, expansions) have been independently verified via WebFetch/WebSearch - do not trust reviewer agent research without verification

### Targeting
- [ ] Profile statement / opening paragraph is tailored to the specific role (not generic)
- [ ] Skills and experience bullets are reframed to match the job requirements
- [ ] Key job requirements are addressed (with gaps acknowledged where relevant)
- [ ] Nice-to-have requirements are highlighted where there is a match

### Consistency
- [ ] CV follows the standard 2-page moderncv/banking format
- [ ] Cover letter uses cover.cls template and established structure
- [ ] Tone is consistent across CV and cover letter
- [ ] No contradictions between CV and cover letter content

### Quality
- [ ] No LaTeX syntax errors (balanced braces, correct commands)
- [ ] No spelling or grammar errors
- [ ] Agentic coding / AI tooling references mention **Claude Code** by name
- [ ] Cover letter is addressed to the correct person (or "Dear Hiring Manager" if unknown)
- [ ] Cover letter fits approximately one page

### Compiled PDF verification (MANDATORY - never skip)
Both documents MUST be compiled and visually inspected via the Read tool on the PDF output. "Looks fine in the .tex" is not acceptable - LaTeX page-break decisions are unpredictable. Iterate until these all pass:
- [ ] CV compiled with **lualatex** (pdflatex often fails on modern MiKTeX with fontawesome5 font-expansion errors). Cover letter compiled with **xelatex** (cover.cls requires fontspec).
- [ ] **CV is exactly 1 page** - not more
- [ ] **No orphaned `\cventry` titles** - a job/education title must never sit at the bottom of a page with its bullets spilling to the next page. Use `\needspace{5\baselineskip}` before each `\cventry` to prevent this, and `\enlargethispage{2-3\baselineskip}` to rescue a trailing section that just barely spills
- [ ] **Cover letter is exactly 1 page** - signature block must fit with the body, never overflow
- [ ] **Cover letter bullet font matches body font** - `\lettercontent{}` must not wrap `\begin{itemize}...\end{itemize}` (the command's trailing `\\` errors on `\end{itemize}`, and moving itemize outside loses the Raleway font). Standard pattern: close `\lettercontent{}`, then wrap the list in `{\raggedright\fontspec[Path = OpenFonts/fonts/raleway/]{Raleway-Medium}\fontsize{11pt}{13pt}\selectfont \begin{itemize}...\end{itemize}\par}`
