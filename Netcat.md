# Netcat

Used to listen (and scan) on ports for connections.

## Flags

<ul>
  <li>`-u` to use udp instead of tcp</li>
  <li>`-l` for listen mode</li>
  <li>`-p` port to listen on</li>
  <li>`-v` verbose mode (can be used twice)</li>
  <li>`-n` skip dns lookups</li>
</ul>

default to listen on a port for tcp connection:

```bash
nc -nvlp <port>
```
