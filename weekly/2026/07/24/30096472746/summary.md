### Weekly Benchmarks

Commit: `31115d3e82208d804988dfbee91241245604e28a`
Runner: `GitHub Actions 1000000997`
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
| 667 | Intersect12 Q->P | 1178.80 | 0.997 | 475.00 | 700.40 | 0.00 | 3.40 | 5 |
| 695 | Intersect12 P->Q | 513.80 | 0.990 | 349.60 | 159.00 | 5.20 | 0.00 | 5 |
| 16 | Intersect12 Q->P | 439.00 | 0.997 | 175.60 | 262.00 | 0.00 | 1.40 | 5 |
| 84 | Intersect12 P->Q | 393.80 | 0.990 | 224.00 | 165.80 | 3.00 | 1.00 | 5 |
| 260 | Intersect12 Q->P | 174.80 | 0.970 | 77.40 | 92.20 | 2.00 | 3.20 | 5 |
| 406 | Intersect12 P->Q | 139.00 | 0.978 | 85.80 | 50.20 | 3.00 | 0.00 | 5 |
| 551 | Intersect12 P->Q | 111.00 | 0.960 | 61.40 | 45.20 | 4.40 | 0.00 | 5 |
| 582 | Intersect12 P->Q | 48.20 | 0.996 | 27.20 | 20.80 | 0.20 | 0.00 | 5 |

Note: phase timings cover `Intersect12` and `Winding03` only; `Intersections (total)` is excluded from the denominator.

#### perfTest Size Sweep

| nTri | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Peak RSS mean (MB) | Peak RSS min (MB) | Peak RSS max (MB) | Runs |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 512 | 1.15 | 1.06 | 0.98 | 1.52 | 4.77 | 4.64 | 4.91 | 5 |
| 2048 | 2.97 | 2.35 | 2.05 | 5.60 | 6.32 | 6.22 | 6.61 | 5 |
| 8192 | 6.96 | 5.78 | 5.36 | 12.23 | 11.72 | 11.30 | 12.81 | 5 |
| 32768 | 21.92 | 15.17 | 13.37 | 50.74 | 35.21 | 31.81 | 37.69 | 5 |
| 131072 | 61.90 | 59.15 | 42.89 | 95.39 | 115.63 | 105.84 | 124.77 | 5 |
| 524288 | 389.53 | 331.52 | 253.54 | 552.59 | 531.52 | 523.22 | 534.95 | 5 |
| 2097152 | 1676.02 | 1367.22 | 898.04 | 3733.92 | 1968.33 | 1521.78 | 2089.97 | 5 |
| 8388608 | 15460.66 | 13275.40 | 11721.80 | 24004.90 | 3962.60 | 3221.69 | 4157.11 | 5 |

#### Existing Regression Tests

| Test | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Runs |
|---|---:|---:|---:|---:|---:|
| Manifold.DeepChainDoesNotOverflowNumLeaves | 1784.80 | 1780.00 | 1629.00 | 1980.00 | 5 |
| ExecutionContextFromMeshGL.CancelConcurrent | 57.60 | 60.00 | 52.00 | 60.00 | 5 |
| Boolean.BatchBoolean | 2.00 | 2.00 | 1.00 | 3.00 | 5 |
| CrossSection.BatchBoolean | 0.20 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Sponge4 | 0.20 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Zebra1 | 2.00 | 2.00 | 2.00 | 2.00 | 5 |
| Polygon.Zebra3 | 918.00 | 916.00 | 891.00 | 959.00 | 5 |

