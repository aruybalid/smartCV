# 01_Job_Scoring - Job Analysis & Scoring Module

## Purpose
This module analyzes all job descriptions against the information in the master CV (`Master_CV.md`), as well as the information in `job_preferences.md` and `work_experiences.md`, all located in the `../00_input` folder, to produce objective match scores and identify the strongest opportunities.

## Process

### Input
- Job description files from `../00_Input/Job_Descriptions/`
- Master CV files for skills/requirements matching
- job preferences in `../00_Input/job_preferences.md`
- work experiences in `../00_Input/work_experiences.md`

### Output
1. `All_Jobs_Scoring_Report.md` - Consolidated ranked report
2. Individual score files in `Individual_Job_Scores/` - Detailed per-job analysis

## Scoring Criteria (Recommended Weights)
- **Skills Match (40%)**: Technical skills, tools, languages alignment
- **Experience Level (25%)**: Years required vs. your experience
- **Role Responsibilities (20%)**: Day-to-day duties alignment
- **Company/Industry Fit (10%)**: Sector, culture, values alignment
- **Location/Remote (5%)**: Work arrangement preferences

## Instructions
1. Process each job description individually
2. Generate detailed score file for each job first
3. Aggregate results into the master scoring report
4. Rank jobs from highest to lowest overall match score
5. Highlight key strengths and gaps for each opportunity

## File Organization
- Keep individual score files named consistently: `Company_Role_Score.md`
- Update the master report after processing new batches
- Archive old reports in `../04_Archive/` when refreshing

## Quality Checks
- Verify all jobs from input folder are represented
- Ensure scores are consistent and defensible
- Cross-reference with master CV to avoid inflated scores
- Cross-reference with `../00_Input/job_preferences.md` and `../00_Input/work_experiences.md`

---
*Module Version: 1.0 | Scoring Framework: Skills-First Approach*