# COLORado Solo Bar 1

## Software Versions

[V1.1.4 - COLORado Solo Bar 1](https://github.com/Chauvet-Pro/COLORADOSOLOBAR1/blob/d962f777ed3b78d23ae46f9fd24de39c41d2f56c/Firmware/V1.1.4.zip)
- Enhanced dimming performance
- Resolved color shift artifact with Red Shift enabled
- Refined Red Shift effect for improved quality and reliability
- Addressed a connection failure anomaly with Art-Net Universe when set to 0 during power-on

[V1.1.3.5 - COLORado Solo Bar 1](https://github.com/Chauvet-Pro/COLORADOSOLOBAR1/blob/main/Firmware/V1.1.3.5.zip)
- Enhances low-end dimming

[V1.1.3 - COLORado Solo Bar 1](https://github.com/Chauvet-Pro/COLORADOSOLOBAR1/blob/940d52a0be98f7b5826f9c548e5511dc94ef1e33/Firmware/V1.1.3.zip)
- Improved calibration algorithms for XY per cell modes
- Fixed typo in personality names
- ***IMPORTANT: For fixtures with v1.0.XXX or earlier – These fixtures can be updated, but precise color matching to the XY coordinate in the new modes (x Cell XY) is not guaranteed to be accurate until fixtures are recalibrated by Chauvet.***

[V1.1.2 - COLORado Solo Bar 1](https://github.com/Chauvet-Pro/COLORADOSOLOBAR1/blob/da6bea9bed0713e89ba67e399e3adf554c26f455/Firmware/V1.1.2.zip)
- Added calibrated XY control modes with individual cell and section control
- ***IMPORTANT: For fixtures with v1.0.XXX or earlier – These fixtures can be updated, but precise color matching to the XY coordinate in the new modes (x Cell XY) is not guaranteed to be accurate until fixtures are recalibrated by Chauvet.***

[V1.0.0 - COLORado Solo Bar 1](https://github.com/Chauvet-Pro/COLORADOSOLOBAR1/blob/bb4d3297ed35cf551d0f104d83d146e2fe21bf0a/Firmware/V1.0.0.zip)
- Released software version

&nbsp;

## USB Software Update Instructions
1. Power on the product and plug the flash drive into the USB port.
2. Once the flash drive has been detected, the message "**Upgrade Firmware**" will be displayed. Press **< ENTER >**.
   >* If a different message appears on the display, search for the updated software in the main menu (**Update Firmware**) and select from ***Only This Fixture***, ***Multiple Fixture***, or ***Other Fixture Type***, and ***Fixture to Fixture***. A list of the updated software files will be displayed.
   
   >* See the separate instructions below for doing a **Fixture to Fixture** software update process.
3. Select the file that needs to be uploaded. The message **"Are you sure?"** will be displayed. Press **< ENTER >**.
   >**If the selected file is incorrect, the upgrade will fail, and the display will go back to the main interface.**
   >**Repeat steps 1-3 using the correct file**.
4. If the selected file is correct, the upgrade will start. DO NOT turn off the power or disconnect the USB during the process. USB update can take several minutes to complete.
5. When the update is complete, the fixture will automatically reboot.
6. Go to Fixture Information on the product’s menu map and confirm the firmware revision.
7. When the boot-up process is finished, restart the product.

### Special Notes
* Place the .chl file in the root directory of the USB drive.
* The product's USB port supports up to 32GB capacity and only works with FAT32 file format.
* Turning off the power or removing the USB while still blinking during the update will cause partial or total firmware failure in the targeted fixture(s). A force upload will be needed to fix firmware failure issues.


&nbsp;  

## Fixture to Fixture Software Update

To update the firmware using a DMX cable connection, follow the instructions below:
1. Power on the products.
2. Connect the DMX out of the STRIKE Array 1 Driver with the latest firmware to the DMX in of the STRIKE Array 1 Driver that needs to be updated.
3. Go to the **Update Firmware** main level of the receiving product.
4. Select the **Fixture to Fixture** option.
5. A warning ***"make sure no other signal, Network, or DMX controller is being sent! and press enter key to start update"*** will show on the display. Press **< ENTER >** to start the update.
   >* DO NOT turn off the power or disconnect the DMX cable during the process. The update can take several minutes to complete.
   >* If the connected product is incorrect or has the incorrect sofware, the upgrade will fail, and the display will go back to the main interface. Repeat **steps 1-5** using a STRIKE Array 1 Driver with valid software.
6. If the connected product is valid, the update will start. DO NOT turn off power or disconnect the DMX cable during the process. The update can take several minutes to complete.
7. When the update is complete, the product will automatically reboot.
8. Go to the **Information** level of the product's main menu and confirm the software update.

### Special Notes
* When updating software using the **Fixture to Fixture** option, make sure no other DMX or Ethernet signals are connected to the products.
* Turning off the power, removing the DMX cable, or not setting the fixture to the correct protocol during the update can cause partial or total firmware failure in the targeted fixture. The user will need an **Upload 03** device to fix the software failure issues. Please contact Chauvet customer service for this device.

&nbsp;

## Force Upload

1.	Link the target fixture to the main fixture via a DMX 5-pin connection. Ensure that the target fixture is turned off.
2.	Turn on the main fixture and set its protocol to DMX512.
3.	Plug the flash drive into the USB-C port of the main fixture.
4.	Go to Upgrade Firmware on the menu map.
5.	Choose between **Multiple Fixture** and **Other Fixture Type**. Press **< ENTER >**.
      * **Multiple Fixture** : Both the target fixture and main fixture are from the same product line (e.g., 2 Color STRIKE M fixtures).
      * **Other Fixture Type**: The target fixture and main fixture are from different product series (e.g., a Color STRIKE M as the target fixture and a Maverick Silens 2 Profile as the main fixture).
6.	Select the file that needs to be uploaded. The message ***“Are you sure?”*** will appear on the screen. Press **< ENTER >**. Turn on the target fixture within 1–2 seconds of pressing **< ENTER >**. The display on the target fixture should remain off.
      a. The main fixture will show the update progress (0–100%).
      b. The target fixture’s display will turn on, and a notification ***“< UPDATE >”*** will appear on the screen.
7.	DO NOT turn off power or remove the USB flash drive. Once the software is done uploading, the target fixture will automatically reboot.
8.	Go to the target fixture’s main menu and confirm that the firmware version has been updated.
9.	Reboot the target fixture.

### Special Notes
* A Force Upload process requires a target fixture (the fixture that needs a Force Upload and a main fixture (the fixture that controls the upload process).
* The Force Upload process can only be done one target fixture at a time.
