# Go-Faster-slot-covers
Building upon work done by [EngineerNick on youtube](https://www.youtube.com/channel/UCNkQ3_g0wfXJV7Hy6gSzFiw) creating custom silicone tubing using caulking silicone Go-Faster Slot Covers uses 3D printed dies allow the extrusion of complex custom profiles. These dies screw directly onto the end of standard caulk and are compatible with standard caulk guns. Go-Faster Slot Covers is aimed at custom slot cover/inserts for aluminium extrusion, but the 3D printed dies work for other profile and were initialled use to make silicone tube with great success.

This is being released because no slot cover could be found for MakerBeam XL which is used in V0 by Voron Design. This seems a simple and cheap, if a bit laborious, method to make a lot of slot cover. Importantly it can be done with parts readily available that are cheap. It can even compete with AliExpress where 2020 slot cover can cost ~£0.35 per metre + shipping, a 300ml tube of silicone gets you 15 metres and costs ~£5.50 so you pay £0.36 per metre for material.

## Requirements
### 3D printing
Access to 3D printing is of course needed, both FDM (PLA/ABS) and SLA (DruckWege Typ D) have been tested and found to work.

Due to the high pressures the extrusion generated the dies need to be strong and so they should be printed solid. For FDM layer adhesion should be prioritised with higher extrusion temperatures, layers thicknesses of <40% of the nozzle diameter and potentially less part cooling. 

SLA is currently preferred to FDM since it can produce the fine detail required for the current slot profile. FDM rounds the corners off too much with standard 0.4mm nozzles, smaller nozzles may work but will require exponential more print time due to the part strength requirements. Methods analogous to optical proximity correction are being investigated to allow FDM to reproduce some of the fine detail with standard nozzles.
### Silicone
It would seem almost any 1-part caulking silicone will work with this method, though this project has so far used Aqua Mate Aquarium Silicone and Rainbow RAL Coloured Silicone. The models are designed for standard ~300ml silicone tubes with a M16x2 thread on the end which seems to be the standard thread. You get many meters of extrusion per tube, e.g. the MakerBeam XL profile uses ~1 ml per 100mm so you get up 30 metres out of a single tube.

The standard ratcheting caulk works well if a bit slow, tedious and straining on the hands. Electric caulking guns look promising but have not been tested yet.

### The Hot Bath
For the extrusion to work the silicone has to cure quickly, which is achieved by extruding into a hot water bath. The hotter the bath the better though safety first so keep it below 60 °C. Keeping the bath hot is definitely useful (topping up from a kettle or directly heating the bath) but not necessary if only extruding small amounts. Dish soap seems to help stop the silicone extrusion sticking to itself though the surface bubbles should be skimmed off as get in the way of extrusion. Adding hydrogen peroxide is useful as it catalyses the curing reaction in 1-part silicone, but it is not strictly required.

The bath itself should be large, an actual hot soapy full-size bath sans bathing person might be the ideal bath to use. However, all the work done in this project used either washing up bowl or a large cooking pot. The more space the easier it is to get good extrusion that doesn't get tangled and twisted, being able to walk around the bath is also useful.

Note that a light amount of stirring also seem useful for long extrusions, so a low speed magnetic stirrer or the occasional manual stir is good.

### Misc.
An oven is useful to post-cure the silicone at higher temperatures while being safes and non-disruptive (unlike boiling water).

## Method
1. 3D print the die, not support required as mentioned before making it solid and prioritise layer adhesion.
* Make hot bath, e.g. fill up a washing bowl with hot and soap as if you were about to wash dishes in it (be liberal with the soap)
* Assemble die, caulk tube and caulk gun
* Aim caulk gun into bath while in a comfortable position
  * The comfortable position is important as you will be there for a while
  * If you can do so safely resting the caulk on the bath rim helps
* Extrude slowly and steadily; it is slow but too much too fast risks either splitting the die or destroying the thread in the 3d printed part
  * If you can get a good ratchet rhythm there are no seems in the extrusion when you release the ratchet
  * The bigger the die area the faster you can extrude, expect 100-200mm a minute with the MakerBeam XL's slot cover  
  * To steal distilling terminology, discard the heads and the tails of the extrusion as these are rough
* You can handle (with care) the extruded silicone quite quickly when it is in the water, so you can lightly push and prod it about the bath
  * Leave for 20 minutes before handling out of water, e.g. taking it out of the bath
* Depending on the silicone you can now test it,  
  * If when squished it returns to its original shape it can be used even though it is not fully cured
  * Leaving it fully cure is advised though, if possible, cut it to length first lay it out straight and separated
    * It can still partially stick to itself and take on deformed shapes as it cures (leave slot cover to fully cure in extrusion works)
  * Post-cure it in an oven @ 80-100 °C if you can (depending on the silicone used)
* Done, you should now have custom silicone slot covers or whatever profile you want.
  * Do not fret if it is twisted or slightly the silicone is very forgiving especially when jammed in an aluminium extrusion's slot
  * kinks or other sharp and short artefacts can be problematic, usually best to cut and discard
  
## Going Forward
* More aluminium profiles to come, Bosch Rexroth 6mm 2020 is modelled but not tested.
* Slot inserts beyond just covers are in the works.
* Improving the finish of the extrusion by smoothing the bore/profile of the die
* The OPC-like idea to get FDM working for small profile i.e. MakerBeam XL
* Separating the part into the die and the mount, similar to how proper extrusion is done, this allowed
  * One to make the die reusable
  * Allow the die and the mount to be fabricated by different methods, e.g. FDM for the mount and send of the dies to be made externally with SLS/Laser/Waterjet/EDM/ETC
* Possibly remove the flange or make flanges-less version, the flange can just breakoff with some caulk tubes and the thread seems to hold up fine
* eBay is begin watched for a cheap electric caulk gun to see how well they work for this
