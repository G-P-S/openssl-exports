# openssl-exports
prebuilt binaries for openssl

#how to build linux-arm-a9s-release built on Ubuntu 12.04x64
./Configure dist --prefix=`pwd`/../openssl-exports/linux-arm-a9s-release
make CC=/opt/BUILD_TOOLS/arm-a9s/bin/arm-linux-gnueabihf-gcc LD=/opt/BUILD_TOOLS/arm-a9s/bin/arm-linux-gnueabihf-ld STRIP=/opt/BUILD_TOOLS/arm-a9s/bin/arm-linux-gnueabihf-strip AS=/opt/BUILD_TOOLS/arm-a9s/bin/arm-linux-gnueabihf-as NM=/opt/BUILD_TOOLS/arm-a9s/bin/arm-linux-gnueabihf-nm RANLIB=/opt/BUILD_TOOLS/arm-a9s/bin/arm-linux-gnueabihf-ranlib
make install

#how to build linux-arm-a9s-debug built on Ubuntu 12.04x64
./Configure dist --prefix=`pwd`/../openssl-exports/linux-arm-a9s-debug
make CC=/opt/BUILD_TOOLS/arm-a9s/bin/arm-linux-gnueabihf-gcc LD=/opt/BUILD_TOOLS/arm-a9s/bin/arm-linux-gnueabihf-ld STRIP=/opt/BUILD_TOOLS/arm-a9s/bin/arm-linux-gnueabihf-strip AS=/opt/BUILD_TOOLS/arm-a9s/bin/arm-linux-gnueabihf-as NM=/opt/BUILD_TOOLS/arm-a9s/bin/arm-linux-gnueabihf-nm RANLIB=/opt/BUILD_TOOLS/arm-a9s/bin/arm-linux-gnueabihf-ranlib
make install
