# 04_Archive - Archiving Framework

## Overview

The 04_Archive directory maintains a historical record of all job application pipeline cycles. Each cycle captures a complete snapshot of the pipeline state at the time of archiving, enabling cross-referencing, learning from past decisions, and tracking application outcomes.

## Cycle Structure

### Cycle Folder Naming Convention
- `Cycle_01/`, `Cycle_02/`, `Cycle_03/`, etc.
- Each cycle represents one complete pipeline execution from scoring through tailored applications

### Cycle Folder Contents

Each Cycle_XX folder mirrors the main pipeline structure:

```
Cycle_XX/
├── 01_Job_Scoring/
│   ├── All_Jobs_Scoring_Report.md
│   ├── CONTEXT.md
│   └── Individual_Job_Scores/
│       └── *.md (all individual job scores)
├── 02_Top_Selection/
│   ├── CONTEXT.md
│   └── Top_3_Jobs.md
├── 03_Tailored_Applications/
│   ├── CONTEXT.md
│   ├── Job_XXX_Company_Role/
│   │   ├── CV_Tailored_Job_XXX_v1.md
│   │   ├── CoverLetter_Job_XXX_v1.md
│   │   └── Tailoring_Notes.md
│   └── ...
└── 04_Archive/
    └── Cycle_XX_Application_Tracking.md (generated during archive)
```

## Archiving Process

### Step 1: Initiate Archive
When the pipeline has completed tailored applications for selected jobs, initiate the archiving process by creating a new cycle folder.

### Step 2: Copy Pipeline State
Copy the complete current state of stages 01-04 into the new cycle folder:
- All scoring reports and individual job scores
- Top selection decisions and rationale
- All tailored application materials
- All CONTEXT.md files from each stage

### Step 3: Application Tracking (Critical Step)

**Before finalizing the archive, the following question must be asked to the user:**

---

### APPLICATION STATUS QUESTION

**Which of the following jobs have you submitted applications for?**

Please indicate for each tailored application folder whether an application has been submitted:

**Tailored Applications in this cycle:**
- [ ] Job_001_Oklo_Materials_Engineer - Application submitted? (Yes/No) | Date: ________ | Method: ________
- [ ] Job_002_Oklo_Design_Engineer - Application submitted? (Yes/No) | Date: ________ | Method: ________
- [ ] Job_003_Kairos_Power_Plant_Operations_Engineer - Application submitted? (Yes/No) | Date: ________ | Method: ________
- [ ] Job_004_RandWorldwide_AnsysSupportEngineer - Application submitted? (Yes/No) | Date: ________ | Method: ________
- [ ] (Additional jobs as applicable)

**Notes on Application Outcomes:**
- [Add any relevant notes about application status, interview invitations, rejections, etc.]

---

### Step 4: Generate Application Tracking Record

Create a file: `Cycle_XX/Cycle_XX_Application_Tracking.md` (at cycle root level)

This file records:
- Date of archive creation
- List of all jobs scored in this cycle
- Top 3 selections with scores
- Application submission status for each tailored application
- Any notes on outcomes or follow-up actions
- **Deletion Confirmation Question** - User confirmation before original content deletion

### Step 5: Deletion Confirmation (Critical Step)

**Before deleting generated results, the user must answer:**

1. "Have you reviewed the archived content in `04_Archive/Cycle_XX/`?"
2. "Are you satisfied that the archive contains all necessary information?"
3. "Do you understand that we will only delete generated results (not CONTEXT.md files, folder structure, Master_CV files, job_preferences.md, or work_experiences.md) from 00_Input/, 01_Job_Scoring/, 02_Top_Selection/, and 03_Tailored_Applications/?"
4. "Do you give permission to delete the generated results?"

**What Gets Deleted (Generated Results Only):**
- `00_Input/Job_Descriptions/` - All job description files (keep folder structure)
- `01_Job_Scoring/All_Jobs_Scoring_Report.md` and `01_Job_Scoring/Individual_Job_Scores/` - All scoring files (keep CONTEXT.md)
- `02_Top_Selection/Top_3_Jobs.md` - Selection decisions (keep CONTEXT.md)
- `03_Tailored_Applications/` - All Job_XXX folders and contents (keep CONTEXT.md)

**What Stays (Framework Infrastructure):**
- All CONTEXT.md files in each stage folder
- All folder structures (00_Input/, 01_Job_Scoring/, 02_Top_Selection/, 03_Tailored_Applications/)
- Master CV files: Master_CV.md, Master_CV.pdf
- Preference files: job_preferences.md, work_experiences.md

Only after receiving explicit user confirmation (with name, date, and initials) may the generated results be deleted to reset the pipeline for new job descriptions.

### Step 6: Preserve Original Content (Until Deletion Confirmed)

**Important:** The archiving process does NOT delete or move content from the main pipeline directories (01_Job_Scoring, 02_Top_Selection, 03_Tailored_Applications). The original content remains in place for continued work. The cycle folder contains a complete snapshot copy for historical reference.

## Purpose and Benefits

### Cross-Reference
- Compare scoring decisions across cycles
- Track how job selection criteria evolve
- Reference past tailored applications for similar roles

### Learning and Improvement
- Analyze which jobs led to interviews/applications
- Refine scoring criteria based on outcomes
- Identify patterns in successful applications

### Historical Record
- Maintain complete audit trail of job search activity
- Document application timeline and outcomes
- Preserve context for future reference

## File Naming Within Cycles

- Maintain original file names from the source pipeline
- Application tracking file: `Cycle_XX_Application_Tracking.md`
- All dates preserved from original files

## Best Practices

- Create a new cycle after each complete pipeline run (scoring → selection → tailoring)
- Always complete the application status question before finalizing the archive
- Update application tracking file as outcomes develop (interview invitations, rejections, offers)
- Keep cycle folders intact - do not modify archived content
- Use archived cycles to inform future job selections and application strategies

---
*Archive Framework Version: 1.0 | Last Updated: 2026-06-01*