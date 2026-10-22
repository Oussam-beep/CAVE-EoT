# Literature Synthesis (Current Draft)

This synthesis follows the CAVE-EoT Research Handbook. It summarizes the currently identified literature; it is not a claim that every paper has been read in full or that the identified corpus is exhaustive.

## 1. Communication protocol is not the same as aggregation

Work on multi-agent debate and cross-model exchange studies how agents see messages, revise answers, or use selected communication patterns. This motivates separating the protocol that generates a pool of answers from the later rule that selects among that pool. A fair aggregation comparison should reuse the same recorded panel where possible.

Relevant examples in the current review include Exchange-of-Thought, vanilla multi-agent debate, Liang et al.'s dissent/judge-led debate, DySCo and DAR.

## 2. Strong aggregation and audit methods already exist

The closest literature includes answer-level reliability/dependence aggregation, learned calibration, argument graphs, reasoning-tree auditing and semantic redundancy reduction. Therefore, CAVE-EoT should not claim that majority voting is flawed in general, or that prior work ignores dependence or reasoning traces.

Relevant close comparisons documented in the handbook include DarkForest, CAGE-CAL, AgentAuditor, Ising-based label aggregation, PPV, Slim-SC and ARGORA.

## 3. Several meanings of dependence must not be conflated

A dataset-level correlation between model errors is not the same target as overlap between two support paths for a single question. Semantic similarity is also not identical to shared inference: two arguments can sound different but rely on the same premise, while two independently produced correct derivations can look similar.

The handbook discusses CAPA in *Great Models Think Alike and this Undermines AI Oversight*, effective-sample-size motivation in DAR, dependence-aware label aggregation via Ising models, and semantic-answer uncertainty as related but distinct objects.

## 4. A preliminary research opportunity

Within the current source-identifiable corpus, the review proposes investigating the combination of (a) operational reasoning/support units, (b) a task-matched no-communication overlap reference, and (c) transparent support accounting tested under controlled redundant-evidence conditions. This is a **preliminary opportunity**, not proof of global novelty. Similar ideas may exist among ambiguous entries or outside the current corpus.

The claimed distinction must be tested against simpler explanations: answer-only weighting, whole-response embeddings and uncalibrated semantic step deduplication.

## 5. What a convincing future result must show

A useful evaluation should separately establish:

1. The estimator responds appropriately to controlled shared-support mechanisms.
2. It does not wrongly penalize common but independently derived valid reasoning too often.
3. Decisions improve, or at minimum the trade-offs are clearly characterized, on a meaningful task metric.
4. Gains persist under fair baselines and transparent compute/token/latency accounting.
5. Failures can be traced to extraction, alignment, reference construction or aggregation rather than hidden in a single score.

## Evidence cautions

- The four-map handbook includes unresolved identities; their unknown cells cannot be treated as negative evidence.
- A checked mark in a literature map may describe an ablation or baseline rather than the paper's main method.
- Citation status and full-text-reading status need separate records.
- No CAVE-EoT system results are reported by the current handbook.
