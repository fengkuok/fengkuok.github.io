---
layout: post
title:  "Ubuntu下安装Eclipse"
date:   2016-07-24 21:51:00 +0800
categories: blog
---
>【前提条件】已安装好JDK

1. 下载最新版 [Eclipse IDE for Java EE Developers](http://www.eclipse.org/downloads/packages/eclipse-ide-java-ee-developers/kepler) 。

2. 解压eclipse到 /opt目录
`$sudo tar -zxvf eclipse-jee-kepler-R-linux-gtk-x86_64.tar.gz -C /opt/`

3. 创建启动快捷方式

- 当前用户

  `$vi ~/.local/share/applications/eclipse.desctop`

- 全局

  `$sudo vi /usr/share/applications/eclipse.desctop`

  内容如下：

  ```
  #!/usr/bin/env xdg-open
  [Desktop Entry]
  Name=Elipse Kepler
  Type=Application
  Icon=/opt/eclipse/icon.xpm
  Exec=/opt/eclipse/eclipse
  Comment=IDE for JavaEE developers
  Categories=Development;IDE;
  Terminal=false
  ```
