### Weekly Benchmarks

Commit: `31115d3e82208d804988dfbee91241245604e28a`
Runner: `GitHub Actions 1000000787`
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
| 667 | Intersect12 Q->P | 1105.20 | 0.997 | 441.40 | 660.80 | 0.00 | 3.00 | 5 |
| 695 | Intersect12 P->Q | 466.00 | 0.990 | 325.20 | 136.20 | 4.60 | 0.00 | 5 |
| 16 | Intersect12 Q->P | 408.40 | 0.998 | 163.40 | 244.00 | 0.00 | 1.00 | 5 |
| 84 | Intersect12 P->Q | 355.20 | 0.992 | 207.00 | 145.20 | 2.00 | 1.00 | 5 |
| 260 | Intersect12 Q->P | 163.80 | 0.971 | 72.20 | 86.80 | 1.80 | 3.00 | 5 |
| 406 | Intersect12 P->Q | 129.40 | 0.977 | 81.00 | 45.40 | 3.00 | 0.00 | 5 |
| 551 | Intersect12 P->Q | 100.60 | 0.960 | 55.80 | 40.80 | 4.00 | 0.00 | 5 |
| 582 | Intersect12 P->Q | 42.40 | 1.000 | 23.80 | 18.60 | 0.00 | 0.00 | 5 |

Note: phase timings cover `Intersect12` and `Winding03` only; `Intersections (total)` is excluded from the denominator.

#### perfTest Size Sweep

| nTri | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Peak RSS mean (MB) | Peak RSS min (MB) | Peak RSS max (MB) | Runs |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 512 | 1.03 | 1.08 | 0.86 | 1.18 | 4.80 | 4.77 | 4.84 | 5 |
| 2048 | 2.31 | 2.18 | 2.00 | 2.96 | 6.33 | 6.25 | 6.61 | 5 |
| 8192 | 6.14 | 5.78 | 5.22 | 7.78 | 11.78 | 11.33 | 12.92 | 5 |
| 32768 | 19.03 | 14.60 | 13.28 | 33.38 | 33.24 | 29.72 | 37.38 | 5 |
| 131072 | 57.02 | 51.78 | 43.92 | 89.48 | 124.79 | 118.31 | 129.69 | 5 |
| 524288 | 320.77 | 292.13 | 222.73 | 521.97 | 528.85 | 522.95 | 538.08 | 5 |
| 2097152 | 1385.23 | 956.21 | 866.58 | 3082.01 | 1946.27 | 1434.09 | 2080.12 | 5 |
| 8388608 | 12975.52 | 12145.70 | 11098.60 | 17419.70 | 3909.64 | 3110.64 | 4125.22 | 5 |

#### Existing Regression Tests

| Test | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Runs |
|---|---:|---:|---:|---:|---:|
| Manifold.DeepChainDoesNotOverflowNumLeaves | 1984.60 | 2000.00 | 1918.00 | 2005.00 | 5 |
| ExecutionContextFromMeshGL.CancelConcurrent | 80.80 | 62.00 | 53.00 | 152.00 | 5 |
| Boolean.BatchBoolean | 5.00 | 1.00 | 1.00 | 20.00 | 5 |
| CrossSection.BatchBoolean | 3.40 | 0.00 | 0.00 | 17.00 | 5 |
| Polygon.Sponge4 | 0.40 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Zebra1 | 2.00 | 2.00 | 2.00 | 2.00 | 5 |
| Polygon.Zebra3 | 929.40 | 899.00 | 847.00 | 1012.00 | 5 |

