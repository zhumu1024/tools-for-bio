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
