# Gobuster

## DNS scan

Scan a domain for commonly used subdomain names

Syntax:
```sh
gobuster dns -w /usr/share/seclists/Discovery/DNS/subdomains-top1million-5000.txt -d 10.129.15.155
```

<ul>
  <li>-d specify domain</li>
  <li>-w specify wordlist (https://github.com/danielmiessler/SecLists/)</li>
  <li>-t amount of threads (default: 10)</li>
  <li>-o output file</li>
</ul>


## DIR scan

Scan a webpage for commonly used url paths.

```sh
gobuster dir -w /usr/share/seclists/Discovery/Web-Content/raft-large-words.txt -u 10.129.15.155
```

<ul>
  <li>-w specify wordlist</li>
  <li>-u url to webpage</li>
  <li>-p password for basic auth</li>
  <li>-U username for basic auth</li>
  <li>-X search for specific file extension</li>
</ul>
