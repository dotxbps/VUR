
#  VUR
VUR is a custom xbps-src repo and custom xbps (binaries) repo that includes packages which can not be accepted into [void-packages](https://github.com/void-linux/void-packages/) or removed from it. 

## supported architectures
all packages **must** support `x86_64-glibc` (with exception of *-bin)
- [X] x86_64-glibc
- [ ] x86-64-musl
- [ ] i686-glibc
- [ ] aarch64-glibc
- [ ] aarch64-musl


## using this custom repo to install binaries 

1. sudo touch /etc/xbps.d/10-vur.conf <br><br>
2. put this in the file : repository=https://siduck76.github.io/VUR/generic/ <br><br>
Update your repos<br><br>
3. sudo xbps-install -S


## quick start for compiling ( using template )
`xtools` and `base-devel` are required for building and installing packages
```
xbps-install base-devel xtools
```
clone repo and bootstrap
```
git clone --depth 1 VUR
cd VUR
./xbps-src binary-bootstrap
```
build `pkgname` and install it
```
./xbps-src pkg <pkgname>
xi <pkgname>
````

I liked the idea of AUR on arch but felt it missing somehow on void so I created this and VUR will host/store all stuffs on github itself  and it will be actively moderated/developed . PR's and contributions are always welcome! ( VUR can be used in two ways : use xbps-src to compile packages from vur or just use the binary repo of VUR ).
