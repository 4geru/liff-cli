# liff-cli

LIFF(LINE Front-end Framework) cli tool  
https://developers.line.me/en/docs/liff/overview/

# Installation
```
$ npm install -g liff
$ export LINE_ACCESS_TOKEN={YOUR_LINE_ACCESS_TOKEN}
```

# Usage

### list
list all registered liff applications.

```
$ liff list
```

### add
create new liff application.

```
$ liff add <url> <type:full|tall|compact>
```

### update
update the liff application.

```
$ liff update <liffId> <url> <type:full|tall|compact>
```

### delete 
delete specified liff.

```
$ liff delete <liffId>
```

### delete all
delete all liff applications.

```
$ liff deleteAll
``` 
    
### send test
send liff application URL to specified line user.

```
$ liff send <liffId> <userId>
```

## examples

```
liff list
liff add https://developers.line.me/en/docs/liff/overview/ tall
liff add https://developers.line.me/en/docs/liff/overview/ compact
liff update 1555709429-5zJQmooA https://developers.line.me/en/docs/liff/overview/ tall
liff delete 1555709429-5zJQmooA
liff deleteAll
liff send 1555709429-5zJQmooA Ue52d11061890315xxxxxxxxxxx
```

# Todo

send to LIFF App URL to Bot
- init {LINE_ACCESS_TOKEN}
export LINE_ACCESS_TOKEN by command
