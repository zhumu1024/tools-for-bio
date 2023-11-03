# tools-for-bio
此处收录整理遇到的工具

## 生信工具
### faTwoBit
`faToTwoBit`是一个与 DNA 序列处理相关的命令行工具,用于将 FASTA 格式的 DNA 序列文件转换为 TwoBit 格式。
TwoBit 格式是一种用于存储大规模 DNA 序列数据的二进制格式，它可以`高效地存储和检索 DNA 序列信息`。TwoBit 格式通常用于 UCSC Genome Browser 中，因为它允许用户高效地查看和浏览大型基因组数据。

faTwoBit的使用方式：
```
faToTwoBit input.fa output.2bit

```

## 代码/软件安装
gcc 是一种开源编译器，用于将源代码文件编译成可执行程序（机器代码）

pkg-config通常用于在构建软件时获取正确的库和头文件路径，以确保软件能够正确链接到所需的库。

autoconf：生成用于配置软件的脚本，使软件能够在不同的系统上构建。
libtool：管理库文件的创建和使用，允许跨平台的库文件共享。
automake：用于生成 Makefile，以便可以轻松地构建和编译软件。

CMake 是一个跨平台的开源构建系统，可以生成适用于不同编译器和平台的构建文件，使软件能够在各种操作系统上构建。

解析器生成器和词法分析器生成器，通常用于编译器和解释器的开发。它们用于生成解析语法和词法规则的 C 代码。bison 生成语法解析器，flex 生成词法分析器。
* 词法解析器也被称为词法分析器。它负责将源代码分割成称为标记（Tokens）的小块。标记是源代码的最小语法单位。
* 语法解析器负责将标记组织成语法结构，以创建抽象语法树


## 文本工具
sed（流编辑器）是一个在 Unix 和类 Unix 操作系统中广泛使用的文本处理工具。它用于对文本进行转换、替换、筛选和编辑，通常与管道一起使用。
* 文本替换   ```sed 's/old_pattern/new_pattern/g' input_file```
* 文本删除   ```sed '/pattern_to_delete/d' input_file```
* 文本插入  ``` sed '3i\This is a new line' input_fi ```
  
