### Weekly Benchmarks

Commit: `31115d3e82208d804988dfbee91241245604e28a`
Runner: `GitHub Actions 1000000807`
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
| 667 | Intersect12 Q->P | 1149.00 | 0.997 | 457.80 | 688.20 | 0.00 | 3.00 | 5 |
| 695 | Intersect12 P->Q | 509.00 | 0.990 | 350.20 | 153.80 | 4.80 | 0.20 | 5 |
| 16 | Intersect12 Q->P | 418.80 | 0.998 | 161.40 | 256.40 | 0.00 | 1.00 | 5 |
| 84 | Intersect12 P->Q | 377.40 | 0.991 | 214.80 | 159.20 | 2.40 | 1.00 | 5 |
| 260 | Intersect12 Q->P | 170.60 | 0.971 | 74.20 | 91.40 | 2.00 | 3.00 | 5 |
| 406 | Intersect12 P->Q | 139.80 | 0.977 | 82.00 | 54.60 | 3.20 | 0.00 | 5 |
| 551 | Intersect12 P->Q | 104.60 | 0.962 | 57.20 | 43.40 | 4.00 | 0.00 | 5 |
| 582 | Intersect12 P->Q | 42.80 | 1.000 | 24.60 | 18.20 | 0.00 | 0.00 | 5 |

Note: phase timings cover `Intersect12` and `Winding03` only; `Intersections (total)` is excluded from the denominator.

#### perfTest Size Sweep

| nTri | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Peak RSS mean (MB) | Peak RSS min (MB) | Peak RSS max (MB) | Runs |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 512 | 1.04 | 1.03 | 0.90 | 1.12 | 4.72 | 4.53 | 4.81 | 5 |
| 2048 | 2.65 | 2.46 | 2.12 | 3.74 | 6.19 | 5.66 | 6.77 | 5 |
| 8192 | 6.86 | 6.48 | 5.48 | 10.09 | 12.70 | 11.67 | 13.61 | 5 |
| 32768 | 19.57 | 15.33 | 13.04 | 34.27 | 35.09 | 33.05 | 38.27 | 5 |
| 131072 | 80.69 | 55.65 | 45.89 | 146.51 | 126.65 | 111.22 | 137.11 | 5 |
| 524288 | 377.71 | 361.28 | 278.74 | 554.64 | 533.91 | 525.50 | 546.16 | 5 |
| 2097152 | 1236.62 | 1069.56 | 928.97 | 1706.07 | 2015.13 | 1717.22 | 2106.62 | 5 |
| 8388608 | 13674.04 | 13372.90 | 10677.70 | 17790.30 | 3643.88 | 3005.83 | 3910.45 | 5 |

#### Existing Regression Tests

| Test | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Runs |
|---|---:|---:|---:|---:|---:|
| Manifold.DeepChainDoesNotOverflowNumLeaves | 1733.00 | 1675.00 | 1524.00 | 2040.00 | 5 |
| ExecutionContextFromMeshGL.CancelConcurrent | 66.60 | 71.00 | 48.00 | 83.00 | 5 |
| Boolean.BatchBoolean | 1.60 | 1.00 | 1.00 | 3.00 | 5 |
| CrossSection.BatchBoolean | 0.20 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Sponge4 | 0.20 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Zebra1 | 2.00 | 2.00 | 2.00 | 2.00 | 5 |
| Polygon.Zebra3 | 988.20 | 984.00 | 918.00 | 1094.00 | 5 |

