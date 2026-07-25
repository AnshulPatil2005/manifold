### Weekly Benchmarks

Commit: `31115d3e82208d804988dfbee91241245604e28a`
Runner: `GitHub Actions 1000001017`
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
| 667 | Intersect12 Q->P | 1031.20 | 0.997 | 408.40 | 619.80 | 0.00 | 3.00 | 5 |
| 695 | Intersect12 P->Q | 445.60 | 0.991 | 313.40 | 128.20 | 4.00 | 0.00 | 5 |
| 16 | Intersect12 Q->P | 382.60 | 0.997 | 153.80 | 227.80 | 0.00 | 1.00 | 5 |
| 84 | Intersect12 P->Q | 339.20 | 0.991 | 192.60 | 143.40 | 2.20 | 1.00 | 5 |
| 260 | Intersect12 Q->P | 150.80 | 0.973 | 66.60 | 80.20 | 1.00 | 3.00 | 5 |
| 406 | Intersect12 P->Q | 122.20 | 0.975 | 75.20 | 44.00 | 3.00 | 0.00 | 5 |
| 551 | Intersect12 P->Q | 95.00 | 0.958 | 53.00 | 38.00 | 4.00 | 0.00 | 5 |
| 582 | Intersect12 P->Q | 40.00 | 1.000 | 22.40 | 17.60 | 0.00 | 0.00 | 5 |

Note: phase timings cover `Intersect12` and `Winding03` only; `Intersections (total)` is excluded from the denominator.

#### perfTest Size Sweep

| nTri | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Peak RSS mean (MB) | Peak RSS min (MB) | Peak RSS max (MB) | Runs |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 512 | 1.07 | 0.83 | 0.77 | 1.95 | 4.78 | 4.73 | 4.81 | 5 |
| 2048 | 2.02 | 1.95 | 1.86 | 2.48 | 6.27 | 6.23 | 6.34 | 5 |
| 8192 | 5.46 | 5.15 | 4.92 | 6.99 | 12.59 | 11.33 | 14.44 | 5 |
| 32768 | 12.47 | 12.41 | 11.85 | 13.75 | 32.07 | 29.64 | 35.42 | 5 |
| 131072 | 44.04 | 43.40 | 41.58 | 49.27 | 119.24 | 109.38 | 128.23 | 5 |
| 524288 | 242.93 | 239.19 | 179.52 | 310.82 | 537.43 | 524.89 | 546.48 | 5 |
| 2097152 | 760.35 | 710.75 | 670.36 | 1027.48 | 1986.57 | 1642.94 | 2073.64 | 5 |
| 8388608 | 11162.44 | 10239.50 | 9611.22 | 15516.30 | 3971.60 | 3234.03 | 4164.44 | 5 |

#### Existing Regression Tests

| Test | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Runs |
|---|---:|---:|---:|---:|---:|
| Manifold.DeepChainDoesNotOverflowNumLeaves | 1544.40 | 1634.00 | 1359.00 | 1677.00 | 5 |
| ExecutionContextFromMeshGL.CancelConcurrent | 51.60 | 52.00 | 45.00 | 59.00 | 5 |
| Boolean.BatchBoolean | 1.20 | 1.00 | 1.00 | 2.00 | 5 |
| CrossSection.BatchBoolean | 0.20 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Sponge4 | 0.20 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Zebra1 | 2.00 | 2.00 | 2.00 | 2.00 | 5 |
| Polygon.Zebra3 | 763.40 | 757.00 | 752.00 | 784.00 | 5 |

