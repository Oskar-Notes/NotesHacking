# John the ripper


## Hash cracking

basically hashes a list of passwords and compares the output hashes with a given hash.

Syntax:
```bash
john --wordlist=/usr/share/wordlists/rockyou.txt hash.txt
```


## password protected zip

### Step 1

Use zip2john to get a crackable hash of the zip file and store it in a file called `zip.hash`.

Syntax:
```bash
zip2john file.zip > zip.hash
```

### Step 2

Crack the hash. Ref: [HashCracking](https://github.com/Oskars-Notes/NotesHacking/blob/main/JohnTheRipper.md#hash-cracking)

```bash
john --wordlist=/usr/share/wordlists/rockyou.txt zip.hash
```

### Resources
https://systemweakness.com/cracking-password-protected-zip-files-using-john-the-ripper-c3b55c27e0fe

