## Adafruit bq25185 USB / DC / Solar Charger with 3.3V Buck Board PCB

<a href="http://www.adafruit.com/products/6092"><img src="assets/6092.jpg?raw=true" width="500px"><br/>
Click here to purchase one from the Adafruit shop</a>

PCB files for the Adafruit bq25185 USB / DC / Solar Charger with 3.3V Buck Board. 

Format is EagleCAD schematic and board layout
* https://www.adafruit.com/product/6092

### Description

We're always on the look out for better ways to make projects portable: being able to charge your battery in the most convenient manner will let projects run no matter what power is available. Then we added a power supply chip with it to let you run your project without a separate board. The result is the Adafruit bq25185 USB / DC / Solar Charger with 3.3V Buck Board!

It uses the new bq25185 is a nifty charger chip with fairly high charge current, power path support, and the ability to charge from USB, DC or solar power. It's also a great value, so it's a good upgrade from MCP73833 or MCP73831-based charger boards. The buck converter is the TPS62569, which will give a clean 1 Amp output with good efficiency, to squeeze the most power possible out of your battery.

This board is meant to be everything you need to power your 3.3V electronics: simply connect a 500mAh or larger battery to the JST PH 2-pin port, then charge it when you can from USB or DC/solar. At the other end is a terminal block which will provide the power-path-load output from the bq25185 which will range from 3.0V (battery near-dead) to 4.5V (USB/DC/Solar is powering the board) at about 1 Amp max. Another terminal port will give 3.3V output, up to 1 A (this will also dip down to 3.0V when the battery is near-empty)

* USB Type C connector with 5.1k CC resistors so it will work with any computer or power supply to get 5V and up to 1A. Data lines available if needed, on the bottom breakout.
* Separate DC or Solar Input - Two pads on the edge can be used to connect a 5 ~ 18V power supply, which can be used instead of USB. If the input is a solar panel, the charging chip will adjust the current draw so that the voltage does not dip below the battery, thus optimizing the solar power input. No large capacitor needed to stabilize it, and you get near-MPPT capability without the cost and complexity of MPPT.
* Default charge rate of 1A, but you can cut the jumper on the back to set the rate to 500mA
* Power Path to Load - If the 4.5V or 3.3V load connector is drawing current while the USB / DC/Solar power is attached, it will default to drawing current from the charger and any left over current will go to the battery. That keeps your battery from constantly charging/discharging which will reduce the battery life.
* Regulated 4.5V-max Output - no matter what voltage you have on the USB or DC / solar inputs, the 4.5V terminal block output port will never go above 4.5V due to an internal voltage regulator. Keep this in mind, though, when dealing with high currents and high DC voltages as the LDO will make the board start to overheat and throttle the current.
* Regulated 3.3V-max Output - a seperate buck converter will take the load output from the bq25185 and switch it down to 3.3V at 1 Amp max load
* Three Status LEDs - Orange Charging LED, red Fault LED, and Green 3.3V output LED.
* Enable pad - to disable the 3.3V buck converter.
* Mounting holes!

This board is pretty much plug-and-play. Change the charging jumper if you like, then connect your battery to the BATT port, and the 4.5V-max and 3.3V-max outputs go to your circuit. Don't forget the two outputs  will never go above 4.5V or 3.3V, but it can go as low as 3.0V if the battery is nearly empty. You can monitor the voltage on the battery via the secondary pads on the bottom edge, if necessary.

To use with solar, pick up a 5~7V solar panel (using a higher voltage panel will only lose the extra voltage as heat so there's no benefit to going over 7V), and either cut the connector off to wire it directly, or use a 2.1mm adapter cable plus a 2.1mm terminal block to get two wires for the DC Input port.

If you need a board with higher charge current or a DC plug already on-board, check out the bq24074 which has up to 1.5A charge rate and a on-board 2.1mm DC jack. It doesn't have a buck converter but you could wire up the TPS62569 separately

### License

Adafruit invests time and resources providing this open source design, please support Adafruit and open-source hardware by purchasing products from [Adafruit](https://www.adafruit.com)!

Designed by Limor Fried/Ladyada for Adafruit Industries.

Creative Commons Attribution/Share-Alike, all text above must be included in any redistribution. 
See license.txt for additional details.
