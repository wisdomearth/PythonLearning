# PythonLearning
多环境Python学习，用来做笔记

## Windows
> 我自己的Windows10
1. 环境配置
  - 安装[Git](https://git-scm.com/download/win)
    - 版本控制，之后做项目肯定离不开的，并且Windows上还能用用gitbash。要学就学官方的[Git Doc](https://git-scm.com/book/zh/v2)
  - [GitHub镜像网站](https://github.com/521xueweihan/GitHub520),如果有更好方式，建议还是直接登录官方网站:www.github.com
    - 顺便说一下，如果用的SwitchHosts，需要右键以管理员身份运行。
  - 安装[pyenv-win](https://github.com/pyenv-win/pyenv-win)
    - 个人比较建议使用pyenv，多环境比较干净，主要是Linux上用来控制Python多版本，Windows上可选
    - VScode 中的 PowerShell 一般默认的用户策略是Undefined(可以在powershell中执行 Get-ExecutionPolicy -List 查看),会使用Windows 默认策略Restricted代替[PowerShell 执行策略](https://docs.microsoft.com/zh-cn/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-7.2),不允许未签名的脚本运行。
    - 处理方法有3种
      - vscode 切换shell终端，选择gitbash
      - 设置用户默认powershell执行策略：Set-ExecutionPolicy -ExecutionPolicy Unrestricted -Scope CurrentUser
      -  为pyenv注册签名，大家可自行搜索windows脚本签名 方法，这里不再赘述
  - 安装[Poetry](https://python-poetry.org/docs/#osx--linux--bashonwindows-install-instructions)
  > python 依赖管理工具。[官方文档](https://python-poetry.org/docs/)
  > 安装失败的看看是不是url打不开，按照上面GitHub镜像网站操作下。
  > 用法[官方文档](https://python-poetry.org/docs/basic-usage/)
  >> 初始化环境：poetry init
  >> 进入环境：poetry shell，会打印当前虚拟环境路径：Spawning shell within xxxxx，复制xxxxx 解释器路径，下面会用到
  >> 更改vscode解释器：ctrl + shift + p，输入 select interpreter 回车，输入上面复制的解释器路径，回车
  >> 至此vscode 的Python 编码环境配置完毕。
## MacOS
> 版本 10.14.6
