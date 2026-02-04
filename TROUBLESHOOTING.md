<details>
<summary>The board shows no signs of life when I plug in my USB power</summary>
  
1. Try to use your PC (not a wall adapter)  
2. Try to use a different cable  
3. Unplug the battery and try again  
4. If nothing helps, inspect the board and reach the support with a photo
</details>

<details>
<summary>The device turns on but my host doesn't see it</summary>
  
1. Ensure the correct boot sequence — restart the device and observe the red LED. The normal behavior is two flashes, then off  
2. Try to discover it with Bluetooth  
3. Make sure it doesn't show up as a flash drive — you need to flash the board in that case  
4. If nothing helps, inspect the board and reach the support with a photo  
</details>

<details>
<summary>My buttons work but pointer doesn't</summary>
  
This indicates an issue with one or both sensors. You need to take a look at logs after device restart.  
See the next item to learn how to read logs, and see FAQ.md to learn how to restart the device.
</details>

<details>
<summary>How to open and read logs?</summary>
  
Option 1 (beta): open [Marshmellow UI](https://efog.tech/marshmellow-ui/) and connect to the device  
Option 2: follow the instructions from ZMK docs: https://zmk.dev/docs/development/usb-logging#viewing-logs 
</details>

<details>
<summary>Pointer moves erratically, jumps and doesn't feel smooth</summary>
  
This indicates either ball incompatibility, or incorrect distance from the ball surface to the lenses.  
1. Make sure to try a standard (stock) red trackball with a reflective coating  
2. Check your bearings or BTUs — ensure they are inserted fully  
3. In case you are using BTUs, try the static bearings to see if it changes anything  
4. If nothing helps, install the debug firmware and open logs, it will allow you to see which sensor reports low surface quality
</details>

<details>
<summary>Pointer works in debug firmware but doesn't work with regular one</summary>
  
This indicates that only one of the sensors is functional. Please restart the device and open logs shortly after to learn which one is at fault. 
</details>

<details>
<summary>Pointer works but is significantly off-axis (maybe even producing horizontal events when rolling vertically)</summary>
  
This indicates that one of the sensor boards is installed in an incorrect orientation. Please consult with the pictures in the assembly guide keeping attention to this aspect. 
</details>

<details>
<summary>One of the sensor reports "unexpected product id"</summary>
  
This typically indicates no electrical connection from the board to the sensor. Try re-seating the cable from both ends.
</details>

<details>
<summary>One of the sensor reports "failed self-test"</summary>
  
This typically indicates either bad electrical connection from the board to the sensor, or issues with soldering. 
Try re-seating the cable from both ends, and inspect the solder job.
</details>
