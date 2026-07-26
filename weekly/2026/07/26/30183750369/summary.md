### Weekly Benchmarks

Commit: `31115d3e82208d804988dfbee91241245604e28a`
Runner: `GitHub Actions 1000001031`
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
| 667 | Intersect12 Q->P | 1052.00 | 0.997 | 422.40 | 626.60 | 0.00 | 3.00 | 5 |
| 695 | Intersect12 P->Q | 437.20 | 0.991 | 306.00 | 127.20 | 4.00 | 0.00 | 5 |
| 16 | Intersect12 Q->P | 385.60 | 0.997 | 153.20 | 231.40 | 0.00 | 1.00 | 5 |
| 84 | Intersect12 P->Q | 337.80 | 0.991 | 193.40 | 141.40 | 2.00 | 1.00 | 5 |
| 260 | Intersect12 Q->P | 153.60 | 0.973 | 67.40 | 82.00 | 1.20 | 3.00 | 5 |
| 406 | Intersect12 P->Q | 125.40 | 0.976 | 77.20 | 45.20 | 3.00 | 0.00 | 5 |
| 551 | Intersect12 P->Q | 95.00 | 0.958 | 52.80 | 38.20 | 4.00 | 0.00 | 5 |
| 582 | Intersect12 P->Q | 39.00 | 1.000 | 22.00 | 17.00 | 0.00 | 0.00 | 5 |

Note: phase timings cover `Intersect12` and `Winding03` only; `Intersections (total)` is excluded from the denominator.

#### perfTest Size Sweep

| nTri | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Peak RSS mean (MB) | Peak RSS min (MB) | Peak RSS max (MB) | Runs |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 512 | 0.86 | 0.85 | 0.76 | 1.01 | 4.80 | 4.78 | 4.83 | 5 |
| 2048 | 1.95 | 1.94 | 1.84 | 2.12 | 6.27 | 6.27 | 6.28 | 5 |
| 8192 | 5.18 | 5.10 | 4.90 | 5.62 | 11.58 | 11.31 | 12.59 | 5 |
| 32768 | 12.82 | 12.34 | 11.93 | 15.22 | 32.50 | 29.62 | 37.00 | 5 |
| 131072 | 50.69 | 47.24 | 42.92 | 66.74 | 121.01 | 101.44 | 143.80 | 5 |
| 524288 | 248.53 | 207.67 | 168.28 | 403.37 | 538.92 | 532.64 | 549.92 | 5 |
| 2097152 | 978.82 | 1084.63 | 641.31 | 1352.80 | 1985.94 | 1569.48 | 2096.20 | 5 |
| 8388608 | 11443.85 | 10411.30 | 9861.98 | 14658.50 | 3852.56 | 3323.02 | 4183.98 | 5 |

#### Existing Regression Tests

| Test | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Runs |
|---|---:|---:|---:|---:|---:|
| Manifold.DeepChainDoesNotOverflowNumLeaves | 1648.40 | 1588.00 | 1315.00 | 2024.00 | 5 |
| ExecutionContextFromMeshGL.CancelConcurrent | 66.00 | 53.00 | 45.00 | 119.00 | 5 |
| Boolean.BatchBoolean | 1.40 | 1.00 | 1.00 | 2.00 | 5 |
| CrossSection.BatchBoolean | 0.20 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Sponge4 | 0.20 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Zebra1 | 2.20 | 2.00 | 2.00 | 3.00 | 5 |
| Polygon.Zebra3 | 775.80 | 754.00 | 751.00 | 858.00 | 5 |

