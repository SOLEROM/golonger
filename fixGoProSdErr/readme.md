# untrack orig

* https://github.com/ponchio/untrunc

```
wget https://libav.org/releases/libav-12.3.tar.xz
wget https://github.com/ponchio/untrunc/archive/master.zip
unzip master.zip

tar -xJf libav-12.3.tar.xz -C untrunc-master

cd untrunc-master/libav-12.3/
./configure
make
cd ..

 g++ -o untrunc -I./libav-12.3 file.cpp main.cpp track.cpp atom.cpp mp4.cpp -L./libav-12.3/libavformat -lavformat -L./libav-12.3/libavcodec -lavcodec -L./libav-12.3/libavresample -lavresample -L./libav-12.3/libavutil -lavutil -lpthread -lz -lX11 -lvdpau -ldl

```


# working fork

* https://github.com/anthwlock/untrunc

```
sudo apt-get install libavformat-dev libavcodec-dev libavutil-dev
git clone https://github.com/anthwlock/untrunc.git .
make
```
