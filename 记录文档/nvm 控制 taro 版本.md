# nvm 控制 taro 版本

#### 1，nvm安装：[github安装地址](https://github.com/nvm-sh/nvm)

**介绍：**它是管理node版本的工具，可以下载或切换对应的node版本，同时可以切换taro版本（用来开发不同的项目）

**注意事项：**安装前删除所有 node.js

`有 node 相关内容`

```html
node 最新文档截至编写
所使用的版本：	v12.10.0	v14.18.0	v16.14.2
```
基本使用：

```
查看所有可下载的 node 版本：nvm list available
查看本地安装的 node 版本：nvm ls

# version 版本号，arch 指定安装32位或64位。
安装指定node版本：nvm install <version> [arch] 

# 同上。
卸载指定node版本：nvm install <version> [arch] 

# 同上。
切换node版本：nvm use <version>[arch] 

# name 自己定义的别名， version 版本号
给不同的版本添加别名：nvm alias <name> <version> 
```

#### 2，taro安装：[taro文档](https://taro-docs.jd.com/taro/docs)

**介绍：** Taro 是一个开放式跨端跨框架解决方案，支持使用 React/Vue/Nerv 等框架来开发 微信 / 京东 / 百度 / 支付宝 / 字节跳动 / QQ / 飞书 小程序 / H5 / RN 等应用。

**注意：**若需要nvm版本控制taro，请使用第一种方式 npm 安装。

```
# 使用 npm 安装 CLI
$ npm install -g @tarojs/cli

# OR 使用 yarn 安装 CLI
$ yarn global add @tarojs/cli

# OR 安装了 cnpm，使用 cnpm 安装 CLI
$ cnpm install -g @tarojs/cli
```

**注意：**如果安装过程出现`sass`相关的安装错误，请在安装 [mirror-config-china](https://www.npmjs.com/package/mirror-config-china) 后重试。

```
$ npm install -g mirror-config-china
```

#### 3，注意版本信息：

```
	node：v12.10.0 --> taro：1.3.**
	node：v14.18.0 --> taro：3.**.**
	node：v16.14.2 --> taro：3.0.10 (并不兼容)
```

