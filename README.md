Change-Resolution-Easy
I made a UI application that does the same thing without you needing to manually edit files.
Just open and change your monitor resolution with a single click.
This tool makes switching your primary monitor’s resolution quick and effortless. It’s especially useful if you frequently change resolutions—like when casting your screen to a TV or using an ultrawide monitor.

How to Use Tools:

Copy the folder to your C: drive so it appears as C:\Tools.
Open the .bat file located at C:\Tools\ResolutionToggle and edit the text at the bottom to set:
The resolution and refresh rate you want to switch to
Example configurations:

  :: Last resolution was 1920x1080, switch to 3440x1440
    echo Switching to 3440x1440 @ 180Hz...
    %NIRCMD% setdisplay 3440 1440 32 180 -primary
    
  :: Last resolution was 3440x1440, switch to 1920x1080
    echo Switching to 1920x1080 @ 120Hz...
    %NIRCMD% setdisplay 1920 1080 32 120 -primary

What you change:

   :: Last resolution was width)x(height, switch to width)x(height
    echo Switching to width)x(height @ (the hz)Hz...
    %NIRCMD% setdisplay (width) (height) 32 (hz) -primary

and then just change it the other way round for the next config

Save your changes.

Create a shortcut to the .bat file on your desktop or Quick Access bar for easy access.
(If you don't create a shortcut for the bat file it will keep creating a flagfile on your desktop)

Now, changing resolutions is as simple as a single click!

This was made possible with the help of
nirsoft net
