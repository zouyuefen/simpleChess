#version 0.0.3
1. 房间里面增加角色.(NOT DONE)
2. 棋盘会被同步到服务端.
3. 使用日志sl4j-log4J.
4. 修复线上BUG(重复点击会连续向服务器发两条信息)
5. 修复BUG(当屏幕存在滚动条时,显示的坐标位置不正确);

#version 0.0.2
1. 进入房间如果人数超过2人,则不能进入房间
2. 优化前后端数据交互,前后端已JSON作为数据交互.
  ```
    Result{
        succss; #是否成功
        errmsg; #错误信息
        model: #内容
    }
  ```
3. 增加一个守护线程,统计房间数量.
4. 展示上一个棋子下在哪里
5. 离开房间后会减少房间的人数.

##########################################################################################
version 0.0.1
1.增加roomId号，表示房间
  1.1用户进入首页，有两个可能1是创建一个新的房间，2是进入一个已经存在的房间。
2.对战页面增加显示自己是哪个颜色，房间号