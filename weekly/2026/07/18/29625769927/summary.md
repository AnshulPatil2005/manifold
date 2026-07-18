### Weekly Benchmarks

Commit: `31115d3e82208d804988dfbee91241245604e28a`
Runner: `GitHub Actions 1000000868`
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
| 667 | Intersect12 Q->P | 1197.60 | 0.997 | 480.60 | 713.40 | 0.00 | 3.60 | 5 |
| 695 | Intersect12 P->Q | 509.20 | 0.991 | 356.40 | 148.40 | 4.40 | 0.00 | 5 |
| 16 | Intersect12 Q->P | 446.60 | 0.997 | 172.00 | 273.40 | 0.00 | 1.20 | 5 |
| 84 | Intersect12 P->Q | 380.00 | 0.991 | 214.60 | 162.00 | 2.40 | 1.00 | 5 |
| 260 | Intersect12 Q->P | 175.80 | 0.969 | 77.60 | 92.80 | 2.00 | 3.40 | 5 |
| 406 | Intersect12 P->Q | 142.60 | 0.979 | 85.40 | 54.20 | 3.00 | 0.00 | 5 |
| 551 | Intersect12 P->Q | 109.80 | 0.957 | 60.20 | 44.80 | 4.80 | 0.00 | 5 |
| 582 | Intersect12 P->Q | 48.40 | 1.000 | 27.20 | 21.20 | 0.00 | 0.00 | 5 |

Note: phase timings cover `Intersect12` and `Winding03` only; `Intersections (total)` is excluded from the denominator.

#### perfTest Size Sweep

| nTri | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Peak RSS mean (MB) | Peak RSS min (MB) | Peak RSS max (MB) | Runs |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 512 | 1.31 | 1.19 | 1.07 | 1.61 | 4.64 | 4.38 | 4.89 | 5 |
| 2048 | 3.10 | 2.71 | 2.24 | 4.43 | 6.08 | 5.64 | 6.27 | 5 |
| 8192 | 7.39 | 7.55 | 5.47 | 8.93 | 11.91 | 11.31 | 12.77 | 5 |
| 32768 | 17.53 | 15.97 | 12.91 | 24.68 | 32.51 | 29.69 | 36.70 | 5 |
| 131072 | 58.90 | 48.62 | 43.09 | 96.02 | 120.82 | 114.11 | 135.56 | 5 |
| 524288 | 318.03 | 266.31 | 227.30 | 565.16 | 532.26 | 527.94 | 535.52 | 5 |
| 2097152 | 1459.30 | 829.59 | 712.96 | 3666.95 | 1962.23 | 1497.94 | 2093.64 | 5 |
| 8388608 | 14351.60 | 11717.80 | 11268.90 | 23334.70 | 3893.94 | 3074.70 | 4141.61 | 5 |

#### Existing Regression Tests

| Test | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Runs |
|---|---:|---:|---:|---:|---:|
| Manifold.DeepChainDoesNotOverflowNumLeaves | 1591.20 | 1537.00 | 1394.00 | 1813.00 | 5 |
| ExecutionContextFromMeshGL.CancelConcurrent | 53.00 | 49.00 | 45.00 | 69.00 | 5 |
| Boolean.BatchBoolean | 1.40 | 1.00 | 1.00 | 2.00 | 5 |
| CrossSection.BatchBoolean | 0.20 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Sponge4 | 0.20 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Zebra1 | 2.40 | 2.00 | 2.00 | 4.00 | 5 |
| Polygon.Zebra3 | 856.80 | 850.00 | 808.00 | 925.00 | 5 |

