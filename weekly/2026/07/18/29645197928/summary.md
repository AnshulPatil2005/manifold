### Weekly Benchmarks

Commit: `31115d3e82208d804988dfbee91241245604e28a`
Runner: `GitHub Actions 1000000876`
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
| 667 | Intersect12 Q->P | 1203.20 | 0.997 | 476.60 | 723.20 | 0.00 | 3.40 | 5 |
| 695 | Intersect12 P->Q | 492.60 | 0.989 | 342.80 | 144.60 | 5.20 | 0.00 | 5 |
| 16 | Intersect12 Q->P | 465.60 | 0.997 | 178.00 | 286.20 | 0.00 | 1.40 | 5 |
| 84 | Intersect12 P->Q | 394.40 | 0.991 | 226.60 | 164.20 | 2.40 | 1.20 | 5 |
| 260 | Intersect12 Q->P | 184.60 | 0.971 | 83.00 | 96.40 | 2.00 | 3.20 | 5 |
| 406 | Intersect12 P->Q | 137.20 | 0.975 | 84.60 | 49.20 | 3.40 | 0.00 | 5 |
| 551 | Intersect12 P->Q | 116.60 | 0.956 | 62.20 | 49.20 | 5.20 | 0.00 | 5 |
| 582 | Intersect12 P->Q | 54.00 | 0.997 | 32.00 | 21.80 | 0.20 | 0.00 | 5 |

Note: phase timings cover `Intersect12` and `Winding03` only; `Intersections (total)` is excluded from the denominator.

#### perfTest Size Sweep

| nTri | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Peak RSS mean (MB) | Peak RSS min (MB) | Peak RSS max (MB) | Runs |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 512 | 2.31 | 2.23 | 1.81 | 2.95 | 4.80 | 4.61 | 4.92 | 5 |
| 2048 | 4.88 | 5.34 | 2.28 | 7.66 | 6.37 | 6.23 | 6.83 | 5 |
| 8192 | 14.76 | 13.58 | 7.91 | 26.88 | 12.74 | 11.73 | 13.42 | 5 |
| 32768 | 34.71 | 37.44 | 20.18 | 41.14 | 35.34 | 32.22 | 36.73 | 5 |
| 131072 | 134.42 | 134.48 | 77.23 | 226.33 | 123.67 | 117.36 | 128.84 | 5 |
| 524288 | 469.49 | 540.99 | 210.26 | 624.40 | 538.31 | 514.08 | 554.92 | 5 |
| 2097152 | 2263.35 | 2183.62 | 1855.93 | 3130.02 | 1995.73 | 1664.16 | 2092.12 | 5 |
| 8388608 | 20729.52 | 20664.30 | 12152.00 | 30756.80 | 3922.58 | 3225.06 | 4183.92 | 5 |

#### Existing Regression Tests

| Test | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Runs |
|---|---:|---:|---:|---:|---:|
| Manifold.DeepChainDoesNotOverflowNumLeaves | 2360.00 | 2178.00 | 1972.00 | 3122.00 | 5 |
| ExecutionContextFromMeshGL.CancelConcurrent | 99.80 | 85.00 | 72.00 | 141.00 | 5 |
| Boolean.BatchBoolean | 2.60 | 2.00 | 1.00 | 5.00 | 5 |
| CrossSection.BatchBoolean | 0.20 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Sponge4 | 0.80 | 1.00 | 0.00 | 1.00 | 5 |
| Polygon.Zebra1 | 2.20 | 2.00 | 2.00 | 3.00 | 5 |
| Polygon.Zebra3 | 978.00 | 1028.00 | 817.00 | 1152.00 | 5 |

