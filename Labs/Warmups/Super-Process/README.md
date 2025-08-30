\# Super Process Warmup Lab



\## Introduction

Super Process warmup is a Hackerviser CAPT lab that focuses on:

\- Discovering vulnerabilities in open-source web applications

\- Gaining access to the target machine

\- Performing privilege escalation to root



\## Objectives

\- Identify open ports and running services

\- Exploit the Supervisor web application

\- Escalate privileges using SUID binaries

\- Verify root access and view sensitive files



\## Lab Summary

\- \*\*Target machine IP:\*\* 172.20.29.30

\- \*\*Tools used:\*\* nmap, msfconsole, searchsploit, python, find, sudo

\- \*\*Key vulnerability:\*\* Supervisor 3.3.2 XML-RPC RCE (CVE-2017-11610)



\## Steps Followed

1\. Perform port scanning using `nmap`

2\. Enumerate directories using `gobuster`

3\. Search for Supervisor exploits with `searchsploit`

4\. Launch Metasploit, set `RHOSTS` and `LHOST`, and exploit the target

5\. Gain a shell using meterpreter

6\. Find SUID binaries with `find / -perm -4000 -type f`

7\. Perform privilege escalation using Python SUID exploit

8\. Verify root access with `whoami`

9\. View the root password hash in `/etc/shadow`



\## References

\- \[Supervisor GitHub Issue](https://github.com/Supervisor/supervisor/issues/964)

\- \[Debian Security Advisory](https://www.debian.org/security/2017/dsa-3942)

\- \[CVE-2017-11610](https://nvd.nist.gov/vuln/detail/CVE-2017-11610)



