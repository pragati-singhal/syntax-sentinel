# Changelog — SyntaxSentinel (PE-B49-07)

## [v4.0 - Final M2] - 2026-11-21
- Split single-prompt workflow into a two-stage chained pipeline (`P1` Code Triage + `P2` Pedagogical Mentor).
- Added strict input validation guardrails for non-code and unsupported languages (Java/C++).
- Executed 12-case evaluation suite (6 Normal, 4 Edge, 2 Invalid) in Google AI Studio (`Gemini 3.8 Flash`).

## [v3.0] - 2026-11-15
- Added few-shot C and Python examples to eliminate JSON schema breakage.
- Achieved 10/10 valid JSON parses on test runs, though complex multi-bug C pointers still triggered occasional partial code leaks.

## [v2.0] - 2026-11-05
- Added explicit negative constraints ("Do NOT write corrected code") and enforced structured JSON output format.
- Reduced direct answer leakage from 80% to 20%, but JSON formatting broke in 3 out of 10 runs.

## [v1.0 - Milestone 1 Baseline] - 2026-10-11
- Created initial zero-shot role prompt for reviewing Python and C snippets.
- Observed frequent full-solution leakage and inconsistent feedback formatting.
