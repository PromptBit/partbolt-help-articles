---
title: Importing a Bill of Materials from CSV
layout: article
description: Learn how easy it is to import a Bill of Materials (BOM) from external software into a PartBolt project.
---

With PartBolt, it's easy to import a Bill of Materials (BOM) into a project.

First, you'll need to export the BOM from the Electronic Design Automation (EDA) software that you used to design your product. Ensure that the export is in CSV format, and includes at least the following columns:

* Reference designator
* Part number/value
* Footprint (optional)
* Description (optional)

The footprint column is only required if you need to distinguish between parts with the same value&mdash;for example, if your design contains 100 nF capacitors in both 0402 and 0603 packages.

Once you've exported your BOM, go to PartBolt and open the project you'd like to import the BOM into. You can create a new project from the **<i class="fas fa-fw fa-atom"></i> Projects** tab. Then, follow these steps:

1. Click the **<i class="fas fa-fw fa-file-import"></i> Import CSV** button.
2. Click the **Choose a file&hellip;** button, and select the CSV file.
3. PartBolt will show the first few rows of your CSV file. Using the dropdowns, label the different columns. (reference designator, part number/value, footprint, description) If you have extra columns, you can mark them as *Ignored*.
4. Once you've labeled all the columns, click **Next <i class="fas fa-fw fa-chevron-right"></i>**.
5. PartBolt will group the parts of your BOM by their number/value. Using the dropdowns on the right, match the groups with the corresponding parts in your inventory.
6. Once you've matched all the parts, click **<i class="fas fa-fw fa-check"></i> Done**.

If you encounter issues with this process, or need to import data from software that cannot export a CSV file, please contact us at [support@partbolt.com](mailto:support@partbolt.com) and we'll be happy to help!