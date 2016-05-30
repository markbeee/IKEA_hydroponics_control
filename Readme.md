##Project to control IKEA hydroponics Krydda/ Växer

#### Planned items

Control growth with microcontroller/ embedded system and sensors (light, humidity, temperature, CO2, water level etc.)  utilizing automated lighting and water refill with the new IKEA Krydda/ Växer system.

##### Sensors

######Light sensor (BH1750FVI)######

Monitors the amount of light the plants accumulate over the day. To save energy in the future I will only switch on the lights as long as necessary if ambient light (sunlight) is available.
You can find an [example sketch and the library for BH1750FVI here](https://github.com/markbeee/BH1750FVI). The light sensor on a breakout board is available on Ebay, AliExpress etc.

BH1750FVI connected to an ESP8266 (ESP-12) breadboard adapter board
(see my project [ESP8266 breadboard adapter board](https://github.com/markbeee/ESP8266_Breakout_Board))

![BH1750FVI breadboard setup with ESP8266](/images/BH1750FVI.jpg)
![Sensors on cultivation unit](/images/Sensors_ESP8266.jpg)

######Temperature and humidity sensor Sensirion SHT21######

Monitors the actual environment values of temperature and humidity. Might be helpful if one of the values gets out of the comfort envelope for the plants.
You can find an [example sketch and the library for SHT21 here](https://github.com/markbeee/SHT21). The sensor on a breakout board is available on Ebay, AliExpress etc.

#### Firmware sketch for ESP8266 with web dashboard on adafruit.io

To monitor your cultivation unit from local/ everywhere I wrote a [sketch](https://github.com/markbeee/IKEA_hydroponics_control/blob/master/firmware/Krydda_growth_control_Adafruit_io/Krydda_growth_control_Adafruit_io.ino) to both send the actual values via the serial port and to adafruit.io which is a nice web service for displaying data in the internet (of things).

Demo-Dashboard of my [Krydda system](https://io.adafruit.com/markb2/growth-control) 

![Adafruit.io dashboard](/images/Adafruit_io_dashboard.jpg)

You can get more information on how to set up your own dashboard on adafruit.io [here](https://io.adafruit.com/)
 
#### Pictures from the seed and growth

| Parsley | Pak Choi | Chard | White cabbage | Rocket | Large-leaved chicory | Curled-leaved endive | Parsley | Watercress | Basil |
|---------|----------|-------|---------------|--------|---------------|----------------|---------|------------|-------|

Day 0 (initial seed)

![Initial seed day 0](/images/Day0_git_800w.jpg)

Day 3

![Seed day 3](/images/Day3_git_slant.jpg)

Day 6
~~(Parsley looks like it's dead seed)~~ Parsley needs much more time to germinate - RTFM! (about 14 days)

![Seed day 6](/images/Day6_git_slant.jpg)

Day 0 (in a new home)
Seedlings moved to cultivation unit

![Cultivation day 0](/images/Day0_git_grow.jpg)

Day 12 in cultivation unit
![Cultivation day 12](/images/Day18_2_3_4_5_labeled_blog.jpg)
![Cultivation day 12](/images/Day18_6_7_9_10_labeled_blog.jpg)
