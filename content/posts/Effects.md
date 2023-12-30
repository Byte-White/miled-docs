+++
title = 'Effects'
date = 2023-12-30T13:01:00+02:00
draft = false
+++

### all of the effects are in the `effects` namespace
```cpp

  void sendfadeleds(MiLed& miled,Led color,int del = 50);
  void pushledsrandom(MiLed& miled,int num,int del = 50);
  
  void rainbow(MiLed& miled);
  void rainbowpush(MiLed& miled);
  void rainbowpushchanging(MiLed& miled);

  void gradient(MiLed& miled,Led color1,Led color2);
  void gradientmove(MiLed& miled,Led color1,Led color2);

  void gravity(MiLed& miled,const Led& color,int del = 50);
  void gravitypush(MiLed& miled,const Led& color,int del = 50);

  void firework(MiLed& miled,int del = 25);
```
---
```cpp
  void pushleds(MiLed& miled,
                const Led& color,
                int num,
                int del = 50);
```

_miled_: a reference to the MiLed instance

_color_: color for the animations

_num_: the number of leds being pushed in the animation

_del_: the delay between each push (default value is 50ms)

---

```cpp
  void pushledsrandom(MiLed& miled,
                      int num,
                      int del = 50);
```

_miled_: a reference to the MiLed instance

_num_: the number of leds being pushed in the animation

_del_: the delay between each push (default value is 50ms)

---

```cpp
void rainbow(MiLed& miled);
```

_miled_: a reference to the MiLed instance

---

```cpp
void rainbowpush(MiLed& miled);
```

_miled_: a reference to the MiLed instance

---

```cpp
void rainbowpushchanging(MiLed& miled);
```

_miled_: a reference to the MiLed instance

---

```cpp
void gradient(MiLed& miled,
              Led color1,
              Led color2);
```

_miled_: a reference to the MiLed instance

_color1_: specifies the first color

_color2_: specifies the second color

---

```cpp
void gradientmove(MiLed& miled,
                  Led color1,
                  Led color2);
```

_miled_: a reference to the MiLed instance

_color1_: specifies the first color

_color2_: specifies the second color

---

```cpp
void gravity(MiLed& miled,
             const Led& color,
             int del = 50);
```

_miled_: a reference to the MiLed instance

_color_: specifies the color

_del_: the delay(speed) of the led (default value is 50ms)

---

```cpp
void gravitypush(MiLed& miled,
                 const Led& color,
                 int del = 50);
```

_miled_: a reference to the MiLed instance

_color_: specifies the color

_del_: the delay(speed) of the led (default value is 50ms)

---

```cpp
void firework(MiLed& miled,
              int del = 25);
```

_miled_: a reference to the MiLed instance

_del_: the delay(speed) of the led (default value is 25ms)

---

**Note:** I will probably not describe all of the effects but I will keep the [list at the top](#effects) up to date.