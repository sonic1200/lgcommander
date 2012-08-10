## lgcommander.py
lgcommander.py is a python script for controlling your Smart Lg TV with your PC.
It can be used for gaining access to hidden menus and modes.

## To use it you need:
A PC, with python 3.x installed, connected to the same network as your Lg TV.

## Some useful codes:

* for EZ_ADJUST menu enter 255
* for IN START menu enter 251
* for Installation menu enter 207
* for POWER_ONLY mode enter 254

Warning: do not enter 254 if you do not know what POWER_ONLY mode is. You can find additional information about menus and modes here: <http://openlgtv.org.ru>   
 
As long as you do not "factory reset" your TV, pairing key doesn't change. You can use an editor to modify the line:

    lgtv["pairingKey"] = "DDGWAF"    

to suit your TV's actual pairing key.  This will eliminate the pairing key acquisition stage.


## Windows users:
You can avoid the black console window if you change the "py" file extension to "pyw".

## Newer LG Smart TV (year 2012) models:
#### Benke Tamás says: 
"I wanted to use your lgcommander script, but i realized that its not working with lg 2012 smart tv series. I made some changes, now its working with the new series, but lg changed the keycodes too. Now, there are keycodes above 255 and ez-adjust, in-start code changed too, but i dont know them yet. I attached my version, if you want to improve yours."

#### I added Benke's version of the script as lg_2012_commander.py 

#### Ajay Ramaswamy says:
quote:

Hi,

Thanks for your lgcommander script. I was playing around with my 2012 55LM6200
TV and LG has provided a Android App Smart TV which provides a remote control
app.

I ran that app thru unzip, dex2class and JD-GUI and found the file 
com/lge/tv/remoteapps/Base/RemoteKeyIndex.class contains these key mappings


        KEY_IDX_3D=400;
        KEY_IDX_ARROW_DOWN=2;
        KEY_IDX_ARROW_LEFT=3;
        KEY_IDX_ARROW_RIGHT=4;
        KEY_IDX_ARROW_UP=1;
        KEY_IDX_BACK=23;
        KEY_IDX_BLUE=29;
        KEY_IDX_BTN_1=5;
        KEY_IDX_BTN_2=6;
        KEY_IDX_BTN_3=7;
        KEY_IDX_BTN_4=8;
        KEY_IDX_CH_DOWN=28;
        KEY_IDX_CH_UP=27;
        KEY_IDX_ENTER=20;
        KEY_IDX_EXIT=412;
        KEY_IDX_EXTERNAL_INPUT=47;
        KEY_IDX_GREEN=30;
        KEY_IDX_HOME=21;
        KEY_IDX_MUTE=26;
        KEY_IDX_MYAPPS=417;
        KEY_IDX_NETCAST=408;
        KEY_IDX_PAUSE=34;
        KEY_IDX_PLAY=33;
        KEY_IDX_POWER_OFF=1;
        KEY_IDX_PREV_CHANNEL=403;
        KEY_IDX_RED=31;
        KEY_IDX_STOP=35;
        KEY_IDX_VOL_DOWN=25;
        KEY_IDX_VOL_UP=24;
        KEY_IDX_YELLOW=32;

I have tried all these codes on my TV and they work OK

I hope you find this useful and someone else can test and confirm, and speed up
the search for the Service Menu codes.

Thanks & best regards

Ajay

unquote

## This software was developed with inspiration and/or information taken from:

*   <http://python.org>


*   <http://openlgtv.org.ru>


*   An application written in ruby where you can find a comprehensive list of command codes:    
<https://github.com/dreamcat4/lgremote>
