# Smbclient

Used to connect to shares over smb (server message block protocol).

## List shares


### anonymous

Syntax:
```bash
smbclient -L <fileserver>
```

Example:
```bash
smbclient -L //10.129.163.38/
```

### with user 

Syntax:
```bash
smbclient -L <fileserver> -U <user>
```

### list contents

Syntax:
```bash
smbclient -L <fileserver>/<share>/<path>/<to>/<folder>
```

## interactive shell

### connect to it shell

#### anonymous

Syntax:
```bash
smbclient <fileserver>/<share>
```

Example:
```bash
smbclient //10.129.163.38/backups
```

#### with user

Syntax:
```bash
smbclient <fileserver>/<share> -U <user>
```

Resources:
https://linuxtect.com/linux-smbclient-command-tutorial/
