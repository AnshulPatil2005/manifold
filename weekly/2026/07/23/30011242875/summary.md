### Weekly Benchmarks

Commit: `31115d3e82208d804988dfbee91241245604e28a`
Runner: `GitHub Actions 1000000979`
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
| 667 | Intersect12 Q->P | 1489.00 | 0.997 | 614.20 | 870.40 | 0.00 | 4.40 | 5 |
| 695 | Intersect12 P->Q | 589.20 | 0.990 | 410.40 | 172.80 | 5.80 | 0.20 | 5 |
| 16 | Intersect12 Q->P | 559.80 | 0.997 | 228.00 | 329.80 | 0.20 | 1.80 | 5 |
| 84 | Intersect12 P->Q | 497.80 | 0.990 | 279.80 | 213.20 | 3.40 | 1.40 | 5 |
| 260 | Intersect12 Q->P | 201.60 | 0.973 | 92.60 | 103.60 | 2.00 | 3.40 | 5 |
| 406 | Intersect12 P->Q | 155.20 | 0.977 | 91.40 | 60.40 | 3.40 | 0.00 | 5 |
| 551 | Intersect12 P->Q | 122.20 | 0.961 | 70.00 | 47.40 | 4.80 | 0.00 | 5 |
| 582 | Intersect12 P->Q | 50.40 | 0.996 | 29.40 | 20.80 | 0.20 | 0.00 | 5 |

Note: phase timings cover `Intersect12` and `Winding03` only; `Intersections (total)` is excluded from the denominator.

#### perfTest Size Sweep

| nTri | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Peak RSS mean (MB) | Peak RSS min (MB) | Peak RSS max (MB) | Runs |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 512 | 1.12 | 1.07 | 1.00 | 1.30 | 4.71 | 4.41 | 4.83 | 5 |
| 2048 | 2.71 | 2.50 | 2.25 | 3.53 | 6.14 | 5.92 | 6.27 | 5 |
| 8192 | 8.94 | 7.72 | 5.82 | 15.65 | 12.35 | 11.14 | 13.09 | 5 |
| 32768 | 23.99 | 21.35 | 13.84 | 40.02 | 33.42 | 30.69 | 35.56 | 5 |
| 131072 | 87.27 | 73.43 | 47.51 | 187.43 | 114.95 | 111.73 | 118.50 | 5 |
| 524288 | 480.23 | 289.03 | 259.51 | 895.69 | 509.63 | 403.19 | 542.14 | 5 |
| 2097152 | 1871.78 | 1531.29 | 1027.17 | 2953.27 | 2037.58 | 1870.42 | 2086.45 | 5 |
| 8388608 | 19478.60 | 16479.80 | 13820.10 | 27155.80 | 3773.63 | 2837.59 | 4089.34 | 5 |

#### Existing Regression Tests

| Test | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Runs |
|---|---:|---:|---:|---:|---:|
| Manifold.DeepChainDoesNotOverflowNumLeaves | 2554.80 | 2412.00 | 2023.00 | 3400.00 | 5 |
| ExecutionContextFromMeshGL.CancelConcurrent | 98.80 | 91.00 | 61.00 | 134.00 | 5 |
| Boolean.BatchBoolean | 1.80 | 2.00 | 1.00 | 3.00 | 5 |
| CrossSection.BatchBoolean | 0.20 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Sponge4 | 0.40 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Zebra1 | 2.00 | 2.00 | 2.00 | 2.00 | 5 |
| Polygon.Zebra3 | 1075.20 | 1102.00 | 911.00 | 1205.00 | 5 |

