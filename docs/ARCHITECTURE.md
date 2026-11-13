# ForgeLM-1B — Architecture notes

## Working assumption

Decoder-only autoregressive Transformer as an initial design candidate. Exact parameter count, vocabulary, width, layers, heads, feed-forward expansion, normalization, position encoding and context length will be decided experimentally. All assumptions must be captured in version-controlled configuration.

## Open decisions

- Model parameter budget, vocabulary, context length and representation dimensions (when applicable).
- Data composition, quality/contamination checks, provenance and licenses.
- Training objectives, optimizer, precision, batching, efficiency and stopping criteria.
- Hardware topology, checkpoint format, artifact lifecycle and reproducibility.
- Evaluation protocols, base model comparisons and safe release criteria.

## Engineering standards

Changes should include shape and numerical tests where relevant, explicit configuration, deterministic small tests, monitored training behavior, checkpoint recovery, and failure analysis. No architecture is described as final until experiments establish it.

## Tracking

See [decision log](DECISIONS.md) and [experiments](EXPERIMENTS.md).
