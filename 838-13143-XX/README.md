# IC BD Gun Sense (838-13143-XX)
<div id="top"></div>

<!-- SUMMARY-->
## Summary
<img src="https://raw.githubusercontent.com/theretrobristolian/Arcade/main/838-13143-XX/diagram1.svg">

Description: The above is a basic representation of the layout from the most common types of IC BD Gun Sense boards, the trough hole component type. This covers board A to B.

The Sega Gun Sense Board 838-13143 is an arcade board developed by Sega in the 1990s to provide accurate aiming and shooting mechanics in light gun games. The board was first used in "The Lost World: Jurassic Park" arcade game in 1997, where it was paired with Sega's Type 2 (Type II) light gun.

Over the years, Sega released several revisions of the Gun Sense Board. The initial release was specific to "The Lost World: Jurassoc Park" and was designed for 12 sensors around the screen not 10 (which was the new standard on the later revisions - although these boards are backwards compatible. These boards can be found in games from the late 90s right up through the 2000s as the technology didn't fundementally change.

The technology was based on a design by a Japaneese company OHMIC, the link to this is here http://www.ohmic.co.jp/cat/zahyou-01.html

Overall, the Sega Gun Sense Board was a critical component in many popular light gun arcade games and contributed to the success of the genre during the 1990s and early 2000s.

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- FIRMWARE -->
## Firmware

There are 3 known firmware revisions for the 838-13146 and 838-13143-XX boards:

EPR-20006A - Probably only supports 12 LED  
EPR-21262 - Supports 12 and 10 LED  
TG12 - Supports 12 and 10 LED  

Dumps of these firmware ROMs are available in many places online (including NAOMI BIOS sets or House of the Dead sets, however I have also included them here on this repository. I do not own the rights to this and I believe these would be owned by Sega.

I have dumped my own chips and using the SHA-1 hashes have confirmed my original sense chips match the dumps available online. using PowerShell you can compare your own chip dumps to the online versions using the following SHA1 hashes and example command.

SHA1 Hashes:  

EPR-20006A - b7cf40a1671dc351b607d8d6bba0d51ea128eb75  
EPR-21262 - fc2a331430ef2f009f653b242220599c824cd1d2  
TG12 - 91813a43851c48d400fde41b1198dabf55bade2d  

Example PowerShell command:

get-filehash .\tg12.ic2 -Algorithm SHA1  

EPROMS known to be used and compatible:

ST M27C512-12FI 58808 9819E  



<p align="right">(<a href="#top">back to top</a>)</p>

<!-- RESOURCES -->
## Resources

http://solid-orange.com/1611

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

As people contribute their names will be added to this list, with thanks.

* []()
* []()

<p align="right">(<a href="#top">back to top</a>)</p>
