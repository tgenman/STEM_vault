---
aliases:
anki: false
created: 2025-09-03 19:35
parent:
  - "[[Set (math)]]"
connected:
tags:
  - fix/empty
  - fix/linking
---


```mermaid
graph TD
  %% Узлы
  SET["Set"]
  MS["Metric space"]
  LS["Linear (vector) space"]
  NS["Normed space"]
  IP["Inner product space"]
  B["Banach space"]
  H["Hilbert space"]
  E["Euclidean space (finite-dim real IP)"]

  %% Подтип → супертип (is-a). Подписи — что добавляет подтип.
  MS -->|adds metric| SET
  LS -->|adds vector ops| SET

  NS -->|adds norm| LS
  NS -->|induces metric| MS

  IP -->|adds inner product| LS
  IP -->|gives norm| NS

  B  -->|complete in norm| NS
  H  -->|complete in inner product| IP
  H  -->|also Banach| B

  E  -->|finite dim over R| IP
  E  -->|finite dim implies complete| H

  %% Цвета
  classDef LA fill:#D4F8C4,stroke:#2E7D32,color:#111;   %% Linear Algebra
  classDef FA fill:#CFE8FF,stroke:#1565C0,color:#111;   %% Functional Analysis
  classDef TOP fill:#FFE0B2,stroke:#EF6C00,color:#111;  %% Topology / Metric
  classDef MIX fill:#E1D5FF,stroke:#5E35B1,color:#111;  %% Overlap / Boundary

  class LS,IP,E MIX;
  class NS,B,H FA;
  class SET,MS TOP;

```

Normed space
Inner product space
Banach space (complete normed)
Hilbert space (complete inner product)
Euclidean space
Metric space