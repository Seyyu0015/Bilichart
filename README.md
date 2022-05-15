# 直播观众贡献排行榜（哔哩哔哩）
## 简介
这是一款OBS用直播插件。  
能够连接到Bilibili直播间，对直播间观众的互动行为进行量化统计并排名，之后以《我的世界》风格展示给观众。  
![OBS内效果](https://user-images.githubusercontent.com/103107612/167257703-1c2f0aa7-ef76-4675-ad16-22aa8343eacb.png)  
## 使用效果展示  
 哔哩哔哩：https://www.bilibili.com/video/BV1jr4y1t71Q/  
## 如何使用插件
![输入id](https://user-images.githubusercontent.com/103107612/167257797-88d416ea-b11e-4040-8a75-d351af61d289.png)  
1. 在“config.py”文件中配置直播间ID  
2. 打开“style.css”文件，复制全部内容  
3. 打开OBS 添加“浏览器源” 勾选本地文件并选择“display_html.html”文件   
    - 宽度： 740  
    - 高度： 97  
    - 自定义css：粘贴（第2步中复制的内容）  
4. 点击“确定”插件就会出现在舞台内  
5. 运行“main.py”  
## 配置文件
* roomid： 直播间id，程序会连接到该直播间  
* rank_add_by_danmu： 每发送一个弹幕所增加的贡献值  
* price： 礼物价值和增加贡献的比值（金瓜子：贡献）  
* free_gift： 免费礼物增加的贡献值,0 为不增加  
* number：排行榜显示个数  
## 其他  
* 可能因为爬取头像过于频繁导致暂时无法获取头像，数小时后恢复  
* “运行”中会输出更详细的排名信息  
* 可以从“config.py”中分别配置每条弹幕和免费礼物增加的贡献值  
![运行中输出](https://user-images.githubusercontent.com/103107612/167257982-18849e35-c38d-4e50-acd2-0bac44809ef6.png)
