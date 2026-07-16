### Weekly Benchmarks

Commit: `31115d3e82208d804988dfbee91241245604e28a`
Runner: `GitHub Actions 1000000834`
OS: `macOS`
Compiler: `AppleClang 17.0.0.17000013`
CPU: `Apple M1 (Virtual)`
CPU count: `3`
CPU model identifier: `VirtualMac2,1`
CPU physical cores: `3`
CPU performance cores: `3`
Repeats: `5`

#### Ember Phase Timings

| Case | Dominant phase | Full mean (ms) | Intersect12 share | P->Q | Q->P | Winding P | Winding Q | Runs |
|---:|---|---:|---:|---:|---:|---:|---:|---:|
| 667 | Intersect12 Q->P | 1359.40 | 0.998 | 557.80 | 798.40 | 0.00 | 3.20 | 5 |
| 16 | Intersect12 Q->P | 591.80 | 0.998 | 222.20 | 368.60 | 0.00 | 1.00 | 5 |
| 695 | Intersect12 P->Q | 581.80 | 0.986 | 406.40 | 167.00 | 8.40 | 0.00 | 5 |
| 84 | Intersect12 P->Q | 475.20 | 0.989 | 252.40 | 217.40 | 4.20 | 1.20 | 5 |
| 260 | Intersect12 Q->P | 200.40 | 0.971 | 90.00 | 104.60 | 2.00 | 3.80 | 5 |
| 406 | Intersect12 P->Q | 163.20 | 0.978 | 95.00 | 64.60 | 3.60 | 0.00 | 5 |
| 551 | Intersect12 P->Q | 125.60 | 0.963 | 67.40 | 53.60 | 4.60 | 0.00 | 5 |
| 582 | Intersect12 P->Q | 45.60 | 0.996 | 26.60 | 18.80 | 0.20 | 0.00 | 5 |

Note: phase timings cover `Intersect12` and `Winding03` only; `Intersections (total)` is excluded from the denominator.

#### perfTest Size Sweep

| nTri | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Peak RSS mean (MB) | Peak RSS min (MB) | Peak RSS max (MB) | Runs |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 512 | 1.58 | 1.20 | 1.00 | 2.46 | 4.75 | 4.53 | 4.98 | 5 |
| 2048 | 2.55 | 2.46 | 2.23 | 3.06 | 6.44 | 6.25 | 7.00 | 5 |
| 8192 | 10.33 | 7.20 | 6.34 | 15.60 | 12.31 | 11.30 | 13.72 | 5 |
| 32768 | 27.98 | 18.56 | 16.68 | 51.73 | 35.85 | 32.30 | 37.98 | 5 |
| 131072 | 144.34 | 159.80 | 87.30 | 208.06 | 125.17 | 121.38 | 132.84 | 5 |
| 524288 | 560.46 | 590.67 | 424.54 | 621.26 | 529.27 | 522.89 | 539.75 | 5 |
| 2097152 | 1776.29 | 1687.16 | 1498.31 | 2294.34 | 2023.15 | 1795.78 | 2097.25 | 5 |
| 8388608 | 18813.92 | 16248.10 | 15735.80 | 26808.80 | 3723.07 | 3178.20 | 4037.84 | 5 |

#### Existing Regression Tests

| Test | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Runs |
|---|---:|---:|---:|---:|---:|
| Manifold.DeepChainDoesNotOverflowNumLeaves | 2843.00 | 2739.00 | 2641.00 | 3142.00 | 5 |
| ExecutionContextFromMeshGL.CancelConcurrent | 131.00 | 117.00 | 76.00 | 196.00 | 5 |
| Boolean.BatchBoolean | 3.80 | 2.00 | 2.00 | 9.00 | 5 |
| CrossSection.BatchBoolean | 0.20 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Sponge4 | 1.40 | 1.00 | 1.00 | 2.00 | 5 |
| Polygon.Zebra1 | 3.60 | 4.00 | 2.00 | 6.00 | 5 |
| Polygon.Zebra3 | 1305.20 | 1321.00 | 1084.00 | 1519.00 | 5 |

