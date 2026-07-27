### Weekly Benchmarks

Commit: `31115d3e82208d804988dfbee91241245604e28a`
Runner: `GitHub Actions 1000001051`
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
| 667 | Intersect12 Q->P | 1188.80 | 0.997 | 497.20 | 688.40 | 0.00 | 3.20 | 5 |
| 695 | Intersect12 P->Q | 503.80 | 0.990 | 353.20 | 145.60 | 5.00 | 0.00 | 5 |
| 16 | Intersect12 Q->P | 440.80 | 0.998 | 178.00 | 261.80 | 0.00 | 1.00 | 5 |
| 84 | Intersect12 P->Q | 389.60 | 0.991 | 220.60 | 165.40 | 2.60 | 1.00 | 5 |
| 260 | Intersect12 Q->P | 175.20 | 0.970 | 77.40 | 92.60 | 2.00 | 3.20 | 5 |
| 406 | Intersect12 P->Q | 142.20 | 0.975 | 86.00 | 52.60 | 3.60 | 0.00 | 5 |
| 551 | Intersect12 P->Q | 110.80 | 0.955 | 59.80 | 46.00 | 5.00 | 0.00 | 5 |
| 582 | Intersect12 P->Q | 46.80 | 1.000 | 27.20 | 19.60 | 0.00 | 0.00 | 5 |

Note: phase timings cover `Intersect12` and `Winding03` only; `Intersections (total)` is excluded from the denominator.

#### perfTest Size Sweep

| nTri | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Peak RSS mean (MB) | Peak RSS min (MB) | Peak RSS max (MB) | Runs |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 512 | 1.47 | 1.41 | 0.98 | 2.00 | 4.77 | 4.72 | 4.80 | 5 |
| 2048 | 4.58 | 4.67 | 2.24 | 6.25 | 6.32 | 6.20 | 6.66 | 5 |
| 8192 | 11.54 | 12.63 | 7.47 | 14.99 | 12.98 | 12.56 | 13.86 | 5 |
| 32768 | 29.53 | 33.11 | 18.66 | 35.67 | 34.97 | 30.98 | 37.33 | 5 |
| 131072 | 108.86 | 105.41 | 64.68 | 154.20 | 124.20 | 114.48 | 132.67 | 5 |
| 524288 | 535.41 | 464.30 | 433.25 | 813.38 | 531.56 | 517.23 | 540.17 | 5 |
| 2097152 | 1788.87 | 1734.32 | 1516.70 | 2128.90 | 1962.09 | 1496.88 | 2084.19 | 5 |
| 8388608 | 17617.44 | 16978.80 | 14479.50 | 23347.90 | 3938.14 | 3277.80 | 4125.80 | 5 |

#### Existing Regression Tests

| Test | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Runs |
|---|---:|---:|---:|---:|---:|
| Manifold.DeepChainDoesNotOverflowNumLeaves | 2322.60 | 2200.00 | 2120.00 | 2723.00 | 5 |
| ExecutionContextFromMeshGL.CancelConcurrent | 109.00 | 109.00 | 80.00 | 138.00 | 5 |
| Boolean.BatchBoolean | 2.20 | 2.00 | 2.00 | 3.00 | 5 |
| CrossSection.BatchBoolean | 0.20 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Sponge4 | 0.40 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Zebra1 | 2.00 | 2.00 | 2.00 | 2.00 | 5 |
| Polygon.Zebra3 | 985.20 | 967.00 | 909.00 | 1063.00 | 5 |

