# Wordpress

## Links

- [wpscan](https://github.com/wpscanteam/wpscan)

## Wordpress scan

```sh
wpscan --url https://$IP -e vp,u
```

## Wordpress bruteforcing

```sh
wpscan --url http://$IP/ --usernames $USER --passwords $WORDLIST --max-threads 300
```

## Windows Wordpress exploit

```sh
exploit/unix/webapp/wp_admin_shell_upload
```
