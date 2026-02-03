---
title: "Irregular Countdown Calendar"
subtitle: "Arduino project to divide life into segments of irregular length"
slug: "irregular-countdown-calendar"
description: |
  I realized that my life needs a balance between regularity and irregularity.
  Weeks and months provide regularity and to have an element of irregularity I have created an Arduino project to show the number of days remaining until my age in days (not y...
date: 2024-06-18
updated: 2025-08-23
status:
  - published
tags:
  - arduino
  - calendar
reading_time: 5
cover_image: "/assets/img/blog/2024-06-18-irregular-countdown-calendar/cover.jpeg"
---
I realized that my life needs a balance between regularity and irregularity.

Weeks and months provide regularity and to have an element of irregularity I have created an Arduino project to show the number of days remaining until my age in days (not years) is a prime number.

Since prime numbers appear at irregular intervals, this will divide my life into segeents of irregular length.

On irregular days I might perform irrational activities such as gambling, praying, dancing or arguing.

The number of days remaing is displayed as a [Matula Tree](https://keithbriggs.info/matula.html). These characters are stored in PROGMEM.

On days where my age is a prime number (an irregular day) the screen will twinkle.

Currently my age in days is around 16000~17000 and primes appear on average every 8 days. A maximal prime gap will appear in ~10 years and will be 44 days long.

To calculate the next prime (until i'm ~100 years old) its only necessary to test numbers for divisibility by the first ~50 primes.

{% include youtube.html id="58BC__LPfAE" title="irregular countdown calendar 1" %}

{% include youtube.html id="UfQskl_oUsU" title="irregular countdown calendar 2" %}

# Components used

* Arduino Nano
    
* RTC DS1307 Clock module
    
* Mod4 Max7219 8x32LED Matrix

# Libraries used

[Chronos Library](https://inductive-kickback.com/projects/chronos/) to calculate number of elapsed days.

# Serial I/O

Connect to phone [Serial USB Terminal](https://play.google.com/store/apps/details?id=de.kai_morich.serial_usb_terminal)

output: current date, days until next prime

input: new current date (RTC does not support time zones)

# Planned improvements

* To resemble pendulum clock, use a sine wave to swing the number across the display rather than bouncing it.
    
* To make the clock seem more lively on prime days, use a sine wave to gradually increase and decrease amount of twinkles every 4 seconds.
    
* Use EEPROM to store led intensity level.
    
* Use EEPROM to store start date.
    
* Perhaps use the parola's font mechanism to store the numbers.
    
* Count down to even more irregular twin primes.

[https://github.com/arnodenhond/IrregularClock](https://github.com/arnodenhond/IrregularClock)
