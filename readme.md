# **🤣使用说明🤣**
## 效果展示
![测试图](https://github.com/leetingjiu/ps1/blob/f2b812a0535b654674f798b899391d13a3cf4ede/test.jpg)
## 第一步~安装oh-my-posh皮肤
* 安装模块<br>`Install-Module oh-my-posh `
* 获取皮肤<br>`Get-PoshThemes`
* 临时设置皮肤agnoster<br>`Set-PoshPrompt -Theme agnoster`
* 更新模块<br>
`Update-Module oh-my-posh`
* 卸载模块<br>
`Uninstall-Module oh-my-posh -Force`
## 第二步~配置用户环境
* 修改脚本策略<br>
`Set-ExecutionPolicy RemoteSigned`
* 创建配置文件<br>
`if (!(Test-Path -Path $PROFILE )) { New-Item -Type File -Path $PROFILE -Force }`
* 写入配置文件<br>
`notepad $profile`<br>
`Import-Module oh-my-posh
Set-PoshPrompt -Theme nu4a`
## 第三步~安装nerd或powerline字体
[下载PoweLine](https://github.com/powerline/fonts.git)，解压Zip
* 安装<br>
运行install.sh
* 卸载<br>
运行uninstall.sh
## 一些问题
Q：有些特殊符号为什么显示不出来？<br>
A：因为Windows下Oh-my-posh皮肤同Linux/MacOS下的Oh-my-zsh皮肤一样，壳shell本身需要支持Powerline字体(这也是操作第三步的必要性)。
