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

![image](https://user-images.githubusercontent.com/79543461/215282462-d1b6b558-b647-42e9-9643-d0010c8d0b35.png)

Then answer the basic questions about your victim and put the path of your wordlist.

![image](https://user-images.githubusercontent.com/79543461/215282431-3f3b9aab-3049-4f0c-b924-81c640babf73.png)

Now it's starting tryng passwords:

![image](https://user-images.githubusercontent.com/79543461/215282544-272182be-ff3d-49ee-8e6f-7938091bc061.png)

And then the password its founded.

![image](https://user-images.githubusercontent.com/79543461/215282564-f4c6100b-e7a2-4d36-a0f7-47a8faa44d6c.png)

# Compile 

g++ BruteForce.cpp -l ssh -o bruteSSH

