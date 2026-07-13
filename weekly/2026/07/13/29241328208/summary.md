### Weekly Benchmarks

Commit: `31115d3e82208d804988dfbee91241245604e28a`
Runner: `GitHub Actions 1000000774`
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
| 667 | Intersect12 Q->P | 1171.80 | 0.997 | 461.20 | 707.40 | 0.00 | 3.20 | 5 |
| 695 | Intersect12 P->Q | 509.00 | 0.990 | 344.00 | 159.80 | 5.20 | 0.00 | 5 |
| 16 | Intersect12 Q->P | 441.60 | 0.997 | 171.60 | 268.60 | 0.00 | 1.40 | 5 |
| 84 | Intersect12 P->Q | 376.00 | 0.990 | 216.00 | 156.40 | 2.60 | 1.00 | 5 |
| 260 | Intersect12 Q->P | 190.60 | 0.970 | 81.40 | 103.60 | 2.00 | 3.60 | 5 |
| 406 | Intersect12 P->Q | 144.60 | 0.979 | 89.40 | 52.20 | 3.00 | 0.00 | 5 |
| 551 | Intersect12 P->Q | 118.00 | 0.964 | 64.60 | 49.20 | 4.20 | 0.00 | 5 |
| 582 | Intersect12 Q->P | 53.60 | 0.996 | 26.60 | 26.80 | 0.20 | 0.00 | 5 |

Note: phase timings cover `Intersect12` and `Winding03` only; `Intersections (total)` is excluded from the denominator.

#### perfTest Size Sweep

| nTri | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Peak RSS mean (MB) | Peak RSS min (MB) | Peak RSS max (MB) | Runs |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 512 | 1.42 | 1.39 | 1.06 | 1.94 | 4.77 | 4.69 | 4.86 | 5 |
| 2048 | 2.93 | 2.75 | 1.95 | 4.26 | 6.24 | 6.09 | 6.36 | 5 |
| 8192 | 10.23 | 8.48 | 7.09 | 14.73 | 12.57 | 11.38 | 13.39 | 5 |
| 32768 | 30.61 | 34.09 | 13.32 | 37.75 | 33.00 | 29.61 | 35.44 | 5 |
| 131072 | 86.01 | 89.68 | 44.14 | 123.61 | 126.53 | 113.22 | 131.84 | 5 |
| 524288 | 387.35 | 413.66 | 306.01 | 457.23 | 526.17 | 524.06 | 528.03 | 5 |
| 2097152 | 1431.63 | 1249.24 | 1074.78 | 2322.53 | 1961.27 | 1487.95 | 2085.61 | 5 |
| 8388608 | 16208.36 | 16011.20 | 13612.60 | 19089.30 | 3928.03 | 3131.02 | 4174.64 | 5 |

#### Existing Regression Tests

| Test | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Runs |
|---|---:|---:|---:|---:|---:|
| Manifold.DeepChainDoesNotOverflowNumLeaves | 2863.80 | 2879.00 | 2757.00 | 2965.00 | 5 |
| ExecutionContextFromMeshGL.CancelConcurrent | 115.80 | 114.00 | 79.00 | 149.00 | 5 |
| Boolean.BatchBoolean | 2.60 | 2.00 | 1.00 | 6.00 | 5 |
| CrossSection.BatchBoolean | 0.20 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Sponge4 | 0.60 | 1.00 | 0.00 | 1.00 | 5 |
| Polygon.Zebra1 | 2.20 | 2.00 | 2.00 | 3.00 | 5 |
| Polygon.Zebra3 | 1217.00 | 1163.00 | 1099.00 | 1360.00 | 5 |

