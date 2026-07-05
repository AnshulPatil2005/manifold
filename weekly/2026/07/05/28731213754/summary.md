### Weekly Benchmarks

Commit: `1713676a9c960eed34da82a95f204214c61194ac`
Runner: `GitHub Actions 1000000531`
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
| 512 | 0.99 | 0.98 | 0.92 | 1.13 | 5 |
| 2048 | 2.88 | 2.41 | 2.05 | 5.21 | 5 |
| 8192 | 6.05 | 5.89 | 5.50 | 6.60 | 5 |
| 32768 | 17.15 | 16.36 | 14.82 | 22.76 | 5 |
| 131072 | 67.23 | 66.77 | 54.95 | 75.87 | 5 |
| 524288 | 297.15 | 277.49 | 233.30 | 421.71 | 5 |
| 2097152 | 1123.42 | 1087.29 | 926.38 | 1395.02 | 5 |
| 8388608 | 11938.40 | 12090.60 | 9924.32 | 14483.30 | 5 |

#### Existing Regression Tests

| Test | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Runs |
|---|---:|---:|---:|---:|---:|
| Boolean.BatchBoolean | 3.80 | 2.00 | 2.00 | 9.00 | 5 |
| CrossSection.BatchBoolean | 0.20 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Sponge4 | 0.20 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Zebra1 | 2.00 | 2.00 | 2.00 | 2.00 | 5 |
| Polygon.Zebra3 | 1376.40 | 1317.00 | 1185.00 | 1625.00 | 5 |

