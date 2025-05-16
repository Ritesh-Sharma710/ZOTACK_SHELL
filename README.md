 This project involves the development of a custom Unix-like command-line shell named “Tux 
Shell” implemented in C programming language. The shell provides a user-friendly interface 
for executing bith built-in and external commands, mimicking the behavior of standard shells 
while itroducing essential features such as command parsing, execution, piping, and history 
management.
 The core functionality includes a robust command parser that tokenizes user input and 
supports multiple commands separated by pipes, enabling inter-process communication. The 
shell handles built-in commands such as cd for directory navigation, help for usage guidance, 
exit to terminate the shell, history for displaying and managing previously executed commands, 
and a custom grep implementation. Command history is persistently stored in a hidden file 
within the user’s home directory, allowing users to recall and re-execute past commands 
efficiently.
 Piping is implemented by creating child processes connected via Unix pipes, allowing 
the output of one command to serve as the input to the next. The shell carefully manages file 
descriptors to handle input/output redirection and restores standard input/output after command 
execution. Signal handling is incorporated to intercept interrupts like Ctrl-C, preventing the 
shell from terminating enexpectedly and ensuring a smooth user experience.
 Memory management is addressed through dynamic allocation for reading input lines 
and token arrays, with safeguards against buffer overflows. The shell continuously prompts the 
user with a coloured command prompt indicating the current working directory enhancing 
usability.
 Overall, this project demonstrates fundamental Operating System concepts including 
inter-process communication, process creation and control, file handling and signal 
management. The modular design allows for easy extension and customization, making “Tux 
Shell” a functional and educational tool for understanding shell internals and Unix system 
programming
