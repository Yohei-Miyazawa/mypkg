## Robot-system
千葉工業大学　未来ロボティクス学科４S

ロボットシステム学　課題2

## 概要
上田准教授が講義で作成したコードを自分で動かし、ライセンスを整備したものである

上田准教授のROSのパッケージの作成動画：https://www.youtube.com/watch?v=PL85Pw_zQH0　

## 環境
ハードウェア

・Raspberry Pi4 ModelB

ソフトウェア

・Ubuntu20.04

・ROS Noetic

## デモ

デモ動画：https://youtu.be/pT44ypUNl1w　

## 実行準備

・ ROS インストール方法

上田准教授の https://github.com/ryuichiueda/ros_setup_scripts_Ubuntu20.04_server において
```
$ ./step0.bash
$ ./step1.bash
```
を実行することでインストールすることが出来る

・ ワークスペースの準備
```
$ mkdir -p catkin/src
$ cd ~/catkin_ws/src
$ catkin_init_workspace
```

・ パッケージのインストール方法
```
$ cd ~/catkin_ws/src
$ git clone https://github.com/Yohei-Miyazawa/mypkg.git
```

・ パッケージのビルド
```
$ cd ~/catkin_ws
$ catkin_make
$ source ~/.bashrc
```

## 実行

端末を4つ用意し以下のコマンドを打ち込む

端末1
```
$ roscore
```

端末2
```
$ rosrun mypkg count.py
```

端末3
```
$ rosrun mypkg twice.py
```

端末4
```
$ rostopic echo /twice
```

端末4からデータを取り出すことが出来た

## ライセンス

このリポジトリには以下のライセンスが付与されている

BSD 3-Clause License







