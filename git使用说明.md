## 如何使用git客户端与github的交互 ##
>1. 启动gitbash.exe  
>
> 2. 从github上检出项目  
>> 命令：git clone [url]；  
>> 例如检出绿叶项目：git clone https://github.com/dolphin0224/GreenLeaf.git    
> 
>3.进入项目的根目录：  
>> cd GreenLeaf
>   
>4.将改动的地方添加到版本管理器  
>>(1)git add .    （"."代表添加所有的文件到暂存区）  
>
>>(2)添加一个或多个文件：git add [filename1] [filename2]...  
>
>5.提交到本地的版本控制库；  
>>git  commit -m "inner into a line words"  
>>备注：引号中的字代表提交数据时的说明信息  

>将本地的仓库提交到github上的master分支；  
>>git push -u origin master  
>>备注：点击enter后会弹出框，要求输入github的账号与密码    

>远程同步更新;    
>>$ git fetch    (默认实现所有分支的更新）
>>$ git fetch <远程主机名> <分支名>   （对特定分支的更新）

>删除工作区文件，而且这次删除是放入暂存区  
>>git rm [filename1] [filename2]...  

>改名文件，并且将这个改名放入暂存区
>>$ git mv [file-original] [file-renamed]

>帮助命令
>>git --help  

>查看每次详细修改内容的  
>>git log -p <file>   
>
> 撤销最近的一个提交:  
>>git revert HEAD
#常用的git命令查看链接：
http://www.ruanyifeng.com/blog/2015/12/git-cheat-sheet.html  
><font color=red>如果提交文件时没有更新到最新版本，可以使用命令：  </font> 
>> git pull origin master  或  
>>git pull --rebase origin master
>  
>>备注:git pull等效于get fetch origin和get merge origin/master这两条命令  
>查看文件状态：git status  

<font color=red> # Git 分支  </font>  
git branch  # 查看分支   
git branch  6.x- 1.x  # 添加分支 6.x-1.x     
git branch checkout master  # 切换到主分支   
git branch  -d  6.x- 1.x  # 删除分支 6.x-1.x   
git push origin :branchname  # 删除远端分支 

####注意：  
每个 commit 只改一件事情。如果一个文档有多个变更，使用 git add --patch 只选择文档中的部分变更进入 stage
· 写清楚 commit message