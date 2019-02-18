<p align=center><img src=https://emojipedia-us.s3.dualstack.us-west-1.amazonaws.com/thumbs/320/apple/155/gear_2699.png width=120px></p>
<h1 align=center>nginx (Docker image)</h1>
<p align=center>Built-from-source container image of the <a href=https://nginx.org/>NGINX HTTP server</a></p>

Available at [`ricardbejarano/nginx`](https://hub.docker.com/r/ricardbejarano/nginx).


## Features

* Super tiny (only `13.7MB`)
* Built from source, including libraries
* Based on `scratch`, see the [Filesystem](#Filesystem) section below for an exhaustive list of the image's contents
* Included [TLS1.3](https://tools.ietf.org/html/rfc8446) protocol support (with [OpenSSL](https://www.openssl.org/))
* Included [brotli](https://github.com/google/brotli) compression support (with [ngx_brotli](https://github.com/google/ngx_brotli))


## Filesystem

The image's contents are:

```
/
├── etc/
│   ├── group
│   ├── nginx/
│   │   ├── html/
│   │   │   ├── 50x.html
│   │   │   └── index.html
│   │   ├── mime.types
│   │   └── nginx.conf
│   └── passwd
├── lib/
│   └── x86_64-linux-gnu/
│       ├── ld-linux-x86-64.so.2
│       ├── libc.so.6
│       ├── libnss_files.so.2
│       ├── libnss_dns.so.2
│       └── libresolv.so.2
├── nginx
└── tmp/
```

## License

See [LICENSE](https://github.com/ricardbejarano/nginx/blob/master/LICENSE).
