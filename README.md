# WORKSHOP_CTF


## WHAT IS A CTF? 

CTF stand for Capture The Flag, the purpose of a CTF is to realise a cyber security exercise where you have to find flags,a flag is a text file with a secret content, the hard part is to gain privilege for accessing to these files.
They are always two flags by CTF
The two flags are
    - user.txt to one of the user directory (In /HOME) 
    - root.txt in /root directory.

## CONFIGURATION

We are going to do the (easyctf)[https://tryhackme.com/room/easyctf] from (TryHackMe)[https://tryhackme.com/] 
So firstly we have to download the (OpenVPN)[https://tryhackme.com/access] file.
    - Generate your configuration file
    - Then Download your configuartion file
    - Finaly run your configuration file with
        > sudo openvpn username.ovpn

refresh the tryHackMe access webpage and check if your connected
if yes go to the (easyctf webpage)[https://tryhackme.com/room/easyctf], join the room and start the box.


## WERE DO I START?

As you can see there are a lot of questions, you have to answer correctly to any of them, these questions are here for guiding throught the CTF.

If all of your answers are correct you WON :)


## STEP 1 Analyse

OK so we have an IP address, good,
try to ping the IP adress with
ping \<IP\>
if you get reply then your ready for the (Protocole detection)[LOCAL]

## STEP 2 WEB

Ok, there is a website, then there is webpage, obviously, do you think that all webpage should be accessible? Surly not!
why not trying to find some intersting file with some (Directory enumeration)[LOCAL]

## STEP 3 FIND THE EXPLOIT

SOMTIMES exploit might be find in some input field, or request,
and sometimes it's juste beacause you forget to update your computer (that why you always should make your update).
WE can see that question : 

What's the CVE you're using against the application? 

that means that there are a application outdated (or not but with some exploit) that we can exploit.
I have noting else to say except ... let's make some shearsh in 
(exploit DB)[https://www.exploit-db.com/]
(the syntaxe for the answer is CVE-YEAR-ID)

## STEP 4 THE PASSWORD IS HASHED :/

Obvously, we don't keep password in raw on database, WAY TO DANGEROUS,
once upon a time a society called Rockyou haven't crypted the password on the data base and guess what, they have been hacked, every password have been leaked, what a mess for the user! (imagine you have the same password for every website) but today we hashed the password (mathématical operation on a string whou couldn't be reversed).
So what can we do ... little hint (here)[LOCAL]  


## STEP 5 USER OWN !

Ok now you should be able to login into the sever throught SSH

(check ssh man if don't know how to use it)


now that's gonna be easy ... 

sudo -l is the first command that you would try, thats for listing all allowed command  

so check the sudo -l command, figure out by yourself the outpout...


you can get some intersting information about what tools can be use to make some privilege escalation (here)[https://gtfobins.github.io/#]

last things: sudo -u is use to execute a command as somme one else.
check the man for more information


## STEP 6 ROOT OWN!

yeah, already you have finished the CTF congratulation!
Generaly the escalation privilege is a bit more complicated but that the fondamental.

If you want to go further in CTF you should try
(hackthebox)[https://www.hackthebox.com/] : intermediate
(root-me)[https://www.root-me.org/] : mini challenge
(TryHackMe)[https://tryhackme.com/] : begginer






