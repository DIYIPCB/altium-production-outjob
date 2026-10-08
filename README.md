# DIYIPCB Altium Production OutJob

An Altium Designer Output Job example for generating Gerber,
NC Drill, BOM and pick-and-place files together.

Once the settings have been checked for your project, click
**Generate content** to regenerate the configured outputs.

## Download

Download `DIYIPCB.OutJob` from this repository.

## How to use

1. Copy `DIYIPCB.OutJob` into your PCB project folder.
2. In Altium Designer, right-click the project and select
   **Add Existing to Project**.
3. Add the OutJob and open it.
4. Review the checklist below.
5. Select **Folder Structure → Generate content**.

The configured output folder is `.\DIYIPCB_Outputs\`,
relative to your project directory.

## Check before generating

- Confirm that every Data Source points to the intended project
  or PCB document.
- Review copper-layer selections for your board's layer stack.
- Confirm the board profile and any routing or milling layers.
- Keep Gerber and NC Drill coordinate origins consistent.
- Check BOM fields, manufacturer part numbers and grouping.
- Select the intended assembly variant and verify DNP exclusions.
- Confirm placement units, component sides and rotations.

This example was configured using Altium Designer 26.10.1
with the FEMTO four-layer PCB project. Settings retain
FEMTO-specific document-path and layer records.
Compatibility with other projects and versions has not been tested.

## Generated files

- Gerber artwork and board profile
- NC Drill data
- BOM CSV
- Pick-and-place CSV

Combine the Gerber and actual drill data into a fabrication ZIP.
Keep the BOM and placement CSV files available separately for assembly.

Always inspect the generated files before manufacturing.

## Tutorial

[Illustrated export guide on DIYIPCB](https://www.diyipcb.com/altium-export-gerber-bom-pick-place-files-diyipcb/)

## License

This repository's original OutJob configuration and documentation
are released under the MIT License. You may use, copy, modify and
redistribute them, including for commercial projects.

The FEMTO example design is a separate project with its own license:
https://github.com/mfolejewski/FEMTO
