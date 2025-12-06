## Repairing encoders

Please note that this is relevant for the owners of a rev03 motherboard who've ordered a repair kit for their encoders. 
Make sure your hardware revision is correct, although in case you're reading this in 2025, it certainly is.

![photo_2025-12-07_00-13-53](https://github.com/user-attachments/assets/9e6c7d3f-dfc7-4461-8eba-a34608745959)

It is highly recommended to use the original boards when possible. In case you have to use the new one, please keep in mind:
the encoder boards from the repair kits don't have certain ("pull-down") resistors because they've migrated to the motherboard.  

Now, you need to ensure that the boards from your repair kit are newer indeed. Here's how to distinguish those:

![photo_2025-12-07_00-13-57](https://github.com/user-attachments/assets/c3811339-807d-414e-8c8c-b49356a2ddb5)


If it's not the case, you can close this page.  
Now, what this whole story means for you: for each newer encoder board, you will get increased power consumption in idle.
Currently the typical draw is ~680 uA, and it will raise up to ~1050 uA if you install two newer boards.

Last but not least, to make the new board actually work, you'd need to make a small adjustment in the firmware. 
Open or create your config repository (see FAQ.md), and find the file: `boards/arm/efogtech_trackball_0/encoders.dtsi`.   
Here's what the declaration of the left encoder looks like:

<img width="287" height="168" alt="image" src="https://github.com/user-attachments/assets/f67a2167-1f66-4dde-9086-71c08bbc9cdd" />

Now, this code is correct for your original encoders. 
For the newer ones, you need to replace the last parameter (0) for `a-gpios` and `b-gpios` of the board node you're replacing.  

Before:
```dts
a-gpios = <&gpio0 17 0>;
b-gpios = <&gpio0 16 0>;
```
After:
```dts
a-gpios = <&gpio0 17 GPIO_PULL_UP>;
b-gpios = <&gpio0 16 GPIO_PULL_UP>;
```

That's it! Commit your changes and flash the fresh firmware. 

### I'd love to use the original board but there's a broken shaft inside
Yep, that unfortunately happens. My recommendation is to use a needle to pick the shaft up, and if it doesn't work, you can heat the needle slightly. 
