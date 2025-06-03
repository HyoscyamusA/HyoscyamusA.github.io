---
title: Git 基础命令入门教程
date: 2025-06-04
categories: 学习
tags: [Git, 版本控制, 教程]
---

# Git 基础命令入门教程

Git 是目前最流行的版本控制工具，适用于管理代码和文件的修改记录。无论是写博客、开发软件还是管理文档，学会 Git 都非常有用。

## 一、Git 的安装和初始化

1. **安装 Git**  
   - Windows: 去 [Git 官网](https://git-scm.com/download/win)下载安装程序  
   - macOS: 可以用 Homebrew 安装 `brew install git`  
   - Linux: 通过包管理器安装，例如 `sudo apt install git`

2. **初始化仓库**  
   在项目文件夹下执行：

   ```bash
   git init
   ```

这会创建一个新的 Git 仓库。

------

## 二、常用 Git 命令

### 1. 查看当前状态

```

git status
```

查看哪些文件被修改、哪些文件被跟踪。

------

### 2. 添加文件到暂存区

```

git add 文件名
```

例如：

```

git add index.md
```

或者一次添加所有修改：

```
bash


复制编辑
git add .
```

------

### 3. 提交改动

```

git commit -m "简短的提交说明"
```

例如：

```

git commit -m "新增博客首页内容"
```

------

### 4. 连接远程仓库（只需执行一次）

```

git remote add origin 仓库地址
```

例如：

```

git remote add origin https://github.com/用户名/仓库名.git
```

------

### 5. 推送代码到远程仓库

```

git push origin main
```

`main` 是主分支名称，如果你的主分支是 `master`，请替换。

------

### 6. 拉取远程仓库最新代码

```bash

git pull origin main
```

------

## 三、常见问题和技巧

- **如何撤销未提交的修改？**

  ```
  git checkout -- 文件名
  ```

- **查看提交历史**

  ```
  git log
  ```

- **查看某个文件的修改记录**

  ```
  git log - 文件名
  ```