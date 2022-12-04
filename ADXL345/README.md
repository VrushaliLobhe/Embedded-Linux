# ADXL345 Raspberry Pi interface

<h3>Install pip3</h3>

    sudo apt update

    sudo apt install python3-pip

-------------------------------------------------------------------------------------------------------------

<h3>Install adxl345 i2c library</h3>


    sudo pip3 install adafruit-circuitpython-adxl34x

------------------------------------------------------------------------------------------------------------------

<h3>Install adxl345 spi library</h3>


    sudo apt-get update
    git clone https://github.com/nagimov/adxl345spi
    cd adxl345spi
    sudo make
    sudo make install

--------------------------------------------------------------------------------------------

<h3> I2C connections </h3>
  
GND &rarr; GND

VCC &rarr; 3V3

SDA &rarr; SDA

SCL &rarr; SCL

<img src="https://cdn.pimylifeup.com/wp-content/uploads/2019/05/Raspberry-Pi-ADXL345-Accelerometer-Wiring-Schematic.png">

<img src="https://cdn.pimylifeup.com/wp-content/uploads/2019/05/Raspberry-Pi-ADXL345-Accelerometer-GPIO-PIns.png">

------------------------------------------------------------

<h3> SPI connections</h3>

GND &rarr; GND

VCC &rarr; 3V3

CS &rarr; CE0

SDO &rarr; MOSI

SDA &rarr; MISO

SCL &rarr; SCL

<img src="https://raw.githubusercontent.com/nagimov/adxl345spi/master/img/adxl345spi_schem.png">

-----------------------------------------------------------

&copy; 2022, Rohit Akurdekar&trade;
