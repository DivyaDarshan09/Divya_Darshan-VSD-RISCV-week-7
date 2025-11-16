# SPEF stage - VSDBabySoC
---
## Objective 
The objective of this step is to extract accurate post-route parasitic information and generate the Standard Parasitic Exchange Format (SPEF) file for the design. After routing, the interconnect wires contribute significant delay due to their resistance (R) and capacitance (C). The goal is to capture these real parasitics using OpenROAD’s extraction engine so that the final Static Timing Analysis (post-route STA) reflects the actual behavior of the silicon. Generating the SPEF file ensures that timing closure is based on physical, layout-driven data rather than pre-route estimations. This enhances timing accuracy, identifies true critical paths, and validates whether the design can reliably meet the target performance after fabrication.

---
### Defnition

- The Standard Parasitic Exchange Format (SPEF) is an industry-standard file used to describe the electrical parasitics of a routed design.
It captures:
 - The resistance of metal segments
 - The capacitance of interconnects
 - The coupling capacitors between adjacent nets
 - Pin and via parasitics
- In other words, SPEF represents the real physical behavior of wires after layout.

---

### Why is the SPEF Required?

- Before routing takes place, timing analysis relies on estimated wire delays—typically from simplified models. These models assume average wire lengths, average fanout, and uniform loading. They are only approximations.

- Once routing is completed, the actual wire topology is known. This means the exact wiring path, detours, jogs, layer usage, and proximity to other nets can be measured.

**SPEF gives us:**

- Accurate wire resistance
- Accurate total and coupling capacitances
- True delay impact of routing congestion
- Realistic propagation delays on each net
- This transforms our timing analysis from rough estimates to actual silicon behavior.

```
Final timing sign-off is always SPEF-based.
Without SPEF, no professional flow can guarantee timing closure.
```

---