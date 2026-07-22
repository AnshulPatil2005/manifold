### Weekly Benchmarks

Commit: `31115d3e82208d804988dfbee91241245604e28a`
Runner: `GitHub Actions 1000000952`
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
| 667 | Intersect12 Q->P | 1117.80 | 0.997 | 447.60 | 667.00 | 0.00 | 3.20 | 5 |
| 695 | Intersect12 P->Q | 480.40 | 0.990 | 333.80 | 141.80 | 4.80 | 0.00 | 5 |
| 16 | Intersect12 Q->P | 427.00 | 0.998 | 168.40 | 257.60 | 0.00 | 1.00 | 5 |
| 84 | Intersect12 P->Q | 365.80 | 0.991 | 209.20 | 153.20 | 2.40 | 1.00 | 5 |
| 260 | Intersect12 Q->P | 169.40 | 0.969 | 76.00 | 88.20 | 2.00 | 3.20 | 5 |
| 406 | Intersect12 P->Q | 136.60 | 0.977 | 82.80 | 50.60 | 3.20 | 0.00 | 5 |
| 551 | Intersect12 P->Q | 111.00 | 0.961 | 61.60 | 45.00 | 4.20 | 0.20 | 5 |
| 582 | Intersect12 P->Q | 42.80 | 1.000 | 24.20 | 18.60 | 0.00 | 0.00 | 5 |

Note: phase timings cover `Intersect12` and `Winding03` only; `Intersections (total)` is excluded from the denominator.

#### perfTest Size Sweep

| nTri | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Peak RSS mean (MB) | Peak RSS min (MB) | Peak RSS max (MB) | Runs |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 512 | 1.81 | 1.32 | 0.99 | 4.13 | 4.80 | 4.77 | 4.83 | 5 |
| 2048 | 2.93 | 2.74 | 2.66 | 3.67 | 6.32 | 6.25 | 6.59 | 5 |
| 8192 | 11.69 | 12.00 | 6.57 | 17.39 | 12.53 | 11.33 | 13.31 | 5 |
| 32768 | 23.29 | 20.44 | 18.73 | 29.60 | 34.74 | 32.67 | 37.95 | 5 |
| 131072 | 92.96 | 103.58 | 56.68 | 114.15 | 121.29 | 116.72 | 124.52 | 5 |
| 524288 | 498.84 | 456.95 | 416.37 | 697.68 | 528.73 | 520.45 | 541.11 | 5 |
| 2097152 | 2029.60 | 1798.96 | 1580.02 | 3241.07 | 1971.68 | 1560.48 | 2079.03 | 5 |
| 8388608 | 17328.34 | 16313.60 | 14631.40 | 23307.80 | 3965.80 | 3314.58 | 4144.05 | 5 |

#### Existing Regression Tests

| Test | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Runs |
|---|---:|---:|---:|---:|---:|
| Manifold.DeepChainDoesNotOverflowNumLeaves | 2105.40 | 1992.00 | 1633.00 | 2800.00 | 5 |
| ExecutionContextFromMeshGL.CancelConcurrent | 79.40 | 65.00 | 62.00 | 139.00 | 5 |
| Boolean.BatchBoolean | 1.80 | 2.00 | 1.00 | 3.00 | 5 |
| CrossSection.BatchBoolean | 0.20 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Sponge4 | 0.20 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Zebra1 | 2.00 | 2.00 | 2.00 | 2.00 | 5 |
| Polygon.Zebra3 | 907.00 | 938.00 | 793.00 | 1035.00 | 5 |

