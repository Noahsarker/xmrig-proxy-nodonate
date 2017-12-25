# XMRig Proxy without donate
XMRig Proxy с полность удалённым донатом

## Usage


sudo apt install git build-essential cmake libuv1-dev uuid-dev libmicrohttpd-dev

git clone https://github.com/xmrig/xmrig-proxy.git

git clone https://github.com/xoste49/xmrig-proxy-nodonate.git

patch -p0 < xmrig-proxy-nodonate/xmrig-proxy.patch

cd xmrig-proxy && mkdir build && cd build

cmake .. && make

rm -r CM* && rm -r Makefile && rm -r cmake_install.cmake

cp ../src/config.json .