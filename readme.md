# **🤣使用说明🤣**
## =================================================
![](https://github.com/leetingjiu/ps1/blob/62e501224da34b86687bce7cd077acbaae9f4f0a/ltj.png)
## 第一步~安装oh-my-posh皮肤
* 安装模块<br>`Install-Module oh-my-posh `
* 获取皮肤<br>`Get-PoshThemes`
* 更新模块<br>`Update-Module oh-my-posh`
* 卸载模块<br>`Uninstall-Module oh-my-posh -Force`
## 第二步~配置用户环境
* 修改脚本策略<br>`Set-ExecutionPolicy RemoteSigned`
* 创建配置文件<br>`if (!(Test-Path -Path $PROFILE )) { New-Item -Type File -Path $PROFILE -Force }`
* 写入脚本保存<br>`notepad $profile`<br>
## 第三步~安装nerd或powerline字体
* 这两种字体均在github上开源，楼主使用的是DejaVuSansMono Nerd Font或Cousine Nerd Font，这两套字体支持的图标比较全。(https://github.com/leetingjiu/ps1/blob/67535c0de58547f94079b5a1ea92287de1516a4e/Meslo%20LG%20M%20DZ%20Italic%20Nerd%20Font%20Complete%20Windows%20Compatible.ttf)。<br>[nerd字体](https://github.com/ryanoasis/nerd-fonts)<br>[powerline字体](https://github.com/powerline/fonts)<br>
## =================================================
## 一些问题
* Q：有些特殊符号为什么显示不出来？<br>
* A：因为oh-my-posh主题中包含着各种角标和字体，需要nerd字体或者powerline字体支持。下载字体压缩包-解压-选中字体-为所有用户安装-设置控制台属性-默认-字体-Meslo Nerd Font。
* Q：怎么样才能永久设置皮肤？
* A：主题最终呈现的效果，均在$profile文件中。用记事本打开，写入设置皮肤命令`Set-PoshPrompt -Theme nu4a`，保存。可参考楼主配置文件[$profile](https://github.com/leetingjiu/ps1/blob/ae0c4dad7e9a16b3972a04ad4736a06ba152f34e/$PROFILE)
