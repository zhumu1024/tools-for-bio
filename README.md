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
### alignDB 
alignDB 可能指的是用于数据对齐（alignment）或数据管理的工具或库。在生物信息学领域，数据对齐通常是将不同样本的生物数据（例如 DNA 或蛋白质序列）进行比对和匹配的过程，以便进行进一步的分析

### Jim Kent /bin下生信工具介绍
待续

### egaz目录下生信工具介绍
待续

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

### 支持GUI相关
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

## windows板块工具

### 编程工具

* Oracle Java Runtime Environment (JRE)：Java运行时环境，用于运行Java应用程序。它提供了Java程序的执行环境，并允许在Windows上运行使用Java编写的应用程序。
* Oracle JDK 18:Java开发工具包（JDK）版本18，用于开发和编译Java应用程序。JDK 包含了 JRE，同时还包括编译器和其他开发工具。
* Strawberry Perl: 一个Windows下的Perl发行版，它包含了Perl编程语言的运行时环境以及与CPAN兼容的模块，适用于Windows平台的开发。
* R Project：R是一种统计计算和数据分析的编程语言和环境。RProject.R 是R的一个包，用于安装R编程语言和环境。
* RStudio (Open Source)：RStudio是一个集成开发环境（IDE），专为R编程语言设计。它提供了一个用户友好的界面，用于开发、调试和可视化数据分析和统计任务。这里安装的是RStudio的开源版本。
* Kitware CMake：CMake是一个跨平台的构建工具，用于配置、构建和测试软件项目。它支持多种编程语言和构建系统，并被广泛用于C++项目。
* Node.js (LTS)：Node.js 是一个用于构建服务器端应用程序的JavaScript运行时环境。

### 进阶
* GitHub Desktop：GitHub Desktop 是 GitHub 提供的一个图形用户界面（GUI）工具，用于更轻松地管理和协作GitHub上的代码仓库。
* GitHub CLI：GitHub CLI 是 GitHub 提供的命令行界面工具，允许你在终端中执行GitHub相关操作，如创建仓库、提交代码等。
* WinSCP：WinSCP 是一个开源的SFTP（SSH文件传输协议）、FTP和SCP（Secure Copy Protocol）客户端，用于在Windows上安全地传输文件。
* Visual Studio Code：Visual Studio Code（VS Code）是一个开源的轻量级代码编辑器，提供了丰富的扩展支持，适用于多种编程语言和开发任务。
* Beyond Compare 4：Beyond Compare 4 是一款用于文件和目录比较的工具，它允许你查找和比较文件的差异，以便进行文件合并和同步。
* JetBrains Toolbox：JetBrains Toolbox 是 JetBrains 公司提供的一个工具集，用于管理和安装其各种开发工具，如IntelliJ IDEA、PyCharm、WebStorm等。
* RealVNC Viewer：RealVNC Viewer 是一个用于远程桌面访问的工具，它允许你在网络上远程控制其他计算机。
* RedisInsight：RedisInsight 是一个图形化的Redis数据库管理工具，用于查看和操作Redis数据。
* Memurai Developer：Memurai Developer 是 Memurai 公司提供的 Windows 下的 Redis 数据库的端口（Port），允许你在Windows上运行和开发Redis应用程序。

### 实用工具

* Everything：Everything 是一个快速的本地文件搜索工具，它允许你在计算机上瞬间查找和定位文件和文件夹。

* Bandizip：Bandizip 是一个压缩文件管理工具，它支持多种常见的压缩文件格式，如ZIP、RAR、7Z等，以及创建和解压这些文件。

* Rufus：Rufus 是一个用于创建启动性能的USB闪存驱动器（例如用于操作系统安装的启动盘）的工具。要求版本3.18或更高。

* QuickLook：QuickLook 是一个快速文件预览工具，它允许你通过按下空格键来快速预览文件内容，而无需打开文件。

* WizTree：WizTree 是一个用于分析磁盘空间使用情况的工具，它可以帮助你查找磁盘上最大的文件和文件夹，以便进行清理和管理。

* Microsoft PowerToys：Microsoft PowerToys 是一组 Windows 实用工具和增强功能的集合，用于改善 Windows 桌面体验。它包括多个工具，如 FancyZones（窗口管理工具）、PowerRename（文件重命名工具）等。

* qBittorrent：qBittorrent 是一个免费开源的BitTorrent客户端，用于下载和分享文件，支持多种BitTorrent功能和协议。

* Rapid Environment Editor：Rapid Environment Editor 是一个用于编辑和管理Windows环境变量的工具，使你能够轻松地配置系统和用户级别的环境变量。

* ExplorerPatcher：ExplorerPatcher 是一个自定义 Windows 文件资源管理器的工具，允许你对文件资源管理器进行各种外观和功能修改。

* Clash for Windows：Clash for Windows 是一个免费的网络代理工具，它允许你在Windows上配置代理服务器以保护隐私和访问被封锁的网站。



  
