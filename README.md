# KismetMobileDashboard

![screenshot](https://raw.githubusercontent.com/elkentaro/KismetMobileDashboard/master/kismetMobileV2.jpg)


###Prerequisite: git-master level kismet. ([https://github.com/kismetwireless/kismet]())

## 1.Installation.

 - git clone into the kismet git. ("/home/[whatever]/kismet") 

 		 wiPi@YoMama:~/kismet# cd ~/kismet
 			
 		 wiPi@YoMama:git clone https://github.com/elkentaro/KismetMobileDashboard.git
                
- cd into kismetmobiledashboard

- sudo make install

	`wiPi@YoMama: sudo make install`
- restart kismet

	### if you have issues :
	
	You can install the plugin manually too.(not recommended)
		
		1. git clone clone https://github.com/elkentaro/KismetMobileDashboard.git
		2. sudo mkdir /usr/local/lib/kismet/mobiledashboard
		3. sudo mkdir /usr/local/lib/kismet/mobiledashboard
		4. sudo mkdir /[USER FOR KISMET:root or regular user home directory ]/.kismet/plugins/mobiledashboard
		5. cd KismetMobileDashboard
		6. sudo cp -r httpd /usr/local/lib/kismet/mobiledashbaord/
		7. sudo cp manifest.conf  *[USER FOR KISMET:root or regular user]*/.kismet/plugins/mobiledashboard/
		8. Restart kismet.

	

##2.Access it via : 
	http://localhost:2501/plugin/mobiledashboard/

The trailing "**/**" is important. Without it you will get a 404.


To get "full screen" UI , access the page via your normal browser on the mobile device and then create a shortcut on the "home screen."

##2.How to :

**1.** Each pane can be expanded by clicking on its title.

**2.** If there is an error with a datasource. (ie: listed in the configuration file but not running, the "Active Sources" in the "System Details" pane will turn to red and show a "Source Error" .

**3.** The last pane "802.11 AP List" will show the APs detected. 
- clicking on the up-down arrow next tot the pane header will expand this list to full screen.
		 	
 **In Fullscreen mode **
 
- Click on a data row will show the Manufacturer name/Channel/List of Associated client's MAC address 


Note:
Most of my development focuses on 802.11 related stuff, so the others should work but besides BT , I don't have the means to test it. 

Its still very eary in development but it should work.

everywhere : @elkentaro (the tweets,the grams, etc etc.)