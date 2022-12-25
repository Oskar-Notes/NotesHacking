# Gobuster

## DNS scan

Scan a domain for commonly used subdomain names

Syntax:
```sh
gobuster dns -w /usr/share/seclists/Discovery/DNS/subdomains-top1million-5000.txt -d 10.129.15.155
```

-d specify domain
-w specify wordlist (https://github.com/danielmiessler/SecLists/)
-t amount of threads (default: 10)
-o output file


## DIR scan

Scan a webpage for commonly used url paths.

```sh
gobuster dir -w /usr/share/seclists/Discovery/Web-Content/raft-large-words.txt -u 10.129.15.155
```

-w specify wordlist
-u url to webpage
-p password for basic auth
-U username for basic auth
