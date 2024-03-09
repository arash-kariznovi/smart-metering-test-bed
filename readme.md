smart metering testbed:

The INA219 chip can very precisely measure the voltage drop across the shunt.  This is the difference between the voltage coming into the shunt and the voltage after the shunt.
It then uses this voltage drop along with the value of the resistor shunt to determine the current flow in amps because Ohm’s law states that current (I) = voltage (V) / resistance (R).  With voltage and current it can calculate wattage using power (P) = voltage(V) x current (I). 

Power Supply:

Raspberry Pi 4B: INA219 is connected to the raspberry pi (ARM A72) using I2C protocol and then raspberry pi is sending the metering data every 5 seconds to the Google Cloud(Firebase)

