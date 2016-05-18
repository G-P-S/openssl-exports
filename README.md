# openssl-exports
prebuilt binaries for openssl 1.0.2h

#Built with openssl 1.0.2h release!
#how to build linux-arm-a9s-release built on Ubuntu 12.04x64
make clean
./Configure linux-armv4 no-ssl2 no-ssl3 -fPIC threads shared --cross-compile-prefix=/opt/BUILD_TOOLS/arm-a9s/bin/arm-linux-gnueabihf- --prefix=`pwd`/../openssl-exports/linux-arm-a9s-release
make 
make install

#Built with openssl 1.0.2h debug!
#how to build linux-arm-a9s-debug built on Ubuntu 12.04x64
make clean
./Configure linux-armv4 no-ssl2 no-ssl3 -fPIC threads shared --cross-compile-prefix=/opt/BUILD_TOOLS/arm-a9s/bin/arm-linux-gnueabihf- --prefix=`pwd`/../openssl-exports/linux-arm-a9s-debug
make 
make install


#Built with openssl 1.0.2h release!
#how to build linux-x64-release built on Ubuntu 12.04x64
make clean
./config shared no-ssl2 no-ssl3 -fPIC threads --prefix=`pwd`/../openssl-exports/linux-x64-release
make 
make install

#Built with openssl 1.0.2h debug!
#how to build linux-x64-debug built on Ubuntu 12.04x64
make clean
./config shared no-ssl2 no-ssl3 -fPIC threads --prefix=`pwd`/../openssl-exports/linux-x64-debug
make 
make install
