### Weekly Benchmarks

Commit: `31115d3e82208d804988dfbee91241245604e28a`
Runner: `GitHub Actions 1000000890`
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
| 667 | Intersect12 Q->P | 1121.20 | 0.997 | 446.00 | 672.00 | 0.00 | 3.20 | 5 |
| 695 | Intersect12 P->Q | 477.40 | 0.990 | 332.80 | 140.00 | 4.60 | 0.00 | 5 |
| 16 | Intersect12 Q->P | 412.20 | 0.998 | 162.60 | 248.60 | 0.00 | 1.00 | 5 |
| 84 | Intersect12 P->Q | 371.00 | 0.991 | 213.80 | 154.00 | 2.20 | 1.00 | 5 |
| 260 | Intersect12 Q->P | 164.80 | 0.970 | 72.40 | 87.40 | 2.00 | 3.00 | 5 |
| 406 | Intersect12 P->Q | 134.60 | 0.978 | 83.00 | 48.60 | 3.00 | 0.00 | 5 |
| 551 | Intersect12 P->Q | 104.60 | 0.962 | 58.00 | 42.60 | 4.00 | 0.00 | 5 |
| 582 | Intersect12 P->Q | 43.20 | 1.000 | 24.40 | 18.80 | 0.00 | 0.00 | 5 |

Note: phase timings cover `Intersect12` and `Winding03` only; `Intersections (total)` is excluded from the denominator.

#### perfTest Size Sweep

| nTri | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Peak RSS mean (MB) | Peak RSS min (MB) | Peak RSS max (MB) | Runs |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 512 | 1.33 | 1.04 | 0.85 | 2.02 | 4.80 | 4.62 | 4.95 | 5 |
| 2048 | 2.59 | 2.19 | 1.91 | 4.59 | 6.21 | 6.03 | 6.31 | 5 |
| 8192 | 6.77 | 5.68 | 5.16 | 11.67 | 11.44 | 11.30 | 11.69 | 5 |
| 32768 | 15.75 | 15.29 | 12.60 | 20.80 | 34.08 | 29.72 | 37.42 | 5 |
| 131072 | 59.24 | 57.47 | 44.28 | 80.57 | 121.44 | 106.33 | 132.91 | 5 |
| 524288 | 239.93 | 258.54 | 169.53 | 271.28 | 531.06 | 528.83 | 535.72 | 5 |
| 2097152 | 931.45 | 879.33 | 678.92 | 1329.33 | 1979.06 | 1591.16 | 2080.42 | 5 |
| 8388608 | 13974.40 | 12914.40 | 12372.10 | 18316.70 | 3863.87 | 3146.31 | 4126.05 | 5 |

#### Existing Regression Tests

| Test | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Runs |
|---|---:|---:|---:|---:|---:|
| Manifold.DeepChainDoesNotOverflowNumLeaves | 1905.00 | 1936.00 | 1807.00 | 1995.00 | 5 |
| ExecutionContextFromMeshGL.CancelConcurrent | 60.20 | 55.00 | 47.00 | 85.00 | 5 |
| Boolean.BatchBoolean | 1.40 | 1.00 | 1.00 | 3.00 | 5 |
| CrossSection.BatchBoolean | 0.20 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Sponge4 | 0.20 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Zebra1 | 2.00 | 2.00 | 2.00 | 2.00 | 5 |
| Polygon.Zebra3 | 1010.40 | 951.00 | 924.00 | 1134.00 | 5 |

