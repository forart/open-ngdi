# Richard Stallman -- On "Free Hardware" #
## Jun 22, 1999, 04:27 ##
### By Richard Stallman GNU ###

A number of people have asked the GNU Project if we would like to branch out from free software into free hardware designs, and expressed their interest in working on them. Some people have even suggested a project to make free chip designs.

To understand this issue clearly, recall that ```free software'' is a matter of freedom, not price; broadly speaking, it means that users are free to copy and modify the software. So if we try to apply the same concept to hardware, ```free hardware'' means hardware that users are free to copy and modify; a ``free hardware design'' means a design that users are free to copy, modify, and convert into hardware.

Free software is often available for zero price, since it often costs you nothing to make your own copy. Thus the tendency to confuse ```free'' with ```gratis''. For hardware, the difference between ``free'' and ``gratis'' is more clear-cut; you can't download hardware through the net, and we don't have automatic copiers for hardware. (Maybe nanotechnology will provide that capability.) So you must expect that making fresh a copy of some hardware will cost you, even if the hardware or design is free. The parts will cost money, and only a very good friend is likely to make circuit boards or solder wires and chips for you as a favor.

Because copying hardware is so hard, the question of whether we're allowed to do it is not vitally important. I see no social imperative for free hardware designs like the imperative for free software. Freedom to copy software is an important right because it is easy now--any computer user can do it. Freedom to copy hardware is not as important, because copying hardware is hard to do. Present-day chip and board fabrication technology resembles the printing press. Copying hardware is as difficult as copying books was in the age of the printing press, or more so. So the ethical issue of copying hardware is more like the ethical issue of copying books 50 years ago, than like the issue of copying software today.

However, a number of hardware ethusiasts are interested in developing free hardware designs, either because they have fun designing hardware, or because they want to customize. If you want to work on this, it is a fine thing to do. The GNU volunteer coordinators (gvc@gnu.org) can put you in touch with other people who share this interest. If organizations are formed for this purpose, the GNU Project will refer interested people to them.

People often ask about the possibility of using the GNU GPL or some other kind of copyleft for hardware designs.

Firmware such as programs for programmable logic devices or microcoded machines are software, and can be copylefted like any other software. For actual circuits, though, the matter is more complex.

Circuits cannot be copylefted because they cannot be copyrighted. Definitions of circuits written in HDL (hardware definition languages) can be copylefted, but the copyleft covers only the expression of the definition, not the circuit itself. Likewise, a drawing or layout of a circuit can be copylefted, but this only covers the drawing or layout, not the circuit itself. What this means is that anyone can legally draw the same circuit topology in a different-looking way, or write a different HDL definition which produces the same circuit. Thus, the strength of copyleft when applied to circuits is limited. However, copylefting HDL definitions and printed circuit layouts may do some good nonetheless.

It is probably not possible to use patents for this purpose either. Patents do not work like copyrights, and they are very expensive to obtain.

Whether or not a hardware device's internal design is free, it is absolutely vital for its interface specifications to be free. We can't write free software to run the hardware without knowing how to operate it. (Selling a piece of hardware, and refusing to tell the customer how to use it, strikes me as unconscionable.) But that is another issue.

### Copyright 1999 Richard Stallman ###
Verbatim copying and redistribution of this entire article is permitted provided this notice is preserved.

> Richard Stallman is the founder of the Free Software Foundation, the author of the GNU General Public License (GPL), and the original developer of such notable software as gcc and Emacs.