# directory fuzzing

## gobuster

### Initial scan:

```
gobuster -u http://<TARGET-IP>> -w /usr/share/wordlists/dirb/small.txt -s 307,200,204,301,302,403 -x txt,sh,cgi,pl -t 30
```

- -u : the target URL or IP address
- -w : the wordlist we want to use
- -s : response codes that we want to be notified about
- -x : file extensions to check for (in conjunction with the wordlist)
- -t : the number of threads to run
