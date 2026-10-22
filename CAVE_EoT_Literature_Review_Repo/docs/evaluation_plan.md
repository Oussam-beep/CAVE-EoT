# Evaluation Plan (Proposed; Not Yet Run)

## Experimental tracks

### Track A — Controlled mechanism tests

Build controlled panels where the support-generation mechanism is known. Include at least:

- Exact repetition of a decisive step.
- Semantic paraphrase of the same premise.
- Partial overlap with some genuinely distinct support.
- Independent repetition of a canonical valid derivation.
- Distinct but irrelevant reasoning that should not earn extra support.

The central question is whether the overlap statistic distinguishes excess sharing from honest/common reasoning. Textual similarity alone is not ground truth for copying.

### Track B — Task performance and aggregation

Replay identical recorded answers/messages through multiple post-hoc rules where possible. Candidate comparators from the handbook include:

- Majority vote.
- Confidence-weighted aggregation.
- Frozen LLM judge.
- Whole-response embedding or semantic-answer clustering.
- Uncalibrated semantic step deduplication.
- Proposed CAVE-EoT support adjustment, once specified and implemented.

An end-to-end debate comparison can be added later, but should not replace the paired replay experiment because different generated candidate pools confound the aggregation effect.

## Metrics to predefine

### Decision quality

- Task accuracy or the appropriate task outcome metric.
- Correct-majority preservation.
- Correct-minority recovery.
- Helpful versus harmful decision flips and flip precision.
- Coverage and accepted-answer risk if abstention is used.

### Dependence target

- Detection rate for known shared support.
- False positives on independently repeated canonical reasoning.
- False negatives on paraphrased shared assumptions.
- Agreement between automatically extracted structure and a human-inspected subset.

### Cost and stability

- Input/output tokens for generation, extraction, reference generation, judging and verification.
- Wall-clock latency and relevant memory/compute usage.
- Variation across seeds and paired uncertainty on question-level results.

## Fairness controls

- Compare methods on the same recorded candidate pool for post-hoc aggregation.
- State whether any component is trained, fitted, tuned or supervised.
- Separate development/threshold selection from test evaluation.
- Record model versions, prompts, sampling settings, dataset versions and failures.
- Report the resource cost of the no-communication reference instead of hiding it.

## Current results

No CAVE-EoT experiments have been run or reported in this repository. Metrics above are proposed evaluation criteria, not measured outcomes.
