# 03_Tailored_Applications - CV & Cover Letter Customization Module

## Purpose
Generate highly tailored CVs and short cover letters for the Top 3 selected jobs, based on the Master CV and all previous analysis.

## Input
- `../00_Input/Master_CV.md` (the master version)
- `../02_Top_Selection/Top_3_Jobs.md`
- Job scoring and analysis files from `../01_Job_Scoring/`

## Output Structure
Create one subfolder per job inside `03_Tailored_Applications/`:
03_Tailored_Applications/
├── Job_001_[Company][Role]/
│   ├── CV_Tailored_Job_001_v1.md
│   ├── CoverLetter_Job_001_v1.md
│   └── Tailoring_Notes.md
├── Job_002[Company][Role]/
├── Job_003[Company]_[Role]/
└── CONTEXT.md
text## Detailed Instructions

### 1. Cover Letter (CoverLetter_[Slug]_v1.md)
- Maximum **half page** (250–350 words)
- Structure:
  - Strong opening paragraph linking your background to the specific role
  - 2–3 strong, quantified achievements tailored to the job requirements
  - Why this company/role excites you
  - Forward-looking close with clear interest
- Use keywords and phrasing from the job description naturally
- Keep it concise and do not use too many paragraphs and only one section with bullet points if at all.

### 2. Tailored CV (CV_Tailored_[Slug]_v1.md)
- Start from `../00_Input/Master_CV.md`
- Reorder bullet points to prioritize the most relevant experience first
- Strengthen or rewrite bullets to better match the job
- Emphasize technical achievements, independence, and impact
- Remove or de-emphasize less relevant content
- Keep total length reasonable (ideally 1.5–2 pages)

### 3. Tailoring_Notes.md
- List key changes made to the CV
- Main themes emphasized in the cover letter
- Strategic decisions and rationale

## Quality Standards
- Every document must feel **specifically written** for that job
- Strong alignment between your highlighted experience and the job requirements
- Professional, confident, and results-oriented tone
- Quantify achievements wherever possible
- Maintain consistency between CV and Cover Letter

## Execution Guidelines
1. Analyze the Top 3 jobs thoroughly using previous scoring
2. Create the three subfolders
3. Generate high-quality tailored CV + Cover Letter for each
4. Create Tailoring_Notes.md for each job
5. After completion, summarize what was created
   
Wait for further human instructions. Do not continue on your own with the next step.