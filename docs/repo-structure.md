# Repository Structure

This repository is curated for version 2 planning. It keeps only the v1 material that is useful as design context.

## Tracked

```text
README.md
docs/
LIA_SPICE_SIM/
LIA_IMG/LIA_System_Mod.png
LIA_IMG/LIA_Flowchart.png
LIA_IMG/LIA_PCB.jpg
LIA_IMG/LIA_block.png
Sim_LIA_V1.asc
Simulation_LIA.asc
```

The tracked files are intended to provide a compact overview of the v1 architecture and retain the circuit schematic sources most likely to inform v2.

## Kept Local

```text
02319080_06059608_AnalogueDesign_LIA.pdf
02319080_06059608_DigitalDesign_LIA.pdf
LIA_DSPCode/
LIA_NUCLEO_CODE/
Auren,Wenjun,LockINamp_PCB/
LIA_IMG/*.raw
*.log
*.zip
```

These files are ignored because they are full reports, early prototype code, manufacturing outputs, generated data, logs, or local archives. They can still be used locally, but they should not shape the public or private Git history unless the release strategy changes.

## Adding Version 2 Work

When version 2 starts, add new work in clearly named folders rather than mixing it into the v1 archive. Suggested top-level folders:

```text
v2_hardware/
v2_firmware/
v2_analysis/
v2_docs/
```

Those names can be adjusted once the v2 design approach is fixed.
