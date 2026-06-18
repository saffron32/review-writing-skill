---
name: review-writing
description: Personalized workflow for drafting, revising, or evaluating Chinese finance master's thesis literature reviews, domestic/foreign research status sections, and literature review comments. Use when the user asks to write, polish, structure, distinguish "国内外研究现状" from "文献综述", or improve review-comment logic for a thesis or opening report, especially when they require verified sources, strict section boundaries, staged domestic/foreign research logic, non-mechanical citations, and reduced AI-like over-expansion.
---

# ReviewWriting

## Core Objective

Write finance thesis literature reviews and review comments as a logically rigorous research-background chain, not as a list of paper summaries.

Target logic:

`research theme/problem -> representative findings -> theoretical or methodological support -> remaining issues or research gaps`

Keep the section faithful to its purpose. A literature review or research-status section summarizes and evaluates existing research. Do not mix in detailed thesis design, model construction, data handling, backtesting steps, technical route, or innovation claims unless the user explicitly asks.

Treat writing templates or school handouts as form guidance, not factual evidence. Placeholder examples such as `XXX`, `学者A`, or invented years must never be retained as real content.

Final prose must read like a completed literature-review section written directly by the student. It must not contain assistant-like interaction, drafting instructions, reader-facing guidance, or process notes such as `下面为`, `建议`, `可放入`, `后文将`, `论文中应当`, `写作时不宜`, `需要说明的是`, or `需要注意的是` when these phrases function as guidance rather than academic argument.

## Mandatory Pre-Task Questionnaire

Before drafting or substantially rewriting thesis text with this skill, ask the user to answer the task-detail questionnaire. The user may respond with compact codes such as `1A, 2A, 3C`.

Skip the questionnaire when the user is only asking to maintain this skill, analyze a source document, or give high-level writing advice without drafting final thesis prose.

If an option is not suitable, the user may choose the final "Other" option and add text.

1. What type of text is this for?
   - A. Opening report
   - B. Master's thesis body
   - C. Standalone literature review chapter
   - D. Revision/polishing of existing text
   - E. Other, please specify

2. Which language-depth level should be used?
   - A. Opening-report level: formal, concise, clear logic
   - B. Master's-thesis-body level: fuller and more detailed
   - C. Light revision level: improve logic/expression without major expansion
   - D. Other, please specify

3. Does the structure distinguish domestic and foreign research?
   - A. No; organize by research theme/problem
   - B. Yes; separate domestic and foreign research
   - C. Existing headings are fixed; keep the original structure
   - D. Other, please specify

4. Is there a separate literature review-comment/evaluation module?
   - A. Yes; research status and review comments are separate
   - B. No; it is one complete literature review chapter
   - C. Only write research status
   - D. Other, please specify

5. May the review-comment section mention "this thesis/paper" or a specific research plan?
   - A. No by default
   - B. Only very restrained connection to the research gap, without plan details
   - C. Yes, briefly state the paper's response
   - D. Other, please specify

6. What is the source scope?
   - A. Only use files provided by the user
   - B. May also use the existing reference list
   - C. May add external verifiable sources
   - D. Other, please specify

7. What is the source-verification requirement?
   - A. Use only provided paper files
   - B. Verify uncertain source information first
   - C. Do not include sources that cannot be verified
   - D. Other, please specify

8. Should the final answer show self-check results?
   - A. Internal self-check only
   - B. Include a short self-check note
   - C. Include a detailed logic-check table
   - D. Other, please specify

9. Should the original structure/headings be preserved?
   - A. Preserve
   - B. May adjust subsection order
   - C. May rebuild the whole literature-review logic
   - D. Other, please specify

10. What is the expected length?
   - A. Concise
   - B. Substantive/content-rich
   - C. Similar to current draft length
   - D. Specific word count, please specify
   - E. Other, please specify

Do not proceed to final drafting until the questionnaire has been answered or the user explicitly instructs you to proceed without it.

## Common Form Requirements

For opening-report tasks, common school templates may expect:

- `国内外研究现状`: about 600-800 Chinese characters unless the user gives another length.
- `文献评述`: about 400-500 Chinese characters unless the user gives another length.
- `参考文献`: list cited and referenced works with complete bibliographic information.

These are defaults only when the user's institution-specific template is available or the user asks to follow common opening-report form. If the user provides a target length, it overrides these defaults.

## Section Type Distinction

