# Projects Built on Resin.io

## Installing a Project

To install a project you will need a [Resin.io][resin] account with an
application set up ready to receive code. See the
[getting started][getting-started] and [deployment][deploy] guides for details
on how to do this.

To deploy a project simply clone it and push it to your application's `resin`
endpoint. E.g. for the [Text to Speech Converter project][text2speech]:-

```
git clone https://github.com/resin-io/text2speech.git .
git remote add resin [endpoint]
git push resin master
```

## Projects

### Node.js Starter Project
[Repository][simple-nodejs]

This is a simple Hello, World project for [node.js][node] designed to act as a
basis for future work. It demonstrates how to install native Linux packages and
configure your application.

### Analog-to-digital converter
[Repository][ADC_py] by [Shaun Mulligan][shaun-mulligan]

This is a simple project so show to read analog sensor values into the raspberry pi using python. It uses the [ADS1x15][ADC_adafruit] family of I2C analog-to-digital converters to read in analog signals between 0 and 3.3V.

### resin-tether
[Repository][resin-tether] by [petrosagg][petrosagg]

This python project allows you to share your ethernet connection to wifi. It essentially allows the raspberry pi to act as a wifi access point.

### Digital Temperature Logger
[Repository][firebase-dtl] by [Shaun Mulligan][shaun-mulligan]

A [Firebase][firebase]-backed Digital Temperature Logger allowing you to connect
devices with multiple temperature sensors to a central cloud-based datastore.

### resin-samba
[Repository][resin-samba] by [Aleksis Brezas][aleksis]

Sets up a samba share that you can use to send and receive files to your Raspberry Pi. You can use this project as a template to add file sharing capabilities to your projects.

### Digitiser
[Repository][digitiser] by [Shaun Mulligan][shaun-mulligan]

A tool for displaying integer values from a JSON endpoint on a MAX7219 7-segment
display.

### Deployment guide for DockerHub images
[Repository][dockerHub] by [nghiant2710][nghiant2710]

Resin.io offers you the flexibility to deploy your application from a custom Dockerfile which allows you to define your own development environment.

Freely constructing the environment gives you all the power but sometimes takes a lot of time to create a proper Dockerfile for your application. Why not save your effort by utilising existing Docker images instead of building from scratch, Resin.io allows you to use Docker image from Docker Hub which contains many repos of pre-built Docker image.

### Example Pi Pins Application
[Repository][example-pi-pins] by [Shaun Mulligan][shaun-mulligan]

A simple application which demonstrates the use of the [Pi Pins][pi-pins]
library to interface with [GPIO][gpio].

### Google Coder

[Repository][coder-fork]

Resin.io-enabled version of Google's excellent [Coder][coder] project which
makes it easy to develop web projects on your device.

### Hoversnap

[Repository][hoversnap]

A tool for controlling a camera using a foot switch in order to capture shots in
which people appear to be flying.

### Pi Miner

[Repository][rpiminer] by [Chris Continanza][csquared]

A [bitcoin][bitcoin] miner for the [Raspberry Pi][rpi].

### Resin CCTV

[Repository][resin-cctv] by [Aleksis Brezas][aleksis]

A project which allows you to use your devices as a CCTV camera system which
hooks into [Dropbox][dropbox].

### Resin Player

[Repository][resin-player] by [Praneeth Bodduluri][lifeeth]

A project which allows you to play [squeezebox][squeezebox] media through your
devices.

### Salesforce Temperature Probe

[Repository][salesforce-temp] by [Shaun Mulligan][shaun-mulligan]

Example application for interfacing with a temperature probe using
[Salesforce.com][salesforce].

### SMS to Speech

[Repository][sms2speech] by [Alexandros Marinos][alex]

A simple tool which uses [Twillio][twillio] to read out incoming SMS messages.

### Simple Digitiser Kiosk

[Repository][digitiser-kiosk] by [Praneeth Bodduluri][lifeeth]

Displays values from a JSON endpoint on your browser in kiosk mode (based on
[this blogpost][kiosk-post].)

### Text to Speech Converter

[Repository][text2speech]

A simple application that makes your device speak out loud.

### Cimon
[Repository][cimon] by [efwe][efwe]

