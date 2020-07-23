# Code once take three output: Web, Android, IOS

This repository is moved to here: https://gitlab.com/msamarehshafeei/mobilewebappartchitecture

This architecture has following advantages:

- Implementation of mobile and web can be shared or separated without holding any state so the developers work only on one source code for web version and mobile (No need to copy web version to mobile version)
- It is pure Angular architecture which can support Cordova (which doese not force any other framework such as Ionic or NativeScript)
- Can separate modules and their routings for mobile and website during compile time so the final web version doese not contain mobile modules and vice versa
- Force lazy load of pages (each page has separate module)
- Pages layers only have dependency to @intermediate layer so it is decoupleded from implementation of services which results in changing of their implementation anytime needed
- Since layouts are in Theme then you can dynamically change the layouts or theme during run time
- Has separate layers for Theme and Core which can be in NPM server


