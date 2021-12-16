# Robottosisutemu

ロボットシステム学2021  課題1
______

# はじめに


 今回使用した、私のRaspberry Pi 4を私以外に佐藤涼耶君も使用しており、課題のmyledやREADMEなどをGitHubにpushするたびにPermission to Daiki414/Robottosisutemu.git denied to Ryoya1012.とErrorを常に出していており調べてもわからず、最終的に佐藤君にGitHub上に貼り付けてもらい、そこから、myledやREADEMEを直接編集させてもらいました。


# 概要


 このプログラムは、講義内で作成したプログラムを参考に佐藤涼耶君に教えてもらいながら自身で改造し、LEDを点灯・消灯を行うプログラムです。


# 動作環境


|OS| Ubuntu20.04server |
---|---
|Hardware|Raspberry Pi 4|


# 使用するもの


・Raspberry Pi 4

・ブレッドボード

・ジャンパーワイヤー ×４

・LED(赤・黄)　×2

・抵抗200Ω ×２


# 回路


・今回、製作した回路の写真です。

<img src=
"https://user-images.githubusercontent.com/95708047/146393574-ff90f7f0-df81-4fb9-8d9c-1a060a62a350.jpg" 
width="320px">



# インストール・ビルド方法


  ・インストール手順
  
     $ git clone http://github.com/Daiki414/Robottosisutemu.git
 
     $ cd Robottosisutemu

     $ make

     $ sudo insmod myled.ko

     $ sudo chmod 666 / dev/myled
     
  ・実行手順
  
     $ echo 0 > /dev/myled0l
         （ledを点灯）
     
     $ echo 1 > /dev/myled0l
         （ledを消灯）
         
     $ echo 2 > /dev/myled0l
         （led1を点灯）
     
     $ echo 3 > /dev/myled0l
     　　（led1を消灯）
     
   ・終了の際は
   
     $ sudo rmmod myled
  



# 実行結果

以下のリンクからyoutubeの動画がご覧できます


https://youtube.com/shorts/P4NYrSSYEhY?feature=share

