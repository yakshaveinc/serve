This repository is mostly an example of using IPython as a Bash replacement. To solve the problem of quickly serving current directory over HTTP, it is better to use https://github.com/philippgille/serve which provides `snap` packages and many convenient features.

---

Precedence (TBD):

- PHP5+
- Python3

### PHP5+

http://php.net/manual/en/features.commandline.webserver.php

```
php -S <addr:port> [-t <docroot>]

  -S <addr>:<port> Run with built-in web server.
  -t <docroot>     Specify document root <docroot> for built-in web server.
```

 * needs explicit host:port
 * option to specify `<docroot>` without `cd`
 * processes .php

### Python3

```
python3 -m http.server [--cgi] [--bind ADDRESS] [port]

  port                  Specify alternate port [default: 8000]

  --cgi                 Run as CGI Server
  -b,--bind ADDRESS     Address to listen on [default: all interfaces]

```
