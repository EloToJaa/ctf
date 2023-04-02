# Recon

## Links

- [SecLists](https://github.com/danielmiessler/SecLists)
- [RustScan](https://rustscan.github.io/RustScan/)

## GoBuster

```sh
gobuster dir -w /usr/share/wordlists/dirbuster/directory-list-2.3-medium.txt --no-error -t 300 -o gobuster.log --url http://$IP
```

## Port scan

```sh
nmap -sC -sV -oN nmap.log $IP
```
