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
　　　　　　
             git clone https://github.com/yuma850/robotsystem1.git      //リポジトリをクローンする。

　　　　　    cd myled
     
              make
     
              sudo insmod myled.ko         //インストールする。
         
              sudo chmod 666 /dev/myled　　//だれでも使えるようにする。
          
 ## LEDの操作方法
             echo 0 >/dev/myled0
             echo 1 >/dev/myled0
             echo 2 >/dev/myled0
             echo 3 >/dev/myled0
             echo 4 > /dev/myled0
             echo 5 >/dev/myled0
0から5までで、３つのLEDを点灯消灯させる。

## アンインストール方法
              sudo rmmod myled
              
## ライセンス

 
