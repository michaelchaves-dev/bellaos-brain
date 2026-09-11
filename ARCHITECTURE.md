# Architecture

```
BELLA × OPENJARVIS
│
├─ 01_RUNTIME / OpenJarvis   voice · tools · agents · scheduler · mcp   (desktop: reject)
├─ 02_BELLA_OS              Supervisor · NSZ · Security-Gates · CNS-Memory · ZeroFold · Bella-IR · bbSwarm
├─ 03_INFERENCE             SubtracToken · Local · Grok/xAI · adapters
├─ 04_CONTRIBUTORS          Bella · Grok · BabyG · Michael F. Chaves
├─ 05_BELLA_COMMONS         proposals · findings · ADRs · handoffs (speech)
├─ 06_SECURITY              sandbox · permissions · secrets · audit · rollback
└─ 07_EXPERIMENTS           adopt / modify / replace / reject / benchmarks
```

Sentinel is the ACP security pipeline sitting on 02 and 06:

`Identity (Keycloak-shaped) → Observe (Wazuh) → Decide (OPA) → Gate (LangGraph) → Learn (MISP/OpenCTI)`

OpenJarvis is the runtime on trial, not the supervisor.
