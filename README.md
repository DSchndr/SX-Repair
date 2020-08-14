# SX-Repair
Nintendo Switch repair instructions

- [SX-Repair](#sx-repair)
- [My Switch doesn't charge / turn on](#my-switch-doesnt-charge--turn-on)
- [My Switch hangs on Nintendo logo and blackscreens / fake charges](#my-switch-hangs-on-nintendo-logo-and-blackscreens--fake-charges)
- [My Switch bluescreens](#my-switch-bluescreens)
- [My Switch hangs on SX logo / doesn't boot](#my-switch-hangs-on-sx-logo--doesnt-boot)
- [I removed a cap on the cpu while soldering on sx c0re / sx l1te](#i-removed-a-cap-on-the-cpu-while-soldering-on-sx-c0re--sx-l1te)
- [No Video in docked mode / Switch logo takes long time to appear and stays](#no-video-in-docked-mode--switch-logo-takes-long-time-to-appear-and-stays)
- ["2101-0001"](#2101-0001)
- [My Joycons don't charge](#my-joycons-dont-charge)



# My Switch doesn't charge / turn on
1. Check usbc port 
2. Open up your Switch
3. Check Capacitors around M92T36, BQ24103, PIUSB3 for Shorts and replace IC / Cap if there is one
4. Short on 3v3 line after chips from #3 are removed? unplug emmc and check again, in both cases the console is worthless because soc / emmc is broken
5. Check if there is a Voltage on the Cap near the joycon zif socket near BQ ic


# My Switch hangs on Nintendo logo and blackscreens / fake charges
Usually you can start the Console by pressing *volume + & volume - & power* after plugging in the battary
1. Check that pin 3 of the battary connector has continuity
2. Check that M92T36 gives BQ24103 a voltage. No voltage? -> Replace it
3. Check that BQ24103 charges the battary while plugged in and on. No charge? -> Replace it

# My Switch bluescreens
Reflow / Reball tegra ic, emmc and ram

Still bluescreens? GPT partitions on emmc are damaged or other issue

# My Switch hangs on SX logo / doesn't boot 
Check if the 2 caps near the shield from the tegra chip exist...
Gone? Replace with [TODO: Image / Info]

# I removed a cap on the cpu while soldering on sx c0re / sx l1te
Should be [81-GRM033R61A105ME5J](https://www.mouser.de/ProductDetail/Murata-Electronics/GRM033R61A105ME15J)

# No Video in docked mode / Switch logo takes long time to appear and stays
Replace PI3USB

# "2101-0001"
Your M92T36 is either not soldered in properly or is broken; try reflow and then replace 

# My Joycons don't charge
Maybe broken M92T36? or dcdc supply
Replace diode with "PU"? marking
