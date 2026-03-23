# Git 常用命令指南

## 1. 克隆仓库 (Clone)

克隆远程仓库到本地：

```bash
git clone <仓库URL>
```

例如：
```bash
git clone https://github.com/1135288997/Test8.git
```

## 2. 初始化仓库 (Init)

在当前目录初始化一个新的git仓库：

```bash
git init
```

## 3. 配置用户信息 (Config)

设置全局用户邮箱和用户名：

```bash
git config --global user.email "your.email@example.com"
git config --global user.name "Your Name"
```

设置当前仓库的用户信息：

```bash
git config user.email "your.email@example.com"
git config user.name "Your Name"
```

## 4. 查看状态 (Status)

查看当前仓库的状态：

```bash
git status
```

## 5. 添加文件 (Add)

添加单个文件到暂存区：

```bash
git add <文件名>
```

添加所有文件到暂存区：

```bash
git add .
```

## 6. 提交更改 (Commit)

提交暂存区的更改：

```bash
git commit -m "提交信息"
```

## 7. 推送代码 (Push)

推送本地分支到远程仓库：

```bash
git push <远程仓库名> <本地分支名>:<远程分支名>
```

例如：
```bash
git push origin master:main
```

设置默认推送分支：

```bash
git push -u origin master:main
```

## 8. 拉取代码 (Pull)

从远程仓库拉取代码并合并到当前分支：

```bash
git pull <远程仓库名> <远程分支名>
```

例如：
```bash
git pull origin main
```

## 9. 查看远程仓库 (Remote)

查看已配置的远程仓库：

```bash
git remote -v
```

添加远程仓库：

```bash
git remote add <远程仓库名> <仓库URL>
```

例如：
```bash
git remote add origin https://github.com/1135288997/Test8.git
```

## 10. 查看分支 (Branch)

查看本地分支：

```bash
git branch
```

查看所有分支（包括远程分支）：

```bash
git branch -a
```

创建新分支：

```bash
git branch <分支名>
```

切换分支：

```bash
git checkout <分支名>
```

## 11. 合并分支 (Merge)

将指定分支合并到当前分支：

```bash
git merge <分支名>
```

## 12. 查看提交历史 (Log)

查看提交历史：

```bash
git log
```

查看简洁的提交历史：

```bash
git log --oneline
```

## 13. 撤销更改 (Reset)

撤销工作区的更改：

```bash
git checkout -- <文件名>
```

撤销暂存区的更改：

```bash
git reset HEAD <文件名>
```

## 14. 标签 (Tag)

创建标签：

```bash
git tag <标签名>
```

推送标签到远程仓库：

```bash
git push origin <标签名>
```

## 15. 发布项目到 GitHub 的完整流程

1. 初始化仓库：
   ```bash
   git init
   ```

2. 配置用户信息：
   ```bash
   git config user.email "your.email@example.com"
   git config user.name "Your Name"
   ```

3. 添加文件：
   ```bash
   git add .
   ```

4. 提交更改：
   ```bash
   git commit -m "Initial commit"
   ```

5. 在 GitHub 上创建新仓库

6. 添加远程仓库：
   ```bash
   git remote add origin https://github.com/your-username/repository-name.git
   ```

7. 推送代码：
   ```bash
   git push -u origin master:main
   ```
