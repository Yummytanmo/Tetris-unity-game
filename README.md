# Tetris-unity-game
游戏软件有macos、windows两个版本，macos直接打开该APP即可开始游戏，windows打开文件夹中的Tetris.exe文件开始游戏。

![image](https://github.com/user-attachments/assets/dd9fe20a-0a4d-4ce1-9904-c8614d7d67da)
![image](https://github.com/user-attachments/assets/9616059c-472e-4406-984d-b126ed3ff9d8)

游戏具有两个场景，游戏启动场景和游戏游玩场景：

![image](https://github.com/user-attachments/assets/7dea477d-c856-4202-939d-81083bae3215)


点击游戏软件，进入开始界面，同时会播放主题音乐：

![image](https://github.com/user-attachments/assets/921aa143-35ef-4d73-94b3-b85d50c67041)


点击Go按钮即可开始游戏，进入游戏界面，生成第一个方块，开始播放默认背景音乐：

![image](https://github.com/user-attachments/assets/9ca6ee41-f3fd-4d23-bfcb-649af612e386)


游戏界面主体是方块游戏区域、UI界面，游戏区域四周为游戏边框，方块无法超过边框，UI界面包括上方的Best最高游戏得分面板、Score当前游戏得分面板，右侧Harder增加游戏难度按钮、More菜单按钮，左侧ClickMe光源切换按钮、Restart重新开始按钮。
此时按照俄罗斯方块游戏玩法开始游戏，使用WASD或者上下左右方向键控制方块。AD和左右方向键控制方块左右移动，点按一次移动一个网格，长按按键一段延迟后会持续在该方向上移动；W和上方向键控制方块旋转，每次按下方块整体会逆时针旋转90°；S和下方向键控制方块加速，按下该按键即可让方块加速下落。
当有一行被填满时，该行就会消除，游戏当前得分会增加，显示增加动态动画，并播放消除音效，若打破最好记录，会播放打破纪录音效。
当游戏失败时，会播放失败音效，停止BGM播放，同时游戏失败UI渐入：

![image](https://github.com/user-attachments/assets/eb53ae82-8fa7-492f-a9af-0bd2e16cf11d)


UI按钮功能：
Restart按钮（空格键）：当游戏失败时，或游戏中希望重新开始游戏时，可以按下Restart按钮或空格键，游戏结束UI会渐出，游戏会重新开始，继续播放BGM；
Harder按钮：每次按下Harder按钮方块下落速度都会增加，同时背景明度增加，点按一次效果不明显，但是若玩家不断按下Harder按钮，就会发现方块速度明显变快，并且背景出现颜色，并且颜色还会不断变化，给玩家一个新奇的体验；

![image](https://github.com/user-attachments/assets/151a06cf-8fa2-4f65-97ff-bd9987b3917e)
![image](https://github.com/user-attachments/assets/dcd64090-bcd7-4f72-bb12-9f393e9b225f)

 
ClickMe按键：该按键对游戏内容没有特殊影响，但是点击可以切换光源是否运动的状态，点击时光源会开始运动模拟昼夜变化，背景上出现阴影变化；

![image](https://github.com/user-attachments/assets/52b87013-59ed-4837-863f-0bd47d48880c)
![image](https://github.com/user-attachments/assets/0bf28647-937b-4c24-bab0-e180645366ef)


More按键：More按键会打开菜单界面，再次点击会关闭菜单界面，打开菜单界面的同时会暂停游戏，方块不会再运动，关闭时游戏恢复正常；

![image](https://github.com/user-attachments/assets/9a64148e-2d8f-4a2a-9376-19718d726c66)


Best面板按钮：点击Best显示历史最高得分面板，会清除历史最高得分，显示清除的文本特效;
菜单UI按钮：
Exit按钮：点击Exit按钮可以退出游戏；
ChangeBGM按钮：点击可以切换预设的不同BGM音乐；
About按钮：点击About按钮会跳转该项目上传的github链接；
