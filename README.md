# ロボットシステム学
--------

## 概要
デバイスドライバについて理解を深めると同時に、著作権やライセンスについても理解を深めるという目的のために、実際にRaspberry Pi4 を使用し、LEDの点灯消灯を操作するという実験を行った。

-------

## 使用機器
・Raspberry Pi4

・LED ×3

・ジャンパー線 ×6

・抵抗 ×3

・ブレッドボード

------

## 環境
・Ubuntu 20.04 server

-------

## 実際に実験を行うために必要なプログラムの準備
-------
### インストール方法
　　
    
    ＄ git clone https://github.com/yuma850/robotsystem1.git      //リポジトリをクローンする。
          
    ＄ cd myled                                                   //myledのディレクトリに移動する。
          
    ＄ make                                                       //コンパイルする。
          
    ＄ sudo insmod myled.ko　　　　　　　　　　　　　　　　　　　　//myledをインストールする。
          
    ＄ sudo chmod 666 /dev/myled                                  //だれでも操作できるようにする。
          
 ### LED(プログラム)の操作方法
 
 #### LED1を消す時
    ＄ echo 0 >/dev/myled0
    
 #### LED1をつける時
    ＄ echo 1 >/dev/myled0
    
 #### LED2を消す時
    ＄ echo 2 >/dev/myled0
    
 #### LED2をつける時
    ＄ echo 3 >/dev/myled0
    
  #### LED2を消す時
    ＄ echo 4 > /dev/myled0
    
  #### LED1をつける時
    ＄ echo 5 >/dev/myled0

### アンインストール方法

    ＄ sudo rmmod myled
-----

## 実際に行っている動画
https://youtu.be/NzFWBAQKTe8


## ライセンス
GNU General Public License v3.0

詳細は以下のリンクから確認可能

https://github.com/yuma850/robotsystem1/blob/be00a7d848222e42bcfa2d4b9dc4224beb8eda73/LICENSE

-----
 
