### Weekly Benchmarks

Commit: `31115d3e82208d804988dfbee91241245604e28a`
Runner: `GitHub Actions 1000000794`
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
| 667 | Intersect12 Q->P | 1053.40 | 0.997 | 420.20 | 630.20 | 0.00 | 3.00 | 5 |
| 695 | Intersect12 P->Q | 451.40 | 0.991 | 314.20 | 133.20 | 4.00 | 0.00 | 5 |
| 16 | Intersect12 Q->P | 383.40 | 0.997 | 151.20 | 231.20 | 0.00 | 1.00 | 5 |
| 84 | Intersect12 P->Q | 337.00 | 0.991 | 193.00 | 141.00 | 2.00 | 1.00 | 5 |
| 260 | Intersect12 Q->P | 152.00 | 0.974 | 67.00 | 81.00 | 1.00 | 3.00 | 5 |
| 406 | Intersect12 P->Q | 122.80 | 0.976 | 75.80 | 44.00 | 3.00 | 0.00 | 5 |
| 551 | Intersect12 P->Q | 95.00 | 0.958 | 53.00 | 38.00 | 4.00 | 0.00 | 5 |
| 582 | Intersect12 P->Q | 40.00 | 1.000 | 22.60 | 17.40 | 0.00 | 0.00 | 5 |

Note: phase timings cover `Intersect12` and `Winding03` only; `Intersections (total)` is excluded from the denominator.

#### perfTest Size Sweep

| nTri | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Peak RSS mean (MB) | Peak RSS min (MB) | Peak RSS max (MB) | Runs |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 512 | 0.97 | 0.89 | 0.76 | 1.53 | 4.78 | 4.58 | 4.89 | 5 |
| 2048 | 1.95 | 1.94 | 1.85 | 2.09 | 6.19 | 5.97 | 6.28 | 5 |
| 8192 | 5.40 | 5.30 | 4.88 | 6.02 | 11.36 | 11.17 | 11.62 | 5 |
| 32768 | 13.22 | 12.19 | 11.76 | 16.93 | 31.19 | 29.62 | 35.45 | 5 |
| 131072 | 48.73 | 42.82 | 40.99 | 64.67 | 119.61 | 101.16 | 138.77 | 5 |
| 524288 | 210.68 | 213.74 | 157.05 | 244.94 | 536.13 | 524.44 | 548.38 | 5 |
| 2097152 | 829.21 | 861.63 | 615.50 | 996.49 | 1953.48 | 1442.31 | 2090.16 | 5 |
| 8388608 | 11154.20 | 10848.20 | 10046.30 | 13428.50 | 3912.19 | 3241.36 | 4156.22 | 5 |

#### Existing Regression Tests

| Test | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Runs |
|---|---:|---:|---:|---:|---:|
| Manifold.DeepChainDoesNotOverflowNumLeaves | 1327.20 | 1329.00 | 1284.00 | 1384.00 | 5 |
| ExecutionContextFromMeshGL.CancelConcurrent | 44.40 | 44.00 | 42.00 | 47.00 | 5 |
| Boolean.BatchBoolean | 1.40 | 1.00 | 1.00 | 2.00 | 5 |
| CrossSection.BatchBoolean | 0.00 | 0.00 | 0.00 | 0.00 | 5 |
| Polygon.Sponge4 | 0.20 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Zebra1 | 2.40 | 2.00 | 2.00 | 4.00 | 5 |
| Polygon.Zebra3 | 755.20 | 753.00 | 750.00 | 768.00 | 5 |

