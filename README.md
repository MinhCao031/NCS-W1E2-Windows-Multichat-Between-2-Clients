# Windows-Multichat-Between-2-Clients
- Note: This only works for Windows OS, and currently works on local machine

- How to compile:
  + Open Window PowerShell
  + Use cd or Set-Location to go to the folder that contains the source code
  + Use these 2 command to compile, `lWs2_32` is to link with the winsock2 library
  
  `gcc win_server.c -o demo_server.exe -lWs2_32`
  
  `gcc win_client.c -o demo_client.exe -lWs2_32`
  
- How to run:
  + Run `demo_server.exe` to setup server, then `demo_client.exe` to setup clients
  + You can open as many client apps as you can, as long as the value in 5th line from `win_socket.c` is modified big enough
  
  ```5. #define MAX_CLIENT 8 // <- Change it here```
  
