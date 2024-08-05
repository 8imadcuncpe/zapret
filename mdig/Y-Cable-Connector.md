
 
I am trying to run a cable between holes in two parts, fix one surface of one part and apply a normal load on one surface of the other part. I am basically trying to see how the cable responds to tension. I am getting a singularity error and I believe it is due to lack of constraints.
 
**Download File ✺✺✺ [https://ammetephy.blogspot.com/?d=2A0Set](https://ammetephy.blogspot.com/?d=2A0Set)**


 
I would greatly appreciate any suggestions as to how I can find a solution to my problem without over constraining my setup. I am unable to get rid of the error unless I have at least one edge/surface of the "loaded" part fully constrained.
 
The answer to your question "how does the cable respond to tension" is this. The cable/rod responds to tension the same as any slender tension element. The displacement = force\*length/modulus of elasticity/cross sectional area. The force in the cable/rod is equal to the applied load (because it all goes through the cable/rod), and everything else is known from the input and the geometry.
 
Thank you so much for your detailed response. I am fairly new to Nastran and I am not a regular FEA user either, so I am having a really hard time understanding most of what you suggested. I hope you wouldn't mind some follow up questions I have to make sure I am going in the right direction.

1) I have switched to Nonlinear Static analysis mode. I am assuming that rods and cables are solved differently in Nastran, so I would like to keep working with a cable to replicate my real world problem.
 
2) To make it simple and figure out how to work this thing first, I have removed the holes and now I'm just running my cable from one surface of one block to the closest surface of the other block. I have also created nodes on the blocks, at the cable end points.
 
You can buy just the cable through their aliexpress store front, but it doesnt say exactly what connector type it is
 aliexpress.com 5.51US $ 5% OFF|CUAV CAN PMU lite high voltage power management module...Smarter Shopping, Better Living! Aliexpress.com
 
It's entirely possible to cut off the plug and install a new one, but you will need a crimping tool. It's about $15. The thing is, your local store will probably charge you more than $15 for a cable - even if you buy it online, it'll probably be close to that when you take shipping into account. Therefore, it's cost-effective in my opinion, even if you only need it occasionally (and those pieces tend to break somewhat frequently, in my experience).
 
For a quick fix, I've successfully used a small piece of paper to wrap the 3 non-conductor sides of the socket and then insert the cable into the socket. Leave some paper extending outside the socket so you can prevent the plug from just pushing the paper into the socket. This hack can work for years, if there is not a lot of movement of the device or cable.
 
Slip a RUBBER BAND all the way under the plug clip if the locking plastic clip is cracked but not broken off. The rubber band will lift the inner non-broken part of the clip just enough for you to hear or feel the click when it locks in place. You can remove the plug by pressing down on the clip and rubber band as usual.
 
This works for a SEMI-PERMANENT FIX, in case you rarely re-insert the plug, to avoid having the cable plug annoyingly disengage when you accidently move the cable or router, especially when you are unaware of it.
 
You can always cut the broken end and add a crimpless plug. Here is an example. They are more expensive than a crimped end, but perfect for an emergency. Different brands/models have different capabilities such as self cutting the wires.
 
Service Wire is a multi-generation, family-owned wire and cable manufacturer and has been since 1968. We are committed to producing the finest quality American made products while providing industry-leading service levels.
 
Our nationwide network of distributors and advanced distribution capabilities enable us to meet and exceed the often-complex needs of industrial, commercial, utility, pump, and irrigation customers throughout North America and the world.
Click here to learn more...
 
The pitch was not listed for the connector on the board. This is measured from the center of one pin to the center of the next one. You can review the options to see if you can make one of these work.
 
It looks like a right angle connector. If it was a hinged flip lock that broke off, Click here for the closest matches, that I was able to find. You will have to check the datasheets to verify compatibility, and whether you need top or bottom contacts. (Will depend on how the cable plugged into it).
 
We use cookies to provide our visitors with an optimal site experience. View our privacy notice and cookie notice to learn more about how we use cookies and how to manage your settings. By proceeding on our website you consent to the use of cookies.
 
