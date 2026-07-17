### Weekly Benchmarks

Commit: `31115d3e82208d804988dfbee91241245604e28a`
Runner: `GitHub Actions 1000000854`
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
| 667 | Intersect12 Q->P | 1191.20 | 0.997 | 501.00 | 687.20 | 0.00 | 3.00 | 5 |
| 695 | Intersect12 P->Q | 526.00 | 0.990 | 366.80 | 154.20 | 5.00 | 0.00 | 5 |
| 16 | Intersect12 Q->P | 409.20 | 0.998 | 162.20 | 246.00 | 0.00 | 1.00 | 5 |
| 84 | Intersect12 P->Q | 366.80 | 0.991 | 208.20 | 155.40 | 2.20 | 1.00 | 5 |
| 260 | Intersect12 Q->P | 168.00 | 0.971 | 73.80 | 89.40 | 1.80 | 3.00 | 5 |
| 406 | Intersect12 P->Q | 133.00 | 0.977 | 81.80 | 48.20 | 3.00 | 0.00 | 5 |
| 551 | Intersect12 P->Q | 102.80 | 0.961 | 57.60 | 41.20 | 4.00 | 0.00 | 5 |
| 582 | Intersect12 P->Q | 42.80 | 1.000 | 24.00 | 18.80 | 0.00 | 0.00 | 5 |

Note: phase timings cover `Intersect12` and `Winding03` only; `Intersections (total)` is excluded from the denominator.

#### perfTest Size Sweep

| nTri | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Peak RSS mean (MB) | Peak RSS min (MB) | Peak RSS max (MB) | Runs |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 512 | 2.72 | 1.87 | 0.96 | 7.28 | 4.72 | 4.61 | 4.80 | 5 |
| 2048 | 3.16 | 2.89 | 2.12 | 4.29 | 6.45 | 6.27 | 6.72 | 5 |
| 8192 | 12.70 | 13.19 | 5.88 | 19.05 | 12.18 | 11.48 | 14.28 | 5 |
| 32768 | 28.67 | 26.67 | 14.28 | 48.74 | 35.83 | 31.97 | 37.89 | 5 |
| 131072 | 104.89 | 114.16 | 47.73 | 151.55 | 119.48 | 112.64 | 130.12 | 5 |
| 524288 | 473.26 | 486.68 | 373.65 | 542.25 | 535.68 | 528.50 | 543.47 | 5 |
| 2097152 | 2063.31 | 1861.50 | 1303.33 | 3200.36 | 1989.24 | 1610.78 | 2093.14 | 5 |
| 8388608 | 18401.40 | 17230.00 | 15590.10 | 21856.30 | 3982.45 | 3386.98 | 4170.75 | 5 |

#### Existing Regression Tests

| Test | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Runs |
|---|---:|---:|---:|---:|---:|
| Manifold.DeepChainDoesNotOverflowNumLeaves | 2436.80 | 2425.00 | 2167.00 | 2734.00 | 5 |
| ExecutionContextFromMeshGL.CancelConcurrent | 121.40 | 126.00 | 105.00 | 139.00 | 5 |
| Boolean.BatchBoolean | 3.40 | 2.00 | 2.00 | 7.00 | 5 |
| CrossSection.BatchBoolean | 0.60 | 0.00 | 0.00 | 2.00 | 5 |
| Polygon.Sponge4 | 0.60 | 1.00 | 0.00 | 1.00 | 5 |
| Polygon.Zebra1 | 2.00 | 2.00 | 2.00 | 2.00 | 5 |
| Polygon.Zebra3 | 1057.20 | 993.00 | 947.00 | 1289.00 | 5 |

