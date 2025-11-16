# Week 7 - RISC-V SoC Tapeout Journey (Divya Darshan)
[![Repo Size](https://img.shields.io/github/repo-size/DivyaDarshan09/Divya_Darshan-VSD-RISCV-week-7)](https://github.com/DivyaDarshan09/Divya_Darshan-VSD-RISCV-week-7)
[![Owner](https://img.shields.io/badge/Owner-DivyaDarshan09-red)](https://github.com/DivyaDarshan09)

---
This repository documents the work done in Week 7 of my 20-week RISC-V SoC Tapeout project powered by VLSI System Design (VSD) and IIT Gandhinagar.

---
## Introduction
- This repository documents the complete Physical Design flow executed for the VSDBabySoC using the OpenROAD open-source EDA tool.
- The goal of this week’s task is to experience a real SoC backend flow — from RTL all the way to post-route parasitic extraction.

**This includes:**

1. Synthesis
2. Floorplanning
3. Placement
4. Clock Tree (if applicable)
5. Routing
6. SPEF Extraction
7. Post-Route Signoff Reports
---
## Why This Task is Important?

- Physical Design is the backend flow that converts RTL → GDSII.
- Real SoC design requires analyzing area, timing, power, and parasitics.
- VSDBabySoC is an ideal teaching platform to understand hierarchical SoC flows.
- SPEF extraction is essential for post-route STA, enabling accurate timing signoff.
---
## Repository Structure
```bash
├── README.md                     # Main documentation – intro, objectives, TOC
│
├── 1_Synthesis.md                # RTL to gate-level synthesis details
├── 2_Floorplan.md                # Floorplanning steps, commands, screenshots
├── 3_Placement.md                # Global + detailed placement reports
├── 4_Routing.md                  # Routing flow, routed layout, DRC notes
├── 5_PostRoute_SPEF.md           # Parasitic extraction + SPEF explanation
```
---
## Setup of VSDBabySoC in OpenROAD Flow Scripts Directory

- Before starting synthesis, floorplanning, placement, and routing, you must properly add the BabySoC design directories into the official OpenROAD-flow-scripts environment.

**Below are the mandatory setup steps.**

```bash
OpenROAD-flow-scripts/
└── flow/
    └── designs/
        └── sky130hd/
            └── vsdbabysoc/
                │
                ├── config.mk                   # Main OpenROAD flow config
                ├── vsdbabysoc_synthesis.sdc    # Synthesis constraints file
                ├── macro.cfg                   # Macro placement configuration
                ├── pin_order.cfg               # Pin placement order file
                │
                ├── src/                        # RTL source files for VSDBabySoC
                │   ├── vsdbabysoc.v
                │   ├── rvmyth.v
                │   ├── rvmyth_gen.v
                │   ├── clk_gate.v
                │   ├── avsdac.v
                │   └── avsdpll.v
                │
                ├── include/                    # SandPiper-generated header files
                │   ├── sandpiper.vh
                │   ├── sandpiper_gen.vh
                │   ├── sp_default.vh
                │   └── sp_verilog.vh
                │
                ├── gds/                        # Macro GDS files
                │   ├── avsddac.gds
                │   └── avsdpll.gds
                │
                ├── lef/                        # Macro LEF files
                │   ├── avsddac.lef
                │   └── avsdpll.lef
                │
                └── lib/                        # Macro Liberty timing files
                    ├── avsddac.lib
                    └── avsdpll.lib
```
---
## Introduction to config.mk in OpenROAD Flow

- Before starting the physical design (back-end flow) in OpenROAD, the tool must know what design we are working on, where all the design files are kept, and what external IPs or macros the SoC uses.
This information is not detected automatically — we have to explicitly specify it.
```
                   This is done using a file called config.mk
```
- The config.mk file acts as the central configuration file for a custom design inside OpenROAD-flow-scripts. It provides all the paths and parameters required for:

a. RTL synthesis
b. Macro integration (DAC, PLL, etc.)
c. Constraint loading
d. Placement and routing setup
e. Output directory creation

**In simple words:**

- config.mk is the file that tells OpenROAD “this is my design, these are my RTL files, these are my macros, and this is how you should run the flow.”`

- Without this file, OpenROAD will not know:
    Which Verilog files to synthesize
```
1. Which IP blocks (macros) to include
2. Where LEF/GDS/LIB files are stored
3. What timing constraints to apply
4. What top module to pick
```
Thus, `config.mk` is essential to correctly registering your design inside the OpenROAD-flow-scripts directory structure and ensuring that the entire PnR flow runs with the right inputs.

[View Config.mk File](#Config.mk)

---

# Acknowledgement
- Thank you `Kunal Ghosh` sir for this oppurtunity. Im always grateful for this oppurtunity.
---