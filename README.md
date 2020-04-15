[![relay8-rpi](readmeres/sequent.jpg)](https://www.sequentmicrosystems.com)

# 8relay-rpi

This is the command to control [8-Relay Stackable Card for Raspberry Pi](https://sequentmicrosystems.com/index.php?route=product/product&path=33&product_id=50)

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
