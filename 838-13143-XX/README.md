# IC BD Gun Sense (838-13143-XX)
<div id="top"></div>

<!-- SUMMARY-->
## Summary
<img src="https://raw.githubusercontent.com/theretrobristolian/Arcade/main/838-13143-XX/838-13143-XX.svg">

The above is a basic representation showing the layout of the most common type of IC BD Gun Sense boards - the throughhole component type. This covers boards 838-13143-03 to 838-13143-11. 838-13143-01 and 838-13143-02 are believed to be an earlier, slightly different layout due to the lack of HOD/JUL DIP switch.

The Sega Gun Sense Board 838-13143 is an arcade board developed by Sega in the 1990s to provide accurate aiming and shooting mechanics in light gun games. The board was first used in "The Lost World: Jurassic Park" arcade game in 1997, where it was paired with Sega's Type 2 (Type II) light gun.

Over the years, Sega released several revisions of the Gun Sense Board. The initial release was specific to "The Lost World: Jurassoc Park" and was designed for 12 sensors around the screen not 10 (which was the new standard on the later revisions - although these boards are backwards compatible. These boards can be found in games from the late 90s right up through the 2000s as the technology didn't fundementally change.

The technology was based on a design by a Japaneese company OHMIC, the link to this is here http://www.ohmic.co.jp/cat/zahyou-01.html

Overall, the Sega Gun Sense Board was a critical component in many popular light gun arcade games and contributed to the success of the genre during the 1990s and early 2000s.

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- BOARDREVISIONS -->
## Board Revisions

There were multiple attempts to revise the board design however over all the boards look very similar so the changes must be minor (and at this stage I have no documentation to explain what they were). However I've created a table of the key knowledge I am aware of:

| Board         | Firmware      | Fullname               | Game                               | Game Release Date | LED No.  |
| ------------- | ------------- | --------------------- | ---------------------------------- | ----------------- | -------- |
| 838-13143-01  | EPR-20006A    | IC BD GUN SENSE       | The Lost World: Jurassic Park      | 1997              | 12 Only  |
| 838-13143-02  | EPR-20006A    | IC BD GUN SENSE       | The Lost World: Jurassic Park      | 1997              | 12 Only  |
| 838-13143-03  | EPR-21262     | IC BD GUN SENSE HOD   | House of the Dead 2                | 1998              | 12 or 10 |
| 838-13143-03A | EPR-21262     | IC BD GUN SENSE HOD   | House of the Dead 2                | 1998              | 12 or 10 |
| 838-13143-04  | EPR-21262     | IC BD GUN SENSE HOD   | House of the Dead 2                | 1998              | 12 or 10 |
| 838-13143-05  | EPR-21786A    | IC BD GUN SENSE FRQ   | Brave Fighters                     | 1999              | 12 or 10 |
| 838-13143-06  | EPR-21262     | IC BD GUN SENSE JPT   | ?                                  |                   | 12 or 10 |
| 838-13143-07  | ?             | ?                      | ?                                  |                   | 12 or 10 |
| 838-13143-08  | TG12          | IC BD GUN SENSE SPY   | Confidential Mission               | 2000              | 12 or 10 |
| 838-13143-09  | TG12          | IC BD GUN SENSE SPY UR| House of the Dead 3                | 2002              | 12 or 10 |
| 838-13143-10  | ?             | ?                      | ?                                  |                   | 12 or 10 |
| 838-13143-11  | ?             | ?                      | ?                                  |                   | 12 or 10 |

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- FIRMWARE -->
## Firmware

There are 4 known firmware revisions for the 838-13146 and 838-13143-XX boards:

EPR-20006A - Probably only supports 12 LED  
EPR-21262 - Supports 12 and 10 LED  
EPR-21786A - Which at this stage is a somewhat rare and undocumented firmware used for Brave Firefighters - this may have something uniquie it it for that game  
TG12 - Supports 12 and 10 LED  

Dumps of these firmware ROMs are available in many places online (including NAOMI BIOS sets or House of the Dead sets, however I have also included them here on this repository. I do not own the rights to this and I believe these would be owned by Sega.

I have dumped my own chips and using the SHA-1 hashes have confirmed my original sense chips match the dumps available online. using PowerShell you can compare your own chip dumps to the online versions using the following SHA1 hashes and example command.

SHA1 Hashes:  

| Firmware    | SHA1 Hash                                      |
|-------------|------------------------------------------------|
| EPR-20006A  | b7cf40a1671dc351b607d8d6bba0d51ea128eb75         |
| EPR-21262   | fc2a331430ef2f009f653b242220599c824cd1d2         |
| EPR-21786A  |                                                |
| TG12        | 91813a43851c48d400fde41b1198dabf55bade2d         |


Example PowerShell command:

`get-filehash .\tg12.ic2 -Algorithm SHA1`

<!-- Firmware EPROMs -->
## Firmware EPROMs

The Firmware ROM dumps are 64KB each which is 512000 bits, so the original EPROMs were 512K. In my limited research I have found the following EPROMS to have been used:

ST M27C512-12FI 5880S 9819E  
ST M27C512-12FI 5880S 0070X  
ST M27C512-10FI 8882X 0130L  
ST M27C512-15FI B8886 9609E 

This would seem to suggest 150ns or quicker is acceptable.



<p align="right">(<a href="#top">back to top</a>)</p>

<!-- LEDARRANGEMENT -->
## LED Arrangement

<img src="https://raw.githubusercontent.com/theretrobristolian/Arcade/main/838-13143-XX/10LED.svg">
<img src="https://raw.githubusercontent.com/theretrobristolian/Arcade/main/838-13143-XX/12LED.svg">

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
