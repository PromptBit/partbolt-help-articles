---
title: Importing data
layout: article
description: Learn how to import existing data into your PartBolt database.
---

If you're coming to PartBolt from different inventory software (or a spreadsheet), we're happy to help import your existing data&mdash;just send an email to [support@partbolt.com](mailto:support@partbolt.com). We'll need two things to process the import:
* **Your existing data** in some sort of machine-readable format, like an Excel spreadsheet, CSV file, or JSON file.
* **The PartBolt database name**, which you can check by clicking the <i class="fas fa-fw fa-database"></i> icon in the top right, and then the **<i class="fas fa-fw fa-cog"></i> Manage databases** option.

We recommend importing data into an empty PartBolt database, since otherwise you might run into issues merging the imported data with what's already in PartBolt. We're happy to create a new database if that's what you want&mdash;just let us know.

If you have any questions about importing data, please don't hesitate to email us at [support@partbolt.com](mailto:support@partbolt.com). We'll be happy to help!

## Using our standard template
A normal data import can take a few days for us to process. If you'd like to expedite your import, you can provide your data using our standard template, which reduces the amount of processing we have to do.

<a href="/img/importing-data/PartBolt Standard Template.xlsx"><i class="fas fa-fw fa-download"></i> Download template as XLSX file</a>

Each line of the template corresponds to a **lot**, and each lot describes the quantity of a part in a location. This is best understood with some sample data:

| Part number | Name                  | Package  | Manufacturer | Location | Quantity | Lot description            |
| ----------- | --------------------- | -------- | ------------ | -------- | -------- | -------------------------- |
| SAMPLE1     | Sample part           | DIP-28   | Test Corp    | Shelf A  | 5        | Order #1234                |
| SAMPLE1     | Sample part           | DIP-28   | Test Corp    | Shelf B  | 15       |                            |
| SAMPLE1     | Sample part           | DIP-28   | Test Corp    | Shelf C  | 100      |                            |
| SAMPLE2     | Different sample part | TSSOP-20 | GeneriCorp   | Shelf B  | 12       |                            |
| SAMPLE3     | Again a sample part   | QFN-56   | GeneriCorp   | Shelf C  | 63       | Quantity may be inaccurate |

Notice that the three entries for "SAMPLE1" will be combined into one PartBolt part with different three lots. The first time that our importer encounters a part number, package, manufacturer, or location that does not already exist, it will automatically be created. For example, as the first row is processed, the package "DIP-28", manufacturer "Test Corp" and location "Shelf A" would be created; however, any future references to that package, manufacturer, or location would then use the existing entry.

Part numbers, packages, manufacturers, and locations are matched by their names, so it's very important to be consistent. For example, if you had one part with a manufacturer of "Test Corp" and another with "Test Corporation", this would be imported as two separate manufacturers.

For each row, all fields are required except for the package and lot description. Conditional formatting has been enabled on our standard template, so if you leave a required field empty, it will be shown in red.