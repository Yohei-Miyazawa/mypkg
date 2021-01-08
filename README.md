# Robot-system
千葉工業大学　未来ロボティクス学科４S

ロボットシステム学　課題2

# 概要
上田准教授が講義で作成したコードを自分で動かし、ライセンスを整備したものである

上田准教授のROSのパッケージの作成動画：https://www.youtube.com/watch?v=PL85Pw_zQH0　

# 環境
ハードウェア

・Raspberry Pi4 ModelB

ソフトウェア

・Ubuntu20.04

・ROS Noetic

# ROS インストール方法

上田准教授の https://github.com/ryuichiueda/ros_setup_scripts_Ubuntu20.04_server において
```
$ ./step0.bash
$ ./step1.bash
```
を実行することでインストールされる


# 実行方法

### ワークスペースの準備
```
$ mkdir -p catkin/src
$ cd ~/catkin_ws/src
$ catkin_init_workspace
```