`国内外研究现状` usually describes what scholars have studied, how the research developed, what representative views or findings exist, and what development tendencies can be seen. It can be split into foreign and domestic research when the school template requires that structure.

`文献综述` is usually broader: it may include research background, review purpose and scope, theoretical foundations, domestic and foreign research paths, research evaluation, outlook, and conclusion. It should show the evolution of the field and the relationship among studies, not merely list who said what.

`文献评述` or `研究评述` is evaluative. Use a compact three-step logic:

1. Summarize: identify the main research focus, methods, and conclusions.
2. Analyze: extract contributions, influence, strengths, and limitations.
3. Integrate: connect the limitations into current gaps and possible research directions.

## Source Truthfulness Rules

- Preserve truthfulness at all times.
- For literature-supported writing, verify source authenticity and bibliographic accuracy before use; the prose claim must match the cited work's actual topic, core finding, or argument.
- Use source claims only when grounded in user-provided papers, extracted text, a verified reference list, or current verifiable sources.
- If the user has provided and saved a paper file, assume the paper itself exists; still avoid inventing its methods, conclusions, journal, or pages unless read or otherwise verified.
- Do not include sources whose existence or bibliographic information cannot be verified when the user requires verification.
- Do not exaggerate what a paper proves. Use cautious verbs when the evidence is limited: "suggests", "indicates", "provides support for", "offers a reference for".

## Literature Selection Priorities

Prefer sources in this order:

1. Directly relevant empirical papers tied to the user's topic.
2. Representative papers that support the research background, research problem, or method basis.
3. Review papers that summarize the field.
4. Classic theory papers, used briefly.
5. Peripheral background papers, only when they improve the logic.

Do not try to use every paper. Include a source only if it supports the section's logic.

## Organization Rules

When domestic/foreign sections are not explicitly separated, organize by research theme or problem. Do not mechanically separate domestic and foreign research.

When headings explicitly separate domestic and foreign research, follow that structure.

For domestic/foreign research-status sections, choose one dominant organizing axis:

- Topic axis: definition/concept -> mechanism/theory -> method/model -> empirical application -> limitations.
- Stage axis for foreign research: origin or foundation -> development and extension -> recent frontier or debate.
- Stage axis for domestic research: introduction or early verification -> local adaptation -> deeper application or independent innovation.
- Application axis: key scenario or industry -> representative method -> evidence or effect -> unresolved issue.

Do not mix all axes in the same subsection unless the draft is long enough to support that complexity.

Within each subsection, prefer this progression when applicable:

1. Field positioning: what this research theme concerns and why it matters.
2. Theoretical or early research background, compressed when classic.
3. Method development or empirical extension.
4. Domestic application or market-specific evidence when relevant.
5. Limitations, unresolved issues, or research gaps.

Classic finance theory should be concise. Readers usually know basic finance theory; the text should spend more space on current field-specific studies, applied evidence, and methods that support the user's topic.

Each paragraph should usually contain no more than about 4-5 sources, but this is not rigid. Prioritize substance, synthesis, and support for the topic over a fixed citation count.

Use subsection wrap-ups only when natural. Avoid mechanical "In summary" endings after every subsection.

For gap extraction, classify the gap before drafting:

- Theoretical gap: concepts, mechanisms, or frameworks remain fragmented, transplanted, or insufficiently localized.
- Application gap: existing evidence is concentrated in certain markets, industries, firms, samples, or cases.
- Method gap: methods are single, static, weakly comparative, or not well matched to the research problem.
- Boundary gap: conclusions depend on specific periods, policy settings, market environments, or participant groups.

Use only gaps that are supported by the reviewed literature. Do not invent a gap simply to justify the thesis.

## Citation Style

Use the user's preferred citation form:

`claim or research finding...（author，year）。`

Prefer:

`Existing research finds that fund performance persistence is not unconditional, and short-term ranking may amplify style-reversal risk（作者，年份）。`

Avoid:

`作者（年份）指出……`

Avoid concentrating many sources in one parenthetical citation. A paragraph may cite several papers, but each citation should support a specific claim:

`...（作者A，年份）。Further research shows ...（作者B，年份）。`

If several papers share a similar claim, classify the claim first and then cite them in separate sentences or tightly related clauses. Citations are evidence, not decoration.

For reference-list formatting, follow the user's school or journal style first. If no style is provided, use standard Chinese thesis-style elements:

