[![relay8-rpi](readmeres/sequent.jpg)](https://www.sequentmicrosystems.com)

# 8relay-rpi

[![relay8-rpi](readmeres/8-RELAYS.jpg)](https://www.sequentmicrosystems.com)

This is the command line and python functions to control the [8-RELAYS Stackable Card for Raspberry Pi](https://sequentmicrosystems.com/collections/all-products/products/raspberry-pi-relays-stackable-card) Ver. 3. If you have Ver. 1-2 with screw-type connectors download from [here](https://github.com/SequentMicrosystems/relay8-rpi).

Don't forget to enable I2C communication:
```bash
~$ sudo raspi-config
```
A good article about I2C on Raspberry can be found [here.](https://www.raspberrypi-spy.co.uk/2014/11/enabling-the-i2c-interface-on-the-raspberry-pi/) 

If you use Ubuntu you need to install ```bash raspi-config ``` first:

```bash
~$ sudo apt update
~$ sudo apt install raspi-config
```

## Usage

```bash

~$ git clone https://github.com/SequentMicrosystems/8relay-rpi.git
~$ cd 8relay-rpi/
~/8relay-rpi$ sudo make install
```

Now you can access all the functions of the relays board through the command "8relay". Use -h option for help:
```bash
~$ 8relay -h
```

If you clone the repository any update can be made with the following commands:

```bash
~$ cd 8relay-rpi/  
~/8relay-rpi$ git pull
~/8relay-rpi$ sudo make install
```  

### [Python library](https://github.com/SequentMicrosystems/8relay-rpi/tree/master/python)

### [Node-Red example based on "exec" node](https://github.com/SequentMicrosystems/8relay-rpi/tree/master/node-red)

### [Node-Red "8relay" node](https://github.com/SequentMicrosystems/8relay-rpi/tree/master/node-red-contrib-sm-8relay)

### [Arduino Library](https://github.com/SequentMicrosystems/8relay-arduino)
