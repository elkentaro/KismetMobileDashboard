# KismetMobileDashboard

This is a major new rewrite of the mobile UI. Ideally I want to test it more but with #hackersummercamp around the corner, I just don't have the time. 

Major functional updates:

1. Devices are now click-able to drill down in details. 
        example: Ap -> List of APs -> AP and its clients. -> client details. 
2. login via the mobile dashboard is now possible. 
3. Pause/Restart of datasources. (you cannot start/stop interfaces itself)


Limitations: 
1. Cannot start/stop interface.
2. Cannot handle non-English SSIDs.

THIS IS A VERY EARLY ALPHA RELEASE...things might not work . 


Prerequisite: git-master level kismet. https://github.com/kismetwireless/kismet

1.Installation.

 - git clone into the kismet git. ("/home/[whatever]/kismet") 
                    
- cd into kismetmobiledashboard

- sudo make install

2.Access it via : http://localhost:2501/plugin/mobiledashboard/

The trailing "/" is important. Without it you will get a 404.

Its still very eary in development but it should work.

To get "full screen" UI , access the page via your normal browser on the mobile device and then create a shortcut on the "home screen."