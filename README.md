[![relay8-rpi](readmeres/sequent.jpg)](https://www.sequentmicrosystems.com)

# 8relay-rpi

This is the command line and python functions to control the Sequent Microsystems 8 Relay Card for Raspberry PI Ver. 3. If you have Ver. 1-2 with screw-type connectors download from   
https://github.com/SequentMicrosystems/relay8-rpi

Don't forget to enable I2C communication:
```bash
~$ sudo raspi-config
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
