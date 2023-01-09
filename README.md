# PhyHubThesis
PhyHub用LaTeX课业论文模板. 

## 编译说明
你需要安装LaTeX的主流发行版. 
推荐[TeX Live 2022](https://www.tug.org/texlive/).

把导言区的`\newcommand{\PATH}{路径}`改成此文档的相对路径 (MAC OS或Linux) 或绝对路径 (Windows), 然后在该目录下使用命令行依次运行:

`xelatex` 文件名 (可以省略.tex)  
`biber` 文件名 (可以省略.bib)  
`xelatex` 文件名  
`xelatex` 文件名

## 更新日志

### v0.4.0
January 9, 2023

分离了 sty 文件，更新了一些宏包和很多自定义命令

### v0.2.1
September 12, 2020
* 添加了braket (`\braket`) 命令

### v0.2.0
August 27, 2020
* 添加了左右矢 (`\bra`, `\ket`), 并矢 (`dyad{a}{b}`) 和内积 (`\inner{a}{b}`, `\varinner{a}{A}{b}`)的命令

### v0.1.2
July 15, 2020
1. 将`\md`指令改成了`\dif`, 而且提供了`\dif[2]`的高阶微分用法
2. 修正了typo

### v0.1.1  
July 13, 2020
* 修正了一处错误：`withstar`版的`printbibliography`在toc中错误显示为「目录」

### v0.1.0  
July 11, 2020  
1. 现在`\diff`和`\pdiff`可以使用可选参数来决定是否是高阶导数了
2. 所以删掉了`\ndiff`和`\npdiff`
3. 增加了一个`\appendix`为分界线的附录部分
4. 可以使用`heading=withstar/withoutstar`来决定参考文献是否显示附录的序号A/B/...
5. 修正typo

