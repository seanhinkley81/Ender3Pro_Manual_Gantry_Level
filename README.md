# Ender3Pro_Manual_Gantry_Level
Manual Mechanical Gantry level For Ender 3 Pro running klipper

My sagging x gantry has always been causing me problems and I've been getting tired of leveling it. So I got a dual z stepper kit! I have a Cr-Touch but didn't want to get a new 5 driver main board to take advantage of Klipper-s Z stepper auto-alignment or Marlins (G34). So I was looking for solutions with just my stock Creality 4.2.2 board. I saw projects for other setups utilizing newer drivers such as the UART tmc2209 

I remembered Prusa printers just use a forced mechanical alignment (now depreciated M915 command in Marlin) so wrote up my own gcode script, printed some mechanical endstops and now have a near perfect level x gantry every time. I found it easiest to have the wheels run into the hard stop rather than the gantry itself just due to space constraints and to prevent the bowden tube from being pulled out or pinched by the frame (ask me how i know). But once I had everythign working I could actually see the gantry level itself! (Video coming soon).


Use at your own risk, there always a chance that you can over heat or stress your motors if used excessivly or if you push too long / hard fast ect. I tried to balance speed with "saftey" so that running a Gantry Level (G34) and Bed Mesh (G29) would take less than 3 minutes total - not a bad timeframe to relevel a Ender 3 series. The gantry level should not have to be run very often, only really if the print get stuck or banged and the gantry alignment is knocked off. But having the printer auto-level the gantry instead of breakign out the blocks, leveling, homing ect - is definatly convient.   
