### C# 定时器笔记

>下拉框 <br>
>>属性：DropDownStyle 为DropDownList不可输入  为DropDown为可输入<br>
>>Item设置静态文本<br>
>>添加选项：`comboBOX1.Items.Add("");`<br>
><br>Label<br>
>>文本显示:`label1.Text = ""`<br> 
><br>Timer定时器<br>
>>属性：Interal 中断时长（毫秒）<br>
>>定时开始：`timer1.Start()`<br>
>>定时暂停：`timer1.Stop()`<br>
><br>转换工具<br>
>>整型转换：`Convert.toInt32("")`<br>
><br>进度条<br>
>>设置进度条当前值：`progressBar1.value = 1`<br>
>>设置进度条最大值：`progressBar1.Maxnum = 100`<br>
><br>弹窗<br>
>>`MessageBox.show("")`<br>
><br>系统提示音<br>
>>`System.Media.SystemSounds.Asterisk.play()`  