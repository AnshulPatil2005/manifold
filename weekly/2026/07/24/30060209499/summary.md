### Weekly Benchmarks

Commit: `31115d3e82208d804988dfbee91241245604e28a`
Runner: `GitHub Actions 1000000990`
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
| 667 | Intersect12 Q->P | 1157.20 | 0.997 | 462.80 | 691.40 | 0.00 | 3.00 | 5 |
| 695 | Intersect12 P->Q | 492.00 | 0.991 | 345.00 | 142.40 | 4.60 | 0.00 | 5 |
| 16 | Intersect12 Q->P | 476.40 | 0.998 | 176.60 | 298.80 | 0.00 | 1.00 | 5 |
| 84 | Intersect12 P->Q | 380.80 | 0.992 | 218.60 | 159.00 | 2.20 | 1.00 | 5 |
| 260 | Intersect12 Q->P | 165.40 | 0.970 | 72.80 | 87.60 | 1.60 | 3.40 | 5 |
| 406 | Intersect12 P->Q | 140.20 | 0.977 | 86.00 | 51.00 | 3.20 | 0.00 | 5 |
| 551 | Intersect12 P->Q | 103.60 | 0.959 | 57.00 | 42.40 | 4.20 | 0.00 | 5 |
| 582 | Intersect12 P->Q | 42.20 | 1.000 | 24.00 | 18.20 | 0.00 | 0.00 | 5 |

Note: phase timings cover `Intersect12` and `Winding03` only; `Intersections (total)` is excluded from the denominator.

#### perfTest Size Sweep

| nTri | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Peak RSS mean (MB) | Peak RSS min (MB) | Peak RSS max (MB) | Runs |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 512 | 1.98 | 1.21 | 0.86 | 5.19 | 4.78 | 4.58 | 4.86 | 5 |
| 2048 | 2.59 | 2.47 | 1.89 | 3.60 | 6.25 | 5.95 | 6.47 | 5 |
| 8192 | 7.20 | 7.49 | 4.95 | 8.76 | 11.67 | 11.11 | 12.86 | 5 |
| 32768 | 20.14 | 18.24 | 11.84 | 27.55 | 34.32 | 29.62 | 38.05 | 5 |
| 131072 | 73.06 | 59.23 | 46.66 | 102.83 | 127.43 | 124.11 | 131.25 | 5 |
| 524288 | 401.90 | 344.35 | 296.60 | 687.27 | 530.29 | 527.91 | 533.84 | 5 |
| 2097152 | 1469.96 | 1321.07 | 990.31 | 2497.77 | 1966.20 | 1521.58 | 2089.75 | 5 |
| 8388608 | 13956.34 | 12401.70 | 10145.10 | 19751.20 | 3952.95 | 3236.38 | 4156.48 | 5 |

#### Existing Regression Tests

| Test | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Runs |
|---|---:|---:|---:|---:|---:|
| Manifold.DeepChainDoesNotOverflowNumLeaves | 1985.40 | 1837.00 | 1556.00 | 2451.00 | 5 |
| ExecutionContextFromMeshGL.CancelConcurrent | 77.00 | 78.00 | 56.00 | 102.00 | 5 |
| Boolean.BatchBoolean | 2.80 | 3.00 | 1.00 | 4.00 | 5 |
| CrossSection.BatchBoolean | 0.20 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Sponge4 | 1.00 | 1.00 | 1.00 | 1.00 | 5 |
| Polygon.Zebra1 | 2.40 | 2.00 | 2.00 | 4.00 | 5 |
| Polygon.Zebra3 | 1155.00 | 1016.00 | 956.00 | 1453.00 | 5 |

