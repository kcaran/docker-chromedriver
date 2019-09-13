# Chromedriver Docker

A docker container based on the SeleniumHQ Selenium Grid Standalone
- Chrome Debug image, but using only chromedriver and not the entire
Selenium Grid.

https://github.com/SeleniumHQ/docker-selenium

## How to use this image

```
$ docker build -t chromedriver:latest .
$ docker run -d -p 9515:9515 -p 5901:5900 -v /dev/shm:/dev/shm chromedriver/latest
```

The default VNC password is *secret*.
