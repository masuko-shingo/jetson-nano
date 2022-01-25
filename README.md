# はじめに
<!--
# Jetson Nano

自分用jetsonnanoの記録するリポジトリ  
-->
Turtlebot3とJetsonNanoを用いたロボット教材のドキュメント  

#### なぜTurtlebot3,JetsonNanoを使うか
* GPUが搭載され、深層学習等に用いやすい
* turltebot3ベースのロボット機体，変更前の制御回路RaspberryPiと同じくlinuxOS，搭載しやすいサイズ
* 身近で一番普及しているもので構成した

<!--
近年，自律移動ロボットの需要が増えており，深層学習を利用して，物体認識を行うような技術の開発が急速に進みつつあります．  
自律移動ロボットの例として，Turtlebot3を挙げます．  
Turtlebot3は，オープンソースで開発された，ROSのプラットフォームとなるロボットです．  
2017年に公表され，使用されている国は比較的多いと言えます．そのため，ユーザーが多く情報に富んでいるプラットフォームだと考えられます．  
また，深層学習を利用した技術では，自動運転時，センサからの障害物検知(物体検出)が挙げられます．  
上記のような背景から，これらの先端的な技術を効率良く学べる教材が求められていると考えられます．  
それを踏まえて，ナビゲーションと深層学習を学べる教材としてTurtlebot3とJetsonNanoを使用した教材を開発しました．  
-->
## どんなことを学ぶか
ドキュメントのおおまかな構成として
- linuxOSやCUI(コマンドライン)について  
- 地図生成やナビゲーション(自律移動)について  
- 深層学習，物体検出について  

の3つで構成されています．

※linuxOSやCUIに慣れてない方は参考文献に記載されている書籍等を読みながら進めると良いと思います。  
[参考書籍]：小林 準　Ubuntuスタートアップバイブル　マイナビ
https://www.amazon.co.jp/Ubuntu%E3%82%B9%E3%82%BF%E3%83%BC%E3%83%88%E3%82%A2%E3%83%83%E3%83%97%E3%83%90%E3%82%A4%E3%83%96%E3%83%AB-%E5%B0%8F%E6%9E%97-%E6%BA%96/dp/4839964866

## 到達目標
この教材の到達目標は，  
- linux，CUIの基本操作がある程度使えるようになる．
- 地図生成やナビゲーション(自律移動)が扱えるようになる.  
- 深層学習を用いた物体認識などの技術を扱えるようになる.  

となっています。

## どんな過程で
- ナビゲーション  
<!--
ナビゲーション面については，  
-->
SLAMやナビゲーションのシステムについてTurtlebot3パッケージを動かしながら理解する。  
- 深層学習  
<!--
深層学習については，  
-->
YOLOv3を用いた、データセットの作成，学習，推論(物体検出)を行う実習を通して，深層学習を用いた物体検出について動かしながら理解する。  

という過程で学んでいきます．

## 環境
今回使う環境は以下の通りです。  

### ハードウェア構成表
| Item | Model | Quantiny |
| :--- | :---: | :---: |
| Base Robot | Turtlebot3 | 1 |
| Actuators | DYNAMIXEL XL430-W250 | 2 |
| Battery | LI-PO Battery 11.1V 1800mAh | 1 |
| LiDAR | LDS-01(HLS-LFCD2) | 1 |
| SBC | OpenCR 1.0 | 1 |
|  | Jetson Nano Developer Kit a02 | 1 |
| Camera | Microsoft LifeCam HD5000 7ND-00006 | 1 |
| WiFi Dongle | TP-Link TL-WN725N | 1 |

### 配線図  
![電気配線回路ブロック図(ハード)](https://user-images.githubusercontent.com/72721963/150423909-6bc43ef9-ece2-4a26-af5e-6e294c44b737.png)

### ソフトウェア構成表
| 　| PC | SBC(JetsonNano) |
| :--- | :---: | :---: |
| OS | Ubuntu 18.04 LTS 64bit | JetPack 4.5.1 ( Ubuntu 18.04 ) |
| Middleware (ROS) | ROS(melodic) | ROS(melodic) |
| YOLO | - | YOLOv3(darknet) |

## 環境構築
Jetsonnano環境構築  
https://github.com/masuko-shingo/jetson-nano/wiki/Jetsonnano%E7%92%B0%E5%A2%83%E6%A7%8B%E7%AF%89

## ドキュメント
はじめに  
https://github.com/masuko-shingo/jetson-nano/wiki/%E3%81%AF%E3%81%98%E3%82%81%E3%81%AB  
実習：Turtlebot3のシステムを動かす(SLAM, Navigation)  
https://github.com/masuko-shingo/jetson-nano/wiki/%E5%AE%9F%E7%BF%92%EF%BC%9ASLAM,-Navigation(Turtlebot3%E3%83%91%E3%83%83%E3%82%B1%E3%83%BC%E3%82%B8)

実習：画像認識，物体検出(YOLOv3)  
https://github.com/masuko-shingo/jetson-nano/wiki/%E5%AE%9F%E7%BF%92%EF%BC%9A%E7%89%A9%E4%BD%93%E6%A4%9C%E5%87%BA(YOLOv3)
