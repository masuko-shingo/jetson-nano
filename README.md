# Jetson Nano
自分用jetsonnanoの記録  
Turltebot3とJetsonNanoを用いた教材のドキュメント  

#### なぜJetsonNanoを使うか(変更した理由)
* GPUが搭載され、深層学習等に用いやすい
* ロボット機体がturtlebot3ベースで変更前の制御回路がlinux準拠のRaspberryPiのため、搭載しやすい
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
(使う機材や環境をまとめた表を載せる）

### 構成
ハードウェア構成図
ソフトウェア構成図
## 環境構築
Jetsonnano環境構築  
https://github.com/masuko-shingo/jetson-nano/wiki/Jetsonnano%E7%92%B0%E5%A2%83%E6%A7%8B%E7%AF%89

## 実習のドキュメント
はじめに：

実習：Turtlebot3のシステムを動かす(SLAM, Navigation)  
https://github.com/masuko-shingo/jetson-nano/wiki/Turtlebot3%E3%81%AE%E3%82%B7%E3%82%B9%E3%83%86%E3%83%A0%E3%82%92%E5%8B%95%E3%81%8B%E3%81%99(SLAM,-Navigation)

実習：画像認識，物体検出(YOLOv3)  
https://github.com/masuko-shingo/jetson-nano/wiki/%E5%AE%9F%E7%BF%92%EF%BC%9A%E7%94%BB%E5%83%8F%E8%AA%8D%E8%AD%98%EF%BC%8C%E7%89%A9%E4%BD%93%E6%A4%9C%E5%87%BA(YOLOv3)
