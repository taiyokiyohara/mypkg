# mypkg
ロボットシステム学課題２
--- 
# 実装内容
- ロボットシステム学第10回のコードを参考につくりました。
- 5times.pyはcount_up.pyの値をを5倍にして出力します。
---
# 実験器具
- Raspberry Pi4 Model B
- Ubuntu 20.04
- ROS Noetic
---
# 実行方法
``` bash
$ cd catkin_ws/src
$ git clone https://github.com/taiyokiyohara/mypkg.git
$ cd ..
$ catkin_make
```

- 端末1
```bash
$ cd catkin_ws/src/mypkg/scripts/ 
$ roscore
```

- 端末2
```bash
$ cd catkin_ws/src/mypkg/scripts/ 
$ rosrun mypkg count.py
```

- 端末3
```bash
$ cd catkin_ws/src/mypkg/scripts/ 
$ rosrun mypkg 5times.py
```

- 端末4
```bash
$ cd catkin_ws/src/mypkg/scripts/ 
$ rostopic echo /count_up
```

- 端末5
```bash
$ cd catkin_ws/src/mypkg/scripts/ 
$ rostopic echo /fivetimes
```
--- 



