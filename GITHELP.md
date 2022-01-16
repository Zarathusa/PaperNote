# 论文笔记

## Git

### Git 全局设置:

```shell
git config --global user.name "Zarathustra"
git config --global user.email "1558769834@qq.com"
```

### 创建 git 仓库:

```shell
mkdir paper-note
cd paper-note
git init
touch README.md
git add README.md
git commit -m "first commit"
git remote add origin https://gitee.com/zarathusa/paper-note.git
git push -u origin master
```

### 已有仓库?

```shell
cd existing_git_repo
git remote add origin https://gitee.com/zarathusa/paper-note.git
git push -u origin master
```

### 第一次pull

~~~shell
git init
git remote add origin https://gitee.com/zarathusa/paper-note.git
git pull origin master
~~~



### Git基本操作

~~~shell
git add .   # 添加文件到暂存区。
git commit -m "message"  # 将暂存区内容添加到仓库中。 
git push -u origin master

# 更新操作
git pull origin master
~~~
### 分支操作

####  1. 新建分支

```shell
git checkout -b [分支名（注意不带中括号）]
```

#### 2. 切换分支

```shell
git checkout [分支名（注意不带中括号）]
```

#### 3. 提交修改

```shell
// 提交所有修改
git add .

// 提交部分修改
git add '文件路径，多个文件用，隔开（带引号）'
```

#### 4. 添加本地提交的注释

```shell
git commit -m '注释内容（带引号）'
```

#### 5. 提交修改

```shell
git push

// 新分支首次提交绘提示设置提交的分支源
git push --set-upstream origin [分支名（注意不带中括号）]
```

#### 6. 合并分支

```shell
// 合并 test 分支到 master
// 先切换到master分支, 然后再合并目标分支, 最后再提交合并
git checkout master
git merge test
git push
```

# 博客地址

https://blog.csdn.net/weixin_44420955/
