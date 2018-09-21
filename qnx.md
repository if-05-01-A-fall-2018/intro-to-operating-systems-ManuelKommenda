# QNX

## General Information

QNX was developed in the 1980s by a Canadian company called Quantum Software Systems. It was renamed QNX Software Systems and acquired by BlackBerry in 2010.

It was one of the first commercially successful microkernel operating systems and it is used by many different devices for example mobile phones and cars.
A microkernel is a near-minimum amount of software which can provide the mechanisms needed to use an OS.

 QNX is based on the idea of running most of the operating system kernel in the form of a number of small tasks, that's called a Resource Managers. This Systems allows developers to turn of any functionality, which they don't need without having to change the OS. Its a quit small, earlier versions fit on a single floppy disk.

 QNX Neutrino has been ported to a number of platforms and now runs on practically any modern CPU that is used in the embedded market. QNX offers a license for non-commercial and academic users.

## Technology

The QNX kernel contains only CPU scheduling, interprocess communication, interrupt redirection and timers. Everything else runs as a user process, including a special process known as proc which performs process creation and memory management by operating in conjunction with the microkernel.
This is made possible by two key mechanisms. The Subroutine-call type interprocess communication, and a boot loader which can load an image containing not only the kernel but any desired collection of user programs. The result is that there are no device drivers in the kernel.

QNX interprocess communication consists of sending a message from one process to another and waiting for a reply. The message is copied, by the kernel, from the address space of the sending process to that of the receiving process. If the receiving process is waiting for the message, control of the CPU is transferred at the same time, without a pass through the CPU scheduler.
