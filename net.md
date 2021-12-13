# NET

## Logins & Security (Test a network connection)

### net accounts
```
NET ACCOUNTS
NET ACCOUNTS /DOMAIN
```
### net user
```
NET USER username {password | *} /ADD [options] [/DOMAIN]
NET USER [username [password | *] [options]] [/DOMAIN]
net user ehsan
net user /add hacker110 Aa123456
net user /add c100$ Aa123456
```
### net group
```
NET GROUP groupname /ADD [/COMMENT:"text"] [/DOMAIN]
```
### net local group
```
NET LOCALGROUP spud /add
```

## Network configuration (Workstation/Server)
```
NET COMPUTER \\ComputerName /ADD
NET CONFIG RDR
NET STATISTICS WORKSTATION
```

## Manage open files and user sessions
```
NET FILE
NET SESSION /DELETE
```

## Help
```
NET HELP SERVICES 
NET HELPMSG 2184 
```

## Create file and printer shares
```
NET SHARE
NET SHARE workgroups=C:\work /REMARK:"workgroups share" /CACHE:No
NET SHARE workgroups /DELETE
```

## Connect to a file/print Share (Drive Map) 
```
net use /Persistent:Yes
net use [LPTx:] \\ComputerName\printer_share /PERSISTENT:YES
net use [driveletter:] \\ComputerName\ShareName /PERSISTENT:YES
net use [driveletter:] \\ComputerName\ShareName\folder1\folder2 /PERSISTENT:No
net use H: /Home
net use J: \\MainServer\Users\%Username%
net use W: \\MainServer\GroupShare /Persistent:No
net use \\MainServer\SharedPrinter
net use \ipaddressipc$ "" /user:administrator
net use K: \computernameC$
```

## View file and printer shares
```
net view \\192.168.72.149
```
