# Server-Based Alcatel-Lucent PBX — SAIL/BSL

Documentation project from a 4-week practical training at **Bokaro Steel Plant (Steel Authority of India Limited)**, Electronics & Telecom Department, studying the design and operation of a large-scale server-based telephony system.

**Duration:** May 13 – June 7, 2024
**Organization:** SAIL, Bokaro Steel Plant

## Overview

The project covers the architecture and working of an **Alcatel-Lucent OmniPCX Enterprise** server-based PBX deployed across BSL's Plant, Admin, and Township exchanges — a multi-site industrial campus network wired for 7,000+ and 3,000+ subscriber lines at the Plant and Admin locations respectively, with additional passive servers at Coke Oven, Blast Furnace, CRM, and Township locations.

## What's Covered

- **System architecture** — logical network diagram across Plant Exchange, Admin Building, Township Exchange, and Remote Line Units (RLUs), connected via a duplicated LAN and fiber/copper backbone.
- **Call-server redundancy** — main/hot-standby failover between Plant and Admin call-server stacks, including a cold-standby tier and continuous database synchronization between active and standby servers.
- **Media gateways** — ACT14/ACT28 gateway hardware, peripheral card functions (analog/digital interfaces, PRI trunk cards, VoIP interface cards), and their role in connecting exchanges over the campus data network.
- **Passive Communication Server (PCS) survivability** — how remote sites maintain basic telephony service during central-site outages or IP-link failures, including automatic/manual database sync and reset-timer behavior.
- **Integrated services** — IVRS-based complaint handling system, Alcatel 4635H voice mail system, and the OmniTouch audio/web conferencing platform.
- **General maintenance & diagnostics** — key command-line tools used to monitor and troubleshoot the system (`config`, `cplstat`, `trkstat`, `incvisu`, `intipstat`, `ippstat`, `twin`, `role`, `pcsview`), covering board status checks, trunk state monitoring, incident logging, and IP phone diagnostics.

## Key Takeaway

The project gave hands-on exposure to how large industrial organizations architect mission-critical, fault-tolerant voice communication infrastructure — balancing redundancy (hot-standby, passive failover), centralized control, and converged voice/data (VoIP) delivery across a geographically distributed plant network.
