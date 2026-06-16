# AI for PowerPoint Demo Project

Advanced Session: **AI for PowerPoint: Creating Impactful Business Presentations using Prompt Engineering**.

## Demo Goal

Create an executive-ready PowerPoint deck from a business case using this workflow:

**Objective → Audience → Storyboard → Slide Draft → Visuals/Data → Speaker Notes → Executive Summary → Review**

## Files to Use During Demo

| File | Use |
|---|---|
| `source-files/AI_PPT_Demo_Source_Brief.docx` | Attach this when asking AI/Copilot to create the storyboard or first deck draft. |
| `source-files/SaaS_Churn_Data.xlsx` | Attach this for chart, KPI, and data-insight slides. |
| `source-files/SaaS_Churn_Data.csv` | Backup if Excel upload is unavailable. |
| `visuals/AI_for_PowerPoint_Workflow_Infographic.png` | Optional visual to show the AI-to-PPT workflow. |
| `presenters-assets/review-checklist.md` | Use for final peer review. |

## Phase-Wise Demo Flow

| Phase | Time | Objective | Attach | Prompt |
|---|---:|---|---|---|
| 1. Define deck objective | 5 min | Convert business need into presentation goal. | `AI_PPT_Demo_Source_Brief.docx` | `prompts/01-objective-audience.txt` |
| 2. Storyboard first | 10 min | Create slide-by-slide narrative before designing slides. | `AI_PPT_Demo_Source_Brief.docx` | `prompts/02-storyboard.txt` |
| 3. Generate starter deck | 15 min | Create first PowerPoint draft from the source brief. | `AI_PPT_Demo_Source_Brief.docx` | `prompts/03-create-deck.txt` |
| 4. Improve message quality | 10 min | Rewrite slide titles and bullets for executive clarity. | Current draft/slide text | `prompts/04-improve-slides.txt` |
| 5. Add data insight slide | 10 min | Convert dataset into chart recommendation and insight slide. | `SaaS_Churn_Data.xlsx` | `prompts/05-data-insight-chart.txt` |
| 6. Convert text to infographic | 10 min | Turn a text-heavy slide into a visual business slide. | Current slide text | `prompts/06-infographic-slide.txt` |
| 7. Generate speaker notes | 8 min | Create presenter notes for a selected slide. | Current slide/deck | `prompts/07-speaker-notes.txt` |
| 8. Executive summary | 7 min | Produce a CEO-ready summary slide. | Current deck/storyboard | `prompts/08-executive-summary.txt` |
| 9. Final review | 5 min | Check clarity, persuasion, visuals, and decision-readiness. | Current deck | `prompts/09-final-review.txt` |

## Expected Output

An 8-slide executive deck:

1. Customer Churn Requires Immediate Executive Action  
2. Churn Is Now Affecting Revenue Predictability  
3. Three Drivers Behind the Churn Increase  
4. Churn Is Concentrated in Specific Customer Groups  
5. 90-Day Churn Reduction Plan  
6. Projected Retention and Revenue Impact  
7. Execution Roadmap and Accountability  
8. Leadership Decisions Required Today  

## Presenter's Tip

Do not start by asking AI to “make a presentation.” First ask for the **storyboard**, then create slides, then refine message, visuals, notes, and summary.
