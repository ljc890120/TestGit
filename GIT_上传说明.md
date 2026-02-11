# 上传到 GitHub 的步骤

本地 Git 已初始化并完成首次提交，只差在 GitHub 上建仓并推送。

## 1. 在 GitHub 上新建仓库

1. 打开：https://github.com/new  
2. **Repository name** 填：`TestGit`（或你喜欢的名字）  
3. 选择 **Public**，**不要**勾选 “Add a README”  
4. 点击 **Create repository**

## 2. 若仓库名不是 TestGit

如果新建的仓库名不是 `TestGit`，需要改一下远程地址：

```powershell
git remote set-url origin https://github.com/ljc890120/你的仓库名.git
```

## 3. 推送到 GitHub

在项目目录下执行：

```powershell
cd d:\cursorProject\TestGit
git push -u origin master
```

若 GitHub 提示默认分支是 `main`，可先改本地分支再推送：

```powershell
git branch -M main
git push -u origin main
```

## 4. 之后日常使用

- 改完代码后：`git add .` → `git commit -m "说明"` → `git push`
- 从 GitHub 拉取：`git pull`
