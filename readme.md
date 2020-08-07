# readme
+ 项目说明文档
  1. 一般会随着项目放在一起
  2. 作为项目说明文档
  
## git init 
1. 把当前目录初始化为版本库
2. 当前目录下生成一个隐藏文件.git
## git add 文件名
1. 把当前目录下的某个文件提交到暂存区
2. git add readme.md 把这个文件提交到暂存区
3. git add . 当前目录所有变动提交到暂存区
## git status 
1. 查看当前目录提交状态(新增，删除，修改)
## git commit -m '提交注释'
1. 把暂存区的内容提交到本地仓库
## 本地仓库涉及到的三个组成部分
1. 工作区(实际文件目录)
2. 暂存区
3. 本地仓库

## git log 
1. 查看日志
## git reflog
1. 查看操作日志(简单版) 最前面生成的是版本号

## git diff 文件名
1. 查看文件变更信息 

## git reset --hard 版本号
1. 版本回退  --hard 版本号 回退到指定版本
2. HEAD^回退到上一个版本


## 远程仓库
 1. git remote add origin(变量名) 仓库地址 
 把本地仓库与远程仓库关联
 2.git remote -v 查看关联的远程仓库地址  一个本地仓库可以连接多个远程仓库

## 远程提交
1. `git push` 本地仓库提交到远程仓库
2.`git push` -u origin master push到默认的远程仓库
执行一次这个命令，以后可以直接`git push` 提交到默认远程仓库的master分支

## 更新
1. 每次拉取前都要保证工作区全存到了本地仓库。
git.status查看状态 。有修改就add commit
## 远程拉取
1. git pull
:wq 回车 退出编辑模式

## 克隆
`git clone ` 克隆一个仓库到本地

## 创建分支
 `git branch 分支名 `创建分支
## 查看分支
 `git branch` 查看分支  当前分支前面有个*
## 切换分支
 `git checkout 分支名 ` 切换分支
## 分支修改
 分支会拷贝主分支的内容。在分支中修改内容后要提交到本地仓库，在主分支是没有的。在分支中测试无误后再合并到主分支
 
## 主要的操作
1. git init 初始化 创建版本库  只有第一次写
2. git add 文件名  git add . 将文件提交到暂存区
3. git commit -m '注释'   暂存区提交到本地仓库
4. git pull 拉取远程的更新
5.git push 推送到远程仓库
<!-- ## 引入js代码
```js
var  abc = 123;
function say(){
    console.log(abc);
}
```
---
## 引入css代码
```css
.box{
    width:100px;
} -->
