# BruteSSH
SSH Bruteforce Basic Script created with C++ to Linux 
# Basic Information

Basic C++ Script to Bruteforce SSH Servers, created with 3 different files BruteForce.cpp, Host.h and banner.h

- **BruteForce.cpp**: Main file focused in call the others, basically it's calling the banner, then questions the user, IP Server, the wordlist path and then it's calling a fuction called readPasswordsFromFile to send the wordlist passwords to vector and then with for loop, try to connect with differents passwords. 
- **Host.h:** The Host file basically contents one class called SSHHost, this class have two attributes, also have one constructor method, and then have two more methods, one of this its SSHConnection, this is to perform a connection with SSH server, and latelly have the last method SSHAuth, this method its to try to authenticate it with username and passwords.
- **Banner.h**: Basically creates the banner

![image](https://user-images.githubusercontent.com/79543461/215282260-12ea92a7-ea97-4e70-98f0-df1f09e35858.png)

# Usage

To use this tool it's very simple, you only need to execute the tool:

