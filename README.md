# Bees
这是一个 beego 实例项目

## 基本信息

## 错误调试
> ### VS code 报错：gopls requires a module at the root of your workspace
gopls需要一个模块在您的工作空间的根部。  
您可以通过打开每个模块作为工作空间文件夹来处理多个模块。  
此工作流程的改进将很快到来，您可以在这里了解更多信息：  
https://github.com/golang/tools/blob/master/gopls/doc/workspace.md  

方法一：将 gopls 的版本回退到 v0.5.5 可以解决  
方法二：
打开：文件 > 首选项 > 设置 > go > settings.json 添加如下内容：
```
"gopls": {
    "experimentalWorkspaceModule": true
},
```
这句话的意思是启用实验功能