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
>>(1)git add .    
>>(2)添加文件：git add [filename]
>
>5.提交到本地的版本控制库；  
>>git  commit -m "inner into a line words"  
>>备注：引号中的字代表提交数据时的说明信息  

>将本地的仓库提交到github上；  
>>git push -u origin master  
>>备注：点击enter后会弹出框，要求输入github的账号与密码