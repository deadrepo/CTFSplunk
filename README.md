#CTFSplunk
-------------------

![](splunk.png)

How to Solve ?
-------------------

- Use base search `index=botsv3 sourcetype="XmlWinEventLog:Microsoft-Windows-Sysmon/Operational" EventCode="1" "fyodor-l.froth.ly" MD5="*"`

- Search for `"C:\windows\temp\hdoor.exe" -hbs 192.168.9.1-192.168.9.50 /b /m /n`

- "C:\windows\temp\hdoor.exe": This is the path to the executable file "hdoor.exe" on a Windows system. It is enclosed in double quotes, which is common when dealing with file paths containing spaces.

- -hbs 192.168.9.1-192.168.9.50: These are command-line options for the "hdoor.exe" program. It appears to be specifying a range of IP addresses from 192.168.9.1 to 192.168.9.50 using the -hbs option. This range might be used for scanning or interacting with devices within that IP range.

- Search for the MD5 Hash files
