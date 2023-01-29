# NMAP

nmap is a scanner of port, he can detect what protocole are running in a port and what version, NMAP is always the first step in a CTF

## PARAMETER

nmap have so many fonctionality that I'm only gonna talk about the most fondamental


## [-p] PARAMETER
\-p : is for the port idication, if you run nmap without -p he only gonna scan the most common open port,

with \-p have mutliple syntaxe
* \-p port1,port2,portX for scaning only the port1, port2, portX
* \-p port1-port2 for scaning from port1 to port2
* \-p- scan from port 1 to 65535 (all of them)

## [-sV] PARAMETER
-sV : is the show version parameter, sometimes nmap gonna tel you that the protocol in port 80 is http (because that's is default port) but you can run any protocol on port 80! for being sur what portocol is running on a port you have to add the show version parametter

## [-O] PARAMETER
-O is for detect what's the OS


## DON'T FORGET 

you have to indicate the host, put the IP adress at the end of the command. 

## DONE

that should be enought for this CTF but there are A LOT of other fonctionality check the man for more information 