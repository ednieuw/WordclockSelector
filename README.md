
<h1 class="auto-style3">Word clock selector</h1>
<p>
<a href="https://github.com/ednieuw">
<img alt="Word clocks" longdesc="Word clocks" src="SelectorPics/Wordclock.jpg" ></a></p>
<p>There are several different designs of the word clock. 
There are examples for English, German, French and Dutch designs.<br>In the software it 
is possible to add your own language.
<br> </p>
<p class="auto-style3">All clocks are designed on PCBs (Printed Circuit board). <br>These PCBs are 
designed in Fritzing and available in a Fritzing design format and as Gerber 
file in a ZIP.<br>The zipped Gerber files can be uploaded to a company like 
my supporter 
<a href="PCBWay.com">PCBway that manufactures excellent PCBs with a good service</a>.<br>The Fritzing 
files can be used as a template for your own design. <br>KiCad can also be used 
for creating electronic circuit schematics but there is unfortunately in 2024 
still no translation between the two formats possible.&nbsp; </p>
<p class="auto-style3">All designs communicate with a Bluetooth serial terminal 
on a phone or tablet but also possess a rotary encoder and DS3231 RTC time module to 
set the time and keep the time accurate to 20 seconds a year.<br><br>There are 
several built options for the word clock:</p>
<ul>
	<li>
	<p>An ATMEGA328 chip with shift registers and white 
	LEDs.</p>
	</li>
	<li>
	<p>An Arduino Nano Every/ATMEGA1280 with WS2812 RGB or SK6812 RGBW 
	LED-strips</p>
	</li>
	<li>
	<p>An Arduino Nano ESP32 with WS2812 RGB or SK6812 RGBW 
	LED-strips</p>
	</li>
	<li>
	<p>An Arduino Nano ESP32 with shift registers and white 
	LEDs.<br></p>
	</li>
</ul>

The colourfull Fibonacci Mondriaan clocks are here:<br>
https://github.com/ednieuw/Fibonacci-ESP32-C3-S3-Clock<br>



<p><br></p>
<hr><H2>Pros and Cons</H2>
<hr><br>
<H3><a href="https://github.com/ednieuw/Woordklok-witte-LEDs">ATMEGA328 chip with shift registers and white LEDs.</a></H3>
<p><strong>Pro</strong></p>
<p>Sturdy design that did not had one failure in 40 clocks for over 10 years.</p>
<p>Can run with DCF77 time receiver.</p>
<p><strong>Cons</strong></p>
<p>A lot of soldering. But a advantage if you like soldering.</p>
<p>No WIFI NTP time. <br>(<a href="https://github.com/ednieuw/ESP32SerialNTP-BLE-Clock">By 
replacing&nbsp; the Bluetooth adapter</a> with a ESP32-C3 or S3 Bluetooth and 
WIFI NTP time can be added) </p>
<p>You have to translate the Dutch instructions to your own language or mail me.</p>
<p><br></p>
<hr>
<p>&nbsp;</p>
<H3><a href="https://github.com/ednieuw/Word-Colour-Clock-SK6812-WS2812">Arduino Nano Every with WS2812 RGB or SK6812 RGBW LED-strips</a></H3>
<p><strong>Pro</strong></p>
<p>Uses colour RGB(W) LED-strips</p>
<p>solid design that did not had one failure in 40 clocks for over 5 years.</p>
<p>Easy to solder</p>
<p><strong>Cons</strong></p>
<p>No WIFI NTP time<br>(<a href="https://github.com/ednieuw/ESP32SerialNTP-BLE-Clock">By 
replacing&nbsp; the Bluetooth adapter</a> with a ESP32-C3 or S3 Bluetooth and 
WIFI NTP time can be added) </p>
<p>DCF77 only possible with receiver 10-15cm cm away from the RGB(W) LEDs.</p>
<p>&nbsp;</p>
<hr>
<p>&nbsp;</p>
<H3><a href="https://github.com/ednieuw/Arduino-ESP32-Nano-Wordclock">The Arduino Nano ESP32 with WS2812 RGB or SK6812 RGBW</a> </H3>
	LED-strips is the most versatile. 
<p><strong>Pro</strong></p>
<p>WIFI and BLE in the microprocessor to control the clock from a phone or PC.</p>
<p>NTP time from the internet in combination with the DS3231 RTC module.<br>(It 
is possible to use the clock without internet) </p>
<p>Software runs on ESP32-C3/S3 and many more MCU's without a PCB.<br>Just 
connect the LED-strip and the DS3231 RTC to the pins and the clock will run<br></p>
<p><strong>Cons</strong></p>
<p>None?</p>
<p>&nbsp;</p>
<hr>
<p>&nbsp;</p>
<H3><a href="https://github.com/ednieuw/ESP32ShiftregisterBWclock">An Arduino Nano ESP32 with shift registers and white LEDs.</a></H3>
<p><strong>Pro</strong></p>
<p>WIFI and BLE in the microprocessor to control the clock from a phone or PC</p>
<p>NTP time from the internet in combination with the DS3231 RTC module.<br>(It 
is possible to use the clock without internet) </p>
<p>&nbsp;</p>
<p><strong>Cons</strong></p>
<p>A lot of soldering. But a advantage if you like soldering.</p>
<p>&nbsp;</p>
<span><br><br><br">

</span>
<p>Oct 2024</p>


