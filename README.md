# The Things Network: RisingHF gateway

Reference setup for [The Things Network](http://thethingsnetwork.org/) gateways based on the RisingHF SPI concentrator with a Raspberry Pi host.

## Setup

Check [a step-by-step HOWTO in our wiki](https://github.com/ttn-zh/ic880a-gateway/wiki) for a detailed explanation of the hardware that needs to be purchased and the software setup you will have to configure. 

## Installation

- Make sure to stop Loriot GW-Server services
        $ sudo update-rc.d loriot-gw remove

- Clone the installer and start the installation

        $ git clone https://github.com/ttn-zh/ic880a-gateway.git ~/ic880a-gateway
        $ cd ~/ic880a-gateway
        $ git checkout risinghf
        $ sudo ./install.sh

## Update

If you have a running gateway and want to update, simply run the installer again:

        $ cd ~/ic880a-gateway
        $ sudo ./install.sh

# Credits

These scripts are largely based on the awesome work by [Ruud Vlaming](https://github.com/devlaam) on the [Lorank8 installer](https://github.com/Ideetron/Lorank).
