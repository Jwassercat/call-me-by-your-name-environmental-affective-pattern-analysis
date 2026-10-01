# AI analysis outputs

This folder collects the prompts and results from three runs of an AI-assisted environmental–affective analysis of 24 selected clips from *Call Me by Your Name*. The analyses use a human codebook, the screenplay, clip screenshots, and CIELAB image measurements. The workbook outputs cover 32 annotated script segments within those clips.

## Run1

- `Run1_prompt.docx` instructs the first analysis to match codebook rows, screenplay scenes, screenshots, and LAB measurements, then code character affect and environmental roles at script, clip, and cross-clip levels.
- `CMBYN_Codex_Environmental_Affective_Run1_Clarified.xlsx` contains 32 script-segment annotations in `Clip_Annotation`. `Detailed_AI_Pattern_Coding` adds clip summaries, within-clip shifts, recurring-environment trajectories, and narrative synthesis.

## Run2

- `Run2_prompt.docx` asks for a revision of Run 1 using film-wide and narrative-stage trends in lightness, chroma, and contrast, alongside a researcher-provided account of Elio's emotional trajectory.
- `CMBYN_Codex_Environmental_Affective_Run1_Patterns_Revised.xlsx` contains the revised annotations and pattern analysis in the same two worksheets as Run 1.
- `Pattern_Label_Changes.csv` logs 11 pattern-label revisions, with each annotation row, old and new label, and reason for the change.

## Run3

Run 3 separates the work into three stages. Each stage has a prompt and a corresponding workbook:

| Subfolder | Prompt | Analytical output |
| --- | --- | --- |
| `stage1/` | `Run3_stage1_prompt.docx` asks for narrative-affect analysis from the human codebook, screenplay, and screenshots, without new color or environmental-pattern coding. | `Underlying_affect.xlsx` contains 32 rows in `Narrative_Affect_Review`, distinguishing visible action and surface emotion from underlying affect, immediate emotional goals, expression, context, evidence, confidence, and review notes. Its `Issues` sheet records questions needing human review. |
| `stage2/` | `Run3_stage2_prompt.docx` asks for a quantitative visual-feeling synthesis from existing CIELAB results, separate from character emotion or narrative interpretation. | `Visual_feeling_synthesis.xlsx` contains one `Clip_Visual_Feeling` row for each of the 24 clips, comparing clip measurements with a film-wide reference and describing within-clip visual progression and overall visual character. It also includes `LAB_Metrics` and `Issues` sheets. |
| `stage3/` | `Run3_stage3_prompt.docx` asks for final integration of the established stage 1 findings, approved stage 2 visual synthesis, human environmental annotations, and spatial evidence from screenshots. | `Environmental_affective_integration.xlsx` contains 32 rows in `Integrated_Analysis`, covering spatial interpretation, environmental-affective quality, scene mood, environment–emotion alignment, pattern labels, explanations, and evidence references. Its `Issues` sheet lists unresolved integration questions. |

Paths embedded in the prompts and workbooks refer to the original local working locations and may differ from this folder's layout. Hidden `.DS_Store` files and names beginning `~$` are operating-system or Office temporary files, not analysis deliverables.
