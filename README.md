# Tony's Snake 3.0.3

### 介绍
  一款基于贪吃蛇的小游戏, 加入了多种有特殊效果的食物, 可以控制蛇向八个方向移动.
  
  这是本系列游戏的第三版, 使用了 EasyX 的图形库, 并添加音效.
  
  此程序是对绘图和鼠标操作的进一步练习, 是对多态与类继承的初步学习.

### 环境
  VC++6.0
  
  EasyX 2018 春分版

### 文件
  startup.h -- 一些全局变量
  
  startup.cpp -- 游戏主程序
  
  game.h -- 常量定义, 与游戏信息类
  
  info.cpp -- 游戏信息处理, 读取外部数据, 用于设置
  
  element.h -- 游戏元素基类定义, 蛇类, 食物类均继承此类
  
  element.cpp -- 基类的实现
  
  snake.cpp -- 蛇类的实现
  
  food.cpp -- 食物类的实现
  
  interface.h -- 界面类定义
  
  interface.cpp -- 界面类实现

### 玩法
  游戏共有 4 种难度, 可以在设置界面中更改. 不同难度蛇的速度, 初始长度, 食物出现频率与属性有区别.
  
  WASD 向基本的四个方向移动, QECZ 向额外的四个方向移动.
  
  移动方向, 特殊食物的出现, 是否可以穿墙也可以在设置界面更改.
  
  只有吃掉普通食物才会更新食物.
  
  由于测试时间有限, 对于游戏数据的不合理之处, 如速度, 效果持续时间等, 可自行在"RESOURCES\DATA"下更改.
  
  用记事本打开前缀为"DIF_"的文件即可修改, 后面的单词与难度对应.
### 不足
  蛇的移动速度并没有随长度增加而加快.
  
  游戏音效可能会有延迟.
  
  代码实现有些笨拙.

### 一直不清楚的问题
  我使用 PlaySound() 播放音效, 在惠普的笔记本上运行程序时, 总会有一点点延迟. 而在打开任意音乐播放软件听音乐时, 就没有延迟了. 这是为什么?
