# Zhananbot
这是一个基于skript和miraimc的Java版多功能机器人  

## 如果大家有好功能欢迎提交issues

### 目前功能

>1.支持加群自动审批，只要玩家输入指定的答案，机器人即可自动审核通过  
>2.玩家加群后即可获得消息提醒  
>3.玩家可以在群里绑定(不绑定不允许进服)
>>用法:  
>>在群中输入#bind 你的id即可
>>例:  
>>我的id是Zhanan  在群内输入#bind Zhanan即可
>>>注意:  
>>>1.一个id和QQ号只可以绑定一次  
>>>2.绑定后会自动更改群玩家昵称为[×]xxxx  
>>>3.必须确保机器人拥有管理员权限  

>4.引用api,支持聊天
>>用法:  
>>在群发送“@机器人 你要说的话”即可  
>>5.支持群消息自动转发到服务器  
>>6.服务器聊天自动发送到群聊  
>>7.支持群内使用指令(如果您是管理员/群主)



### 依赖下载
>1.下载skript最新版[点我下载](https://github.com/SkriptLang/Skript/releases)
>2.下载Skript-reflect[点我下载](https://github.com/TPGamesNL/skript-reflect/releases)
>3.下载skUtilities[点我下载](https://github.com/tim740/skUtilities/releases)
>4.下载skript-yaml[点我下载](https://github.com/Sashie/skript-yaml/releases)
>5.下载miraimc[点我下载](https://github.com/DreamVoid/MiraiMC/releases)

### 如何使用
>1.下载上面全部插件  
>2.运行一次所有插件  
>3.找到服务器根目录下的"plugins/Skript/script",把下载到的ZhananBot.sk文件放到该文件夹里  
>4.在控制台输入'skript reload ZhananBot.sk'  
>5.运行以后会在"plugins\ZhananBot"文件夹内找到config.yml文件，双击打开，根据注释编辑即可  
>6.使用Miraimc登陆进QQ账号，<font color=red>注意:登陆账号的QQ号，应该和config文件夹内的Bot_Account保持一致</font>

### TO DO
1.支持群服消息互通  
2.支持群输入指令  
3.支持#help等更多群指令  
4.未来无限可能  

---

# 优化
- ***优化了玩家进服提示语***
- ***优化了未绑定账号踢出服务器时机器人必须在线***
- ***优化了消息转换功能***
<br>

---

# 新增
- ***新增入群审核***
   - 进入群聊自动禁言
   - 禁言后玩家需要加机器人为好友并输入“审核”
   - 审核通过后会计算玩家分数
   - 若通过自动解除禁言
   - 反之则需要手动审核
   - $\color{red} {注意：此功能仅为测试版,需要等待过几日的更新才可正式使用}$
- ***新增群昵称绑定***
  - 玩家不可更改昵称
  - $\color{red} {注意：该功能的更多优化会在后几个版本继续迭代}$

### 写在最后
>本作品部分代码非常冗余，欢迎大佬对代码优化方面提供建议  
>遇到问题加Q323569086
