Twin-Linux
==========

Twin-Linux: Running independent Linux kernels simultaneously on separate cores of a multi-core system. Undergraduate project work done at Pune University

Abstract:
There are three classes of common consumer and enterprise
computing - Server, Interactive and Real-Time.
These are characterized respectively by the need to obtain
highest throughput, sustained responsiveness, and
hard real-time guarantees. These are contradictory requirements
hence it’s not possible to implement an operating
system to achieve all these goals. Most operating
systems are designed towards serving only one of these
classes and try to do justice to the other two classes to a
reasonable extent.

We demonstrate a technique to overcome this limitation
when a single hardware box is required to fulfill multiple
of these computing classes. We propose to run different
copies of kernels simultaneously on different cores
of a multi-core system and provide synchronization between
the kernels using IPIs (Inter Processor Interrupts)
and common memory. Our solution enables users to run
multiple operating systems each one the best for its class
of computing. For ex., using our idea we can configure a
quad core system with 2 cores dedicated for server class
computing (database processing), 1 core for UI applications
and remaining 1 core for real-time applications.

This idea has been used in the past, primarily on nonx86
processors and custom designed hardware. Our proposal
opens the doors of this idea to the off-the shelf
hardware resources. We present Twin-Linux, an implementation
of this scenario for 2 processing units using
Intel-Core-2-Duo system. This idea finds applications
in - Filers,Intelligent Switches, Graphics Processing Engines,
where different types of functions are performed
in a pipelined manner.
