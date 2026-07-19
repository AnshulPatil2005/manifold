### Weekly Benchmarks

Commit: `31115d3e82208d804988dfbee91241245604e28a`
Runner: `GitHub Actions 1000000898`
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
| 667 | Intersect12 Q->P | 1047.60 | 0.997 | 413.80 | 630.80 | 0.00 | 3.00 | 5 |
| 695 | Intersect12 P->Q | 439.20 | 0.991 | 306.00 | 129.20 | 4.00 | 0.00 | 5 |
| 16 | Intersect12 Q->P | 386.00 | 0.997 | 153.80 | 231.20 | 0.00 | 1.00 | 5 |
| 84 | Intersect12 P->Q | 339.00 | 0.991 | 194.40 | 141.60 | 2.00 | 1.00 | 5 |
| 260 | Intersect12 Q->P | 155.40 | 0.973 | 68.00 | 83.20 | 1.20 | 3.00 | 5 |
| 406 | Intersect12 P->Q | 122.80 | 0.976 | 75.60 | 44.20 | 3.00 | 0.00 | 5 |
| 551 | Intersect12 P->Q | 95.00 | 0.958 | 53.00 | 38.00 | 4.00 | 0.00 | 5 |
| 582 | Intersect12 P->Q | 39.40 | 1.000 | 22.40 | 17.00 | 0.00 | 0.00 | 5 |

Note: phase timings cover `Intersect12` and `Winding03` only; `Intersections (total)` is excluded from the denominator.

#### perfTest Size Sweep

| nTri | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Peak RSS mean (MB) | Peak RSS min (MB) | Peak RSS max (MB) | Runs |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 512 | 0.98 | 1.00 | 0.90 | 1.06 | 4.73 | 4.55 | 4.84 | 5 |
| 2048 | 2.02 | 2.02 | 1.88 | 2.18 | 6.21 | 6.03 | 6.27 | 5 |
| 8192 | 5.35 | 5.32 | 5.00 | 5.71 | 11.34 | 11.23 | 11.48 | 5 |
| 32768 | 17.50 | 13.32 | 12.12 | 35.34 | 31.53 | 29.62 | 34.91 | 5 |
| 131072 | 70.39 | 64.17 | 42.82 | 112.18 | 123.43 | 118.59 | 129.52 | 5 |
| 524288 | 266.19 | 204.59 | 157.94 | 429.35 | 528.86 | 523.50 | 536.34 | 5 |
| 2097152 | 917.98 | 884.99 | 638.36 | 1289.44 | 1976.00 | 1564.20 | 2083.97 | 5 |
| 8388608 | 11675.50 | 11400.80 | 10808.20 | 12860.70 | 3860.00 | 3375.45 | 4143.50 | 5 |

#### Existing Regression Tests

| Test | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Runs |
|---|---:|---:|---:|---:|---:|
| Manifold.DeepChainDoesNotOverflowNumLeaves | 1604.00 | 1629.00 | 1398.00 | 1714.00 | 5 |
| ExecutionContextFromMeshGL.CancelConcurrent | 50.20 | 50.00 | 45.00 | 56.00 | 5 |
| Boolean.BatchBoolean | 1.20 | 1.00 | 1.00 | 2.00 | 5 |
| CrossSection.BatchBoolean | 0.20 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Sponge4 | 0.20 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Zebra1 | 2.00 | 2.00 | 2.00 | 2.00 | 5 |
| Polygon.Zebra3 | 805.80 | 774.00 | 757.00 | 922.00 | 5 |

