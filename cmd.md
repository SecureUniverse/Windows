# CMD
![reference](https://ss64.com)

### ping (Test a network connection)
```
ping 8.8.8.8
ping -n 1 Server64
```

### nslookup (Name server lookup)
```
nslookup www.google.com
nslookup -querytype=TXT -timeout=10 google.com
```

### tracert (Trace route to a remote host)
```
tracert www.google.com
tracert 8.8.8.8
tracert local_server
```

### arp (Address Resolution Protocol)
``` 
arp -a
arp -a > a.txt
(arp -a & time /t & date /t) > arp.txt
arp -a -N 10.1.4.99
arp -s 10.1.4.77 00-AA-21-4A-2F-9A
```

### ipconfig (Configure IP)
```
ipconfig /all
ipconfig /displaydns
ipconfig /flushdns

ipconfig /release
ipconfig /renew
ipconfig /release && ipconfig /renew
```

### netstat (Display networking statistics - TCP/IP)
```
netstat -nao
netstat -s -p icmp
netstat -na 2
```
 
### route (Manipulate network routing tables)
```
route print
```

### tasklist (List running applications and services)
```
taskkill /PID 1532 /F
tasklist /svc
tasklist /FI "imagename eq svchost.exe" /svc
tasklist /v /fi "STATUS eq running"
tasklist /FI "IMAGENAME eq c*"
tasklist /v /fi "username eq e_ebadi
tasklist /M
```

### pathping (Trace route plus network latency and packet loss)
```
pathping www.google.com
```

### getmac (Display the Media Access Control (MAC) address)
```
getmac
getmac /fo table /nh /v
getmac /v /fo csv > T:\macaddresses.csv
```

### netsh (Configure Network Interfaces, Firewall & Remote access)
```
netsh advfirewall firewall set rule group="File and Printer Sharing" new enable=Yes
netsh interface set interface name="Local Area Connection" admin=ENABLED
netsh interface ip show config
netsh interface ip set address name="Local Area Connection" source=static addr=192.168.0.10 mask=255.255.255.0 gateway=192.168.0.1 gwmetric=1
netsh interface ip set address name="Local Area Connection" source=dhcp
netsh interface ipv4 add dns "Local Area Connection" 10.0.0.1
netsh interface ipv4 add dns "Local Area Connection" 10.0.0.3 index=2
netsh interface ip set dns name="Local Area Connection" source=static addr=192.168.0.2 register=none
```

### more (Display output, one screen at a time)
```
more a.txt
```

### type (Display the contents of a text file)
```
type file.txt > Newfile.txt
type file.txt >> ExistingFile.txt
type nul >filename.log
```

### findstr (Search for strings in files)
```
systeminfo | findstr Boot
findstr /s /i smith *.*
findstr "\<comp.*" C:\work\inventory.txt
```

### query user / quser (Display user sessions (TS/Remote Desktop))
```
user ursula /server:Server64
```

### dir (Display a list of files and folders)
```
dir
dir /ahd
dir /ahd
dir /R
```

### doskey (Edit command line, recall commands, and create macros)
```
doskey /history
```

### systeminfo (List system configuration)
```
susteminfo | find "me:  "
```

### find (Search for a text string in a file)
```
tasklist > tasklist.txt
find /i “svchost” < tasklist.txt

type names.txt | find "Jones"
```

### cd (Change Directory - move to a specific Folder)
```
cd \
cd ..
```

### del (Delete one or more files)
```
del A*
del *A.*
del *.doc
```

### md (Create a new Directory)
```
md newdirectory
```

### wmic (WMI Commands)
```
wmic process
wmic process list brief
wmic process list full
wmic startup list full
wmic process list brief /every:1
wmic OS get * /format:list | more
wmic COMPUTERSYSTEM get * /format:list | more
wmic OS LIST BRIEF
wmic OS GET csname, locale, bootdevice /value
wmic LOGICALDISK where drivetype!=4 get deviceid, description, volumename
wmic NICCONFIG where (IPEnabled=True and TcpipNetbiosOptions!=null and TcpipNetbiosOptions!=2) GET caption,index,TcpipNetbiosOptions,IPEnabled
wmic SERVICE where (state="running") GET caption, name, state > services.tsv
```

### hostname (Display the host name of the computer)
```
hostname
```

### mapisend (Send email from the command line)
```
mapisend -u "MS Exchange Settings" -p MyPassword -r billg@sun.com -s "Subject" -m "Test message text"
mapisend -u "MS Exchange Settings" -p MyPassword -r billg@hp.com -s "Subject" -t c:\MyMail.txt >> c:\mail.log
```

### msinfo32 (System Information)
```
msinfo32 /report C:\TEMP\test.txt
```

