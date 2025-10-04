# Mesh Topology Implementation

## Overview
Full-mesh between nodes modeled by connecting each PC to a dedicated switch and interconnecting switches in a full mesh.

## Devices
- 4 × PCs
- 4 × Cisco 2960 switches
- 6 × inter-switch links (copper/fiber)

## IP Addressing
| Device | IPv4 Address     |
|--------|------------------|
| PC0    | 192.168.2.2      |
| PC1    | 192.168.2.3      |
| PC2    | 192.168.2.4      |
| PC3    | 192.168.2.5      |

IPv6 addresses follow `2001:DB8:ACAD:2::X/64`.

## How to verify
1. Open `Mesh_Topology.pkt`.
2. From each PC ping every other PC (expect replies, STP might block some L2 paths).
3. Evidence:
   - `screenshots topology.png`
   - `screenshots ip_config.png`
   - `screenshots ping_test.png`

