### Weekly Benchmarks

Commit: `31115d3e82208d804988dfbee91241245604e28a`
Runner: `GitHub Actions 1000000918`
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
| 667 | Intersect12 Q->P | 1094.00 | 0.997 | 444.00 | 647.00 | 0.00 | 3.00 | 5 |
| 695 | Intersect12 P->Q | 472.00 | 0.991 | 324.60 | 143.00 | 4.40 | 0.00 | 5 |
| 16 | Intersect12 Q->P | 394.40 | 0.997 | 156.80 | 236.60 | 0.00 | 1.00 | 5 |
| 84 | Intersect12 P->Q | 356.00 | 0.992 | 205.20 | 147.80 | 2.00 | 1.00 | 5 |
| 260 | Intersect12 Q->P | 164.20 | 0.970 | 71.60 | 87.60 | 1.80 | 3.20 | 5 |
| 406 | Intersect12 P->Q | 134.40 | 0.978 | 83.20 | 48.20 | 3.00 | 0.00 | 5 |
| 551 | Intersect12 P->Q | 104.20 | 0.961 | 58.80 | 41.40 | 4.00 | 0.00 | 5 |
| 582 | Intersect12 P->Q | 43.00 | 0.996 | 24.00 | 18.80 | 0.20 | 0.00 | 5 |

Note: phase timings cover `Intersect12` and `Winding03` only; `Intersections (total)` is excluded from the denominator.

#### perfTest Size Sweep

| nTri | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Peak RSS mean (MB) | Peak RSS min (MB) | Peak RSS max (MB) | Runs |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 512 | 2.34 | 1.47 | 0.88 | 4.75 | 4.79 | 4.72 | 4.89 | 5 |
| 2048 | 6.00 | 2.89 | 2.07 | 17.84 | 6.28 | 6.02 | 6.56 | 5 |
| 8192 | 9.08 | 7.95 | 5.73 | 13.80 | 12.43 | 11.47 | 13.11 | 5 |
| 32768 | 32.98 | 25.30 | 15.69 | 68.87 | 36.25 | 33.28 | 37.72 | 5 |
| 131072 | 73.25 | 74.55 | 54.82 | 87.91 | 117.51 | 112.94 | 120.30 | 5 |
| 524288 | 393.16 | 371.67 | 287.43 | 533.12 | 533.67 | 520.77 | 551.56 | 5 |
| 2097152 | 1809.48 | 1649.09 | 1208.65 | 2563.00 | 2014.45 | 1770.16 | 2084.14 | 5 |
| 8388608 | 19023.92 | 18537.80 | 14956.20 | 21904.70 | 3786.29 | 3285.53 | 4074.20 | 5 |

#### Existing Regression Tests

| Test | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Runs |
|---|---:|---:|---:|---:|---:|
| Manifold.DeepChainDoesNotOverflowNumLeaves | 2346.80 | 2266.00 | 2149.00 | 2642.00 | 5 |
| ExecutionContextFromMeshGL.CancelConcurrent | 95.60 | 101.00 | 66.00 | 112.00 | 5 |
| Boolean.BatchBoolean | 2.40 | 2.00 | 1.00 | 4.00 | 5 |
| CrossSection.BatchBoolean | 0.20 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Sponge4 | 0.00 | 0.00 | 0.00 | 0.00 | 5 |
| Polygon.Zebra1 | 2.00 | 2.00 | 2.00 | 2.00 | 5 |
| Polygon.Zebra3 | 982.80 | 1008.00 | 824.00 | 1107.00 | 5 |

