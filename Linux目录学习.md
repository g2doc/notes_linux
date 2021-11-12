<!--
 * @Author: zhanghao
 * @Date: 2021-10-31 17:13:06
 * @LastEditTime: 2021-10-31 17:33:53
 * @Description: Do not edit
 * @FilePath: /Self_Notes/Linux目录学习.md
-->



Linux 的根目录 `/` 是最重要的 !!!

也被称为 root 目录 

Let us see My Root :
```shell
zhanghao@debian:/$ tree -L 1
.
├── bin -> usr/bin
├── boot
├── dev
├── etc
├── fcitx-baidupinyin.deb
├── home
├── initrd.img -> boot/initrd.img-5.10.0-9-amd64
├── initrd.img.old -> boot/initrd.img-5.10.0-9-amd64
├── lib -> usr/lib
├── lib32 -> usr/lib32
├── lib64 -> usr/lib64
├── libx32 -> usr/libx32
├── lost+found
├── media
├── mnt
├── opt
├── proc
├── root
├── run
├── sbin -> usr/sbin
├── srv
├── sys
├── tmp
├── usr
├── var
├── vmlinuz -> boot/vmlinuz-5.10.0-9-amd64
└── vmlinuz.old -> boot/vmlinuz-5.10.0-9-amd64

```

| 目录名  | 解释 |
| :-:     | :-   |
`bin/`    | 系统的二进制可执行文件
`sbin/`   | 只有root才能访问的可执行文件
`etc/`    | 系统的配置文件
`usr/`    | 可以理解为C:/Windows/
||/usr/lib理解为C:/Windows/System32
|| 很重要 !!! 搞坏了要重装系统的
`usr/local/`|用户级的程序目录，可以理解为C:/Progrem Files/
||用户自己编译的软件默认会安装到这个目录下
`usr/src/` | 系统级的源码目录
`usr/local/src/`|用户级的源码目录
`dev/` | device, 存放设备文件、驱动等
`root/` | root 用户的家目录(主目录)
`boot/` | 系统启动时需要用到的文件
`mnt/` | root 安装临时文件的安装点
`lib/` | 放置系统运行和第三方程序运行所依赖的lib库
`tmp/` | 放置各种的临时文件
`var/` | 放置运行时需要改变数据的文件 (ex: 日志文件)
`opt/` | 也是用户级的程序目录，可以理解为D:/Software。
||安装的一些大型工具都可以放在这里,ex:PyCharm,IDEA,Qt ...