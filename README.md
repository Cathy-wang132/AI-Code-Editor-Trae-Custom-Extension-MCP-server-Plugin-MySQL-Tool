# AI-Code-Editor-Trae-Custom-Extension-MCP-server-Plugin-MySQL-Tool
# AI代码编辑器 Trae 自定义扩展 MCP-server插件-mysql工具-让AI编辑器有操作数据库能力！【本地化】

#### 1、介绍

在AI代码编辑器Trae里，自定义扩展 MCP-server插件-mysql工具，让AI编辑器有操作数据库能力！附操作步骤！

#### 2、详情文章

在分享怎么集成mcp-server工具之前，先简单分享一下 mcp-server 的基础概念！

MCP server

MCP server是为提供AI MCP（模型上下文协议）的服务。

MCP即模型上下文协议，它为开发者在AI大爆发的时代缺少规范导致效率低提供了解决思路，MCP让AI能更自由地调用工具。

简单的说：大家可以通过mcp server协议写一些插件，然后大模型可以通过此协议调用我们编写的工具，让大模型不仅有说话的能力，还可以赋予有手有脚干活的能力~

今天跟大家分享一下怎么在trae编辑器里集成 MCP-server-mysql 工具。让AI编辑器有操作数据库能力，不需要再手动去操作数据库，让我们的开发更便捷~

mysql-mcp-server工具源码地址：

https://github.com/designcomputer/mysql_mcp_server

以下描述的内容资料可在文末获取~

这篇文章分享的主要内容：怎么把开源工具集成到我们的trae AI编辑器里？其实不仅可以集成到trae编辑器 ,也可以集成到cursor 编辑器里，只需要根据相关规则配置即可。

先截图一下开源地址里的说明：

提供了两种编辑器的 json 的配置方式

![image](https://github.com/user-attachments/assets/a49867c7-88f5-43c1-a258-832ad3079586)


有一种方式可以不下载源码 ，直接通过trae编辑器里的mcp广场里搜索是可以安装的。

小编分享的是通过下载源码到本地 ，然后手动配置安装的。

因为源码里的 json 配置不太适合我的python 环境，就自己对json字符串 进行了调整。这个json字符串大家可以根据自己的需求调整~

这个json字符串的作用就是启动python代码并连接到你的数据库。

![image](https://github.com/user-attachments/assets/259c6158-2ec4-4466-b6ec-f5d20b9be53d)


对于python环境 ，大家可以自由百度搜索安装。我是用conda来管理python环境的。对于 conda 也自行百度即可。 json字符串解释完后，接下来就来安装~

### 第一步：编辑器选择 mcp

![image](https://github.com/user-attachments/assets/a0f34bdc-719b-4d6d-8032-1e901f2ddbfb)


### 第二步：添加 mcp

![image](https://github.com/user-attachments/assets/f7ca46bd-5a02-4ce1-af17-133ca403f077)


### 第三步：手动添加

![image](https://github.com/user-attachments/assets/93b38a0b-62b5-4749-98ef-c2bf353bae42)


### 第四步：编写json配置

![image](https://github.com/user-attachments/assets/7444d777-318d-4839-9ba1-5fa3a85f334f)


### 第五步：把编写好的json 复制粘贴到里面

![image](https://github.com/user-attachments/assets/7043ba17-6722-467e-9688-3c3c2697a417)


### 第六步：检测显示是否正常，如果启动失败，大部分是因为路径问题。所以json字符串里的命令可以先通过cmd 测试一下

![image](https://github.com/user-attachments/assets/f58c6483-1f68-458f-8cfc-3e7086662918)


### 第七步：智能体添加

![image](https://github.com/user-attachments/assets/fc0c0c61-5789-4cf5-ad21-cfdadd0b9302)


智能体简单介绍：就是我们来定义一个规范，让AI大模型回答的问题更垂直~

### 第八步：智能体配置

![image](https://github.com/user-attachments/assets/e91bf50a-c481-44cc-9715-85d51d368440)


### 提示词书写：

![image](https://github.com/user-attachments/assets/814c6252-0367-499b-950d-f8c7c8585373)

### 第九步：测试

![image](https://github.com/user-attachments/assets/a5d9500c-4f49-4a3e-89f1-9357fd2a516c)

### 第十步：结果

![image](https://github.com/user-attachments/assets/e234bbc5-aa29-414d-aadc-6ecb26611834)

### 第十一步：验证

![image](https://github.com/user-attachments/assets/76271afd-8390-4894-8d26-7ec233fece5d)

这样以后在开发项目的时候，尤其是做一些小项目，我们就不需要去关心数据库了，非常方便！

![image](https://github.com/user-attachments/assets/c126d311-9215-4317-827c-066d8f475efd)


![image](https://github.com/user-attachments/assets/e52c11b8-9eb1-49ac-b770-d98f9e0cd19e)

对于以上的内容资料，已经做了整理，有需要的小伙伴可以

### 点击链接获取：

https://www.wwwoop.com/home/Index/projectInfo?goodsId=96&typeParam=3&subKey=2
