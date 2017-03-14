Git使用指南
在Windows下找到Git Bash并打开

1.配置身份。
git config --global user.name "zhangyang"
git config --global user.email "zhangyang@sis.sh.cn"

2.查看身份
git config --global user.name
git config --global user.email

3.给项目建立代码仓库
进入到项目的目录下面输入git init
仓库创建完成后会生成一个隐藏的.git文件夹

4.查看代码仓库
通过ls -al查看
5.提交代码
    5.1 添加单个文件
    git add build.gradle
    5.2 添加目录
    git add app
    5.3 添加所有文件
    git add .
    5.4 git commit -m "Message"
6.查看分支
git branch
7.创建分支
git branch version1.0  #创建一个名称为version1.0的分支。
8.切换分支
git checkout version1.0
9.合并分支
git checkout master
git merge version1.0   #将version1.0的修改合并到master上。(这里需要自己去解决冲突。解决完冲突后才可以commit)
直接获取某一个分支。GB32960为分支名，后面为远程地址。
git clone -b GB32960 git@192.168.30.46:QTB01/TBoxIntegratedServiceLibs.git


## 与远程版本库协作
1.从远程版本库下载代码到本地
git clone https://github.com/example/test.git
2.本地修改的内容同步到远程库
git push origin master #origin指定的是远程版本库Git的地址。
                       #master指定的是同步到哪一个分支。
3.将远程版本库上的修改同步到本地
git fetch origin master
4.查看远程版本库上修改了哪些东西
git diff origin/master
5.将origin/master分支上的修改合并到主分支上
git merge origin/master
6.从远程版本库上获取最新代码并合并到本地
git pull origin master        #相当于将3和5命令一起执行（fetch和merge）
