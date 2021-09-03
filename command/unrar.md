unrar
===

解压rar文件命令，从rar档案中提取文件

###  语法

```shell
unrar [选项][switch 命令] [文件名...][路径]
   unrar <command> [-<switch 1> -<switch N>] archive [files...] [path...]
```

###  选项

```shell
e             # 解压压缩文件到当前目录
l[t,b]        # 列出压缩文件[技术信息,简洁]
p             # 将文件打印到标准输出。
t             # 测试压缩文件
v[t,b]        # 详细列出压缩文件[技术信息,简洁]
x             # 用绝对路径解压文件
```

### SWITCHES  开关设置

注意：每个开关必须用空格分隔。你不能把它们放在一起。
       
```shell
-av-       # 禁用，真实性验证检查。
-c-        # 禁用，评论显示
-f         # 刷新文件
-kb        # 保留破碎的提取文件
-ierr      # 将所有消息发送给stderr。
-inul      # 禁用，所有消息。
-o+        # 覆盖现有文件。
-o-        # 不要覆盖现有文件
-p<password>
     	   # 设置密码。
-p-        # 不查询密码
-r         # 递归子目录。
-u         # 更新文件。
-v         # 列出所有卷。
-x<file>
     	   # 排除指定的文件。
-x@<list>
     	   # 排除指定列表文件中的文件。
-x@        # 读取要从stdin中排除的文件名。
-y         # 对所有查询都假设为是。
```

###  参数

目录：指定要显示列表的目录，也可以是具体的文件。

###  实例

将压缩文件 text.rar 在当前目录下解压缩,并解压完整路径。

```shell
unrar x test.rar
```

### AUTHOR

```shell
This  manual  page  was  written by Petr Cech <cech@debian.org> according to "unrar -h"for the Debian
GNU/Linux system (but may be used by others).
```