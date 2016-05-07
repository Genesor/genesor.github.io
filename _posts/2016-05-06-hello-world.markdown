---
layout: post
title: Hello World !
date: 2016-05-06 	20:30:00
comments: true
description: My first words and my first project...
---

## Connecting my Infrared lamps

<hr>

One of my hobby is to connect things. I'm currently owning three types of Phillips Hue lamps, but as you know those lamps are already connected so there is almost no challenge to use them with a web UI or a mobile app.

What I want to do is to "connect" some of my infrared generic lamps to my Raspberry Pi using [LIRC](http://www.lirc.org/){:target="_blank"}{:target="_blank"} and [Go](https://golang.org/){:target="_blank"}. Then I'll be able to interact with the lamps using an API and a Web UI (maybe an iOS app if I'm brave enough)

I'll start by connecting the three following lamps, a multicolor LED bulb and two multicolor table lamps

<div class="img_row">
	<img class="col one" src="/img/01_ampoule_ir.jpg">
	<img class="col one" src="/img/01_lampe_ir.jpeg">
	<img class="col one" src="/img/01_lampe_ir_2.jpg">
</div>

> The three lamps i'm trying to connect

<hr>

#### Schematic:

![IR electronic schematic](/img/01_ir_schematic.png)

> The basic schematic of my IR receiver/emitter available [here](https://123d.circuits.io/circuits/2107586-basic-ir-receiver-emitter-raspberry){:target="_blank"}

I intend to use the GPIO 8 to read the incoming IR signals from the differents sources and the GPIO 1 to send the signals. To do so I only need to have the good LIRC configuration.

<hr>

#### Parts:


* 1 [P2N2222AGOD-ND transistor](https://octopart.com/p2n2222ag-on+semiconductor-55396558){:target="_blank"}
* 1 [10k Ohm resistor](https://octopart.com/od103je-ohmite-133027){:target="_blank"}
* 1 [TSOP38238 38KHz IR receiver](https://octopart.com/tsop38238-vishay-5517697){:target="_blank"}
* 1 [940nm 40deg IR LEDs](https://octopart.com/ir333c-everlight-17677690){:target="_blank"}
* 1 [Raspberry Pi](https://www.raspberrypi.org/products/raspberry-pi-2-model-b/){:target="_blank"}
* 1 [Breadboard](https://octopart.com/gs-830-global+specialties-11900592){:target="_blank"}

<hr>

##### External ressources:

* 123D Circuits Raspberry Pi B+ GPIO - [link](https://123d.circuits.io/components/2107543-raspberry-pi-b){:target="_blank"}
* 123D Circuits Schematic - [link](https://123d.circuits.io/circuits/2107586-basic-ir-receiver-emitter-raspberry){:target="_blank"}
* Golang - [link](http://www.lirc.org/){:target="_blank"}
* LIRC - [link](https://golang.org/){:target="_blank"}