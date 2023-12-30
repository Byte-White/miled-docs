+++
title = 'Getting Started'
date = 2023-12-30T13:01:48+02:00
draft = false
+++

## Installing the library

1. Copy [Miled](https://github.com/Byte-White/MiLed) library into your Arduino libraries directory.
2. Include MiLed in Your Sketch
3. Write code

### Example code for making the first led blink in red 

```cpp
#include <MiLed.h>

#define DATA_PIN  11
#define LED_COUNT  8

MiLed ml(DATA_PIN,LED_COUNT);

void setup()
{

}

void loop()
{
    ml[0] = Led(30,0,0);
    ml.show();
    delay(500);
    ml[0] = Led(0);
    ml.show();
    delay(500);
}
```

### Example code showing some of the effects

```cpp
#include <MiLed.h>

#define DATA_PIN  11
#define LED_COUNT  8

MiLed ml(DATA_PIN,LED_COUNT);

void setup()
{

}

void loop()
{
    effects::gravitypush(ml, Led(30,0,0),35);
    effects::sendfadeleds(ml,Led(70));
    effects::firework(ml);
}
```