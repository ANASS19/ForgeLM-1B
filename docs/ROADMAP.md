# ForgeLM-1B — Research roadmap

> **Status:** Research preparation. All model parameter counts are research targets until verified.

ForgeLM-1B is an open research engineering project to design, pretrain, evaluate, and eventually serve an approximately one-billion-parameter decoder-only language model. The model size is a target, not an accomplished training run.

| Stage | Milestone | Acceptance criterion | Status |
|---|---|---|---|
| 01 | Define research requirements | Architecture candidates, token budget, context length, evaluation and compute envelope | In progress |
| 02 | Build and test model internals | Tokenizer, embeddings, normalization, attention, MLP, loss and training loop | Planned |
| 03 | Run small-scale validation | Gradient checks, convergence, reproducibility and checkpoint recovery | Planned |
| 04 | Prepare data and training systems | Licensed datasets, filtering, deduplication, sharding, profiling and monitoring | Planned |
| 05 | Train approximately 1B parameters | Run only when data quality and sufficient compute are secured | Planned |
| 06 | Evaluate and document release | Holdout metrics, inference benchmarks, failure analysis and model card | Planned |

## Definition of done

A milestone is completed only with reproducible implementation evidence, configuration, verification/test results, and where applicable hardware/data manifests, published artifacts and measured results. A proposed design or a prepared repository is not evidence of a trained model.

## Decision gates

- **Data:** legally usable source, provenance, filtering, leak checks and quality report.
- **Engineering:** independently rerunnable pipeline, numerical tests, checkpoints and monitoring.
- **Compute:** hardware access, throughput benchmark, memory plan and realistic budget.
- **Evaluation:** frozen protocols, explicit baselines, failure cases and reproducible scoring.

## Next action

Architecture candidates, token budget, context length, evaluation and compute envelope.
