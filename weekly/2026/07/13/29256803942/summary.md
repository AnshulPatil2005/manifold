### Weekly Benchmarks

Commit: `31115d3e82208d804988dfbee91241245604e28a`
Runner: `GitHub Actions 1000000777`
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
| 667 | Intersect12 Q->P | 1094.40 | 0.997 | 439.60 | 651.60 | 0.00 | 3.20 | 5 |
| 695 | Intersect12 P->Q | 470.20 | 0.991 | 329.00 | 137.00 | 4.20 | 0.00 | 5 |
| 16 | Intersect12 Q->P | 431.80 | 0.998 | 171.40 | 259.40 | 0.00 | 1.00 | 5 |
| 84 | Intersect12 P->Q | 348.00 | 0.991 | 200.80 | 144.20 | 2.00 | 1.00 | 5 |
| 260 | Intersect12 Q->P | 171.20 | 0.972 | 73.00 | 93.40 | 1.40 | 3.40 | 5 |
| 406 | Intersect12 P->Q | 126.80 | 0.976 | 78.80 | 45.00 | 3.00 | 0.00 | 5 |
| 551 | Intersect12 P->Q | 105.00 | 0.962 | 60.00 | 41.00 | 4.00 | 0.00 | 5 |
| 582 | Intersect12 P->Q | 42.20 | 1.000 | 24.00 | 18.20 | 0.00 | 0.00 | 5 |

Note: phase timings cover `Intersect12` and `Winding03` only; `Intersections (total)` is excluded from the denominator.

#### perfTest Size Sweep

| nTri | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Peak RSS mean (MB) | Peak RSS min (MB) | Peak RSS max (MB) | Runs |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 512 | 1.08 | 0.98 | 0.88 | 1.53 | 4.78 | 4.64 | 4.83 | 5 |
| 2048 | 2.32 | 2.18 | 1.96 | 3.16 | 6.18 | 5.97 | 6.27 | 5 |
| 8192 | 5.90 | 5.35 | 5.05 | 7.93 | 11.77 | 11.33 | 13.34 | 5 |
| 32768 | 15.87 | 13.55 | 12.56 | 25.28 | 32.80 | 29.66 | 35.62 | 5 |
| 131072 | 58.55 | 47.70 | 44.85 | 99.39 | 123.73 | 112.94 | 129.17 | 5 |
| 524288 | 305.61 | 260.99 | 161.28 | 599.51 | 528.50 | 521.55 | 543.66 | 5 |
| 2097152 | 1080.73 | 979.19 | 768.71 | 1823.14 | 1953.70 | 1467.61 | 2085.22 | 5 |
| 8388608 | 13592.46 | 12190.30 | 11378.30 | 20380.90 | 3854.71 | 2990.75 | 4164.17 | 5 |

#### Existing Regression Tests

| Test | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Runs |
|---|---:|---:|---:|---:|---:|
| Manifold.DeepChainDoesNotOverflowNumLeaves | 1809.80 | 1847.00 | 1690.00 | 1905.00 | 5 |
| ExecutionContextFromMeshGL.CancelConcurrent | 64.40 | 61.00 | 60.00 | 75.00 | 5 |
| Boolean.BatchBoolean | 1.60 | 1.00 | 1.00 | 3.00 | 5 |
| CrossSection.BatchBoolean | 0.20 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Sponge4 | 0.20 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Zebra1 | 2.00 | 2.00 | 2.00 | 2.00 | 5 |
| Polygon.Zebra3 | 853.80 | 812.00 | 790.00 | 1016.00 | 5 |

