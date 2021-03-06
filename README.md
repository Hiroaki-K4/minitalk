# minitalk
- You must create a communication program in the form of a client and server.
- The server must be launched first, and after being launched it must display its PID.
- The client will take as parameters:
◦ The server PID.
◦ The string that should be sent.
- The client must communicate the string passed as a parameter to the server. Once the string has been received, the server must display it.
- Communication between your programs should ONLY be done using UNIX signals.
- The server must be able to display the string pretty quickly. By quickly we mean that if you think it is too long, then it is probably too long (hint: 1 second for 100 characters is COLOSSAL)
- Your server should be able to receive strings from several clients in a row, without needing to be restarted.
- You can only use the two signals SIGUSR1 and SIGUSR2.

<br>

# My score
![minitalk](https://user-images.githubusercontent.com/51109408/129360769-11a520a6-6662-4609-9cca-e7a10cac2515.png)

# How to build
Build the files.

```
make
```
Rebuild
```
make re
```
Clean .o files
```
make clean
```
Clean all files
```
make fclean
```

# How to run
First, start the Server with the following command.
```
./server
```
Please open another terminal and send a string from the Client to the Server based on the Server's process ID.
```
./client PID Hello
```
The string sent to the terminal running the Server is displayed.
