# Bomblab
Diffusing "Binary Bombs" using gdb

*   Purpose
    -------
    *   bomblab tests your ability to comprehend assembly instructions in an executable file and accurately predict their output.
    *   Specifically, you will be provided with an executable object file and the C source code for the basic structure of the program.
    *   Your task will be to examine the assembly instructions and determine the exact nature of the input required in order for each function to work properly.
    *   The lab is referred to as "bomblab" because each function is considered to be a bomb that you must defuse. If you provide the correct input, the bomb is defused and the program outputs a congratulatory message. Conversely, if you enter incorrect input, the bomb explodes and the program terminates abruptly.
    *   There are six functions, or bombs, in the program that you must defuse. Each one is progressively more difficult.
    *   Your goal is to determine the strings and/or numbers that you must enter as input for each function. If a function is expecting several arguments, you may enter them on the same line, separated by space.
    *   You may use the debugger, `gdb`, `objdump`, and any other tools that you wish, to disassemble the executable file and determine the exact nature of the input that each function demands.
*   Getting the Files
    -----------------
    *   The files you need for this lab are included within an archive file named `bomblab-handout.tar`. It is posted on D2L, but you may also copy it on the class server from `/home/DPU/kheart/bomblab-handout.tar`.
    *   You can unpack the archive by using the `tar` command as follows: 
        $\> tar xvf bomblab-handout.tar        
    *   A new directory named "`bomblab`" will be created. There are two files in that directory:
        1.  `bomb` \-\- a binary executable in ELF format, which is the native executable format for Linux. This file was compiled and linked on the class server, which is running CentOS 7.2. It can be executed on any compatible platform.
        2.  `bomb.c` \-\- the original source code for the `main` function in `bomblab`.
*   Evaluation
    ----------
    
    *   As you determine the correct inputs for each function, you must enter them into a file, named "solution.txt".
    *   You can run the program with the solution file as the sole command line argument, as follows:
        
        #\> bomb solution.txt
        
        The bomb program will read "solution.txt" one line at a time and use that input for the next function.
