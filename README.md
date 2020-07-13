# PhyHubThesis
PhyHub用LaTeX课业论文模板. 

## 编译说明
你需要安装LaTeX的主流发行版. 
推荐[TeX Live 2020](https://www.tug.org/texlive/).

把导言区的`\newcommand{\PATH}{路径}`改成此文档的相对路径 (MAC OS或Linux) 或绝对路径 (Windows), 然后在该目录下使用命令行依次运行:

`xelatex` 文件名 (可以省略.tex)  
`biber` 文件名 (可以省略.bib)  
`xelatex` 文件名  
`xelatex` 文件名

## 更新日志
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

