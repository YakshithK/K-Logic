#ground fill and fixing annoying red errors

session all about making the board less wires and more like actual pcb and honestly it was kinda confusing but also cool at the same time. i learned about this thing called a ground fill which is basically just dumping a big pool of copper all over the board instead of routing a million separate ground traces by hand. you grab the filled zone tool, set the net to gnd, turn it on for both layers, and use thermal reliefs so soldering later isn’t total hell with the copper just sucking all the heat away. then you smash b and like most of the gnd ratlines just disappear and suddenly the board looks way less like spaghetti and more like something you’d actually get from a fab.
​
after that it was just fighting the drc, i fucking hate drc. i ran the check and it spat out a stupid number of errors, most of them because of the ground pour being slightly wrong or pads not actually connecting how kicad wanted. i messed with the thermal relief gap and clearance to pull the fill closer, then started[ i spent too much time tryna solve drc errors lol](https://hackclub.slack.com/archives/C09HSQM550A/p1773702418651709)

![Screenshot 2026-03-16 190301](https://stasis.hackclub-assets.com/images/1774072498013-vxxnyd.png)

![Screenshot 2026-03-16 190729](https://stasis.hackclub-assets.com/images/1774072498114-hsslps.png)

![Screenshot 2026-03-16 190621](https://stasis.hackclub-assets.com/images/1774072497772-4siz5v.png)