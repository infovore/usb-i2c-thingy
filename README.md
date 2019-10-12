# usb-i2c-thingy

An I2C dongle designed to interface devices like [monome norns][norns] with 3.3V i2c.

3.5mm stereo jack uses _tip_ for `SDA` and _ring_ for `SCL`.

Take a [digispark][digispark]; replace the usb tab with a micro-usb socket; add a 3.5mm jack for I2C connection; add I2C level shifting as per [this datasheet][level-shifting]. Add its own 3.3V regulator for the level-shfiting.

You can then flash this pseudo-digispark with the [I2C-Tiny-USB firmware][i2ctiny], which is supported by the Linux kernel.

## STATE

nowhere near finished don't even think about using it.

## TODO

- ~~replace 402 parts with 603~~
- ~~connect SDA/SCL to pins~~
- break out programming header?
- caps for 3.3V regulator?

## LICENSE

CC-BY-SA; digispark accredition to be supplied in fullness of time



[digispark]: http://digistump.com/products/1
[norns]: https://monome.org/norns
[i2ctiny]: https://github.com/harbaum/I2C-Tiny-USB/blob/master/digispark/README.md
[level-shifting]: https://www.nxp.com/docs/en/application-note/AN10441.pdf