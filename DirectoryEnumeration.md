# FFUF

Fuff is a quick directory fuzzer I used to using gobuster or dirb but trust me fuff is quicker so let's learn how to use it 

## What is a FUZZER?
A fuzzer is the tool we use to make fuzzing, the objective is to try a lot of different data and if the application crash, that mean that there are some default to patch

but we have a WEB fuzzer, we not (normaly) gonna crash any things, instead we gonna try a path a inspect the reply, if the status isn't 404 then the file/directory exist.

fuff isn't a package, you can found the logiciel from is (github webpage)[https://github.com/ffuf/ffuf]

## PARAMETER

## [-w] PARAMETER 

-w is for indicate a wordlist (a list of common words that we can found in a URL like "index")

the usage is -w /path/to/the/wordlist


## [-u] PARAMETER

-u is for the URL of the host

the usage is -u http://\<IP\>/FUZZ.
FUZZ keyword is remplaced by each word in the wordlist, he is just here to indicate were you want to inject the words.


## DONE

as nmap, TONE of other things to say on FFUF but it should be enought.

