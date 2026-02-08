# Process Improvement for Ram 1500 Box Assembly (DT Inner)

## Executive Summary
This project targeted critical inefficiencies within the **Ram 1500 (DT Inner)** box assembly line at the Thai Summit Howell facility. By optimizing robotic motion paths, engineering dynamic PLC logic, and transitioning to high-durability consumables, the project achieved a **10% increase in throughput (JPH)** and **zero-downtime model changeovers**.

---

## Product Application: RamBox® Cargo Management System
The **DT Boxside Inner** assembly is the core structural component for the Ram 1500's innovative storage solutions.

![Ram 1500 RamBox Application](./assets/rambox_application.jpg)  

*Figure: The final application of the DT Inner assembly within the Ram 1500.*

---

## Technical Stack
A specialized suite of industrial automation and data tools was utilized to execute these optimizations:
* **PLC Programming:** Omron CX-Programmer (Ladder Logic).
* **HMI Development:** Omron CX-Designer.
* **Robotics:** FANUC HandlingTool (Motion path optimization).
* **Logic Frameworks:** Bit Shift Registers for real-time part tracking.
* **Analysis Tools:** ROI Financial Modeling and OEE (Overall Equipment Effectiveness) analysis.

---

## Implementation: Logic & Robotics
The primary bottleneck involved legacy "static" changeovers that required the entire assembly line to be purged before a new vehicle model could enter.

### **1. Dynamic Part Tracking (Shift Registers)**
I engineered a **dynamic model changeover program** utilizing PLC **shift registers** to track different part types in real-time as they moved through the line. 
* **Mechanism:** Shift registers allow the system to "remember" the specific model of each part at every station along the conveyor, shifting that data forward as the physical part moves.
* **Result:** Eliminated the "line purge" requirement, allowing mixed-model processing with **zero downtime during changeovers**.

### **2. Robotic Cycle Time Optimization**
To increase **Jobs-Per-Hour (JPH)**, I reprogrammed FANUC robotic motion paths to include **"Pounce" or "Pre-pick" positions**.
* **Logic:** Robots now move to a ready-state position closer to the work area during the PLC's idle scan time, significantly shaving seconds off the critical path cycle.

---

## Post-Improvement OEE Data
By identifying and addressing the "Six Big Losses" (Breakdowns, Setup, Idling, Slow Cycles, Startup Rejects, and Production Rejects), the following OEE gains were realized:

| OEE Pillar | Baseline (Pre-Improvement) | Post-Improvement Standard | Improvement |
| :--- | :--- | :--- | :--- |
| **Availability** | ~75% | **88%** | **+13%** (Improved Sequencing and Auto-Cap Changer) |
| **Performance** | ~80% | **91%** | **+11%** (Robotic Pounce Logic) |
| **Quality** | 98.4% | **98.8%** | **+0.4%** (Stable Process Control) |
| **Total OEE** | **~59%** | **~79%** | **+20% Total Efficiency Gain** |


---

## Weld Consumables
The cost of consumables was addressed through a strategic transition in weld consumable hardware and automation.

* **Weld Cap Material:** Transitioned to long-lasting specialized alloys to reduce replacement frequency.
* **Cap Replacement:** Implemented **Automatic Weld Cap Changers** to eliminate manual line stops.
* **Cost Impact:** Realized **$45,000+ in annual savings** through consumable lifecycle extension.

---

## Quantified Impact & Success Metrics
The combined logic and hardware improvements delivered immediate and sustained operational gains:

* **Throughput Increase:** Achieved a **10% increase in parts produced per hour (JPH)**.
* **Downtime Elimination:** Removed legacy model change delays, resulting in **zero downtime** during transitions.
* **Process Reliability:** Standardized Poka-Yoke logic to ensure proper sequencing and prevent missing components.

> *Disclaimer: All data presented has been normalized or rounded to protect proprietary production information. No confidential CAD data or internal plant photography has been used.*
