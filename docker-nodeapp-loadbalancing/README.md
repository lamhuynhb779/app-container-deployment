# Project Title

Docker nodejs haproxy 

---
## Requirements

Install node
Install npm
Install Docker Toolbox or Visual studio code: extension Docker

### Check version

Command:
    $ node --version
    v8.11.3

    $ npm --version
    6.1.0
## Docker Command

    Build image haproxy
        $ docker build -t my-haproxy .
    Test the configuration file
        $ docker run -it --rm --name haproxy-syntax-check my-haproxy haproxy -c -f /usr/local/etc/haproxy/haproxy.cfg

    Build image node
        $ docker build -t nodeapp .

## Docker-compose Command

    $ docker-compose up
    $ docker-compose down
