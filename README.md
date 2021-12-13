# Windows

## Recon
- Host Discovery
  - Nmap: ```nmap -Pn -sV -p 80 10.0.30.43```
  - Zenmap
  - Powershell: [Github](https://github.com/BornToBeRoot/PowerShell_IPv4NetworkScanner)
- IIS
  - whatweb
    - Find information about the running IIS Server 
    - ```whatweb 10.0.29.163``` 
  - [httpie](https://github.com/httpie/httpie)) 
    - Gather target sever information
    - ```http 10.0.29.163```
  - dirb
    - discover the web server’s directories and subdirectories 
    - ```dirb http://10.0.29.163```
  - [Browsh](https://github.com/browsh-org/browsh) 
    - To use the terminal to access the web application
    - ```browsh --startup-url http://10.0.29.163/Default.aspx``` 

## Basic Exploitation

## Post Exploitation

## Service Exploitation

## Privilege Escalation

## Maintaining Access

## Other
- [cmd](/cmd.md)
- [net](/net.md)
- [path](/path.md)
- [powershell](/powershell.md)
