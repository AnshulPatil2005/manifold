### Weekly Benchmarks

Commit: `31115d3e82208d804988dfbee91241245604e28a`
Runner: `GitHub Actions 1000001066`
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
| 667 | Intersect12 Q->P | 1817.20 | 0.998 | 709.40 | 1104.80 | 0.00 | 3.00 | 5 |
| 695 | Intersect12 P->Q | 1017.20 | 0.995 | 785.80 | 226.80 | 4.60 | 0.00 | 5 |
| 16 | Intersect12 Q->P | 684.20 | 0.999 | 257.40 | 425.80 | 0.00 | 1.00 | 5 |
| 84 | Intersect12 P->Q | 602.00 | 0.995 | 338.80 | 260.00 | 2.20 | 1.00 | 5 |
| 260 | Intersect12 Q->P | 338.00 | 0.988 | 129.40 | 204.40 | 1.20 | 3.00 | 5 |
| 406 | Intersect12 P->Q | 244.20 | 0.988 | 167.00 | 74.20 | 3.00 | 0.00 | 5 |
| 551 | Intersect12 P->Q | 194.40 | 0.979 | 123.60 | 66.80 | 4.00 | 0.00 | 5 |
| 582 | Intersect12 P->Q | 76.80 | 1.000 | 47.60 | 29.20 | 0.00 | 0.00 | 5 |

Note: phase timings cover `Intersect12` and `Winding03` only; `Intersections (total)` is excluded from the denominator.

#### perfTest Size Sweep

| nTri | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Peak RSS mean (MB) | Peak RSS min (MB) | Peak RSS max (MB) | Runs |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 512 | 1.04 | 1.07 | 0.89 | 1.09 | 4.71 | 4.53 | 4.91 | 5 |
| 2048 | 2.21 | 2.22 | 1.98 | 2.53 | 6.07 | 5.67 | 6.27 | 5 |
| 8192 | 6.86 | 5.66 | 5.42 | 10.02 | 12.23 | 11.59 | 13.02 | 5 |
| 32768 | 18.18 | 16.74 | 13.44 | 27.24 | 34.09 | 29.62 | 37.38 | 5 |
| 131072 | 80.08 | 72.53 | 53.54 | 124.27 | 116.91 | 109.17 | 126.81 | 5 |
| 524288 | 387.08 | 404.84 | 299.88 | 489.28 | 535.44 | 513.98 | 555.22 | 5 |
| 2097152 | 1143.76 | 1085.76 | 933.51 | 1416.60 | 2019.47 | 1791.03 | 2080.61 | 5 |
| 8388608 | 13650.82 | 12836.60 | 11035.80 | 16401.90 | 3704.95 | 3185.97 | 3858.20 | 5 |

#### Existing Regression Tests

| Test | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Runs |
|---|---:|---:|---:|---:|---:|
| Manifold.DeepChainDoesNotOverflowNumLeaves | 2003.20 | 2016.00 | 1743.00 | 2251.00 | 5 |
| ExecutionContextFromMeshGL.CancelConcurrent | 70.80 | 74.00 | 55.00 | 84.00 | 5 |
| Boolean.BatchBoolean | 1.60 | 2.00 | 1.00 | 2.00 | 5 |
| CrossSection.BatchBoolean | 0.20 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Sponge4 | 0.40 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Zebra1 | 2.00 | 2.00 | 2.00 | 2.00 | 5 |
| Polygon.Zebra3 | 995.80 | 1017.00 | 893.00 | 1067.00 | 5 |

