Welcome to the W6100EVB-TLS wiki!

# How to make certificate.
## make ca.crt and ca.key file.
<p align="center">
  <img width="90%" src="Certificate01.png" />
</p>

## make server.key file.
<p align="center">
  <img width="90%" src="Certificate02.png" />
</p>

## make server.csr file.
<p align="center">
  <img width="90%" src="Certificate03.png" />
</p>

## make ca.srl and server.crt file.
<p align="center">
  <img width="90%" src="Certificate04.png" />
</p>

## make cerificate.h
 - Please server.crt file transporates to header format.
<p align="center">
  <img width="90%" src="Certificate05.png" />
</p>

# How to modity program.
## Program setting.
 - change server ip and device ip.

# Result
## open server(openssl s_server)
 - build project and excute program.
<p align="center">
  <img width="90%" src="result01.png" />
</p>

## mesage loop back test
 - if end masage send, connect closed.
<p align="center">
  <img width="90%" src="result02.png" />
</p>