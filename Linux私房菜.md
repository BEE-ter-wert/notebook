#### 基础命令

```shell
sudo su # 进入超级用户界面
```

```shell
exit # 退出当前命令
```

```shell
fdisk -l # 查看盘符设备
```

```Shell
calc  # 计算器
```

```shell
locale # 显示语言信息
LANG=en_US.utf8 # 切换语言
```

```shell
ls {显示文件列表} [-a]{显示隐藏文件} [-l]{以列表形式展示} ~{不知道这是干啥的}
ls {同上} [-al]{同时执行上面两个}
```

```shell
date # 显示日历
```

````shell
bc #打开bc计算器
/
*
+
_
^
%
quit # 退出计算器

<命令首字母串> + TAB # 获取本机可以使用的命令列表
man <命令名> # 查看命令介绍信息
<命令名> --help # 查看命令帮助
````

#### 环境变量

```shell
echo $PATH # 输出环境变量的值
/bin/ls # 使用绝对路径执行命令
```

#### 文件操作

```shell
cp # 复制
rm # 删除
mv # 移动 改名
basename <文件路径> # 文件名
dirname <文件路径> # 目录名
```

