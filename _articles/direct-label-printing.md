---
title: Direct label printing
layout: article
children: ["direct-label-printing-windows"]
description: Learn about direct label printing, which lets you print PartBolt inventory labels straight from your browser. Compatible label printer required.
---

{% include paid_required.html %}

If you've got a compatible label printer, you can print tracking labels directly from PartBolt. To learn more about tracking labels and how they work, see our article on [item codes](/articles/item-codes).

Currently, the supported label printers are:
* Brother QL-800

The supported label sizes are:
* DK-2210 (1.1" width)

We're always looking to expand this list! If you have a label printer that isn't listed above, contact us at [support@partbolt.com](mailto:support@partbolt.com), and we'll look into adding support for it.

## Adding a printer
First, make sure you're using Google Chrome, as direct label printing requires it. Also, if you're using Windows, you must [follow these one-time setup instructions](/articles/direct-label-printing-windows) first.

1. Click on the tracking code for any item in your inventory, and, in the window that appears with your label, click **<i class="fas fa-fw fa-print"></i> Print**.
2. Click **<i class="fas fa-fw fa-plus"></i> Add printer**
3. Make sure your label printer is plugged into power, turned on, and connected to your computer.
4. Make sure the "Editor Lite" mode is **OFF**&mdash;that means the light above that button should be off. If it's on, you can turn it off by pressing and holding the "Editor Lite" button for a few seconds.
    <div style="max-width: 500px"><img src="/img/direct-label-printing/editor_lite_off.jpg" alt="The Editor Lite button" /></div>
5. Click **<i class="fas fa-fw fa-plug"></i> Got it, connect printer**.
6. Select your label printer from the list that appears.
7. You're done!

## Printing labels
When you click on an item's tracking code, you'll open up its label. Once you've opened its label, you can print it by clicking **<i class="fas fa-fw fa-print"></i> Print**.

## Troubleshooting
If your label printer doesn't appear in the list of printers, or you're having some other difficulties, there are some things you can check first.
* Make sure the printer's power light is on, and make sure it's plugged into your computer.
* Make sure the "Editor Lite" mode is **OFF**&mdash;that means the light above that button should be off. If it's on, you can turn it off by pressing and holding the "Editor Lite" button for a few seconds.
    <div style="max-width: 500px"><img src="/img/direct-label-printing/editor_lite_off.jpg" alt="The Editor Lite button" /></div>
* Try a different USB port.
* If you're using Windows, make sure you've completed the [Windows-specific setup instructions](/articles/direct-label-printing-windows).
* If you're using Linux, you might need to disable the existing `usblp` printer driver. You can do this by running `sudo modprobe -r usblp`. The driver will be disabled until you reboot, or you run `sudo modprobe usblp` to reload it.

If you're still having trouble with your label printer, please contact us at [support@partbolt.com](mailto:support@partbolt.com), and we'll be happy to help!