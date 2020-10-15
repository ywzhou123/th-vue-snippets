# Tellhow Vue Snippets for Visual Studio Code

## Component

主要为Vue基础组件库提供代码片段

```sh
    npm i th-vue-component -S
```

## Snippets

### vue模板快捷键

`t-`开头

| Prefix | Vue Snippet Content |
| ------ | ------------ |
| `t-init` | `vue模板` |
| `t-template` | `template标签` |
| `t-script` | `script标签` |
| `t-script-all` | `script完整标签` |
| `t-style` | `style标签` |

### html标签快捷键

`th-`开头

### util工具类快捷键

`u-`开头

### rule校验规则快捷键

`r-`开头

### localStorage存储快捷键

`s-`开头

### mixin混入快捷键

`m-`开头

### directive自定义指令快捷键

`d-`开头

### filter过滤器快捷键

`f-`开头


## Deploy

### 方式一、打包插件

```sh
    npm i vsce -g
    vsce package
```

打包成vsix插件，发送给别人进行安装
切换到扩展页，点击右上角...选择`Install form VSIX`

### 方式二、发布到应用市场

[注册登录](https://login.live.com/)

[访问Azure](https://aka.ms/SignupAzureDevOps)

创建令牌：personal access tokens，保存好

```sh
    npm i vsce -g
    # 创建发布账号, 输入昵称、邮箱、令牌
    vsce create-publisher ywzhou
    # 登录, 创建后不需要再登录
    vsce login ywzhou
    # 发布，每次更新要修改版本号
    vsce publish
```

[应用市场查找](https://marketplace.visualstudio.com/items?itemName=ywzhou.th-vue-snippets)



