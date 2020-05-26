## Сборка deb пакета: ```fakeroot dpkg-deb --build (folder name)```

##  Зависимости (при установке через apt установятся автоматически):

- ### libsdl2-2.0-0

- ### libsdl2-mixer-2.0-0

- ### libsdl2-ttf-2.0-0

- ###  libsdl2-image-2.0-0

- ### libgl1-mesa-dev

## Уже собранный пакет можно скачать здесь: [sourceforge](https://sourceforge.net/projects/hse-settlers-of-catan/files/)

- ###  ```$ sudo apt install ./Catan_1.0_all.deb``` — установить

- ### ```$ catan``` — запустить

- ###  ```$ sudo apt remove catan``` — удалить

## Запуск в Docker:

```
$ xhost local:root
$ sudo docker run -e DISPLAY=unix$DISPLAY -v /tmp/.X11-unix:/tmp/.X11-unix -it -v /dev/snd:/dev/snd --privileged ubuntu:18.04
$ apt-get update
$ cd home
$ wget https://sourceforge.net/projects/hse-settlers-of-catan/files/Catan_1.1_x64.deb
$ apt install ./Catan_1.1_x64.deb
$ catan
```
