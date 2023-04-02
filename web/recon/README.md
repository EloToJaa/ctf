# Recon

## Links

- [SecLists](https://github.com/danielmiessler/SecLists)
- [RustScan](https://rustscan.github.io/RustScan/)

## Dir enumeration

```sh
gobuster dir -w /usr/share/wordlists/dirbuster/directory-list-2.3-medium.txt --no-error -t 300 -o gobuster.log --url http://$IP
```

## Subdomain enumeration

```sh
gobuster vhost -w /usr/share/seclists/Discovery/DNS/subdomains-top1million-5000.txt -t 300 --append-domain -o vhost.log -u DOMAIN
```

## Port scan

```sh
nmap -sC -sV -oN nmap.log $IP
```