i just harvested a touch pad from an old laptop and have got it working great with arduino (PS2 protocol).
the touch pad has a tiny, 12 connector ribbon cable (basically like this but smaller).
so far i have managed to (barely) connect it using alligator clips, but of course they snap off at the slightest touch.
 
my question: can i buy the connector for these ribbon cables? i tried soldering a wire to another ribbon cable and it just melted away, and i cannot desolder the receptacles on the old motherboard. i would greatly appreciate any help, this touchpad really gets my mind going!
 
I'm not sure how the sensitivity compares on the two, haven't used either with the Arduino yet, but here's the links for the two.
 \_info.php?products\_id=8977
and connector:
 \_info.php?products\_id=9105
 
By using really fine wire, you can do the solder joint very quickly, and avoid melting the ribbon cable. Pick up some self-closing tweezers with long parallel jaws (I got mine for a couple of bucks each at the flea market), and use them to hold down the wires as you solder them. Having the wire steady also makes it easier to do the soldering quickly.
 
i actually just broke my connector, does anyone have any tips on how i can get that fixed and how much does it cost, if i can do it myself please tell me how. i just bought a brand new battery but now i have to keep my mac plugged in while im using it.
 
I actually don't think you broke anything. The ZIF connector looks perfect. I'm wondering if the sticker which normally goes over the whole connector is hiding the cable end which is supposed to plug in here. I can still see the two notches which would be the parts that catch in the ZIF connector.
 
The function of the lever that you're now missing is to act as a cam to exert pressure on the pins to press them down onto the flex cable. This serves two purposes; first to make a solid electrical contact between the connector and the cable, and second to secure the cable in place so it doesn't slide out on its own.
 
I ran across a discussion on the Electrical Engineering forum on Stack Exchange where they were talking about this exact problem. The original poster was looking for a replacement connector, which would have to be removed from the board (using hot air rather than a soldering iron, I believe) and then the new one installed. Since this is iFixit and not Professional Repair Technician Discussion Forum, I'm going to go with the assumption that replacing the socket would be more of a last resort for you, as it would be for me. Here's a link to that discussion.
 
So the two choices we're left with are to either repair the existing socket or find another way to secure the cable. It seems quite likely that it would be possible to replace the missing lever; however, that means you have to a) locate a suitable replacement, b) successfully remove the lever from it, and c) succeed in installing it into the socket that's missing it.
 
The final option would be to make it work as is. The best idea I saw on the Stack Exchange forum was to place a piece of thin plastic under the cable and insert it along with the cable into the connector. It will (and should) be a tight fit, so you'll have to be careful not to damage the cable while you're basically forcing it in, but the extra thickness provided by the plastic piece will press the contacts up to those on the connector and give you a satisfactory connection between the two.
 
The last piece of this puzzle is figuring out how to secure it. It may be fairly secure by itself, depending on the thickness of the plastic and the routing of the cable, but you might want a bit more assurance. Personally, I think a dab of hot glue placed where the flex cable goes into the connector would probably do the job; you could also glue it in place but I'm thinking the hot glue would be more amenable to being removed when the time comes to disconnect the battery again in the future.
 
I just came here to say I had a similar issue with the keyboard data cable on a MacBook Pro 15" Retina display, the clip broke off when I was closing it after replacing the battery. Ugh. The keyboard worked except for select keys as the connector wasn't holding the contacts to the ribbon I assume. I read your comment, and was able to trim a small piece of clear plastic from the packaging iFixit sent the replacement battery in, slide it into the connector and then push the ribbon cable into the connector tightly. Voila. Genius! Thank you so much.
 
So you may only need a new ribbon cable if the end is damaged. As you hadn't posted it I have to assume the real issue is you can't feed the cable in as in the current state the connector won't accept it until you open it up.
 
If that's the case, is the end of the cable still intact? That is, the part with the little gold fingers that slips into the board connector? If it is, you should actually be okay; I'm not sure exactly what the function of the cable part is, but I'm pretty sure you