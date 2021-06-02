# **🤣使用说明🤣**
## 效果展示
![测试图](https://github.com/leetingjiu/ps1/blob/f2b812a0535b654674f798b899391d13a3cf4ede/test.jpg)
## 第一步~修改Console颜色
* 安装<br>
在路径“C:\Windows\System32\WindowsPowerShell\v1.0”下新增profile.ps1文件，写入脚本代码<br>
详情见[profile.ps1](https://github.com/leetingjiu/ps1/blob/0c073da7126fa2703757098eea6422a8f63c96d1/profile.ps1)
* 更换颜色<br>
用颜色关键词修改ps1文件，详情见[color.txt](https://github.com/leetingjiu/ps1/blob/0c073da7126fa2703757098eea6422a8f63c96d1/color.txt)
* 卸载<br>
删除profile.ps1文件
## 第二步~安装Oh-my-posh皮肤
* 安装模块<br>`Install-Module oh-my-posh -Scope CurrentUser`
* 获取皮肤<br>`Get-PoshThemes`
* 临时设置皮肤agnoster<br>`Set-PoshPrompt -Theme agnoster`
* 永久设置皮肤agnoster<br>
在路径“C:\Users\ltj\Documents\WindowsPowerShell”下新增Microsoft.PowerShell_profile.ps1文件，写入脚本代码<br>
详情见[Microsoft.PowerShell_profile.ps1](https://github.com/leetingjiu/ps1/blob/0c073da7126fa2703757098eea6422a8f63c96d1/Microsoft.PowerShell_profile.ps1)
* 更新模块<br>
`Update-Module oh-my-posh`
* 卸载模块<br>
`Uninstall-Module oh-my-posh -Force`
## 第三步~安装Powerline字体
[下载PoweLine](https://github.com/powerline/fonts.git)，解压Zip
* 安装<br>
运行install.sh
* 卸载<br>
运行uninstall.sh
## 一些问题
Q：有些特殊符号为什么显示不出来？<br>
A：因为Windows下Oh-my-posh皮肤同Linux/MacOS下的Oh-my-zsh皮肤一样，壳shell本身需要支持Powerline字体(这也是操作第三步的必要性)。
