# medchrome
chrome调用动态库中间件，操作系统环境Win10, Chrome版本76.0.3809.132。关闭Win10的UAC体验更佳
## 引用方式
### 1. `csp`中引用中间件环境
```html
<ADDINS/>
```
### 2.`组件`中引用中间件环境
```vb
d ##class(websys.AddInsTmpl).WriteInvokerJsCode()
```
已配置对象列表如下：

|对象名|方法列表|功能说明|
|:-----:|:--------:|:---------:|
|CmdShell|GetInfo,GetIP,Run|调用cmd命令|
|DHCOPPrint|ToPrintHDLPStr|DHCOPPrint.CAB包打印|
|LODOP|FORMAT,PRINT_INIT,PRINT等方法|LODOP打印对象|
|TrakWebEdit3|ShowLayout|调用组件|
|PrjSetTime|SetTime|设置本地时间|

## 更新日志
### 2019-06-16 ###
#### 版本1.0.0.0 ####
* http协议下POST请求本地服务
* 自动下载配置的文件
* 自动安装exe,msi
* 自动注册ocx,dll
* 反射调用本地程序及cmd
