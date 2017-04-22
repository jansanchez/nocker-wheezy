# **nocker-wheezy**

An Image for Node.js based in Debian Wheezy

## Run + bash (temporaly)
```
docker run -it --rm jansanchez/nocker-wheezy bash
```

## How to use

### I'm working in that...

## Run in a "nodejs" container
```
docker run -it --name nodejs jansanchez/nocker-wheezy bash
```

## Add dependency with Yarn
```
docker run -it --name nodejs --rm \
  -u node \
  -v ~/yarn_cache/:/tmp/cache/yarn/ \
  -v app:/home/node/app/ \
  js/nocker-wheezy yarn add css-url-versioner
```

This image of Alpine Linux don't contain bash use sh, ash, /bin/sh or /bin/ash instead
i.e.: `docker run -it --rm image_name /bin/sh`

# **If you want your Own Build**


## Clone repository
```
git clone git@github.com:jansanchez/nocker-wheezy.git
```

## Build
```
docker build -t nocker-wheezy .
```
