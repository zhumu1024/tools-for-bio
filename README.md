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



## 通用工具

### 文本工具
sed（流编辑器）是一个在 Unix 和类 Unix 操作系统中广泛使用的文本处理工具。它用于对文本进行转换、替换、筛选和编辑，通常与管道一起使用。
* 文本替换   ```sed 's/old_pattern/new_pattern/g' input_file```
* 文本删除   ```sed '/pattern_to_delete/d' input_file```
* 文本插入  ``` sed '3i\This is a new line' input_fi ```

jq、jid、pup：用于处理和查询 JSON 数据的命令行工具。

datamash、miller、tsv-utils：用于处理文本和表格数据的工具，包括统计、转换和过滤。

hyperfine 性能分析工具

ripgrep：文本搜索工具

tokei：  代码统计工具。

bat：代码高亮显示的 cat 替代工具。

exa：现代的 ls 替代工具。

tealdeer：TUI（命令行界面） 风格的 Man 页面查看工具。

gpg2：GnuPG（GNU Privacy Guard）的版本2，用于加密和签名文件，以确保文件的安全性和完整性。

pandoc：文档转换工具，可将一个文档格式转换为另一个文档格式，如将Markdown文件转换为HTML、PDF、Word文档等。
  
### 系统监视和管理工具
screen：终端会话管理工具，允许在同一终端窗口中运行多个会话。

stow：用于管理软件包的符号链接的工具，通常用于配置管理。

htop：交互式系统监视工具，用于查看和管理系统资源的使用。

tree：显示目录结构的工具，以树状图的形式显示文件和子目录。

pv：管道查看器，用于监视数据流的进度。

bottom：系统监视工具，提供有关系统资源使用的信息。

### 其他工具
parallel：并行化工具，用于并行执行命令和任务。

pigz：并行压缩/解压缩工具，用于处理 gzip 压缩文件。

librsvg、udunits：用于处理图像和单位转换的库。

proxychains-ng：通过代理服务器访问网络资源的工具。


gnuplot：绘图工具，用于生成各种类型的图表和图形，可用于数据可视化和绘图。

graphviz：开源图形可视化工具，用于创建和渲染图形结构，如流程图、组织结构图和网络拓扑图。

imagemagick：图像处理工具套件，用于处理、编辑和转换图像文件，包括图像格式转换、图像裁剪、缩放、旋转等操作。

支持图形用户界面（GUI）应用程序的构建和运行的工具

* libpthread-stubs：模拟 POSIX 线程标准，以便在多线程应用程序中使用线程相关的功能。

* renderproto：这是 X Window System 的一个渲染协议的开发库，用于支持 2D 图形渲染。
* kbproto：这是键盘协议的开发库，用于支持键盘输入。
* xextproto：这是 X Window System 扩展协议的开发库，用于支持 X 窗口系统的扩展功能。
* gsettings-desktop-schemas：这个包含了 GSettings 桌面配置数据库的模式
* gtk+3：这是 GTK+ 库的版本3，它是一种用于构建跨平台 GUI 应用程序的工具包，特别适用于 Linux 桌面应用程序的开发。
* adwaita-icon-theme：这是 Adwaita 图标主题，它包含了一套常见图标，通常用于 GNOME 桌面环境中的图形应用程序。
* gobject-introspection：这是 GNOME 的 GObject 类型系统的一部分，它允许通过元数据来生成不同编程语言的绑定，以便其他编程语言可以与 GObject 进行交互。这对于跨语言开发非常有用。


## 下载工具

aria2
* 满足多协议、多连接下载并有其他高级功能要求。
  
curl
* 提供了广泛的命令行选项，允许用户执行各种网络操作，并可以将输出重定向到文件或终端。

wget  
* 专注于下载文件,主要特点是它可以通过递归下载整个网站或目录，包括链接和子链接。

## 代码/软件安装
gcc 是一种开源编译器，用于将源代码文件编译成可执行程序（机器代码）

pkg-config通常用于在构建软件时获取正确的库和头文件路径，以确保软件能够正确链接到所需的库。

autoconf：生成用于配置软件的脚本，使软件能够在不同的系统上构建。

libtool：管理库文件的创建和使用，允许跨平台的库文件共享。

automake：用于生成 Makefile，以便可以轻松地构建和编译软件。

CMake 是一个跨平台的开源构建系统，可以生成适用于不同编译器和平台的构建文件，使软件能够在各种操作系统上构建。

bison 生成语法解析器，flex 生成词法分析器。通常用于编译器和解释器的开发。它们用于生成解析语法和词法规则的 C 代码。

* 词法解析器也被称为词法分析器。它负责将源代码分割成称为标记（Tokens）的小块。标记是源代码的最小语法单位。
* 
* 语法解析器负责将标记组织成语法结构，以创建抽象语法树

cpanm 是 Perl 的一个模块安装工具，它的全名是 "App::cpanminus"。

它是 CPAN（Comprehensive Perl Archive Network） 生态系统的一部分，用于安装和管理 Perl 模块。

两个 Java 开发工具
 * Ant,更灵活，使用 XML 文件来定义构建任务和依赖关系，可以用于编译、打包、测试和部署 Java 应用程序等任务,特别适用于管理和构建 Java 项目。
   
 * Maven,更加规范化，提供了一种一致的方式来构建、测试、打包和发布 Java 项目，同时管理项目的依赖项。



  
