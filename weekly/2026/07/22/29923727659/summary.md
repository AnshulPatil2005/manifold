### Weekly Benchmarks

Commit: `31115d3e82208d804988dfbee91241245604e28a`
Runner: `GitHub Actions 1000000959`
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
| 667 | Intersect12 Q->P | 1187.60 | 0.997 | 476.60 | 707.20 | 0.00 | 3.80 | 5 |
| 695 | Intersect12 P->Q | 501.20 | 0.990 | 343.60 | 152.60 | 5.00 | 0.00 | 5 |
| 16 | Intersect12 Q->P | 445.80 | 0.998 | 174.20 | 270.60 | 0.00 | 1.00 | 5 |
| 84 | Intersect12 P->Q | 391.20 | 0.991 | 224.80 | 162.80 | 2.60 | 1.00 | 5 |
| 260 | Intersect12 Q->P | 178.00 | 0.970 | 75.00 | 97.60 | 2.00 | 3.40 | 5 |
| 406 | Intersect12 P->Q | 148.20 | 0.974 | 88.20 | 56.20 | 3.80 | 0.00 | 5 |
| 551 | Intersect12 P->Q | 113.00 | 0.963 | 63.60 | 45.20 | 4.20 | 0.00 | 5 |
| 582 | Intersect12 P->Q | 44.80 | 1.000 | 25.20 | 19.60 | 0.00 | 0.00 | 5 |

Note: phase timings cover `Intersect12` and `Winding03` only; `Intersections (total)` is excluded from the denominator.

#### perfTest Size Sweep

| nTri | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Peak RSS mean (MB) | Peak RSS min (MB) | Peak RSS max (MB) | Runs |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 512 | 1.94 | 1.99 | 0.80 | 2.99 | 4.81 | 4.80 | 4.83 | 5 |
| 2048 | 2.80 | 2.34 | 1.96 | 4.83 | 6.45 | 6.27 | 7.17 | 5 |
| 8192 | 8.62 | 8.26 | 5.87 | 12.29 | 11.71 | 11.28 | 12.55 | 5 |
| 32768 | 28.51 | 29.45 | 13.67 | 43.37 | 33.23 | 29.62 | 37.28 | 5 |
| 131072 | 72.29 | 66.08 | 49.36 | 117.60 | 126.17 | 108.72 | 132.16 | 5 |
| 524288 | 498.75 | 357.45 | 250.56 | 1046.83 | 527.79 | 512.89 | 541.59 | 5 |
| 2097152 | 1479.03 | 1426.36 | 743.69 | 2229.86 | 1974.22 | 1547.75 | 2098.16 | 5 |
| 8388608 | 17274.10 | 18460.00 | 13615.90 | 19615.60 | 4007.95 | 3363.44 | 4211.44 | 5 |

#### Existing Regression Tests

| Test | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Runs |
|---|---:|---:|---:|---:|---:|
| Manifold.DeepChainDoesNotOverflowNumLeaves | 2390.40 | 2278.00 | 2186.00 | 2661.00 | 5 |
| ExecutionContextFromMeshGL.CancelConcurrent | 97.60 | 97.00 | 88.00 | 112.00 | 5 |
| Boolean.BatchBoolean | 2.80 | 3.00 | 2.00 | 4.00 | 5 |
| CrossSection.BatchBoolean | 0.20 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Sponge4 | 0.60 | 1.00 | 0.00 | 1.00 | 5 |
| Polygon.Zebra1 | 2.20 | 2.00 | 2.00 | 3.00 | 5 |
| Polygon.Zebra3 | 1110.20 | 1108.00 | 1046.00 | 1149.00 | 5 |

