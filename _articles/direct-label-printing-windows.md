---
title: Windows setup
layout: article
parent: direct-label-printing
description: Learn how to set up direct label printing for Windows, so you can print PartBolt inventory labels straight from your browser. Compatible label printer required.
---

On Windows, there's a few extra steps you need to do so that we can access your label printer. You'll only need to do this once.

First, [download Zadig](https://zadig.akeo.ie/), a free tool that will let you reconfigure your label printer. Then, follow these steps:

1. Make sure your label printer is powered on and plugged into your computer.
2. Open Zadig.
3. From the <strong>Options</strong> menu, select <strong>List All Devices</strong>.
    <div class="step-image" style="max-width: 575px"><img src="/img/direct-label-printing/windows/zadig_options.png" alt="Image of the List All Devices menu item." /></div>
4. In the devices dropdown, select the name of your label printer. In our case, this is QL-800.
    <div class="step-image" style="max-width: 575px"><img src="/img/direct-label-printing/windows/zadig_select_printer.png" alt="Image of the device menu, with QL-800 selected." /></div>
5. To the right of the green arrow, make sure that <strong>WinUSB</strong> is selected. If it isn't, use the up and down arrows to select WinUSB.
    <div class="step-image" style="max-width: 575px"><img src="/img/direct-label-printing/windows/zadig_winusb.png" alt="Image of the driver list, with WinUSB selected." /></div>
6. Click the <strong>Replace Driver</strong> button. It might take a few minutes to install.
    <div class="step-image" style="max-width: 575px"><img src="/img/direct-label-printing/windows/zadig_replace_driver.png" alt="Image of the Replace Driver button." /></div>
7. Once it's done, you should see a message confirming that the installation was successful.
    <div class="step-image" style="max-width: 575px"><img src="/img/direct-label-printing/windows/zadig_success.png" alt="Image of the success dialog." /></div>
8. After this process, your label printer will be compatible with PartBolt, and you can follow the [regular procedure to add a printer](/articles/direct-label-printing#adding-a-printer). However, your label printer might not work with other software &mdash; to restore that functionality, follow the steps below.

## Undoing these instructions
After following the above procedure, your label printer might not work with any software from its original manufacturer. If you want to restore operation with that software, follow these steps:

1. Make sure your label printer is powered on and plugged into your computer.
2. Right-click on the Start menu, and select <strong>Device Manager</strong> from the menu that appears.
    <div class="step-image" style="max-width: 575px"><img src="/img/direct-label-printing/windows/uninstall_start.png" alt="Image of the Start menu options, with Device Manager circled." /></div>
3. In Device Manager, scroll to the bottom and expand the <strong>Universal Serial Bus devices</strong> category.
    <div class="step-image" style="max-width: 781px"><img src="/img/direct-label-printing/windows/uninstall_category.png" alt="Image of Device Manager, with the Universal Serial Bus devices category circled." /></div>
4. In <strong>Universal Serial Bus devices</strong>, you should see your printer. Right-click on it and select <strong>Uninstall device</strong>.
    <div class="step-image" style="max-width: 781px"><img src="/img/direct-label-printing/windows/uninstall_menu.png" alt="Image of Device Manager, with a right-click menu open and the Uninstall device option circled." /></div>
5. In the dialog that appears, make sure <strong>Delete the driver software for this device</strong> is checked. Then, click <strong>Uninstall</strong>.
    <div class="step-image" style="max-width: 781px"><img src="/img/direct-label-printing/windows/uninstall_confirm.png" alt="Image of the uninstall dialog, with Delete the driver software for this device checked." /></div>
6. Once it's uninstalled, disconnect and reconnect your label printer.
7. After you reconnect your label printer, Windows should recognize it and you'll be able to use it with other software. If you need to use it with PartBolt again, just follow the steps at the top of this article.