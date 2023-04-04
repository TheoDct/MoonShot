# Moonshot Project Report - February 2023

## Overview

My moonshot project is a kernel/operating system build to only execute binary code in an embedded system, for instance, the infotainment system of a car or on a microcontroller, the purpose of this project is to let the software focus on the application and not on the stack of the operating system.

It is just like the ``` FROM scratch ``` docker image, but directly on the hardware.

## Current state

I have taken into the consideration the report of my presentation and I decided to focus only on a single CPU architecture, which is the ARMv7 architecture, I will not support other architectures for now.

I also decided to do the kernel in rust, I started to write it in C and then Go but I realized that C was not the best choice for memory management and for the case of Go even if it is a good "low" level language I do not have a lot of control on the hardware and I do not want to use a different library to do it.

That's how I ended up with rust, where I searched for documentation about low-level programming, and for me, it's the most optimal choice for a project like that.

Overall the project is in a pretty good state, I can run a simple hello world program on a virtual machine of an ARM architecture with my kernel written in rust and assembly, which is a pretty good start.

## Next steps

I think about the next steps and the next features to implement, I am thinking about being able to run a simple go program compiled to a binary file to test the behavior of the kernel.

I also want to implement a debug mode to be able to see the output of the kernel and the program running on it which is going to make the development way much easier.

And finally, I want to implement a way to just read a file directly from an SD card/USB stick and execute it directly, I want to make something very simple and plug and play, I still need to find a way to make it safe and secure but I think it is possible.
