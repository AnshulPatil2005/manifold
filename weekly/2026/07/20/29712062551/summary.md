### Weekly Benchmarks

Commit: `31115d3e82208d804988dfbee91241245604e28a`
Runner: `GitHub Actions 1000000912`
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
| 667 | Intersect12 Q->P | 1040.60 | 0.997 | 415.20 | 622.20 | 0.00 | 3.20 | 5 |
| 695 | Intersect12 P->Q | 445.80 | 0.991 | 310.80 | 131.00 | 4.00 | 0.00 | 5 |
| 16 | Intersect12 Q->P | 386.80 | 0.997 | 152.40 | 233.40 | 0.00 | 1.00 | 5 |
| 84 | Intersect12 P->Q | 344.60 | 0.991 | 197.00 | 144.60 | 2.00 | 1.00 | 5 |
| 260 | Intersect12 Q->P | 151.60 | 0.974 | 67.00 | 80.60 | 1.00 | 3.00 | 5 |
| 406 | Intersect12 P->Q | 123.80 | 0.976 | 76.00 | 44.80 | 3.00 | 0.00 | 5 |
| 551 | Intersect12 P->Q | 95.00 | 0.958 | 53.00 | 38.00 | 4.00 | 0.00 | 5 |
| 582 | Intersect12 P->Q | 40.20 | 1.000 | 22.60 | 17.60 | 0.00 | 0.00 | 5 |

Note: phase timings cover `Intersect12` and `Winding03` only; `Intersections (total)` is excluded from the denominator.

#### perfTest Size Sweep

| nTri | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Peak RSS mean (MB) | Peak RSS min (MB) | Peak RSS max (MB) | Runs |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 512 | 1.19 | 1.19 | 0.76 | 1.66 | 4.68 | 4.48 | 4.81 | 5 |
| 2048 | 1.98 | 1.98 | 1.86 | 2.17 | 6.35 | 6.25 | 6.72 | 5 |
| 8192 | 5.32 | 5.22 | 4.97 | 6.16 | 11.32 | 11.30 | 11.34 | 5 |
| 32768 | 12.76 | 12.72 | 11.77 | 13.89 | 33.27 | 29.64 | 37.23 | 5 |
| 131072 | 44.90 | 46.49 | 41.55 | 46.87 | 128.57 | 123.77 | 135.92 | 5 |
| 524288 | 321.89 | 243.67 | 174.81 | 643.73 | 537.04 | 518.75 | 575.72 | 5 |
| 2097152 | 865.76 | 741.65 | 666.50 | 1430.90 | 1988.99 | 1623.50 | 2092.09 | 5 |
| 8388608 | 11743.84 | 10871.60 | 10241.50 | 15638.40 | 4004.16 | 3400.41 | 4168.58 | 5 |

#### Existing Regression Tests

| Test | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Runs |
|---|---:|---:|---:|---:|---:|
| Manifold.DeepChainDoesNotOverflowNumLeaves | 1478.80 | 1457.00 | 1366.00 | 1609.00 | 5 |
| ExecutionContextFromMeshGL.CancelConcurrent | 48.60 | 46.00 | 44.00 | 56.00 | 5 |
| Boolean.BatchBoolean | 1.20 | 1.00 | 1.00 | 2.00 | 5 |
| CrossSection.BatchBoolean | 0.20 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Sponge4 | 0.00 | 0.00 | 0.00 | 0.00 | 5 |
| Polygon.Zebra1 | 2.00 | 2.00 | 2.00 | 2.00 | 5 |
| Polygon.Zebra3 | 778.60 | 758.00 | 748.00 | 867.00 | 5 |

