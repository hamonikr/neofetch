<h3 align="center"><img src="https://i.imgur.com/ZQI2EYz.png" alt="logo" height="100px"></h3>
<p align="center">A command-line system information tool written in bash 3.2+</p>

<p align="center">
<a href="./LICENSE.md"><img src="https://img.shields.io/badge/license-MIT-blue.svg"></a>
<a href="https://github.com/dylanaraps/neofetch/releases"><img src="https://img.shields.io/github/release/dylanaraps/neofetch.svg"></a>

This project origin is https://github.com/dylanaraps/neofetch


Neofetch는 터미널에서 시스템의 정보를 모두 보여주는 도구입니다. (`bash 3.2+`)

* 이 저장소는 하모니카 4.0 에 적합한 정보를 보여주도록 수정된 버전입니다.

![neofetch](docs/neofetch-hamonikr.png)


## How to build debian package on HamoniKR
```
git clone git@github.com:hamonikr/neofetch.git
mv neofetch neofetch-7.0.0-1+hamonikr2
cd neofetch-7.0.0-1+hamonikr2
dh_make --createorig -i -c gpl3
TYPE y
mv ../neofetch-7.0.0_1+hamonikr2.orig.tar.xz neofetch_7.0.0.orig.tar.xz
dpkg-buildpackage --sign-key=9FA298A1E42665B8
