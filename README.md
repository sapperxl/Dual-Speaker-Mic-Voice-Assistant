I tried out a few of the voice assistant designs on Makerworld and tried the ESP32-S3-Box3 and I found all of them to be lacking either in the mic or speaker output so I came up with this design. This utilizes 2 10W 2” full range speakers and 2 INMP441 microphones. The ESP32-S3 I use also includes an external antenna which I find greatly increases wifi signal. 

BOM:
1ea 3a+ 12V Power Supply, combined speaker output is up to 20W so you will need at least a 3a power supply 5a is better.  
1ea 12V input jack that matches the power supply barrel & pin dimensions  
1ea PCM5102 I2S IIS Lossless Digital Audio DAC  
1ea PAM8610 2x15W Digital Dual Channel Stereo Audio Amplifier Board  
2ea 10K 1/4watt metal film resistors  
1ea ESP32-S3 Development Board 16MB Flash/8MB PSRAM /w IPEX External Antenna  
1ea 12V to 5V Regulator Buck Converter  
2ea INMP441 Mics  

Keep in mind the 3.5mm output from the PCM5102 is for a line level load, it will not drive headphones but works great with an external self-powered speaker.

On the PCM5102s I got from Amazon none of the solder pads were soldered so I wasn’t getting any output initially, it should look like this:
Thanks to A. Pauna on Amazon for their review of the PCM5102 that included a schematic and Carey Brown on Amazon that pointed out the PCM5102 solder pad issue on a review. Also 3DMN on Makerworld for their voice assistant design that inspired some of this one.

PCM5102 Module
<img width="1386" height="958" alt="image" src="https://github.com/user-attachments/assets/8fcd9d0d-2ba7-4073-a1c8-c2b304238e4d" />

PAM8610 Module
<img width="1111" height="867" alt="image" src="https://github.com/user-attachments/assets/a27363eb-0761-4803-975d-52077debdbe6" />

Buck Converter
<img width="1484" height="925" alt="image" src="https://github.com/user-attachments/assets/66fb9182-bd41-4c0c-8d48-fc0801f80b35" />

ESP32
<img width="1500" height="1172" alt="image" src="https://github.com/user-attachments/assets/60b6fa43-9994-4733-a2bf-421afeb2f556" />
<img width="585" height="1500" alt="image" src="https://github.com/user-attachments/assets/737f72c1-f1bb-4072-bf0a-ad8c40a624e2" />
