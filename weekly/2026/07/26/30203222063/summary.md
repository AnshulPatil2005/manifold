### Weekly Benchmarks

Commit: `31115d3e82208d804988dfbee91241245604e28a`
Runner: `GitHub Actions 1000001038`
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
| 667 | Intersect12 Q->P | 1034.00 | 0.997 | 412.60 | 618.20 | 0.00 | 3.20 | 5 |
| 695 | Intersect12 P->Q | 439.20 | 0.991 | 307.20 | 128.00 | 4.00 | 0.00 | 5 |
| 16 | Intersect12 Q->P | 389.40 | 0.997 | 152.00 | 236.40 | 0.00 | 1.00 | 5 |
| 84 | Intersect12 P->Q | 350.20 | 0.991 | 201.20 | 146.00 | 2.00 | 1.00 | 5 |
| 260 | Intersect12 Q->P | 155.60 | 0.972 | 68.40 | 82.80 | 1.40 | 3.00 | 5 |
| 406 | Intersect12 P->Q | 127.60 | 0.976 | 78.60 | 46.00 | 3.00 | 0.00 | 5 |
| 551 | Intersect12 P->Q | 98.80 | 0.959 | 55.20 | 39.60 | 4.00 | 0.00 | 5 |
| 582 | Intersect12 P->Q | 40.20 | 1.000 | 22.80 | 17.40 | 0.00 | 0.00 | 5 |

Note: phase timings cover `Intersect12` and `Winding03` only; `Intersections (total)` is excluded from the denominator.

#### perfTest Size Sweep

| nTri | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Peak RSS mean (MB) | Peak RSS min (MB) | Peak RSS max (MB) | Runs |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 512 | 0.80 | 0.79 | 0.76 | 0.86 | 4.76 | 4.62 | 4.80 | 5 |
| 2048 | 1.95 | 1.87 | 1.83 | 2.23 | 6.16 | 5.81 | 6.27 | 5 |
| 8192 | 5.08 | 4.95 | 4.93 | 5.62 | 11.28 | 11.14 | 11.33 | 5 |
| 32768 | 12.68 | 12.25 | 11.72 | 15.27 | 32.24 | 29.66 | 37.09 | 5 |
| 131072 | 44.81 | 42.85 | 41.45 | 54.42 | 128.83 | 120.59 | 142.47 | 5 |
| 524288 | 186.66 | 182.40 | 155.47 | 238.27 | 532.99 | 524.77 | 541.39 | 5 |
| 2097152 | 785.93 | 684.68 | 617.21 | 1070.42 | 2019.61 | 1699.52 | 2127.72 | 5 |
| 8388608 | 10420.29 | 10070.50 | 9105.34 | 12264.60 | 3905.54 | 3278.28 | 4156.92 | 5 |

#### Existing Regression Tests

| Test | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Runs |
|---|---:|---:|---:|---:|---:|
| Manifold.DeepChainDoesNotOverflowNumLeaves | 1359.80 | 1363.00 | 1308.00 | 1406.00 | 5 |
| ExecutionContextFromMeshGL.CancelConcurrent | 45.80 | 46.00 | 44.00 | 49.00 | 5 |
| Boolean.BatchBoolean | 1.20 | 1.00 | 1.00 | 2.00 | 5 |
| CrossSection.BatchBoolean | 0.20 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Sponge4 | 0.20 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Zebra1 | 2.00 | 2.00 | 2.00 | 2.00 | 5 |
| Polygon.Zebra3 | 762.00 | 759.00 | 749.00 | 791.00 | 5 |

