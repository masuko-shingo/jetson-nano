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
[参考書籍]：Ubuntuスタートアップバイブル  
https://www.amazon.co.jp/Ubuntu%E3%82%B9%E3%82%BF%E3%83%BC%E3%83%88%E3%82%A2%E3%83%83%E3%83%97%E3%83%90%E3%82%A4%E3%83%96%E3%83%AB-%E5%B0%8F%E6%9E%97-%E6%BA%96/dp/4839964866

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
![電気配線回路ブロック図(ハード)](https://user-images.githubusercontent.com/72721963/150422835-86211800-9806-4cfd-a970-539c2638760d.png)


<!--
ソフトウェア構成図
-->
## 環境構築
Jetsonnano環境構築  
https://github.com/masuko-shingo/jetson-nano/wiki/Jetsonnano%E7%92%B0%E5%A2%83%E6%A7%8B%E7%AF%89

## 実習のドキュメント
はじめに  
https://github.com/masuko-shingo/jetson-nano/wiki/%E3%81%AF%E3%81%98%E3%82%81%E3%81%AB  
実習：Turtlebot3のシステムを動かす(SLAM, Navigation)  
https://github.com/masuko-shingo/jetson-nano/wiki/%E5%AE%9F%E7%BF%92%EF%BC%9ASLAM,-Navigation(Turtlebot3)

実習：画像認識，物体検出(YOLOv3)  
https://github.com/masuko-shingo/jetson-nano/wiki/%E5%AE%9F%E7%BF%92%EF%BC%9A%E7%89%A9%E4%BD%93%E6%A4%9C%E5%87%BA(YOLOv3)
