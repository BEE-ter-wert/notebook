

# 杂项

```shell
mkdir <name> # 创建目录<目录名>
rmdir <name> # 删除目录<目录名>
touch <name> # 创建文件<文件名>
mv <被修改的文件名> <新的文件名> # 修改文件名

source <shell脚本全名> # 将定义好的shell脚本添加到系统中

!! # 执行上一条执行过的命令
$? # 获取报错信息
$_ # 获取参数
foo=$(pwd) # 变量获取当前工作目录
echo $foo # 输出当前工作目录
* # 通配符
? # 缺省符号
{a..j} # 范围匹配
# 例如
touch {foo,bar}/{a..j} # 在foo和bar文件夹下创建文件名为a到j的文件

diff # 检查两个文件或者目录之间的不同


shellcheck <shell文件名> # 检查shell中的语法错误
find . -name src -type d # 递归查找文件名为src文件类型为Dir(目录)类型的文件

tree # 打印本文件夹所有的文件和目录
broot # 在文件树中查找文件

head # 获取输出的指定行数
```





# 打印

## echo

```shell
echo "hello world" # 打印字符串
echo 'hello world' # 同上
a=100 # 注意a = 100是错误的，因为这样的话计算机会认为有三个参数
echo $a # 打印变量a

echo "hello $a" # 打印字符串和变量
echo "hello $a" # 会将后面的 $a 识别成字符串
```



# 编辑

## vim

```shell
vim <文件名> # 进入文件
<i>  # 进入输入模式
<esc> # 退回到正常模式
<:w> # 写入
<:q> # 关闭当前所在的窗口，如果没有其他窗口则退出Vim
<:aq> # 退出所有的窗口
<:quit> # 退出
<:help :W> # 查看输入：w后的作用帮助
<:help w> # 查看输入w后的帮助
<:sp> # 打开一个新的窗口
u # 撤销
CTRL+R # 恢复
y # 复制
p # 粘贴
yw # 复制这个单词
yy # 复制整行
v # 进入可视模式，可以通过移动键盘移动光标位置到行，页，单词，段落，屏幕上，中，下，并选择在其中的内容进行操作
V # 同上，但是选择整行
CTRL+v # 同上，但是选择一个矩形块
~ # 改变所选内容的大小写
j k h l # 上下左右
4j # 向上移动四行...以此类推
e # 选择一个单词
3e # 选择三个单词
eee # 同上
c # 改变，删除内容然后进入insert模式
d # 删除，只是删除内容
2dw # 删除两个单词
2dwi == 2cw # 左右两边命令相等，注意一下
ci[ # 修改方括号内部的内容	change inside [
ci\' # 修改''内的内容,没有那个反斜杠
di( # 删除圆括号内的内容
G # 跳转到文件底部
o/O # 创建新行在光标下/上
/ # 搜索
. # 没听清是啥作用，翻译的锅
```

网站原课程

<p><iframe style="width: 100%; height: 720px;" src="https://missing-semester-cn.github.io/2020/editors" frameborder="0" width="1080" height="720"></iframe></p>

## 字符串相关

```shell
sed 正则表达式 # 替换字符串，修改文件的内容，不用通过管道
sed -E 正则表达式 # 支持现代的正则表达式语法

awk 正则表达式 # 用于文本处理的脚本语言

paste -sd+ # 使用加号连接文本	
wc # 单词计数程序
sort # 排序
uniq # 每种只会打印一次
```

# 数据整理（包含正则表达式教程）

<p><iframe style="width: 100%; height: 720px;" src="https://missing-semester-cn.github.io/2020/data-wrangling/" frameborder="0" width="1080" height="720"></iframe></p>

# 终端控制，文件，远程控制

```shell
sleep 秒数 # 控制机器休眠固定秒数

ctrl+c # 发送结束进程的信号SIGINT
man signal # 查看控制进程的信号
```

