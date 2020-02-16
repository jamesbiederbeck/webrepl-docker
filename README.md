# webrepl-docker
WebREPL client and related tools for MicroPython
Containerized webrepl reused from [micropython/webrepl](https://github.com/micropython/webrepl).
Its license and related files are distributed in the webrepl directory of this repository.

This container is based on the httpd docker image. 

To get started, clone this repository:
>git clone https://github.com/jamesbiederbeck/webrepl-docker.git

Build the image:
>docker build -t  webrepl .

Run the image:
>docker run -p 8266:80 --name webrepl webrepl

Then navigate to http://container-host:8266/webrepl.html
  
Please note that using the webrepl over https is not support due to webrepl's implementation, so it is recommended that you access this continer securely.
