History of Linux for the PowerPC
================================

*Originally from http://gate.crashing.org/doc/ppc/doc003.htm*

*The followng history was compiled from postings on the LinuxPPC-user mailing list.*

In late 1994 Gary Thomas started thinking about Linux for the PowerPC.  After asking around the mailing lists little interest was generated so Gary set off to do it himself.  At the time PowerPC hardware was hard to come by and the tools were non existant.  Gary proceeded to get GNU tools needed to create PowerPC ELF files.  He also came up with a PowerPC simulator due to lack of hardware.  By January of 1995 basic utilities were working on the simulator.

By mid 1995 interest was starting to develop for a PowerPC port of Linux.  Gary finally had access to real PowerPC hardware and was doing development on real machines.  Joseph Brothers took up the evangelizing and support was gaining for the port.  Eventually Motorola, IBM and Be donated hardware to the project.

At this point Cort Dougan (and others) started playing with Linux on PowerPC hardware.  The original system was based on a late 1.2 series kernel, and was soon moved to the 1.3 series of development kernels.  Development continued and the user community slowly grew in size.

In October 1995, the Open Software Foundation (now known as the Open Group) and Apple Computer, Inc. started working on porting Linux to work as a server on the Mach microkernel.  In February of 1996 Apple and OSF publically announced the MkLinux project at the Free Software Foundation converence held in Boston.  This project used the tools and many kernel items that Gary and others had previously ported for the monolithic, or non-Microkernel, PowerPC Linux Port.  In May 1996 at Apple's World Wide Developers Conference and later in August at MacWorld Boston Apple gave away over 20,000 CDs containing MkLinux DR1.

By the Summer of 1996 a very complete PowerPC system had developed, both Linux and MkLinux.  Because of MkLinux, the user community mushroomed, and Linux on the PowerPC started to become mainstream.  There was some divide in the community, but most of the users viewed MkLinux and Linux being one community with two different kernels.

In June 1996, Pat Kane of Motorola produced the first non-Apple CD-ROM distribution.  His distribution could boot and install LinuxPPC on many PReP boxes.

The divide in the LinuxPPC community between LinuxPPC and MkLinux was because many people wanted more hardware information then Apple was willing to release, the latest PCI Macintosh computers were not yet supported by MkLinux and many did not want to run Linux on Mach for one reason or another.  The Linux-pmac development was started by Paul Mackerras to fill this void.  The PCI architecture and Open Firmware allowed him to take the PReP 1.3.xx code, MkLinux code, items that he and others had reverse engineered to create a monolithic port of Linux for the Macintosh.  A third branch was created.

At this point work continued on all three branches, each at various stages of development.  Soon Gary updated to kernel 2.0.xx, Paul followed.  The new development series 2.1.x was created and Cort Dougan started development for PReP (and other) PowerPC machines. Paul soon followed by updating to 2.1.x and continued to work on PowerMacintosh support.

In the fall of 1996, Mike Meissner worked with Gary to get shared library support for the PowerPC.  After trying MIT libc and various other things, a snapshot of glibc (121296) was used as the basis of the PowerPC's shared libraries.  PowerPC Linux has used these snapshot libraries until very recently.

In August of 1996 MkLinux DR2 was released as a major update to DR1.  By May 1997 Apple had readied MkLinux DR2.1, and given it away to developers at WWDC and MacWorld Boston again.  However, this did not use the shared libraries as they were still considered unproven by the MkLinux team.  By the summer 1997 MkLinux DR2.1 update 3 was released with official support for shared libraries.  This lead developers to start working with shared libraries and the possibility of a direct Red Hat Linux port instead of the mish mash of custom packages that had previously been assembled.  Also in early 1997 the LinuxPPC (maintained by Cort Dougan) and Linux-pmac started to merge their code into a single PowerPC Linux kernel source.  This meant there was now a single monolithic kernel and a microkernel based Linux for the PowerPC.  At this point, MkLinux started to lose it's appeal to some in the community.  However, MkLinux remained a starting point for thousands of new users.

In the Spring of 1997 around the same time as MkLinux DR2, LinuxPPC, Inc.  released their own distribution using a modified Red Hat installer.  Previously, you had to install MkLinux and then convert it to Linux-pmac.  This marked the first "easy to use" installation process suited for the novice to the guru.

Enter a bored college student in southern Minnesota.  Once shared library support was started Mark Hatle started to work on a Linux for the PowerPC distribution.  It was a port of the current Red Hat Linux and it used the current Red Hat Linux installer.  Along with many others in the community, he convinced both Apple and LinuxPPC, Inc. to base their next releases on this single work.  This futher brought the community together.  Developers working on both MkLinux and LinuxPPC got together and started to work on the "next" distribution.  This one would contain everything as standard as possible.  We were still using many of Gary's original tools and the glibc snapshot.

After the release of MkLinux DR3 and LinuxPPC Inc.'s R4 work began on a new distribution.  Using the latest version of Red Hat and working with the latest GNU tools such as glibc-2.1, and egcs a new distribution was created: The Linux PPC Developers Release.  This release attempts to make the most of all of the PowerPC technologies and provide a complete release, however it is not intended as "The" distribution.  Our distribution is intended to be used by the various companys involved with making Red Hat Linux "based" distributions for the PowerPC.

This is in no means a complete history of all Linux for the PowerPC.  Many important events, people, and companys have been left out.  Either we forgot them, or things started to become to complicated to explain here.  We suggestion that you look at mailing list archives from the past few years to see how fluid the LinuxPPC community really is!

With that in mind, while this distribution was being created many things happened in the Linux PowerPC world.  The Open Group (formerly OSF) had stopped working on MkLinux, Apple's public support had dropped to a background role.  However, MkLinux development started to come from the user community.  MkLinux development is where it should be, in the hands of the users.  BootX was created by Ben Herrenschmidt to allow an easier way to boot LinuxPPC on the Machintosh.  X was updated to work with XFree86 instead of X11R6.  Kernels through 2.2.5 were released, each containing official PowerPC support.  LinuxPPC, Inc. and others released distributions, while others announced plans to release distributions.

In our humble opinion, the PowerPC is "where it's at" right now in the Linux world.  Linux for the PowerPC currently supports PReP, CHRP, Be Box, Amiga PowerUP System, Macintosh, and other architectures.  We only have good things in the future.  We look forward to the community being a continued success.

*Written February 1999 by Mark Hatle*
