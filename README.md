## Beaglebone Temperature Logger

This is a bit of python code that uses the
[Adafruit Python IO library](https://github.com/adafruit/adafruit-beaglebone-io-python)
to read the temperature and pressure from
[TMP102]http://www.ti.com/product/tmp102)( (temperature) and
[BMP085](http://www.bosch-sensortec.com/en/homepage/products_3/environmental_sensors_1/bmp085_1/bmp085)
(Pressure) I2C sensors. Both sensors were purchased assembled from
[Sparkfun](http://www.sparkfun.com). They're a good company!



### Things I used in putting this together The Adafruit team has done
a really nice job in putting together the IO library which includes
the I2C module.

I was able to (more or less) implement the code to read the sensors
directly from Adafruit examples. The development time for this was on
the order of a few hours.

I'm using the Xively API right now to push the data somewhere and save
it in the cloud. They've changed their business model significantly
from the Pachube days and are more B2B oriented at the moment. I think
I'm going to migrate this to some sqlite solution soon.

The code was originally developed in an IPython notebook and then
saved as a python file using their nbconvert tool. This makes it nice
and easy to step through blocks of code to see what's working and what
isn't.
