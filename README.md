# dea-catalog-tenets

> DEA catalog for **Tenet** — OpenDEAM v0.4.0 (ADR-0004; renamed from `dea-catalog-principles`).

## Tenet (`TNT`)

- **Entity id:** `dea:entity-tenet`
- **Allocation:** L2 · L2-rules-guidance
- **Status:** planned

A non-binding, human-authored belief that guides decisions (e.g. API-first,
prefer managed services). Informs one or more Guardrails; enforces nothing on
its own. Renamed from **Principle** in v0.4.0 (ADR-0004 D3).

## Relationships (from the OpenDEAM model)

- **TNT → GRD** — informs (dependency, 0..N:0..N)
- **KA → TNT** — informs (dependency, 0..N:0..N)

## Allocation contract

This repo's `metamodel-pointer.yaml` is validated in CI against the pinned
OpenDEAM root model (`v0.4.0`) via the reusable
`validate-against-model.yml` workflow. Drift fails CI.

Content (entity instances) lands when the entity promotes from
`planned` to `scaffold` per the model lifecycle.

## License

Apache 2.0 — see [LICENSE](./LICENSE) and [NOTICE](./NOTICE).
