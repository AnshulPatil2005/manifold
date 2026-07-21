### Weekly Benchmarks

Commit: `31115d3e82208d804988dfbee91241245604e28a`
Runner: `GitHub Actions 1000000935`
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
| 667 | Intersect12 Q->P | 1434.20 | 0.997 | 561.00 | 869.40 | 0.00 | 3.80 | 5 |
| 695 | Intersect12 P->Q | 583.80 | 0.989 | 403.00 | 174.60 | 6.00 | 0.20 | 5 |
| 16 | Intersect12 Q->P | 507.20 | 0.998 | 196.60 | 309.40 | 0.00 | 1.20 | 5 |
| 84 | Intersect12 P->Q | 447.60 | 0.990 | 243.00 | 200.00 | 3.40 | 1.20 | 5 |
| 260 | Intersect12 Q->P | 201.60 | 0.970 | 88.60 | 107.00 | 2.00 | 4.00 | 5 |
| 406 | Intersect12 P->Q | 166.20 | 0.978 | 104.40 | 58.20 | 3.60 | 0.00 | 5 |
| 551 | Intersect12 P->Q | 125.60 | 0.962 | 70.20 | 50.60 | 4.80 | 0.00 | 5 |
| 582 | Intersect12 P->Q | 50.40 | 0.996 | 28.20 | 22.00 | 0.20 | 0.00 | 5 |

Note: phase timings cover `Intersect12` and `Winding03` only; `Intersections (total)` is excluded from the denominator.

#### perfTest Size Sweep

| nTri | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Peak RSS mean (MB) | Peak RSS min (MB) | Peak RSS max (MB) | Runs |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 512 | 3.03 | 2.34 | 0.84 | 8.33 | 4.67 | 4.50 | 4.83 | 5 |
| 2048 | 3.29 | 3.10 | 2.66 | 4.44 | 6.21 | 5.94 | 6.39 | 5 |
| 8192 | 9.41 | 9.66 | 6.85 | 11.39 | 11.70 | 11.28 | 12.27 | 5 |
| 32768 | 27.42 | 26.01 | 20.06 | 36.71 | 34.31 | 32.05 | 37.67 | 5 |
| 131072 | 105.83 | 107.12 | 88.38 | 123.40 | 126.76 | 122.44 | 132.75 | 5 |
| 524288 | 556.83 | 473.24 | 378.81 | 800.18 | 528.89 | 521.11 | 532.69 | 5 |
| 2097152 | 1740.20 | 1769.86 | 1344.98 | 2147.42 | 1952.15 | 1466.80 | 2080.31 | 5 |
| 8388608 | 18405.50 | 17344.10 | 11450.60 | 26031.20 | 3761.96 | 3095.42 | 4100.16 | 5 |

#### Existing Regression Tests

| Test | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Runs |
|---|---:|---:|---:|---:|---:|
| Manifold.DeepChainDoesNotOverflowNumLeaves | 2826.40 | 2719.00 | 2281.00 | 3743.00 | 5 |
| ExecutionContextFromMeshGL.CancelConcurrent | 116.80 | 122.00 | 90.00 | 141.00 | 5 |
| Boolean.BatchBoolean | 4.00 | 3.00 | 2.00 | 9.00 | 5 |
| CrossSection.BatchBoolean | 0.20 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Sponge4 | 0.80 | 1.00 | 0.00 | 1.00 | 5 |
| Polygon.Zebra1 | 2.20 | 2.00 | 2.00 | 3.00 | 5 |
| Polygon.Zebra3 | 1237.60 | 1224.00 | 1081.00 | 1506.00 | 5 |

