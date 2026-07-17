### Weekly Benchmarks

Commit: `31115d3e82208d804988dfbee91241245604e28a`
Runner: `GitHub Actions 1000000847`
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
| 667 | Intersect12 Q->P | 1118.40 | 0.997 | 441.20 | 674.20 | 0.00 | 3.00 | 5 |
| 695 | Intersect12 P->Q | 483.60 | 0.990 | 336.20 | 142.40 | 5.00 | 0.00 | 5 |
| 16 | Intersect12 Q->P | 407.20 | 0.998 | 160.60 | 245.60 | 0.00 | 1.00 | 5 |
| 84 | Intersect12 P->Q | 365.20 | 0.992 | 209.60 | 152.60 | 2.00 | 1.00 | 5 |
| 260 | Intersect12 Q->P | 164.40 | 0.970 | 71.80 | 87.60 | 2.00 | 3.00 | 5 |
| 406 | Intersect12 P->Q | 135.00 | 0.978 | 83.40 | 48.60 | 3.00 | 0.00 | 5 |
| 551 | Intersect12 P->Q | 100.20 | 0.960 | 55.60 | 40.60 | 4.00 | 0.00 | 5 |
| 582 | Intersect12 P->Q | 42.60 | 1.000 | 24.00 | 18.60 | 0.00 | 0.00 | 5 |

Note: phase timings cover `Intersect12` and `Winding03` only; `Intersections (total)` is excluded from the denominator.

#### perfTest Size Sweep

| nTri | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Peak RSS mean (MB) | Peak RSS min (MB) | Peak RSS max (MB) | Runs |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 512 | 1.05 | 1.05 | 0.88 | 1.20 | 4.76 | 4.56 | 4.97 | 5 |
| 2048 | 2.26 | 2.17 | 2.05 | 2.59 | 6.22 | 6.02 | 6.42 | 5 |
| 8192 | 6.31 | 6.16 | 5.53 | 7.61 | 11.91 | 11.33 | 13.00 | 5 |
| 32768 | 17.91 | 17.23 | 15.14 | 22.60 | 35.47 | 32.88 | 37.73 | 5 |
| 131072 | 57.37 | 57.73 | 51.46 | 63.33 | 121.65 | 118.08 | 125.47 | 5 |
| 524288 | 316.30 | 330.07 | 265.58 | 364.20 | 538.45 | 523.05 | 552.28 | 5 |
| 2097152 | 1139.46 | 1091.98 | 859.34 | 1500.39 | 2014.10 | 1768.20 | 2091.31 | 5 |
| 8388608 | 12687.08 | 11914.70 | 10869.80 | 17763.90 | 3867.32 | 3258.02 | 4063.72 | 5 |

#### Existing Regression Tests

| Test | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Runs |
|---|---:|---:|---:|---:|---:|
| Manifold.DeepChainDoesNotOverflowNumLeaves | 1943.20 | 1927.00 | 1856.00 | 2015.00 | 5 |
| ExecutionContextFromMeshGL.CancelConcurrent | 63.20 | 65.00 | 52.00 | 71.00 | 5 |
| Boolean.BatchBoolean | 1.60 | 1.00 | 1.00 | 3.00 | 5 |
| CrossSection.BatchBoolean | 0.20 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Sponge4 | 0.40 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Zebra1 | 2.00 | 2.00 | 2.00 | 2.00 | 5 |
| Polygon.Zebra3 | 917.80 | 907.00 | 844.00 | 1041.00 | 5 |

