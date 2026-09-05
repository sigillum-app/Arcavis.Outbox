# Arcavis.Outbox

A provider-independent Outbox library for .NET applications.

Arcavis.Outbox separates the Outbox abstraction from its persistence
implementation, allowing different storage providers to be used without
coupling application code to a specific database technology.

## Packages

- `Arcavis.Outbox.Abstraction` — Core Outbox contracts and abstractions.
- `Arcavis.Outbox.Mongo` — MongoDB implementation.
- `Arcavis.Outbox.PostgreSql` — PostgreSQL implementation.
- `Arcavis.Outbox.Oracle` — Oracle implementation.

Provider implementations are maintained as separate packages and can be
built and published independently.

## Design

```text
Arcavis.Outbox.Abstraction
│
├── Arcavis.Outbox.Mongo
├── Arcavis.Outbox.PostgreSql
└── Arcavis.Outbox.Oracle

The abstraction package is provider-independent and does not require a
specific database technology.
```

## Status

Work in progress.

The API may change before the first stable release.