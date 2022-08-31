---
title: Importing a Bill of Materials
layout: article
description: Learn how easy it is to import a Bill of Materials (BOM) from external software into a PartBolt project.
redirect_from: /articles/import-bom-from-csv
---

With PartBolt, it's easy to import a Bill of Materials (BOM) into a project. We can import a BOM from an Altium Designer file, a KiCad file, or a CSV file.

## Supported formats
#### Altium Designer
PartBolt is able to read a PCB file (.PcbDoc) created by Altium Designer. You just need to upload an individual .PcbDoc file&mdash;any schematic (.SchDoc) or project (.PcbPrj) files are not required.

Please note that we currently only support Altium's "PCB Binary Version 6.0" format. (This version was introduced in Altium Designer 6.3, which was released in 2006&mdash;so, you're probably already using it!)

#### KiCad
PartBolt is able to read a PCB file (.kicad_pcb) created by KiCad. As with Altium Designer, we only require the PCB file&mdash;you do not need to upload schematic or project files.

We support both the older KiCad 5.0 format and the newer KiCad 6.0 format. It's likely that KiCad 4.0 PCB files will also work, but this has not been tested extensively. Any older versions of KiCad use a different PCB file format and are not supported.

#### CSV
If you don't use Altium or KiCad, you can also import a BOM from a CSV file. Just make sure it includes at least the following columns:

* Reference designator
* Part number/value
* Footprint (optional)
* Description (optional)

The columns don't need to be in this exact order&mdash;once you upload the file, you'll be able to label which column is which.

Also, the footprint column is only required if you need to distinguish between parts with the same value&mdash;for example, if your design contains 100 nF capacitors in both 0402 and 0603 packages.

## Importing a file
Once you have a file in one of the above formats, go to PartBolt and open the project you'd like to import the BOM into. (You can create a new project from the **<i class="fas fa-fw fa-atom"></i> Projects** tab.) Then, follow these steps:

1. Click the **<i class="fas fa-fw fa-file-import"></i> Import BOM** button.
2. Click the **Choose a file&hellip;** button, and select the file.
3. _[CSV files only]_ PartBolt will show the first few rows of your file. Using the dropdowns, label the different columns. (reference designator, part number/value, footprint, description) If you have extra columns, you can mark them as *Ignored*.
4. _[CSV files only]_ Once you've labeled all the columns, click **Next <i class="fas fa-fw fa-chevron-right"></i>**.
5. PartBolt will group the parts of your BOM by their number/value. Using the dropdowns on the right, match the groups with the corresponding parts in your inventory.
6. Once you've matched all the parts, click **<i class="fas fa-fw fa-check"></i> Done**.

If you encounter issues with this process, or want to request that we add support for a different file format, please contact us at [support@partbolt.com](mailto:support@partbolt.com) and we'll be happy to help!