# ORI offline analysis

Source run: `../runs/seed67-qwen38flash-gpt6luna-recovery-20261002`

Source integrity: **structural-public-projection-only** (not a cryptographic attestation).
Benchmark completion: **partial**.
Analysis coverage: public aggregate report only; task evidence not independently revalidated.
Publication status: **not published**.

## Findings

1. **observed behavior** — direct / qwen3.8-flash-nous / repetition 1: 31/50 correct on the scheduled denominator (62.0%) (Evidence: report.json#/results/0)
2. **observed behavior** — Recorded outcome/failure counts: {'OUTPUT_INVALID': 13, 'QUERY_ERROR': 3} (Evidence: report.json#/results/0)
3. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=31; outcomes={'COMPLETED': 34, 'QUERY_ERROR': 3, 'OUTPUT_INVALID': 13}. (Evidence: report.json#/question_results)
4. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/0)
5. **observed behavior** — direct / qwen3.8-flash-nous / repetition 2: 35/50 correct on the scheduled denominator (70.0%) (Evidence: report.json#/results/1)
6. **observed behavior** — Recorded outcome/failure counts: {'OUTPUT_INVALID': 12, 'QUERY_ERROR': 1} (Evidence: report.json#/results/1)
7. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=35; outcomes={'COMPLETED': 37, 'OUTPUT_INVALID': 12, 'QUERY_ERROR': 1}. (Evidence: report.json#/question_results)
8. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/1)
9. **observed behavior** — direct / qwen3.8-flash-nous / repetition 3: 30/50 correct on the scheduled denominator (60.0%) (Evidence: report.json#/results/2)
10. **observed behavior** — Recorded outcome/failure counts: {'OUTPUT_INVALID': 12, 'QUERY_ERROR': 4} (Evidence: report.json#/results/2)
11. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=30; outcomes={'COMPLETED': 34, 'QUERY_ERROR': 4, 'OUTPUT_INVALID': 12}. (Evidence: report.json#/question_results)
12. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/2)
13. **observed behavior** — mcp / qwen3.8-flash-nous / repetition 1: 28/50 correct on the scheduled denominator (56.0%) (Evidence: report.json#/results/3)
14. **observed behavior** — Recorded outcome/failure counts: {'OUTPUT_INVALID': 5} (Evidence: report.json#/results/3)
15. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=28; outcomes={'COMPLETED': 45, 'OUTPUT_INVALID': 5}. (Evidence: report.json#/question_results)
16. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/3)
17. **observed behavior** — mcp / qwen3.8-flash-nous / repetition 2: 26/50 correct on the scheduled denominator (52.0%) (Evidence: report.json#/results/4)
18. **observed behavior** — Recorded outcome/failure counts: {'OUTPUT_INVALID': 6} (Evidence: report.json#/results/4)
19. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=26; outcomes={'COMPLETED': 44, 'OUTPUT_INVALID': 6}. (Evidence: report.json#/question_results)
20. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/4)
21. **observed behavior** — mcp / qwen3.8-flash-nous / repetition 3: 28/50 correct on the scheduled denominator (56.0%) (Evidence: report.json#/results/5)
22. **observed behavior** — Recorded outcome/failure counts: {'OUTPUT_INVALID': 5} (Evidence: report.json#/results/5)
23. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=28; outcomes={'COMPLETED': 45, 'OUTPUT_INVALID': 5}. (Evidence: report.json#/question_results)
24. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/5)
25. **observed behavior** — mcp / qwen3.8-flash-nous / repetition 1: 12/50 correct on the scheduled denominator (24.0%) (Evidence: report.json#/results/6)
26. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 50/50; missing slots=0; state=failed (Evidence: report.json#/results/6)
27. **observed behavior** — Recorded outcome/failure counts: {'INFRA_ERROR': 6, 'OUTPUT_INVALID': 6} (Evidence: report.json#/results/6)
28. **hypothesis** — Infrastructure or harness conditions could contribute to these recorded outcomes; the public aggregate alone cannot distinguish that from other causes or establish model-quality effects. (Evidence: report.json#/results/6)
29. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/6)
30. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=10; correct=12; outcomes={'INFRA_ERROR': 6, 'COMPLETED': 38, 'OUTPUT_INVALID': 6}. (Evidence: report.json#/question_results)
31. **observed behavior** — Recorded provider attempt count: 60 (Evidence: report.json#/results/6)
32. **observed behavior** — mcp / qwen3.8-flash-nous / repetition 2: 14/50 correct on the scheduled denominator (28.0%) (Evidence: report.json#/results/7)
33. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 50/50; missing slots=0; state=failed (Evidence: report.json#/results/7)
34. **observed behavior** — Recorded outcome/failure counts: {'INFRA_ERROR': 9, 'OUTPUT_INVALID': 4} (Evidence: report.json#/results/7)
35. **hypothesis** — Infrastructure or harness conditions could contribute to these recorded outcomes; the public aggregate alone cannot distinguish that from other causes or establish model-quality effects. (Evidence: report.json#/results/7)
36. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/7)
37. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=9; correct=14; outcomes={'COMPLETED': 37, 'INFRA_ERROR': 9, 'OUTPUT_INVALID': 4}. (Evidence: report.json#/question_results)
38. **observed behavior** — Recorded provider attempt count: 59 (Evidence: report.json#/results/7)
39. **observed behavior** — mcp / qwen3.8-flash-nous / repetition 3: 0/50 correct on the scheduled denominator (0.0%) (Evidence: report.json#/results/8)
40. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 1/50; missing slots=49; state=failed (Evidence: report.json#/results/8)
41. **observed behavior** — Recorded outcome/failure counts: {'INFRA_ERROR': 1, 'MISSING': 49} (Evidence: report.json#/results/8)
42. **hypothesis** — Infrastructure or harness conditions could contribute to these recorded outcomes; the public aggregate alone cannot distinguish that from other causes or establish model-quality effects. (Evidence: report.json#/results/8)
43. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/8)
44. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=49; recorded extra attempts/retries=0; correct=0; outcomes={'INFRA_ERROR': 1, 'MISSING': 49}. (Evidence: report.json#/question_results)
45. **observed behavior** — Recorded provider attempt count: 1 (Evidence: report.json#/results/8)
46. **observed behavior** — mcp / qwen3.8-flash-nous / repetition 1: 21/50 correct on the scheduled denominator (42.0%) (Evidence: report.json#/results/9)
47. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 50/50; missing slots=0; state=failed (Evidence: report.json#/results/9)
48. **observed behavior** — Recorded outcome/failure counts: {'OUTPUT_INVALID': 5} (Evidence: report.json#/results/9)
49. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/9)
50. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=1; correct=21; outcomes={'COMPLETED': 45, 'OUTPUT_INVALID': 5}. (Evidence: report.json#/question_results)
51. **observed behavior** — Recorded provider attempt count: 51 (Evidence: report.json#/results/9)
52. **observed behavior** — mcp / qwen3.8-flash-nous / repetition 2: 26/50 correct on the scheduled denominator (52.0%) (Evidence: report.json#/results/10)
53. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 50/50; missing slots=0; state=failed (Evidence: report.json#/results/10)
54. **observed behavior** — Recorded outcome/failure counts: {'OUTPUT_INVALID': 5} (Evidence: report.json#/results/10)
55. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/10)
56. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=26; outcomes={'COMPLETED': 45, 'OUTPUT_INVALID': 5}. (Evidence: report.json#/question_results)
57. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/10)
58. **observed behavior** — mcp / qwen3.8-flash-nous / repetition 3: 23/50 correct on the scheduled denominator (46.0%) (Evidence: report.json#/results/11)
59. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 50/50; missing slots=0; state=failed (Evidence: report.json#/results/11)
60. **observed behavior** — Recorded outcome/failure counts: {'OUTPUT_INVALID': 6} (Evidence: report.json#/results/11)
61. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/11)
62. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=23; outcomes={'COMPLETED': 44, 'OUTPUT_INVALID': 6}. (Evidence: report.json#/question_results)
63. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/11)
64. **observed behavior** — mcp / gpt-6-luna-nous / repetition 1: 49/50 correct on the scheduled denominator (98.0%) (Evidence: report.json#/results/12)
65. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 50/50; missing slots=0; state=failed (Evidence: report.json#/results/12)
66. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/12)
67. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=2; correct=49; outcomes={'COMPLETED': 50}. (Evidence: report.json#/question_results)
68. **observed behavior** — Recorded provider attempt count: 52 (Evidence: report.json#/results/12)

## Comparisons

- `../runs/seed67-qwen38flash-gpt6luna-recovery-20261002` vs `../runs/seed67-step1-six-models-3rep-3mcp-20260930`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-qwen38flash-gpt6luna-recovery-20261002` vs `../runs/deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-qwen38flash-gpt6luna-recovery-20261002` vs `../runs/luna-nous-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-qwen38flash-gpt6luna-recovery-20261002` vs `../runs/glm53flash-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-qwen38flash-gpt6luna-recovery-20261002` vs `../runs/shared-matrix-seed67-bloodhound-nous-codex-20260928`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-qwen38flash-gpt6luna-recovery-20261002` vs `../runs/qwen3.8-json-rerun-2`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-step1-six-models-3rep-3mcp-20260930` vs `../runs/deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-step1-six-models-3rep-3mcp-20260930` vs `../runs/luna-nous-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-step1-six-models-3rep-3mcp-20260930` vs `../runs/glm53flash-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-step1-six-models-3rep-3mcp-20260930` vs `../runs/shared-matrix-seed67-bloodhound-nous-codex-20260928`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-step1-six-models-3rep-3mcp-20260930` vs `../runs/qwen3.8-json-rerun-2`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929` vs `../runs/luna-nous-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929` vs `../runs/glm53flash-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable
- `../runs/deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929` vs `../runs/shared-matrix-seed67-bloodhound-nous-codex-20260928`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929` vs `../runs/qwen3.8-json-rerun-2`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/luna-nous-shared-matrix-seed67-3mcp-20260929` vs `../runs/glm53flash-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/luna-nous-shared-matrix-seed67-3mcp-20260929` vs `../runs/shared-matrix-seed67-bloodhound-nous-codex-20260928`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/luna-nous-shared-matrix-seed67-3mcp-20260929` vs `../runs/qwen3.8-json-rerun-2`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/glm53flash-shared-matrix-seed67-3mcp-20260929` vs `../runs/shared-matrix-seed67-bloodhound-nous-codex-20260928`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/glm53flash-shared-matrix-seed67-3mcp-20260929` vs `../runs/qwen3.8-json-rerun-2`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/shared-matrix-seed67-bloodhound-nous-codex-20260928` vs `../runs/qwen3.8-json-rerun-2`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ


---

# ORI offline analysis

Source run: `../runs/seed67-step1-six-models-3rep-3mcp-20260930`

Source integrity: **structural-public-projection-only** (not a cryptographic attestation).
Benchmark completion: **partial**.
Analysis coverage: public aggregate report only; task evidence not independently revalidated.
Publication status: **not published**.

## Findings

1. **observed behavior** — direct / gpt-6-luna-nous / repetition 1: 40/50 correct on the scheduled denominator (80.0%) (Evidence: report.json#/results/0)
2. **observed behavior** — Recorded outcome/failure counts: {'QUERY_ERROR': 3, 'QUERY_TIMEOUT': 6} (Evidence: report.json#/results/0)
3. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=40; outcomes={'COMPLETED': 41, 'QUERY_TIMEOUT': 6, 'QUERY_ERROR': 3}. (Evidence: report.json#/question_results)
4. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/0)
5. **observed behavior** — direct / gpt-6-luna-nous / repetition 2: 43/50 correct on the scheduled denominator (86.0%) (Evidence: report.json#/results/1)
6. **observed behavior** — Recorded outcome/failure counts: {'QUERY_ERROR': 4, 'QUERY_TIMEOUT': 1} (Evidence: report.json#/results/1)
7. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=43; outcomes={'COMPLETED': 45, 'QUERY_TIMEOUT': 1, 'QUERY_ERROR': 4}. (Evidence: report.json#/question_results)
8. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/1)
9. **observed behavior** — direct / gpt-6-luna-nous / repetition 3: 45/50 correct on the scheduled denominator (90.0%) (Evidence: report.json#/results/2)
10. **observed behavior** — Recorded outcome/failure counts: {'QUERY_ERROR': 3, 'QUERY_TIMEOUT': 2} (Evidence: report.json#/results/2)
11. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=45; outcomes={'COMPLETED': 45, 'QUERY_TIMEOUT': 2, 'QUERY_ERROR': 3}. (Evidence: report.json#/question_results)
12. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/2)
13. **observed behavior** — mcp / gpt-6-luna-nous / repetition 1: 47/50 correct on the scheduled denominator (94.0%) (Evidence: report.json#/results/3)
14. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 50/50; missing slots=0; state=failed (Evidence: report.json#/results/3)
15. **observed behavior** — Recorded outcome/failure counts: {'INFRA_ERROR': 1} (Evidence: report.json#/results/3)
16. **hypothesis** — Infrastructure or harness conditions could contribute to these recorded outcomes; the public aggregate alone cannot distinguish that from other causes or establish model-quality effects. (Evidence: report.json#/results/3)
17. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/3)
18. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=47; outcomes={'COMPLETED': 49, 'INFRA_ERROR': 1}. (Evidence: report.json#/question_results)
19. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/3)
20. **observed behavior** — mcp / gpt-6-luna-nous / repetition 2: 49/50 correct on the scheduled denominator (98.0%) (Evidence: report.json#/results/4)
21. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 50/50; missing slots=0; state=failed (Evidence: report.json#/results/4)
22. **observed behavior** — Recorded outcome/failure counts: {'OUTPUT_INVALID': 1} (Evidence: report.json#/results/4)
23. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/4)
24. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=49; outcomes={'COMPLETED': 49, 'OUTPUT_INVALID': 1}. (Evidence: report.json#/question_results)
25. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/4)
26. **observed behavior** — mcp / gpt-6-luna-nous / repetition 3: 49/50 correct on the scheduled denominator (98.0%) (Evidence: report.json#/results/5)
27. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 50/50; missing slots=0; state=failed (Evidence: report.json#/results/5)
28. **observed behavior** — Recorded outcome/failure counts: {'OUTPUT_INVALID': 1} (Evidence: report.json#/results/5)
29. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/5)
30. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=49; outcomes={'COMPLETED': 49, 'OUTPUT_INVALID': 1}. (Evidence: report.json#/question_results)
31. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/5)
32. **observed behavior** — mcp / gpt-6-luna-nous / repetition 1: 32/50 correct on the scheduled denominator (64.0%) (Evidence: report.json#/results/6)
33. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 50/50; missing slots=0; state=failed (Evidence: report.json#/results/6)
34. **observed behavior** — Recorded outcome/failure counts: {'INFRA_ERROR': 1, 'OUTPUT_INVALID': 1} (Evidence: report.json#/results/6)
35. **hypothesis** — Infrastructure or harness conditions could contribute to these recorded outcomes; the public aggregate alone cannot distinguish that from other causes or establish model-quality effects. (Evidence: report.json#/results/6)
36. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/6)
37. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=32; outcomes={'COMPLETED': 48, 'INFRA_ERROR': 1, 'OUTPUT_INVALID': 1}. (Evidence: report.json#/question_results)
38. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/6)
39. **observed behavior** — mcp / gpt-6-luna-nous / repetition 2: 32/50 correct on the scheduled denominator (64.0%) (Evidence: report.json#/results/7)
40. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 50/50; missing slots=0; state=failed (Evidence: report.json#/results/7)
41. **observed behavior** — Recorded outcome/failure counts: {'INFRA_ERROR': 2, 'OUTPUT_INVALID': 1} (Evidence: report.json#/results/7)
42. **hypothesis** — Infrastructure or harness conditions could contribute to these recorded outcomes; the public aggregate alone cannot distinguish that from other causes or establish model-quality effects. (Evidence: report.json#/results/7)
43. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/7)
44. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=32; outcomes={'COMPLETED': 47, 'INFRA_ERROR': 2, 'OUTPUT_INVALID': 1}. (Evidence: report.json#/question_results)
45. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/7)
46. **observed behavior** — mcp / gpt-6-luna-nous / repetition 3: 31/50 correct on the scheduled denominator (62.0%) (Evidence: report.json#/results/8)
47. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 50/50; missing slots=0; state=failed (Evidence: report.json#/results/8)
48. **observed behavior** — Recorded outcome/failure counts: {'INFRA_ERROR': 2, 'OUTPUT_INVALID': 1} (Evidence: report.json#/results/8)
49. **hypothesis** — Infrastructure or harness conditions could contribute to these recorded outcomes; the public aggregate alone cannot distinguish that from other causes or establish model-quality effects. (Evidence: report.json#/results/8)
50. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/8)
51. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=31; outcomes={'COMPLETED': 47, 'INFRA_ERROR': 2, 'OUTPUT_INVALID': 1}. (Evidence: report.json#/question_results)
52. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/8)
53. **observed behavior** — mcp / gpt-6-luna-nous / repetition 1: 50/50 correct on the scheduled denominator (100.0%) (Evidence: report.json#/results/9)
54. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 50/50; missing slots=0; state=failed (Evidence: report.json#/results/9)
55. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/9)
56. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=50; outcomes={'COMPLETED': 50}. (Evidence: report.json#/question_results)
57. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/9)
58. **observed behavior** — mcp / gpt-6-luna-nous / repetition 2: 48/50 correct on the scheduled denominator (96.0%) (Evidence: report.json#/results/10)
59. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 50/50; missing slots=0; state=failed (Evidence: report.json#/results/10)
60. **observed behavior** — Recorded outcome/failure counts: {'INFRA_ERROR': 1, 'OUTPUT_INVALID': 1} (Evidence: report.json#/results/10)
61. **hypothesis** — Infrastructure or harness conditions could contribute to these recorded outcomes; the public aggregate alone cannot distinguish that from other causes or establish model-quality effects. (Evidence: report.json#/results/10)
62. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/10)
63. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=48; outcomes={'COMPLETED': 48, 'OUTPUT_INVALID': 1, 'INFRA_ERROR': 1}. (Evidence: report.json#/question_results)
64. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/10)
65. **observed behavior** — mcp / gpt-6-luna-nous / repetition 3: 19/50 correct on the scheduled denominator (38.0%) (Evidence: report.json#/results/11)
66. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 23/50; missing slots=27; state=failed (Evidence: report.json#/results/11)
67. **observed behavior** — Recorded outcome/failure counts: {'INFRA_ERROR': 3, 'MISSING': 27, 'OUTPUT_INVALID': 1} (Evidence: report.json#/results/11)
68. **hypothesis** — Infrastructure or harness conditions could contribute to these recorded outcomes; the public aggregate alone cannot distinguish that from other causes or establish model-quality effects. (Evidence: report.json#/results/11)
69. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/11)
70. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=27; recorded extra attempts/retries=0; correct=19; outcomes={'COMPLETED': 19, 'OUTPUT_INVALID': 1, 'INFRA_ERROR': 3, 'MISSING': 27}. (Evidence: report.json#/question_results)
71. **observed behavior** — Recorded provider attempt count: 23 (Evidence: report.json#/results/11)
72. **observed behavior** — direct / glm-5.3-flash-nous / repetition 1: 38/50 correct on the scheduled denominator (76.0%) (Evidence: report.json#/results/12)
73. **observed behavior** — Recorded outcome/failure counts: {'OUTPUT_INVALID': 5, 'QUERY_ERROR': 4} (Evidence: report.json#/results/12)
74. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=38; outcomes={'COMPLETED': 41, 'OUTPUT_INVALID': 5, 'QUERY_ERROR': 4}. (Evidence: report.json#/question_results)
75. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/12)
76. **observed behavior** — direct / glm-5.3-flash-nous / repetition 2: 39/50 correct on the scheduled denominator (78.0%) (Evidence: report.json#/results/13)
77. **observed behavior** — Recorded outcome/failure counts: {'OUTPUT_INVALID': 5, 'QUERY_ERROR': 2} (Evidence: report.json#/results/13)
78. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=39; outcomes={'COMPLETED': 43, 'OUTPUT_INVALID': 5, 'QUERY_ERROR': 2}. (Evidence: report.json#/question_results)
79. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/13)
80. **observed behavior** — direct / glm-5.3-flash-nous / repetition 3: 36/50 correct on the scheduled denominator (72.0%) (Evidence: report.json#/results/14)
81. **observed behavior** — Recorded outcome/failure counts: {'OUTPUT_INVALID': 9, 'QUERY_ERROR': 4} (Evidence: report.json#/results/14)
82. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=36; outcomes={'COMPLETED': 37, 'OUTPUT_INVALID': 9, 'QUERY_ERROR': 4}. (Evidence: report.json#/question_results)
83. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/14)
84. **observed behavior** — mcp / glm-5.3-flash-nous / repetition 1: 23/50 correct on the scheduled denominator (46.0%) (Evidence: report.json#/results/15)
85. **observed behavior** — Recorded outcome/failure counts: {'OUTPUT_INVALID': 10} (Evidence: report.json#/results/15)
86. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=23; outcomes={'COMPLETED': 40, 'OUTPUT_INVALID': 10}. (Evidence: report.json#/question_results)
87. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/15)
88. **observed behavior** — mcp / glm-5.3-flash-nous / repetition 2: 26/50 correct on the scheduled denominator (52.0%) (Evidence: report.json#/results/16)
89. **observed behavior** — Recorded outcome/failure counts: {'OUTPUT_INVALID': 12} (Evidence: report.json#/results/16)
90. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=26; outcomes={'COMPLETED': 38, 'OUTPUT_INVALID': 12}. (Evidence: report.json#/question_results)
91. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/16)
92. **observed behavior** — mcp / glm-5.3-flash-nous / repetition 3: 24/50 correct on the scheduled denominator (48.0%) (Evidence: report.json#/results/17)
93. **observed behavior** — Recorded outcome/failure counts: {'OUTPUT_INVALID': 13} (Evidence: report.json#/results/17)
94. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=24; outcomes={'COMPLETED': 37, 'OUTPUT_INVALID': 13}. (Evidence: report.json#/question_results)
95. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/17)
96. **observed behavior** — mcp / glm-5.3-flash-nous / repetition 1: 15/50 correct on the scheduled denominator (30.0%) (Evidence: report.json#/results/18)
97. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 50/50; missing slots=0; state=failed (Evidence: report.json#/results/18)
98. **observed behavior** — Recorded outcome/failure counts: {'INFRA_ERROR': 2, 'OUTPUT_INVALID': 9} (Evidence: report.json#/results/18)
99. **hypothesis** — Infrastructure or harness conditions could contribute to these recorded outcomes; the public aggregate alone cannot distinguish that from other causes or establish model-quality effects. (Evidence: report.json#/results/18)
100. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/18)
101. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=15; outcomes={'COMPLETED': 39, 'OUTPUT_INVALID': 9, 'INFRA_ERROR': 2}. (Evidence: report.json#/question_results)
102. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/18)
103. **observed behavior** — mcp / glm-5.3-flash-nous / repetition 2: 19/50 correct on the scheduled denominator (38.0%) (Evidence: report.json#/results/19)
104. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 50/50; missing slots=0; state=failed (Evidence: report.json#/results/19)
105. **observed behavior** — Recorded outcome/failure counts: {'INFRA_ERROR': 2, 'OUTPUT_INVALID': 7} (Evidence: report.json#/results/19)
106. **hypothesis** — Infrastructure or harness conditions could contribute to these recorded outcomes; the public aggregate alone cannot distinguish that from other causes or establish model-quality effects. (Evidence: report.json#/results/19)
107. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/19)
108. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=19; outcomes={'COMPLETED': 41, 'OUTPUT_INVALID': 7, 'INFRA_ERROR': 2}. (Evidence: report.json#/question_results)
109. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/19)
110. **observed behavior** — mcp / glm-5.3-flash-nous / repetition 3: 17/50 correct on the scheduled denominator (34.0%) (Evidence: report.json#/results/20)
111. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 50/50; missing slots=0; state=failed (Evidence: report.json#/results/20)
112. **observed behavior** — Recorded outcome/failure counts: {'INFRA_ERROR': 3, 'OUTPUT_INVALID': 10} (Evidence: report.json#/results/20)
113. **hypothesis** — Infrastructure or harness conditions could contribute to these recorded outcomes; the public aggregate alone cannot distinguish that from other causes or establish model-quality effects. (Evidence: report.json#/results/20)
114. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/20)
115. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=17; outcomes={'COMPLETED': 37, 'OUTPUT_INVALID': 10, 'INFRA_ERROR': 3}. (Evidence: report.json#/question_results)
116. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/20)
117. **observed behavior** — mcp / glm-5.3-flash-nous / repetition 1: 27/50 correct on the scheduled denominator (54.0%) (Evidence: report.json#/results/21)
118. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 50/50; missing slots=0; state=failed (Evidence: report.json#/results/21)
119. **observed behavior** — Recorded outcome/failure counts: {'INFRA_ERROR': 1, 'OUTPUT_INVALID': 4} (Evidence: report.json#/results/21)
120. **hypothesis** — Infrastructure or harness conditions could contribute to these recorded outcomes; the public aggregate alone cannot distinguish that from other causes or establish model-quality effects. (Evidence: report.json#/results/21)
121. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/21)
122. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=27; outcomes={'COMPLETED': 45, 'OUTPUT_INVALID': 4, 'INFRA_ERROR': 1}. (Evidence: report.json#/question_results)
123. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/21)
124. **observed behavior** — mcp / glm-5.3-flash-nous / repetition 2: 30/50 correct on the scheduled denominator (60.0%) (Evidence: report.json#/results/22)
125. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 50/50; missing slots=0; state=failed (Evidence: report.json#/results/22)
126. **observed behavior** — Recorded outcome/failure counts: {'INFRA_ERROR': 1, 'OUTPUT_INVALID': 4} (Evidence: report.json#/results/22)
127. **hypothesis** — Infrastructure or harness conditions could contribute to these recorded outcomes; the public aggregate alone cannot distinguish that from other causes or establish model-quality effects. (Evidence: report.json#/results/22)
128. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/22)
129. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=30; outcomes={'COMPLETED': 45, 'OUTPUT_INVALID': 4, 'INFRA_ERROR': 1}. (Evidence: report.json#/question_results)
130. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/22)
131. **observed behavior** — mcp / glm-5.3-flash-nous / repetition 3: 30/50 correct on the scheduled denominator (60.0%) (Evidence: report.json#/results/23)
132. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 50/50; missing slots=0; state=failed (Evidence: report.json#/results/23)
133. **observed behavior** — Recorded outcome/failure counts: {'OUTPUT_INVALID': 7} (Evidence: report.json#/results/23)
134. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/23)
135. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=30; outcomes={'COMPLETED': 43, 'OUTPUT_INVALID': 7}. (Evidence: report.json#/question_results)
136. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/23)
137. **observed behavior** — direct / deepseek-v4.1-flash-nous / repetition 1: 32/50 correct on the scheduled denominator (64.0%) (Evidence: report.json#/results/24)
138. **observed behavior** — Recorded outcome/failure counts: {'OUTPUT_INVALID': 3, 'QUERY_ERROR': 5, 'TASK_TIMEOUT': 5} (Evidence: report.json#/results/24)
139. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=32; outcomes={'COMPLETED': 37, 'TASK_TIMEOUT': 5, 'OUTPUT_INVALID': 3, 'QUERY_ERROR': 5}. (Evidence: report.json#/question_results)
140. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/24)
141. **observed behavior** — direct / deepseek-v4.1-flash-nous / repetition 2: 35/50 correct on the scheduled denominator (70.0%) (Evidence: report.json#/results/25)
142. **observed behavior** — Recorded outcome/failure counts: {'OUTPUT_INVALID': 7, 'QUERY_ERROR': 5} (Evidence: report.json#/results/25)
143. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=35; outcomes={'COMPLETED': 38, 'OUTPUT_INVALID': 7, 'QUERY_ERROR': 5}. (Evidence: report.json#/question_results)
144. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/25)
145. **observed behavior** — direct / deepseek-v4.1-flash-nous / repetition 3: 32/50 correct on the scheduled denominator (64.0%) (Evidence: report.json#/results/26)
146. **observed behavior** — Recorded outcome/failure counts: {'OUTPUT_INVALID': 10, 'QUERY_ERROR': 5} (Evidence: report.json#/results/26)
147. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=32; outcomes={'COMPLETED': 35, 'OUTPUT_INVALID': 10, 'QUERY_ERROR': 5}. (Evidence: report.json#/question_results)
148. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/26)
149. **observed behavior** — mcp / deepseek-v4.1-flash-nous / repetition 1: 28/50 correct on the scheduled denominator (56.0%) (Evidence: report.json#/results/27)
150. **observed behavior** — Recorded outcome/failure counts: {'OUTPUT_INVALID': 4} (Evidence: report.json#/results/27)
151. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=28; outcomes={'COMPLETED': 46, 'OUTPUT_INVALID': 4}. (Evidence: report.json#/question_results)
152. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/27)
153. **observed behavior** — mcp / deepseek-v4.1-flash-nous / repetition 2: 27/50 correct on the scheduled denominator (54.0%) (Evidence: report.json#/results/28)
154. **observed behavior** — Recorded outcome/failure counts: {'OUTPUT_INVALID': 3} (Evidence: report.json#/results/28)
155. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=27; outcomes={'COMPLETED': 47, 'OUTPUT_INVALID': 3}. (Evidence: report.json#/question_results)
156. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/28)
157. **observed behavior** — mcp / deepseek-v4.1-flash-nous / repetition 3: 27/50 correct on the scheduled denominator (54.0%) (Evidence: report.json#/results/29)
158. **observed behavior** — Recorded outcome/failure counts: {'OUTPUT_INVALID': 4} (Evidence: report.json#/results/29)
159. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=27; outcomes={'COMPLETED': 46, 'OUTPUT_INVALID': 4}. (Evidence: report.json#/question_results)
160. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/29)
161. **observed behavior** — mcp / deepseek-v4.1-flash-nous / repetition 1: 25/50 correct on the scheduled denominator (50.0%) (Evidence: report.json#/results/30)
162. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 50/50; missing slots=0; state=failed (Evidence: report.json#/results/30)
163. **observed behavior** — Recorded outcome/failure counts: {'INFRA_ERROR': 1, 'OUTPUT_INVALID': 2} (Evidence: report.json#/results/30)
164. **hypothesis** — Infrastructure or harness conditions could contribute to these recorded outcomes; the public aggregate alone cannot distinguish that from other causes or establish model-quality effects. (Evidence: report.json#/results/30)
165. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/30)
166. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=25; outcomes={'COMPLETED': 47, 'INFRA_ERROR': 1, 'OUTPUT_INVALID': 2}. (Evidence: report.json#/question_results)
167. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/30)
168. **observed behavior** — mcp / deepseek-v4.1-flash-nous / repetition 2: 26/50 correct on the scheduled denominator (52.0%) (Evidence: report.json#/results/31)
169. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 50/50; missing slots=0; state=failed (Evidence: report.json#/results/31)
170. **observed behavior** — Recorded outcome/failure counts: {'INFRA_ERROR': 2, 'OUTPUT_INVALID': 4} (Evidence: report.json#/results/31)
171. **hypothesis** — Infrastructure or harness conditions could contribute to these recorded outcomes; the public aggregate alone cannot distinguish that from other causes or establish model-quality effects. (Evidence: report.json#/results/31)
172. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/31)
173. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=26; outcomes={'COMPLETED': 44, 'INFRA_ERROR': 2, 'OUTPUT_INVALID': 4}. (Evidence: report.json#/question_results)
174. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/31)
175. **observed behavior** — mcp / deepseek-v4.1-flash-nous / repetition 3: 22/50 correct on the scheduled denominator (44.0%) (Evidence: report.json#/results/32)
176. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 50/50; missing slots=0; state=failed (Evidence: report.json#/results/32)
177. **observed behavior** — Recorded outcome/failure counts: {'INFRA_ERROR': 2, 'OUTPUT_INVALID': 2} (Evidence: report.json#/results/32)
178. **hypothesis** — Infrastructure or harness conditions could contribute to these recorded outcomes; the public aggregate alone cannot distinguish that from other causes or establish model-quality effects. (Evidence: report.json#/results/32)
179. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/32)
180. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=22; outcomes={'COMPLETED': 46, 'INFRA_ERROR': 2, 'OUTPUT_INVALID': 2}. (Evidence: report.json#/question_results)
181. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/32)
182. **observed behavior** — mcp / deepseek-v4.1-flash-nous / repetition 1: 35/50 correct on the scheduled denominator (70.0%) (Evidence: report.json#/results/33)
183. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 50/50; missing slots=0; state=failed (Evidence: report.json#/results/33)
184. **observed behavior** — Recorded outcome/failure counts: {'OUTPUT_INVALID': 3} (Evidence: report.json#/results/33)
185. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/33)
186. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=35; outcomes={'COMPLETED': 47, 'OUTPUT_INVALID': 3}. (Evidence: report.json#/question_results)
187. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/33)
188. **observed behavior** — mcp / deepseek-v4.1-flash-nous / repetition 2: 35/50 correct on the scheduled denominator (70.0%) (Evidence: report.json#/results/34)
189. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 50/50; missing slots=0; state=failed (Evidence: report.json#/results/34)
190. **observed behavior** — Recorded outcome/failure counts: {'OUTPUT_INVALID': 3} (Evidence: report.json#/results/34)
191. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/34)
192. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=35; outcomes={'COMPLETED': 47, 'OUTPUT_INVALID': 3}. (Evidence: report.json#/question_results)
193. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/34)
194. **observed behavior** — mcp / deepseek-v4.1-flash-nous / repetition 3: 34/50 correct on the scheduled denominator (68.0%) (Evidence: report.json#/results/35)
195. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 50/50; missing slots=0; state=failed (Evidence: report.json#/results/35)
196. **observed behavior** — Recorded outcome/failure counts: {'OUTPUT_INVALID': 3} (Evidence: report.json#/results/35)
197. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/35)
198. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=34; outcomes={'COMPLETED': 47, 'OUTPUT_INVALID': 3}. (Evidence: report.json#/question_results)
199. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/35)
200. **observed behavior** — direct / qwen3.8-27b-q4km / repetition 1: 6/50 correct on the scheduled denominator (12.0%) (Evidence: report.json#/results/36)
201. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 50/50; missing slots=0; state=interrupted (Evidence: report.json#/results/36)
202. **observed behavior** — Recorded outcome/failure counts: {'TASK_TIMEOUT': 44} (Evidence: report.json#/results/36)
203. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/36)
204. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=6; outcomes={'TASK_TIMEOUT': 44, 'COMPLETED': 6}. (Evidence: report.json#/question_results)
205. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/36)
206. **observed behavior** — direct / qwen3.8-27b-q4km / repetition 2: 6/50 correct on the scheduled denominator (12.0%) (Evidence: report.json#/results/37)
207. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 21/50; missing slots=29; state=interrupted (Evidence: report.json#/results/37)
208. **observed behavior** — Recorded outcome/failure counts: {'INTERRUPTED': 1, 'MISSING': 29, 'TASK_TIMEOUT': 13} (Evidence: report.json#/results/37)
209. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/37)
210. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=29; recorded extra attempts/retries=0; correct=6; outcomes={'TASK_TIMEOUT': 13, 'COMPLETED': 7, 'INTERRUPTED': 1, 'MISSING': 29}. (Evidence: report.json#/question_results)
211. **observed behavior** — Recorded provider attempt count: 21 (Evidence: report.json#/results/37)
212. **observed behavior** — direct / qwen3.8-27b-q4km / repetition 3: 0/50 correct on the scheduled denominator (0.0%) (Evidence: report.json#/results/38)
213. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 0/50; missing slots=50; state=interrupted (Evidence: report.json#/results/38)
214. **observed behavior** — Recorded outcome/failure counts: {'MISSING': 50} (Evidence: report.json#/results/38)
215. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/38)
216. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=50; recorded extra attempts/retries=0; correct=0; outcomes={'MISSING': 50}. (Evidence: report.json#/question_results)
217. **observed behavior** — Recorded provider attempt count: 0 (Evidence: report.json#/results/38)
218. **observed behavior** — mcp / qwen3.8-27b-q4km / repetition 1: 0/50 correct on the scheduled denominator (0.0%) (Evidence: report.json#/results/39)
219. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 0/50; missing slots=50; state=unknown (Evidence: report.json#/results/39)
220. **observed behavior** — Recorded outcome/failure counts: {'MISSING': 50} (Evidence: report.json#/results/39)
221. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/39)
222. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=50; recorded extra attempts/retries=0; correct=0; outcomes={'MISSING': 50}. (Evidence: report.json#/question_results)
223. **observed behavior** — Recorded provider attempt count: 0 (Evidence: report.json#/results/39)
224. **observed behavior** — mcp / qwen3.8-27b-q4km / repetition 2: 0/50 correct on the scheduled denominator (0.0%) (Evidence: report.json#/results/40)
225. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 0/50; missing slots=50; state=unknown (Evidence: report.json#/results/40)
226. **observed behavior** — Recorded outcome/failure counts: {'MISSING': 50} (Evidence: report.json#/results/40)
227. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/40)
228. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=50; recorded extra attempts/retries=0; correct=0; outcomes={'MISSING': 50}. (Evidence: report.json#/question_results)
229. **observed behavior** — Recorded provider attempt count: 0 (Evidence: report.json#/results/40)
230. **observed behavior** — mcp / qwen3.8-27b-q4km / repetition 3: 0/50 correct on the scheduled denominator (0.0%) (Evidence: report.json#/results/41)
231. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 0/50; missing slots=50; state=unknown (Evidence: report.json#/results/41)
232. **observed behavior** — Recorded outcome/failure counts: {'MISSING': 50} (Evidence: report.json#/results/41)
233. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/41)
234. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=50; recorded extra attempts/retries=0; correct=0; outcomes={'MISSING': 50}. (Evidence: report.json#/question_results)
235. **observed behavior** — Recorded provider attempt count: 0 (Evidence: report.json#/results/41)
236. **observed behavior** — mcp / qwen3.8-27b-q4km / repetition 1: 0/50 correct on the scheduled denominator (0.0%) (Evidence: report.json#/results/42)
237. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 0/50; missing slots=50; state=unknown (Evidence: report.json#/results/42)
238. **observed behavior** — Recorded outcome/failure counts: {'MISSING': 50} (Evidence: report.json#/results/42)
239. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/42)
240. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=50; recorded extra attempts/retries=0; correct=0; outcomes={'MISSING': 50}. (Evidence: report.json#/question_results)
241. **observed behavior** — Recorded provider attempt count: 0 (Evidence: report.json#/results/42)
242. **observed behavior** — mcp / qwen3.8-27b-q4km / repetition 2: 0/50 correct on the scheduled denominator (0.0%) (Evidence: report.json#/results/43)
243. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 0/50; missing slots=50; state=unknown (Evidence: report.json#/results/43)
244. **observed behavior** — Recorded outcome/failure counts: {'MISSING': 50} (Evidence: report.json#/results/43)
245. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/43)
246. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=50; recorded extra attempts/retries=0; correct=0; outcomes={'MISSING': 50}. (Evidence: report.json#/question_results)
247. **observed behavior** — Recorded provider attempt count: 0 (Evidence: report.json#/results/43)
248. **observed behavior** — mcp / qwen3.8-27b-q4km / repetition 3: 0/50 correct on the scheduled denominator (0.0%) (Evidence: report.json#/results/44)
249. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 0/50; missing slots=50; state=unknown (Evidence: report.json#/results/44)
250. **observed behavior** — Recorded outcome/failure counts: {'MISSING': 50} (Evidence: report.json#/results/44)
251. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/44)
252. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=50; recorded extra attempts/retries=0; correct=0; outcomes={'MISSING': 50}. (Evidence: report.json#/question_results)
253. **observed behavior** — Recorded provider attempt count: 0 (Evidence: report.json#/results/44)
254. **observed behavior** — mcp / qwen3.8-27b-q4km / repetition 1: 0/50 correct on the scheduled denominator (0.0%) (Evidence: report.json#/results/45)
255. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 0/50; missing slots=50; state=unknown (Evidence: report.json#/results/45)
256. **observed behavior** — Recorded outcome/failure counts: {'MISSING': 50} (Evidence: report.json#/results/45)
257. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/45)
258. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=50; recorded extra attempts/retries=0; correct=0; outcomes={'MISSING': 50}. (Evidence: report.json#/question_results)
259. **observed behavior** — Recorded provider attempt count: 0 (Evidence: report.json#/results/45)
260. **observed behavior** — mcp / qwen3.8-27b-q4km / repetition 2: 0/50 correct on the scheduled denominator (0.0%) (Evidence: report.json#/results/46)
261. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 0/50; missing slots=50; state=unknown (Evidence: report.json#/results/46)
262. **observed behavior** — Recorded outcome/failure counts: {'MISSING': 50} (Evidence: report.json#/results/46)
263. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/46)
264. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=50; recorded extra attempts/retries=0; correct=0; outcomes={'MISSING': 50}. (Evidence: report.json#/question_results)
265. **observed behavior** — Recorded provider attempt count: 0 (Evidence: report.json#/results/46)
266. **observed behavior** — mcp / qwen3.8-27b-q4km / repetition 3: 0/50 correct on the scheduled denominator (0.0%) (Evidence: report.json#/results/47)
267. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 0/50; missing slots=50; state=unknown (Evidence: report.json#/results/47)
268. **observed behavior** — Recorded outcome/failure counts: {'MISSING': 50} (Evidence: report.json#/results/47)
269. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/47)
270. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=50; recorded extra attempts/retries=0; correct=0; outcomes={'MISSING': 50}. (Evidence: report.json#/question_results)
271. **observed behavior** — Recorded provider attempt count: 0 (Evidence: report.json#/results/47)
272. **observed behavior** — direct / muse-glimmer-30b / repetition 1: 0/50 correct on the scheduled denominator (0.0%) (Evidence: report.json#/results/48)
273. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 0/50; missing slots=50; state=unknown (Evidence: report.json#/results/48)
274. **observed behavior** — Recorded outcome/failure counts: {'MISSING': 50} (Evidence: report.json#/results/48)
275. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/48)
276. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=50; recorded extra attempts/retries=0; correct=0; outcomes={'MISSING': 50}. (Evidence: report.json#/question_results)
277. **observed behavior** — Recorded provider attempt count: 0 (Evidence: report.json#/results/48)
278. **observed behavior** — direct / muse-glimmer-30b / repetition 2: 0/50 correct on the scheduled denominator (0.0%) (Evidence: report.json#/results/49)
279. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 0/50; missing slots=50; state=unknown (Evidence: report.json#/results/49)
280. **observed behavior** — Recorded outcome/failure counts: {'MISSING': 50} (Evidence: report.json#/results/49)
281. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/49)
282. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=50; recorded extra attempts/retries=0; correct=0; outcomes={'MISSING': 50}. (Evidence: report.json#/question_results)
283. **observed behavior** — Recorded provider attempt count: 0 (Evidence: report.json#/results/49)
284. **observed behavior** — direct / muse-glimmer-30b / repetition 3: 0/50 correct on the scheduled denominator (0.0%) (Evidence: report.json#/results/50)
285. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 0/50; missing slots=50; state=unknown (Evidence: report.json#/results/50)
286. **observed behavior** — Recorded outcome/failure counts: {'MISSING': 50} (Evidence: report.json#/results/50)
287. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/50)
288. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=50; recorded extra attempts/retries=0; correct=0; outcomes={'MISSING': 50}. (Evidence: report.json#/question_results)
289. **observed behavior** — Recorded provider attempt count: 0 (Evidence: report.json#/results/50)
290. **observed behavior** — mcp / muse-glimmer-30b / repetition 1: 0/50 correct on the scheduled denominator (0.0%) (Evidence: report.json#/results/51)
291. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 0/50; missing slots=50; state=unknown (Evidence: report.json#/results/51)
292. **observed behavior** — Recorded outcome/failure counts: {'MISSING': 50} (Evidence: report.json#/results/51)
293. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/51)
294. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=50; recorded extra attempts/retries=0; correct=0; outcomes={'MISSING': 50}. (Evidence: report.json#/question_results)
295. **observed behavior** — Recorded provider attempt count: 0 (Evidence: report.json#/results/51)
296. **observed behavior** — mcp / muse-glimmer-30b / repetition 2: 0/50 correct on the scheduled denominator (0.0%) (Evidence: report.json#/results/52)
297. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 0/50; missing slots=50; state=unknown (Evidence: report.json#/results/52)
298. **observed behavior** — Recorded outcome/failure counts: {'MISSING': 50} (Evidence: report.json#/results/52)
299. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/52)
300. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=50; recorded extra attempts/retries=0; correct=0; outcomes={'MISSING': 50}. (Evidence: report.json#/question_results)
301. **observed behavior** — Recorded provider attempt count: 0 (Evidence: report.json#/results/52)
302. **observed behavior** — mcp / muse-glimmer-30b / repetition 3: 0/50 correct on the scheduled denominator (0.0%) (Evidence: report.json#/results/53)
303. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 0/50; missing slots=50; state=unknown (Evidence: report.json#/results/53)
304. **observed behavior** — Recorded outcome/failure counts: {'MISSING': 50} (Evidence: report.json#/results/53)
305. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/53)
306. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=50; recorded extra attempts/retries=0; correct=0; outcomes={'MISSING': 50}. (Evidence: report.json#/question_results)
307. **observed behavior** — Recorded provider attempt count: 0 (Evidence: report.json#/results/53)
308. **observed behavior** — mcp / muse-glimmer-30b / repetition 1: 0/50 correct on the scheduled denominator (0.0%) (Evidence: report.json#/results/54)
309. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 0/50; missing slots=50; state=unknown (Evidence: report.json#/results/54)
310. **observed behavior** — Recorded outcome/failure counts: {'MISSING': 50} (Evidence: report.json#/results/54)
311. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/54)
312. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=50; recorded extra attempts/retries=0; correct=0; outcomes={'MISSING': 50}. (Evidence: report.json#/question_results)
313. **observed behavior** — Recorded provider attempt count: 0 (Evidence: report.json#/results/54)
314. **observed behavior** — mcp / muse-glimmer-30b / repetition 2: 0/50 correct on the scheduled denominator (0.0%) (Evidence: report.json#/results/55)
315. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 0/50; missing slots=50; state=unknown (Evidence: report.json#/results/55)
316. **observed behavior** — Recorded outcome/failure counts: {'MISSING': 50} (Evidence: report.json#/results/55)
317. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/55)
318. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=50; recorded extra attempts/retries=0; correct=0; outcomes={'MISSING': 50}. (Evidence: report.json#/question_results)
319. **observed behavior** — Recorded provider attempt count: 0 (Evidence: report.json#/results/55)
320. **observed behavior** — mcp / muse-glimmer-30b / repetition 3: 0/50 correct on the scheduled denominator (0.0%) (Evidence: report.json#/results/56)
321. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 0/50; missing slots=50; state=unknown (Evidence: report.json#/results/56)
322. **observed behavior** — Recorded outcome/failure counts: {'MISSING': 50} (Evidence: report.json#/results/56)
323. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/56)
324. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=50; recorded extra attempts/retries=0; correct=0; outcomes={'MISSING': 50}. (Evidence: report.json#/question_results)
325. **observed behavior** — Recorded provider attempt count: 0 (Evidence: report.json#/results/56)
326. **observed behavior** — mcp / muse-glimmer-30b / repetition 1: 0/50 correct on the scheduled denominator (0.0%) (Evidence: report.json#/results/57)
327. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 0/50; missing slots=50; state=unknown (Evidence: report.json#/results/57)
328. **observed behavior** — Recorded outcome/failure counts: {'MISSING': 50} (Evidence: report.json#/results/57)
329. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/57)
330. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=50; recorded extra attempts/retries=0; correct=0; outcomes={'MISSING': 50}. (Evidence: report.json#/question_results)
331. **observed behavior** — Recorded provider attempt count: 0 (Evidence: report.json#/results/57)
332. **observed behavior** — mcp / muse-glimmer-30b / repetition 2: 0/50 correct on the scheduled denominator (0.0%) (Evidence: report.json#/results/58)
333. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 0/50; missing slots=50; state=unknown (Evidence: report.json#/results/58)
334. **observed behavior** — Recorded outcome/failure counts: {'MISSING': 50} (Evidence: report.json#/results/58)
335. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/58)
336. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=50; recorded extra attempts/retries=0; correct=0; outcomes={'MISSING': 50}. (Evidence: report.json#/question_results)
337. **observed behavior** — Recorded provider attempt count: 0 (Evidence: report.json#/results/58)
338. **observed behavior** — mcp / muse-glimmer-30b / repetition 3: 0/50 correct on the scheduled denominator (0.0%) (Evidence: report.json#/results/59)
339. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 0/50; missing slots=50; state=unknown (Evidence: report.json#/results/59)
340. **observed behavior** — Recorded outcome/failure counts: {'MISSING': 50} (Evidence: report.json#/results/59)
341. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/59)
342. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=50; recorded extra attempts/retries=0; correct=0; outcomes={'MISSING': 50}. (Evidence: report.json#/question_results)
343. **observed behavior** — Recorded provider attempt count: 0 (Evidence: report.json#/results/59)
344. **observed behavior** — direct / gemma-4-26b-it-qat-q4-0-64k / repetition 1: 0/50 correct on the scheduled denominator (0.0%) (Evidence: report.json#/results/60)
345. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 0/50; missing slots=50; state=unknown (Evidence: report.json#/results/60)
346. **observed behavior** — Recorded outcome/failure counts: {'MISSING': 50} (Evidence: report.json#/results/60)
347. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/60)
348. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=50; recorded extra attempts/retries=0; correct=0; outcomes={'MISSING': 50}. (Evidence: report.json#/question_results)
349. **observed behavior** — Recorded provider attempt count: 0 (Evidence: report.json#/results/60)
350. **observed behavior** — direct / gemma-4-26b-it-qat-q4-0-64k / repetition 2: 0/50 correct on the scheduled denominator (0.0%) (Evidence: report.json#/results/61)
351. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 0/50; missing slots=50; state=unknown (Evidence: report.json#/results/61)
352. **observed behavior** — Recorded outcome/failure counts: {'MISSING': 50} (Evidence: report.json#/results/61)
353. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/61)
354. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=50; recorded extra attempts/retries=0; correct=0; outcomes={'MISSING': 50}. (Evidence: report.json#/question_results)
355. **observed behavior** — Recorded provider attempt count: 0 (Evidence: report.json#/results/61)
356. **observed behavior** — direct / gemma-4-26b-it-qat-q4-0-64k / repetition 3: 0/50 correct on the scheduled denominator (0.0%) (Evidence: report.json#/results/62)
357. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 0/50; missing slots=50; state=unknown (Evidence: report.json#/results/62)
358. **observed behavior** — Recorded outcome/failure counts: {'MISSING': 50} (Evidence: report.json#/results/62)
359. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/62)
360. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=50; recorded extra attempts/retries=0; correct=0; outcomes={'MISSING': 50}. (Evidence: report.json#/question_results)
361. **observed behavior** — Recorded provider attempt count: 0 (Evidence: report.json#/results/62)
362. **observed behavior** — mcp / gemma-4-26b-it-qat-q4-0-64k / repetition 1: 0/50 correct on the scheduled denominator (0.0%) (Evidence: report.json#/results/63)
363. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 0/50; missing slots=50; state=unknown (Evidence: report.json#/results/63)
364. **observed behavior** — Recorded outcome/failure counts: {'MISSING': 50} (Evidence: report.json#/results/63)
365. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/63)
366. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=50; recorded extra attempts/retries=0; correct=0; outcomes={'MISSING': 50}. (Evidence: report.json#/question_results)
367. **observed behavior** — Recorded provider attempt count: 0 (Evidence: report.json#/results/63)
368. **observed behavior** — mcp / gemma-4-26b-it-qat-q4-0-64k / repetition 2: 0/50 correct on the scheduled denominator (0.0%) (Evidence: report.json#/results/64)
369. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 0/50; missing slots=50; state=unknown (Evidence: report.json#/results/64)
370. **observed behavior** — Recorded outcome/failure counts: {'MISSING': 50} (Evidence: report.json#/results/64)
371. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/64)
372. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=50; recorded extra attempts/retries=0; correct=0; outcomes={'MISSING': 50}. (Evidence: report.json#/question_results)
373. **observed behavior** — Recorded provider attempt count: 0 (Evidence: report.json#/results/64)
374. **observed behavior** — mcp / gemma-4-26b-it-qat-q4-0-64k / repetition 3: 0/50 correct on the scheduled denominator (0.0%) (Evidence: report.json#/results/65)
375. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 0/50; missing slots=50; state=unknown (Evidence: report.json#/results/65)
376. **observed behavior** — Recorded outcome/failure counts: {'MISSING': 50} (Evidence: report.json#/results/65)
377. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/65)
378. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=50; recorded extra attempts/retries=0; correct=0; outcomes={'MISSING': 50}. (Evidence: report.json#/question_results)
379. **observed behavior** — Recorded provider attempt count: 0 (Evidence: report.json#/results/65)
380. **observed behavior** — mcp / gemma-4-26b-it-qat-q4-0-64k / repetition 1: 0/50 correct on the scheduled denominator (0.0%) (Evidence: report.json#/results/66)
381. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 0/50; missing slots=50; state=unknown (Evidence: report.json#/results/66)
382. **observed behavior** — Recorded outcome/failure counts: {'MISSING': 50} (Evidence: report.json#/results/66)
383. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/66)
384. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=50; recorded extra attempts/retries=0; correct=0; outcomes={'MISSING': 50}. (Evidence: report.json#/question_results)
385. **observed behavior** — Recorded provider attempt count: 0 (Evidence: report.json#/results/66)
386. **observed behavior** — mcp / gemma-4-26b-it-qat-q4-0-64k / repetition 2: 0/50 correct on the scheduled denominator (0.0%) (Evidence: report.json#/results/67)
387. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 0/50; missing slots=50; state=unknown (Evidence: report.json#/results/67)
388. **observed behavior** — Recorded outcome/failure counts: {'MISSING': 50} (Evidence: report.json#/results/67)
389. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/67)
390. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=50; recorded extra attempts/retries=0; correct=0; outcomes={'MISSING': 50}. (Evidence: report.json#/question_results)
391. **observed behavior** — Recorded provider attempt count: 0 (Evidence: report.json#/results/67)
392. **observed behavior** — mcp / gemma-4-26b-it-qat-q4-0-64k / repetition 3: 0/50 correct on the scheduled denominator (0.0%) (Evidence: report.json#/results/68)
393. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 0/50; missing slots=50; state=unknown (Evidence: report.json#/results/68)
394. **observed behavior** — Recorded outcome/failure counts: {'MISSING': 50} (Evidence: report.json#/results/68)
395. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/68)
396. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=50; recorded extra attempts/retries=0; correct=0; outcomes={'MISSING': 50}. (Evidence: report.json#/question_results)
397. **observed behavior** — Recorded provider attempt count: 0 (Evidence: report.json#/results/68)
398. **observed behavior** — mcp / gemma-4-26b-it-qat-q4-0-64k / repetition 1: 0/50 correct on the scheduled denominator (0.0%) (Evidence: report.json#/results/69)
399. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 0/50; missing slots=50; state=unknown (Evidence: report.json#/results/69)
400. **observed behavior** — Recorded outcome/failure counts: {'MISSING': 50} (Evidence: report.json#/results/69)
401. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/69)
402. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=50; recorded extra attempts/retries=0; correct=0; outcomes={'MISSING': 50}. (Evidence: report.json#/question_results)
403. **observed behavior** — Recorded provider attempt count: 0 (Evidence: report.json#/results/69)
404. **observed behavior** — mcp / gemma-4-26b-it-qat-q4-0-64k / repetition 2: 0/50 correct on the scheduled denominator (0.0%) (Evidence: report.json#/results/70)
405. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 0/50; missing slots=50; state=unknown (Evidence: report.json#/results/70)
406. **observed behavior** — Recorded outcome/failure counts: {'MISSING': 50} (Evidence: report.json#/results/70)
407. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/70)
408. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=50; recorded extra attempts/retries=0; correct=0; outcomes={'MISSING': 50}. (Evidence: report.json#/question_results)
409. **observed behavior** — Recorded provider attempt count: 0 (Evidence: report.json#/results/70)
410. **observed behavior** — mcp / gemma-4-26b-it-qat-q4-0-64k / repetition 3: 0/50 correct on the scheduled denominator (0.0%) (Evidence: report.json#/results/71)
411. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 0/50; missing slots=50; state=unknown (Evidence: report.json#/results/71)
412. **observed behavior** — Recorded outcome/failure counts: {'MISSING': 50} (Evidence: report.json#/results/71)
413. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/71)
414. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=50; recorded extra attempts/retries=0; correct=0; outcomes={'MISSING': 50}. (Evidence: report.json#/question_results)
415. **observed behavior** — Recorded provider attempt count: 0 (Evidence: report.json#/results/71)

## Comparisons

- `../runs/seed67-qwen38flash-gpt6luna-recovery-20261002` vs `../runs/seed67-step1-six-models-3rep-3mcp-20260930`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-qwen38flash-gpt6luna-recovery-20261002` vs `../runs/deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-qwen38flash-gpt6luna-recovery-20261002` vs `../runs/luna-nous-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-qwen38flash-gpt6luna-recovery-20261002` vs `../runs/glm53flash-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-qwen38flash-gpt6luna-recovery-20261002` vs `../runs/shared-matrix-seed67-bloodhound-nous-codex-20260928`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-qwen38flash-gpt6luna-recovery-20261002` vs `../runs/qwen3.8-json-rerun-2`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-step1-six-models-3rep-3mcp-20260930` vs `../runs/deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-step1-six-models-3rep-3mcp-20260930` vs `../runs/luna-nous-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-step1-six-models-3rep-3mcp-20260930` vs `../runs/glm53flash-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-step1-six-models-3rep-3mcp-20260930` vs `../runs/shared-matrix-seed67-bloodhound-nous-codex-20260928`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-step1-six-models-3rep-3mcp-20260930` vs `../runs/qwen3.8-json-rerun-2`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929` vs `../runs/luna-nous-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929` vs `../runs/glm53flash-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable
- `../runs/deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929` vs `../runs/shared-matrix-seed67-bloodhound-nous-codex-20260928`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929` vs `../runs/qwen3.8-json-rerun-2`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/luna-nous-shared-matrix-seed67-3mcp-20260929` vs `../runs/glm53flash-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/luna-nous-shared-matrix-seed67-3mcp-20260929` vs `../runs/shared-matrix-seed67-bloodhound-nous-codex-20260928`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/luna-nous-shared-matrix-seed67-3mcp-20260929` vs `../runs/qwen3.8-json-rerun-2`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/glm53flash-shared-matrix-seed67-3mcp-20260929` vs `../runs/shared-matrix-seed67-bloodhound-nous-codex-20260928`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/glm53flash-shared-matrix-seed67-3mcp-20260929` vs `../runs/qwen3.8-json-rerun-2`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/shared-matrix-seed67-bloodhound-nous-codex-20260928` vs `../runs/qwen3.8-json-rerun-2`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ


---

# ORI offline analysis

Source run: `../runs/deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929`

Source integrity: **structural-public-projection-only** (not a cryptographic attestation).
Benchmark completion: **partial**.
Analysis coverage: public aggregate report only; task evidence not independently revalidated.
Publication status: **not published**.

## Findings

1. **observed behavior** — direct / deepseek-v4.1-flash-nous / repetition 1: 29/50 correct on the scheduled denominator (58.0%) (Evidence: report.json#/results/0)
2. **observed behavior** — Recorded outcome/failure counts: {'QUERY_ERROR': 4, 'QUERY_TIMEOUT': 1, 'TASK_TIMEOUT': 12} (Evidence: report.json#/results/0)
3. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=29; outcomes={'COMPLETED': 33, 'TASK_TIMEOUT': 12, 'QUERY_ERROR': 4, 'QUERY_TIMEOUT': 1}. (Evidence: report.json#/question_results)
4. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/0)
5. **observed behavior** — mcp / deepseek-v4.1-flash-nous / repetition 1: 38/50 correct on the scheduled denominator (76.0%) (Evidence: report.json#/results/1)
6. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 50/50; missing slots=0; state=failed (Evidence: report.json#/results/1)
7. **observed behavior** — Recorded outcome/failure counts: {'INFRA_ERROR': 1, 'OUTPUT_INVALID': 4} (Evidence: report.json#/results/1)
8. **hypothesis** — Infrastructure or harness conditions could contribute to these recorded outcomes; the public aggregate alone cannot distinguish that from other causes or establish model-quality effects. (Evidence: report.json#/results/1)
9. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/1)
10. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=38; outcomes={'COMPLETED': 45, 'OUTPUT_INVALID': 4, 'INFRA_ERROR': 1}. (Evidence: report.json#/question_results)
11. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/1)
12. **observed behavior** — mcp / deepseek-v4.1-flash-nous / repetition 1: 23/50 correct on the scheduled denominator (46.0%) (Evidence: report.json#/results/2)
13. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 50/50; missing slots=0; state=failed (Evidence: report.json#/results/2)
14. **observed behavior** — Recorded outcome/failure counts: {'INFRA_ERROR': 1, 'OUTPUT_INVALID': 2} (Evidence: report.json#/results/2)
15. **hypothesis** — Infrastructure or harness conditions could contribute to these recorded outcomes; the public aggregate alone cannot distinguish that from other causes or establish model-quality effects. (Evidence: report.json#/results/2)
16. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/2)
17. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=23; outcomes={'COMPLETED': 47, 'OUTPUT_INVALID': 2, 'INFRA_ERROR': 1}. (Evidence: report.json#/question_results)
18. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/2)
19. **observed behavior** — mcp / deepseek-v4.1-flash-nous / repetition 1: 36/50 correct on the scheduled denominator (72.0%) (Evidence: report.json#/results/3)
20. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 50/50; missing slots=0; state=failed (Evidence: report.json#/results/3)
21. **observed behavior** — Recorded outcome/failure counts: {'OUTPUT_INVALID': 3} (Evidence: report.json#/results/3)
22. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/3)
23. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=36; outcomes={'COMPLETED': 47, 'OUTPUT_INVALID': 3}. (Evidence: report.json#/question_results)
24. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/3)

## Comparisons

- `../runs/seed67-qwen38flash-gpt6luna-recovery-20261002` vs `../runs/seed67-step1-six-models-3rep-3mcp-20260930`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-qwen38flash-gpt6luna-recovery-20261002` vs `../runs/deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-qwen38flash-gpt6luna-recovery-20261002` vs `../runs/luna-nous-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-qwen38flash-gpt6luna-recovery-20261002` vs `../runs/glm53flash-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-qwen38flash-gpt6luna-recovery-20261002` vs `../runs/shared-matrix-seed67-bloodhound-nous-codex-20260928`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-qwen38flash-gpt6luna-recovery-20261002` vs `../runs/qwen3.8-json-rerun-2`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-step1-six-models-3rep-3mcp-20260930` vs `../runs/deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-step1-six-models-3rep-3mcp-20260930` vs `../runs/luna-nous-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-step1-six-models-3rep-3mcp-20260930` vs `../runs/glm53flash-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-step1-six-models-3rep-3mcp-20260930` vs `../runs/shared-matrix-seed67-bloodhound-nous-codex-20260928`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-step1-six-models-3rep-3mcp-20260930` vs `../runs/qwen3.8-json-rerun-2`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929` vs `../runs/luna-nous-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929` vs `../runs/glm53flash-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable
- `../runs/deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929` vs `../runs/shared-matrix-seed67-bloodhound-nous-codex-20260928`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929` vs `../runs/qwen3.8-json-rerun-2`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/luna-nous-shared-matrix-seed67-3mcp-20260929` vs `../runs/glm53flash-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/luna-nous-shared-matrix-seed67-3mcp-20260929` vs `../runs/shared-matrix-seed67-bloodhound-nous-codex-20260928`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/luna-nous-shared-matrix-seed67-3mcp-20260929` vs `../runs/qwen3.8-json-rerun-2`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/glm53flash-shared-matrix-seed67-3mcp-20260929` vs `../runs/shared-matrix-seed67-bloodhound-nous-codex-20260928`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/glm53flash-shared-matrix-seed67-3mcp-20260929` vs `../runs/qwen3.8-json-rerun-2`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/shared-matrix-seed67-bloodhound-nous-codex-20260928` vs `../runs/qwen3.8-json-rerun-2`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ


---

# ORI offline analysis

Source run: `../runs/luna-nous-shared-matrix-seed67-3mcp-20260929`

Source integrity: **structural-public-projection-only** (not a cryptographic attestation).
Benchmark completion: **partial**.
Analysis coverage: public aggregate report only; task evidence not independently revalidated.
Publication status: **not published**.

## Findings

1. **observed behavior** — direct / gpt-6-luna-nous / repetition 1: 46/50 correct on the scheduled denominator (92.0%) (Evidence: report.json#/results/0)
2. **observed behavior** — Recorded outcome/failure counts: {'QUERY_ERROR': 1, 'QUERY_TIMEOUT': 2} (Evidence: report.json#/results/0)
3. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=46; outcomes={'COMPLETED': 47, 'QUERY_TIMEOUT': 2, 'QUERY_ERROR': 1}. (Evidence: report.json#/question_results)
4. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/0)
5. **observed behavior** — mcp / gpt-6-luna-nous / repetition 1: 49/50 correct on the scheduled denominator (98.0%) (Evidence: report.json#/results/1)
6. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=3; correct=49; outcomes={'COMPLETED': 50}. (Evidence: report.json#/question_results)
7. **observed behavior** — Recorded provider attempt count: 53 (Evidence: report.json#/results/1)
8. **observed behavior** — mcp / gpt-6-luna-nous / repetition 1: 30/50 correct on the scheduled denominator (60.0%) (Evidence: report.json#/results/2)
9. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 50/50; missing slots=0; state=failed (Evidence: report.json#/results/2)
10. **observed behavior** — Recorded outcome/failure counts: {'INFRA_ERROR': 1} (Evidence: report.json#/results/2)
11. **hypothesis** — Infrastructure or harness conditions could contribute to these recorded outcomes; the public aggregate alone cannot distinguish that from other causes or establish model-quality effects. (Evidence: report.json#/results/2)
12. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/2)
13. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=1; correct=30; outcomes={'COMPLETED': 49, 'INFRA_ERROR': 1}. (Evidence: report.json#/question_results)
14. **observed behavior** — Recorded provider attempt count: 51 (Evidence: report.json#/results/2)
15. **observed behavior** — mcp / gpt-6-luna-nous / repetition 1: 48/50 correct on the scheduled denominator (96.0%) (Evidence: report.json#/results/3)
16. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 50/50; missing slots=0; state=failed (Evidence: report.json#/results/3)
17. **observed behavior** — Recorded outcome/failure counts: {'OUTPUT_INVALID': 1} (Evidence: report.json#/results/3)
18. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/3)
19. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=48; outcomes={'COMPLETED': 49, 'OUTPUT_INVALID': 1}. (Evidence: report.json#/question_results)
20. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/3)
21. **observed behavior** — direct / gpt-5.6-luna-nous / repetition 1: 42/50 correct on the scheduled denominator (84.0%) (Evidence: report.json#/results/4)
22. **observed behavior** — Recorded outcome/failure counts: {'QUERY_ERROR': 5} (Evidence: report.json#/results/4)
23. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=42; outcomes={'COMPLETED': 45, 'QUERY_ERROR': 5}. (Evidence: report.json#/question_results)
24. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/4)
25. **observed behavior** — mcp / gpt-5.6-luna-nous / repetition 1: 18/50 correct on the scheduled denominator (36.0%) (Evidence: report.json#/results/5)
26. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 23/50; missing slots=27; state=failed (Evidence: report.json#/results/5)
27. **observed behavior** — Recorded outcome/failure counts: {'INFRA_ERROR': 3, 'MISSING': 27, 'OUTPUT_INVALID': 1} (Evidence: report.json#/results/5)
28. **hypothesis** — Infrastructure or harness conditions could contribute to these recorded outcomes; the public aggregate alone cannot distinguish that from other causes or establish model-quality effects. (Evidence: report.json#/results/5)
29. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/5)
30. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=27; recorded extra attempts/retries=3; correct=18; outcomes={'COMPLETED': 19, 'OUTPUT_INVALID': 1, 'INFRA_ERROR': 3, 'MISSING': 27}. (Evidence: report.json#/question_results)
31. **observed behavior** — Recorded provider attempt count: 26 (Evidence: report.json#/results/5)
32. **observed behavior** — mcp / gpt-5.6-luna-nous / repetition 1: 35/50 correct on the scheduled denominator (70.0%) (Evidence: report.json#/results/6)
33. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 50/50; missing slots=0; state=failed (Evidence: report.json#/results/6)
34. **observed behavior** — Recorded outcome/failure counts: {'INFRA_ERROR': 1, 'OUTPUT_INVALID': 1} (Evidence: report.json#/results/6)
35. **hypothesis** — Infrastructure or harness conditions could contribute to these recorded outcomes; the public aggregate alone cannot distinguish that from other causes or establish model-quality effects. (Evidence: report.json#/results/6)
36. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/6)
37. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=35; outcomes={'COMPLETED': 48, 'OUTPUT_INVALID': 1, 'INFRA_ERROR': 1}. (Evidence: report.json#/question_results)
38. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/6)
39. **observed behavior** — mcp / gpt-5.6-luna-nous / repetition 1: 44/50 correct on the scheduled denominator (88.0%) (Evidence: report.json#/results/7)
40. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 50/50; missing slots=0; state=failed (Evidence: report.json#/results/7)
41. **observed behavior** — Recorded outcome/failure counts: {'INFRA_ERROR': 1, 'OUTPUT_INVALID': 2} (Evidence: report.json#/results/7)
42. **hypothesis** — Infrastructure or harness conditions could contribute to these recorded outcomes; the public aggregate alone cannot distinguish that from other causes or establish model-quality effects. (Evidence: report.json#/results/7)
43. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/7)
44. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=3; correct=44; outcomes={'COMPLETED': 47, 'OUTPUT_INVALID': 2, 'INFRA_ERROR': 1}. (Evidence: report.json#/question_results)
45. **observed behavior** — Recorded provider attempt count: 53 (Evidence: report.json#/results/7)

## Comparisons

- `../runs/seed67-qwen38flash-gpt6luna-recovery-20261002` vs `../runs/seed67-step1-six-models-3rep-3mcp-20260930`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-qwen38flash-gpt6luna-recovery-20261002` vs `../runs/deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-qwen38flash-gpt6luna-recovery-20261002` vs `../runs/luna-nous-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-qwen38flash-gpt6luna-recovery-20261002` vs `../runs/glm53flash-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-qwen38flash-gpt6luna-recovery-20261002` vs `../runs/shared-matrix-seed67-bloodhound-nous-codex-20260928`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-qwen38flash-gpt6luna-recovery-20261002` vs `../runs/qwen3.8-json-rerun-2`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-step1-six-models-3rep-3mcp-20260930` vs `../runs/deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-step1-six-models-3rep-3mcp-20260930` vs `../runs/luna-nous-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-step1-six-models-3rep-3mcp-20260930` vs `../runs/glm53flash-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-step1-six-models-3rep-3mcp-20260930` vs `../runs/shared-matrix-seed67-bloodhound-nous-codex-20260928`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-step1-six-models-3rep-3mcp-20260930` vs `../runs/qwen3.8-json-rerun-2`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929` vs `../runs/luna-nous-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929` vs `../runs/glm53flash-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable
- `../runs/deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929` vs `../runs/shared-matrix-seed67-bloodhound-nous-codex-20260928`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929` vs `../runs/qwen3.8-json-rerun-2`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/luna-nous-shared-matrix-seed67-3mcp-20260929` vs `../runs/glm53flash-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/luna-nous-shared-matrix-seed67-3mcp-20260929` vs `../runs/shared-matrix-seed67-bloodhound-nous-codex-20260928`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/luna-nous-shared-matrix-seed67-3mcp-20260929` vs `../runs/qwen3.8-json-rerun-2`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/glm53flash-shared-matrix-seed67-3mcp-20260929` vs `../runs/shared-matrix-seed67-bloodhound-nous-codex-20260928`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/glm53flash-shared-matrix-seed67-3mcp-20260929` vs `../runs/qwen3.8-json-rerun-2`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/shared-matrix-seed67-bloodhound-nous-codex-20260928` vs `../runs/qwen3.8-json-rerun-2`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ


---

# ORI offline analysis

Source run: `../runs/glm53flash-shared-matrix-seed67-3mcp-20260929`

Source integrity: **structural-public-projection-only** (not a cryptographic attestation).
Benchmark completion: **partial**.
Analysis coverage: public aggregate report only; task evidence not independently revalidated.
Publication status: **not published**.

## Findings

1. **observed behavior** — direct / glm-5.3-flash-nous / repetition 1: 39/50 correct on the scheduled denominator (78.0%) (Evidence: report.json#/results/0)
2. **observed behavior** — Recorded outcome/failure counts: {'OUTPUT_INVALID': 7, 'QUERY_ERROR': 2} (Evidence: report.json#/results/0)
3. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=39; outcomes={'OUTPUT_INVALID': 7, 'COMPLETED': 41, 'QUERY_ERROR': 2}. (Evidence: report.json#/question_results)
4. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/0)
5. **observed behavior** — mcp / glm-5.3-flash-nous / repetition 1: 28/50 correct on the scheduled denominator (56.0%) (Evidence: report.json#/results/1)
6. **observed behavior** — Recorded outcome/failure counts: {'OUTPUT_INVALID': 6} (Evidence: report.json#/results/1)
7. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=28; outcomes={'COMPLETED': 44, 'OUTPUT_INVALID': 6}. (Evidence: report.json#/question_results)
8. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/1)
9. **observed behavior** — mcp / glm-5.3-flash-nous / repetition 1: 16/50 correct on the scheduled denominator (32.0%) (Evidence: report.json#/results/2)
10. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 50/50; missing slots=0; state=failed (Evidence: report.json#/results/2)
11. **observed behavior** — Recorded outcome/failure counts: {'INFRA_ERROR': 2, 'OUTPUT_INVALID': 6} (Evidence: report.json#/results/2)
12. **hypothesis** — Infrastructure or harness conditions could contribute to these recorded outcomes; the public aggregate alone cannot distinguish that from other causes or establish model-quality effects. (Evidence: report.json#/results/2)
13. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/2)
14. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=16; outcomes={'COMPLETED': 42, 'INFRA_ERROR': 2, 'OUTPUT_INVALID': 6}. (Evidence: report.json#/question_results)
15. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/2)
16. **observed behavior** — mcp / glm-5.3-flash-nous / repetition 1: 31/50 correct on the scheduled denominator (62.0%) (Evidence: report.json#/results/3)
17. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 50/50; missing slots=0; state=failed (Evidence: report.json#/results/3)
18. **observed behavior** — Recorded outcome/failure counts: {'OUTPUT_INVALID': 3} (Evidence: report.json#/results/3)
19. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/3)
20. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=31; outcomes={'COMPLETED': 47, 'OUTPUT_INVALID': 3}. (Evidence: report.json#/question_results)
21. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/3)

## Comparisons

- `../runs/seed67-qwen38flash-gpt6luna-recovery-20261002` vs `../runs/seed67-step1-six-models-3rep-3mcp-20260930`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-qwen38flash-gpt6luna-recovery-20261002` vs `../runs/deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-qwen38flash-gpt6luna-recovery-20261002` vs `../runs/luna-nous-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-qwen38flash-gpt6luna-recovery-20261002` vs `../runs/glm53flash-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-qwen38flash-gpt6luna-recovery-20261002` vs `../runs/shared-matrix-seed67-bloodhound-nous-codex-20260928`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-qwen38flash-gpt6luna-recovery-20261002` vs `../runs/qwen3.8-json-rerun-2`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-step1-six-models-3rep-3mcp-20260930` vs `../runs/deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-step1-six-models-3rep-3mcp-20260930` vs `../runs/luna-nous-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-step1-six-models-3rep-3mcp-20260930` vs `../runs/glm53flash-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-step1-six-models-3rep-3mcp-20260930` vs `../runs/shared-matrix-seed67-bloodhound-nous-codex-20260928`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-step1-six-models-3rep-3mcp-20260930` vs `../runs/qwen3.8-json-rerun-2`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929` vs `../runs/luna-nous-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929` vs `../runs/glm53flash-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable
- `../runs/deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929` vs `../runs/shared-matrix-seed67-bloodhound-nous-codex-20260928`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929` vs `../runs/qwen3.8-json-rerun-2`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/luna-nous-shared-matrix-seed67-3mcp-20260929` vs `../runs/glm53flash-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/luna-nous-shared-matrix-seed67-3mcp-20260929` vs `../runs/shared-matrix-seed67-bloodhound-nous-codex-20260928`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/luna-nous-shared-matrix-seed67-3mcp-20260929` vs `../runs/qwen3.8-json-rerun-2`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/glm53flash-shared-matrix-seed67-3mcp-20260929` vs `../runs/shared-matrix-seed67-bloodhound-nous-codex-20260928`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/glm53flash-shared-matrix-seed67-3mcp-20260929` vs `../runs/qwen3.8-json-rerun-2`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/shared-matrix-seed67-bloodhound-nous-codex-20260928` vs `../runs/qwen3.8-json-rerun-2`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ


---

# ORI offline analysis

Source run: `../runs/shared-matrix-seed67-bloodhound-nous-codex-20260928`

Source integrity: **structural-public-projection-only** (not a cryptographic attestation).
Benchmark completion: **partial**.
Analysis coverage: public aggregate report only; task evidence not independently revalidated.
Publication status: **not published**.

## Findings

1. **observed behavior** — direct / glm-5.3-flash-nous / repetition 1: 44/50 correct on the scheduled denominator (88.0%) (Evidence: report.json#/results/0)
2. **observed behavior** — Recorded outcome/failure counts: {'OUTPUT_INVALID': 2, 'QUERY_ERROR': 3, 'QUERY_TIMEOUT': 1} (Evidence: report.json#/results/0)
3. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=44; outcomes={'COMPLETED': 44, 'OUTPUT_INVALID': 2, 'QUERY_TIMEOUT': 1, 'QUERY_ERROR': 3}. (Evidence: report.json#/question_results)
4. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/0)
5. **observed behavior** — mcp / glm-5.3-flash-nous / repetition 1: 26/50 correct on the scheduled denominator (52.0%) (Evidence: report.json#/results/1)
6. **observed behavior** — Recorded outcome/failure counts: {'OUTPUT_INVALID': 7} (Evidence: report.json#/results/1)
7. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=26; outcomes={'COMPLETED': 43, 'OUTPUT_INVALID': 7}. (Evidence: report.json#/question_results)
8. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/1)
9. **observed behavior** — direct / qwen3.8-flash-nous / repetition 1: 31/50 correct on the scheduled denominator (62.0%) (Evidence: report.json#/results/2)
10. **observed behavior** — Recorded outcome/failure counts: {'OUTPUT_INVALID': 11, 'QUERY_ERROR': 6} (Evidence: report.json#/results/2)
11. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=31; outcomes={'COMPLETED': 33, 'OUTPUT_INVALID': 11, 'QUERY_ERROR': 6}. (Evidence: report.json#/question_results)
12. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/2)
13. **observed behavior** — mcp / qwen3.8-flash-nous / repetition 1: 24/50 correct on the scheduled denominator (48.0%) (Evidence: report.json#/results/3)
14. **observed behavior** — Recorded outcome/failure counts: {'OUTPUT_INVALID': 6} (Evidence: report.json#/results/3)
15. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=24; outcomes={'COMPLETED': 44, 'OUTPUT_INVALID': 6}. (Evidence: report.json#/question_results)
16. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/3)
17. **observed behavior** — direct / gpt-6-luna / repetition 1: 0/50 correct on the scheduled denominator (0.0%) (Evidence: report.json#/results/4)
18. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 3/50; missing slots=47; state=failed (Evidence: report.json#/results/4)
19. **observed behavior** — Recorded outcome/failure counts: {'INFRA_ERROR': 3, 'MISSING': 47} (Evidence: report.json#/results/4)
20. **hypothesis** — Infrastructure or harness conditions could contribute to these recorded outcomes; the public aggregate alone cannot distinguish that from other causes or establish model-quality effects. (Evidence: report.json#/results/4)
21. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/4)
22. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=47; recorded extra attempts/retries=0; correct=0; outcomes={'INFRA_ERROR': 3, 'MISSING': 47}. (Evidence: report.json#/question_results)
23. **observed behavior** — Recorded provider attempt count: 3 (Evidence: report.json#/results/4)
24. **observed behavior** — mcp / gpt-6-luna / repetition 1: 0/50 correct on the scheduled denominator (0.0%) (Evidence: report.json#/results/5)
25. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 3/50; missing slots=47; state=failed (Evidence: report.json#/results/5)
26. **observed behavior** — Recorded outcome/failure counts: {'INFRA_ERROR': 3, 'MISSING': 47} (Evidence: report.json#/results/5)
27. **hypothesis** — Infrastructure or harness conditions could contribute to these recorded outcomes; the public aggregate alone cannot distinguish that from other causes or establish model-quality effects. (Evidence: report.json#/results/5)
28. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/5)
29. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=47; recorded extra attempts/retries=0; correct=0; outcomes={'INFRA_ERROR': 3, 'MISSING': 47}. (Evidence: report.json#/question_results)
30. **observed behavior** — Recorded provider attempt count: 3 (Evidence: report.json#/results/5)
31. **observed behavior** — direct / gpt-5.6-luna / repetition 1: 0/50 correct on the scheduled denominator (0.0%) (Evidence: report.json#/results/6)
32. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 3/50; missing slots=47; state=failed (Evidence: report.json#/results/6)
33. **observed behavior** — Recorded outcome/failure counts: {'INFRA_ERROR': 3, 'MISSING': 47} (Evidence: report.json#/results/6)
34. **hypothesis** — Infrastructure or harness conditions could contribute to these recorded outcomes; the public aggregate alone cannot distinguish that from other causes or establish model-quality effects. (Evidence: report.json#/results/6)
35. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/6)
36. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=47; recorded extra attempts/retries=0; correct=0; outcomes={'INFRA_ERROR': 3, 'MISSING': 47}. (Evidence: report.json#/question_results)
37. **observed behavior** — Recorded provider attempt count: 3 (Evidence: report.json#/results/6)
38. **observed behavior** — mcp / gpt-5.6-luna / repetition 1: 0/50 correct on the scheduled denominator (0.0%) (Evidence: report.json#/results/7)
39. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 3/50; missing slots=47; state=failed (Evidence: report.json#/results/7)
40. **observed behavior** — Recorded outcome/failure counts: {'INFRA_ERROR': 3, 'MISSING': 47} (Evidence: report.json#/results/7)
41. **hypothesis** — Infrastructure or harness conditions could contribute to these recorded outcomes; the public aggregate alone cannot distinguish that from other causes or establish model-quality effects. (Evidence: report.json#/results/7)
42. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/7)
43. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=47; recorded extra attempts/retries=0; correct=0; outcomes={'INFRA_ERROR': 3, 'MISSING': 47}. (Evidence: report.json#/question_results)
44. **observed behavior** — Recorded provider attempt count: 3 (Evidence: report.json#/results/7)

## Comparisons

- `../runs/seed67-qwen38flash-gpt6luna-recovery-20261002` vs `../runs/seed67-step1-six-models-3rep-3mcp-20260930`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-qwen38flash-gpt6luna-recovery-20261002` vs `../runs/deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-qwen38flash-gpt6luna-recovery-20261002` vs `../runs/luna-nous-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-qwen38flash-gpt6luna-recovery-20261002` vs `../runs/glm53flash-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-qwen38flash-gpt6luna-recovery-20261002` vs `../runs/shared-matrix-seed67-bloodhound-nous-codex-20260928`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-qwen38flash-gpt6luna-recovery-20261002` vs `../runs/qwen3.8-json-rerun-2`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-step1-six-models-3rep-3mcp-20260930` vs `../runs/deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-step1-six-models-3rep-3mcp-20260930` vs `../runs/luna-nous-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-step1-six-models-3rep-3mcp-20260930` vs `../runs/glm53flash-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-step1-six-models-3rep-3mcp-20260930` vs `../runs/shared-matrix-seed67-bloodhound-nous-codex-20260928`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-step1-six-models-3rep-3mcp-20260930` vs `../runs/qwen3.8-json-rerun-2`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929` vs `../runs/luna-nous-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929` vs `../runs/glm53flash-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable
- `../runs/deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929` vs `../runs/shared-matrix-seed67-bloodhound-nous-codex-20260928`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929` vs `../runs/qwen3.8-json-rerun-2`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/luna-nous-shared-matrix-seed67-3mcp-20260929` vs `../runs/glm53flash-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/luna-nous-shared-matrix-seed67-3mcp-20260929` vs `../runs/shared-matrix-seed67-bloodhound-nous-codex-20260928`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/luna-nous-shared-matrix-seed67-3mcp-20260929` vs `../runs/qwen3.8-json-rerun-2`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/glm53flash-shared-matrix-seed67-3mcp-20260929` vs `../runs/shared-matrix-seed67-bloodhound-nous-codex-20260928`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/glm53flash-shared-matrix-seed67-3mcp-20260929` vs `../runs/qwen3.8-json-rerun-2`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/shared-matrix-seed67-bloodhound-nous-codex-20260928` vs `../runs/qwen3.8-json-rerun-2`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ


---

# ORI offline analysis

Source run: `../runs/qwen3.8-json-rerun-2`

Source integrity: **structural-public-projection-only** (not a cryptographic attestation).
Benchmark completion: **partial**.
Analysis coverage: public aggregate report only; task evidence not independently revalidated.
Publication status: **not published**.

## Findings

1. **observed behavior** — direct / qwen3.8-27b-q4km / repetition 1: 29/50 correct on the scheduled denominator (58.0%) (Evidence: report.json#/results/0)
2. **observed behavior** — Recorded outcome/failure counts: {'OUTPUT_INVALID': 17, 'QUERY_ERROR': 2} (Evidence: report.json#/results/0)
3. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=29; outcomes={'COMPLETED': 31, 'OUTPUT_INVALID': 17, 'QUERY_ERROR': 2}. (Evidence: report.json#/question_results)
4. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/0)
5. **observed behavior** — mcp / qwen3.8-27b-q4km / repetition 1: 34/50 correct on the scheduled denominator (68.0%) (Evidence: report.json#/results/1)
6. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 50/50; missing slots=0; state=failed (Evidence: report.json#/results/1)
7. **observed behavior** — Recorded outcome/failure counts: {'INFRA_ERROR': 2, 'OUTPUT_INVALID': 4} (Evidence: report.json#/results/1)
8. **hypothesis** — Infrastructure or harness conditions could contribute to these recorded outcomes; the public aggregate alone cannot distinguish that from other causes or establish model-quality effects. (Evidence: report.json#/results/1)
9. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/1)
10. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=34; outcomes={'INFRA_ERROR': 2, 'COMPLETED': 44, 'OUTPUT_INVALID': 4}. (Evidence: report.json#/question_results)
11. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/1)
12. **observed behavior** — mcp / qwen3.8-27b-q4km / repetition 1: 2/50 correct on the scheduled denominator (4.0%) (Evidence: report.json#/results/2)
13. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 5/50; missing slots=45; state=failed (Evidence: report.json#/results/2)
14. **observed behavior** — Recorded outcome/failure counts: {'INFRA_ERROR': 3, 'MISSING': 45} (Evidence: report.json#/results/2)
15. **hypothesis** — Infrastructure or harness conditions could contribute to these recorded outcomes; the public aggregate alone cannot distinguish that from other causes or establish model-quality effects. (Evidence: report.json#/results/2)
16. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/2)
17. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=45; recorded extra attempts/retries=0; correct=2; outcomes={'COMPLETED': 2, 'INFRA_ERROR': 3, 'MISSING': 45}. (Evidence: report.json#/question_results)
18. **observed behavior** — Recorded provider attempt count: 5 (Evidence: report.json#/results/2)
19. **observed behavior** — mcp / qwen3.8-27b-q4km / repetition 1: 20/50 correct on the scheduled denominator (40.0%) (Evidence: report.json#/results/3)
20. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 50/50; missing slots=0; state=failed (Evidence: report.json#/results/3)
21. **observed behavior** — Recorded outcome/failure counts: {'INFRA_ERROR': 5, 'OUTPUT_INVALID': 7, 'TASK_TIMEOUT': 2} (Evidence: report.json#/results/3)
22. **hypothesis** — Infrastructure or harness conditions could contribute to these recorded outcomes; the public aggregate alone cannot distinguish that from other causes or establish model-quality effects. (Evidence: report.json#/results/3)
23. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/3)
24. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=20; outcomes={'OUTPUT_INVALID': 7, 'COMPLETED': 36, 'TASK_TIMEOUT': 2, 'INFRA_ERROR': 5}. (Evidence: report.json#/question_results)
25. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/3)
26. **observed behavior** — mcp / qwen3.8-27b-q4km / repetition 1: 35/50 correct on the scheduled denominator (70.0%) (Evidence: report.json#/results/4)
27. **observed behavior** — Coverage is incomplete or lifecycle is not completed: attempted 50/50; missing slots=0; state=failed (Evidence: report.json#/results/4)
28. **observed behavior** — Recorded outcome/failure counts: {'INFRA_ERROR': 1, 'OUTPUT_INVALID': 5} (Evidence: report.json#/results/4)
29. **hypothesis** — Infrastructure or harness conditions could contribute to these recorded outcomes; the public aggregate alone cannot distinguish that from other causes or establish model-quality effects. (Evidence: report.json#/results/4)
30. **supported explanation** — The report marks the campaign partial and this row records missing coverage, an incomplete flag, or a non-completed lifecycle state; this explains the partial label without implying a model-quality cause. (Evidence: report.json#/status, report.json#/results/4)
31. **observed behavior** — Public question-level coverage: 50 rows; explicitly missing=0; recorded extra attempts/retries=0; correct=35; outcomes={'COMPLETED': 44, 'OUTPUT_INVALID': 5, 'INFRA_ERROR': 1}. (Evidence: report.json#/question_results)
32. **observed behavior** — Recorded provider attempt count: 50 (Evidence: report.json#/results/4)

## Comparisons

- `../runs/seed67-qwen38flash-gpt6luna-recovery-20261002` vs `../runs/seed67-step1-six-models-3rep-3mcp-20260930`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-qwen38flash-gpt6luna-recovery-20261002` vs `../runs/deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-qwen38flash-gpt6luna-recovery-20261002` vs `../runs/luna-nous-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-qwen38flash-gpt6luna-recovery-20261002` vs `../runs/glm53flash-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-qwen38flash-gpt6luna-recovery-20261002` vs `../runs/shared-matrix-seed67-bloodhound-nous-codex-20260928`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-qwen38flash-gpt6luna-recovery-20261002` vs `../runs/qwen3.8-json-rerun-2`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-step1-six-models-3rep-3mcp-20260930` vs `../runs/deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-step1-six-models-3rep-3mcp-20260930` vs `../runs/luna-nous-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-step1-six-models-3rep-3mcp-20260930` vs `../runs/glm53flash-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-step1-six-models-3rep-3mcp-20260930` vs `../runs/shared-matrix-seed67-bloodhound-nous-codex-20260928`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/seed67-step1-six-models-3rep-3mcp-20260930` vs `../runs/qwen3.8-json-rerun-2`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929` vs `../runs/luna-nous-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929` vs `../runs/glm53flash-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable
- `../runs/deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929` vs `../runs/shared-matrix-seed67-bloodhound-nous-codex-20260928`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/deepseek-v41-flash-nous-shared-matrix-seed67-3mcp-20260929` vs `../runs/qwen3.8-json-rerun-2`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/luna-nous-shared-matrix-seed67-3mcp-20260929` vs `../runs/glm53flash-shared-matrix-seed67-3mcp-20260929`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/luna-nous-shared-matrix-seed67-3mcp-20260929` vs `../runs/shared-matrix-seed67-bloodhound-nous-codex-20260928`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/luna-nous-shared-matrix-seed67-3mcp-20260929` vs `../runs/qwen3.8-json-rerun-2`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/glm53flash-shared-matrix-seed67-3mcp-20260929` vs `../runs/shared-matrix-seed67-bloodhound-nous-codex-20260928`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/glm53flash-shared-matrix-seed67-3mcp-20260929` vs `../runs/qwen3.8-json-rerun-2`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
- `../runs/shared-matrix-seed67-bloodhound-nous-codex-20260928` vs `../runs/qwen3.8-json-rerun-2`: diagnostic only — task contract differs or is unavailable; track/repetition scheduled denominators or cohort multiplicity differ
