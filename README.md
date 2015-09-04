# openssl-exports
prebuilt binaries for openssl

#Built with openssl 1.0.1p release!
#how to build linux-arm-a9s-release built on Ubuntu 12.04x64
make clean
./Configure dist no-shared no-ssl2 -fPIC --prefix=`pwd`/../openssl-exports/linux-arm-a9s-release
make CC=/opt/BUILD_TOOLS/arm-a9s/bin/arm-linux-gnueabihf-gcc LD=/opt/BUILD_TOOLS/arm-a9s/bin/arm-linux-gnueabihf-ld STRIP=/opt/BUILD_TOOLS/arm-a9s/bin/arm-linux-gnueabihf-strip AS=/opt/BUILD_TOOLS/arm-a9s/bin/arm-linux-gnueabihf-as NM=/opt/BUILD_TOOLS/arm-a9s/bin/arm-linux-gnueabihf-nm RANLIB=/opt/BUILD_TOOLS/arm-a9s/bin/arm-linux-gnueabihf-ranlib
make install

#Built with openssl 1.0.1p release!
#how to build linux-arm-a9s-debug built on Ubuntu 12.04x64
make clean
./Configure dist no-shared no-ssl2 -fPIC --prefix=`pwd`/../openssl-exports/linux-arm-a9s-debug
make CC=/opt/BUILD_TOOLS/arm-a9s/bin/arm-linux-gnueabihf-gcc LD=/opt/BUILD_TOOLS/arm-a9s/bin/arm-linux-gnueabihf-ld STRIP=/opt/BUILD_TOOLS/arm-a9s/bin/arm-linux-gnueabihf-strip AS=/opt/BUILD_TOOLS/arm-a9s/bin/arm-linux-gnueabihf-as NM=/opt/BUILD_TOOLS/arm-a9s/bin/arm-linux-gnueabihf-nm RANLIB=/opt/BUILD_TOOLS/arm-a9s/bin/arm-linux-gnueabihf-ranlib
make install


