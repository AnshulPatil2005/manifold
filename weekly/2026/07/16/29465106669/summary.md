### Weekly Benchmarks

Commit: `31115d3e82208d804988dfbee91241245604e28a`
Runner: `GitHub Actions 1000000826`
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
| 667 | Intersect12 Q->P | 1126.00 | 0.997 | 448.60 | 674.40 | 0.00 | 3.00 | 5 |
| 695 | Intersect12 P->Q | 509.80 | 0.989 | 347.60 | 156.80 | 5.40 | 0.00 | 5 |
| 16 | Intersect12 Q->P | 417.60 | 0.998 | 166.40 | 250.20 | 0.00 | 1.00 | 5 |
| 84 | Intersect12 P->Q | 384.40 | 0.992 | 223.20 | 158.00 | 2.20 | 1.00 | 5 |
| 260 | Intersect12 Q->P | 170.00 | 0.966 | 74.00 | 90.20 | 2.20 | 3.60 | 5 |
| 406 | Intersect12 P->Q | 144.60 | 0.979 | 88.80 | 52.80 | 3.00 | 0.00 | 5 |
| 551 | Intersect12 P->Q | 108.00 | 0.960 | 60.00 | 43.60 | 4.40 | 0.00 | 5 |
| 582 | Intersect12 P->Q | 44.00 | 1.000 | 25.20 | 18.80 | 0.00 | 0.00 | 5 |

Note: phase timings cover `Intersect12` and `Winding03` only; `Intersections (total)` is excluded from the denominator.

#### perfTest Size Sweep

| nTri | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Peak RSS mean (MB) | Peak RSS min (MB) | Peak RSS max (MB) | Runs |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 512 | 3.83 | 2.66 | 1.04 | 7.59 | 4.76 | 4.69 | 4.83 | 5 |
| 2048 | 3.91 | 3.84 | 2.35 | 5.74 | 6.41 | 6.17 | 6.72 | 5 |
| 8192 | 13.00 | 14.75 | 6.69 | 18.48 | 12.47 | 11.31 | 13.16 | 5 |
| 32768 | 29.64 | 30.92 | 18.87 | 40.67 | 34.34 | 33.33 | 35.62 | 5 |
| 131072 | 118.84 | 124.78 | 66.21 | 148.31 | 128.21 | 119.14 | 136.19 | 5 |
| 524288 | 487.56 | 497.98 | 454.54 | 516.85 | 534.03 | 527.08 | 547.23 | 5 |
| 2097152 | 1824.08 | 1800.05 | 1641.12 | 2026.00 | 1971.28 | 1532.05 | 2092.48 | 5 |
| 8388608 | 18423.56 | 16997.40 | 16448.20 | 24584.20 | 3949.02 | 3127.66 | 4177.42 | 5 |

#### Existing Regression Tests

| Test | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Runs |
|---|---:|---:|---:|---:|---:|
| Manifold.DeepChainDoesNotOverflowNumLeaves | 2363.60 | 2193.00 | 2115.00 | 2752.00 | 5 |
| ExecutionContextFromMeshGL.CancelConcurrent | 99.20 | 94.00 | 81.00 | 118.00 | 5 |
| Boolean.BatchBoolean | 3.00 | 3.00 | 1.00 | 5.00 | 5 |
| CrossSection.BatchBoolean | 0.20 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Sponge4 | 0.40 | 0.00 | 0.00 | 2.00 | 5 |
| Polygon.Zebra1 | 2.00 | 2.00 | 2.00 | 2.00 | 5 |
| Polygon.Zebra3 | 1066.00 | 1017.00 | 982.00 | 1194.00 | 5 |

