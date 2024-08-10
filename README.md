# Extending Bridge
## Overview
**Starting Date:** July 2022

**Project Completion:** October 2022

**Motivation:** University Assignment

**Status:** Complete


This was a project I worked on in my first year of university to design and build an extending bridge. Although I've completed a lot of projects during my degree, this is one I'm very proud of.

It was created in collaboration with the students Rex Buckle, Dev Kalsi, Tinotenda Mapani and Sofia Lopez.

## Context

This project was completed as part of my first year ENG1011 Engineering Methods unit.

We were tasked with designing an extending bridge that fit within a 100x100x100mm cube when retraced and could span a 300mm gap when fully extended. The bridge also had to be able to support a 1kg load, and be opened with a hex key.

The design was modeling in SolidWorks, printed in PLA, and then assembled with screws, axles, and nuts.

I had a lot of experience with 3d modeling in Blender3d as a hobby before starting this project, so I used this expertise to complete the majority of the SolidWorks modeling for this project.
In particular, I found the spatial reasoning skills I had gained and the speed I was able to use the program was a large benefit to the team.

## Design and Features

The bridge was composed of two frames on each end, with a scissor mechanism between them.
When closed these two frames form a cube, with the scissor mechanism enclosed within them.

![The SolidWorks model fully extended](https://onedrive.live.com/embed?resid=BE406011F5E2A3C1%21816474&authkey=%21ACF7c0Q8UcIdwqI&width=1044&height=832)

![The SolidWorks model fully retracted](https://onedrive.live.com/embed?resid=BE406011F5E2A3C1%21816475&authkey=%21ALdXZph68x6tAAA&width=814&height=814)

One of the frames is the smaller follower frame, which ensures that side of the bridge can actuate freely while keeping the frame perpendicular to the scissor mechanism.
This is achieved by having the upper joints of the scissor constrained to only rotating, while the lower joints are allowed to move vertically on a track. This track also stops the scissor from overextending.

![Diagram of the follower frame](https://onedrive.live.com/embed?resid=BE406011F5E2A3C1%21816471&authkey=%21ACW3KgrcmAquJTs&width=660)

The other is the larger driver frame, and it contains the mechanism to extend the scissor.
Once again the top joints are pinned in place, however for this frame the lower joints are connected to a rack and pinion mechanism.
The scissor joint connects to a set of racks that travels vertically along a track when the pinion gear shaft is rotated with a hex key.

![Model of the driver frame, with it's rack and pinion mechanism](https://onedrive.live.com/embed?resid=BE406011F5E2A3C1%21816477&authkey=%21AAHcWTZr2FZK_Gk&width=787&height=808)

![Model of the gear shaft and racks that make up the mechanism](https://onedrive.live.com/embed?resid=BE406011F5E2A3C1%21816476&authkey=%21AJbuDc3h9EDwACo&width=811&height=807)

One feature of the design I was very happy with was the gear shaft.
This was composed of 3 separate pieces that were held  together by the side frames.
This made the printing easier as we could print each part in whatever orientation worked best for it, instead of all facing the same way.
This also allowed us to quickly replace subparts of it when they broke during testing, without needing to reprint the entire part.

![enter image description here](https://onedrive.live.com/embed?resid=BE406011F5E2A3C1%21816478&authkey=%21AN54bjqfq2HKuEM&width=885&height=610)

## Results

After a few minor issues, this design worked excellently. The opening mechanism worked as expected and it easily managed the load requirement.
This design stood out from the other student's for a few reasons. One was that ours was capable of both extending and retracting, unlike a number of other designs that utilised elastic bands or other mechanisms that could only be deployed once and not retracted. Another was that our bridge had the frame integrated into it whereas most others just had an exposed mechanism.

Overall I was very proud of this design and happy with how it turned out.

![enter image description here](https://onedrive.live.com/embed?resid=BE406011F5E2A3C1%21816453&authkey=%21AN0w8xsExxiHN-w&width=424&height=245)

A video of the opening sequence can be found below.

## Issues and Future Improvements
### 3d Printing Efficiency
One lesson I learnt very early on was to keep the printing time as low as possible. This design took 8.5 hours to print, and this was after I reduced the design to remove unnecessary solid segments.

This image shows an early model before we removed the unnecessary parts.

![enter image description here](https://onedrive.live.com/embed?resid=BE406011F5E2A3C1%21816479&authkey=%21AGiIY_M1mI3fXiI&width=975&height=888)

I also learnt the importance of understanding the printer options and setting them right the first time instead of wasting time with failed prints. When printing out the gear, which was the most complex part, we struggled to get the hex socket to be the right size. After several redesigns and a lot of time, we finally realised that the design was fine. It was the printer's filament width setting being too high, which meant the accuracy wasn't enough. Once this was fixed the design worked perfectly.

![enter image description here](https://onedrive.live.com/embed?resid=BE406011F5E2A3C1%21816451&authkey=%21AHwwB2tusou0zkc&width=552&height=179)

### Fail Fast

An unforeseen issue we encountered was that we were unable to test if this design would work and be able to carry the load until after it was printed.
This meant if it did fail, we wouldn't be able to redesign and print a new version before the deadline.

In the end this design did succeed admirably. However it came close to failing when the rack would loose traction with the pinion gear due to the PLA bending under the load. This was fixed by printing and adding a bracket that stopped the rack from bending, however this could have required a major redesign.

It was a important reminder of the engineering principle of "Fail Fast", or testing in increments so if the design failed it would fail quickly before we invested too much time into it.
In the future I would just design a mounting for the mechanism without printing the rest of the frames to ensure it worked. I would only commit to printing the larger frames once I was sure the mechanism worked and was sttrong enough.

## Viewing the Model
The SolidWork model are available in this repository, and have been tested in SolidWorks 2024.

The main assembly file is:
ScissorBridgeFinal.SLDASM

## Further Links
- [Video of Bridge Deployment](https://1drv.ms/v/s!AsGj4vURYEC-sepVkZ4p2qBsM1MrJg?e=dqk6c2)
- [Slides used during pitch presentation.](https://1drv.ms/p/s!AsGj4vURYEC-sepWxoLERqLRnZ4RdQ?e=KtqlJ5) (Note that team member pictures have been removed for privacy)
