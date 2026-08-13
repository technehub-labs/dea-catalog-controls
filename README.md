# dea-catalog-controls

> DEA catalog for **Control** — OpenDEAM v0.3.0 (ADR-0003).

## Control (`CTL`)

- **Entity id:** `dea:entity-control`
- **Allocation:** L2 · L2-risk-compliance
- **Status:** proposed

A mechanism (process, technical, or organizational) that mitigates a Risk or enforces a Regulation.

## Relationships (from the OpenDEAM model)

- **CTL → RSK** — mitigates (governance, 0..N:0..N)
- **REG → CTL** — mandates (governance, 1:0..N)

## Allocation contract

This repo's `metamodel-pointer.yaml` is validated in CI against the pinned
OpenDEAM root model (`v0.3.0`) via the reusable
`validate-against-model.yml` workflow. Drift fails CI.

Content (entity instances) lands when the entity promotes from
`proposed` to `planned`/`scaffold` per the model lifecycle.

## License

Apache 2.0 — see [LICENSE](./LICENSE) and [NOTICE](./NOTICE).
