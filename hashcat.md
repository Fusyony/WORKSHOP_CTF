# HASHCAT

Brutforce hash with hashcat

how does it works?

if I cannot get a password from a hash... but i can have a hash from a password.
then why not hash some random text and compare the result with the hash
if that the same hash, then we have find the password!

but obvouly brut force password gonna take a while.
so we use a dictonary attack.

we give a wordlist to hashcat and a hashing protocol and he gonna compare  every hashed word in the wordlist whith the hash.

another things HASH can be salted (we add a key to the encryption protocol)
if you have a saleted hash, you have to indicate the salt key to hashcat 


## PARAMETER


## [-a] PARAMETER

-a is for the attack time (stay with -a 0)


## [-m] PARAMETER

-m is for the hash-time, you can find what kind of hash you have with hashid


## DON'T FOREGET

don't foreget to add the hash and the wordlist path


## EXEMPLE


    hashcat -a 0 -m 20 'HASH:SALT' /PATH/TO/WORDLIST.txt
    hashcat -a 0 -m 0 'HASH' /PATH/TO/WORDLIST.data


