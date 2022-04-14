# shell
## 单双引号：
* 单引号里的任何字符都会原样输出，单引号字符串中的变量是无效的；
* 单引号字串中不能出现单独一个的单引号（对单引号使用转义符后也不行），但可成对出现，作为字符串拼接使用。
* 双引号里可以有变量
* 双引号里可以出现转义字符

## 字符串
* 获取字符串的长度
```shell
string="abcd"
echo ${#string}
```
* 提取字符串
```shell
echo ${string:1:4}
```
* 查找字符串
```shell
string="ansoh "
echo `expr index "$string" io` #查找i或o的位置
```
多行注释
```shell
:<<EOF
注释内容
EOF
```