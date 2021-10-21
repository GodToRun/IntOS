# Int OS App Development Guide
# Hello World Application
#include <apilib.h><br>
void HariMain(void) {<br>
    api_putstr0("Hello, World!");<br>
    api_end();
<br>
}
# Code Interpretation
first, #include <apilib.h> is include api library.<br>
and Haribote Kernel use starting point 'HariMain'.<br>
api_putstr0 is print text into console. (like puts)<br>
api_end is like return 0. dont forget use api_end at last HariMain function!<br>
# Hello World Application in Stdlib
But we have problems. Hello World Program is so different from<br>
other operating systems.<br>
so, we'll use stdlib library.<br><br>
#include <stdlibs.h> //include stdlib library<br>
void main(void) { //stdlib will change main to HariMain.<br>
  printf("Hello, World!"); // Standard print function <br>
  exit(0); //api_end <br>
} <br>
# GUI
#include "apilib.h"

void HariMain(void)
{<br>
	int win;<br>
	char buf[150 * 50];
  
	win = api_openwin(buf, 150, 50, -1, "hello");
	for (;;) {
      //Infinity loop
	}
	api_end();
}
