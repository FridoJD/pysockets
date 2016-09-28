## pysockets
#### Required:
_Two Linux machines with python3.4 installed._
<br>
<br>
#### Usage:
##### On your first machine which will be the host:
Edit the socketserver file and on line 12 replace the IP address behind "host" with the address of this machine.
<br>
<br>
Make the script executable: `chmod +x socketserver`
<br>
Run the script: `./socketserver`
<br>
<br>
##### Now on your second machine which will connect to the host:
Edit the socketclient file and on line 12 replace the IP address behind "host" with the address of the _remote_ machine.
<br>
<br>
Make the script executable: `chmod +x socketclient`
<br>
Run the script: `./socketclient`
<br>
<br>
After executing the script on the client machine you will be prompted to enter a command. The socketclient will then send a bash command such as `ifconfig` `reboot` or `mkdir` to the remote machine running the socketserver script.
