# GCC 4.9.3 cross-compiler for Raspberry Pi (supports Pi 1) on Mac 
> It's hard but it's possible! (**tested on 10.11.6**)

I took me days and a lot of anger to compile this gcc-version on my Mac  
Clang is a nice compiler but ct-ng support for Mac/Clang is quite poor.

The guys behind Raspberry-PI.org think the whole world develops on Linux...  

Anyways - if this repo helps other developers 
to avoid reinventing the wheel over and over again I met my goals!
 
## What I used to compile the whole thing 

   - ct-ng 1.22   
   brew install crosstool-ng
   
   - [Raspberry Pi -- Cross Compiling on Mac OSX](http://www.jaredwolff.com/blog/cross-compiling-on-mac-osx-for-raspberry-pi/)  
   By far the best infos I could find on the net  
   
   - [arm-rpi-4.9.3-linux-gnueabihf.config](https://github.com/raspberrypi/tools/tree/master/configs)  
   From Raspberry-Tools on GH but this config does not work on Mac
       
   - Nerves, nerves, nerves and a lot of reading and googling
           
## Which toolchain do I use
Here you have it: [arm-rpi-linux-gnueabihf.cmake](https://github.com/MikeMitterer/cmake/blob/master/arm-rpi-linux-gnueabihf.cmake)

## IDE
At the time of writing: CLion 2016.3.2 - which got nice Toolchain-support in the last release!
 
## How to install the cross-compiler
Unpack it! ;-)  
As you can see in my toolchain-file - I've copied the arm-rpi-linux-gnueabihf folder to
  
    /usr/local/Mike/arm-rpi-linux-gnueabihf 
           
Adapt this to your needs  
   
## Support   
If this repo is helpful for you - please 
  - [(Circle)](http://gplus.mikemitterer.at/) me, follow me on 
  - [Twitter / MikeMitterer](http://t.co/azTkrn2M6E) or on 
  - [FaceBook](https://www.facebook.com/mikemitterer.at)
   
It would be also cool if you **star** this repo here on GitHub   
   



   
   
   