# thesis-paper

> 写论文的正确的姿势（这里以复旦大学硕士论文为例）

## 依赖

- 安装 Tex Live 2019
  - 安装方法可以知乎搜索，各个系统的安装方法都有。安装包还是蛮大的（好几个 G，虽然支持连线安装，但不靠谱，还是下载后离线安装吧），Windows 有相应的 iso 文件，用虚拟光驱打开即可安装。
- tlmgr install fduthesis（tlmgr 是 Tex Live 的包管理工具，这里安装复旦大学论文包）
- tlmgr install graphviz（这个包画图很方便）
- 安装 graphviz（虽然上一步已经安装到了 Tex Live，但是还要安装到操作系统里，否则会报 dot 应用程序找不到的错误。）
  - Windows: 下载相应的 Installer，装完后还需要把 dot 所在的目录加到 PATH 里
  - Mac: 可以使用 Homebrew 安装

## 本地编译

```shell
latexmk -xelatex -shell-escape main
```

## 编译结果

[`main.pdf`](main.pdf)

## 自动化

- Windows 下运行 [`.\build.bat`](build.bat) 即可
