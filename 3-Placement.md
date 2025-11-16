# Placement Stage — VSDBabySoC
---
## Objective

- Global + detailed placement of cells
- Reduce congestion
- Optimize wirelength
---

## Commands Used

```bash
make DESIGN_CONFIG=./designs/sky130hd/VSDBabySoC/config.mk place
```
- This will do both detailed and global placement by default.
---
## Terminal Screenshot

![placement](.Screenshots/placement_1.jpg)


![placement](.Screenshots/placement_2.jpg)

---
## Placement View

![Placement](.Screenshots/placement_view.jpg)

**Observation**

- The placement view clearly shows all standard cells arranged in legal rows with no overlaps, indicating successful global and detailed placement.
- Macros remain fixed at their predefined locations, while standard cells are optimally clustered around them, ensuring balanced density and reduced routing congestion.

---

## Placement Timing and Power Summary

- **TNS = 0.00** → No setup timing violations after placement.
- **WNS = 0.00** → All critical paths close timing successfully.
- **Worst Slack = +0.33 ns** → Placement improved timing margin.
- **Clock Min Period = 10.08 ns** → Maximum achievable frequency ≈ 99 MHz.
- **Hold Slack = MET** → No hold-time violations observed.
- **Setup Slack = MET** → All setup constraints remain satisfied post-placement.
- **Power Breakdown**
    - Sequential Cells: 73.5%
    - Combinational Cells: 26.5%
    - Total Power ≈ **6.45 mW**

---

**The placement results confirm timing closure with improved slack and stable power characteristics. Cell legalization and optimization are successful, and the design is ready to proceed to routing.**