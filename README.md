# xboxroller
These files are a set of pd pure data patches that utilize an xbox controller. The xboxcontrollertpl.pd file is an attempt a template for starting new projects and does not produce sound, it is instead a set of visualization of the controller input.

using windows and pure data vanilla with hidin (for windows only) and cyclone

the inputdevices file is roughly equivalent to the one shown in this video: https://www.youtube.com/watch?v=MbGxJtenvkQ

the hidin directory should go in Pd>extra per usual: http://puredata.info/docs/faq/how-do-i-install-externals-and-help-files

the first step is to bang hidin for the print message output. Then the console shows something like this:

hidin: ** found 2 devices on your system

-1 None
1 Afterglow Gamepad for Xbox 360 (Controller)
2 Nintendo RVL-CNT-01

And then since I know I want the Xbox Controller I pass an "open 1" message to hidin. Then the route object shows me the numbers for the input from controller.

Alternatively you could just guess ("open 1", "open 2", "open 3," "open 4", etc) and hope to get lucky

The "sounds" directory can be ignored. The "instances" directory holds patches that utilize the template and output sound.