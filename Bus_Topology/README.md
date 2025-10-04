# Bus Topology Implementation

## Overview
Classic bus-like network simulated using a Hub (shared medium). Four PCs connected to the same broadcast domain.

## Devices Used
- 4 × PCs (PC0–PC3)
- 1 × Hub-PT
- 4 × Copper Straight-Through cables

## IPv4 Addressing
| Device | IPv4 Address  | Subnet Mask     |
|--------|---------------|-----------------|
| PC0    | 192.168.1.2   | 255.255.255.0   |
| PC1    | 192.168.1.3   | 255.255.255.0   |
| PC2    | 192.168.1.4   | 255.255.255.0   |
| PC3    | 192.168.1.5   | 255.255.255.0   |

## IPv6 Addressing
| Device | IPv6 Address              | Prefix |
|--------|---------------------------|--------|
| PC0    | 2001:DB8:ACAD:1::2        | 64     |
| PC1    | 2001:DB8:ACAD:1::3        | 64     |
| PC2    | 2001:DB8:ACAD:1::4        | 64     |
| PC3    | 2001:DB8:ACAD:1::5        | 64     |

## How to verify
1. Open `Bus_Topology.pkt`.
2. On PC0: Desktop → Command Prompt → `ping 192.168.1.3` and `ping 2001:DB8:ACAD:1::3`.
3. Expect replies for both IPv4 and IPv6.

## Files / Evidence
- `Bus_Topology.pkt`
- `screenshots topology.png`
- `screenshots ip_config.png`
- `screenshots ping_tests.png`

