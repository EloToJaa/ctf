# Wordpress

## Links

- [wpscan](https://github.com/wpscanteam/wpscan)

## Wordpress scan

```sh
wpscan -e vp,u --url https://$IP
```

## Wordpress bruteforcing

```sh
wpscan --max-threads 300 --usernames $USER --passwords $WORDLIST --url http://$IP/
```
