# Dyalog docker image with .netcore support
**Note:**
Dyalog APL 18.0 is needed.
## Linux
### Build docker image
```docker
docker build -t l_dya18_netcore3_0  --build-arg  DYALOG_DEB_PKG=linux_64_18.0.37886_unicode.x86_64.deb . 
```
where docker argument **DYALOG_DEB_PKG** is just a Dyalog Debian package. 

### Run image
```docker
docker run -it -p 4502:4502  l_dya18_netcore3_0
```

and access over RIDE and try:
```apl
      ⎕USING←'System'
      DateTime.Now
2/27/2020 12:55:33 PM

```


