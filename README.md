# ロボットシステム学
--------

## 実験内容
Raspberry Pi4 を使用し、LEDの点灯消灯を操作する。

-------

## 使用機器
・LED ×3

・ジャンパー線 ×6

・抵抗 ×3

・ブレッドボード

・Raspberry Pi4

------

## 環境
・Ubuntu 20.04 server

-------

## インストール方法
　　　　　　
 リポジトリをクローンする。
                ＄git clone https://github.com/yuma850/robotsystem1.git

　　　　　       ＄cd myled
     
                  $make
     
 　　　　インストールする。
          $sudo insmod myled.ko
          
          だれでも使えるゆようｂする。
          sudo chmod 666 /dev/myled
