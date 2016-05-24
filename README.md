# Senior-Project a Blog of Senior Project Updates
######March 31, 2016

I somehow managed to lose my webpage for this project....

######April 12, 2016

I've managed to complete the CodeAcademy tutorial for java. I now have a basic understanding of the structure of java and simple commands. I've downloaded Android Studio which will be my coding environment for the project. I have also borrowed an Android phone from the innovations lab which will serve as a test device as I progress.

######April 28, 2016

First day of Senior projects! I'm beginning to realize what I've gotten myself into. I just finished reading through the guide on how to make your first app. Seems very challenging. The course on how to use all the api's says it requires three years of coding experience. I've got about three weeks. This is going to be so much fun. Also I've been sick all day so I've been very unproductive.

######April 29, 2016

I finally found the developer controls on the phone! Only took an hour or so. Turns out ZTE phones hide them in a different place than standard Android phones. It's under a different tab and labeled differently. Plus they make it so you have to tap the icon four times before the developer controls get turned on. 

Spent the last couple of hours trying to get the phone to connect to the Android Studios. I can access the files on the phone but the studios won't recognize the phone as a device. No idea why. I have tried changing the way the phone connects, MTP and PTP, most of the developer controls and tried installing google usb software. None of it has worked. Very frustrated with this whole thing. 

######May 4, 2016

After several days of sickness I'm finally feeling well enough to look at a screen. Today I completed the button intro. Took a while but taught me how important the order of code is. In the Android Studio, there's several sections of code generated with every new tab opened and certain things have to go in certain places or it returns errors that point back to the base code. Which is very frustrating. However now I know how to start new activities and activate them using buttons. 

######May 9,2016

Over the last few days I've been planning out the interface of the app. I now want to have three screens. One of select a color to change, one to select the replacement color and a final one to display which colors have been changed. I found someone elses project that has a color picker which I plan to use. It'll teach me how to imbed other peoples libraries into my own project. Today I had a mix-up with build values. The phone that I'm using to test uses an older version of SDK so I had to figure out how to change that. They make it pretty easy. Just change a value and the whole build recompiles into the new version. 

Currently I am trying to create my own button that starts another activity without the help of the guide and I am failing miserably. There's going to be a lot of that I feel like. The guide walks through a bunch of steps that seem like they shouldn't matter like displaying message, sending the string with the message in it etc. I want to eluminate those steps somehow. It's an interesting balance of not putting lines then realizing I need them or putting lines and realizing I don't need them. The whole things very frustrating.

And it works! The button now opens a new activity! Now I have to embed a library into it.

I have now added the color selector to the second screen. Seems to work pretty well. allows most colors to be selected very easily. Now I need to find where the output of what color that's selected gets put. I'll then hopefully add a way so that the background changes based upon the color selected. Only problem is the white in the center is pretty hard to select.

######May 10, 2016

I've found the script for the color picker. Now I just have to move the parts I need into the script I have set up. After looking into how to add the color selector, I decided to try to add the color selector as a library. Tomorrow I will be looking more into that.

######May 11, 2016

I've decided to change the format of the project. Now instead of having three screens I hope to only have two. The first one will have four buttons on it. One to select a color to change, another to select the one that is replacing the first one, the third to confirm that the change should be made. Once the third is pressed the colors should reset. The final button will be used to access the second screen which will show all the changes that have been made. Hopefully I will have little 'x's next to them to revert the change but that may not be feasible. This whole thing seems like a big stretch with my limited knowledge but we'll see what happens. 

This is very interesting. I tried to import the library by including both a statement saying its dependent on the color picker. Then that didn't work for some reason. So I tried to putting an include "color picker file name" in the gradle settings. That fixed a lot of the problems but not all of them. I feel like I'm still missing some part of the library but I don't know where to look to get it. Also including the file name generated three new files. So now I have the app file, a color picker file, a com.github.QuadFlask, and a 0.0.10 file. The last three files are all blank tho. But when I tried to copy the color picker dialogue into the file, most of its still says there's an error. 

I think I was finally successful in installing the library into my build. There are still several problems with the build but hopefully I can fix those tomorrow. This project is incredibly frustrating.

######May 12, 2016

I'm going to start making a set of goals at the beginning of each day so that I have a set stopping point. Today my goals are to add the two buttons to the Color Picker app and to learn about hexadecimal colors and how android reads them. I have abandoned the idea of building my own app from the ground up and have chosen instead to modify the Color Picker to do what I want it to. I have also changed the layout design from being three buttons to two. One to select the new white point and one to run it. I may just fall back on having one button. I've decided to just change the white point of the screen because that way every variation of white will be included. Hopefully this will allow me to be more successful in this project.  

I managed to add the two buttons and begin working on the dialog for the run button. I want to have it pop up a dialog asking if the user is sure they want to change the color of the screen. 

######May 13, 2016

