# intial scans

## nmap

Initial scan:
```
$ nmap -sC -sV -oA nmap/initial <TARGET_IP>
```

-sC = standard scripts
-sV = enumarate services and tell us what they are
-oA = output the results to specified location

To scan all ports, add -p-, this usually takes a while so consider leaving it running in the background by using &
```
$ nmap -sC -sV -oA -p- nmap/initial-all-ports <TARGET_IP> &
```
