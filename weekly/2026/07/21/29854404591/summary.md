### Weekly Benchmarks

Commit: `e00c5f5784eefa27255681dce4105bd45be3daa0`
Runner: `GitHub Actions 1000000941`
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
| 667 | Intersect12 Q->P | 1048.80 | 0.997 | 417.20 | 628.60 | 0.00 | 3.00 | 5 |
| 695 | Intersect12 P->Q | 453.00 | 0.991 | 317.00 | 132.00 | 4.00 | 0.00 | 5 |
| 16 | Intersect12 Q->P | 386.80 | 0.997 | 151.80 | 234.00 | 0.00 | 1.00 | 5 |
| 84 | Intersect12 P->Q | 332.20 | 0.990 | 192.20 | 136.60 | 2.40 | 1.00 | 5 |
| 260 | Intersect12 Q->P | 156.60 | 0.973 | 69.40 | 83.00 | 1.20 | 3.00 | 5 |
| 406 | Intersect12 P->Q | 119.40 | 0.975 | 74.80 | 41.60 | 3.00 | 0.00 | 5 |
| 551 | Intersect12 P->Q | 97.40 | 0.959 | 53.80 | 39.60 | 4.00 | 0.00 | 5 |
| 582 | Intersect12 P->Q | 40.20 | 1.000 | 22.60 | 17.60 | 0.00 | 0.00 | 5 |

Note: phase timings cover `Intersect12` and `Winding03` only; `Intersections (total)` is excluded from the denominator.

#### perfTest Size Sweep

| nTri | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Peak RSS mean (MB) | Peak RSS min (MB) | Peak RSS max (MB) | Runs |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 512 | 1.48 | 1.48 | 0.91 | 2.01 | 4.84 | 4.73 | 4.92 | 5 |
| 2048 | 2.63 | 2.48 | 2.04 | 3.51 | 6.23 | 6.20 | 6.27 | 5 |
| 8192 | 7.64 | 7.48 | 5.36 | 9.76 | 12.60 | 11.61 | 13.48 | 5 |
| 32768 | 36.25 | 24.50 | 12.80 | 85.04 | 33.95 | 30.95 | 37.53 | 5 |
| 131072 | 94.51 | 106.27 | 41.48 | 148.89 | 117.48 | 105.19 | 124.42 | 5 |
| 524288 | 437.95 | 451.25 | 319.91 | 512.84 | 531.98 | 518.52 | 540.31 | 5 |
| 2097152 | 1919.29 | 1991.29 | 966.07 | 2642.63 | 1973.23 | 1562.47 | 2083.17 | 5 |
| 8388608 | 19345.50 | 17801.00 | 12821.00 | 26109.40 | 3921.67 | 3175.64 | 4146.47 | 5 |

#### Existing Regression Tests

| Test | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Runs |
|---|---:|---:|---:|---:|---:|
| Manifold.DeepChainDoesNotOverflowNumLeaves | 2486.60 | 2343.00 | 2110.00 | 2910.00 | 5 |
| ExecutionContextFromMeshGL.CancelConcurrent | 96.40 | 82.00 | 65.00 | 145.00 | 5 |
| Boolean.BatchBoolean | 4.00 | 2.00 | 1.00 | 13.00 | 5 |
| CrossSection.BatchBoolean | 2.60 | 1.00 | 0.00 | 11.00 | 5 |
| Polygon.Sponge4 | 1.00 | 1.00 | 0.00 | 3.00 | 5 |
| Polygon.Zebra1 | 2.40 | 2.00 | 2.00 | 4.00 | 5 |
| Polygon.Zebra3 | 1043.40 | 1064.00 | 880.00 | 1231.00 | 5 |

