# Recon

## Links

- [SecLists](https://github.com/danielmiessler/SecLists)
- [RustScan](https://rustscan.github.io/RustScan/)

## GoBuster

```sh
gobuster dir --url http://$IP -w /usr/share/wordlists/dirbuster/directory-list-2.3-medium.txt -t 300 -o gobuster.log --no-error
```

## Port scan

```sh
rustscan -a $IP -- -sC -sV -oN nmap.log
```
