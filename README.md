# ZhananBot-v2.0
一个好用强大的机器人插件 

## 功能介绍
* 支持违禁词撤回（new）
* 查询在线玩家
* 绑定系统
* 消息互通
* 进出服提醒
* 退群解绑（new）

## To Do
* 支持加群自动通过
* 支持自动更新插件
* 支持自动更新依赖
* 进群欢迎
* 群内执行指令
* 节假日祝贺词
* 大家可以[进群](https://qm.qq.com/cgi-bin/qm/qr?k=EMwr4Uxb2Wn1Jja4ibVhyHPqBmcW7gsH&jump_from=webapi&authKey=HL/SyJpAJ0uuskkiEhJcxZ4FlO9kK2FvRmz/sAcPkVttmwpIuuskkT9sfbeERIjLs">)积极提出好点子



## 依赖下载
1. 下载skript最新版[点我下载](https://github.com/SkriptLang/Skript/releases)
2. 下载Skript-reflect[点我下载](https://github.com/TPGamesNL/skript-reflect/releases)
3. 下载skUtilities[点我下载](https://github.com/tim740/skUtilities/releases)
4. 下载skript-yaml[点我下载](https://github.com/Sashie/skript-yaml/releases)
5. 下载miraimc[点我下载](https://github.com/DreamVoid/MiraiMC/releases)

## 使用
下载`ZhananBot.sk`本体后，下载上方所有依赖，运行服务器，使用`mirai login QQ号 QQ密码`登陆
登陆后将`ZhananBot.sk`放入`plugins/skript/scripts`目录下，输入`skript reload ZhananBot.sk`即可加载
之后按照下文编辑`plugins/ZhananBot`文件内的`config.yml`和`function.yml`文件

## 文件配置
#### config
```yaml
# 这里填写你的机器人QQ号
Bot_Account: 123456789

# 您可以在这里填写多个管理员名,用英文字符“,”分割
Bot_Administrator: 123456789,123456789

# 在这里填写您用来监听的群号,可填写多个,用英文符号“,”分割
Bot_Group: 123456789,123456789

# 在这里填写您希望显示的服务器名
Bot_logotext: Minecraft
```

#### function
```yaml
# 违禁词自动撤回功能,默认为关闭,可自行开启,赞助地址https://afdian.net/a/yimin/plan
Function_Check: false

# 是否开启强制绑定,开启后必须绑定QQ才可以入服,方便通过id查找QQ用户,默认开启
Function_Bind: true

# 是否开启群服消息互通以及玩家进出服提示
Function_Message: true
```

## 比较
功能|老版|新版
:---:|:--:|:---:
#bind-||仅支持一个群聊且无法开关|支持多个群聊并且可以开关
#unbind-|仅支持一个群聊切玩家退群不会自动解绑|支持多个群聊且退服自动解绑
#punbind|无此功能|-支持管理员进行手动解绑
#list|旧版list返回格式奇丑无比不支持多个群，玩家在关闭服务器时名称依然在list列表中|支持多个群聊且更加美观，修复了关服时未退出玩家一直存在的bug

## 指令
指令名称|作用域|执行权限|描述
:---:|:--:|:---:|:---:
#bind <玩家游戏id>|QQ群|所有群成员|将玩家QQ与玩家ID进行绑定
#unbind|QQ群|所有群成员|将玩家QQ与玩家ID进行解绑
#punbind <@指定玩家>|QQ群|群主/管理员/配置文件管理员|将指定玩家QQ与玩家ID进行解绑
#list|QQ群|所有群成员|查询服务器的玩家详情(在线人数,在线玩家)

