# directory fuzzing

## gobuster

### Initial scan:

```
gobuster -u http://<TARGET-IP>> -w /usr/share/wordlists/dirb/small.txt -s 307,200,204,301,302,403 -x txt,sh,cgi,pl -t 50
```
