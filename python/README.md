
[![8relay-rpi](res/sequent.jpg)](https://sequentmicrosystems.com/index.php?route=product/product&path=33&product_id=50)

# lib8relay

This is the python library to control the [8relay](https://sequentmicrosystems.com/index.php?route=product/product&path=33&product_id=50) 8-Relay Stackable Card for Raspberry Pi.

## Install

```bash
~$ sudo apt-get update
~$ sudo apt-get install build-essential python-pip python-dev python-smbus git
~$ git clone https://github.com/SequentMicrosystems/8relay-rpi.git
~$ cd 8relay-rpi/python/8relay/
~/8relay-rpi/python/8relay$ sudo python setup.py install
```
## Update

```bash
~$ cd 8relay-rpi/
~/8relay-rpi$ git pull
~$ cd 8relay-rpi/python/8relay/
~/8relay-rpi/python/8relay$ sudo python setup.py install
```

## Usage 

Now you can import the megaio library and use its functions. To test, read relays status from the board with stack level 0:

```bash
~$ python
Python 2.7.9 (default, Sep 17 2016, 20:26:04)
[GCC 4.9.2] on linux2
Type "help", "copyright", "credits" or "license" for more information.
>>> import lib8relay
>>> lib8relay.get_all(0)
0
>>>
```

## Functions

### set(stack, relay, value)
Set one relay state.

stack - stack level of the 8-Relay card (selectable from address jumpers [0..7])

relay - relay number (id) [1..8]

value - relay state 1: turn ON, 0: turn OFF[0..1]


### set_all(stack, value)
Set all relays state.

stack - stack level of the 8-Relay card (selectable from address jumpers [0..7])

value - 4 bit value of all relays (ex: 15: turn on all relays, 0: turn off all relays, 1:turn on relay #1 and off the rest)

### get(stack, relay)
Get one relay state.

stack - stack level of the 8-Relay card (selectable from address jumpers [0..7])

relay - relay number (id) [1..8]

return 0 == relay off; 1 - relay on

### get_all(stack)
Return the state of all relays.

stack - stack level of the 8-Relay card (selectable from address jumpers [0..7])

return - [0..255]

