### Weekly Benchmarks

Commit: `1713676a9c960eed34da82a95f204214c61194ac`
Runner: `GitHub Actions 1000000588`
OS: `macOS`
Compiler: `AppleClang 17.0.0.17000013`
CPU: `Apple M1 (Virtual)`
CPU count: `3`
CPU model identifier: `VirtualMac2,1`
CPU physical cores: `3`
CPU performance cores: `3`
Repeats: `5`

#### Ember Phase Timings

| Case | Dominant phase | Full mean (ms) | Intersect12 share | Assembly | Triangulation | Simplification | Sorting | P->Q | Q->P | Winding P | Winding Q | Runs |
|---:|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 16 | Assembly | 0.00 | 0.000 | 0.00 | 0.00 | 0.00 | 0.00 | 0.00 | 0.00 | 0.00 | 0.00 | 5 |
| 84 | Assembly | 0.00 | 0.000 | 0.00 | 0.00 | 0.00 | 0.00 | 0.00 | 0.00 | 0.00 | 0.00 | 5 |
| 667 | Assembly | 0.00 | 0.000 | 0.00 | 0.00 | 0.00 | 0.00 | 0.00 | 0.00 | 0.00 | 0.00 | 5 |
| 695 | Assembly | 0.00 | 0.000 | 0.00 | 0.00 | 0.00 | 0.00 | 0.00 | 0.00 | 0.00 | 0.00 | 5 |
| 260 | Assembly | 0.00 | 0.000 | 0.00 | 0.00 | 0.00 | 0.00 | 0.00 | 0.00 | 0.00 | 0.00 | 5 |
| 406 | Assembly | 0.00 | 0.000 | 0.00 | 0.00 | 0.00 | 0.00 | 0.00 | 0.00 | 0.00 | 0.00 | 5 |
| 551 | Assembly | 0.00 | 0.000 | 0.00 | 0.00 | 0.00 | 0.00 | 0.00 | 0.00 | 0.00 | 0.00 | 5 |
| 582 | Assembly | 0.00 | 0.000 | 0.00 | 0.00 | 0.00 | 0.00 | 0.00 | 0.00 | 0.00 | 0.00 | 5 |

Note: phase timings use independent phases only; `Intersections (total)` is not added to the denominator.

#### perfTest Size Sweep

| nTri | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Runs |
|---:|---:|---:|---:|---:|---:|
| 512 | 1.48 | 1.06 | 0.78 | 2.72 | 5 |
| 2048 | 2.49 | 2.20 | 1.99 | 3.41 | 5 |
| 8192 | 7.79 | 6.74 | 5.20 | 11.17 | 5 |
| 32768 | 30.03 | 25.39 | 14.02 | 49.71 | 5 |
| 131072 | 118.76 | 98.65 | 48.90 | 264.12 | 5 |
| 524288 | 385.97 | 418.21 | 314.56 | 433.70 | 5 |
| 2097152 | 1600.98 | 1671.59 | 1129.64 | 2254.42 | 5 |
| 8388608 | 12380.81 | 12469.70 | 9237.43 | 15167.10 | 5 |

#### Existing Regression Tests

| Test | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Runs |
|---|---:|---:|---:|---:|---:|
| Boolean.BatchBoolean | 3.40 | 2.00 | 2.00 | 7.00 | 5 |
| CrossSection.BatchBoolean | 0.20 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Sponge4 | 0.00 | 0.00 | 0.00 | 0.00 | 5 |
| Polygon.Zebra1 | 1.20 | 1.00 | 1.00 | 2.00 | 5 |
| Polygon.Zebra3 | 746.20 | 736.00 | 700.00 | 853.00 | 5 |

