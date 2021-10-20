# IntOS
Fast and light-weight operating system
# Architecture
<h3> Kernel </h3>
IntOS Based 30dayMakeOS.
<h3> Syscall </h3>
IntOS has a system call table, the call index is separated by EDX,<br> and the interrupt call number is 0x40. <br>IntOS currently has approximately 60 system calls.<br>
System call code is included on 'kernel/console.c'

# App Dev
You can use Apilib and Stdlib.<br>
I recommend config malloc=0k, for GUI Apps, stack 200k, for Console Apps, stack 10k.

# Librarys
<h3> Apilib </h3>
apilib is library for system call. <br>there are many functions and many return values are kernel memory address.
<h3> Stdlib </h3>
Originally, Stdlib was a library that collected C's standard functions,<br>
but we collected various widgets such as buttons and list boxes.

# GUI

IntOS has a GUI and mimics the graphics of Windows 95.

# Checked Error List

When you type a name of picture file or text file on command prompt,<br>System halted.<br><br>
Gview and mmlplay and some text files not working.<br><br>
Some applications failed memory management.

# LICENSE

IntOS Currently has GPL. see license.
