# Moonshot Project Report - April 2023

## Advancement

My moonshot project is going well; I have discovered a lot of things about kernel development and compilation; I did some research on execution of binary files in Rust where I found a built-in function called ```std::process::Command::new("file").output()``` that can allow me to execute a binary file and add some arguments to it; also I am planning to buy a board to test my kernel on real hardware instead of a virtual machine.

For the kernel on itself, I just reused plenty of concepts from my first attempt at a kernel in Go where I had to use a lot of assembly code, Rust provides built-in functions to put assembly code in Rust code which is really convenient.

## Next steps

Now that I have a better understanding of the project and since I want to have a really simple but secure kernel, I will focus on **CPU exceptions** and **Hardware interrupts**; it will allow me to have a better control on the hardware and to be able to handle errors and interrupts from the hardware which is one of the most significant part of this project.

For now, I need to think about one thing "How to flash code on the board?"; I am thinking about letting the user flash on the board with a USB stick or an SD card, altough I need to find a way to make it secure and safe for the end user without being too restrictive or too easy to bypass.

### Why not pushing on this repository?

For the time being, I do not want to push on this repository because I am unsure if I will try to monetize this project at some point since ARMv7 is not a free architecture. If I do, I will simply migrate the code from my private repository to this one.
