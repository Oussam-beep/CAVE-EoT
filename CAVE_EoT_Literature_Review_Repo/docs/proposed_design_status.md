# Proposed Design and Current Status

## Status

**Literature review and research design only.** The steps below are a proposed architecture described in the handbook. They are not represented as implemented components.

## Proposed modules

1. **Debate record:** preserve question, prompt/model settings, rounds, raw messages, parent-message exposure, parsed answers and token usage.
2. **Support extraction:** identify meaningful claims, premises, assumptions, conclusions, source references and original text spans.
3. **Support alignment:** retrieve candidate matches and compare logical role, assumptions, proposition and conclusion; keep uncertainty visible.
4. **Local support graph:** represent links from premises and inferences to answer-supporting paths.
5. **Matched reference:** estimate overlap for comparable solvers that did not exchange current outputs.
6. **Excess-overlap statistic:** compare observed overlap to the reference while retaining raw scores and reference spread.
7. **Support accounting:** test a bounded, inspectable way to discount repeated decisive support while preserving quality and partial overlap.
8. **Decision and diagnostics:** select or abstain under an explicit policy and preserve enough evidence to explain the result.

## Unresolved design questions

- What extraction unit is reliable enough for the first experiment?
- Which pairwise overlap statistic should be the primary measure?
- How many matched reference panels are needed, and at what compute cost?
- How should partial overlap and incompatible steps be treated?
- Which support-credit function is simple enough to audit and robust enough to test?
- Can the estimator detect paraphrased shared premises without penalizing canonical independent reasoning?

## Implementation boundary

No CAVE-EoT estimator, graph-building module or support-credit mechanism is claimed to exist yet. The immediate milestone is to complete the focused literature review and agree with the supervisor on the smallest defensible experiment before starting the implementation.
