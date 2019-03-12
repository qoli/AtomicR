# 如何编写自己的脚本

Plane Router 具备强大的开放性，允许用户编写自己的 VPS 管理脚本。

当前为 1.0 阶段，请有能力的作者参考此 GitHub 项目，在 app/srouce 下为当前已有脚本的范例。



## addList.json

此为 Plane Router App 的脚本来源列表。



## srouce / system.json，bbr.json，SSRServer.json

我们以 system.json，bbr.json，SSRServer.json 这三个脚本作为例子解说。

data 是一个数组，有如下架构。

##### 标题

```json
{
    "type": "title",
    "value": "操作"
}
```

##### 操作

操作将会调用终端，并自动输入 action 中的指令。

```json
{
    "type": "action",
    "value": "打开终端",
    "action": "pwd"
}
```

##### 网页链接

```json
{
    "type": "webview",
    "value": "https://shadowsocks.be/9.html"
}
```

##### 提示信息

```json
{
    "type": "message",
    "value": "脚本要求",
    "action": "需要 root 用户执行"
}
```

##### 读取服务器信息

在页面打开时候，会自动透过 SSH 背景运行命令，并返回信息到页面。

```json
{
    "type": "status",
    "value": "BBR 状态",
    "action": "echo $(sysctl net.ipv4.tcp_available_congestion_control)"
}
```



## 提交修改好的脚本到此开源项目

我（App 作者）将会检查你们所提交的脚本，如果认为合适于开放给大家使用将会允许你们的提交合并到此项目上。



## 私有脚本？

App 在 1.0 阶段暂时还没支持私有脚本，将会在以后的更新加入私有脚本。



---

感谢你们的使用

2019年03月13日