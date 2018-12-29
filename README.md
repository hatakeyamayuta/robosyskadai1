# 2018ロボットシステム学課題1
## 動作説明
 自作デバイスドライバによりRaspberryPi3B+のGPIOを操作することでLEDを点滅させる <p> 
動画

### 動作環境

|||
|:--:|:--:|
|Raspberry Pi|Raspberry Pi Model 3B+|
|OS| Ubuntu16.04|
## 回路説明
* GPIO25とGNDの間にLEDを接続
  * GPIO25: 22番ピン
  * GND: 39番ピン

## インストール方法
```
$ git clone https://github.com/hatakeyamayuta/robosyskadai1.git
$ cd robosyskadai1
$ make
$ ./setup.sh
```
### 実行方法
```
$ echo 1 > /dev/myled0
```
### デバイスドライバのアンインストール
```
$ sudo rmmod myled
```
