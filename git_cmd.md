Git Command Notes:
======
1.git init:初始化版本库；   

2.git status:查看版本库的状态，可以检测出当前工作区改动包括：修改、增加、删除；   

3.git diff <filename>:查看被改文件filename的详细改动；   

4.git add <filename>:添加文件file到暂存区(stage)；   

5.git commit -m "discript":提交暂存区里的更改到分支；   

6.git checkout -- <filename>:丢弃工作区的修改；   

7.git reset --hard head^ :回到上一个版本；   

8.git rm <filename>:从版本库中删除文件；   

9.git log:查看由进及远的提交日志，可以加上‘--pretty=oneline’参数，然后在一行内查看较简洁的日志信息:   

>$ git log   

>commit ea34578d5496d7dd233c827ed32a8cd576c5ee85   

>Author: xinyang <xyzheng@gmail.com>   

>Date:   Tue Aug 20 14:53:12 2013 +0800   

>    add distributed   

>commit cb926e7ea50ad11b8f9e909c05226233bf755030   

>Author: xinyang <xyzheng@gmail.com>   

>Date:   Mon Aug 19 17:51:55 2013 +0800   

>    wrote a readme file   

     
>$ git log --pretty=oneline   

>3628164fb26d48395383f8f31179f24e0882e1e0 append GPL   

>ea34578d5496d7dd233c827ed32a8cd576c5ee85 add distributed   

>cb926e7ea50ad11b8f9e909c05226233bf755030 wrote a readme file   


10.git reflog:用来记录每一次操作的命令：   
>$ git reflog   

>ea34578 HEAD@{0}: reset: moving to HEAD^   

>3628164 HEAD@{1}: commit: append GPL   

>ea34578 HEAD@{2}: commit: add distributed   

>cb926e7 HEAD@{3}: commit (initial): wrote a readme file   

11.设置SSH Key：   

>$ ssh-keygen -t rsa -C "your\_email@example.com"   

12.将本地仓库与远程仓库关联：   

>$ git remote add origin git@github.com:xinyangandme/Gostudy.git   

13.关联后就可以把本地仓库的所有内容推送到远程仓库上：   

>git push -u origin master   

以上是第一次将本地仓库的内容推送到远程仓库，之后的推送（即同步）只要如下形式：   

>git push origin master   

14.将远程仓库的最新提交（版本）抓到本地仓库，也就是将远程库同步到本地库，有时多人同时推送时会发生冲突，也要先执行这个操作：  
>git pull   
====
今天先学到这里 2013-12-19 23.05（渐渐熟悉了命令后感觉github桌面版并不好用）   

