### Weekly Benchmarks

Commit: `d46168c860507c5c668585cfb664446011e6177f`
Runner: `GitHub Actions 1000000714`
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
| 667 | Intersect12 Q->P | 1062.20 | 0.997 | 420.60 | 638.60 | 0.00 | 3.00 | 5 |
| 695 | Intersect12 P->Q | 454.00 | 0.991 | 315.80 | 134.00 | 4.20 | 0.00 | 5 |
| 16 | Intersect12 Q->P | 399.60 | 0.997 | 157.20 | 241.40 | 0.00 | 1.00 | 5 |
| 84 | Intersect12 P->Q | 347.00 | 0.991 | 198.00 | 146.00 | 2.00 | 1.00 | 5 |
| 260 | Intersect12 Q->P | 165.20 | 0.976 | 72.00 | 89.20 | 1.00 | 3.00 | 5 |
| 406 | Intersect12 P->Q | 127.80 | 0.977 | 77.60 | 47.20 | 3.00 | 0.00 | 5 |
| 551 | Intersect12 P->Q | 104.20 | 0.962 | 56.20 | 44.00 | 4.00 | 0.00 | 5 |
| 582 | Intersect12 P->Q | 49.60 | 1.000 | 25.00 | 24.60 | 0.00 | 0.00 | 5 |

Note: phase timings cover `Intersect12` and `Winding03` only; `Intersections (total)` is excluded from the denominator.

#### perfTest Size Sweep

| nTri | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Peak RSS mean (MB) | Peak RSS min (MB) | Peak RSS max (MB) | Runs |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 512 | 1.42 | 1.27 | 0.77 | 2.17 | 4.64 | 4.34 | 4.81 | 5 |
| 2048 | 2.11 | 1.97 | 1.88 | 2.40 | 6.27 | 6.25 | 6.30 | 5 |
| 8192 | 5.49 | 5.27 | 4.95 | 6.27 | 11.33 | 11.30 | 11.38 | 5 |
| 32768 | 15.18 | 13.30 | 11.99 | 23.68 | 34.23 | 29.59 | 37.44 | 5 |
| 131072 | 56.83 | 43.85 | 42.20 | 108.12 | 123.23 | 116.50 | 132.03 | 5 |
| 524288 | 315.89 | 276.96 | 231.83 | 519.18 | 535.80 | 526.92 | 555.30 | 5 |
| 2097152 | 936.21 | 856.40 | 716.15 | 1370.08 | 1950.29 | 1412.09 | 2100.09 | 5 |
| 8388608 | 12179.98 | 11065.00 | 10376.60 | 16944.10 | 3950.60 | 3302.97 | 4131.12 | 5 |

#### Existing Regression Tests

| Test | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Runs |
|---|---:|---:|---:|---:|---:|
| Manifold.DeepChainDoesNotOverflowNumLeaves | 1588.00 | 1581.00 | 1408.00 | 1801.00 | 5 |
| ExecutionContextFromMeshGL.CancelConcurrent | 55.00 | 47.00 | 45.00 | 80.00 | 5 |
| Boolean.BatchBoolean | 1.20 | 1.00 | 1.00 | 2.00 | 5 |
| CrossSection.BatchBoolean | 0.20 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Sponge4 | 0.20 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Zebra1 | 2.00 | 2.00 | 2.00 | 2.00 | 5 |
| Polygon.Zebra3 | 798.80 | 788.00 | 774.00 | 862.00 | 5 |

