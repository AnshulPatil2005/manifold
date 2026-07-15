### Weekly Benchmarks

Commit: `31115d3e82208d804988dfbee91241245604e28a`
Runner: `GitHub Actions 1000000814`
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
| 667 | Intersect12 Q->P | 1183.60 | 0.997 | 468.40 | 712.20 | 0.00 | 3.00 | 5 |
| 695 | Intersect12 P->Q | 526.80 | 0.991 | 369.20 | 152.80 | 4.80 | 0.00 | 5 |
| 16 | Intersect12 Q->P | 442.80 | 0.998 | 181.00 | 260.80 | 0.00 | 1.00 | 5 |
| 84 | Intersect12 P->Q | 394.40 | 0.990 | 224.40 | 166.20 | 2.80 | 1.00 | 5 |
| 260 | Intersect12 Q->P | 184.40 | 0.968 | 82.20 | 96.40 | 2.60 | 3.20 | 5 |
| 406 | Intersect12 P->Q | 146.80 | 0.979 | 91.80 | 52.00 | 3.00 | 0.00 | 5 |
| 551 | Intersect12 P->Q | 112.80 | 0.964 | 64.40 | 44.40 | 4.00 | 0.00 | 5 |
| 582 | Intersect12 P->Q | 42.80 | 1.000 | 24.20 | 18.60 | 0.00 | 0.00 | 5 |

Note: phase timings cover `Intersect12` and `Winding03` only; `Intersections (total)` is excluded from the denominator.

#### perfTest Size Sweep

| nTri | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Peak RSS mean (MB) | Peak RSS min (MB) | Peak RSS max (MB) | Runs |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 512 | 2.75 | 1.77 | 0.86 | 7.78 | 4.76 | 4.47 | 4.91 | 5 |
| 2048 | 3.81 | 3.79 | 2.22 | 5.49 | 5.96 | 5.73 | 6.25 | 5 |
| 8192 | 13.78 | 13.37 | 6.52 | 23.07 | 12.65 | 11.69 | 13.45 | 5 |
| 32768 | 36.27 | 33.21 | 23.69 | 48.81 | 33.94 | 32.09 | 37.08 | 5 |
| 131072 | 168.65 | 178.60 | 72.16 | 279.01 | 125.27 | 122.05 | 129.98 | 5 |
| 524288 | 669.70 | 583.03 | 435.42 | 1030.87 | 535.78 | 531.27 | 540.67 | 5 |
| 2097152 | 1926.31 | 1994.21 | 1580.79 | 2304.10 | 1987.00 | 1591.97 | 2104.05 | 5 |
| 8388608 | 19170.16 | 18044.90 | 14960.30 | 26404.30 | 3745.32 | 3013.61 | 4043.52 | 5 |

#### Existing Regression Tests

| Test | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Runs |
|---|---:|---:|---:|---:|---:|
| Manifold.DeepChainDoesNotOverflowNumLeaves | 3293.80 | 3463.00 | 2444.00 | 3974.00 | 5 |
| ExecutionContextFromMeshGL.CancelConcurrent | 114.20 | 107.00 | 77.00 | 145.00 | 5 |
| Boolean.BatchBoolean | 3.00 | 3.00 | 2.00 | 5.00 | 5 |
| CrossSection.BatchBoolean | 0.60 | 1.00 | 0.00 | 1.00 | 5 |
| Polygon.Sponge4 | 1.20 | 1.00 | 1.00 | 2.00 | 5 |
| Polygon.Zebra1 | 3.00 | 2.00 | 2.00 | 5.00 | 5 |
| Polygon.Zebra3 | 1568.20 | 1554.00 | 1505.00 | 1671.00 | 5 |

