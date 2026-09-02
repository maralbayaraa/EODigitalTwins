# Reference Architecture

Use this chapter to describe the technical architecture of EODigitalTwins.

```{mermaid}
flowchart LR
  A[Earth Observation Data] --> B[Data Integration]
  B --> C[Models and Simulation]
  C --> D[Digital Twin Services]
  D --> E[Applications and Decisions]
  E --> C
```

## Architecture layers

1. Data acquisition and discovery
2. Harmonization and integration
3. Models and simulation
4. APIs and platform services
5. Visualization and decision support
