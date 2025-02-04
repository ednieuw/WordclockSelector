
<h1 class="auto-style3">Word clock and Fibonacci clock selector</h1>

<img alt="Word clocks" longdesc="Word clocks" src="SelectorPics/Wordclock.jpg" ></a>
There are three different designs of the word clock built with a:
- a bare ATMEGA328 chip and white LEDs<br>
- an Arduino Nano Every <br> 
- an Arduino Nano ESP32.<br>

The last two supports WS2812 RGB and SK6812 RGBW LEDs.<br>

The software of all clocks supports a Bluetooth connection to control the clock and as backup a rotary encoder, an accurate DS3231 RTC and a LDR light intensity detector.<br>

The Nano ESP32 designs supports a web page and WIFI/NTP time.

This page gives an overview and the pros and cons of the possibilities.<br>

With some spare RGB(W) LED-strip a Fibonnaci clock can be made.<br>
This Fibonacci clock displays time with three colours and looks like a constantly changing painting from the Dutch painter Mondriaan.<br>
The colourfull [Fibonacci Mondriaan clocks are here for an ESP32-C3 and S3](https://github.com/ednieuw/Fibonacci-ESP32-C3-S3-Clock)
or [here for a Arduino Nano](https://github.com/ednieuw/Fibonacci-Vierkantekokerklok) with a 3D-printer design for the stick version.<br>

And finally the latest Fibonacci-clock designs for the [Arduino Nano ESP32](https://github.com/ednieuw/Fibonacci-Nano-ESP32-clock). 

The first designs of the word clock are are over 10 years in operation. They have a clock face with a 11 x 11 character grid.<br>
These clocks uses white 2835/3528 LED-strips, an ATMEGA328 and use shift registers to turn on and off LED-strips.<br>
Later designs were made with WS2812 RGB and SK6812 RGBW LED strips and an Arduino Nano.<br>
These clocks are 30 x 30 cm.

The four-language clock uses a 25 x 25 character grid. 
Because the French language front plate could only be designed in a 12 x 12 character grid the other single language character faces were redesigned and some words added.<br>

These 12 x 12 character grid clocks are operated with the Arduino Nano Every or a ATMEGA1280 chip and use SK6812 or WS2812 LED-strips to light the characters.<br>
These clocks have in my designs a standard size of 25 x 25 cm or 50 x 50 cm.  

In 2023 the Arduino Nano ESP32 with onboard WIFI and BLE functionality became available. The latest designs use this microprocessor. 

The software sketches contains coding to display four languages; English, German, French and Dutch.<br>

[All clocks are designed on PCBs (Printed Circuit Board)](https://github.com/ednieuw/NanoESP32PCB). <br>
These PCBs are designed in Fritzing and available in a Fritzing design format and as Gerber file in a ZIP.
	
The zipped Gerber files can be uploaded to a company like my supporter [PCBway](https://PCBWay.com) that manufactures excellent PCBs with a good service.<br>
The Fritzing files can be used as a template for your own design.<br>
KiCad can also be used for creating electronic circuit schematics but there is unfortunately in 2024 still no translation between the two formats possible.</p>

All designs communicate with a Bluetooth serial terminal app on a phone or tablet but also includes a rotary encoder and DS3231 RTC time module to set the time and keep the time accurate to 20 seconds a year.<br><br>
There are several built options for the word clock:
<ul>
	<li>
	<p>An ATMEGA328 chip with shift registers and white LEDs.</p>
	</li>
	<li>
	<p>An Arduino Nano Every/ATMEGA1280 with WS2812 RGB or SK6812 RGBW LED-strips</p>
	</li>
	<li>
	<p>An Arduino Nano ESP32 with WS2812 RGB or SK6812 RGBW	LED-strips</p>
	</li>
	<li>
	<p>An Arduino Nano ESP32 with shift registers and white	LED-strips.</p>
	</li>
	<li>
	<p>A combination of all on one PCB the Ultimate Arduino Nano ESP32 with shift registers and white LEDs and with WS2812 RGB or SK6812 RGBW.</p>
	</li>
</ul>
<hr><H2>Pros and Cons of the different clock designs</H2>
<hr>
<a href="https://github.com/ednieuw/Woordklok-witte-LEDs">ATMEGA328 chip with shift registers and white LEDs.</a>
<br><br>
<p><strong>Pro</strong></p>
<p>Sturdy design that did not had one failure in 40 clocks for over 10 years.</p>
<p>Can run with DCF77 time receiver.</p>
<p><strong>Cons</strong></p>
<p>A lot of soldering. But a advantage if you like soldering.</p>
<p>No WIFI NTP time. <br>(<a href="https://github.com/ednieuw/ESP32SerialNTP-BLE-Clock">
By replacing the Bluetooth adapter with a ESP32-C3 or S3 Bluetooth and WIFI NTP time can be added)

You have to translate the Dutch instructions to your own language or mail me.

<hr>
<a href="https://github.com/ednieuw/Word-Colour-Clock-SK6812-WS2812">Arduino Nano Every with WS2812 RGB or SK6812 RGBW LED-strips</a>
<br><br>
<p><strong>Pro</strong></p>
<p>Uses colour RGB(W) LED-strips</p>
<p>Solid design that did not had one failure in 40 clocks for over 5 years.</p>
<p>Easy to solder</p>
<p><strong>Cons</strong></p>
<p>No WIFI NTP time<br>(<a href="https://github.com/ednieuw/ESP32SerialNTP-BLE-Clock">By 
replacing&nbsp; the Bluetooth adapter</a> with a ESP32-C3 or S3 Bluetooth and 
WIFI NTP time can be added) </p>
<p>DCF77 only possible with receiver 10-15cm cm away from the RGB(W) LEDs.</p>
<p>&nbsp;</p>
<hr>

<a href="https://github.com/ednieuw/Arduino-ESP32-Nano-Wordclock">The Arduino Nano ESP32 with WS2812 RGB or SK6812 RGBW</a> 
<br><br>
<p><strong>Pro</strong></p>
<p>WIFI and BLE in the microprocessor to control the clock from a phone or PC.</p>
<p>NTP time from the internet in combination with the DS3231 RTC module.<br>(It 
is possible to use the clock without internet) </p>
<p>Software runs on ESP32-C3/S3 and many more MCU's without a PCB.<br>
Just connect the LED-strip and the DS3231 RTC to the pins and the clock will run<br></p>
<p><strong>Cons</strong></p>
<p>None?</p>

<hr>

<a href="https://github.com/ednieuw/ESP32ShiftregisterBWclock">An Arduino Nano ESP32 with shift registers and white LEDs.</a>
<br><br>
<p><strong>Pro</strong></p>
<p>WIFI and BLE in the microprocessor to control the clock from a phone or PC</p>
<p>NTP time from the internet in combination with the DS3231 RTC module.<br>(It is possible to use the clock without internet) </p>
<p>&nbsp;</p>
<p><strong>Cons</strong></p>
<p>A lot of soldering. But an advantage if you like soldering.</p>

<hr>

<a href="https://github.com/ednieuw/NanoESP32-BW-RGBW-clock">A combination of all on one PCB the Ultimate Arduino Nano ESP32 with shift registers and white LEDs and with WS2812 RGB or SK6812 RGBW.</a>
<br><br>
<p><strong>Pro</strong></p>
<p>WIFI and BLE in the microprocessor to control the clock from a phone or PC</p>
<p>NTP time from the internet in combination with the DS3231 RTC module.<br>(It is possible to use the clock without internet) </p>
<p>One PCB with all possibilities of above designs.</p>
<p>&nbsp;</p>
<p><strong>Cons</strong></p>
<p>A lot of soldering.</p>
---
<p>Oct 2024</p>


