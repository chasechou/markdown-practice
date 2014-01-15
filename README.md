# Raspberry Pi Garage Door Opener

When I was little, I used to push the garage door button from inside the garage and
then run out the garage while it's closing... carefully jumping over the sensor so
I don't trip the safety mechanism. It was easy back then and a little fun. But
nowadays, not so much. There are times when I wish I had a way to close (and open)
the garage door remotely and preferably with something I always have on me... my
mobile phone!

So, I looked into building something so I could use my smartphone as a garage door
opener. I've read about the Arduino and Raspberry Pi platforms before that I believed
would accomplish the task and, ultimately, I decided on the Raspberry Pi. The Arduino
platform after some research and cost analysis would have cost more than the Raspberry
Pi! That wasn't something I was expecting since the Raspberry Pi is more robust and
a full-blown mini-Linux computer. The possibilities are really endless.

A wifi Raspberry Pi connected to a 2-channel relay connected to my actual garage door
remote allows me to open and close my garage door with just a browser on my smartphone.

Below I'll go through the steps and the issues I ran into while working on this project.

## Step 1 - Parts

Below is a list of the parts I gathered together to get started. Prices will most likely
not be same.

* Raspberry Pi (model B) + Case + Wireless Wifi Adapter - $50
* 8GB or greater SD card - $6
* a power supply with at least 1A and 5V output and a micro-usb connector. The power
supply that comes with most smartphones nowadays should work just fine. Just check the
label for the power ratings. The Raspberry Pi is documented to have a maximum power draw
of 1A so it's better to have a power supply that is greater than 1A just to be safe else
you might run into system stability issues causing reboots/freezes.
* a 2-channel relay - $10
* female-to-female jumper wires - $8
* ethernet cable
* a LED to test out the GPIO pins
* solder gun + solder (if hooking it up to a garage door remote)
* usb keyboard and mouse, HDMI monitor and HDMI cable. These are only necessary for the initial setup until you have the Pi networked after which you can go headless and SSH in from another computer.
Total cost for me: $74 since I had a few of the needed parts already.


### List

* item 1
* item 2
* item 3

### Ordered List

1. item 1
2. item 2
3. item 3

### Ordered List (Skip a number)

1. item 1
3. item 2?

### Source code

```Ruby
def f(x)
  x + 2
end

p f(1)
```

### ASCII art

```
           .               ,.
          T."-._..---.._,-"/|
          l|"-.  _.v._   (" |
          [l /.'_ \; _~"-.`-t
          Y " _(o} _{o)._ ^.|
          j  T  ,-<v>-.  T  ]
          \  l ( /-^-\ ) !  !
           \. \.  "~"  ./  /c-..,__
             ^r- .._ .- .-"  `- .  ~"--.
              > \.                      \
              ]   ^.                     \
              3  .  ">            .       Y  -Row
 ,.__.--._   _j   \ ~   .         ;       |
(    ~"-._~"^._\   ^.    ^._      I     . l
 "-._ ___ ~"-,_7    .Z-._   7"   Y      ;  \        _
    /"   "~-(r r  _/_--._~-/    /      /,.--^-._   / Y
    "-._    '"~~~>-._~]>--^---./____,.^~        ^.^  !
        ~--._    '   Y---.                        \./
             ~~--._  l_   )                        \
                   ~-._~~~---._,____..---           \
                       ~----"~       \
                                      \

```

