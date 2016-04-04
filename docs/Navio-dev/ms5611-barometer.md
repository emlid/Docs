**MS5611 example**

If you haven't already done that, download Navio drivers and examples code [here](navio-repository-cloning/).


***C++***

Move to the folder with the source code, compile and run the example:

```bash
cd C++/Examples/Barometer
make
./Barometer
```

***Python***

Move to the folder with the code and run the example:

```bash
cd Python
python Barometer.py
```

You should see pressure and temperature values. Keep in mind that board tends to get hot from Raspberry and would show slightly higher temperature than it is in your room.

```bash
Temperature(C): 34.3509172821 Pressure(millibar): 1030.4646104
Temperature(C): 34.2971904755 Pressure(millibar): 1030.4639519
Temperature(C): 34.2795449066 Pressure(millibar): 1030.45554448
Temperature(C): 34.3018652344 Pressure(millibar): 1030.46921925
```


For further information see source code, which is mostly self-explanatory. As it takes some time for the sensor to perform conversion delays are added between calls to methods that start the conversion and read the resulting data. After reading both pressure and temperature values temperature compensation can be performed to get resulting pressure value. 

More information about MS5611 is available in the [datasheet](http://files.emlid.com/MS5611-01BA03.pdf)
