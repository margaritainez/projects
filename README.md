Margarita Maligaya
Hello World NCURSES Project

This program contains two files: hello.cpp and Makefile. I started by creating hello.cpp and beginning the ncurses tutorial provided: https://tldp.org/HOWTO/NCURSES-Programming-HOWTO/helloworld.html. This tutorial provided the foundation of my program, as it uses the mandatory functions like initscr() and endwin(). After following the tutorial and running the code to make sure it worked, I began the Makefile. I had some trouble making this work. Professor Bart Massey provided an outline during lecture for a Makefile; however, I stumbled upon a few obstacles. First, my terminal was automatically indenting lines for me; I had to set those spaces into tabs. My Makefile still was not working when running ./hello. I altered the code by adding a TARGET, all:, and .PHONY: as suggested by a user on Stack Overflow (https://stackoverflow.com/questions/15566405/run-executable-from-makefile). This seemed to fix my command problem. I went back into the hello.cpp file to code the actual program required for the assignment. I found another helpful page from the first website listed (tldp.org) that focused on windows in ncurses. This page(https://tldp.org/HOWTO/NCURSES-Programming-HOWTO/windows.html) helped me understand the logistics of ncurses and how to maneuver the windows and borders. The last problem I had was moving the cursor to the bottom right of the terminal. When using wmove() with the arguments LINES and COLS as provided by the library, the cursor would begin at the top left. By subtracting 1 from both variables, I was able to move the cursor to the lower right corner of the terminal while it waits for a user input to end the program. Overall, this program went well. I have not made my own Makefile in a long time, and this definitely helped me remember (and learn).
# projects
