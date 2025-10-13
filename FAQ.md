<details>
<summary>How to restart the device?</summary>
Press the button on the back of the device (next to the USB port).
</details>

<details>
<summary>How to enter Device Firmware Upgrade (DFU) mode?</summary>
Double-click the reset button quickly. Connect to the PC with the USB cable. 
The device should appear as a mass storage device.
You can copy a new UF2 firmware file directly to the root folder of the device.
Wait for it to eject itself. That's it!
</details>

<details>
<summary>Will firmware update change my keymap?</summary>
No, if you've made at least one change to your keymap via ZMK Studio, new firmware will not overwrite your settings.
</details>

<details>
<summary>How to reset all the settings to defaults?</summary>
Please see the <a href="https://zmk.dev/docs/config/settings#clearing-persisted-setting">corresponding section</a> of ZMK docs. Here is <a href="https://nightly.link/efogtech/endgame-trackball-config/workflows/build/reset-fw/firmware.zip">firmware-eraser, binary</a>. TLDR: flash it onto the device, wait 5 seconds, flash the regular firmware.
</details>

<details>
<summary>What is the default keymap?</summary>
You will find the keymap description at the <a href="https://github.com/efogtech/endgame-trackball/tree/main?tab=readme-ov-file#default-keymap">root README</a>.
</details>

<details>
<summary>Can I disable twist scroll?</summary>
Yes, but it's not possible with ZMK Studio at the moment, you need to add this to your keymap: 
  
```diff
--- config/efogtech_trackball_0.keymap
+++ config/efogtech_trackball_0.keymap
@@ -1,5 +1,10 @@
     trackball {
+        default {
+            layers = <DEFAULT>;
+            input-processors = <&zip_scroll_scaler 0 1>;
+        };

         scroll {
             layers = <LAYER_SCROLL>;
             input-processors = <&zip_xy_scaler SCROLL_MULTIPLIER SCROLL_DIVISOR>, <&zip_axis_clamper>,
```
</details>

<details>
<summary>Twist scroll is getting triggered unintentionally, anything I can do?</summary>
  
Yes — open the keymap, scroll to the very end, then either decrease `twist-interference-thres` or increase `twist-thres` (or both). 
</details>

