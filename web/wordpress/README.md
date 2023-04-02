# Wordpress

## Links

- [wpscan](https://github.com/wpscanteam/wpscan)

## Note

Correct order of cmd args is required!

## Wordpress scan

```sh
wpscan --url http://$IP --api-token $TOKEN  -e ap,t,u
```

## Wordpress bruteforcing

```sh
wpscan --url http://$IP --usernames $USER --passwords $WORDLIST --max-threads 300
```
