# recalbox-rpi_zero_v1.3-gpi_case_2w
This repo contains the custom configuration used to successfully boot the retro gaming OS Recalbox v9.2.3-Pulstar from a Raspberry PI Zero v1.3 (2015) bundled with a [Retroflag GPi CASE 2W](https://retroflag.com/gpi_case_2w.html).

![image](https://github.com/user-attachments/assets/8154768a-3842-4089-8b67-35668af06534)
![image](https://github.com/user-attachments/assets/5edd690a-c433-4803-8934-1811e2d32937)

### Boot issues and troubleshooting
Ensure to flash the right Recalbox v9.2.3-Pulstar image into your SD card. Please note that the image named `GPiCase 2W + Raspberry Pi Zero`, being available into the [recalbox website RPI download section](https://www.recalbox.com/download/stable/rpi/) at this [link](https://www.recalbox.com/it/download/stable/rpi/rpizerogpicase2/alternative/) (see also the image below), could be misleading. Once flashed into a SD card, it won't boot on your Rasperry PI Zero v1.3, ending up in a endless black screen.

![image](https://github.com/user-attachments/assets/91ba6a8d-44bb-4685-afac-cc3314a66d39)

The right procedure to make a bootable Recalbox v9.2.3-Pulstar image for your RPI Zero v1.3 is flashing it through the Raspberry PI Imager tool, being downloadable from [here](https://www.raspberrypi.com/software/). Once you've installed the Imager tool on your computer, go through the following steps:

1. Click on CHOOSE OS and select Recalbox from the Emulation and game OS category.
2. Select Recalbox - Raspberry Pi Zero / 1 / GPiCase1 (see image below).
3. Flash the image.

![image](https://github.com/user-attachments/assets/32897574-79ba-43a4-b4ba-014eadeaa59c)

You should have ended up now with a bootable Recalbox image, be ready to try it out on your GPi CASE 2W.

### Screen issues (sideways-rendered image)
Some users, with an overall different setup, have reported encountering a sideways-rendered image immediately after Recalbox boots. This issue was highlighted in this [Reddit discussion](https://www.reddit.com/r/retroflag_gpi/comments/zr1nf7/anyone_else_this_screen_issue_with_their_gpi_case/)), refer to the image below for an example.

![image](https://github.com/user-attachments/assets/133d7552-fa68-4037-9c86-4392af2c715c)

In order to fix this issue, you must overwrite the default `recalbox-user-config.txt` config file, sitting on the root folder of your SD card, with the one made available [here](https://github.com/mirkochip/recalbox-rpi_zero_v1.3-gpi_case_2w/blob/main/recalbox-user-config.txt).

Now you should be all set, being ready to enjoy your favorite retro game titles ran by a Raspberry PI Zero v1.3 on a GPi Case 2W!
