koko
====

instant file server (proxy server).

Koko start server on port picked randomly,
and current directory is set as document root.

### Install
```bash
% npm install -g koko
```

### start server
```bash
% cd your/document/root
% koko
document root : your/document/root
[listen 59733]
```

or, with path. use option -p (--path).

```bash
% koko -p your/document/root
document root : your/document/root
[listen 1835]
```

### auto open

with -o (--open), Koko auto open url on browser.

```bash
% koko -o -p your/document/root
document root : your/document/root
[listen 4797]
[open http://172.0.0.1:4797]
```

use -o with argument, Koko open url with path on browser.

```bash
% koko -o default.html -p your/document/root
document root : your/document/root
[listen 4797]
[open http://172.0.0.1:4797/default.html]
```

### proxy

with -u (--url), Koko work as proxy server for url.

```bash
% koko -u http://fnobi.com/
document root : your/document/root
proxy : fnobi.com:80
[listen 6022]
```
