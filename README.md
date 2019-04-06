# KismetMobileDashboard

![screenshot](https://raw.githubusercontent.com/elkentaro/KismetMobileDashboard/master/kismetMobileV2.jpg)


**Prerequisite**: You need to clone kismet git repo. ([https://github.com/kismetwireless/kismet]())

## 1. Installation

 - clone the repo

        $ git clone https://github.com/elkentaro/KismetMobileDashboard.git
        $ cd KismetMobileDashboard
        $ sudo make install

- restart kismet

### If you have issues :

You can install the plugin manually too (not recommended)

    $ git clone https://github.com/elkentaro/KismetMobileDashboard.git
    $ TOP=/home/elkentaro # or TOP=/root
    $ sudo mkdir /usr/local/lib/kismet/mobiledashboard
    $ sudo mkdir $TOP/.kismet/plugins/mobiledashboard
    $ cd KismetMobileDashboard
    $ sudo cp -r httpd /usr/local/lib/kismet/mobiledashbaord/
    $ sudo cp manifest.conf $TOP/.kismet/plugins/mobiledashboard/
Restart kismet

## 2. Access it via :
Go to http://localhost:2501/plugin/mobiledashboard/

The trailing "**/**" is important. Without it, you will get a 404.

To get a "full screen" UI , access the page via your normal browser on the mobile device and then create a shortcut on the "home screen."

## 3. How to :

**1.** Each pane can be expanded by clicking on its title.

**2.** If there is an error with a datasource. (ie: listed in the configuration file but not running, the "Active Sources" in the "System Details" pane will turn to red and show a "Source Error" .

**3.** The last pane "802.11 AP List" will show the APs detected.
- clicking on the up-down arrow next tot the pane header will expand this list to full screen.

**In Fullscreen mode**

- Click on a data row will show the Manufacturer name/Channel/List of Associated client's MAC address


Note:
Most of my development focuses on 802.11 related stuff, so the others should work but besides BT, I don't have the means to test it.

It's still very eary in development but it should work.

everywhere : @elkentaro (the tweets, the grams, etc etc.)
