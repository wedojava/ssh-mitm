# Preparetion for install AppArmor

## Download

```
wget http://ftp.gnu.org/gnu/automake/automake-1.15.tar.gz
wget http://gnu.askapache.com/libtool/libtool-2.4.6.tar.gz
wget https://www.python.org/ftp/python/3.7.6/Python-3.7.6.tar.xz
wget http://ftp.gnu.org/gnu/glibc/glibc-2.25.tar.gz
wget ftp://gcc.gnu.org/pub/gcc/infrastructure/gmp-4.3.2.tar.bz2
wget ftp://gcc.gnu.org/pub/gcc/infrastructure/mpfr-3.1.4.tar.bz2
wget ftp://gcc.gnu.org/pub/gcc/infrastructure/mpc-1.0.3.tar.gz
wget http://ftp.tsukuba.wide.ad.jp/software/gcc/releases/gcc-6.3.0/gcc-6.3.0.tar.gz
wget https://sourceforge.net/projects/pcre/files/pcre/8.41/pcre-8.41.tar.gz
wget https://github.com/swig/swig/archive/rel-4.0.1.tar.gz
```

## Install from source

Ordinary command:

```
tar zxf foobar.tar.gz
cd foobar
./configure
make
make install
```

Spacial condition:

```
tar jxf mpfr-3.1.4.tar.bz2
tar jxf gmp-4.3.2.tar.bz2
./configure
make
make install
```

```
tar zxf swig-4.0.1
cd swig-4.0.1
./autogen.sh
./configure --without-pcre
make
```

Python:
```
xz Python-3.7.6.tar.xz
tar xf Python-3.7.6.tar
cd Python-3.7.6
./configure --enable-optimizations
make
make install
```

# Apparmor
```
sh ./autogen.sh
```
