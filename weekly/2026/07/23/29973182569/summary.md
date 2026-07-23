### Weekly Benchmarks

Commit: `31115d3e82208d804988dfbee91241245604e28a`
Runner: `GitHub Actions 1000000972`
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
| 667 | Intersect12 Q->P | 1048.20 | 0.997 | 414.00 | 631.20 | 0.00 | 3.00 | 5 |
| 695 | Intersect12 P->Q | 450.00 | 0.991 | 314.40 | 131.60 | 4.00 | 0.00 | 5 |
| 16 | Intersect12 Q->P | 377.00 | 0.997 | 149.20 | 226.80 | 0.00 | 1.00 | 5 |
| 84 | Intersect12 P->Q | 341.20 | 0.991 | 195.40 | 142.80 | 2.00 | 1.00 | 5 |
| 260 | Intersect12 Q->P | 154.00 | 0.973 | 68.20 | 81.60 | 1.20 | 3.00 | 5 |
| 406 | Intersect12 P->Q | 126.00 | 0.976 | 77.40 | 45.60 | 3.00 | 0.00 | 5 |
| 551 | Intersect12 P->Q | 96.80 | 0.959 | 53.60 | 39.20 | 4.00 | 0.00 | 5 |
| 582 | Intersect12 P->Q | 39.40 | 1.000 | 22.40 | 17.00 | 0.00 | 0.00 | 5 |

Note: phase timings cover `Intersect12` and `Winding03` only; `Intersections (total)` is excluded from the denominator.

#### perfTest Size Sweep

| nTri | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Peak RSS mean (MB) | Peak RSS min (MB) | Peak RSS max (MB) | Runs |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 512 | 1.25 | 1.34 | 0.81 | 1.49 | 4.75 | 4.66 | 4.84 | 5 |
| 2048 | 2.26 | 2.11 | 1.88 | 2.91 | 6.25 | 6.23 | 6.28 | 5 |
| 8192 | 5.83 | 5.61 | 4.95 | 7.82 | 11.35 | 11.31 | 11.45 | 5 |
| 32768 | 14.76 | 14.93 | 12.08 | 17.82 | 33.65 | 30.95 | 36.45 | 5 |
| 131072 | 52.72 | 49.08 | 42.51 | 68.59 | 120.60 | 113.33 | 128.69 | 5 |
| 524288 | 269.16 | 246.89 | 158.65 | 420.52 | 529.90 | 518.36 | 537.83 | 5 |
| 2097152 | 1021.46 | 845.21 | 621.91 | 2014.89 | 1984.01 | 1552.53 | 2101.59 | 5 |
| 8388608 | 11601.15 | 10789.00 | 9684.98 | 16785.20 | 4002.84 | 3251.23 | 4218.39 | 5 |

#### Existing Regression Tests

| Test | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Runs |
|---|---:|---:|---:|---:|---:|
| Manifold.DeepChainDoesNotOverflowNumLeaves | 1447.60 | 1437.00 | 1319.00 | 1641.00 | 5 |
| ExecutionContextFromMeshGL.CancelConcurrent | 46.20 | 44.00 | 43.00 | 51.00 | 5 |
| Boolean.BatchBoolean | 1.40 | 1.00 | 1.00 | 2.00 | 5 |
| CrossSection.BatchBoolean | 0.20 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Sponge4 | 0.00 | 0.00 | 0.00 | 0.00 | 5 |
| Polygon.Zebra1 | 2.00 | 2.00 | 2.00 | 2.00 | 5 |
| Polygon.Zebra3 | 775.60 | 759.00 | 747.00 | 815.00 | 5 |

