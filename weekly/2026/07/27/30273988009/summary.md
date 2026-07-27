### Weekly Benchmarks

Commit: `31115d3e82208d804988dfbee91241245604e28a`
Runner: `GitHub Actions 1000001056`
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
| 667 | Intersect12 Q->P | 1985.20 | 0.997 | 785.40 | 1194.40 | 0.20 | 5.20 | 5 |
| 695 | Intersect12 P->Q | 903.20 | 0.986 | 615.40 | 274.00 | 13.80 | 0.00 | 5 |
| 16 | Intersect12 Q->P | 676.60 | 0.997 | 271.00 | 403.80 | 0.00 | 1.80 | 5 |
| 84 | Intersect12 P->Q | 633.40 | 0.991 | 355.00 | 273.00 | 3.60 | 1.80 | 5 |
| 260 | Intersect12 Q->P | 348.20 | 0.969 | 153.80 | 183.60 | 3.60 | 7.20 | 5 |
| 406 | Intersect12 P->Q | 213.40 | 0.974 | 128.60 | 79.20 | 5.60 | 0.00 | 5 |
| 551 | Intersect12 P->Q | 198.20 | 0.968 | 111.80 | 80.20 | 6.20 | 0.00 | 5 |
| 582 | Intersect12 Q->P | 86.20 | 0.993 | 42.20 | 43.40 | 0.60 | 0.00 | 5 |

Note: phase timings cover `Intersect12` and `Winding03` only; `Intersections (total)` is excluded from the denominator.

#### perfTest Size Sweep

| nTri | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Peak RSS mean (MB) | Peak RSS min (MB) | Peak RSS max (MB) | Runs |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 512 | 2.54 | 2.51 | 1.12 | 3.54 | 4.82 | 4.64 | 4.97 | 5 |
| 2048 | 6.64 | 3.77 | 3.16 | 16.99 | 6.41 | 6.09 | 7.16 | 5 |
| 8192 | 15.20 | 12.78 | 6.38 | 26.55 | 12.84 | 11.50 | 14.59 | 5 |
| 32768 | 34.24 | 33.47 | 17.79 | 63.04 | 34.11 | 30.80 | 38.41 | 5 |
| 131072 | 132.70 | 111.02 | 54.69 | 292.52 | 117.94 | 110.58 | 126.11 | 5 |
| 524288 | 677.33 | 678.43 | 421.47 | 917.54 | 518.41 | 435.58 | 557.53 | 5 |
| 2097152 | 2134.92 | 2181.32 | 1057.91 | 2743.90 | 1984.84 | 1608.62 | 2092.42 | 5 |
| 8388608 | 27746.38 | 26577.30 | 22834.50 | 35448.20 | 3869.78 | 3172.34 | 4128.97 | 5 |

#### Existing Regression Tests

| Test | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Runs |
|---|---:|---:|---:|---:|---:|
| Manifold.DeepChainDoesNotOverflowNumLeaves | 1872.60 | 1681.00 | 1596.00 | 2400.00 | 5 |
| ExecutionContextFromMeshGL.CancelConcurrent | 68.20 | 70.00 | 50.00 | 92.00 | 5 |
| Boolean.BatchBoolean | 1.80 | 2.00 | 1.00 | 3.00 | 5 |
| CrossSection.BatchBoolean | 0.20 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Sponge4 | 0.20 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Zebra1 | 2.00 | 2.00 | 2.00 | 2.00 | 5 |
| Polygon.Zebra3 | 917.80 | 922.00 | 849.00 | 996.00 | 5 |

