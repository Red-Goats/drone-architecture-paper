# Fig. 1 — Conceptual System Architecture

*Distributed Embedded Architecture for Modular Unmanned Aerial Systems*

```
             +-----------------------+
             |    Ground Interface   |
             |  (Command / Telemetry)|
             +-----------+-----------+
                         |
                         v
             +-----------------------+
             |  Flight Control Node  |
             |-----------------------|
             | - Power Management    |
             | - Attitude Control    |
             | - Stabilization Loops |
             | - System Monitoring   |
             | - Fail-Safe Modes     |
             +-----------+-----------+
                         |
                 [Data Interface Layer]
               (Asynchronous / Fault-Tolerant)
                         |
             +-----------v-----------+
             |   Sensor Processing   |
             |         Node          |
             |-----------------------|
             | - Thermal Sensing     |
             | - Visual Processing   |
             | - IMU Aggregation     |
             | - Altitude Estimation |
             | - Sensor Fusion       |
             | - Data Conditioning   |
             +-----------------------+
```

**Note:** This diagram represents a conceptual model only. No specific hardware implementations, component selections, or physical interconnects are depicted. Refer to Section II of `paper.md` for architectural context.
