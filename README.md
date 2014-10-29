# Golden Gate Assembly Tool

[![Build Status](https://travis-ci.org/wookoouk/GoldenGate.svg)](https://travis-ci.org/wookoouk/GoldenGate)

<img src="https://raw.githubusercontent.com/wookoouk/GoldenGate/master/public/gate2.png">

>A tool for SynBio

Golden Gate is a tool developed by Martin Page of [Team Maclean](http://danmaclean.info) for SynBio of [The Sainsbury Laboratory](http://tsl.ac.uk).
The tool was designed to work with the data found [here](https://github.com/TSLSynBio/Golden-Gate-Data/)  but can work with any data that follows the same annotation style.

## Install
Depends on:
* Perl
  * "5.20"
  * "5.18"
  * "5.16"
  * "5.14"
  * "5.12"
  * "5.10"
* NodeJS
* MongoDB

Install Bower
```sh
$ npm install -f bower
```

Install Perl modules
```sh
$ curl -L cpanmin.us | perl - -n Mojolicious
$ curl -L cpanmin.us | perl - -n Mango
$ curl -L cpanmin.us | perl - -n Data::Printer
$ curl -L cpanmin.us | perl - -n JSON
$ curl -L cpanmin.us | perl - -n Bio::SeqIO
```

Install web components
```sh
$ bower install
```

Checkout data
```sh
$ cd data
$ git clone https://github.com/TSLSynBio/Golden-Gate-Data.git
```

Start the app
```sh
$ perl goldengate.pl daemon -m production
```

## Docker
To test the app via docker
```sh
$ docker pull wookoouk/goldengate
$ sudo docker run --name goldengate -d wookoouk/goldengate
```
[More info about this Docker container](https://registry.hub.docker.com/u/wookoouk/goldengate/)

