# Jetson Nano
自分用jetsonnanoの記録するリポジトリ  
Turltebot3とJetsonNanoを用いた教材のドキュメント  

#### なぜJetsonNanoを使うか(変更した理由)
* GPUが搭載され、深層学習等に用いやすい
* turltebot3ベースのロボット機体なので，変更前の制御回路RaspberryPiと同じくlinux準拠かつ，搭載しやすいサイズ
* 身近で一番普及しているもので構成した

## はじめに
#### どんなことを学ぶか
linux、ubuntuをある程度使えるようになり、自律移動やnavigationが扱えるようになる.  
加えて物体認識など深層学習を用いた技術を扱える、開発できるようになる.

※linux,ubuntuに慣れてない方は参考文献に記載されている書籍等を読みながら進めると良いと思います。  
[参考]：
#### どんな過程で
JetsonNanoのセットアップを行うことや、turtlebot3のSLAMやnavigationのシステムを動かしながら理解する。  
YOLO等を通して、深層学習を用いた物体認識について動かしながら理解する。


## 環境
今回使う環境は以下の通りです。  

ハードウェア構成表
| Item | Model | Quantiny |
| :--- | :---: | :---: |
| Base Robot | Tutlebot3 | 1 |
| Actuators | DYNAMIXEL XL430-W250 | 2 |
| Battery | LI-PO Battery 11.1V 1800mAh | 1 |
| Lidar | LDS-01(HLS-LFCD2) | 1 |
| SBC | OpenCR 1.0 | 1 |
|  | Jetson Nano Developer Kit a02 | 1 |
| Camera | Microsoft LifeCam HD5000 7ND-00006 | 1 |
| WiFi Dongle | TP-Link TL-WN725N | 1 |

配線図  
![OV-electrical-circuits](https://user-images.githubusercontent.com/72721963/149656563-da94c3ae-b666-449d-8ca7-84106d417e76.png)

ソフトウェア構成図
## 環境構築
Jetsonnano環境構築  
https://github.com/masuko-shingo/jetson-nano/wiki/Jetsonnano%E7%92%B0%E5%A2%83%E6%A7%8B%E7%AF%89

## 実習のドキュメント
はじめに  
https://github.com/masuko-shingo/jetson-nano/wiki/%E3%81%AF%E3%81%98%E3%82%81%E3%81%AB  
実習：Turtlebot3のシステムを動かす(SLAM, Navigation)  
https://github.com/masuko-shingo/jetson-nano/wiki/%E5%AE%9F%E7%BF%92%EF%BC%9ASLAM,-Navigation(Turtlebot3)

実習：画像認識，物体検出(YOLOv3)  
https://github.com/masuko-shingo/jetson-nano/wiki/%E5%AE%9F%E7%BF%92%EF%BC%9A%E7%94%BB%E5%83%8F%E8%AA%8D%E8%AD%98%EF%BC%8C%E7%89%A9%E4%BD%93%E6%A4%9C%E5%87%BA(YOLOv3)
