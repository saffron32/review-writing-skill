# ReviewWriting Skill

`review-writing` is a Codex skill for Chinese finance master's thesis writing tasks, especially literature reviews, domestic/foreign research-status sections, and literature review comments.

It is designed for cases where the output must be logically rigorous, source-faithful, and closer to finished thesis prose than to generic writing advice.

## Skill Description

This skill guides Codex to draft, revise, or evaluate Chinese academic literature-review text in finance-related master's thesis contexts.

It focuses on four core requirements:

- Build literature-review logic around `research theme -> representative findings -> theoretical or methodological support -> remaining issues`.
- Distinguish `国内外研究现状`, `文献综述`, and `文献评述` instead of treating them as the same section.
- Avoid fabricated, unverifiable, or overclaimed citations.
- Remove assistant-like process traces so the final text reads like student-written academic prose.

## Framework

The skill follows a structured workflow:

1. **Task clarification**
   It asks a mandatory questionnaire before substantial drafting, unless the user is only maintaining the skill or asking for high-level advice.

2. **Section-type judgment**
   It first identifies whether the task is an opening-report research-status section, a thesis-body literature review, a standalone review chapter, or a review-comment module.

3. **Source discipline**
   It requires cited claims to be grounded in user-provided papers, verified reference lists, extracted text, or verifiable external sources.

4. **Logic skeleton**
   It organizes the section by research theme, domestic/foreign distinction, research stage, application scenario, or method, depending on the user's requirements.

5. **Academic drafting**
   It writes by research logic rather than paper order, with citations supporting specific claims.

6. **Boundary control**
   It prevents literature-review sections from drifting into thesis design, model construction, data processing, backtesting workflow, or innovation claims unless explicitly requested.

7. **Final self-check**
   It internally checks logic continuity, citation support, section boundaries, gap validity, and AI-like phrasing before output.

## Suitable Use Cases

Use this skill when you need to:

- Draft or revise a Chinese finance master's thesis literature review.
- Write `国内外研究现状` for an opening report.
- Separate domestic and foreign research into a clearer staged structure.
- Write a `文献评述` or `研究评述` that synthesizes existing studies rather than repeating paper summaries.
- Polish an existing literature-review draft so it has stronger paragraph logic and fewer AI-like traces.
- Check whether cited papers actually support the claims made in the text.
- Convert a loose list of references into a more coherent research-background chain.

This skill is less suitable for:

- General English academic writing outside Chinese thesis contexts.
- Writing methods, empirical design, data processing, or model implementation sections.
- Generating citations from nothing.
- Producing final literature-supported prose when no usable source material or verifiable references are available.

## Installation

Clone or download this repository, then copy the `review-writing` folder into your Codex skills directory:

```bash
mkdir -p ~/.codex/skills
cp -R review-writing ~/.codex/skills/review-writing
```

Restart Codex after installation so the skill is loaded.

## Usage

In Codex, refer to the skill by name:

```text
Use $review-writing to revise this opening-report 国内外研究现状 section.
```

Example prompts:

```text
Use $review-writing. I need to write a 文献评述 for a finance master's opening report. I will provide my reference list and current draft.
```

```text
Use $review-writing to polish this literature review. Keep the original headings, reduce AI-like phrasing, and do not add unverifiable sources.
```

```text
Use $review-writing to distinguish 国内外研究现状 and 文献评述. Tell me which parts of my draft belong in each section.
```

## Recommended Input

For best results, provide:

- Thesis topic or proposed title.
- Required section type, such as `国内外研究现状`, `文献综述`, or `文献评述`.
- School template or formatting requirements, if any.
- Current draft, if revising existing text.
- Reference list or source papers.
- Citation style requirements.
- Expected length.
- Whether external source verification is allowed.

## Truthfulness And Citation Boundaries

The skill is intentionally conservative about sources.

It should not invent authors, years, paper titles, journals, page ranges, conclusions, methods, or findings. If the source cannot be verified or has not been read, claims should be excluded, qualified, or flagged instead of presented as fact.

## License

This repository is licensed under the MIT License.

The license applies only to the contents of this repository, including the `review-writing` skill and its accompanying documentation. It does not apply to other skills, private drafts, thesis materials, or repositories outside this project.
