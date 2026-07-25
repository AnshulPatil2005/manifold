### Weekly Benchmarks

Commit: `31115d3e82208d804988dfbee91241245604e28a`
Runner: `GitHub Actions 1000001010`
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
| 667 | Intersect12 Q->P | 1262.40 | 0.997 | 493.00 | 766.00 | 0.00 | 3.40 | 5 |
| 695 | Intersect12 P->Q | 535.00 | 0.990 | 372.80 | 156.60 | 5.60 | 0.00 | 5 |
| 16 | Intersect12 Q->P | 428.80 | 0.997 | 172.00 | 255.60 | 0.00 | 1.20 | 5 |
| 84 | Intersect12 P->Q | 395.20 | 0.989 | 222.60 | 168.20 | 3.20 | 1.20 | 5 |
| 260 | Intersect12 Q->P | 193.80 | 0.967 | 81.40 | 105.80 | 2.60 | 4.00 | 5 |
| 406 | Intersect12 P->Q | 157.00 | 0.975 | 93.00 | 60.00 | 4.00 | 0.00 | 5 |
| 551 | Intersect12 P->Q | 126.40 | 0.964 | 72.20 | 49.60 | 4.60 | 0.00 | 5 |
| 582 | Intersect12 P->Q | 52.20 | 1.000 | 30.80 | 21.40 | 0.00 | 0.00 | 5 |

Note: phase timings cover `Intersect12` and `Winding03` only; `Intersections (total)` is excluded from the denominator.

#### perfTest Size Sweep

| nTri | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Peak RSS mean (MB) | Peak RSS min (MB) | Peak RSS max (MB) | Runs |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| 512 | 2.39 | 2.48 | 1.38 | 3.84 | 4.68 | 4.50 | 4.89 | 5 |
| 2048 | 6.02 | 3.57 | 3.21 | 10.64 | 6.30 | 6.05 | 6.80 | 5 |
| 8192 | 13.71 | 13.85 | 8.00 | 19.18 | 12.69 | 11.31 | 14.53 | 5 |
| 32768 | 32.35 | 31.10 | 19.96 | 48.98 | 35.82 | 30.27 | 40.19 | 5 |
| 131072 | 104.47 | 102.56 | 81.36 | 140.17 | 118.99 | 116.45 | 120.77 | 5 |
| 524288 | 465.43 | 417.12 | 394.66 | 556.04 | 530.60 | 525.72 | 537.45 | 5 |
| 2097152 | 1762.39 | 1796.83 | 1512.50 | 1936.07 | 1962.63 | 1496.33 | 2088.12 | 5 |
| 8388608 | 22899.82 | 20430.90 | 17133.40 | 35775.90 | 3828.58 | 2980.03 | 4122.11 | 5 |

#### Existing Regression Tests

| Test | Mean (ms) | Median (ms) | Min (ms) | Max (ms) | Runs |
|---|---:|---:|---:|---:|---:|
| Manifold.DeepChainDoesNotOverflowNumLeaves | 2599.80 | 2459.00 | 2261.00 | 3323.00 | 5 |
| ExecutionContextFromMeshGL.CancelConcurrent | 110.80 | 104.00 | 75.00 | 165.00 | 5 |
| Boolean.BatchBoolean | 2.80 | 3.00 | 2.00 | 4.00 | 5 |
| CrossSection.BatchBoolean | 0.40 | 0.00 | 0.00 | 1.00 | 5 |
| Polygon.Sponge4 | 0.80 | 1.00 | 0.00 | 2.00 | 5 |
| Polygon.Zebra1 | 3.20 | 2.00 | 2.00 | 6.00 | 5 |
| Polygon.Zebra3 | 1236.80 | 1286.00 | 1069.00 | 1330.00 | 5 |

