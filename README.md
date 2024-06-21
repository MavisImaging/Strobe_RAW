# Strobe Controller Communication

Work undertaken by  [Mavis Imaging GmbH](https://www.mavis-imaging.com/) aims to establish effective communication with strobe controllers via raw commands. This code assists customers in efficiently managing network and user parameters.

## Folders to Use

### StrobeRaw_NetworkP

This code is designed for reading and writing network parameters on a strobe controller (IPSC or HPSC). To use this code:
1. Update the IP addresses of both the computer and the strobe.
2. Write the desired command.
3. Utilize the `SendPacket` function to send it.

### StrobeRaw_UserP

This code is designed for reading and writing user parameters on a strobe controller (IPSC or HPSC). To use this code:
1. Update the IP address with the appropriate IP address of your strobe controller.
2. Write the desired command.
3. Use the functions `sendPacketIPSC` or `sendPacketHPSC` to send it.

### Crc-16

In the `crc-16` folder, you can run the code where you only need to add your payload. It will generate the correct codes to introduce in your raw command.

## About

<img src="images/mavis.png" alt="xLogo" width="700">

For the installation of the ScLib Strobe Controller Configuration Software and Development Kit, visit the [Mavis Imaging Support Tab](https://www.mavis-imaging.com/en/support/). With this installation, you will be able to use the Smartek ScLib API.