Today I'm going to finish the dialog hopefully. I found some code to use online now I just have to make it work. That seems to be how I'm doing most things now. Finding a base to stand on then changing it to fit my purpose. I really don't know enough to write things from scratch. 

I think I'm going to create an overlay of the screen. It won't be as effective but I can do it much easier than changing the actual colors. It'll be basically what they give you to fix the light disorders, a thin film that you can place over books or computer screens. Phones are harder because they're touch so this would allow you to just use this instead. Apparently overlays disable Android from installing apps due to the easy potential for scamming. 

I managed to write the confirmation dialog to Android Studio's liking, however I can't seem to get it to run off of the button. I tried several different things but none of them seem to work. I tried several different ways of recieving the output but they won't run. The button's in a different activities xml file and that might be messing with it. Tomorrow I'll try using intents to activate that program. We'll see how it goes. 

######May 14, 2016

I've run into the weirdest problem. So java won't let me put the second dialog in the same folder as the first so I had to move it into another folder. Then in order to run that file I have to use intents. Once that file runs though, it doesn't just run the dialog, it changes the layout as well. Then you have to click on the run button a second time in order for the dialog to pop up. But when I tried to put the dialog just into one folder, it gave a ton of errors.

And it works!! The Alert Dialog Fragment just had to be put under the Sample Activity Class. Getting everything in the right brackets is pretty hard when transferring code between classes. Now I will put an intent statement under the confirm button that runs the overlay part. 

######May 16, 2016

Today I'm starting the overlay part of the project. This is should comprise the bulk of what the work I'll do on the project. Everything I've done so far has been leading up to this. Fun day today. I made an overlay that should go over the screen on every app. Unfortunately I have no idea how to set the color. This also means that there's no way to test if it's actually working because it's a blank screen. 

######May 17, 2016

This project is starting to get enjoyable. It's still extremely frustrating, but I'm starting to learn enough to move code into where it's supposed to be. 

Just as I say that the next part gets extremely annoying. I put the method getSystemService into one Colors, only to realize that the section its in needs to be its own activity, ColorOverlay. Then upon transferring it into the new activity android no longer recognizes getSystemService as a method even though it's defined under the import Context which I imported into both. In order to fix the error on that line, I have to have the class extend IntentService, but that triggers another error saying that Service needs to be an abstract class. Turns out it was supposed to be the Service class I just had to use IBinder to do do something. 

Next problem. The program crashes when trying to run the overlay. It says that "ColorOverlay" needs to be defined as an activity in the manifest.xml file. When I define it as an activity, android studio says its wrong and should be defined as a class. Changed the startActivity to startService and it works. Also defined ColorOverlay as a service. Had to give it permission to access the rest of the phone. It works with a set hex value now I need to make it work with the variable. The color selector outputs a integer which is weird. I think it's supposed to be a hex string. 

In order for this to work, the value has to be in the format 0xAARRGGBB. Where A is the alpha value, R is red, G is green and B is blue. However, the value that the color selector outputs is an integer and doesn't have the 0x on the front. So somehow I have to put that there then assign it to a new variable. 

######May 18, 2016

Today I should have a working project! All I have to do is make a the selectedColor into a global variable. I'm going to do that using shared preferences. Hopefully this will not only allow other activities to access the variable but it should also save it between startups which would be nice. 

I think I've managed to create a sharedpreference string. But I can't seem to call it. For some reason android studio keeps saying it doesn't recognize the name.

######May 19, 2016

And the app works! The only problem is you can create overlays that completely hide the screen. I managed to create the sharedpreferences. I had to import Colors into ColorOverlay in order to make it work. But now I can effectively bluescreen my phone over and over. The app doesn't have any way to call an onDestroy() for the overlay so it remains until you reboot. I'll try to implement one of those today. Also I'm going to try to limit the Alpha channels levels so that it doesn't completely cover the screen.

######May 23, 2016

Over the last several days I've trying to implement a way to remove the overlay. I think I created a way to do it but I'm not sure. I think the app calls a method when it gets cancelled out called onDestroy(). This can be set up to remove the overlay. However, it only works if you close the app exit it out, open it again then close it out again. Also the first time you close the app it removes the overlay for a second then it comes back. It then removes the overlay but if you try to open the app back up again the entire screen is overlayed with a white color. Then if you click the button to close apps down and manage to swipe off of the app it removes the overlay for about 10 seconds then it comes back. 

The app has to be creating an overlay on start or on destroy. The white value is the default value of the app when it boots up. So when it must be setting the chosen color value equal to the white then when it boots up again it activates that color as an overlay? 

######May 24, 2016

Today I did a lot of things. First I set up a way to remove the overlay but for some reason it doesn't work right. Then I tried to change the app launch picture but my computer ran out of memory and froze when I tried to upload the picture I wanted. So I tried again and it froze again. So I don't think I'll be able to change my app selector.  
