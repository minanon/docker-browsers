## Build

```bash
docker build -t browsers .
```

## Run

Chromium parameters are for root options. If you run Chromium by general user, you use just '--no-sandbox' parameter.

```bash
docker run --rm -it -e DISPLAY=192.168.0.1:0 browsers firefox
docker run --rm -it -e DISPLAY=192.168.0.1:0 browsers chromium --user-data-dir=/tmp --no-sandbox
docker run --rm -it -e DISPLAY=192.168.0.1:0 browsers phantomjs
```