A simple tool for reading temperatures from a USB-enabled thermometer. This
project is used as the backend to [efwe][efwe]'s awesome temperature
visualisation at [123k.de](http://123k.de).

## Programming Language Starter Projects

Below is a list of simple 'Hello, World' projects written in a number of
different programming languages, which are designed to form the basis of your
own projects written in each language.

The projects use [Dockerfile][dockerfile]s to install packages and configure the
local environment as needed for each language. This step is performed on the
Resin.io build server and the finished product is pushed to your devices.

A link is provided for each project's individual Dockerfile below for easy
customisation:-

### C♯

[Repository][hello-dotnet]

Hello World written in [C#][csharp] using a
[custom Dockerfile][csharp-dockerfile].

__NOTE:__ This project can be adapted to target any [.net][dotnet]
language.

### Java

[Repository][hello-java]

Hello World written in [Java][java] using a
[custom Dockerfile][java-dockerfile].

__NOTE:__ This project can be adapted to target any [JVM][jvm] language.

### Python

[Repository][hello-python]

Hello World written in [Python][python] using a [custom Dockerfile][python-dockerfile].

### Ruby

[Repository][hello-ruby]

Hello World written in [Ruby][ruby] using a [custom Dockerfile][ruby-dockerfile].

[resin]:https://resin.io
[dropbox]:https://www.dropbox.com/

[deploy]:/pages/deployment.md
[dockerfile]:/pages/dockerfile.md

[rpi]:http://www.raspberrypi.org/
[firebase]:https://www.firebase.com/

[getting-started]:/pages/gettingStarted.md
[text2speech]:https://github.com/resin-io/text2speech
[coder-fork]:https://github.com/resin-io/coder
[coder]:https://googlecreativelab.github.io/coder/
[rpiminer]:https://github.com/csquared/resin-piminer
[bitcoin]:http://en.wikipedia.org/wiki/Bitcoin
[resin-player]:https://bitbucket.org/lifeeth/resin_player/
[squeezebox]:http://www.mysqueezebox.com/index/Home
[cimon]:https://bitbucket.org/efwe/cimon
[digitiser-kiosk]:https://bitbucket.org/lifeeth/resin-kiosk
[kiosk-post]:http://blogs.wcode.org/2013/09/howto-boot-your-raspberry-pi-into-a-fullscreen-browser-kiosk/
[sms2speech]:https://github.com/alexandrosm/sms2speech
[twillio]:https://www.twilio.com/
[hoversnap]:https://github.com/resin-io/hoversnap
[digitiser]:https://github.com/shaunmulligan/digitiser
[firebase-dtl]:https://github.com/shaunmulligan/firebaseDTL
[resin-cctv]:https://github.com/abresas/resin-cctv
[simple-nodejs]:https://github.com/resin-io/basic-resin-node-project
[example-pi-pins]:https://github.com/shaunmulligan/basic-gpio
[salesforce-temp]:https://github.com/shaunmulligan/salesforceTemp

[hello-dotnet]:https://github.com/nghiant2710/hello.NET
[hello-java]:https://github.com/nghiant2710/Hello-Java
[hello-python]:https://github.com/alexandrosm/hello-python
[hello-ruby]:https://github.com/nghiant2710/Hello-Ruby

[csharp]:http://msdn.microsoft.com/en-gb/vstudio/hh341490.aspx
[dotnet]:http://www.microsoft.com/net
[jvm]:http://en.wikipedia.org/wiki/Java_virtual_machine
[java]:https://www.java.com/en/
[python]:https://www.python.org/
[ruby]:https://www.ruby-lang.org/en/

[csharp-dockerfile]:https://github.com/resin-io/hello.NET/blob/master/Dockerfile
[java-dockerfile]:https://github.com/resin-io/Hello-Java/blob/master/Dockerfile
[python-dockerfile]:https://github.com/alexandrosm/hello-python/blob/master/Dockerfile
[ruby-dockerfile]:https://github.com/resin-io/Hello-Ruby/blob/master/Dockerfile

[efwe]:https://bitbucket.org/efwe/
[shaun-mulligan]:https://github.com/shaunmulligan
[csquared]:https://github.com/csquared/
[aleksis]:https://github.com/abresas/
[lifeeth]:https://bitbucket.org/lifeeth/
[alex]:https://github.com/alexandrosm
[petrosagg]:https://github.com/petrosagg
[nghiant2710]:https://github.com/nghiant2710

[node]:https://nodejs.org/
[bitcoin]:https://bitcoin.org/
[gpio]:http://en.wikipedia.org/wiki/General-purpose_input/output
[pi-pins]:https://github.com/natevw/pi-pins
[salesforce]:https://www.salesforce.com
[ADC_py]:https://github.com/shaunmulligan/resin-rpi-py-ADC
[ADC_adafruit]:http://www.adafruit.com/product/1085
[resin-tether]:https://github.com/petrosagg/resin-tether
[dockerHub]:https://github.com/nghiant2710/resin-DockerHubDeploymentGuide
