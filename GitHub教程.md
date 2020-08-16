### Git 原理简介

仓库：**本地仓库**和**远程仓库**（托管在网络端的仓库）

本地仓库：工作区和版本区，其中版本区包含暂存区和仓库区

从本地仓库将文件 git 到远程仓库的流程：工作区 --> 暂存区 --> 仓库区 --> 远程仓库

![](D:\Software\Git\repository\Github\images\git原理图.png)

将本地文件 git 到 Github 远程仓库

```bash
$ git init	--初始化版本库

$ git remote add origin 仓库地址	--添加远程仓库

$ git pull --rebase origin master	--获取远程仓库与本地一致

$ git add test.txt	--将工作区创建的 test.txt 文件添加到暂存区

$ git commit -m "备注信息"	--将暂存区的内容提交到仓库区，-m 为备注的内容

$ git push origin master	--将仓库区的内容推送到远程 GitHub 仓库上
```

