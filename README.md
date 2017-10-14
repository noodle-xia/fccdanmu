# fccdanmu
### 仿fcc弹幕机作业 用于学习
示例一 演示地址：www.nooxia.cn/fccdanmu/111.html

在输入框内输入内容点击发送把用户输入的东西发送到野狗云，野狗是一个实时后端云服务。通过 SDK，野狗向用户提供数据存储和实时通信服务，帮助用户提升应用开发速度。野狗可以很方便的和用户的系统集成，使用户只需要简单的几行代码，就可以实现 app 到服务端的双向实时通信。如果用户没有自己的后端服务器，也可以将野狗作为一站式的后端服务，无需编写后端代码，也无需租用服务器，就可以快速完成应用开发。
```
var ref = new;
 
var ref = new Wilddog("https://<appId>.wilddogio.com/");　//URL作为参数，定位到数据库根节点
```
在www.wildog.com 注册一个账号，创建一个应用，自动生成一个url,替换代码内的url即可 

示例二 演示地址：www.nooxia.cn/fccdanmu/666.html
相关代码注释 
```
<javascript 前端中能做什么
    1.响应用户的操作 事件（键盘事件、鼠标事件）
    2.操作dom元素（增删改查、属性操作、样式等）
    3.数据交互 表单验证 ajax json jsonp 正则表达式
    4.造轮子 mvvm mvc nodeJS jquery

<需求分析
   用户点击发送按钮 把input的内容展示到box里面
   1.元素 .con .send-btn .box span（创建）
   2.事件：点击事件 键盘事件
   3.行为
       1.点击.send-btn获取.con的内容
           (1)规范发送信息
           (2)禁止空及全空格
           (3)存储value值
       2.根据内容动态生成span标签
           (1)创建节点document.createElement
           (2)改变节点内容innerHTML
           (3)节点 生成初始化位置等
           (4)标签添加到oBox appendChild
       3.message运动
           (1)改变元素的left值
           (2)定时器改变 setInterval
           (3)this代表当前弹幕
           (4)弹幕left = 当前left-1
       4.随机函数
           Math.random 0-1 包括0但不包括1
           (1)top
           (2)color
           (3)fontsize
           (4)textShadow
           (5)timing运动曲线
               linear
               ease-out
       5.业务完善
           (1)过去的删除掉
               停止计时器
               删除自身
               终止函数
           (2)完善回车输入
               在oCon上回车 发送弹幕
```
