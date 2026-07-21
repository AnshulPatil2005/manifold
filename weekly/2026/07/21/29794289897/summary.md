### Weekly Benchmarks

Commit: `31115d3e82208d804988dfbee91241245604e28a`
Runner: `GitHub Actions 1000000928`
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
| 667 | Intersect12 Q->P | 1254.60 | 0.997 | 500.00 | 751.20 | 0.00 | 3.40 | 5 |
| 695 | Intersect12 P->Q | 525.40 | 0.989 | 358.40 | 161.40 | 5.60 | 0.00 | 5 |
| 16 | Intersect12 Q->P | 482.00 | 0.998 | 181.80 | 299.00 | 0.00 | 1.20 | 5 |
| 84 | Intersect12 P->Q | 415.20 | 0.991 | 240.60 | 170.80 | 2.80 | 1.00 | 5 |
| 260 | Intersect12 Q->P | 182.40 | 0.969 | 83.00 | 93.80 | 2.00 | 3.60 | 5 |
| 406 | Intersect12 P->Q | 152.40 | 0.976 | 94.20 | 54.60 | 3.60 | 0.00 | 5 |
| 551 | Intersect12 P->Q | 115.80 | 0.960 | 65.80 | 45.40 | 4.60 | 0.00 | 5 |
| 582 | Intersect12 P->Q | 45.20 | 0.996 | 25.20 | 19.80 | 0.20 | 0.00 | 5 |

Note: phase timings cover `Intersect12` and `Winding03` only; `Intersections (total)` is excluded from the denominator.

#### perfTest Size Sweep

| nTri | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Peak RSS mean (MB) | Peak RSS min (MB) | Peak RSS max (MB) | Runs |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 512 | 1.96 | 1.62 | 1.49 | 2.81 | 4.66 | 4.27 | 4.92 | 5 |
| 2048 | 2.93 | 2.47 | 2.37 | 4.05 | 6.36 | 6.27 | 6.69 | 5 |
| 8192 | 11.36 | 9.67 | 6.78 | 20.21 | 12.75 | 11.70 | 13.47 | 5 |
| 32768 | 26.12 | 24.63 | 19.49 | 34.06 | 33.79 | 31.33 | 35.30 | 5 |
| 131072 | 89.06 | 80.29 | 67.73 | 115.81 | 123.86 | 113.84 | 131.91 | 5 |
| 524288 | 473.76 | 478.76 | 377.65 | 548.06 | 528.27 | 520.81 | 538.02 | 5 |
| 2097152 | 1834.12 | 1786.96 | 1511.65 | 2530.70 | 1973.77 | 1544.48 | 2088.08 | 5 |
| 8388608 | 17346.62 | 15742.90 | 15295.40 | 21786.40 | 3949.03 | 3297.69 | 4149.33 | 5 |

#### Existing Regression Tests

| Test | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Runs |
|---|---:|---:|---:|---:|---:|
| Manifold.DeepChainDoesNotOverflowNumLeaves | 2258.20 | 2167.00 | 2148.00 | 2631.00 | 5 |
| ExecutionContextFromMeshGL.CancelConcurrent | 94.60 | 83.00 | 69.00 | 131.00 | 5 |
| Boolean.BatchBoolean | 2.80 | 3.00 | 1.00 | 4.00 | 5 |
| CrossSection.BatchBoolean | 0.20 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Sponge4 | 1.00 | 1.00 | 1.00 | 1.00 | 5 |
| Polygon.Zebra1 | 2.40 | 2.00 | 2.00 | 3.00 | 5 |
| Polygon.Zebra3 | 1100.40 | 1062.00 | 1052.00 | 1237.00 | 5 |

