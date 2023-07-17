# 一、初始化设置

````markdown
git -v   //查看版本
git config --global user.name "lphhhhh"  //添加姓名
git config --global user.email lph20020529@gmail.com   //添加邮箱
git config --global credential.helper store  //保存用户名和密码
git config --global --list  //查看用户名和邮箱
````



# 二、新建仓库（Repository   Repo)

1. 找到一个合适的位置创建一个空仓库

2. 输入 git init即可创建仓库

3. 查看是否有git文件

   ````markdown
   ls  //查看目录
   ls -a //查看隐藏目录
   ````

   

# 三、git工作区域

## 1.工作区

1. 本地目录

## 2.暂存区

1. 是一种临时存储区域，用于保存即将提交到Git仓库的修改内容

## 3.本地仓库

1. 二中建立的仓库

## 4.git中的文件状态

1. 未跟踪：还没有被git管理起来的文件
2. 未修改：已经被git管理，但是文件的内容未发生改变
3. 已修改：已经修改了的文件，但是还没有添加到暂存区
4. 已暂存：添加到暂存区内的文件



# 四、将文件添加到仓库里

````markdown
git init  //创建仓库
git status  //查看仓库状态
git add “文件名称”  //添加到暂存区
git add *。文件后缀  //把该文件后置的所有文件添加到暂存区
git add .    //将所有文件添加到暂存区
git commit -m "注释"  //提交，只会提交暂存区的文件而不会提交工作区
git log  //查找提交
````

1. 在Vscode中新建内容
2. 查看仓库状态（此时所有文件为未跟踪状态，显示为红色）
3. 将文件添加至暂存区（此时文件颜色应该未绿色）
4. 提交
5. 查看仓库状态，此时仓库中之前在暂存区的文件应该已经不见了，因为已经被提交了
6. change——first
7. change__second
