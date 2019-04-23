# dht11-22-temperature-humidity-sensor-on-Raspberry-pi
dht11/22 temperature humidity sensor on Raspberry pi (based on pigpio)

It is a tool to fetch the DHT11/22(1-wire protocol).


1. select the available GPIO port and connect DHT11/22 (signal pin) with it. 
https://www.raspberrypi-spy.co.uk/2012/06/simple-guide-to-the-rpi-gpio-header-and-pins/

2. Compile it by gcc.
gcc -Wall -pthread -o dhtxx2 dhtxx2.c -lpigpio -lrt

3. Run the tool with sudo & assign a port number.
sudo ./dhtxx2 port


If you want to know more about 1-wire protocol, you can google more about it.
https://www.rototron.info/wp-content/uploads/DHT22_Datasheet.pdf

It is based on the pigpio library. Refer below link.
https://github.com/joan2937/pigpio
