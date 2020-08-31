我是光年实验室高级招聘经理。
我在github上访问了你的开源项目，你的代码超赞。你最近有没有在看工作机会，我们在招软件开发工程师，拉钩和BOSS等招聘网站也发布了相关岗位，有公司和职位的详细信息。
我们公司在杭州，业务主要做流量增长，是很多大型互联网公司的流量顾问。公司弹性工作制，福利齐全，发展潜力大，良好的办公环境和学习氛围。
公司官网是http://www.gnlab.com,公司地址是杭州市西湖区古墩路紫金广场B座，若你感兴趣，欢迎与我联系，
电话是0571-88839161，手机号：18668131388，微信号：echo 'bGhsaGxoMTEyNAo='|base64 -D ,静待佳音。如有打扰，还请见谅，祝生活愉快工作顺利。

# ![](https://raw.githubusercontent.com/schollz/find/master/static/img/FIND_icon_larger.png) FIND

[![Build Status](https://travis-ci.org/schollz/find.svg?branch=master)](https://travis-ci.org/schollz/find)
[![Version 2.4](https://img.shields.io/badge/version-2.4-brightgreen.svg)](https://www.internalpositioning.com/guide/development/) 
[![Github All Releases](https://img.shields.io/github/downloads/schollz/find/total.svg)](https://github.com/schollz/find/releases)
[![FIND documentation](https://img.shields.io/badge/find-documentation-blue.svg)](https://www.internalpositioning.com/) 
![Coverage](https://img.shields.io/badge/coverage-57%25-orange.svg) 
[![Donate](https://img.shields.io/badge/donate-$1-brown.svg)](https://www.paypal.me/ZackScholl/1.00)
[![Join the chat at https://gitter.im/schollz/find](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/schollz/find?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) 

[![](https://raw.githubusercontent.com/schollz/find/master/static/splash.gif)](https://www.internalpositioning.com/)

**Keywords**: indoor GPS, WiFi positioning, indoor mapping, indoor navigation, indoor positioning

# About

**The Framework for Internal Navigation and Discovery** (_FIND_) allows you to use your (Android) smartphone or WiFi-enabled computer (laptop or Raspberry Pi or etc.) to determine your position within your home or office. You can easily use this system in place of motion sensors as its resolution will allow your phone to distinguish whether you are in the living room, the kitchen or the bedroom, etc. The position information can then be used in a variety of ways including home automation, way-finding, or tracking!

> Simply put, FIND will allow you to replace _tons_ of motion sensors with a _single_ smartphone!

The system is built on two main components - [a server](https://ml.internalpositioning.com/) and a fingerprinting device. The fingerprinting device ([computer program](https://github.com/schollz/find/releases/tag/v0.5) or [android app](https://play.google.com/store/apps/details?id=com.hcp.find)) sends the specified data to the machine learning server which stores the fingerprints and analyzes them. It then returns the result to the device and stores the result on the server for accessing via a web browser or triggering via hooks.

**FAQ (abbreviated)**:

- How does it work? It uses already available WiFi information to classify locations. [See here for more detailed information](https://www.internalpositioning.com/faq/#how-does-it-work).
- Doesn't this already exist? [Yes, kinda](https://www.internalpositioning.com/faq/#doesnt-this-already-exist).
- What's the point? This short piece of code can do [home automation](https://www.internalpositioning.com/faq/#can-i-run-the-server-at-home-on-the-lan-connection) and [replace motion sensors](https://www.internalpositioning.com/faq/#can-it-replace-motion-sensors) and [more](https://www.internalpositioning.com/faq/#whats-the-point-of-this).
- Can I use an iPhone? [Sorry, no](https://www.internalpositioning.com/faq/#can-i-use-an-iphone).
- Does it work on a Raspberry Pi? [Yes](https://www.internalpositioning.com/faq/#can-you-run-the-server-on-a-raspberry-pi).
- Does it work with [home-assistant.io](https://home-assistant.io/)? [Yes](https://www.internalpositioning.com/faq/#does-it-work-with-home-assistantio).
- Can I help? [Yes, please](https://github.com/schollz/find/issues).
- How do I try it? It's easy. Just [download and run](https://github.com/schollz/find#usage).

More questions? See the [unabbreviated FAQ](https://www.internalpositioning.com/faq/).

# Quickstart

If you'd like to install things yourself, see [the documentation](https://www.internalpositioning.com/setup/). You don't need to do this to try it though. Follow the 3 steps below to get started quickly.

## 1\. Download the software

**Android users:** [download the current version of the app](https://play.google.com/store/apps/details?id=com.hcp.find). _Sorry iPhone users but [the Apple store prevents apps that access WiFi information](https://www.internalpositioning.com/faq/#can-i-use-an-iphone), so I will be unable to release a iPhone version._

**OR**

**Computer users:** you can [download the current version of the fingerprinting program](https://github.com/schollz/find/releases/tag/v0.5), available for Rasbperry Pi, OSX, Linux, and Windows.

## 2\. Gather fingerprint data

First, to get started using **FIND** you will need to gather fingerprint data in your locations.

**Android users:** When you start up the app you will be asked for a username (enter whatever you want) and you'll be assigned a unique group name. Simply click "Learn" and you'll be prompted for a location name. After you enter a location, the app will connect to the server and then submit fingerprints.

<center><img src="https://i.imgur.com/fbcYom5.png" width="200px">
<img src="https://i.imgur.com/Ab9eXIk.png" width="200px"></center>

<br>

**Computer users:** To start learning locations simply use `./fingerprint -e`.

## 3\. Track yourself

Once you've collected data in a few locations, you can track yourself.

**Android users:** Just press the "Track" button when you're ready to track.

**Computer users:** Type in `./fingerprint` to start tracking yourself.

# More information

See the documentation at <https://www.internalpositioning.com>.

# Acknowledgements

![](https://i.imgur.com/Ze51DJ6.png) Funding from [Duke University Colab](https://colab.duke.edu/)

Thanks to [tscholl2](https://github.com/tscholl2), [sjsafranek](https://github.com/sjsafranek), and [jschools](https://github.com/jschools) for their help in guiding the development of **FIND** and creating the early versions of FIND with me! Thanks to Rishabh Rajgarhia and [CanvasJS](http://canvasjs.com/) for help implementing a nice graph. Thanks [arafsheikh](https://github.com/arafsheikh) for adding interface selection, [Pugio](https://github.com/Pugio) and [ScottSWu](https://github.com/ScottSWu) for adding OS X/Windows support for the fingerprint program, including a better [Windows scanning utility](https://github.com/ScottSWu/windows-wlan-util/releases)! Thanks [Thom-x](https://github.com/Thom-x) for the Dockerfile. Thanks [certifiedloud](https://github.com/certifiedloud) for implementing the change to `DELETE` requests and implementing sockets for unix. Thanks [bebus77](https://github.com/bebus77) for making a awesome generic struct for OS support on the fingerprinting program! Thanks [christoph-wagner](https://github.com/Christoph-Wagner) for help with polling interval on app. Thanks to [patorjk](http://patorjk.com/software/taag/) and [asciiworld](http://www.asciiworld.com/) for the ASCII art. Thanks to [Imgur](https://imgur.com/a/yjvci) for [hosting](https://imgur.com/a/3yGjV) images.

## Donate

Like this? Help me keep it alive [by donating $5](https://www.paypal.me/ZackScholl/5.00) to [pay for server costs](http://rpiai.com/donate/).
