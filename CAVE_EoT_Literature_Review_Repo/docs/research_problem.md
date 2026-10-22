# Research Problem and Terminology

## Problem statement

Multi-agent LLM systems may produce several answers and supporting traces. Aggregation commonly counts final answers, confidence, reliability estimates or judge decisions. These signals do not necessarily reveal whether supporting reasoning paths provide distinct evidence or repeat a shared premise.

CAVE-EoT studies whether observable overlap between supporting derivations can be compared with an appropriate no-communication reference and then used as one signal in answer aggregation.

## Working research question

Can per-question derivation-level overlap relative to a matched no-communication reference improve dependence-sensitive aggregation beyond answer-only and uncalibrated semantic-redundancy baselines, under controlled redundant-evidence conditions and comparable budgets?

## Terms that must remain distinct

- **Agreement:** multiple agents produce the same answer or compatible outputs.
- **Correctness:** an answer or inference matches the task's ground truth or validity criterion.
- **Generation independence:** agents generate without exposure to each other's current outputs.
- **Error independence:** correctness events do not depend on one another under specified conditions.
- **Evidence-source independence:** support does not rely on the same source or upstream assumption.
- **Derivation independence:** supporting paths differ in meaningful inference or decisive evidence, not merely wording.
- **Excess overlap:** an operational comparison between observed support overlap and overlap expected in a matched reference. It is not proof of copying.

## Why a no-communication reference matters

Honest solvers may use the same formula, definition or canonical proof. Penalizing all similarity would create false positives. Conversely, paraphrases may conceal reuse of the same decisive assumption. The reference must therefore be matched to the question, model mixture, prompts, sampling and relevant budget conditions.

## Scope boundaries

The project does not assume all debate hurts, that disagreement implies useful diversity, or that text alone reveals hidden causal provenance. It also does not assume that a scalar overlap score is automatically a calibrated probability. These are empirical and methodological questions to investigate.
