# Bash

## out/in
0 = stdin
1 = stdout
2 = stderr

you can create custom file descriptor

## Redirects

<ul>
  <li>`>` to redirect the standard ouput</li>
  <li>`n>` to redirect a specified file descriptor (e.g. `2>` to redirect stderr</li>
  <li>`&>` to redirect stout and stderr</li>
  <li>`n>&m` to redirect one file descriptor to another file descriptor (e.g. `2>&1` to redirect stderr to the output of stdout)</li>
</ul>

to surpress stdout and stderr
```bash
command &> /dev/null 
```

### Resources
https://catonmat.net/bash-one-liners-explained-part-three