- Journal article: `[序号] 作者. 题名[J]. 刊名, 年, 卷(期): 起止页码.`
- Monograph, thesis, proceedings, report: `[序号] 作者. 题名[文献类型]. 出版地: 出版者, 年: 起止页码.`
- Newspaper: `[序号] 作者. 题名[N]. 报纸名, 出版日期(版次).`
- Standard or patent: include the standard number/name or patent owner/title/country/number/date.
- Electronic source: include author, title, carrier/source URL if available, update date or access date when required.

Do not fabricate page ranges, issue numbers, publishers, URLs, or access dates.

## Section Boundary Rules

If research status and literature review comments are separate:

- Research status: summarize existing research only.
- Review comments: synthesize consensus and limitations only.
- Do not write detailed model design, data processing, backtesting route, technical route, or innovation claims.
- Avoid "this paper will..." unless the questionnaire allows it.

If the task is one complete literature review chapter without a separate review-comment module:

- Each subsection may end with a natural synthesis paragraph.
- The synthesis may state what current research mainly covers and what remains underexplored.
- Keep the logic as: current research background -> scholars' findings -> validated useful models/tools/methods -> remaining problems or gaps.
- Still avoid detailed implementation plans.

## Review-Comment Section Rules

A review-comment section is not a compressed repetition of the research status section. It should abstract from the review.

Answer:

1. What consensus or foundations have existing studies formed?
2. What limitations or gaps remain?
3. Why are these limitations relevant to the thesis topic?

Use "First, Second, Third" only occasionally when it improves clarity. Avoid excessive list-like writing, quotation marks, stock transitions, and obvious AI-style phrasing.

When the review comment compares domestic and foreign literature, it may synthesize:

- Common foundations: shared theories, methods, models, variables, or application concerns.
- Different emphases: foreign frontier exploration vs. domestic local adaptation, or any other evidence-backed contrast.
- Current limitations: fragmented theory, narrow application scenarios, limited sample types, weak method integration, or insufficient local/external validity.
- Relevance to the thesis topic: state the connection to the selected research gap only as far as the questionnaire allows.

Avoid overconfident phrases such as "填补空白" unless the evidence is strong. Prefer restrained wording such as "可在一定程度上补充", "有助于拓展", or "为后续研究提供参考".

Do not leave review-writing process traces in the final prose. Sentences about how to use a source, where to place content, what the later paper will do, or how the writer should handle a claim must be rewritten as literature-based analysis or removed.

## Model and Method Detail Boundary

Allowed in literature review:

- What problem a model/method is suited for.
- What effect or advantage prior studies found.
- How the method supports the field background.

Avoid in literature review:

- Parameter settings.
- Training windows.
- Label construction.
- Backtesting workflow.
- Detailed technical route.
- The user's exact implementation plan.

## Workflow

1. Confirm task details with the questionnaire.
2. Read the target draft and source materials before rewriting.
3. Extract each useful paper's topic, method, conclusion, and relevance.
4. Decide the section type: domestic/foreign research status, literature review chapter, or review-comment module.
5. Choose the organizing axis: theme, domestic/foreign, research stage, application scenario, or method.
6. Build a logic skeleton before drafting.
7. Draft by research logic, not by paper order.
8. Check paragraph-to-paragraph and subsection-to-subsection transitions.
9. Remove content that is diffuse, repetitive, over-technical, placeholder-like, or belongs to another thesis section.
10. Verify citation format and source truthfulness.
11. Remove any AI-dialogue or drafting-process traces so the output reads as a finished student-written section.
12. Output the revised text or document according to the user's requested format.

## Self-Check Before Final Output

Always perform an internal self-check:

- Does each subsection have a clear theme?
- Does each paragraph connect to the previous and next paragraph?
- Does each cited paper support a specific claim?
- Are citations in `claim（author，year）` form?
- Are there any concentrated citation piles?
- Did the text avoid mixing in research design or technical-route content?
- Did the review-comment section avoid repeating the research-status section?
- Did the draft correctly distinguish `国内外研究现状`, `文献综述`, and `文献评述`?
- Are all stated gaps supported by the literature rather than invented for convenience?
- Were placeholder-style template phrases removed?
- Were all assistant-like, reader-facing, or drafting-process traces removed?
- Are uncertain or unverifiable sources excluded or flagged?
- Is the language suitable for the chosen depth level?

Only show this self-check in the final response if the questionnaire requests it.
