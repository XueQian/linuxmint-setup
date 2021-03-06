# Linux Mint 17 Setup

1. 将软件源切换至国内服务器（推荐中国科技大学服务器USTC）
2. 更新系统（选择并应用全部更新）
3. 将鼠标和触摸板设置设置为最适合触摸板工作的方式（双指触摸、拖拽和滚动、输入时禁用触摸板等）
4. 安装Chrome浏览器
5. 安装Skype

  ```
  sudo apt-get install skype
  ```
6. 添加所需要使用的工具的第三方PPA源

  ```
  sudo add-apt-repository ppa:git-core/ppa
  sudo add-apt-repository ppa:webupd8team/atom
  sudo add-apt-repository ppa:webupd8team/java
  sudo add-apt-repository ppa:jerzy-kozera/zeal-ppa
  ```
7. 更新软件包数据并安装所需要使用的工具

  ```
  sudo apt-get update
  sudo apt-get install curl git atom zeal oracle-java8-installer
  sudo apt-get remove openjdk*
  ```
8. 配置Git全局设置参数

  ```
  git config --global user.name '<用户名>'
  git config --global user.email '<电子邮件地址>'
  git config --global color.ui true
  ```
9. 生成SSH密钥并将其注册到GitHub账号
10. 安装Atom编辑器的扩展包

  ```
  apm install linter linter-jshint editorconfig atom-beautify
  ```
11. 安装 IntelliJ IDEA 编辑器
12. 安装 IntelliJ IDEA 编辑器插件
  - .gitignore support
  - EditorConfig
  - NodeJS
  - AngularJS
  - Karma
13. 安装搜狗输入法依赖包

  ```
  sudo apt-get install fcitx fcitx-bin fcitx-config-common fcitx-config-gtk fcitx-data fcitx-frontend-all fcitx-frontend-gtk2:amd64 fcitx-frontend-gtk3:amd64 fcitx-frontend-qt4:amd64 fcitx-libs:amd64 fcitx-libs-gclient:amd64 fcitx-libs-qt:amd64 fcitx-module-dbus fcitx-module-kimpanel fcitx-module-lua fcitx-module-x11 fcitx-modules fcitx-ui-classic
  ```
14. 安装搜狗输入法
15. 安装NVM

  https://github.com/creationix/nvm
16. 在home目录下创建 ```.bashrc``` 文件并添加如下内容

  ```
  source ~/.nvm/nvm.sh
  ```
17. 使用NVM安装NodeJS并设置默认版本
18. 安装文泉驿微米黑和文泉驿正黑字体解决界面中文缺失问题

  ```
  sudo apt-get install fonts-wqy-microhei fonts-wqy-zenhei
  ```

