# Index
- [TLS Client Example for W6100-EVB](#TLS-Client-Example-for-W6100-EVB)
- [Hardware Environment](#Hardware-Environment)
- [Software Environments](#Software-Environment)
- [Run](#Run)
- [Code review](#Code-review)
  - [Test packet capture file](#Test-packet-capture-file)



------
# TLS Client Example for W6100-EVB
Common to Any MCU, Easy to Add-on. Internet Offload co-Processor, HW TCP/IP chip,
best fits for low-end Non-OS devices connecting to Ethernet for the Internet of Things. These will be updated continuously.

## Hardware Environment
* W6100EVB
  - connecting Micro usb.
  - connecting Ethernet cable. <br>
<p align="center">
  <img width="60%" src="https://docs.wiznet.io/assets/images/w6100-evb_callout-d5d88d99555cd8b78d6a8327b849cd58.png" />
</p>

## Software Environment
In case of used to TrueSTUDIO, It is the same as HTTP Server example.
 - Link : [Software Environment of W6100EVB-HTTP_Server](https://github.com/WIZnet-ioLibrary/W6100EVB-HTTP_Server#Software-Environment)

 ### How to make certificate. <br>
 - make ca.crt and ca.key file.
<p align="center">
  <img width="90%" src="https://github.com/WIZnet-ioLibrary/W6100EVB-TLS/wiki/Certificate01.png" />
</p>

 - make server.key file.
 <p align="center">
  <img width="90%" src="https://github.com/WIZnet-ioLibrary/W6100EVB-TLS/wiki/Certificate02.png" />
 </p>

- make server.csr file.
<p align="center">
  <img width="90%" src="https://github.com/WIZnet-ioLibrary/W6100EVB-TLS/wiki/Certificate03.png" />
</p>

- make ca.srl and server.crt file.
<p align="center">
  <img width="90%" src="https://github.com/WIZnet-ioLibrary/W6100EVB-TLS/wiki/Certificate04.png" />
</p>

- make cerificate.h
  - Please server.crt file transporates to header format.
<p align="center">
  <img width="90%" src="https://github.com/WIZnet-ioLibrary/W6100EVB-TLS/wiki/Certificate05.png" />
</p>

### Program setting.
- change server ip and device ip.
<p align="center">
  <img width="90%" src="https://github.com/WIZnet-ioLibrary/W6100EVB-TLS/wiki/ipset.png" />
</p>

## Run
* Demo Environment & Program <br>

  - Windows 10 <br>
  - Internet Explorer <br>
  - Hercules <br>


* Demo Result <br>
  - Power On and push Reset button to start Program<br>
  - Program Run Serial display <br>
  - open server(openssl s_server)
    - build project and excute program.
<p align="center">
  <img width="90%" src="https://github.com/WIZnet-ioLibrary/W6100EVB-TLS/wiki/result01.png" />
</p>

  - mesage loop back test
    - if end masage send, connect closed.
<p align="center">
  <img width="90%" src="https://github.com/WIZnet-ioLibrary/W6100EVB-TLS/wiki/result02.png" />
</p>

## Code review
- main.c code flow
<p align="center">
  <img width="50%" src="https://github.com/WIZnet-ioLibrary/W6100EVB-TLS/wiki/W6100EVB-TLS-FlowChart.png" />
</p>

## Test packet capture file
<p align="center">
  <img width="90%" src="https://github.com/WIZnet-ioLibrary/W6100EVB-TLS/wiki/packet_capture.png" />
</p>

- Test packet capture file : [W6100EVB-TLS-packet.zip](https://github.com/WIZnet-ioLibrary/W6100EVB-TLS/wiki/W6100EVB-TLS-packet.zip)
