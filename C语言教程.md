# C语言教程

## 目录

* Visual Studio Code及其配置
  
  * 如何运行代码
  
  * 断点调试
* C语言程序构成
* 注释
* 关键字
* 标识符
* C语言数据类型
* 常量 
* 输出
  
  * printf函数
  
  * putchar和getchar
* 变量
  
  - extern关键字
  
  - static关键字
  
  - auto和register关键字
* scanf函数
* 运算符
  
  * 算术运算符
  
  * 赋值运算符
  
  * 自增自减运算符
  
  * sizeof运算符
  
  * strlen函数
  
  * 逗号运算符
  
  * 关系运算符
  
  * 逻辑运算符
  
  * 三目运算符
* 数据类型转换
* 选择结构
* 循环结构
  
  * 四大跳转
  
  * 循环的嵌套
  
  * 图形打印
* 函数
  
  * 函数的定义
  
  * 函数的声明与实现
  
  * argc、argv[ ]
  
  * 递归函数
* 位运算符
* 转义字符
* 类型说明符
  
  * short和long
  
  * signed和unsigned
* 一维数组
  
  * 数组的遍历
  
  * 数组长度的计算
  
  * 数组越界
  
  * 数组和函数
* 二维数组
  
  * 二维数组的遍历
  
  * 二维数组的存储

  * 二维数组与函数
* 字符串
* 指针

  * 指针变量
  * 指针变量的运算
  * 数组指针
  * 字符串指针
  * 指针与函数
  * 二级指针
  * 指针数组
  * 二维数组指针
  * 函数指针
* 结构体

  * 结构体数组

  * 结构体指针

  * 结构体内存分析

  * 结构体嵌套

  * 结构体和函数
* 位域（位段）
* 共用体
* 枚举
* 预处理命令
  * #include用法详解
* 宏
* 条件编译
* typedef关键字
  * 宏与typedef关键字的区别
* const关键字
* 内存管理

  * 栈内存（stack）

  * 堆内存（heap）

  * malloc函数

  * free函数

  * calloc函数

  * realloc函数
* 链表

  * 静态链表

  * 动态链表

  * 链表优化

  * 链表销毁

  * 链表长度计算

  * 链表查找

  * 链表删除
* 计数排序
* 选择排序
* 冒泡排序
* 插入排序
* 折半查找

  * 进制转换（查表法）
* 希尔排序
* 文件
  
  * 文件的打开与关闭
  
  * 一次读写一个字符
  
  * 一次读写一行字符
  
  * 一次读写一块数据
  
  * 读写结构体
  
  * 其他文件操作函数
* C标准库

# Visual Studio Code及其配置

       编写代码不是一件随便的事情，要想编写好代码，不仅得有好的技术，还得有一个趁手的编写代码的工具。Clion就是编写C/C++的一个很好用的IDE（集成开发环境），但是Clion是要收费的，这点让人望而却步。Visual Studio也很好用，但是太大了，很臃肿。而Visual Studio Code是一个免费且好用的文本编辑器，通过插件可以将其打造成为一个IDE。

![](D:\Programmering Learning\Markdown文档\C语言教程\图片\Clion.png)

​                                                                                                        Clion

![](D:\Programmering Learning\Markdown文档\C语言教程\图片\vs.png)

​                                                                                                       Visual Studio

![](D:\Programmering Learning\Markdown文档\C语言教程\图片\vscode.png)

​                                                                                                 Visual Studio Code

1. 安装vscode
   
   官网：[Visual Studio Code - Code Editing. Redefined](https://code.visualstudio.com/))
   
   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\vscode官网.png)
   
   选择对应的系统版本进行下载即可。下载完成以后默认设置安装即可。**切记，不要将软件安装在C盘，一定要改默认路径。**
   
   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\vscode安装01.png)
   
   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\vscode安装02.png)
   
   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\vscode安装03.png)

2. 下载mingw64
   
      mingw64是C/C++编译器gcc在Windows上的发行形式。C/C++的编译器还有很多，比如说clang。
   
   下载地址：https://pan.baidu.com/s/1lXnBx6gTh-IO6XCplo8DcQ
   
   提取密码：8888

3. 配置环境
   
   【windows10以下版本系统（不含windows10）】
   
   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\配置环境01.png)
   
   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\配置环境02.png)
   
   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\配置环境03.png)
   
   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\配置环境04.png)
   
   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\配置环境05.png)
   
   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\配置环境06.png)
   
      最后编辑的时候在最后面加上一个分号，然后将mingw64中的bin目录的路径（例如：F:\mingw64\bin）粘贴进去。
   
   【windows10/11】
   
    右键我的电脑，点击属性
   
   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\配置环境07.png)
   
   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\配置环境08.png)
   
   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\配置环境09.png)
   
   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\配置环境10.png)
   
   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\配置环境11.png)
   
   将mingw64的路径（例如：F:\mingw64\bin）粘贴进去，最后确定保存就行。

4. 配置vscode
   
      打开vscode，Ctrl+Shift+X打开插件市场，在搜索框里输入Chinese，选择第一个安装，安装过后右下角会有重启软件提示，点击restart重启即可，重启过后界面即为中文界面。
   
   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\配置环境12.png)
   
   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\配置环境13.png)
   
      打开插件市场，安装C/C++插件。
   
      在C盘之外创建一个英文名的文件夹，路径之中不可含有英文，文件夹名称不可含有中文。然后在创建好的文件夹里面再创建一个.vscode文件夹（注意不要把点忘记了）。然后打开vscode，点击左上角的文件，打开文件夹，打开事先创建好的文件夹。
   
   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\配置环境14.png)
   
   点击展开.vscode文件夹，点击上方的加号创建c_cppproperties.json、launch.json、settings.json、tasks.json四个文件。
   
   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\配置环境15.png)

5. 配置文件（C）
   
   c_cpp_properties.json
   
   ```javascript
   {
       "configurations": [
           {
               "name": "Win32",
               "includePath": [
                   "${workspaceFolder}/**"
               ],
               "defines": [
                   "_DEBUG",
                   "UNICODE",
                   "_UNICODE"
               ],
               "windowsSdkVersion": "10.0.17763.0",
               "compilerPath": "D:\\programmering software\\mingw64\\bin\\gcc.exe", //需改成自己的路径
               "cStandard": "c11",
               "cppStandard": "c++17",
               "intelliSenseMode": "${default}",
               "compilerArgs": [
                   "-fexec-charset=GBK"
               ]
           }
       ],
       "version": 4
   }
   ```
   
   launch.json
   
   ```javascript
   {
       // 使用 IntelliSense 了解相关属性。 
       // 悬停以查看现有属性的描述。
       // 欲了解更多信息，请访问: https://go.microsoft.com/fwlink/?linkid=830387
       "version": "0.2.0",
       "configurations": [
           {
               "name": "gcc.exe - 生成和调试活动文件",
               "type": "cppdbg",
               "request": "launch",
               "program": "${fileDirname}\\${fileBasenameNoExtension}.exe",
               "args": [],
               "stopAtEntry": false,
               "cwd": "D:\\programmering software\\mingw64\\bin", //需改成自己的路径
               "environment": [],
               "externalConsole": true,
               "MIMode": "gdb",
               "miDebuggerPath": "D:\\programmering software\\mingw64\\bin\\gdb.exe", //需改成自己的路径
               "setupCommands": [
                   {
                       "description": "为 gdb 启用整齐打印",
                       "text": "-enable-pretty-printing",
                       "ignoreFailures": true
                   },
                   {
                       "description": "将反汇编风格设置为 Intel",
                       "text": "-gdb-set disassembly-flavor intel",
                       "ignoreFailures": true
                   }
               ],
               "preLaunchTask": "C/C++: gcc.exe 生成活动文件"
           }
       ]
   }
   ```
   
   settings.json
   
   ```javascript
   {
       "files.associations": {
           "stdlib.h": "c",
           "stdio.h": "c",
       },
       "docwriter.progress.trackMethods": false,
       "docwriter.progress.trackFunctions": true,
       "C_Cpp.errorSquiggles": "disabled",
       "rainbowString": {
           "extensions": [
               ".cs",
               ".csx",
               ".fs",
               ".fsx",
               ".js",
               ".jsx",
               ".ts",
               ".tsx",
               ".csproj",
               ".fsproj"
           ]
       }
   }
   ```
   
   tasks.json
   
   ```javascript
   {
       "version": "2.0.0",
       "tasks": [
           {
               "type": "shell",
               "label": "task g++",
               "command": "D:\\programmering software\\mingw64\\bin\\gcc.exe", //需改成自己的路径
               "args": [
                   "-g",
                   "${file}",
                   "-o",
                   "${fileDirname}\\${fileBasenameNoExtension}.exe",
                   "-I",
                   "D:\\programmering software\\mingw64\\vscode", //需改成自己的路径
                   "-std=c++17"
               ],
               "options": {
                   "cwd": "D:\\programmering software\\mingw64\\bin" //需改成自己的路径
               },
               "problemMatcher": [
                   "$gcc"
               ],
               "group": "build"
           },
           {
               "type": "cppbuild",
               "label": "C/C++: gcc.exe 生成活动文件",
               "command": "D:\\programmering software\\mingw64\\bin\\gcc.exe", //需改成自己的路径
               "args": [
                   "-fdiagnostics-color=always",
                   "-g",
                   "${file}",
                   "-o",
                   "${fileDirname}\\${fileBasenameNoExtension}.exe",
                   "-fexec-charset=GBK"
               ],
               "options": {
                   "cwd": "D:\\programmering software\\mingw64\\bin" //需改成自己的路径
               },
               "problemMatcher": [
                   "$gcc"
               ],
               "group": {
                   "kind": "build",
                   "isDefault": true
               },
               "detail": "调试器生成的任务。"
           }
       ]
   }
   ```

6. 配置文件（C++）
   
    其他配置文件都相同，只是tasks.json文件需稍作改动
   
   tasks.json
   
   ```javascript
   {
       "version": "2.0.0",
       "tasks": [
           {
               "type": "shell",
               "label": "task g++",
               "command": "D:\\programmering software\\mingw64\\bin\\g++.exe", //需改成自己的路径
               "args": [
                   "-g",
                   "${file}",
                   "-o",
                   "${fileDirname}\\${fileBasenameNoExtension}.exe",
                   "-I",
                   "D:\\programmering software\\mingw64\\vscode", //需改成自己的路径
                   "-std=c++17"
               ],
               "options": {
                   "cwd": "D:\\programmering software\\mingw64\\bin" //需改成自己的路径
               },
               "problemMatcher": [
                   "$gcc"
               ],
               "group": "build"
           },
           {
               "type": "cppbuild",
               "label": "C/C++: gcc.exe 生成活动文件",
               "command": "D:\\programmering software\\mingw64\\bin\\g++.exe", //需改成自己的路径
               "args": [
                   "-fdiagnostics-color=always",
                   "-g",
                   "-std=c++23",
                   "${file}",
                   "-o",
                   "${fileDirname}\\${fileBasenameNoExtension}.exe",
                   "-fexec-charset=GBK"
               ],
               "options": {
                   "cwd": "D:\\programmering software\\mingw64\\bin" //需改成自己的路径
               },
               "problemMatcher": [
                   "$gcc"
               ],
               "group": {
                   "kind": "build",
                   "isDefault": true
               },
               "detail": "调试器生成的任务。"
           }
       ]
   }
   ```

## 如何运行代码

![](D:\Programmering Learning\Markdown文档\C语言教程\图片\运行代码01.png)

![](D:\Programmering Learning\Markdown文档\C语言教程\图片\运行代码02.png)

## 断点调试

有些时候，我们写的代码出现了问题，我们可能就会用到断点调试。断点调试可以监视变量的值以及数组中的值的变化。

![](D:\Programmering Learning\Markdown文档\C语言教程\图片\断点调试01.png)

![](D:\Programmering Learning\Markdown文档\C语言教程\图片\断点调试02.png)

# C语言程序构成

C语言基本结构包括头文件，主函数。下图是一个最简单的C语言程序。

C语言的每个语句都以分号   ;    结束。

C语言文件的后缀名为.c

注：C语言的文件路径、文件名中不可含有中文，否则会编译错误。

![](D:\Programmering Learning\Markdown文档\C语言教程\图片\1-1 C语言结构02.png)

**注**：其中system（“pause”）可以省略，这段指令包含在库文件stdlib.h中，但是上面的vscode配置为外置终端显示运行结果，如果不添加这两行代码，就会出现运行结果一闪而过的情况，这两段代码的作用就是暂停程序的执行，使得你能够看到运行结果。

    #include 是引入头文件的意思。

# 注释

   好的代码不只是你自己能看懂，还应当能够让别人看懂。在企业当中一个大的项目的开发往往会分工很多人进行开发，这时候你的代码就不能只是让你自己能够看懂，还应能让他人看懂。此时，注释就显得尤为重要。同时，**注释也能够帮助你自己理解代码，避免代码量较大的时候出现自己写的代码自己不理解的情况。**

   在代码运行的时候，编译器会自动忽略注释部分，也就是说注释是写给人看的，不是写给机器看的。

1. 单行注释
   
   在代码前面加上双斜杠  //  即代表注释改行。
   
   ```c
   //思路：现将时间转换成分钟，再按分钟计算，最后转换成题设形式
   #include <stdio.h>
   
   int main()
   {
       //输入当前时间与经过的时间
       int start_time,add_time;
       scanf("%d%d",&start_time,&add_time);
       //计算最终时间
       int min=(start_time/100)*60+start_time%100;
       int final_time=min+add_time;
       //输出最终时间
       if(final_time%60>=10)
       {
           printf("%d%d",final_time/60,final_time%60);
       }
       else
       {
           printf("%d0%d",final_time/60,final_time%60);
       }
   
       return 0;
   }
   ```

2. 多行注释
   
   用 /* */ 将代码括住，即代表多行注释。
   
   注意：多行注释里面不能套用多行注释，套用的话就会因为无法确定范围而错乱。
   
   ```c
   //思路：现将时间转换成分钟，再按分钟计算，最后转换成题设形式
   /* #include <stdio.h>
   
   int main()
   {
       //输入当前时间与经过的时间
       int start_time,add_time;
       scanf("%d%d",&start_time,&add_time);
       //计算最终时间
       int min=(start_time/100)*60+start_time%100;
       int final_time=min+add_time;
       //输出最终时间
       if(final_time%60>=10)
       {
           printf("%d%d",final_time/60,final_time%60);
       }
       else
       {
           printf("%d0%d",final_time/60,final_time%60);
       }
   
       return 0;
   } */
   ```

# 关键字

1. 关键字，也叫作保留字。是指一些被C语言赋予了特殊含义的单词。

2. 特点：全部为小写，在编辑器中会有不同颜色的高亮。

3. 注意点：关键字在C语言中均有特殊含义，不可用于变量名。

4. C语言中的32个关键字
   
   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\关键字.png)

5. 关键字的分类
   
   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\关键字分类.png)

# 标识符

1. 标识符就是写程序时给函数、变量的命名。

2. 标识符命名规则：
   
   1. 只能由字母(a~z、 A~Z)、数字、下划线组成；
   
   2. 不能包含除下划线以外的其它特殊字符串；
   
   3. 不能以数字开头；
   
   4. 不能是C语言中的关键字；
   
   5. 标识符严格区分大小写, test和Test是两个不同的标识符；

3. 标识符命名规范
   
   驼峰命名法：当变量名或函数名是由多个单词连接在一起,构成标识符时,第一个单词以小写字母开始;第二个单词的首字母大写。例：Start_time、FirstName。

# C语言数据类型

C语言4大数据类型：基本类型、构造类型、指针类型、空类型。

![](D:\Programmering Learning\Markdown文档\C语言教程\图片\C语言数据类型.png)

```c
1 B(Byte字节) = 8 bit(位)
    // 00000000 就是一个字节
    // 11111111 也是一个字节
    // 10101010 也是一个字节
    // 任意8个0和1的组合都是一个字节
1 KB(KByte) = 1024 B
1 MB = 1024 KB
1 GB = 1024 MB
1 TB = 1024 GB
```

# 常量

1. 常量即固定不变的数据，不能改变。比如说人的性别就是一个常量，人生下来之后，人的性别就定了，不能改变（不讨论变性人）。

2. 常量的类型
   
   1. 整型常量
   
   2. 实型常量
      
      1. 小数形式
         
         1. 单精度：以字母f或F结尾。如：0.0f、1.01f。
         
         2. 双精度：十进制小数形式。如：3.14、7.28.
      
      2. 指数形式：以幂的形式表示, 以字母e或字母E后跟一个10为底的幂数。如3.14e10，即表示3.14乘10的10次方。
         
         **注意：1. 字母e或字母E后面的指数必须为整数；2. 字母e或字母E前后必须要有数字；3. 字母e或字母E前后不能有空格**
   
   3. 字符常量
      
         字符型常量都是用''(单引号)括起来的。例如:'a'、'b'、'c'。字符常量的单引号中只能有一个字符。
      
         **特殊情况**: 如果是转义字符,单引号中可以有两个字符。例如:'\n'、'\t'。
      
      **注：‘\0’是字符常量，"0"是字符串常量，0是整型常量。**
   
   4. 字符串常量
      
      字符型常量都是用""(双引号)括起来的。例如:"a"、"abc"、"lnj"。
      系统会自动在字符串常量的末尾加一个字符'\0'作为字符串结束标志。
   
   5. 自定义常量

# 输出

## printf函数

1. printf函数称之为格式输出函数,方法名称的最后一个字母f表示format。其功能是按照用户指定的格式,把指定的数据输出到屏幕上、

2. 调用格式：
   
   ```c
   printf("格式控制字符串",输出项列表 );
   
   printf("a = %d, b = %d",a, b);
   ```

3. 格式控制字符串：
   
   形式：`%[标志][输出宽度][.精度][长度]类型。`
   
   格式：
   
   ```c
   printf("a = %类型", a);
   ```
   
   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\类型字符串.png)

4. 示例
   
   ```c
   #include <stdio.h>
   
   int main()
   {    
       int a = 10;    
       int b = -10;    
       float c = 6.6f;    
       double d = 3.1415926;    
       double e = 10.10;    
       char f = 'a';    
       // 有符号整数(可以输出负数)    
       printf("a = %d\n", a); // 10    
       printf("a = %i\n", a); // 10    
       // 无符号整数(不可以输出负数)    
       printf("a = %u\n", a); // 10    
       printf("b = %u\n", b); // 429496786    
       // 无符号八进制整数(不可以输出负数)    
       printf("a = %o\n", a); // 12    
       printf("b = %o\n", b); // 37777777766    
       // 无符号十六进制整数(不可以输出负数)    
       printf("a = %x\n", a); // a    
       printf("b = %x\n", b); // fffffff6    
       // 无符号十六进制整数(不可以输出负数)    
       printf("a = %X\n", a); // A    
       printf("b = %X\n", b); // FFFFFFF6    
       // 单、双精度浮点数(默认保留6位小数)    
       printf("c = %f\n", c); // 6.600000    
       printf("d = %lf\n", d); // 3.141593
       // 以指数形式输出单、双精度浮点数    
       printf("e = %e\n", e); // 1.010000e+001    
       printf("e = %E\n", e); // 1.010000E+001        
       // 以最短输出宽度,输出单、双精度浮点数    
       printf("e = %g\n", e); // 10.1    
       printf("e = %G\n", e); // 10.1        
       // 输出字符    
       printf("f = %c\n", f); // a
   
       return 0;
   }
   ```

5. 宽度
   
   1. 格式：`printf("a = %[宽度]类型", a);`
      
      用十进制整数来指定输出的宽度, 如果实际位数多于指定宽度,则按照实际位数输出, 如果实际位数少于指定宽度则以空格补位。
      
      ```c
      #include <stdio.h>
      
      int main()
      {    
          // 实际位数小于指定宽度    
          int a = 1;    
          printf("a =|%d|\n", a); // |1|    
          printf("a =|%5d|\n", a); // |    1|    
          // 实际位数大于指定宽度    
          int b = 1234567;    
          printf("b =|%d|\n", b); // |1234567|    
          printf("b =|%5d|\n", b); // |1234567|
      
          return 0;
      }
      ```
   
   2. 标志：`printf("a = %[标志][宽度]类型", a);`
   
      ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\宽度标志.png)
   
      ```C
      #include <stdio.h>
      
      int main()
      {
          int a = 1;
          int b = -1;
          // -号标志
          printf("a =|%d|\n", a); // |1|    
          printf("a =|%5d|\n", a); // |    1|    
          printf("a =|%-5d|\n", a);// |1    |    
          // +号标志    
          printf("a =|%d|\n", a); // |1|    
          printf("a =|%+d|\n", a);// |+1|    
          printf("b =|%d|\n", b); // |-1|    
          printf("b =|%+d|\n", b);// |-1|    
          // 0标志    
          printf("a =|%5d|\n", a); // |    1|    
          printf("a =|%05d|\n", a); // |00001|    
          // 空格标志    
          printf("a =|% d|\n", a); // | 1|    
          printf("b =|% d|\n", b); // |-1|    
          // #号    
          int c = 10;    
          printf("c = %o\n", c); // 12    
          printf("c = %#o\n", c); // 012    
          printf("c = %x\n", c); // a    
          printf("c = %#x\n", c); // 0xa
      
          return 0;
      }
      ```

      
   
6. 精度
   
   1. 格式：``printf("a = %[精度]类型", a);``
   
   2. 精度格式符以"."开头, 后面跟上十进制整数, 用于指定需要输出多少位小数, 如果输出位数大于指定的精度, 则删除超出的部分
   
   3. 示例
      
      ```c
      #include <stdio.h>
      
      int main()
      {    
          double a = 3.1415926;    
          printf("a = %.2f\n", a); // 3.14
      
          return 0;
      }
      ```
   
   4. 动态指定小数保留位数
      
      1. 格式：`printf("a = %.*f", a);`
      
      2. 示例
         
         ```c
         #include <stdio.h>
         
         int main()
         {    
             double a = 3.1415926;    
             printf("a = %.*f", 2, a); // 3.14
         
             return 0;
         }
         ```
   
   5. 实型(浮点类型)有效位数问题
      
      1. 对于单精度数,使用%f格式符输出时,仅前6~7位是有效数字
      
      2. 对于双精度数,使用%lf格式符输出时,前15~16位是有效数字
      
      3. 有效位数和精度(保留多少位)不同, 有效位数是指从第一个非零数字开始,误差不超过本数位半个单位的、精确可信的数位
      
      4. 有效位数包含小数点前的非零数位
      
      5. 示例
         
         ```c
         #include <stdio.h>
         int main()
         {    
             //        1234.567871093750000    
             float a = 1234.567890123456789;    
             //         1234.567890123456900    
             double b = 1234.567890123456789;    
             printf("a = %.15f\n", a); // 前8位数字是准确的, 后面的都不准确    
             printf("b = %.15f\n", b); // 前16位数字是准确的, 后面的都不准确
         
             return 0;
         }
         ```

7. 长度
   
   1. 格式：`printf("a = %[长度]类型", a);`
      
      ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\长度.png)
   
   2. 示例
      
      ```c
      #include <stdio.h>
      
      int main()
      {
          char a = 'a';
          short int b = 123;
          int c = 123;
          long int d = 123;
          long long int e = 123;
          printf("a = %hhd\n", a); // 97
          printf("b = %hd\n", b); // 123
          printf("c = %d\n", c); // 123
          printf("d = %ld\n", d); // 123
          printf("e = %lld\n", e); // 123
      
          return 0;
      }
      ```

8. 转义字符
   
   1. 格式：`printf("%f%%", 3.1415);`
   
   2. %号在格式控制字符串中有特殊含义, 所以想输出%必须添加一个转移字符
   
   3. 示例
      
      ```c
      #include <stdio.h>
      
      int main()
      {
          printf("%f%%", 3.1415); // 输出结果3.1415%
      
          return 0;
      }
      ```

## putchar和getchar

1. putchar: 向屏幕输出一个字符
   
   ```c
   #include <stdio.h>
   
   int main()
   {    
       char ch = 'a';    
       putchar(ch); // 输出a
   
       return 0;
   }
   ```

2. getchar: 从键盘获得一个字符
   
   ```c
   #include <stdio.h>
   
   int main()
   {    
       char ch;    
       ch = getchar();// 获取一个字符    
       printf("ch = %c\n", ch);
   
       return 0;
   }
   ```

# 变量

1. 变量表是一些不固定的数据，可以改变。

2. 定义变量
   
   ```c
   格式1：变量类型 变量名称 ;
   
   int a;
   float b;
   char ch;
   ```
   
   ```c
   格式2：变量类型 变量名称,变量名称;
       连续定义, 多个变量之间用逗号(,)号隔开
   
   int a,b,c;
   ```

3. 变量的初始化
   
   ```c
   //先定义，后初始化
   int num;
   num1=520;
   
   //同时定义与初始化
   int num2=520;
   
   //这里面的“=”不是数学里面的等号，而是赋值运算符，表示将后面的值赋给前面的变量/常量
   //如果不初始化，变量里面存储的就会是随机数、上次程序分配的存储空间,存数一些 内容,“垃圾”、系统正在用的一些数据变量值的修改多次赋值覆盖原来的值 
   ```

4. 变量值的修改
   
   多次赋值覆盖
   
   ```c
   int i=10;
   i=20;//赋值过后i的值
   ```

5. 变量之间的值传递
   
   ```c
   int a=10;
   int b;
   b=a;//b=10
   ```

6. 变量的作用域
   
   1. 局部变量（内部变量）
      
      `局部变量是在代码块内定义的, 其作用域仅限于代码块内, 离开该代码块后无法使用。进入作用域变量创建，出作用域变量自动销毁。`
      
      ```c
      #include <stdio.h>
      
      int main()
      {
          int i = 998; // 作用域开始
      
          return 0;// 作用域结束
      }
      ```
      
      ```c
      #include <stdio.h>
      
      int main()
      {
          {
              int i = 998; // 作用域开始
          }// 作用域结束
          printf("i = %d\n", i); // 不能使用
      
          return 0;
      }
      ```
      
      ```c
      #include <stdio.h>
      
      int main()
      {
          {
              {
                  int i = 998;// 作用域开始
              }// 作用域结束
              printf("i = %d\n", i); // 不能使用
          }
      
          return 0;
      }
      ```
   
   2. 全局变量（外部变量）
      
      全局变量的作用域是整个工程。
      
      ```c
      #include <stdio.h>
      
      int i = 666;
      
      int main()
      {
          printf("i = %d\n", i); // 可以使用
      
          return 0;
      }// 作用域结束
      
      int call()
      {
          printf("i = %d\n", i); // 可以使用
      
          return 0;
      }
      ```
      
      注：同一作用域范围内不能有相同名称的变量。
      
      ```c
      #include <stdio.h>
      
      int main()
      {
          int i = 998; // 作用域开始
          int i = 666; // 报错, 重复定义
      
          return 0;
      }// 作用域结束
      ```
      
      ```c
      #include <stdio.h>
      
      int i = 666;
      int i = 998; // 报错, 重复定义
      
      int main()
      {
          return 0;
      }
      ```
      
      注：不同作用域可以有相同名称的变量
      
      ```c
      #include <stdio.h>
      
      int i = 666;
      
      int main()
      {
          int i = 998; // 不会报错
      
          return 0;
      }
      ```
      
      ```c
      #include <stdio.h>
      
      int main()
      {
          int i = 998; // 不会报错
          
          return 0;
      }
      
      int call()
      {
          int i = 666; // 不会报错
      
          return 0;
      }
      ```

7. 变量内存分析
   
   1. 变量存储占用空间
   
   ![](D:\Programmering%20Learning\Markdown文档\C语言教程\图片\变量内存分析.png)
   
   2. 变量存储过程
      
         根据定义变量时声明的类型和当前编译环境确定需要开辟多大存储空间；在内存中开辟一块存储空间，开辟时从内存地址大的开始开辟（内存寻址从大到小）；将数据保存到已经开辟好的对应内存空间中。
      
      ```c
      #include <stdio.h>
      
      int main()
      {
          int num;
          char ch;
          double num_lf;
          float num_f;
      
          printf("%p\n",&num);
          printf("%p\n",&ch);
          printf("%p\n",&num_lf);
          printf("%p\n",&num_f);
      
          return 0;
      }
      ```
      
      ![](D:\Programmering%20Learning\Markdown文档\C语言教程\图片\变量内存分析_地址01.png)
      
      ![](D:\Programmering%20Learning\Markdown文档\C语言教程\图片\变量内存分析_地址02.png) 
      
      **注：每次运行代码，变量的内存地址都是随机分配的，所以每次运行的结果都不一样。**

## extern关键字

全局变量和函数具有外部连接属性。在一个项目当中 ，源文件不会只有一个，而是会有很多个，这时候我们就可能会使用别的源文件中的变量，但是又不能直接使用，这时候只需要使用extern关键字对变量进行声明即可。

**注：声明的结尾处必须加分号“;”。**

![](D:\Programmering%20Learning\Markdown文档\C语言教程\图片\extern声明01.png)

![](D:\Programmering%20Learning\Markdown文档\C语言教程\图片\extern声明02.png)

注：extern对局部变量没用。extern代表声明一个变量, 而不是定义一个变量, 变量只有定义才会开辟存储空间。所以如果是局部变量, 虽然提前声明有某个局部变量, 但是局部变量只有执行到才会分配存储空间。 

## static关键字

1. 对局部变量：static关键字可以使局部变量在出作用域之后不销毁，但其本质上还是局部变量，在作用域之外不可直接使用。对局部变量，static改变的是局部变量的存储位置。
   
   在内存当中，有三个分区，分别是栈区、堆区和静态区，栈区放的就是局部变量等，静态区放的是静态变量，全局变量。static修饰之后，在创建变量分配内存的时候，就会将变量存放在静态区，被修饰的局部变量在出作用域之后不会立即被销毁，而是在程序结束之后销毁。
   
   ```c
   //输出结果为10个2
   #include <stdio.h>
   
   int fuc()
   {
       int a=1;
       a++;
       printf("%d ",a);
   }
   
   int main()
   {
       int i=0;
       while(i<10)
       {
           fuc();
           i++;
       }
   
       return 0;
   }
   ```
   
   ```c
   //输出结果为2 3 4 5 6 7 8 9 10 11
   #include <stdio.h>
   
   int fuc()
   {
       static int a=1;
       a++;
       printf("%d ",a);
   }
   
   int main()
   {
       int i=0;
       while(i<10)
       {
           fuc();
           i++;
       }
   
       return 0;
   }
   ```

2. 对全局变量：全局变量具有外部链接属性，在一个项目当中，其他源文件中的全局变量是可以在当前源文件中引用，只需声明一下即可。static关键字可以使全局变量的外部连接属性变为内部链接属性。
   
   ![](D:\Programmering%20Learning\Markdown文档\C语言教程\图片\static关键字01.png)
   
   ![](D:\Programmering%20Learning\Markdown文档\C语言教程\图片\static关键字02.png)

3. 对函数：函数具有外部链接属性，在一个项目当中，其他源文件中的函数是可以在当前源文件中引用，只需声明一下即可。static关键字可以使函数的外部连接属性变为内部链接属性。
   
   ![](D:\Programmering%20Learning\Markdown文档\C语言教程\图片\static关键字03.png)
   
   ![](D:\Programmering%20Learning\Markdown文档\C语言教程\图片\static关键字04.png)

## auto和register关键字

1. auto（自动）关键字
   
   在变量的作用域那里说过，局部变量在进入作用域之后创建，出作用域之后销毁。那么是什么控制的这个过程，这个auto关键字就是这么一个作用，auto修饰局部变量且只能修饰局部变量，自动控制变量的创建和销毁。可以在定义局部变量的时候在前面加上一个auto，但是没必要，因为在创建局部变量的时候，编辑器会自动在局部变量前面加上auto。所以这个关键字可以说没什么用。
   
   **注：只能修饰局部变量！！！**
   
   ```c
   auto int num;
   等价于
   int num;
   ```

2. register关键字
   
   register关键字与auto关键字一样，也是**只能修饰局部变量**。register关键字的功能就是 将内存中变量提升到CPU寄存器中存储, 这样访问速度会更快。但是由于CPU寄存器数量相当有限, 通常不同平台和编译器在优化阶段会自动转换为auto。
   
   ```c
   register int num;
   ```

# scanf函数

1. scanf函数用于接收键盘输入的内容, 是一个阻塞式函数,程序会停在scanf函数出现的地方, 直到接收到数据才会执行后面的代码。

2. 格式：`scanf("格式控制字符串", 地址列表);`

   例：`scanf("%d",%num);`

3. 基本用法

   1. 地址列表项中只能传入变量地址, 变量地址可以通过&符号+变量名称的形式获取。
      
      ```c
      #include <stdio.h>
      
      int main()
      {
          int number;
          scanf("%d", &number); // 接收一个整数
          printf("number = %d\n", number);
      
          return 0;
      }
      ```

   2. 接收非字符和字符串类型时, 空格、Tab和回车会被忽略。
      
      ```c
      #include <stdio.h>
      
      int main()
      {
          float num;
          // 例如:输入 Tab 空格 回车 回车 Tab 空格 3.14 , 得到的结果还是3.14
          scanf("%f", &num);
          printf("num = %f\n", num);
      
          return 0;
      }
      ```

   3. 接收多条数据
      
      格式控制字符串和地址列表项在数量和类型上必须一一对应。
      
      ```c
      #include <stdio.h>
      
      int main()
      {
          int num;
          char ch;
          double num_f;
      
          //输入数字 空格 字符 空格 双精度数字或者数字 回车 字符 回车 双精度数字
          scanf("%d %c %lf",&num,&ch,&num_f);
      
          printf("%d %c %.2lf\n",num,ch,num_f);
      
          return 0;
      }
      ```
      
      非字符和字符串情况下建议明确指定多条数据之间分隔符。尤其是有字符和字符串的情况下，如果不明确制定多条数据之间分隔符，scanf函数就会读入空格和Tab。
      
      ```c
      #include <stdio.h>
      
      int main()
      {
          int num1,num2;
      
          //输入数字 空格 数字或者数字 回车 数字
          scanf("%d,%d",&num1,&num2);
      
          printf("%d %d\n",num1,num2);
      
          return 0;
      }
      ```

4. 注意：\n是scanf函数的结束符号, 所以格式化字符串中不能出现\n

   ```c
   #include <stdio.h>
   
   int main()
   {
       int num;
   
       //输入完毕按下回车之后无法结束输入
       scanf("%d\n",&num);
   
       printf("%d\n",num);
   
       return 0;
   }
   ```

   但是，下面这种情况格式化字符串能够出现\n，这里的\n作为分隔符，避免scanf函数输入时将空格赋给字符变量。

   ```C
   #include <stdio.h>
   
   int main()
   {
       char str1;
       char str2;
       
       scanf("%c\n%c",&str1,&str2);
       printf("str1 = %c\n",str1);
       printf("str2 = %c\n",str2);
       
       return 0;
   }
   ```

   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\scanf函数01.png)

5. scanf函数运行原理

   系统会将用户输入的内容先放入输入缓冲区。

   scanf方式会从输入缓冲区中逐个取出内容赋值给变量。

   如果输入缓冲区的内容不为空,scanf会一直从缓冲区中获取,而不要求再次输入。

   对于输入的%d、%f、%lf类型的数据，scanf函数会自动过滤掉数据前面的空格。

   <img title="" src="file:///D:/Programmering%20Learning/Markdown文档/C语言教程/图片\scanf函数原理.png" alt="" data-align="center">

6. 清空缓冲区

   1. 利用fflush方法清空缓冲区(不是所有平台都能使用)
      
      ```C
      C和C++的标准里从来没有定义过 fflush(stdin)。MSDN 文档里清楚的描述着"fflush on input stream is an extension to the C standard"（fflush 是在标准上扩充的函数, 不是标准函数, 所以不是所有平台都支持）
      ```
      
      格式： `fflush(stdin);`
      
   2. 利用setbuf方法清空缓冲区(所有平台有效)
      
      格式：` setbuf(stdin, NULL);`

   3. 示例
      
      ```c
      #include <stdio.h>
      
      int main()
      {
          int num1;
          int num2;
          char ch1;
          scanf("%d%c%d", &num1, &ch1, &num2);
          printf("num1 = %d, ch1 = %c, num2 = %d\n", num1, ch1, num2);
          fflush(stdin); // 清空输入缓存区 
          setbuf(stdin, NULL); // 清空输入缓存区
          char ch2;
          int num3;
          scanf("%c%d",&ch2, &num3);
          printf("ch2 = %c, num3 = %d\n", ch2, num3);
      
          return 0;
      }
      ```

# 运算符

 C语言中的运算符是告诉程序执行特定算术或逻辑操作的符号。

1. 运算符分类
   
   1. 按照功能划分
      
      算术运算符、赋值运算符、关系运算符、逻辑运算符、位运算符。
   
   2. 按照参与运算的操作数个数划分
      
      单目运算符（如：i++）、双目运算符（如：a+b）、三目运算符（如：a>b?1:0）。

2. 运算符的优先级和结合性
   
   ![](D:\Programmering%20Learning\Markdown文档\C语言教程\图片\位运算符的优先级和结合性01.png)
   ![](D:\Programmering%20Learning\Markdown文档\C语言教程\图片\位运算符的优先级和结合性02.png)

## 算术运算符

![](D:\Programmering%20Learning\Markdown文档\C语言教程\图片\算术运算符.png)

1. 如果参与运算的两个操作数皆为整数, 那么结果也为整数；如果参与运算的两个操作数其中一个是浮点数, 那么结果一定是浮点数。
   求余运算符, 本质上就是数学的商和余"中的余数；参与运算的两个操作数必须都是整数, 不能包含浮点数；被除数小于除数, 那么结果就是被除数；运算结果的正负性取决于被除数,跟除数无关, 被除数是正数结果就是正数,被除数是负数结果就是负数； 被除数为0, 结果为0。

2. 示例
   
   ```c
   #include <stdio.h>
   
   int main()
   {    
       int a = 10;    
       int b = 5;    
       // 加法    
       int result = a + b;    
       printf("%i\n", result); // 15    
       // 减法    
       result = a - b;    
       printf("%i\n", result); // 5
       // 乘法    
       result = a * b;    
       printf("%i\n", result); // 50    
       // 除法    
       result = a / b;    
       printf("%i\n", result); // 2        
       // 算术运算符的结合性和优先级    
       // 结合性: 左结合性, 从左至右    
       int c = 50;    
       result = a + b + c; // 15 + c;  65;    
       printf("%i\n", result);
       // 优先级: * / % 大于 + -    
       result = a + b * c; // a + 250; 260;    
       printf("%i\n", result);
   
       return 0;
   }
   ```
   
   ```c
   #include <stdio.h>
   
   int main()
   {    
       // 整数除以整数, 结果还是整数    
       printf("%i\n", 10 / 3); // 3    
       // 参与运算的任何一个数是小数, 结果就是小数    
       printf("%f\n", 10 / 3.0); // 3.333333
   
       return 0;
   }
   ```
   
   ```c
   #include <stdio.h>
   
   int main()
   {    
       // 10 / 3 商等于3, 余1    
       int result = 10 % 3;    
       printf("%i\n", result); // 1    
       // 左边小于右边, 那么结果就是左边    
       result = 2 % 10;    
       printf("%i\n", result); // 2    
       // 被除数是正数结果就是正数,被除数是负数结果就是负数    
       result = 10 % 3;    
       printf("%i\n", result); // 1    
       result = -10 % 3;    
       printf("%i\n", result); // -1    
       result = 10 % -3;
       printf("%i\n", result); // 1
   
       return 0;
   }
   ```

## 赋值运算符

![](D:\Programmering%20Learning\Markdown文档\C语言教程\图片\赋值运算符.png)

1. 简单赋值运算符
   
   ```c
   #include <stdio.h>
   
   int main()
   {    
       // 简单的赋值运算符 =    
       // 会将=右边的值赋值给左边    
       int a = 10;    
       printf("a = %i\n", a); // 10
   
       return 0;
   }
   ```

2. 复合赋值运算符
   
   ```c
   #include <stdio.h>
   
   int main()
   {     
       // 复合赋值运算符 += -= *= /= %=     
       // 将变量中的值取出之后进行对应的操作, 操作完毕之后再重新赋值给变量     
       int num1 = 10;     
       // num1 = num1 + 1; num1 = 10 + 1; num1 = 11;     
       num1 += 1;     
       printf("num1 = %i\n", num1); // 11     
       int num2 = 10;     
       // num2 = num2 - 1; num2 = 10 - 1; num2 = 9;     
       num2 -= 1;     
       printf("num2 = %i\n", num2); // 9     
       int num3 = 10;     
       // num3 = num3 * 2; num3 = 10 * 2; num3 = 20;     
       num3 *= 2;     
       printf("num3 = %i\n", num3); // 20     
       int num4 = 10;     
       // num4 = num4 / 2; num4 = 10 / 2; num4 = 5;     
       num4 /= 2;     
       printf("num4 = %i\n", num4); // 5     
       int num5 = 10;     
       // num5 = num5 % 3; num5 = 10 % 3; num5 = 1;     
       num5 %= 3;     
       printf("num5 = %i\n", num5); // 1
   
       return 0;
   }
   ```

3. 结合性和优先级
   
   ```c
   #include <stdio.h>
   
   int main()
   {    
       int number = 10;    
       // 赋值运算符优先级是14, 普通运算符优先级是3和4, 所以先计算普通运算符    
       // 普通运算符中乘法优先级是3, 加法是4, 所以先计算乘法    
       // number += 1 + 25; number += 26; number = number + 26; number = 36;    number += 1 + 5 * 5;    
       printf("number = %i\n", number); // 36
   
       return 0;
   }
   ```

## 自增自减运算符

![](D:\Programmering%20Learning\Markdown文档\C语言教程\图片\自增自减运算符.png)

1. 自增
   
   1. 如果只有单个变量，无论++写在前面还是后面都会对变量做+1操作。
   
      ```C
      #include <stdio.h>
      
      int main()
      {    
          int number = 10;    
          number++;    
          printf("number = %i\n", number); // 11    
          ++number;    
          printf("number = %i\n", number); // 12
      
          return 0;
      }
      ```
   
   2. 如果出现在一个表达式中, 那么++写在前面和后面就会有所区别
   
      1. 前缀表达式:++x, --x;其中x表示变量名,先完成变量的自增自减1运算,再用x的值作为表达式的值;即“先变后用”,也就是变量的值先变,再用变量的值参与运算。
   
      2. 后缀表达式:x++, x--;先用x的当前值作为表达式的值,再进行自增自减1运算。即“先用后变”,也就是先用变量的值参与运算,变量的值再进行自增自减变化。
   
         ```C
         #include <stdio.h>
         
         int main()
         {    
             int number = 10;    
             // ++在后, 先参与表达式运算, 再自增    
             // 表达式运算时为: 3 + 10;    
             int result = 3 + number++;    
             printf("result = %i\n", result); // 13    
             printf("number = %i\n", number); // 11
         
             return 0;
         }
         ```
   
         ```C
         #include <stdio.h>
         
         int main()
         {    
             int number = 10;    
             // ++在前, 先自增, 再参与表达式运算    
             // 表达式运算时为: 3 + 11;    
             int result = 3 + ++number;    
             printf("result = %i\n", result); // 14    
             printf("number = %i\n", number); // 11
         
             return 0;
         }
         ```

2. 自减
   
   ```c
   #include <stdio.h>
   
   int main()
   {    
       int number = 10;    
       // --在后, 先参与表达式运算, 再自减    
       // 表达式运算时为: 10 + 3;    
       int result = number-- + 3;    
       printf("result = %i\n", result); // 13    
       printf("number = %i\n", number); // 9
   
       return 0;
   }
   ```
   
   ```c
   #include <stdio.h>
   
   int main()
   {    
       int number = 10;    
       // --在前, 先自减, 再参与表达式运算    
       // 表达式运算时为: 9 + 3;    
       int result = --number + 3;    
       printf("result = %i\n", result); // 12    
       printf("number = %i\n", number); // 9
   
       return 0;
   }
   ```

3. 注意
   
   1. 自增、自减运算只能用于单个变量,只要是标准类型的变量,不管是整型、实型,还是字符型变量等,但不能用于表达式或常量。
   
   2. 企业开发中尽量让++ -- 单独出现, 尽量不要和其它运算符混合在一起
      
      ```c
      int i = 10;
      int b = i++; // 不推荐
      或者
      int b = ++i; // 不推荐
      或者
      int a = 10;
      int b = ++a + a++;  // 不推荐
      ```
      
      ```c
      int i = 10;
      int b = i; // 推荐
      i++;
      或者;
      i++;
      int b = i; // 推荐
      或者
      int a = 10;
      ++a;
      int b = a + a; // 推荐
      a++;
      ```
   
   3. C语言标准没有明确的规定，同一个表达式中同一个变量自增或自减后如何运算, 不同编译器得到结果也不同, 在企业开发中千万不要这样写
      
      ```c
      #include <stdio.h>
      
      int main()
      {
          int a = 1;    
          // 下列代码利用Qt运行时6, 利用Xcode运行是5    
          // 但是无论如何, 最终a的值都是3   
          //  在C语言中这种代码没有意义, 不用深究也不要这样写   
          // 特点: 参与运算的是同一个变量, 参与运算时都做了自增自减操作, 并且在同一个表达式中    
          int b = ++a + ++a;    
          printf("b = %i\n", b);
      
          return 0;
      }
      ```

## sizeof运算符

sizeof可以用来**计算一个变量或常量、数据类型所占的内存字节数**。

1. 标准格式：` sizeof(常量 or 变量);`

2. 几种形式
   
   1. `sizeof( 变量\常量 );`
      
      例：`sizeof(10);`     `char c = 'a'; sizeof(c);`
   
   2. `sizeof 变量\常量;`
      
      例：`sizeof 10;`  `char c = 'a'; sizeof c;`
   
   3. `sizeof( 数据类型);`
      
      例：`sizeof(float);`  `如果是数据类型不能省略括号`

3. sizeof面试题：sizeof()和+=、*=一样是一个复合运算符, 由sizeof和()两个部分组成, 但是代表的是一个整体。所以sizeof不是一个函数, 是一个运算符, 该运算符的优先级是2。

4. 示例
   
   ```c
   #include <stdio.h>
   
   int main()
   {
       int a = 10;
       double b = 3.14;
       // 由于sizeof的优先级比+号高, 所以会先计算sizeof(a);
       // a是int类型, 所以占4个字节得到结果4
       // 然后再利用计算结果和b相加, 4 + 3.14 = 7.14
       double res = sizeof a+b;
       printf("res = %lf\n", res); // 7.14
   
       return 0;
   }
   ```

## strlen函数

strlen函数是string.h库文件里面包含的一个函数，其功能是**计算字符串中字符的个数**。

注：strlen函数计算出来的字符的个数不包括字符串结束处的结束标志'\0'。

格式：`strlen(字符串)`

示例：

```c
#include <stdio.h>
#include <string.h>

int main()
{
    char fuc[]="Hello";

    int len=strlen(fuc);

    printf("%d\n",len);//5

    return 0;
}
```

```c
#include <stdio.h>
#include <string.h>

int main()
{
    char fuc1[]={'H','e','l','l','o'};
    char fuc2[]={'H','e','l','l','o','\0'};

    int len1=strlen(fuc1);
    int len2=strlen(fuc2);

    printf("%d\n",len1);//随机值，因为没有结束标志‘\0’
    printf("%d\n",len2);//5

    return 0;
}
```

## 逗号运算符

1. 在C语言中逗号“,”也是一种运算符,称为**逗号运算符**。 其功能是把多个表达式连接起来组成一个表达式,称为**逗号表达式**。

2. 逗号运算符会从左至右依次取出每个表达式的值, 最后整个逗号表达式的值等于最后一个表达式的值。

3. 格式：`表达式1，表达式2，表达式3，......  ，表达式n`
   
   例如：`int result =a+1,b=3*4;`    `"1+2,6+8"//14`

4. 特点：优先级别最低; ；自左往右执行表达式；返回值为表达式最后一个。

5. 示例
   
   ```c
   #include <stdio.h>
   
   int main()
   {
       int a=10,b=15,c=20;
   
       //(a,b,c)是逗号表达式，而后面的逗号只是参数之间的分隔符
       printf("%d %d %d",(a,b,c),b,c);//20 15 20
   
       return 0;
   }
   ```
   
   ```c
   #include <stdio.h>
   
   int main()
   {    
       int a = 10, b = 20, c;    
       // ()优先级高于逗号运算符和赋值运算符, 所以先计算()中的内容    
       // c = (11, 21);    
       // ()中是一个逗号表达式, 结果是最后一个表达式的值, 所以计算结果为21    
       // 将逗号表达式的结果赋值给c, 所以c的结果是21    
       c = (a + 1, b + 1);    
       printf("c = %i\n", c); // 21
   
       return 0;
   }
   ```

## 关系运算符

1. C语言的真假性
   
   C语言规定，任何数值都有真假性，非“0”值为真，“0”为假。

2. 关系运算符的运算结果只有2种：如果条件成立，结果就为1，也就是“真”；如果条件不成立，结果就为0，也就是“假”。![](D:\Programmering%20Learning\Markdown文档\C语言教程\图片\关系运算符.png)
   
   ```c
   #include <stdio.h>int result2 = (3>4) + 7
   
   int main()
   {
       int result = 10 > 5;
       printf("result = %i\n", result); // 1
       result = 5 < 10;
       printf("result = %i\n", result); // 1
       result = 5 > 10;
       printf("result = %i\n", result); // 0
       result = 10 >= 10;
       printf("result = %i\n", result); // 1
       result = 10 <= 10;
       printf("result = %i\n", result); // 1
       result = 10 == 10;
       printf("result = %i\n", result); // 1
       result = 10 != 9;
       printf("result = %i\n", result); // 1
   
       return 0;
   }
   ```

3. 优先级和结合性
   
   ```c
   #include <stdio.h>
   
   int main()
   {
       // == 和 != 优先级一样, 所以按照结合性
       // 关系运算符是左结合性, 所以从左至右计算
       // result = 0 != 3; result = 1;
       int result = 10 == 5 != 3;
       printf("result = %i\n", result); // 1
   
       return 0;
   }
   ```
   
   ```c
   #include <stdio.h>
   
   int main()
   {
       // == 优先级 小于 >, 所以先计算>
       // result = 10 == 1; result = 0;
       int result = 10 == 5 > 3;
       printf("result = %i\n", result); // 0
   
       return 0;
   }
   ```

4. 注意
   
   无论是float还是double都有精度问题, 所以一定要避免利用==判断浮点数是否相等。
   
   ```c
   #include <stdio.h>
   
   int main()
   {        
       float a = 0.1;
       float b = a * 10 + 0.00000000001;
       double c = 1.0 + + 0.00000000001;
       printf("b = %f\n", b);
       printf("c = %f\n", c);
       int result = b == c;
       printf("result = %i\n", result); // 0
   
       return 0;
   }
   ```

5. 练习
   
   ```c
   int result1 = 3 > 4 + 7//0
   int result2 = (3>4) + 7//7
   int result3 = 5 != 4 + 2 * 7 > 3 == 10//0
   //运算符优先级：*大于+大于>大于（!=等于==）
   //（4+14=18>3）=1
   //（5！=1）=1,5不等于1，真
   //（1==10）=0,1不等于10.
   ```

## 逻辑运算符

![](D:\Programmering%20Learning\Markdown文档\C语言教程\图片\逻辑运算符.png)

1. 逻辑非
   
   1. 格式：`! 条件A;`
   
   2. 运算结果：真变假，假变真
   
   3. 运算过程：先判断条件A是否成立，如果添加A成立, 那么结果就为0，即“假”；
      如果条件A不成立，结果就为1，即“真”。
   
   4. 注意：可以多次连续使用逻辑非运算符。例如：`!!!0;`相当于`(!(!(!0)));`最终结果为1。
      
      ```c
      #include <stdio.h>
      
      int main()
      {                                    
          // ()优先级高, 先计算()里面的内容
          // 10==10为真, 所以result = !(1);
          // !代表真变假, 假变真,所以结果是假0
          int result = !(10 == 10);
          printf("result = %i\n", result); // 0
      
          return 0;
      }
      ```

2. 逻辑与
   
   1. 格式：`条件A&&条件B`
   
   2. 运算结果：一假则假，全真为真
   
   3. 运算过程：总是先判断"条件A"是否成立，如果"条件A"成立，接着再判断"条件B"是否成立，如果"条件B"也成立，结果就为1，即“真”；如果"条件A"成立，"条件B"不成立，结果就为0，即“假”；如果"条件A"不成立，不会再去判断"条件B"是否成立, 因为逻辑与只要一个不为真结果都不为真。
   
   4. 注意："条件A"为假, "条件B"不会被执行。
      
      ```c
      #include <stdio.h>
      
      int main()
      {
          int a = 10;
          int b = 20;
          // 逻辑与, 前面为假, 不会继续执行后面    
          int result = (a == 9) && (++b);
          printf("result = %i\n", result); // 1    
          printf("b = %i\n", b); // 20
      
          return 0;
      }
      ```
      
      ```c
      #include <stdio.h>
      
      int main()
      {    
          //               真     &&    真    
          int result = (10 == 10) && (5 != 1);    
          printf("result = %i\n", result); // 1    
          //          假     &&    真    
          result = (10 == 9) && (5 != 1);    
          printf("result = %i\n", result); // 0    
          //          真     &&    假    
          result = (10 == 10) && (5 != 5);    
          printf("result = %i\n", result); // 0    
          //          假     &&    假    
          result = (10 == 9) && (5 != 5);    
          printf("result = %i\n", result); // 0
      
          return 0;
      }
      ```

3. 逻辑或
   
   1. 格式：`条件A || 条件B;`
   
   2. 运算结果：一真则真，全假为假
   
   3. 运算过程：总是先判断"条件A"是否成立；如果"条件A"不成立，接着再判断"条件B"是否成立, 如果"条件B"成立，结果就为1，即“真”；如果"条件A"不成立，"条件B"也不成立成立, 结果就为0，即“假”；如果"条件A"成立, 不会再去判断"条件B"是否成立, 因为逻辑或只要一个为真结果都为真。
   
   4. 注意："条件A"为真, "条件B"不会被执行。
      
      ```c
      #include <stdio.h>
      
      int main()
      {
          int a = 10;
          int b = 20;
          // 逻辑或, 前面为真, 不会继续执行后面    
          int result = (a == 10) || (++b);
          printf("result = %i\n", result); // 1    
          printf("b = %i\n", b); // 20
      
          return 0;    
      }
      ```
      
      ```c
      #include <stdio.h>
      
      int main()
      {
          //               真     ||    真    
          int result = (10 == 10) || (5 != 1);
          printf("result = %i\n", result); // 1    
          //          假     ||    真    
          result = (10 == 9) || (5 != 1);
          printf("result = %i\n", result); // 1    
          //          真     ||    假    
          result = (10 == 10) || (5 != 5);
          printf("result = %i\n", result); // 1    
          //          假     ||    假    
          result = (10 == 9) || (5 != 5);
          printf("result = %i\n", result); // 0
      
          return 0;
      }
      ```
   
   5. 练习
      
      ```c
      int result = 3>5 || 2<4 && 6<1;//0
      //优先级：（>等于<）大于&&大于||大于=
      //（3>5）=0
      //（2<4）=1
      //（6<1）=0
      //(1&&0)=0
      //(0||0)=0
      //result=0
      ```

## 三目运算符

1. 格式：`表达式1？表达式2(结果A)：表达式3(结果B)`

2. 求职规则：如果"表达式1"为真，三目运算符的运算结果为"表达式2"的值(结果A)，否则为"表达式3"的值(结果B)。

3. 示例
   
   ```c
   示例：
       int a = 10;
       int b = 20;
       int max = (a > b) ? a : b;
       printf("max = %d", max);
       输出结果: 20
   等价于:
       int a = 10;
       int b = 20;
       int max = 0;
       if(a>b)
       {
           max=a;
       }
       else
       { 
           max=b;
       }
       printf("max = %d", max);
   ```
   
   ```c
   #include <stdio.h>
   
   int main()
   {
       int a = 10;
       int b = 5;
       // 先计算 a > b    
       // 然后再根据计算结果判定返回a还是b    
       // 相当于int max= (a>b) ? a : b;    
       int max= a>b ? a : b;
       printf("max = %i\n", max); // 10
   
       return 0;    
   }
   ```
   
   ```c
   #include <stdio.h>
   
   int main()
   {
       int a = 10;
       int b = 5;
       int c = 20;
       int d = 10;
       // 结合性是从右至左, 所以会先计算:后面的内容    
       // int res = a>b?a:(c>d?c:d);    
       // int res = a>b?a:(20>10?20:10);    
       // int res = a>b?a:(20);    
       // 然后再计算最终的结果    
       // int res = 10>5?10:(20);    
       // int res = 10;    
       int res = a>b?a:c>d?c:d;
       printf("res = %i\n", res);
   
       return 0;
   }
   ```

4. 注意：条件运算符的运算优先级低于关系运算符和算术运算符，但高于赋值符；条件运算符?和:是一个整体,不能分开使用。

# 数据类型转换

数据类型转换就是将数据（变量、数值、表达式的结果等）从一种类型转换为另一种类型。

1. 自动类型转换（隐式转换）
   
   1. 赋值转换
      
      在赋值运算中，赋值号两边的数据类型不同时，需要先将右边的类型转换为左边的类型，然后才能进行赋值运算。但是，这样的转换会导致数据失真，或者精度降低。所以自动类型转换不一定安全，对于不安全的类型转换，编译器一般会发出警告。
      
      ```c
      float f=100;
      //100是int类型，需要先将100转换成float类型，才能赋值给f。
      int n=f;
      //f为float类型，需要先将f转换成int类型，才能赋值给n。
      ```
   
   2. 算术转换
      
         在不同类型的混合运算中，编译器也会自动地转换数据类型，将参与运算的所有数据先转换为同一种类型，然后再进行计算。
      
      转换规则：
      
      1. 转换按数据长度增加的方向进行，以保证数值不失真，或者精度不降低。例如，int 和 long 参与运算时，先把 int 类型的数据转成 long 类型后再进行运算。
      
      2. 所有的浮点运算都是以双精度进行的，即使运算中只有 float 类型，也要先转换为 double 类型，才能进行运算。
      
      3. char 和 short 参与运算时，必须先转换成 int 类型。
         
         ![](D:\Programmering%20Learning\Markdown文档\C语言教程\图片\数据类型转换.png)
         
         注：unsigned 也即 unsigned int，此时可以省略 int，只写 unsigned。
   
   3. 示例
      
      ```c
      #include<stdio.h>
      
      int main()
      {
          float PI = 3.14159;
          int s1, r = 5;
          double s2;
          s1 = r * r * PI;
          s2 = r * r * PI;
          printf("s1=%d, s2=%f\n", s1, s2);//s1=78, s2=78.539749
          /*在计算表达式r*r*PI时，r 和 PI 都被转换成 double 类型，表达式的结果
      也是 double 类型。但由于 s1 为整型，所以赋值运算的结果仍为整型，舍去了小数
      部分，导致数据失真。*/
      
          return 0;
      }
      ```

2. 强制类型转换
   
   1. 格式：（目标类型）（表达式）
      
      ```c
      (float) a;  //将变量 a 转换为 float 类型
      (int)(x+y);  //把表达式 x+y 的结果转换为 int 整型
      (float) 100;  //将数值 100（默认为int类型）转换为 float 类型
      ```
   
   2. 示例
      
      ```c
      #include <stdio.h>
      
      int main()
      {
          int sum = 103;  //总数
          int count = 7;  //数目
          double average;  //平均数
          average = (double) sum / count;
          printf("Average is %lf!\n", average);//Average is 14.714286!
      
          return 0;
      }
      ```
      
      ``sum 和 count 都是 int 类型，如果不进行干预，那么sum / count的运算结果也是 int 类型，小数部分将被丢弃；虽然是 average 是 double 类型，可以接收小数部分，小数部分提前就被舍弃了，它只能接收到整数部分，这就导致除法运算的结果严重失真。``
      
      ``为了提高运算精度，我们需将 sum 或者 count 其中之一转换为 double 类型即可。上面的代码中，我们将 sum 强制转换为 double 类型，这样sum / count的结果也将变成 double 类型，就可以保留小数部分了，average 接收到的值也会更加精确。``
      
      ``( )的优先级高于/，对于表达式(double) sum / count，会先执行(double) sum，将 sum 转换为 double 类型，然后再进行除法运算，这样运算结果也是 double 类型，能够保留小数分。注意不要写作(double) (sum / count)，这样写运算结果将是 3.000000，仍然不能保留小数部分。``
   
3. 无论是自动类型转换还是强制类型转换，都只是为了本次运算而进行的临时性转换，转换的结果也会保存到临时的内存空间，不会改变数据本来的类型或者值。
   
   ```c
   #include <stdio.h>
   
   int main()
   {
       double total = 400.8;  //总价
       int count = 5;  //数目
       double unit;  //单价
       int total_int = (int)total;
       unit = total / count;
       printf("total=%lf, total_int=%d, unit=%lf\n", total, total_int, unit);
       //total=400.800000, total_int=400, unit=80.160000
   
       return 0;
   }
   ```

# 选择结构

1. 选择结构if（如果）
   
   1. 格式：
   
      ```c
      //满足表达式1，执行语句块1，否则执行语句块2
      if(表达式1)
      {
          语句块1
      }
      else
      {
          语句块2
      }
      ```
   
      ```c
      //满足表达式1，执行语句块1；若不满足表达式1，判断表达式2，若符合，执行语句块2，否则，执行语句块3
      if(表达式1)
      {
          语句块1
      }
      else if(表达式2)
      {
          语句块2
      }
      else
      {
          语句块3
      }
      ```
   
   2. if嵌套
   
      ```c
      if(表达式1)
      {
          语句块1;
          if(表达式2)
          {
              语句块2;  
          }
      }
      else
      {
          if(表达式3)
          {
              语句块3;  
          }else
          { 
              语句块4;  
          }
      }
      ```
   
   3. if注意点
   
      1. 任何数值都有真假性
         
         ```c
         #include <stdio.h>
         
         //if(0)，0为假，即如果为假，执行“执行了if“的打印，但是程序运行不为假，则执行”执行了else“打印
         int main(){
             if(0)
             { 
                 printf("执行了if");
             }
             else
             {
                 printf("执行了else"); // 被执行了else  
             }
         
             return 0;
         }
         ```
   
      2. 当if else后面只有一条语句时, if else后面的大括号可以省略
         
         ```c
         //不推荐
         #include <stdio.h>
         
         int main()
         {
             int age = 17;
             if (age >= 18)
                 printf("开网卡\n");
             else 
                 printf("喊家长来开\n");
         
             return 0;
         }
         ```
   
      3. 当if else后面的大括号被省略时, else会自动和距离最近的一个if匹配
         
         ```c
         #include <stdio.h>
         
         int main()
         {
             if(0)
             if(1)
             printf("A\n");
             else // 和if(1)匹配    
             printf("B\n");
             else // 和if(0)匹配, 因为if(1)已经被匹配过了    
             if (1)
             printf("C\n"); // 输出C    
             else // 和if(1)匹配    
             printf("D\n");
         
             return 0;
         }
         ```
   
      4. 如果if else省略了大括号, 那么后面不能定义变量
         
         ```c
         #include <stdio.h>
         
         int main()
         {
             if(1)
             int number = 10; // 系统会报错    
             printf("number = %i\n", number);
         
             return 0;
         }
         ```
         
         ```c
         #include <stdio.h>
         
         int main()
         {
             if(0)
             {
                 int number = 10;
             }
             else
                 int value = 20; // 系统会报错    
             printf("value = %i\n", value);
         
             return 0;
         }
         ```
   
      5. C语言中分号(;)也是一条语句, 称之为空语句
         
         ```c
         // 因为if(10 > 2)后面有一个分号, 所以系统会认为if省略了大括号
         // if省略大括号时只能管控紧随其后的那条语句, 所以只能管控分号
         if(10 > 2);
         {
             printf("10 > 2");
         }
         // 输出结果: 10 > 2
         ```
   
      6. 但凡遇到比较一个变量等于或者不等于某一个常量的时候，把常量写在前面
         
         ```c
         #include <stdio.h>
         
         int main()
         {
             int a = 8;
             //    if(a = 10){// 错误写法, 但不会报错    
             if (10 == a)
             { 
                 printf("a的值是10\n");
             }
             else
             {
                 printf("a的值不是10\n");
             }
         
             return 0;
         }
         ```
   
   4. 实现石头剪刀布
   
      ```c
      剪刀石头布游戏:
      1)定义游戏规则
      剪刀 干掉 布
      石头 干掉 剪刀
      布 干掉石头
      2)显示玩家开始猜拳
      3)接收玩家输入的内容
      4)让电脑随机产生一种拳
      5)判断比较
      (1)玩家赢的情况(显示玩家赢了)
      (2)电脑赢的情况(显示电脑赢了)
      (3)平局(显示平局)
      ```
   
      ```c
      #include <stdio.h>
      #include <time.h>
      
      int main()
      {
          // 用户出拳
          int a;
          printf("请出拳:");
          scanf("%d", &a);
          // 判断用户出拳
          if (a < 0 || a > 2)
          {
              printf("请重新输入：");
              scanf("%d",&a);
          }
          // 电脑出拳（获取随机数）
          srand(time(NULL));
          int cm = rand() % 3;
          //  判断双方出拳
          if ((cm == 0 && a == 2) ||
              (cm == 1 && a == 0) ||
              (cm == 2 && a == 1))
          {
              printf("电脑出的是%i,玩家出的是%i,玩家赢了\n", cm, a);
          }
          else if ((cm == 0 && a == 1) ||
                   (cm == 1 && a == 2) ||
                   (cm == 2 && a == 0))
          {
              printf("电脑出的是%i,玩家出的是%i,玩家输了\n", cm, a);
          }
          else
          {
              printf("电脑出的是%i,玩家出的是%i,平手\n", cm, a);
          }
      
          return 0;
      ```
   
      ```c
      //优化循环出拳
      #include <stdio.h>
      #include <time.h>
      
      int main()
      {
          // 用户出拳
          int a;
      code:
          printf("请出拳:");
          scanf("%d", &a);
          // 判断用户出拳
          if (a < 0 || a > 2)
          {
              printf("滚\n");
              goto code;
          }
          // 电脑出拳（获取随机数）
          srand(time(NULL));
          int cm = rand() % 3;
          //  判断双方出拳
          if ((cm == 0 && a == 2) ||
              (cm == 1 && a == 0) ||
              (cm == 2 && a == 1))
          {
              printf("电脑出的是%i,玩家出的是%i,玩家赢了\n", cm, a);
          }
          else if ((cm == 0 && a == 1) ||
                   (cm == 1 && a == 2) ||
                   (cm == 2 && a == 0))
          {
              printf("电脑出的是%i,玩家出的是%i,玩家输了\n", cm, a);
          }
          else
          {
              printf("电脑出的是%i,玩家出的是%i,平手\n", cm, a);
          }
          //实现循环出
          while (1)
          {
              goto code;
          }
      
          return 0;
      }
      ```

   5. 随机数
   
      1. `rand()`函数
   
         1. 作用：生成随机数
   
         2. 用法：`int rand(void);` 
   
            `void`表示不需要传递参数。
   
         3. 所在头文件：`#include <stdlib.h>`
   
         4. C语言中还有一个`random()`函数可以获取随机数，但是 random() 不是标准函数，不能在 VC/VS 等编译器通过，所以比较少用。
   
         5. `rand()`会随机生成一个位于 `0` ~ `RAND_MAX`之间的整数。
   
            `RAND_MAX`是`<stdlib.h>`头文件中的一个宏，它用来指明`rand()`所能返回的随机数的最大值。C语言标准并没有规定 `RAND_MAX`的具体数值，只是规定它的值至少为 32767。在实际编程中，我们也不需要知道`RAND_MAX`的具体值，把它当做一个很大的数来对待即可。
   
         6. 示例
   
            ```c
            #include <stdio.h>
            #include <stdlib.h>
            
            int main()
            {
                int a = rand();
                printf("%d\n",a);
                
                return 0;
            }
            ```
   
            ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\rand().png)
   
      2. 随机数的本质
   
         多次运行上面的代码，你会发现每次产生的随机数都一样，这是怎么回事呢？为什么随机数并不随机呢？
   
         实际上，`rand()`函数产生的随机数是伪随机数，是根据一个数值按照某个公式推算出来的，这个数值我们称之为“种子”。种子和随机数之间的关系是一种正态分布，如下图所示：
   
         ![](D:\Programmering Learning\Markdown文档\C语言教程\动画\随机数的本质.gif)
   
         种子在每次启动计算机时是随机的，但是一旦计算机启动以后它就不再变化了；也就是说，每次启动计算机以后，种子就是定值了，所以根据公式推算出来的结果（也就是生成的随机数）就是固定的。
   
      3. 重新播种—`srand()`
   
         我们可以通过`srand()`函数来重新“播种”，这样种子就会发生改变。`srand()`的用法为：
   
         ```c
         void srand (unsigned int seed);
         ```
   
         它需要一个`unsigned int`类型的参数。在实际开发中，我们可以用时间作为参数，只要每次播种的时间不同，那么生成的种子就不同，最终的随机数也就不同。
   
         使用`<time.h>`头文件中的`time()`函数即可得到当前的时间（精确到秒），就像下面这样：
   
         ```c
         srand((unsigned)time(NULL));
         ```
   
         对上面的代码进行修改，生成随机数之前先进行播种：
   
         ```c
         #include <stdio.h>
         #include <stdlib.h>
         #include <time.h>
         
         int main()
         {
             int a;
             srand((unsigned)time(NULL));
             a = rand();
             printf("%d\n", a);
             
             return 0;
         }
         ```
   
         多次运行程序，会发现每次生成的随机数都不一样了。但是，这些随机数会有逐渐增大或者逐渐减小的趋势，这是因为我们以时间为种子，时间是逐渐增大的，结合上面的正态分布图，很容易推断出随机数也会逐渐增大或者减小。
   
      4. 生成一定范围内的随机数
   
         在实际开发中，我们往往需要一定范围内的随机数，过大或者过小都不符合要求，那么，如何产生一定范围的随机数呢？我们可以利用取模的方法：
   
         ```c
         int a = rand() % 10;    //产生0~9的随机数，注意10会被整除
         ```
   
         如果要规定上下限：
   
         ```c
         int a = rand() % 51 + 13;    //产生13~63的随机数
         ```
   
         分析：取模即取余，`rand()%51+13`我们可以看成两部分：`rand()%51`是产生 0~50 的随机数，后面 `+13` 保证 a 最小只能是 13，最大就是`50+13=63`。
   
         最后给出产生 13~63 范围内随机数的完整代码：
   
         ```c
         #include <stdio.h>
         #include <stdlib.h>
         #include <time.h>
         
         int main()
         {
             int a;
             srand((unsigned)time(NULL));
             a = rand() % 51 + 13;
             printf("%d\n",a);
             
             return 0;
         }
         ```
   
      5. 连续生成随机数
   
         有时候我们需要一组随机数（多个随机数），该怎么生成呢？很容易想到的一种解决方案是使用循环，每次循环都重新播种，请看下面的代码：
   
         ```c
         #include <stdio.h>
         #include <stdlib.h>
         #include <time.h>
         
         int main()
         {
             int a, i;
             //使用for循环生成10个随机数
             for (i = 0; i < 10; i++)
             {
                 srand((unsigned)time(NULL));
                 a = rand();
                 printf("%d ", a);
             }
         
             return 0;
         }
         ```
   
         ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\连续生成随机数01.png)
   
         ​	运行结果非常奇怪，每次循环我们都重新播种了呀，为什么生成的随机数都一样呢？
   
         ​	这是因为，for 循环运行速度非常快，在一秒之内就运行完成了，而`time()`函数得到的时间只能精确到秒，所以每次循环得到的时间都是一样的，这样一来，种子也就是一样的，随机数也就一样了。
   
         ​	下面提供两种解决方案：
   
         ```c
         //将srand()放在for循环外面
         #include <stdio.h>
         #include <stdlib.h>
         #include <time.h>
         
         int main()
         {
             int a, i;
             //使用for循环生成10个随机数
             srand((unsigned)time(NULL));
             for (i = 0; i < 10; i++)
             {
                 a = rand();
                 printf("%d ", a);
             }
         
             return 0;
         }
         ```
   
         ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\连续生成随机数02.png)
         
         ```c
         #include <stdio.h>
         #include <stdlib.h>
         #include <time.h>
         
         int main()
         {
             int a, i;
             //使用for循环生成10个随机数
             for (i = 0; i < 10; i++)
             {
                 srand((unsigned)time(NULL) + (unsigned)rand());
                 a = rand();
                 printf("%d ", a);
             }
         
             return 0;
         }
         ```
         
         ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\连续生成随机数03.png)
   
2. 选择结构switch
   
   1. 格式：
      
      ```c
      switch(表达式)
      {
          case 常量表达式1:
              语句1;
              break;
          case 常量表达式2:
              语句2;
              break;
          case 常量表达式n:
              语句n;
              break;
          default:
              语句n+1;
              break;
      }
      ```
   
   2. 语义
      
         计算"表达式"的值, 逐个与其后的"常量表达式"值相比较,当"表达式"的值与某个"常量表达式"的值相等时, 即执行其后的语句, 然后跳出switch语句。
   
   3. 示例
      
      ```c
      #include <stdio.h>
      
      int main()
      {
          int num = 3;
          switch(num)
          {
          case 1:
              printf("星期一\n");
              break;
          case 2:
              printf("星期二\n");
              break;
          case 3:
              printf("星期三\n");//输出星期三
              break;
          case 4:
              printf("星期四\n");
              break;
          case 5:
              printf("星期五\n");
              break;
          case 6:
              printf("星期六\n");
              break;
          case 7:
              printf("星期日\n");
              break;
          default:
              printf("回火星去\n");
              break;
          }
      
          return 0;
      }
      ```
   
   4. 注意点
      
      1. switch条件表达式的类型必须是整型, 或者可以被提升为整型的值(char、short)
         
         ```c
         #include <stdio.h>
         
         int main()
         {
             switch(1.1) // 报错 
             {
             case 1:
                 printf("星期一\n"); 
                 break; 
             case 2:
                 printf("星期二\n");
                 break;
             default:
                 printf("回火星去\n");
                 break;
             }
         
             return 0;
         }
         ```
      
      2. case的值只能是常量, 并且还必须是整型, 或者可以被提升为整型的值(char、short)
         
         ```c
         #include <stdio.h>
         
         int main() {
             int num = 3;
             switch(1)
             {
             case 1:
                 printf("星期一\n");
                 break;
             case 'a':
                 printf("星期二\n");
                 break;
             case num: // 报错        
                 printf("星期三\n");
                 break;
             case 4.0: // 报错        
                 printf("星期四\n");
                 break;
             default:
                 printf("回火星去\n");
                 break;
             }
         
             return 0;
         }
         ```
      
      3. case后面常量表达式的值不能相同
         
         ```c
         #include <stdio.h>
         
         int main()
         {
             switch(1)
             {
             case 1: // 报错        
                 printf("星期一\n");
                 break;
             case 1: // 报错        
                 printf("星期一\n");
                 break;
             default:
                 printf("回火星去\n");
                 break;
             }
         
             return 0;
         }
         ```
      
      4. case后面要想定义变量,必须给case加上大括号
         
         ```c
         #include <stdio.h>
         
         int main()
         {    
             switch(1)
             {    
                 case 1:
                     {
                         int num = 10;        
                         printf("num = %i\n", num);        
                         printf("星期一\n");        
                         break;        
                     }    
                 case 2:
                     printf("星期一\n");        
                     break;    
                 default:
                     printf("回火星去\n");        
                     break;    
             }
         
             return 0;
         }
         ```
      
      5. switch中只要任意一个case匹配, 其它所有的case和default都会失效. 所以如果case和default后面没有break就会出现穿透问题
         
         ```c
         #include <stdio.h>
         
         int main()
         {    
             int num = 2;    
             switch(num)
             {    
                 case 1:
                     printf("星期一\n");        
                     break;    
                 case 2:
                     printf("星期二\n"); // 被输出    
                 case 3:
                     printf("星期三\n"); // 被输出    
                 default:
                     printf("回火星去\n"); // 被输出        
                     break;        
              }
         
             return 0;
         }
         ```
      
      6. switch中default可以省略
         
         ```c
         #include <stdio.h>
         
         int main()
         {    
             switch(1)
             {    
                 case 1:
                     printf("星期一\n");        
                     break;    
                 case 2:
                     printf("星期一\n");        
                     break;    
             }
         
             return 0;
         }
         ```
      
      7. switch中default的位置不一定要写到最后, 无论放到哪都会等到所有case都不匹配才会执行(穿透问题除外)
         
         ```c
         #include <stdio.h>
         
         int main()
         {    
             switch(3)
             {    
                 case 1:
                     printf("星期一\n");        
                     break;    
                 default:
                     printf("Other,,,\n");        
                     break;    
                 case 2:
                     printf("星期一\n");        
                     break;    
              }
         
             return 0;
         }
         ```

# 循环结构

1. 循环结构while（当）
   
   1. 格式
      
      ```c
      while(循环控制条件)
      {
          循环体语句；
          循环结束的语句；
      } 
      ```
   
   2. 构成循环结构的条件
      
      1. 循环控制条件
         
         循环退出的主要依据,来控制循环到底什么时候退出。
      
      2. 循环体
         
         循环的过程中重复执行的代码段。
      
      3. 使循环结束的语句
         
         能够让循环条件为假的依据,否则退出循环。一般为递增/减，真/假。
   
   3. 示例
      
      1. 首先会判定"循环控制条件"是否为真, 如果为假直接跳到循环语句后面
      
      2. 如果"循环控制条件"为真, 执行一次循环体, 然后再次判断"循环控制条件"是否为真, 为真继续执行循环体,为假跳出循环。
      
      3. 重复以上操作, 直到"循环控制条件"为假为止
      
      ```c
      #include <stdio.h>
      
      //运行结果：0 1 2 3 4 5 6 7 8 9
      int main()
      {
          int n=0;
          //n=0,满足n<10的条件，输出0，n+1=1
          //n=1,满足n<10的条件，输出1，n+1=2
          ......
          //直到n的值不满足n<10的时候循环结束
          while(n<10)//循环控制条件
          {
              printf("%d ",n);//循环体语句
              n++;//使循环结束的语句
          }
      
          return 0;
      }
      ```
   
   4. 注意点
      
      1. 任何数值都有真假性
         
         ```c
         #include <stdio.h>
         
         int main(){
             //程序运行
             while(1)//最简单的死循环
             {
                 printf("死循环");
             }
         
             return 0;
         }
         ```
      
      2. 当while后面只有一条语句时,while后面的大括号可以省略（无意义，别这样干）
         
         ```c
         //当大括号省略之后，循环直接变为死循环
         //大括号省略之后，循环体的第一行就充当了“循环体”，后面的结束语句也就失效了
         //下面代码的实际循环体就是“printf("发射子弹~哔哔哔哔\n");”
         #include <stdio.h>
         
         int main()
         {
             int n=0;
             while (n<10) // 死循环
             printf("发射子弹~哔哔哔哔\n");
             n++;
         
             return 0;
         }
         ```
      
      3. C语言中分号(;)也是一条语句, 称之为空语句
         
         ```c
         #include <stdio.h>
         
         int main()
         {
             int count = 0;
             while (count < 3);
             { 
                 // 无输出
                 printf("发射子弹~哔哔哔哔\n");
                 count++;
             }
         
             return 0;
         }
         ```

2. 循环结构do while
   
   1. 格式
      
      ```c
      do
      {
          循环体中的语句;
          能够让循环结束的语句;
      } while (循环控制条件 );
      ```
   
   2. 示例
      
      1. 首先不管while中的条件是否成立, 都会执行一次"循环体"
      
      2. 执行完一次循环体,接着再次判断while中的条件是否为真, 为真继续执行循环体,为假跳出循环
      
      3. 重复以上操作, 直到"循环控制条件"为假为止
      
      ```c
      #include <stdio.h>
      
      //输出结果为10行Hello
      int main()
      {
          int count = 0;
          do
          {
              printf("Hello\n");
              count++;
          }while(count < 10);
      
          return 0;
      }
      ```
   
   3. 应用场景——口令校验
      
      ```c
      #include<stdio.h>
      
      int main()
      {
          int num = -1;
          do
          {
              printf("请输入密码\n");
              scanf("%d", &num);
          }while(123456 != num);
          printf("密码正确\n");
      
          return 0;
      }
      ```
   
   4. 注意点
      
      1. 绝大多数情况下while和do while可以互换, 所以能用while就用while。
      
      2. 无论如何都需要先执行一次循环体的情况, 才使用do while。

3. 循环结构for
   
   1. 格式
      
      ```c
      for(初始化表达式；循环条件表达式；循环后的操作表达式)
      {
          循环体中的语句;
      }
      ```
   
   2. 示例
      
      1. 首先执行"初始化表达式"，而且在整个循环过程中,只会执行一次初始化表达式。
      
      2. 接着判断"循环条件表达式"是否为真，为真执行循环体中的语句。（循环条件表达式不一定是范围）
      
      3. 循环体执行完毕后，接下来会执行"循环后的操作表达式"，然后再次判断条件是否为真,为真继续执行循环体,为假跳出循环。
      
      4. 重复上述过程，直到条件不成立就结束for循环。
      
      ```c
      #include<stdio.h>
      
      //输出结果为：0 1 2 3 4 5 6 7 8 9
      int main()
      {
          for(int i=0;i<10;i++)
          {
              printf("%d ",i);
          }
      
          return 0;
      }
      ```
   
   3. 注意点
      
      最简单死循环——`for(;;)`
      
      ```c
      #include<stdio.h>
      
      int main()
      {
          for(;;)
          {
              printf("Hello\n");
          }
      
          return 0;
      }
      ```
   
   4. 应用场景
      
         while能做的for都能做, 所以企业开发中能用for就用for, 因为for更为灵活。而且对比while来说for更节约内存空间
      
      ```c
      #include <stdio.h>
      
      int main()
      {
          int count = 0; // 初始化表达式
          while (count < 10)//条件表达式
          {
              printf("第%i次\n", count+1);
              count++; // 循环后增量表达式
          }
          // 如果初始化表达式的值, 需要在循环之后使用, 那么就用while
          printf("count = %i\n", count);
      
          return 0;
      }
      ```
      
      ```c
      #include <stdio.h>
      
      int main()
      {
          // 注意: 在for循环初始化表达式中定义的变量, 只能在for循环后面的{}中访问
          // 所以: 如果初始化表达式的值, 不需要在循环之后使用, 那么就用for
          // 因为如果初始化表达式的值, 在循环之后就不需要使用了 , 那么用while会导致性能问题
          for (int count = 0; count < 10; count++)
          {
              printf("发射子弹~哔哔哔哔 %i\n", count);
          }
          printf("count = %i\n", count);//报错
      
          return 0;
      }
      ```
      
      ```c
      #include <stdio.h>
      
      int main()
      {
          // 如果需要使用初始化表达式的值, 也可以将初始化表达式写到外面    
          int count=0;
          for (; count < 10; count++)
          {
              printf("第%i次\n", count+1);
          }
          printf("count = %i\n", count);//count=10
      
          return 0;
      }
      ```

## 四大跳转

四大跳转分别是：return、break、continue、goto

1. break
   
   1. 应用场景：立即跳出switch语句或循环。
   
   2. 注意点
      
      1. break离开应用范围，存在是没有意义的
         
         ```c
         if(1)
         {
             break; // 会报错
         }
         ```
      
      2. 在多层循环中,一个break语句只向外跳一层
         
         ```c
         while(1)
         {
             while(2)
             {
                 break;// 只对while2有效, 不会影响while1
             }
             printf("while1循环体\n");
         }
         ```
      
      3. break下面不可以有语句，因为执行不到
         
         ```c
         while(2)
         {
             break;
             printf("你打我啊!唉，你打不到，就是这么气人！");// 执行不到
         }
         ```

2. continue
   
   结束本轮循环，进入下一轮循环
   
   1. 应用场景：循环结构
      
      ```c
      #include <stdio.h>
      
      int main()
      {
          int count=0;
      
          while(count<=10)
          {
              count++;
              if(count%2 !=0)
              {
                  continue;
              }
              printf("count=%i\n",count);
          }
      
          return 0;
      }
      ```
      
      ![](D:\Programmering%20Learning\Markdown文档\C语言教程\图片\continue跳转.png)
      
      ![](D:\Programmering%20Learning\Markdown文档\C语言教程\图片\continue跳转运行结果.png)
   
   2. 注意点
      
      1. continue离开应用范围，存在是没有意义的
         
         ```c
         if(1)
         {
             continue; // 会报错
         }
         ```

3. goto
   
   1. goto 会破坏结构化程序设计流程，它将使程序层次不清，且不易读，所以慎用。
   
   2. 其仅能在本函数内实现跳转，不能实现跨函数跳转(短跳转)。但是他在跳出多重循环的时候效率还是蛮高的。
   
   3. 示例
      
      `goto code;`表示跳转到标志`code:`处。
      
      ![](D:\Programmering%20Learning\Markdown文档\C语言教程\图片\goto跳转.png)
      
      ```c
      #include <stdio.h>
      
      int main()
      {
          while (1)
          {
              while(2)
              {
                  goto lnj;
              }
          }
          lnj:printf("跳过了所有循环");
      
          return 0;
      }
      ```

## 循环的嵌套

1. 定义：循环结构的循环体中存在其他的循环结构，我们称之为循环嵌套。

2. 注意：一般循环嵌套不超过三层。外循环执行的次数 * 内循环执行的次数就是内循环总共执行的次数。

3. 格式.
   
   ```c
   while(条件表达式) 
   {
       while循环结构 or do while循环结构 or for循环结构
   }
   ```
   
   ```c
   for(初始化表达式；循环条件表达式；循环后的操作表达式)
   {
       while循环结构 or do while循环结构 or for循环结构
   }
   ```
   
   ```c
   do
   {
       while循环结构 or do while循环结构 or for循环结构
   } while (循环控制条件 );
   ```

4. 循环优化
   
      在多重循环中，如果有可能，应当将最长的循环放在最内层，最短的循环放在最外层，以减少 CPU跨切循环层的次数。
   
   ```c
   for (row=0; row<100; row++)
   {
       // 低效率：长循环在最外层
       for ( col=0; col<5; col++ )
       {
           sum = sum + a[row][col];
       }
   }
   ```
   
   ```c
   for (col=0; col<5; col++ )
   {
       // 高效率：长循环在最内层
       for (row=0; row<100; row++)
       {
           sum = sum + a[row][col];
       }
   }
   ```

5. 打印好友列表
   
   ```c
   好友列表1
       好友1
       好友2
   好友列表2
       好友1
       好友2
   好友列表3
       好友1
       好友2
   ```
   
   ```c
   for (int i = 0; i < 4; i++)
   {
       printf("好友列表%d\n", i+1);
       for (int j = 0; j < 4; j++)
       {
           printf(" 角色%d\n", j);
       }
   }
   ```

## 图形打印

一重循环解决线性的问题，而二重循环和三重循环就可以解决平面和立体的问题了

1. 打印矩形
   
   ```c
   #include <stdio.h>
   
   int main()
   {
       // 3行4列
       // 外循环控制行数
       for (int i = 0; i < 3; i++)
       {
           // 内循环控制列数
           for (int j = 0; j < 4; j++)
           {    
               printf("*"); 
           } 
           printf("\n");
       }
   
       return 0;
   }
   ```
   
   ![](D:\Programmering%20Learning\Markdown文档\C语言教程\图片\图形打印01.png)

2. 打印三角形
   
   1. 尖尖朝上，改变内循环的条件表达式，让内循环的条件表达式随着外循环的i值变化
      
      ```c
      #include <stdio.h>
      
      int main()
      {
          /*最多打印5行最多打印5列每一行和每一列关系是什么? 列数<=行数*/
          for(int i = 0; i< 5; i++)
          {
              for(int j = 0; j <= i; j++)
              { 
                  printf("*");
              } 
              printf("\n");
          }
      
          return 0;
      }
      ```
      
      ![](D:\Programmering%20Learning\Markdown文档\C语言教程\图片\图形打印02.png)
   
   2. 尖尖朝下，改变内循环的初始化表达式，让内循环的初始化表达式随着外循环的i值变化
      
      ```c
      #include <stdio.h>
      
      int main()
      {
          for(int i = 0; i< 5; i++)
          { 
              for(int j = i; j < 5; j++)
              { 
                  printf("*");
              } 
              printf("\n");
          }
      
          return 0;
      }
      ```
      
      ![](D:\Programmering%20Learning\Markdown文档\C语言教程\图片\图形打印03.png)
   
   3. 等腰三角形
      
      ```c
      #include <stdio.h>
      
      int main()
      {
          int sides, i, j, spaceCount;
      
          printf("请输入打印的等边三角形的边长(即行数): ");
          scanf("%d", &sides);
      
          // 打印等边三角形
          for (i = 1; i <= sides; i++)
          {
              spaceCount = sides - i;
              for (j = 1; j <= spaceCount; j++)
              {
                  printf(" ");
              }
              for (j = 1; j <= 2 * i - 1; j++)
              { 
                  // 每行输出星号数量是奇数，确保形成等边三角形
                  printf("*");
              }
              printf("\n");
          }
      
          return 0;
      }
      ```
      
      ![](D:\Programmering%20Learning\Markdown文档\C语言教程\图片\图形打印04.png)

3. 打印特殊三角形
   
   1. 1 12 123
      
      ```c
      #include <stdio.h>
      
      int main()
      {
          for (int i = 0; i < 3; i++)
          { 
              for (int j = 0; j <= i; j++)
              {
                  printf("%d", j+1); 
              } 
              printf("\n");
          }
      
          return 0;
      }
      ```
      
      ![](D:\Programmering%20Learning\Markdown文档\C语言教程\图片\图形打印05.png)
   
   2. 1 22 333
      
      ```c
      #include <stdio.h>
      
      int main()
      {
          for (int i = 1; i <= 3; i++)
          { 
              for (int j = 1; j <= i; j++)
              {
                  printf("%d", i); 
              } 
              printf("\n");
          }
      
          return 0;
      }
      ```
      
      ![](D:\Programmering%20Learning\Markdown文档\C语言教程\图片\图形打印06.png)
   
   3. --*-********
      
      ```c
      #include <stdio.h>
      
      int main()
      {
          for (int i = 0; i <= 5; i++)
          { 
              for (int j = 0; j < 5 - i; j++)
              {
                  printf("-"); 
              } 
              for (int m = 0; m < 2*i+1; m++)
              { 
                  printf("*"); 
              }
              printf("\n");
          }
      
          return 0;
      }
      ```
      
      ![](D:\Programmering%20Learning\Markdown文档\C语言教程\图片\图形打印07.png)

4. 打印九九乘法表
   
   ```c
   #include <stdio.h>
   
   int main()
   {
       for (int i = 1; i <= 9; i++)
       { 
           for (int j = 1; j <= i; j++)
           {
               printf("%d * %d = %d \t", j, i, (j * i));
           }
           printf("\n");
       }
   
       return 0;
   }
   ```
   
   ![](D:\Programmering%20Learning\Markdown文档\C语言教程\图片\图形打印08.png)

# 函数

1. 函数的定义
   
      函数是一组一起执行一个任务的语句。每个 C 程序都至少有一个函数，即主函数 **main()** ，所有简单的程序都可以定义其他额外的函数。

2. 函数的分类
   
   `从函数的定义者分`
   
   1. 库函数
      
      C语言库文件中定义好的函数，无需自己定义，只需在文件中引入头文件即可直接使用。
      
      注：库文件可以在文章最后了解。
   
   2. 自定义函数
   
   `从有无返回值分`
   
   4. 有返回值函数
      
         此类函数被调用执行完后将向调用者返回一个执行结果,称为函数返回值。(必须指
      定返回值类型和使用return关键字返回对应数据)。
   
   5. 无返回值函数
      
         此类函数用于完成某项特定的处理任务,执行完成后不向调用者返回函数值。(返回值类型为void, 不用使用return关键字返回对应数据)。
   
   `从有无参数分`
   
   7. 有参函数
      
         在函数定义及函数说明时都有参数,称为形式参数(简称为形参)。在函数调用时也必须给出参数,称为实际参数(简称为实参)。
   
   8. 无参函数
      
         在函数定义及函数说明及函数调用中均不带参数。主调函数和被调函数之间不进行参数传送。

## 函数的定义

1. 有返回值函数
   
   1. 格式
      
      ```c
      返回值类型 函数名(参数类型 形式参数1，参数类型 形式参数2，……)
      { 
          函数体;
      
          返回值;
      }
      ```
   
   2. 示例
      
      ```c
      //有参数
      //实现两个整数的求和
      int add(int x,int y)
      {
          return x=y;
      }
      ```
      
      ```c
      //无参数
      //实现两个整数的求和
      int add()
      {
          int x;
          int y;
      
          return x=y;
      }
      ```

2. 无返回值函数
   
   1. 格式
      
      ```c
      void 函数名(参数类型 形式参数1，参数类型 形式参数2，……)
      { 
          函数体;
      }
      ```
   
   2. 示例
      
      ```c
      void add(int x,int y)
      {
          printf("%i\n",x+y)
      }
      ```
      
      ```c
      void add()
      {
          int x;
          int y;
          printf("%i\n",x+y);
      }
      ```

3. 注：函数名称不能相同。自定义函数名不能与库函数名称相同，无论你用不用库函数。

4. 函数的参数和返回值
   
   1. 形式参数：函数名后面小括号()中定义的变量称为形式参数，简称形参。
      
      1. 形参变量只有在被调用时才分配内存单元,在调用结束时,即刻释放所分配的内存单元。
      
      2. 形参只有在函数内部有效,函数调用结束返回主调函数后则不能再使用该形参变量。
      
      3. 示例
         
         ```c
         int add(int x,int y)//形式参数
         {
             return x=y;
         }
         ```
   
   2. 实际参数：在调用函数时, 传入的值称为实际参数，简称实参。
      
      1. 实参可以是常量、变量、表达式、函数等,无论实参是何种类型的量,在进行函数调用时,它们都必须具有确定的值,以便把这些值传送给形参。
      
      2. 应预先用赋值,输入等办法使实参获得确定值。
      
      3. 示例
         
         ```c
         int main()
         {
             int a,b;//实际参数
             scanf("%d %d",&a,&b);//给实参赋值
         
             return 0;
         }
         ```
   
   3. 注意点
      
      1. 调用函数时传递的实参个数必须和函数的形参个数必须保持一致。
         
         ```c
         #include <stdio.h>
         
         void add(int x,int y)//两个形式参数
         {
             printf("%i\n",x+y);
         }
         
         int main()
         {
             int a,b;
             scanf("%d %d",&a,&b);
         
             //调用函数
             add(a,b);//两个实际参数
         
             return 0;
         }
         ```
         
      2. 形参实参类型不一致, 会自动转换为形参类型。
         
         ```c
         #include <stdio.h>
         
         void change(double number1, double number2)//  形式参数
         { 
             // 输出结果:10.000000, 20.000000   
             // 自动将实参转换为double类型后保存   
             printf("number1 =%f, number2 = %f", number1, number2);
         }
         int main()
         {
             //调用函数
             change(10,20);
             
             return 0;
         }
         ```
         
      3. 当使用基本数据类型（char、int、float等）作为实参时，实参和形参之间只是值传递，修改形参的值并不影响到实参函数可以没有形参。
         
         ```c
         #include <stdio.h>
         
         void change(int number1, int number2)//  形式参数
         { 
             number1 = 250; // 不会影响实参    
             number2 = 222;
         }
         
         int main()
         {
             int a = 88;
             int b = 99;
         
             change(a, b);
         
             printf("a  = %d, b = %d", a, b); // 输出结果: 88, 99    
         
             return 0;
         }
         ```
      
      4. 如果没有写返回值类型，默认是int。
         
         ```c
         max(int number1, int number2)//  形式参数
         {
             return number1 > number2 ? number1 : number2;
         }
         ```
      
      5. 函数返回值的类型和return实际返回的值类型应保持一致。如果两者不一致,则以返回值类型为准,自动进行类型转换。
         
         ```c
         #include <stdio.h>
         
         int height()
         {
             return 3.14;
         }
         
         int main()
         {
             double temp = height();
             printf("%lf", temp);// 输出结果: 3.000000
         
             return 0;
         }
         ```
      
      6. 一个函数内部可以多次使用return语句，但是return语句后面的代码就不再被执行。
         
         ```c
         int max(int number1, int number2)//  形式参数
         {
             return number1 > number2 ? number1 : number2;
         
             printf("执行不到"); // 执行不到    
             return 250; // 执行不到
         }
         ```

## 函数的声明与实现

1. 函数声明定义：函数声明,就是在函数调用之前告诉系统, 该函数叫什么名称, 该函数接收几个参数, 该函数的返回值类型是什么。
   
    默认情况下，只有后面定义的函数才可以调用前面定义过的函数。如果想把函数的定义写在main函数后面，而且main函数能正常调用这些函数，那就必须在main函数的前面进行函数的声明, 否则系统搞不清楚有没有这个函数、系统搞不清楚这个函数接收几个参数、系统搞不清楚这个函数的返回值类型是什么。

2. 示例
   
   ```c
   #include <stdio.h>
   
   // 函数声明
   void getMax(int v1, int v2);
   
   int main(int argc, const char * argv[])
   {
       getMax(10, 20); // 调用函数    
   
       return 0;
   }
   
   // 函数实现
   void getMax(int v1, int v2)
   {
       int max = v1 > v2 ? v1 : v2;
       printf("max = %i\n", max);
   }
   ```

3. 注意点
   
   1. 函数的实现不能重复, 而函数的声明可以重复。
      
      ```c
      // 函数声明
      void getMax(int v1, int v2);
      
      void getMax(int v1, int v2);
      
      void getMax(int v1, int v2); // 不会报错
      
      int main(int argc, const char * argv[])
      {
          getMax(10, 20); // 调用函数    
      
          return 0;
      }
      
      // 函数实现
      void getMax(int v1, int v2)
      {
          int max = v1 > v2 ? v1 : v2;
          printf("max = %i\n", max);
      }
      ```
   
   2. 函数声明可以写在函数外面,也可以写在函数里面, 只要在调用之前被声明即可。
      
      ```c
      int main(int argc, const char * argv[])
      {
          void getMax(int v1, int v2); //函数声明, 不会报错    
      
          getMax(10, 20); // 调用函数    
      
          return 0;
      }
      
      // 函数实现
      voidgetMax(int v1, int v2)
      {
          int max = v1 > v2 ? v1 : v2;
          printf("max =%i\n", max);
      }
      ```
   
   3. 当被调函数的函数定义出现在主调函数之前时,在主调函数中也可以不对被调函数再作声明。
      
      ```c
      // 函数实现
      void getMax(int v1, int v2)
      {
          int max = v1 > v2 ? v1 : v2;
          printf("max = %i\n", max);
      }
      
      int main(int argc, const char * argv[])
      {
          getMax(10, 20); // 调用函数    
      
          return 0;
      }
      ```
   
   4. 如果被调函数的返回值是整型时,可以不对被调函数作说明,而直接调用。
      
      ```c
      int main(int argc, const char * argv[])
      {
          int res = getMin(5, 3); // 不会报错    
          printf("result = %d\n", res ); 
      
          return 0;
      }
      
      int getMin(int num1, int num2)'
      {
          // 返回int, 不用声明
          return num1 < num2 ? num1:num2;
      }
      ```

## argc、argv[ ]（命令行参数）

1. argc
   
   系统在启动程序时调用main函数时传递给argv的值的个数，也就是命令行参数数量。

2. argv[ ]
   
      **argv[]** 是一个指针数组，指向传递给程序的每个参数。
   
      系统在启动程序时传入的的值, 默认情况下系统只会传入一个值, 这个值就是main函数执行文件的路径。
   
   注：数组的详细知识会在后面讲到。

3. 解释
   
   ```c
   #include <stdio.h>
   
   int main(int argc, char *argv[])
   {
       printf("argc is %d\n",argc);
   
       for(int i=0;i<argc;i++)
       {
           printf("argv[%d] is: %s\n",i,argv[i]);    
       }
   
       return 0;
   }
   ```
   
   命令行编译
   
   没有传入参数（只含有默认值）
   
   ![](D:\Programmering%20Learning\Markdown文档\C语言教程\图片\argc、argv[%20]01.png)
   
   传入参数（默认值+传入参数）
   
   ![](D:\Programmering%20Learning\Markdown文档\C语言教程\图片\argc、argv[%20]02.png) 

4. 使用场景
   
   这个参数在windows操作系统不常用，常在linux中使用。当你需要在命令行中运行此程序，然后你又不想在程序运行输入参数，然后你就可以使用命令行参数在命令行中传递参数，也就是说程序在运行的时候就带有参数，在需要用的时候直接代入，不需要你进行输入。
   
   例如说`ping 172.0.2.1` 其中的`ping`就是一个程序，后面的`172.0.2.1`就是参数。

## 递归函数

1. 定义：一个函数在它的函数体内调用它自身称为递归调用。

2. 构成条件
   
   1. 自己调用自己
   
   2. 存在一个条件能够让递归结束
   
   3. 问题的规模能够缩小

3. 示例
   
   ```c
   #include <stdio.h>
   
   void getNumber()
   { 
       int number = -1; 
       while (number < 0)
       { 
           printf("请输入一个正数\n"); 
           scanf("%d", &number); 
       } 
       printf("number = %d\n",number);
   }
   
   int main()
   {
       getNumber();
   
       return 0;
   }
   ```
   
   ![](D:\Programmering%20Learning\Markdown文档\C语言教程\图片\递归函数01.png)
   
   ```c
   #include <stdio.h>
   
   void getNumber2()
   { 
       int number = -1; 
       printf("请输入一个正数abc\n");
       scanf("%d", &number); 
       if (number < 0) 
       {
           // 负数 
           getNumber2();
       }else
       {
           // 正数 
           printf("number = %d\n", number); 
       }
   }
   
   int main()
   {
       getNumber2();
   
       return 0;
   }
   ```
   
   ![](D:\Programmering%20Learning\Markdown文档\C语言教程\图片\递归函数02.png)

4. 递归和循环的区别
   
   1. 能用循环实现的功能,用递归都可以实现
   
   2. 递归常用于"回溯", "树的遍历","图的搜索"等问题
   
   3. 但代码理解难度大，内存消耗大(易导致栈溢出), 所以考虑到代码理解难度和内存消耗问题, 在企业开发中一般能用循环都不会使用递归

5. 练习
   
   1. 有5个人坐在一起,问第5个人多少岁?他说比第4个人大两岁。问 第4个人岁数,他说比第3个人大两岁。问第3个人,又说比第2个 人大两岁。问第2个人,说比第1个人大两岁。最后问第1个人, 他说是10岁。请问第5个人多大?
      
      ```c
      #include <stdio.h>
      
      int next_age(int age)
      {
          return age + 2;
      }
      
      int main()
      {
          int first_person_age = 10;
          int fifth_person_age = first_person_age;
      
          for (int i = 1; i <= 4; i++)
          {
              fifth_person_age = next_age(fifth_person_age);
          }
      
          printf("第5个人的年龄是%d岁\n", fifth_person_age);
      
          return 0;
      }
      ```
   
   2. 用递归法求N的阶乘
      
      ```c
      #include <stdio.h>
      
      // 定义阶乘函数
      long long factorial(int n)
      {
          if (n == 0 || n == 1)
          {
              return 1;
          }
          else
          {
              return n * factorial(n - 1);
          }
      }
      
      int main()
      {
          int n;
          printf("请输入一个整数：");
          scanf("%d", &n);
          printf("%d的阶乘为%lld\n", n, factorial(n));
      
          return 0;
      }
      ```
   
   3. 设计一个函数用来计算B的n次方（B和n均为正整数）
      
      ```c
      #include <stdio.h>
      
      int power(int base, int exponent)
      {
          if (exponent == 0)
          {
              return 1;
          }
          else
          {
              return base * power(base, exponent - 1);
          }
      }
      
      int main()
      {
          int B, n;
          printf("请输入基数B:");
          scanf("%d", &B);
          printf("请输入指数n:");
          scanf("%d", &n);
          printf("%d的%d次方等于%d\n", B, n, power(B, n));
      
          return 0;
      }
      ```

# 位运算符

* 程序中的所有数据在计算机内存中都是以二进制的形式储存的。

* 位运算就是直接对整数在内存中的二进制位进行操作

* C语言提供了6个位操作运算符, 这些运算符只能用于整型操作数  

![](D:\Programmering Learning\Markdown文档\C语言教程\图片\位运算符01.png)

1. 按位与
   
   1. 定义：只有对应的两个二进位均为1时，结果位才为1，否则为0
   
   2. 规律：规律: 二进制中，与1相&就保持原位，与0相&就为0
   
   3. 解释
      
      ![](D:\Programmering%20Learning\Markdown文档\C语言教程\图片\drawio\按位与.drawio.png)

2. 按位或
   
   1. 定义：只要对应的二个二进位有一个为1时，结果位就为1，否则为0
   
   2. 解释
      
      ![](D:\Programmering%20Learning\Markdown文档\C语言教程\图片\drawio\按位或.drawio.png)

3. 按位异或
   
   1. 定义：当对应的二进位相异（不相同）时，结果为1，否则为0
   
   2. 规律
      
      1. 相同整数相^的结果是0。比如5^5=0
      
      2. 多个整数相^的结果跟顺序无关。例如: 5^6^7=5^7^6
      
      3. 同一个数异或另外一个数两次, 结果还是那个数。例如: 5^7^7 = 5
   
   3. 解释
      
      ![](D:\Programmering%20Learning\Markdown文档\C语言教程\图片\drawio\按位异或.drawio.png)

4. 按位取反
   
   1. 定义：各二进位进行取反（0变1，1变0）
   
   2. 解释
      
      ```c
      ~9=-10
      //取反前
      0000 1001
      //取反后（补码）
      1111 0110
      //取反后得到的数字符号位为1，表明为负数，计算机中负数运算以补码进行
      //负数补码变原码，先减1得到反码，符号位不变，其他取反
      //反码
      11110101
      //原码
      10001010
      //十进制
      -10
      ```

5. 按位左移
   
   1. 定义：把整数a的各二进位全部左移n位，高位丢弃，低位补0
   
   2. 注意：由于左移是丢弃最高位，0补最低位，所以符号位也会被丢弃，左移出来的结果值可能会改变正负性。
   
   3. 规律：左移n位其实就是乘以2的n次方。
   
   4. 解释
      
      ```c
      2<<1（表示2左移1位）  =4
      //相当于2*=2   //4
      //左移前
      0010  十进制2
      //左移后
      0100  十进制4
      
      2<<2（表示2左移两位） =8
      //相当于2*2^2 //8
      //左移前
      0010 十进制2
      //左移后
      1000 十进制8
      ```

6. 按位右移
   
   1. 定义：把整数a的各二进位全部右移n位，保持符号位不变。
   
   2. 注意
      
      1. 为正数时， 符号位为0，最高位补0
      
      2. 为负数时，符号位为1，最高位是补0或是补1(取决于编译系统的规定)
   
   3. 规律：快速计算一个数除以2的n次方。
   
   4. 解释
      
      ```c
      2>>1（表示2右移一位）  =1
      //相当于2/=2   //1
      //右移前
      0010  十进制2
      //右移后
      0001  十进制1 
      
      4>>2（表示4右移两位） =1
      //相当于4/=2 //1
      //右移前
      0100 十进制4
      //右移后
      0001 十进制1
      ```

7. 应用场景
   
   1. 判断奇偶（按位与）
      
      ```c
      偶数: 其二进制是以0结尾 
      8 -> 1000 
      10 -> 1010 
      奇数: 二进制是以1结尾
      9 -> 1001 
      11 -> 1011 
      
      规律：任何数和1进行&操作,得到这个数的最低位 
      
        1000 
      & 0001
      ------- 
        0000 // 结果为0, 代表是偶数 
      
        1011 
      & 0001 
      ------- 
        0001 // 结果为1,代表是奇数
      ```
   
   2. 权限系统
   
   3. 交换两个数的值（按位异或）（不推荐使用此方法交换两个数的值）
      
      前提：这两个数的值是不同的，否则交换完的数值就是0。
      
      ```c
      #include <stdio.h>
      
      void swap(int a, int b)
      {
          a = a ^ b;
          b = a ^ b;
          a = a ^ b;
      }
      
      int main()
      {
          int num1, num2;
          printf("请输入两个整数：");
          scanf("%d%d", &num1, &num2);
      
          printf("交换前：\n");
          printf("num1 = %d\nnum2=%d\n", num1, num2);
      
          swap(&num1, &num2);
      
          printf("交换后：\n");
          printf("num1 = %d\nnum2 = %d\n", num1, num2);
      
          return 0;
      }
      ```

8. 练习
   
   写一个函数把一个10进制数按照二进制格式输出
   
   ```c
   #include <stdio.h>
   
   void printBinary(int num)
   { 
       int len =sizeof(int)*8; 
       int temp; 
       for (int i=0; i<len; i++)
       { 
           temp = num; 
           //每次都在原数的基础上进行移位运算 
           temp = temp>>(31-i); 
           //每次移动的位数 
           int t = temp&1; 
           //取出最后一位 
           if(i!=0&&i%4==0)
           printf(" "); 
           printf("%d",t);
       }
       printf("\n");
   }
   
   int main(int argc, const char *argv[])
   { 
       int num;
       scanf("%d",&num);
       printBinary(num);
   
       return 0;
   }
   //此处主函数括号中的参数的解释
   //argc,argv可以使程序接受命令行参数，更方便的IO（输入输出）
   ```

# 转义字符

1. 定义：使用编码值来间接地表示字符的方式称为转义字符（Escape Character）。

2. 转义字符以`\`或者`\x`开头，以`\`开头表示后跟八进制形式的编码值，以`\x`开头表示后跟十六进制形式的编码值。对于转义字符来说，只能使用八进制或者十六进制。

3. 注意
   
   1. 转义字符的初衷是用于 ASCII 编码，所以它的取值范围有限
   
   2. 八进制形式的转义字符最多后跟三个数字，也即`\ddd`，最大取值是`\177`
   
   3. 十六进制形式的转义字符最多后跟两个数字，也即`\xdd`，最大取值是`\x7f`
   
   4. 超出范围的转义字符的行为是未定义的，有的编译器会将编码值直接输出，有的编译器会报错。

![](D:\Programmering%20Learning\Markdown文档\C语言教程\图片\转义字符.png)

```c
printf("Hello,\\\n");//Hello,\

char a = '\61';  //字符1
char b = '\141';  //字符a
char c = '\x31';  //字符1
char d = '\x61';  //字符a
char *str1 = "\x31\x32\x33\x61\x62\x63";  //字符串"123abc"
char *str2 = "\61\62\63\141\142\143";  //字符串"123abc"
char *str3 = "The string is: \61\62\63\x61\x62\x63"  //混用八进制和十六进制形式
```

# 类型说明符

C语言提供了说明长度和说明符号位的两种类型说明符, 这两种类型说明符一共有4个

1. short 短整型 (说明长度)

2. long 长整型 (说明长度)

3. signed 有符号型 (说明符号位)

4. unsigned 无符号型 (说明符号位)

5. 这些说明符一般都是用来修饰int类型的，所以在使用时可以省略int

## short和long

1. 在64位编辑器环境下
   
   1. int占用4个字节（32bit），取值范围是-2^31 ~ （2^31）-1
   2. short占用2个字节（16bit），取值范围是-2^15 ~ （2^15）-1
   3. long占用8个字节（64bit），取值范围是-2^63 ~（ 2^63）-1

2. 在其他位数编辑器环境下
   
   1. short跟int至少为16位(2字节)
   
   2. long至少为32位(4字节)
   
   3. short的长度不能大于int，int的长度不能大于long
   
   4. char一定为为8位(1字节)

3. 可以连续使用2个long，也就是long long。一般来说，long long的范围是不小于long的，比如在32bit编译器环境下，long long占用8个字节，long占用4个字节。不过在64bit编译器环境下，long long跟long是一样的，都占用8个字节。

4. 解释
   
   ```c
   #include <stdio.h>
   
   int main()
   { 
       // char占1个字节, char的取值范围 -2^7~2^7 
       char num = 129; 
       printf("size = %i\n", sizeof(num)); // 1 
       printf("num = %i\n",num); // -127 
   
       // short int 占2个字节, short int的取值范围 -2^15~（2^15）-1 
       short int num1 = 32769;// -32767 
       printf("size = %i\n", sizeof(num1)); // 2
       printf("num1 = %hi\n", num1); 
   
       // int占4个字节, int的取值范围 -2^31~（2^31）-1 
       int num2 = 12345678901; 
       printf("size = %i\n", sizeof(num2)); // 4 
       printf("num2= %i\n", num2); 
   
       // long在32位占4个字节, 在64位占8个字节 
       long int num3 =12345678901; 
       printf("size = %i\n", sizeof(num3)); // 4或8 
       printf("num3 =%ld\n", num3); 
   
       // long在32位占8个字节, 在64位占8个字节 -2^63~（2^63）-1 
       long long int num4 = 12345678901; 
       printf("size = %i\n", sizeof(num4)); // 8
       printf("num4 = %lld\n", num4); 
   
       // 由于short/long/long long一般都是用于修饰int, 所以int可以省略 
       short num5 = 123; 
       printf("num5 = %lld\n", num5); 
       long num6 = 123; 
       printf("num6 = %lld\n", num6); 
       long long num7 = 123;
       printf("num7 = %lld\n", num7); 
   
       return 0;
   }
   ```
   
   ![](D:\Programmering%20Learning\Markdown文档\C语言教程\图片\short、long02.png)
   
   ![](D:\Programmering%20Learning\Markdown文档\C语言教程\图片\short、long01.png)

## signed和unsigned

1. signed int等价于signed，unsigned int等价于unsigned

2. signed和unsigned的区别
   
   它们的最高位是否要当做符号位，并不会像short和long那样改变数据的长度，即所占的字节数。

3. signed
   
   1. 定义：表示有符号，也就是说最高位要当做符号位。
   
   2. 注意：int的最高位本来就是符号位，因此signed和int是一样的，signed等价于signed int，也等价于int。
   
   3. 取值范围：-2^31 ~ （2^31）-1

4. unsigned
   
   1. 定义：表示无符号，也就是说最高位并不当做符号位，所以不包括负数。
   
   2. 取值范围：0 ~ （2^32） - 1

5. 解释
   
   ```c
   #include <stdio.h>
   
   int main()
   { 
       // 1.默认情况下所有类型都是由符号的 
       int num1 = 9;
       int num2 = -9; 
       int num3 = 0; 
       printf("num1 = %i\n", num1);
       printf("num2 = %i\n", num2); 
       printf("num3 = %i\n", num3); 
   
       // 2.signed用于明确说明, 当前保存的数据可以是有符号的, 一般情况下很少使用 
       signed int num4 = 9;
       signed int num5 = -9; 
       signed int num6 = 0; 
       printf("num4 = %i\n", num4);
       printf("num5 = %i\n", num5); 
       printf("num6 = %i\n", num6); 
   
       // signed也可以省略数据类型, 但是不推荐这样编写 
       signed num7 = 9; 
       printf("num7 = %i\n", num7);
   
       // 3.unsigned用于明确说明, 当前不能保存有符号的值, 只能保存0和正数 
       // 应用场景: 保存银行存款,学生分数等不能是负数的情况 
       unsigned int num8 = -9; 
       unsigned int num9 =0; 
       unsigned int num10 = 9; 
   
       // 注意: 不看怎么存只看怎么取 
       printf("num8 =%u\n", num8); 
       printf("num9 = %u\n", num9); 
       printf("num10 = %u\n", num10);
   
       return 0;
   }
   ```
   
   ![](D:\Programmering%20Learning\Markdown文档\C语言教程\图片\signed、unsigned01.png)

6. 注意
   
   1. 修饰符号的说明符可以和修饰长度的说明符混合使用
   
   2. 相同类型的说明符不能混合使用
   
   3. 解释
      
      ```c
      signed short int num1 = 666; 
      
      signed unsigned int num2 = 666; // 报错
      ```

# 一维数组

1. 定义：一组相同数据类型的有序集合。数据可以是数字，数字数组，简称数组；可以使字符，字符数组。数组属于构造数据类型。

2. 作用：存储一组数据。

3. 相关名词
   
   1. 数组元素：构成数组的每一个数据
   
   2. 数组元素位置的索引(从0开始)

4. 定义数组
   
   1. 格式：`元素类型 数组名[元素个数];`
   
   2. 示例
      
      ```c
      int num[32];
      //int 元素类型
      //num 数组名
      //32 元素个数
      char str[5];
      //char 元素类型
      //str 数组名
      //5 元素个数
      ```

5. 初始化数组
   
   1. 定义时初始化
      
      1. 完全初始化
         
         1. 指定元素数量
            
            ```c
            int nums[5] = {1,2,3,5,6};
            ```
         
         2. 不指定元素数量
            
            ```c
            int ages[] = {4, 6, 9};
            //根据花括号｛｝中的数字数量确定数组元素数量
            ```
      
      2. 部分初始化
         
         1. 指定元素数量
            
            ```c
            int nums[10] = {1,2};
            
            int nums[5] = {[4] = 3,[1] = 2};
            ```
         
         2. 不指定元素数量
            
            ```c
            int nums[] = {[4] = 3};
            ```

   2. 先定义后初始化
   
      ```C
      int nums[3];
      nums[0] = 1;
      nums[1] = 2;
      nums[2] = 3;
      ```
   
   3. 不初始化
   
      如果定义数组后,没有初始化,数组中是有值的,是随机的垃圾数。
   
8. 注意
   
   1. 使用数组时不能超出数组的索引范围使用, 索引从0开始, 到元素个数-1结束。
   
   2. 使用数组时不要随意使用未初始化的元素, 有可能是一个随机值。
   
   3. 对于数组来说, 只能在定义的同时初始化多个值, 不能先定义再初始化多个值。
      
      ```c
      int ages[3];
      ages = {4, 6, 9}; // 报错
      ```

9. 数组的使用
   
   通过下标（索引）访问
   
   ```c
   #include <stdio.h>
   
   int main()
   {
       int nums[3]={1,2,3};
   
       //访问数组
       int a=nums[2];
   
       printf("%d\n",a);//3
   
       return 0;
   }
   ```

## 数组的遍历

有序的访问并输出数组元素。

```c
//正序输出
for(int i=0;i<4;i++)
{
    printf("%d ",nums[i]);
}

//逆序输出
for(int i=3;i>=0;i--)
{
    printf("%d ",nums[i]);
}
```

```c
#include <stdio.h>

int main()
{
    int m;
    printf("请输入数组长度：");
    scanf("%d",&m);

    int nums[m];
    //此处注意，原生数组里面是不支持动态的，也就是说数组长度只能是常量或者常量表达式，不能为变量，但是在C99标准当中引入了一个C语言特性VLA（Variable-Length Array），这个特性使得数组长度可以为变量，也就是说数组的大小从编译期确定变成了运行期确定，但是部分编译器不支持该特性，所以一般还是不要这样使用，如果想使用变长的数组，后面会讲到。
    //因此不推荐这样写，但这样写在支持VLC的编译器上面是没错的。（Visual Studio不支持此特性）

    //循环初始化数组
    printf("请输入数组元素：");
    for(int i=0;i<m;i++)
    {
        scanf("%d",&nums[i]);
    }

    //遍历数组
    for(int i=0;i<m;i++)
    {
        printf("%d ",nums[i]);
    }
    printf("\n");

    return 0;
}
```

![](D:\Programmering%20Learning\Markdown文档\C语言教程\图片\遍历数组.png)

## 数组长度的计算

1. 原理：数组所占用存储空间 = 一个元素所占用存储空间 * 元素个数(数组长度)

2. 方法：数组的长度 = 数组占用的总字节数 / 数组元素占用的字节数

3. 示例
   
   ```c
   #include <stdio.h>
   
   int main()
   {
       int nums[]={1,2,3};
   
       int length=sizeof(nums)/sizeof(int);
   
       printf("%d\n",length);//3
   
       return 0;
   }
   ```

4. 注意
   
   如果指定了数组长度，那么无论你是否完全初始化数组，计算出来的结果都是你指定好的数组长度。

## 数组越界

1. 数组内部存储细节
   
   1. 存储方式
      
      1. 内存寻址从大到小, 从高地址开辟一块连续没有被使用的内存给数组
      
      2. 从分配的连续存储空间中, 地址小的位置开始给每个元素分配空间
      
      3. 从每个元素分配的存储空间中, 地址最大的位置开始存储数据
      
      4. 用数组名指向整个存储空间最小的地址
   
   2. 示例
      
      ```c
      #include <stdio.h>
      
      int main()
      { 
          int num = 9; 
          printf("%p\n",&num);
      
          char cs[] = {'l','n','j'};
          printf("cs = %p\n", &cs);
          printf("cs[0] = %p\n",&cs[0]);
          printf("cs[1] = %p\n", &cs[1]);
          printf("cs[2] = %p\n", &cs[2]);
      
          int nums[] ={2, 6}; 
          printf("nums = %p\n", &nums);
          printf("nums[0] = %p\n", &nums[0]);
          printf("nums[1] =%p\n", &nums[1]);
      
          return 0;
      }
      ```
      
      ![](D:\Programmering%20Learning\Markdown文档\C语言教程\图片\数组存储细节01.png)
      
      注：地址是随机分配的，所以每次运行结果均不同。
      
      ![](D:\Programmering%20Learning\Markdown文档\C语言教程\图片\数组存储细节02.png)
      
      注：字符在内存中是以对应ASCII码值的二进制形式存储的,而非上述的形式。

2. 数组越界
   
   1. 示例
      
      ```c
      #include <stdio.h>
      
      int main()
      { 
          char cs1[2] = {1, 2};
          char cs2[3] = {3, 4, 5};
          cs2[3] = 88; // 注意:这句访问到了不属于cs1的内存
          printf("cs1[0] = %d\n", cs1[0]);//88
      
          return 0;
      }
      ```
   
   2. 分析
      
      ```c
      #include <stdio.h>
      
      int main()
      { 
          char cs1[2] = {1, 2};
          printf("cs1 = %p\n",&cs1);
          printf("cs1[0] = %p\n",&cs1[0]);
          printf("cs1[1] = %p\n",&cs1[1]);
          printf("cs1[2] = %p\n",&cs1[2]);
      
          char cs2[3] = {3, 4, 5};
          printf("cs2 = %p\n",&cs2);
          printf("cs2[0] = %p\n",&cs2[0]);
          printf("cs2[1] = %p\n",&cs2[1]);
          printf("cs2[2] = %p\n",&cs2[2]);
      
          return 0;
      }
      ```
      
      ![](D:\Programmering%20Learning\Markdown文档\C语言教程\图片\数组越界01.png)
      
      ![](D:\Programmering%20Learning\Markdown文档\C语言教程\图片\数组越界02.png)

3. 数组注意事项
   
   在定义数组的时候[ ]里面只能写整型常量或者是返回整型常量的表达式
   
   ```c
   int ages4['A'] = {19, 22, 33}; 
   printf("ages4[0] = %d\n", ages4[0]); 
   
   int ages5[5 + 5] = {19, 22, 33}; 
   printf("ages5[0] = %d\n", ages5[0]);
   
   int ages5['A' + 5] = {19, 22, 33}; 
   printf("ages5[0] = %d\n", ages5[0]);
   ```

## 数组和函数

1. 数组元素作为函数参数
   
   1. 数组的元素作为函数实参，与同类型的简单变量作为实参一样，如果是基本数据类型, 那么形参的改变不影响实参。
      
      ```c
      #include <stdio.h>
      
      void change(int val)// int val = number
      {
          val = 55;
      }
      int main(int argc, const char * argv[])
      {
          int ages[3] = {1, 5, 8};
          printf("ages[0] = %d", ages[0]);// 1
          change(ages[0]);
          printf("ages[0] = %d", ages[0]);// 1
          
          return 0;
      }
      ```
   
   2. 用数组元素作函数参数不要求形参也必须是数组元素。 

2. 数组名作为函数参数
   
   1. 在C语言中,数组名除作为变量的标识符之外,数组名还代表了该数组在内存中的起始地址,因此,当数组名作函数参数时,实参与形参之间不是"值传递",而是"地址传递"。
   
   2. 实参数组名将该数组的起始地址传递给形参数组,两个数组共享一段内存单元, 系统不再为形参数组分配存储单元。既然两个数组共享一段内存单元, 所以形参数组修改时，实参数组也同时被修改了。
      
      ```c
      #include <stdio.h>
      
      void change2(int array[3])// int array = 0ffd1
      {
          array[0] = 88;
      }
      int main(int argc, const char * argv[])
      {
          int ages[3] = {1, 5, 8};
          printf("ages[0] = %d", ages[0]);// 1
          change(ages);
          printf("ages[0] = %d", ages[0]);// 88
      
          return 0;
      }
      ```
   
   3. 注意点
      
      1. 在函数形参表中,允许不给出形参数组的长度
         
         ```c
         void change(int array[])
         {
             array[0] = 88;
         }
         ```
      
      2. 形参数组和实参数组的类型必须一致,否则将引起错误。
         
         ```c
         void prtArray(double array[3]) // 错误写法
         {
             for (int i = 0; i < 3; i++)
             {
                 printf("array[%d], %f", i, array[i]);
             }
         }
         
         int main(int argc, const char * argv[])
         {
             int ages[3] = {1, 5, 8};
             prtArray(ages[0]);
         }
         ```
         
      3. 当数组名作为函数参数时, 因为自动转换为了指针类型，所以在函数中无法动态计算除数组的元素个数。
         
         ```c
         void printArray(int array[])
         {
             printf("printArray size = %lu\n", sizeof(array)); // 8
             int length = sizeof(array)/ sizeof(int); // 2
             printf("length = %d", length);
         }
         ```

3. 练习

   1. 设计一个函数实现找出数组元素的最大值

      ```C
      #include <stdio.h>
      
      int arrayMax(int a[],int n)
      {
          int max=a[0];
          for(int i=1;i<n;i++)
          {
              if(a[i]>max)
              {
                  max=a[i];
              }
          }
          
          return max;
      }
      
      int main()
      {
          int n;
          scanf("%d",&n);
          int a[n];
          for(int i=0;i<n;i++)
          {
              scanf("%d",&a[i]);
          }
          arrayMax(a,n);
          printf("%d\n",arrayMax(a,n));
      
          return 0;
      }
      ```

   2. 从键盘输入3个0~9的数字，然后输出0~9中有哪些数字不曾出现

      ```c
      #include <stdio.h>
      
      int main()
      {
          int num1, num2, num3;
          printf("请输入3个0-9的数字:");
          code:scanf("%d%d%d", &num1, &num2, &num3);
          if(num1>9||num2>9||num3>9||num1<0||num2<0||num3<0)
          {
              printf("输入错误，请输入三个0~9的数字：");
              goto code;
          }
      
          printf("0-9中没有出现过这些数字:");
          for (int i = 0; i <= 9; i++)
          {
              if (i == num1 || i == num2 || i == num3)
              {
                  
              } 
              else
              {
                  printf("%d", i);
              }
          }
          printf("\n");
      
          return 0;
      }
      ```

# 二维数组

1. 定义

   二维数组是什么意思呢，从字面意思上看，就是这个数组的维数是2，想想我们日常生活中说的空间的维度，一维就是一个点，一条线，只有长没有宽，二维呢，就是一个平面，既有长，又有宽，三维就是一个立体，有长宽高。类比这理解，二维数组大致如下。

   但总体而言，二维数组还是由一维数组组成的。

2. 示例

   ```c
   int a[2][3]= {{80,75,92}, {61,65,71}};
   ```

   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\二维数组01.png)

3. 二维数组的定义

   1. 格式：`数据类型 数组名[一维数组的个数][一维数组的元素个数]`

      一维数组的个数：当前二维数组中包含多少个一维数组。

      一维数组的元素个数：每个一维数组的元素个数。

   2. 示例

      ```c
      int num[2][3];
      
      char str[2][3];
      ```

4. 二维数组的初始化

   1. 定义时初始化

      1. 完全初始化

         1. 按行分段赋值

            ```C
            int a[2][3]={ {80,75,92}, {61,65,71}};
            ```

         2. 按行连续赋值

            ```C
            int a[2][3]={ 80,75,92,61,65,71};
            ```

      2. 部分初始化

         1. 按行分段赋值

            ```C
            int a[2][3]={{1},{4,5}};
            ```

         2. 按行连续赋值

            ```C
            int a[2][3]={1,2,3,4};
            ```

      3. 其他赋值方法

         1. 无论是完全初始化还是部分初始化，都可以省去第一维的长度，也就是一维数组的个数。

            ```C
            //完全初始化
            int a[][3]={{1,2,3},{4,5,6}};
            int a[][3]={1,2,3,4,5,6};
            
            //部分初始化
            int a[][3]={{1},{4,5}};
            int a[][3]={1,2,3,4};
            ```

            注：无论何种初始化方法，都不可省略第二维的长度，也就是一维数组元素的个数，因为初始化的时候会先存放第一行，如果第一行的长度不确定，那么就会存储错乱。

         2. 指定元素的初始化

            ```C
            int a[2][3]={[1][2]=10};
            int a[2][3]={[1]={1,2,3}};
            ```

   2. 先定义后初始化

      ```c
      int a[2][3];
      a[0][0] = 80;
      a[0][1] = 75;
      a[0][2] = 92;
      a[1][0] = 61;
      a[1][1] = 65;
      a[1][2] = 71;
      ```

5. 应用场景

   使用一维不好解决或者解决起来比较麻烦的，比如：

   五子棋、象棋、围棋等棋类游戏。

   俄罗斯方块。

## 二维数组的遍历

```C
#include <stdio.h>

int main()
{
    int num[2][3]={{1,5,6},{4,8,9}};

    //外循环控制行数
    for(int i=0;i<2;i++)
    {
        //内循环控制列数
        for(int j=0;j<3;j++)
        {
            printf("%d ",num[i][j]);
        }
        printf("\n");
    }
    
    return 0;
}
```

![](D:\Programmering Learning\Markdown文档\C语言教程\图片\二维数组的遍历.png)

## 二维数组的存储

```C
#include <stdio.h>

int main()
{
    int nums[2][4]={{1,6,7,5},{2,8,4,9}};

    for(int i=0;i<2;i++)
    {
        for(int j=0;j<4;j++)
        {
            printf("nums[%d][%d] = %p\n",i,j,&nums[i][j]);
        }
    }

    return 0;
}
```

![](D:\Programmering Learning\Markdown文档\C语言教程\图片\二维数组存储01.png)

![](D:\Programmering Learning\Markdown文档\C语言教程\图片\二维数组存储02.png)

## 二维数组与函数

1. 值传递

   ```C
   #include <stdio.h>
   
   void change(char ch)
   {
       ch='h';
   }
   
   int main()
   {
   	char[2][3]={{'a','b','c'},{'d','e','f'}};
       printf("cs[0][0] = %c\n",cs[0][0]);//a
       change(cs[0][0]);
       printf("cs[0][0] = %c\n",cs[0][0]);//a
       
       return 0;
   }
   ```

2. 地址传递

   ```C
   #include <stdio.h>
   
   // 和一位数组一样, 只看形参是基本类型还是数组类型
   // 如果是数组类型在函数中修改形参会影响实参
   
   void change(char ch[])
   {
   	ch[0] = 'n';
   }
   int main()
   {
   	char cs[2][3] = {{'a', 'b', 'c'},{'d', 'e', 'f'}};
   	printf("cs[0][0] = %c\n", cs[0][0]); // a
   	change(cs[0]);
   	printf("cs[0][0] = %c\n", cs[0][0]); // n
   
       return 0;
   }
   ```

   ```C
   #include <stdio.h>
   
   // 和一位数组一样, 只看形参是基本类型还是数组类型
   // 如果是数组类型在函数中修改形参会影响实参
   
   void change(char ch[][3])
   {
   	ch[0][0] = 'n';
   }
   int main()
   {
   	char cs[2][3] = {{'a', 'b', 'c'},{'d', 'e', 'f'}};
   	printf("cs[0][0] = %c\n", cs[0][0]); // a
   	change(cs);
   	printf("cs[0][0] = %c\n", cs[0][0]); // n
   
       return 0;
   }
   ```

3. 形参错误写法

   ```C
   void test(char cs[2][]) // 错误写法
   {
   printf("我被执行了\n");
   }
   
   void test(char cs[2][3]) // 正确写法
   {
       printf("我被执行了\n");
   }
   
   void test(char cs[][3]) // 正确写法
   {
   printf("我被执行了\n");
   }
   ```

4. 二维数组作为函数参数，在被调函数中不能获得其有多少行，需要通过参数传入

   ```C
   void test(char cs[2][3])
   {
   	int row = sizeof(cs); // 输出4或8
   	printf("row = %zu\n", row);
   }
   ```

5. 二维数组作为函数参数，在被调函数中可以计算出二维数组有多少列

   ```C
   void test(char cs[2][3])
   {
   	size_t col = sizeof(cs[0]); // 输出3
   	printf("col = %zd\n", col);
   }
   
   ```

6. 练习

   1. 题目：玩家通过键盘录入 w,s,a,d控制小人向不同方向移动,其中w代表向上移动,s代表向 下移动,a代表向左
      移动,d 代表向右移动,当小人移动到出口位置,玩家胜利。

   2. 思路

      1. 定义二维数组存放地图

         ```C
         ######
         #O #
         # ## #
         # # #
         ## #
         ######
         ```

      2. 规定地图的方向

         纵向为X轴，横向为Y轴

      3. 编写程序控制方向

         当输入w或者W, 小人向上移动. x-1
         当输入s 或者S, 小人向下. x+1
         当输入a或者A, 小人向左. y-1
         当输入d或者D, 小人向右. y+1

      4. 移动小人

         用变量记录小人当前的位置

         * 如果小人将要移动的位置是墙,则无法移动
         * 如果小人将要移动的位置是路,则可以移动

      5. 判断是否走出迷宫

   3. 示例

      ```C
      #include <stdio.h>
      #include <stdlib.h>
      
      void printMap(char map[6][6],int row,int col);
      char getDirection(char ch);
      char lowercase(char ch);
      void moveMan(char ch,char map[6][6]);
      
      
      int startRow = 1;
      int startCol = 1;
      
      int endRow = 1;
      int endCol = 5;
      
      int main()
      {
          //定义二维数组存放地图
          char map[6][6] = {
                  {'#','#','#','#','#','#'},
                  {'#','R',' ','#',' ',' '},
                  {'#',' ','#','#',' ','#'},
                  {'#',' ',' ','#',' ','#'},
                  {'#','#',' ',' ',' ','#'},
                  {'#','#','#','#','#','#'}
          };
      
          //在企业开发中尽量用表达式代替数字
          int row = sizeof(map)/sizeof(map[1]);
          int col = sizeof(map[1]);
      
          do{
              //打印地图
              printMap(map,row,col);
      
              //获取小人运动方向
              char ch = getDirection(ch);
      
              //移动小人
              moveMan(ch,map);
      
              //打印地图
              printMap(map,row,col);
      
              //结束
              if(startRow == endRow && startCol == endCol)
              {
                  break;
              }
          }while(1);
      
          //输出结束语
          printf("恭喜你走出迷宫\n");
      
          return 0;
      }
      
      /**
       * @param printMap 封装打印地图函数
       * @param map 地图
       * @param row 二维数组行数
       * @param col 二维数组列数
       * @return
       */
      void printMap(char map[6][6],int row,int col)
      {
          //清屏
          system("cls");
      
          for(int i = 0;i < row;i++)
          {
              for (int j = 0; j < col; j++)
              {
                  printf("%c", map[i][j]);
              }
              printf("\n");
          }
      }
      
      /**
       * @param getDirection 获取小人运动方向
       * @param ch 用户传入数据（小人运动方向）
       * @return
       */
      char getDirection(char ch)
      {
          //提示用户输入
          printf("请输入w、a、s、d中的其一控制小人移动方向\n");
      
          //获取输入
          scanf("%c",&ch);
      
          //清空缓冲区
          //如果不清空缓冲区的话会出现bug，解释见下
          //不过清空缓冲区可能会造成运行程序卡顿，为解决卡顿可以省略，上面的清屏指令可以覆盖该bug
          setbuf(stdin,NULL);
      
          //转换字母（将用户输入的数据统一为小写字母）
          ch = lowercase(ch);
      
          return ch;
      }
      
      /**
       * lowercase 转换字母
       * @param ch 待转换数据
       * @return
       */
      char lowercase(char ch)
      {
          if(ch >= 'A' && ch <= 'Z')
          {
              return ch + ('a'-'A');
          }
      
          return ch;
      }
      
      /**
       * @param moveMan 移动小人
       * @param ch 小人移动方向
       * @param map 地图
       */
      void moveMan(char ch,char map[6][6])
      {
          switch (ch) {
              //向上走
              case 'w':
                  if (map[startRow - 1][startCol] != '#') {
                      //清空当前位置数据源
                      map[startRow][startCol] = ' ';
                      //移动小人
                      map[startRow - 1][startCol] = 'R';
                      //修改小人位置
                      startRow = startRow - 1;
                  }
                  break;
                  //向下走
              case 's':
                  if (map[startRow + 1][startCol] != '#') {
                      //清空当前位置数据源
                      map[startRow][startCol] = ' ';
                      //移动小人
                      map[startRow + 1][startCol] = 'R';
                      //修改小人位置
                      startRow = startRow + 1;
                  }
                  break;
                  //向左走
              case 'a':
                  if (map[startRow][startCol - 1] != '#') {
                      //清空当前位置数据源
                      map[startRow][startCol] = ' ';
                      //移动小人
                      map[startRow][startCol - 1] = 'R';
                      //修改小人位置
                      startCol = startCol - 1;
                  }
                  break;
                  //向右走
              case 'd':
                  if (map[startRow][startCol + 1] != '#') {
                      //清空当前位置数据源
                      map[startRow][startCol] = ' ';
                      //移动小人
                      map[startRow][startCol + 1] = 'R';
                      //修改小人位置
                      startCol = startCol + 1;
                  }
                  break;
              default:
                  printf("没有此方向");
          }
      }
      ```

4. bug解释

   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\迷宫小游戏bug.png)

   ​       在前面讲scanf原理的时候说过，scanf在运行的时候会将输入的数据现存入缓冲区，这里输入了s然后回车，s被使用之后，还有一个回车被使用，就出现了这部分bug，解决此问题的方法就是清空缓冲区。但是，慎用清空缓冲区，因为可能会造成卡顿。

# 字符串

1. 字符串：字符串是使用空字符`\0`结尾的一堆字符数组。

2. 空字符：空字符（Null character）又称结束符，缩写 **NUL**，是一个数值为 **0** 的控制字符，**\0** 是转义字符，意思是告诉编译器，这不是字符 **0**，而是空字符。

3. 初始化字符串

   C语言当中没有专门的字符串变量，因而通常使用字符数组存储字符串。

   ```c
   char str1[10] = "string"; //系统会自动在尾部添加上结束标志  \0
   char str2[10] = {'H','e','l','l','o'}; //系统不会自动在尾部添加上结束标志
   
   //这两种写法等效，str3和str4中的\0和0都是字符数组元素的一部分，所以元素个数应加上其
   char str3[10] = {'H','e','l','l','o','\0'};
   char str4[10] = {'H','e','l','l','o',0};
   
   //如果省略数组元素个数，下面这种写法就只是一个字符数组，不是字符串
   char str5[] = {'H','e','l','l','o'};
   
   //如果不省略数组元素个数，下面这种写法也可看作字符串
   char str6[10] = {'H','e','l','l','o'};
   
   //当字符数组长度大于实际存储字符数量时，未被初始化的部分默认是0
   ```

   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\初始化字符串01.png)

4. 输出与输出

   1. 输出

      字符串的输出可以使用for循环一个一个的输出，但是这样比较麻烦。对于字符串的输出，直接使用格式化字符串`%s`即可。

      ```c
      char str[10] = "Hello";
      
      printf("%s\n",str);
      ```

   2. 输入

      ```c
      char str[10];
      
      scanf("%s",str);//输入string
      
      printf("%s\n",str);//输出string
      ```

      就目前学到的知识而言，int、char、float 等类型的变量用于`scanf()`时都要在前面添加`&`，而**数组或者字符串用于`scanf()`时**

      **不用添加`&`**，它们本身就会转换为地址。读者一定要谨记这一点。

   3. 注意点

      1. 对一个字符串数组, 如果不做初始化赋值, 必须指定数组长度。

      2. 一个字符数组只能存储其对应的数组长度 - 1个字符组成的字符串，比如说数组长度为10的字符数组，其能存储的字符串的字符数最大为9，如果存储10位字符组成的字符串就会出现错误（因为结束标志的位置被占用，没有结束标志）。

         ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\字符串输出.png)

      3. 当用scanf函数输入字符串时,字符串中不能含有空格,否则将以空格作为串的结束符。

5. 字符串处理函数

   1. 字符串输出函数

      1. 格式：`puts(字符数组名);`

      2. 所在头文件：`stdio.h`

      3. 优点：自动换行、可以是数组元素的任意地址

      4. 缺点：不能自定义输出格式

         ```c
         puts(Hello %i);
         ```

      5. 示例

         ```c
         #include <stdio.h>
         
         int main()
         {
             char str[10] = "string";
         
             puts(str);
         
             return 0;
         }
         ```

         ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\puts.png)

   2. 字符串输入函数

      1. 格式：`gets(字符数组名);`

      2. 所在头文件：`stdio.h`

      3. 示例

         ```c
         #include <stdio.h>
         
         int main()
         {
             char str[10];
         
             gets(str);
         
             puts(str);
         
             return 0;
         }
         ```

         ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\gets01.png)

      4. 注意

         1. gets函数不以空格作为字符串输入的结束标志，而以回车作为字符串输入的结束标志。

         2. gets函数是不安全，其很容易造成数组下标越界，因此不是很推荐使用。

            ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\gets02.png)

   3. 字符串长度

      1. sizeof

         sizeof是计算变量、数组占用的内存，字符数组中的字符一个字符占用一字节，所以也就可以使用sizeof来计算字符串的长度。

         1. 格式：`sizeof(字符数组名);`

         2. 示例

            ```c
            #include <stdio.h>
            
            int main()
            {
                //此处字符数组不能填写数组长度，不然计算出来的结果就是字符数组的长度，而不是字符串的长度
            	char str[] = "string";
                
                int length = sizeof(str);
                
                printf("str的长度为：%d\n",length);//7，原因：计算结果包含结束标志
                
                return 0;
            }
            ```

      2. strlen函数

         1. 格式：`strlen(字符数组名);`

         2. 功能：计算字符串中字符个数，其在计算时不包含结束标志`\0`

         3. 所在头文件：`string.h`

         4. 示例

            ```c
            #include <stdio.h>
            #include <string.h>
            
            int main()
            {
                char str1[10] = "string";
                int length1 = strlen(str1);
                
                char str2[] = "string";
                int length2 = strlen(str2);
                
                char str3[] = {'s','t','r','i','n','g','\0'};
                int length3 = strlen(str3);
                
                char str4[] = {'s','t','r','i','n','g'};
                int length4 = strlen(str4);
                
                printf("str1的长度为：%d\n",length1);//6
                printf("str2的长度为：%d\n",length2);//6
                printf("str3的长度为：%d\n",length3);//6
                printf("str4的长度为：%d\n",length4);//随机值，因为没有结束标志
                
                return 0;
            }
            ```

            ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\strlen.png)

   4. 字符串连接函数

      1. 格式：`strcat(字符数组名1，字符数组名2);`

      2. 功能：把字符数组2中的字符串连接到字符数组1 中字符串的后面,并删去字符串1后的串标志`\0`。本函数返回值是字符数组1的首地址。

      3. 所在头文件：`string.h`

      4. 示例

         ```c
         #include <stdio.h>
         #include <string.h>
         
         int main()
         {
             char str1[] = "Hello,";
         
             char str2[] = "World!";
             
             strcat(str1,str2);
         
             puts(str1);
         
             return 0;
         }
         ```

         ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\strcat.png)

      5. 注意

         本程序把初始化赋值的字符数组与动态赋值的字符串连接起来。要注意的是,字符数组1应定义足够的长度,否则不能全部装入被连接的字符串。哪怕是说编译器放过了你，但实际上这样是错误的。

         ```c
         //正确
         char str1[20] = "Hello,";
         char str2[10] = ",World!";
         
         strcat(str1,str2);
         
         puts(str1);
         
         //错误
         char str1[10] = "Hello,";
         char str2[10] = ",World!";
         
         strcat(str1,str2);
         
         puts(str1);
         ```

         ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\strcat注意.png)

   5. 字符串拷贝函数

      1. 格式：`strcpy(字符数组名1，字符数组名2);`

      2. 功能：把字符数组2中的字符串拷贝到字符数组1中，拷贝的时候字符串结束标志`\0`也一同拷贝。字符数组名2的位置也可以是一个字符串常量，这样就代表把一个字符串赋给一个字符数组。

      3. 所在头文件：`string.h`

      4. 示例

         ```c
         #include <stdio.h>
         #include <string.h>
         
         int main()
         {
             char str1[10] = "string";
         
             char str2[5] = "Word";
         
             strcpy(str1,str2);//str1中原先的字符串被覆盖
         
             puts(str1);//word
         
             return 0;
         }
         ```

         ```c
         #include <stdio.h>
         #include <string.h>
         
         int main()
         {
             char str1[10] = "string";
         
             strcpy(str1,"word");//str1中原先的字符串被覆盖
         
             puts(str1);//word
         
             return 0;
         }
         ```

      5. 注意

         和strcat函数一样，字符数组1的数组长度必须足够装下字符数组2的字符串。

   6. 字符串比较函数

      1. 格式：`strcmp(字符数组名1，字符数组名2);`

      2. 功能：按照ASCII码，顺序比较两个数组中的字符串，并由函数返回值返回比较结果。

      3. 比较规则

         1. 字符串1 = 字符串2 ， 返回值 = 0
         2. 字符串1 < 字符串2 ， 返回值 < 0
         3. 字符串1 > 字符串2 ， 返回值 > 0

      4. 所在头文件：`string.h`

      5. 示例

         ```c
         #include <stdio.h>
         #include <string.h>
         
         int main()
         {
             char str1[10] = "0";
             char str2[10] = "1";
             printf("%d\n", strcmp(str1, str2));//-1
         
             char str3[10] = "1";
             char str4[10] = "1";
             printf("%d\n", strcmp(str3, str4));//0
         
             char str5[10] = "1";
             char str6[10] = "0";
             printf("%d\n", strcmp(str5, str6));//1
         
             return 0;
         }
         ```

6. 字符串数组

   1. 字符串数组：保存字符串的数组。一维数组可以保存一个字符串，二维数组可以保存两个字符串。

   2. 示例

      ```c
      //一维数组
      char str1[10] = "string";
      
      //二维数组
      char str2[2][10] = {{'H','e','l','l','o','\0'},{'W','o','r','l','d','\0'}};
      char str3[2][10] = {"Hello","World"};
      ```

# 指针

1. 变量地址：系统分配给“变量”的“内存单元”的起始地址。
2. 指针：在计算机中所有数据都存储在内存单元中,而每个内存单元都有一个对应的地址, 只要通过这个地址就能找到对应单元中存储的数据。由于通过地址能找到所需的变量单元，所以我们说该地址指向了该变量单元。将地址形象化的称为“指针”。
3. 内存单元的指针是地址，而内存单元里的内容是实际数据。

## 指针变量

1. 指针变量：用来存放变量地址的变量。指针变量里面存放的是另外一个变量的地址，其指向另外一个变量。比如说指针变量`a`里面存放的是变量`c`的地址，那么指针变量`a`就指向变量`c`。

2. 格式：`指针的指向数据类型 * 指针变量名称;`

   *：指针运算符，用来获取某个地址上的数据。

   ```c
   #include <stdio.h>
   
   int main()
   {
       int a = 15;
       int *p = &a;
       printf("%d, %d\n", a, *p);  //两种方式都可以输出a的值
       
       return 0;
   }
   ```

   假设一个指针变量`*pa`，其指向变量`a`，其中的pa的值是变量`a`的地址，而`*pa`则代表的是变量`a`的值。

3. 示例

   ```c
   char ch = 'a';
   char *pch;//定义指针变量
   pch = &ch;
   
   int num = 10;
   int *pnum;//定义指针变量
   pnum = &num;
   ```

4. 注意

   1. 指针变量也可以连续定义

      ```c
      int *a, *b, *c;  //a、b、c 的类型都是 int*
      ```

   2. 每个指针变量前面都要带`*`。如果写成下面的形式，那么只有 a 是指针变量，b、c 都是类型为 int 的普通变量。

      ```c
      int *a, b, c;
      ```

   3. 假设有一个 int 类型的变量 a，pa 是指向它的指针，那么`*&a`和`&*pa`分别是什么意思呢？
      1. `*&a`可以理解为`*(&a)`，`&a`表示取变量 a 的地址（等价于 pa），`*(&a)`表示取这个地址上的数据（等价于 *pa），绕来绕去，又回到了原点，`*&a`仍然等价于 a。
      2. `&*pa`可以理解为`&(*pa)`，`*pa`表示取得 pa 指向的数据（等价于 a），`&(*pa)`表示数据的地址（等价于 &a），所以`&*pa`等价于 pa。

5. 初始化

   1. 定义的同时初始化

      ```c
      int a = 5;
      int *p = &a;
      ```

   2. 先定义后初始化

      ```c
      int a = 5;
      int *p;
      p = &a;//不需要加 * ，因为编译器已经知道这是一个指针变量，加上的话就会报错
      ```

   3. 把指针初始化为NULL（空指针）

      ```c
      int *p = NULL;
      int *q = 0;
      ```

   4. 不合法初始化

      1. 指针变量只能存储地址, 不能存储其它类型

         ```c
         int a = 10;
         int * p;
         p = 250;//错误
         ```

      2. 给指针变量赋值时,指针变量前不能再加`*`

         ```c
         int a = 10;
         int * p;
         * p = &a;//错误
         ```

   5. 注意点

      1. 多个指针变量可以指向同一个地址

         ```c
         int a = 10;
         int *p = &a;
         int *q = &a;
         ```

      2. 指针的指向可以改变

         ```c
         int a = 10;
         int *p = &a;
         int b = 15;
         p = &b;//修改指针指向
         ```

      3. 指针没有初始化里面是一个垃圾值,这时候我们这是一个野指针

         野指针可能会导致程序崩溃，野指针会访问你不该访问的数据。
      
      4. 对于暂时没有指向的指针，建议赋值`NULL`

6. 访问指针所指向的存储空间

   ```c
   #include <stdio.h>
   
   int main()
   {
       int num = 10;
   
       int *pnum = &num;
   
       printf("%d\n",*pnum);//10
   
       return 0;
   }
   ```

7. 指针变量占用内存

   **在64位架构计算机当中**（如今的电脑多数（可以说是全部）都是64位架构），**指针变量的占用内存都是8字节**，不管是什么类型的还是说几级指针，都是8字节。

   ```c
   #include <stdio.h>
   
   int main()
   {
       //一级指针
       int num = 20;
       int *pnum = &num;
       printf("*pnum占用的内存为：%d\n",sizeof(pnum));
   
       char str = 'a';
       char *pstr = &str;
       printf("*pstr占用的内存为：%d\n",sizeof(pstr));
   
       float num_fl = 3.14;
       float *pnum_fl = &num_fl;
       printf("*pnum_fl占用的内存为：%d\n",sizeof(pnum_fl));
   
       double num_db = 3.14159;
       double *pnum_db = &num_db;
       printf("*pnum_db占用的内存为：%d\n",sizeof(pnum_db));
   
       //二级指针
       int **number = &pnum;
       printf("**number占用的内存为：%d\n",sizeof(number));
   
       char **string = &pstr;
       printf("**string占用的内存为：%d\n",sizeof(string));
   
       float **p_num_fl = &pnum_fl;
       printf("**p_num_fl占用的内存为：%d\n",sizeof(p_num_fl));
   
       double **p_num_db = &pnum_db;
       printf("**p_num_db占用的内存为：%d\n",sizeof(p_num_db));
   
       return 0;
   }
   ```

   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\指针变量占用内存.png)

8. 练习

   1. 编写一个函数改变数字的值（形参改变实参）

      ```c
      #include <stdio.h>
      
      void change_num(int *num);
      
      int main()
      {
          int num = 10;
      
          printf("%d\n",num);//10
      
          change_num(&num);
      
          printf("%d\n",num);//15
      
          return 0;
      }
      
      //将函数的形参改性指针变量，这样，就能实现形参改变实参
      void change_num(int *num)
      {
          *num = 15;//修改指针内容的时候需要加上*
      }
      ```

   2. 定义一个函数交换两个变量的值（这样写纯属蛋疼）

      ```c
      #include <stdio.h>
      
      int main()
      {
          int a = 100, b = 999, temp;
          int *pa = &a, *pb = &b;
          printf("a=%d, b=%d\n", a, b);
          /*****开始交换*****/
          temp = *pa;  //将a的值先保存起来
          *pa = *pb;  //将b的值交给a
          *pb = temp;  //再将保存起来的a的值交给b
          /*****结束交换*****/
          printf("a=%d, b=%d\n", a, b);
          
          return 0;
      }
      ```

## 指针变量的运算

1. 指针变量保存的是地址，而地址本质上是一个整数，所以指针变量可以进行部分运算，例如加法、减法、比较等。

2. 示例

   ```c
   #include <stdio.h>
   
   int main()
   {
       int a = 10, *pa = &a, *paa = &a;
       
       double b = 99.9, *pb = &b;
       
       char c = '@',*pc = &c;
       
       //最初的值
       printf("&a=%#X, &b=%#X, &c=%#X\n", &a, &b, &c);
       printf("pa=%#X, pb=%#X, pc=%#X\n", pa, pb, pc);
       
       //加法运算
       pa++; pb++; pc++;
       printf("pa=%#X, pb=%#X, pc=%#X\n", pa, pb, pc);
       
       //减法运算
       pa -= 2; pb -= 2; pc -= 2;
       printf("pa=%#X, pb=%#X, pc=%#X\n", pa, pb, pc);
       
       //比较运算
       if(pa == paa)
       {
           printf("%d\n", *paa);
       }
       else
       {
           printf("%d\n", *pa);
       }
       
       return 0;
   }
   ```

   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\指针变量的运算01.png)

3. 解释

   ​       从运算结果可以看出：pa、pb、pc 每次加 1，它们的地址分别增加 4、8、1，正好是 int、double、char 类型的长度；减 2 

   时，地址分别减少 8、16、2，正好是 int、double、char 类型长度的 2 倍。

   ​       这很奇怪，指针变量加减运算的结果跟数据类型的长度有关，而不是简单地加 1 或减 1，这是为什么呢？

   ​	以 a 和 pa 为例，a 的类型为 int，占用 4 个字节，pa 是指向 a 的指针，如下图所示：

   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\指针变量的运算02.jpg)

   ​	刚开始的时候，pa 指向 a 的开头，通过 *pa 读取数据时，从 pa 指向的位置向后移动 4 个字节，把这 4 个字节的内容作为要获

   取的数据，这 4 个字节也正好是变量 a 占用的内存。

   ​	如果`pa++;`使得地址加 1 的话，就会变成如下图所示的指向关系：

   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\指针变量的运算03.jpg)

   ​	这个时候 pa 指向整数 a 的中间，*pa 使用的是红色虚线画出的 4 个字节，其中前 3 个是变量 a 的，后面 1 个是其它数据的，把

   它们“搅和”在一起显然没有实际的意义，取得的数据也会非常怪异。

   ​	如果`pa++;`使得地址加 4 的话，正好能够完全跳过整数 a，指向它后面的内存，如下图所示：

   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\指针变量的运算04.jpg)

4. 注意

   1. 当对指针变量进行比较运算时，比较的是指针变量本身的值，也就是数据的地址。如果地址相等，那么两个指针就指向同一份数据，否则就指向不同的数据。上面的代码（第一个例子）在比较 pa 和 paa 的值时，pa 已经指向了 a 的上一份数据，所以它们不相等。而 a 的上一份数据又不知道是什么，所以会导致 printf() 输出一个没有意义的数，这正好印证了上面的观点，不要对指向普通变量的指针进行加减运算。

   2. 不要尝试通过指针获取下一个变量的地址

      ​      C语言并没有规定变量的存储方式，如果连续定义多个变量，它们有可能是挨着的，也有可能是分散的，这取决于变量的类型、编译器的实现以及具体的编译模式，所以对于指向普通变量的指针，我们往往不进行加减运算，虽然编译器并不会报错，但这样做没有意义，因为不知道它后面指向的是什么数据。

      ```c
      #include <stdio.h>
      
      int main()
      {
          int a = 1, b = 2, c = 3;
          int *p = &c;
          int i;
          for(i=0; i<8; i++)
          {
              printf("%d, ", *(p+i) );
          }
          
          return 0;
      }
      ```
      
   
   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\指针变量的运算05.png)
   
   可以发现，变量 a、b、c 并不挨着，它们中间还参杂了别的辅助数据。
   
3. 不能对指针变量进行乘法、除法、取余等其他运算，除了会发生语法错误，也没有实际的含义。

## 数组指针

1. 数组指针：如果一个指针指向了数组，我们就称它为数组指针（Array Pointer）。

2. 以指针的方式遍历数组（元素地址法）

   ```c
   #include <stdio.h>
   
   int main()
   {
       int arr[] = { 99, 15, 100, 888, 252 };
       int len = sizeof(arr) / sizeof(int);  //求数组长度
       int i;
       for(i=0; i<len; i++)
       {
           printf("%d  ", *(arr+i) );  //*(arr+i)等价于arr[i]
       }
       printf("\n");
       return 0;
   }
   ```

3. 解释

   ​       `*(arr+i)`这个表达式，arr 是数组名，指向数组的第 0 个元素，表示数组首地址， arr+i 指向数组的第 i 个元素，*(arr+i) 表示取

   第 i 个元素的数据，它等价于 arr[i]。

   ​	`arr`是`int*`类型的指针，指针也就是地址，地址本质上就是数字，`arr`每次加 1 时它自身的值会增加 `sizeof(int)`，加 i 时自

   身的值会增加`sizeof(int) * i`。

   ​	定义一个指向数组的指针，如：

   ```c
   int nums[] = {12,56,15,48,64};
   int *p = nums;
   ```

   ​	`nums`本身可以看作一个指针（指向数组的第0个元素），可以直接赋值给指针变量 p。`nums`是数组第 0 个元素的地址，所以

   `int *p = nums;`也可以写作`int *p = &nums[0];`。也就是说，`nums`、`p`、`&nums[0]`这三种写法都是等价的，它们都指向数组第

    0 个元素，或者说指向数组的开头。

   ​	但是需说明的是，`nums`本身可以看作指针，这种说法不是很严谨，应该说是`nums`被转换成了一个指针。指针和数组是不等价

   的，但是在大多数情况下数组会转换成指针。

   ​	数组指针指向的是数组中的一个具体元素，而不是整个数组，所以数组指针的类型和数组元素的类型有关。

   ​	更改上面的示例代码：（指针变量法）

   ```C
   #include <stdio.h>
   
   int main()
   {
       int arr[] = { 99, 15, 100, 888, 252 };
       int i, *p = arr, len = sizeof(arr) / sizeof(int);
   
       for(i=0; i<len; i++)
       {
           printf("%d  ", *(p+i) );//此处的*（p + i）也可以替换成*p++
       }
       printf("\n");
       return 0;
   }
   ```

   ​	数组在内存中只是数组元素的简单排列，没有开始和结束标志，在求数组的长度时不能使用`sizeof(p) / sizeof(int)`，因为 

   `p`只是一个指向`int`类型的指针，编译器并不知道它指向的到底是一个整数还是一系列整数（数组），所以`sizeof(p)`求得的是`p`这

   个指针变量本身所占用的字节数，而不是整个数组占用的字节数。

   ​	也就是说，根据数组指针不能逆推出整个数组元素的个数，以及数组从哪里开始、到哪里结束等信息。不像字符串，数组本身也

   没有特定的结束标志，如果不知道数组的长度，那么就无法遍历整个数组。

4. 注意

   假设 p 是指向数组 arr 中第 n 个元素的指针，那么 `p++`、`++p`、`(*p)++` 分别是什么意思呢？

   1. `*p++`等价于`*(p++)`，表示先取得第 n 个元素的值，再将 p 指向下一个元素。
   2. `*++p`等价于`*(++p)`，会先进行`++p`运算，使得 p 的值增加，指向下一个元素，整体上相当于`*(p+1)`，所以会获得第 n+1 个数组元素的值。
   3. `(*p)++`会先取得第 n 个元素的值，再对该元素的值加 1。假设 p 指向第 0  个元素，并且第 0 个元素的值为 99，执行完该语句后，第 0  个元素的值就会变为 100。

## 字符串指针

1. 字符串指针：如果一个指针指向了字符串，那么我们就称它为字符串指针。

2. 字符串存储在字符数组中，字符数组也是数组，所以前面说过的指针和数组的规则对字符数组一样适用。

   ```c
   #include <stdio.h>
   #include <string.h>
   
   int main()
   {
       char str[] = "string";
       char *pstr = str;
       int len = strlen(str), i;
   
       //使用*(pstr+i)
       for(i=0; i<len; i++)
       {
           printf("%c", *(pstr+i));
       }
       printf("\n");
       //使用pstr[i]
       for(i=0; i<len; i++)
       {
           printf("%c", pstr[i]);
       }
       printf("\n");
       //使用*(str+i)
       for(i=0; i<len; i++)
       {
           printf("%c", *(str+i));
       }
       printf("\n");
   
       return 0;
   }
   ```

   除了字符数组，C语言还支持另外一种表示字符串的方法，就是直接使用一个指针指向字符串，例如：

   ```c
   char *str = "string";
   
   char *str;
   str = "string";
   ```

   ​	字符串中的所有字符在内存中是连续排列的，str 指向的是字符串的第 0 个字符；我们通常将第 0  个字符的地址称为字符串的首

   地址。字符串中每个字符的类型都是`char`，所以 str 的类型也必须是`char *`。

   ```c
   #include <stdio.h>
   #include <string.h>
   
   int main(){
       char *str = "string";
       int len = strlen(str), i;
      
       //直接输出字符串
       printf("%s\n", str);
       //使用*(str+i)
       for(i=0; i<len; i++)
       {
           printf("%c", *(str+i));
       }
       printf("\n");
       //使用str[i]
       for(i=0; i<len; i++)
       {
           printf("%c", str[i]);
       }
       printf("\n");
   
       return 0;
   }
   ```

3. 字符数组与字符串常量的区别

   ​	**这一切看起来和字符数组是多么地相似，它们都可以使用`%s`输出整个字符串，都可以使用`*`或`[ ]`获取单个字符，这两种表示字符串的方式是不是就没有区别了呢？**

   ​	有！它们最根本的区别是在内存中的存储区域不一样，字符数组存储在全局数据区或栈区，第二种形式的字符串存储在常量区。

   全局数据区和栈区的字符串（也包括其他数据）有读取和写入的权限，而常量区的字符串（也包括其他数据）只有读取权限，没有写

   入权限。

   ​	内存权限的不同导致的一个明显结果就是，字符数组在定义后可以读取和修改每个字符，而对于第二种形式的字符串，一旦被定

   义后就只能读取不能修改，任何对它的赋值都是错误的。

   ```c
   #include <stdio.h>
   
   int main()
   {
       char *str = "Hello World!";
       str = "I love C!";  //正确
       str[3] = 'P';  //错误
   
       return 0;
   }
   ```

   ​	这段代码能够正常编译和链接，但在运行时会出现段错误（Segment Fault）或者写入位置错误。

   ​	第6行代码是正确的，可以更改指针变量本身的指向；第7行代码是错误的，不能修改字符串中的字符。

   ​	**那么到底使用字符数组还是字符串常量？**

   ​	在编程过程中如果只涉及到对字符串的读取，那么字符数组和字符串常量都能够满足要求；如果有写入（修改）操作，那么只能

   使用字符数组，不能使用字符串常量。

   ​	获取用户输入的字符串就是一个典型的写入操作，只能使用字符数组，不能使用字符串常量，请看下面的代码：

   ```c
   #include <stdio.h>
   
   int main()
   {
       char str[30];
       gets(str);
       printf("%s\n", str);
   
       return 0;
   }
   ```

## 指针与函数

1. 指针变量作为函数参数

   ​	在C语言中，函数的参数不仅可以是整数、小数、字符等具体的数据，还可以是指向它们的指针。用指针变量作函数参数可以将

   函数外部的地址传递到函数内部，使得在函数内部可以操作函数外部的数据，并且这些数据不会随着函数的结束而被销毁。

   ​	像数组、字符串、动态分配的内存等都是一系列数据的集合，没有办法通过一个参数全部传入函数内部，只能传递它们的指针，

   在函数内部通过指针来影响这些数据集合。有的时候，对于整数、小数、字符等基本类型数据的操作也必须要借助指针，一个典型的

   例子就是交换两个变量的值。

   ```c
   #include <stdio.h>
   
   void swap(int a, int b)
   {
       int temp;  //临时变量
       temp = a;
       a = b;
       b = temp;
   }
   
   int main()
   {
       int a = 66, b = 99;
       swap(a, b);
       printf("a = %d, b = %d\n", a, b);
       
       return 0;
   }
   ```

   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\指针变量作为函数的形参01.png)

   ​	从结果可以看出，a、b 的值并没有发生改变，交换失败。这是因为`swap()`函数内部的 a、b 和`main()`函数内部的 a、b 是不同

   的变量，占用不同的内存，它们除了名字一样，没有其他任何关系，swap() 交换的是它内部 a、b 的值，不会影响它外部（`main()`

   内部） a、b 的值。

   ```c
   #include <stdio.h>
   
   void swap(int *p1, int *p2)
   {
       int temp;  //临时变量
       temp = *p1;
       *p1 = *p2;
       *p2 = temp;
   }
   
   int main(){
       int a = 66, b = 99;
       swap(&a, &b);
       printf("a = %d, b = %d\n", a, b);
       
       return 0;
   }
   ```

   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\指针变量作为函数的形参02.png)

   ​	调用`swap()`函数时，将变量 a、b 的地址分别赋值给 p1、p2，这样 *p1、*p2 代表的就是变量 a、b 本身，交换 *p1、*p2 的值也就

   是交换 a、b 的值。函数运行结束后虽然会将 p1、p2 销毁，但它对外部 a、b 造成的影响是“持久化”的，不会随着函数的结束而“恢复

   原样”。

   ```c
   #include <stdio.h>
   
   int max(int *intArr, int len)
   {
       int maxValue = intArr[0];  //假设第0个元素是最大值
       for(int i=1; i<len; i++)
       {
           if(maxValue < intArr[i])
           {
               maxValue = intArr[i];
           }
       }
      
       return maxValue;
   }
   
   int main()
   {
       int nums[6];
       int len = sizeof(nums)/sizeof(int);
       //读取用户输入的数据并赋值给数组元素
       for(int i=0; i<len; i++)
       {
           scanf("%d", nums+i);
       }
       printf("Max value is %d!\n", max(nums, len));
   
       return 0;
   }
   ```

   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\指针变量作为函数的形参03.png)

   ​	参数 intArr 仅仅是一个数组指针，在函数内部无法通过这个指针获得数组长度，必须将数组长度作为函数参数传递到函数内部。

   数组 nums 的每个元素都是整数，scanf() 在读取用户输入的整数时，要求给出存储它的内存的地址，`nums+i`就是第 i 个数组元素的

   地址。

   ​	用数组做函数参数时，参数也能够以“真正”的数组形式给出。例如对于上面的 max() 函数，它的参数可以写成下面的形式：

   ```c
   int max(int intArr[6], int len)//也可以省略长度写为int intArr[]
   {
       int i, maxValue = intArr[0];  //假设第0个元素是最大值
       for(i=1; i<len; i++)
       {
           if(maxValue < intArr[i])
           {
               maxValue = intArr[i];
           }
       }
       return maxValue;
   }
   ```

   ​	`int intArr[6]`好像定义了一个拥有 6 个元素的数组，调用 max() 时可以将数组的所有元素“一股脑”传递进来。实际上这两种形

   式的数组定义都是假象，不管是`int intArr[6]`还是`int intArr[]`都不会创建一个数组出来，编译器也不会为它们分配内存，实际

   的数组是不存在的，它们最终还是会转换为`int *intArr`这样的指针。这就意味着，两种形式都不能将数组的所有元素“一股脑”传递

   进来，大家还得规规矩矩使用数组指针。

   ​	`int intArr[6]`这种形式只能说明函数期望用户传递的数组有 6 个元素，并不意味着数组只能有 6 个元素，真正传递的数组可

   以有少于或多于 6 个的元素。不管使用哪种方式传递数组，都不能在函数内部求得数组长度，因为`intArr`仅仅是一个指针，而不是

   真正的数组，所以必须要额外增加一个参数来传递数组长度。

   ​	**C语言为什么不允许直接传递数组的所有元素，而必须传递数组指针呢？**

   ​	参数的传递本质上是一次赋值的过程，赋值就是对内存进行拷贝。所谓内存拷贝，是指将一块内存上的数据复制到另一块内存

   上。对于像 int、float、char 等基本类型的数据，它们占用的内存往往只有几个字节，对它们进行内存拷贝非常快速。而数组是一系

   列数据的集合，数据的数量没有限制，可能很少，也可能成千上万，对它们进行内存拷贝有可能是一个漫长的过程，会严重拖慢程序

   的效率，为了防止技艺不佳的程序员写出低效的代码，C语言没有从语法上支持数据集合的直接赋值。

2. 指针变量作为函数返回值

   1. 指针函数：如果一个函数的返回值是一个指针（地址），那我们称这个函数为指针函数。

   2. 示例

      ```c
      #include <stdio.h>
      #include <string.h>
      
      char *strlong(char *str1, char *str2);
      
      int main(){
          char str1[30], str2[30], *str;
          gets(str1);
          gets(str2);
          str = strlong(str1, str2);
          printf("Longer string: %s\n", str);
      
          return 0;
      }
      
      char *strlong(char *str1, char *str2)
      {
          if(strlen(str1) >= strlen(str2))
          {
              return str1;//str1为数组，其被转换成指针，无需加*
          }
          else
          {
              return str2;//str2为数组，其被转换成指针，无需加*
          }
      }
      ```

      ```c
      #include <stdio.h>
      #include <stdlib.h>
      
      int fun(char *s,int *t);
      
      int main()
      {
          char str[256] = {0};
          gets(str);
          int t = 0;
          printf("%d",fun(str,&t));
      
          system("pause");
          return 0;
      }
      
      int fun(char *s,int *t)
      {
          char c = '#';
          int i = 0;
          if(s != NULL)
          {
              for(i = 0;s[i] != '\0';i++)
              {
                  if(s[i] == c)
                  {
                      (*t)++;
                  }
              }
          }
      
          return *t;//返回值是普通变量，需要加上*
      }
      ```

      ```c
      #include <stdio.h>
      #include <stdlib.h>
      
      char fun(char *p);
      
      int main()
      {
          char ch = 's';
          char *p = &ch;
      
          fun(&ch);
      
          printf("%c\n",*p);
      
          system("pause");
          return 0;
      }
      
      char fun(char *p)
      {
          char a = 'w';
          *p = a;//改变指针变量的值需加上*
          return *p;//返回值是普通变量，需要加上*
      }
      ```

   3. 注意

      ​	函数运行结束后会销毁在它内部定义的所有局部数据，包括局部变量、局部数组和形式参数，函数返回的指针请尽量不要指

      向这些数据，C语言没有任何机制来保证这些数据会一直有效，它们在后续使用过程中可能会引发运行时错误。

      ```c
      #include <stdio.h>
      
      int *func()
      {
          int n = 100;
          return &n;
      }
      
      int main()
      {
          int *p = func(), n;
          n = *p;
          printf("value = %d\n", n);
          return 0;
      }
      ```

      ​	在比较老旧的编译器当中，会输出`value = 100`的结果，但是在现在的编译器中，编译器会直接报错，无法给出结果。

      ​	n 是`func()`内部的局部变量，`func()`返回了指向 n 的指针，根据上面的观点，`func()`运行结束后 n 将被销毁，使用 *p 

      应该获取不到 n 的值。但是从运行结果来看，我们的推理好像是错误的，`func()`运行结束后`*p`依然可以获取局部变量 n 的值，

      这个上面的观点不是相悖吗？那么看接下的这个例子。

      ```c
      #include <stdio.h>
      
      int *func()
      {
          int n = 100;
          return &n;
      }
      
      int main(){
          int *p = func(), n;
          printf("string\n");
          n = *p;
          printf("value = %d\n", n);
          return 0;
      }
      ```

      ​	在比较老旧的编译器中，会输出如下结果：

      ```c
      string
      value = -2
      ```

      ​	但是在如今的编译器中，编译器会直接报错，报错如下：

      ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\指针变量作为函数返回值注意01.png)

      ​	可以看到，程序直接报错了，与前面的代码相比，该段代码仅仅是在 *p 之前增加了一个函数调用，这一细节的不同却导致

      运行结果有天壤之别，究竟是为什么呢？

      ​	前面我们说函数运行结束后会销毁所有的局部数据，这个观点并没错。但是，这里所谓的销毁并不是将局部数据所占用的内

      存全部抹掉，而是程序放弃对它的使用权限，弃之不理，后面的代码可以随意使用这块内存。对于上面的两个例子，`func()`运

      行结束后`n`的内存依然保持原样，值还是 100，如果使用及时也能够得到正确的数据，如果有其它函数被调用就会覆盖这块内

      存，得到的数据就失去了意义。第一个例子在调用其他函数之前使用`*p`抢先获得了 n 的值并将它保存起来，第二个例子显然没

      有抓住机会，有其他函数被调用后才使用`*p`获取数据，这个时候已经晚了，内存已经被后来的函数覆盖了，而覆盖它的究竟是一

      份什么样的数据我们无从推断（一般是一个没有意义甚至有些怪异的值）。

## 二级指针

1. 二级指针：如果一个指针变量中存储的是另外一个指针变量的地址，则称这个指针变量为指向指针的指针变量，又名“二级指针”。

2. 示例

   ```c
   char ch = 'a';
   char *p = &ch;
   char **qp = &p;
   printf("%c\n",**qp);//a
   ```

3. 多级指针

   ```c
   #include <stdio.h>
   
   int main()
   {
       int a =100;
       int *p1 = &a;
       int **p2 = &p1;
       int ***p3 = &p2;
   
       printf("%d, %d, %d, %d\n", a, *p1, **p2, ***p3);
       printf("&p2 = %#X, p3 = %#X\n", &p2, p3);
       printf("&p1 = %#X, p2 = %#X, *p3 = %#X\n", &p1, p2, *p3);
       printf(" &a = %#X, p1 = %#X, *p2 = %#X, **p3 = %#X\n", &a, p1, *p2, **p3);
       return 0;
   }
   ```

   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\三级指针01.png)

   ​	以三级指针`***p3`为例分析上面的代码，`***p3`等价于`*(*(*p3))`。`*p3`得到的是`p2`的值，也就是`p1`的地址；`*(*p3)`得到的是`p1`的值，也就是`a`的地址；`*(*(*p3))`得到的是a的值。

   ​	假设 a、p1、p2、p3 的地址分别是 0X00A0、0X1000、0X2000、0X3000，它们之间的关系可以用下图来描述：

   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\三级指针02.jpg)

   ​	方框里面是变量本身的值，方框下面是变量的地址。

## 指针数组

1. 指针数组：如果一个数组中的所有元素保存的都是指针，那么我们就称它为指针数组。

2. 格式：`dataType *arrayName[length];`

   `[ ]`的优先级高于`*`，该定义形式应该理解为：

   ```c
   dataType *(arrayName[length]);
   ```

   括号里面说明`arrayName`是一个数组，包含了`length`个元素，括号外面说明每个元素的类型为`dataType *`。

3. 示例

   ```c
   int a = 16, b = 932, c = 100;
   int *arr[3] = {&a, &b, &c};
   ```

4. 注意

   1. 除了每个元素的数据类型不同，指针数组和普通数组在其他方面都是一样的

      ```c
      #include <stdio.h>
      
      int main()
      {
          int a = 16, b = 932, c = 100;
          //定义一个指针数组
          int *arr[3] = {&a, &b, &c};//也可以不指定长度，直接写作 int *arr[]
          //定义一个指向指针数组的指针
          int **parr = arr;
          printf("%d, %d, %d\n", *arr[0], *arr[1], *arr[2]);
          printf("%d, %d, %d\n", **(parr+0), **(parr+1), **(parr+2));
      
          return 0;
      }
      ```

      ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\指针数组01.png)

      ​	`parr`是指向数组`arr`的指针，确切地说是指向`arr`第 0 个元素的指针，它的定义形式应该理解为`int *(*parr)`，括号中的

      `*`表示`parr`是一个指针，括号外面的`int *`表示 parr 指向的数据的类型。arr 第 0 个元素的类型为 int *，所以在定义`parr`

      时要加两个 *。

      ​	第一个`printf()`语句中，`arr[i]`表示获取第 i 个元素的值，该元素是一个指针，还需要在前面增加一个 * 才能取得它指向

      的数据，也即`*arr[i]`的形式。

      ​	第二个`printf()`语句中，`parr+i`表示第 i 个元素的地址，`*(parr+i)`表示获取第 i 个元素的值（该元素是一个指针），

      `**(parr+i)`表示获取第 i 个元素指向的数据。

   2. 指针数组也可以和字符串数组结合使用

      ```c
      #include <stdio.h>
      
      int main()
      {
          char *str[3] = 
          {
              "Hello",
              "World",
              "I'm fine"
          };
          printf("%s\n%s\n%s\n", str[0], str[1], str[2]);
          
          return 0;
      }
      ```

      ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\指针数组02.png)

      ​	需要注意的是，**字符数组`str`中存放的是字符串的首地址，不是字符串本身，字符串本身位于其他的内存区域，和字符数组**

      **是分开的。**

      ​	**也只有当指针数组中每个元素的类型都是`char *`时，才能像上面那样给指针数组赋值，其他类型不行。**

      ​	为了便于理解，可以将上面的字符串数组改成下面的形式，它们都是等价的。

      ```c
      #include <stdio.h>
      
      int main()
      {
          char *str0 = "Hello";
          char *str1 = "World";
          char *str2 = "I'm fine";
          char *str[3] = {str0, str1, str2};
          printf("%s\n%s\n%s\n", str[0], str[1], str[2]);
          
          return 0;
      }
      ```

      ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\指针数组02.png)

## 二维数组指针

1. 二维数组指针：指向二维数组的指针。

2. 解释

   对于下面这个二维数组来说：

   ```c
   int a[3][4] = { 
       {0, 1, 2, 3}, 
       {4, 5, 6, 7}, 
       {8, 9, 10, 11} 
   };
   ```

   ​	C语言中的二维数组是按行排列的，也就是先存放`a[0]`行，再存放`a[1]`行，最后存放`a[2]`行；每行中的 4 个元素也是依次存

   放。数组`a`为`int`类型，每个元素占用 4 个字节，整个数组共占用`4×(3×4) = 48`个字节。

   ​	C语言允许把一个二维数组分解成多个一维数组来处理。对于数组 a，它可以分解成三个一维数组，即`a[0]`、`a[1]`、`a[2]`。每

   一个一维数组又包含了 4 个元素，例如 a[0] 包含`a[0][0]`、`a[0][1]`、`a[0][2]`、`a[0][3]`。

   ​	我们先来定义一个指向 a 的指针变量 p：

   ```c
   int (*p)[4] = a;
   ```

   ​	括号中的`*`表明`p`是一个指针，它指向一个数组，数组的类型为`int [4]`，这正是`a`所包含的每个一维数组的类型。

   ​	`[ ]`的优先级高于`*`，`( )`是必须要加的，如果赤裸裸地写作`int *p[4]`，那么应该理解为`int *(p[4])`，`p`就成了一个指针数

   组，而不是二维数组指针。

   ​	对指针进行加法（减法）运算时，它前进（后退）的步长与它指向的数据类型有关，p 指向的数据类型是`int [4]`，那么`p+1`就

   前进 4×4 = 16 个字节，`p-1`就后退 16 个字节，这正好是数组 a 所包含的每个一维数组的长度。也就是说，`p+1`会使得指针指向二维

   数组的下一行，`p-1`会使得指针指向数组的上一行。

   ​	**数组名`a`在表达式中也会被转换为和 p 等价的指针。**

   下面我们就来探索一下如何使用指针 p 来访问二维数组中的每个元素。按照上面的定义：

   1. `p`指向数组 a 的开头，也即第 0 行；`p+1`前进一行，指向第 1 行。

   2. `*(p+1)`表示取地址上的数据，也就是整个第 1 行数据。注意是一行数据，是多个数据，不是第 1 行中的第 0 个元素。

      ```c
      #include <stdio.h>
      
      int main()
      {
          int a[3][4] = 
          { 
              {0, 1, 2, 3}, 
              {4, 5, 6, 7}, 
              {8, 9, 10, 11} 
          };
          int (*p)[4] = a;
          printf("%d\n", sizeof(*(p+1)));//16
      
          return 0;
      }
      ```

   3. `*(p+1)+1`表示第 1 行第 1 个元素的地址。如何理解呢？

      `*(p+1)`单独使用时表示的是第 1 行数据，放在表达式中会被转换为第 1 行数据的首地址，也就是第 1 行第 0 个元素的地址，因

      为使用整行数据没有实际的含义，编译器遇到这种情况都会转换为指向该行第 0 个元素的指针；就像一维数组的名字，在定义时

      或者和`sizeof`、`&`一起使用时才表示整个数组，出现在表达式中就会被转换为指向数组第 0 个元素的指针。

   4. `*(*(p+1)+1)`表示第 1 行第 1 个元素的值。很明显，增加一个 * 表示取地址上的数据。

      根据上面的结论，可以很容易推出以下的等价关系：

      ```c
      a+i == p+i
      a[i] == p[i] == *(a+i) == *(p+i)
      a[i][j] == p[i][j] == *(a[i]+j) == *(p[i]+j) == *(*(a+i)+j) == *(*(p+i)+j)
      ```

3. 示例

   使用指针遍历二维数组

   ```c
   #include <stdio.h>
   
   int main()
   {
       int a[3][4]=
       {
           {0,1,2,3},
           {4,5,6,7},
           {8,9,10,11}
       };
       int(*p)[4];
       int i,j;
       p=a;
       for(i=0; i<3; i++)
       {
           for(j=0; j<4; j++) printf("%2d  ",*(*(p+i)+j));
           printf("\n");
       }
   
       return 0;
   }
   ```

   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\二维数组指针.png)

4. 指针数组与二维数组指针的区别

   指针数组和二维数组指针在定义时非常相似，只是括号的位置不同：

   ```c
   int *(p1[5]);  //指针数组，可以去掉括号直接写作 int *p1[5];
   int (*p2)[5];  //二维数组指针，不能去掉括号
   ```

   指针数组和二维数组指针有着本质上的区别：指针数组是一个数组，只是每个元素保存的都是指针，以上面的`p1`为例，在32位环境

   下它占用`4×5 = 20`个字节的内存。二维数组指针是一个指针，它指向一个二维数组，以上面的`p2`为例，它占用 4 个字节的内存。

## 函数指针

1. 函数指针：一个函数总是占用一段连续的内存区域，函数名在表达式中有时也会被转换为该函数所在内存区域的首地址，这和数组名非常类似。**我们可以把函数的这个首地址（或称入口地址）赋予一个指针变量，使指针变量指向函数所在的内存区域，然后通过指针变量就可以找到并调用该函数**。这种指针就是函数指针。

2. 格式：`returnType (*pointerName)(param list);`

   `returnType`为函数返回值类型，`pointerName`为指针名称，`param list`为函数参数列表。参数列表中可以同时给出参数的类型和

   名称，也可以只给出参数的类型，省略参数的名称，这一点和函数原型非常类似。

   注意`( )`的优先级高于`*`，第一个括号不能省略，如果写作`returnType *pointerName(param list);`就成了函数原型，它表明函

   数的返回值类型为`returnType *`。

3. 示例

   用指针来实现对函数的调用。

   ```c
   #include <stdio.h>
   
   //返回两个数中较大的一个
   int max(int a, int b)
   {
       return a>b ? a : b;
   }
   
   int main()
   {
       int x, y, maxval;
       //定义函数指针
       int (*pmax)(int, int) = max;  //也可以写作int (*pmax)(int a, int b)
       printf("Input two numbers:");
       scanf("%d %d", &x, &y);
       maxval = (*pmax)(x, y);
       printf("Max value: %d\n", maxval);
   
       return 0;
   }
   ```

   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\函数指针.png)

   第 16 行代码对函数进行了调用。`pmax`是一个函数指针，在前面加`*`就表示对它指向的函数进行调用。注意`( )`的优先级高于`*`，

   第一个括号不能省略。

# 结构体

1. 结构体：用来保存不同类型数据的构造类型。结构体与数组不同，数组是保存同一类型的数据。

2. 格式

   ```c
   struct 结构体名
   {
   	类型名1 成员名1;
   	类型名2 成员名2;
   	……
   	类型名n 成员名n;
   };
   ```

3. 示例

   ```c
   struct Student
   {
   	char *name; // 姓名
   	int age; // 年龄
   	float height; // 身高
   };
   ```

4. 定义结构体变量

   1. 格式：`struct 结构体名 结构体变量名;`

   2. 定义结构体变量

      1. 先定义结构体类型，再定义变量

         ```c
         struct Student
         {
         	char *name;
         	int age;
         };
         
         struct Student stu;
         ```

      2. 定义结构体类型的同时定义变量

         ```c
         struct Student
         {
         	char *name;
         	int age;
         } stu;
         
         ```

      3. 匿名结构体定义结构体变量

         ```c
         struct
         {
         	char *name;
         	int age;
         } stu;
         
         ```

         第三种方法与第二种方法的区别在于,第三种方法中省去了结构体类型名称,而直接给出结构变量,**这种结构体最大的问题是结**

         **构体类型不能复用**

5. 结构体成员访问

   1. 格式：`结构体变量名.成员名`

   2. 示例

      ```c
      struct Student
      {
      	char *name;
      	int age;
      };
      
      //定义结构体变量
      struct Student stu;
      
      // 访问stu的age成员
      stu.age = 27;
      printf("age = %d", stu.age);
      ```

6. 结构体变量初始化

   1. 定义同时初始化

      1. 按顺序初始化

         ```c
         struct Student
         {
         	char *name;
         	int age;
         };
         
         struct Student stu = {“lnj", 27};
         ```

      2. 不按顺序初始化

         ```c
         struct Student
         {
         	char *name;
         	int age;
         };
         
         struct Student stu = {.age = 35, .name = “lnj"};
         
         ```

   2. 先定义后初始化

      1. 逐个初始化

         ```c
         struct Student
         {
         	char *name;
         	int age;
         };
         
         struct Student stu;
         
         stu.name = "lnj";
         stu.age = 35;
         
         ```

      2. 一次性初始化

         ```c
         struct Student
         {
         	char *name;
         	int age;
         };
         
         struct Student stu;
         
         stu2 = (struct Student){"lnj", 35};
         
         ```

7. 结构体类型作用域

   1. 结构类型定义在**函数内部**的作用域与**局部变量**的作用域是相同的

   2. 结构类型定义在**函数外部**的作用域与**全局变量**的作用域是相同的

   3. **同一作用域内不要定义两个名称一样的结构体**，会出错，如果真的这样做了，那么局部结构体会屏蔽全局结构体，但还是不推荐这样做。

   4. 示例

      ```c
      #include <stdio.h>
      
      //定义一个全局结构体,作用域到文件末尾
      struct Person
      {
      	int age;
      	char *name;
      };
      
      void test();
      
      int main()
      {
      	//定义局部结构体名为Person,会屏蔽全局结构体
      	//局部结构体作用域,从定义开始到“}”块结束
      	struct Person_
          //struct Person
          {
      		int age;
      	};
      	// 使用局部结构体类型
      	struct Person_ pp;
          //struct Person pp;
      	pp.age = 50;
          //pp.name = "lnj";//会报错，提示没有此成员
          printf("%d\n",pp.age);
          
      	test();
          
      	return 0;
      }
      
      void test()
      {
      	//使用全局的结构体定义结构体变量p
      	struct Person p = {10,"sb"};
      	printf("%d,%s\n",p.age,p.name);
      }
      ```

      ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\结构体类型作用域.png)

## 结构体数组

1. 结构体数组：由结构体组成的数组。结构体数组常用来表示一个拥有相同数据结构的群体，比如一个班的学生、一个车间的职工。

2. 格式：`struct 结构体类型名称 数组名称[元素个数];`

3. 示例

   ```c
   struct Student
   {
   	char *name;
   	int age;
   };
   
   struct Student stu[2];
   ```

4. 初始化

   1. 定义同时初始化

      ```c
      struct Student
      {
      	char *name;
      	int age;
      };
      
      struct Student stu[2] = {{"lnj", 35},{"zs", 18}};
      ```

   2. 先定义后初始化

      ```c
      struct Student
      {
      	char *name;
      	int age;
      };
      
      struct Student stu[2];
      
      stu[0] = {"lnj", 35};
      stu[1] = {"zs", 18};
      
      ```

## 结构体指针

1. 结构体指针：指向结构体变量的指针，称为结构体指针。

2. 格式：`struct 结构名 *结构指针名;`

3. 示例

   ```c
   //结构体
   struct stu
   {
       char *name;  //姓名
       int num;  //学号
       int age;  //年龄
       char group;  //所在小组
       float score;  //成绩
   } stu1 = { "Tom", 12, 18, 'A', 136.5 };
   
   //结构体指针
   struct stu *pstu = &stu1;
   ```

   ```c
   //定义结构体的同时定义结构体指针
   struct stu
   {
       char *name;  //姓名
       int num;  //学号
       int age;  //年龄
       char group;  //所在小组
       float score;  //成绩
   } stu1 = { "Tom", 12, 18, 'A', 136.5 }, *pstu = &stu1;
   ```

4. 注意

   ​	注意，结构体变量名和数组名不同，数组名在表达式中会被转换为数组指针，而结构体变量名不会，无论在任何表达式中它表示.

   的都是整个集合本身，要想取得结构体变量的地址，必须在前面加`&`，所以给 pstu 赋值只能写作：

   ```c
   struct stu *pstu = &stu1;
   ```

   而不能写作：

   ```c
   struct stu *pstu = stu1;
   ```

   ​	还应该注意，结构体和结构体变量是两个不同的概念：结构体是一种数据类型，是一种创建变量的模板，编译器不会为它分配内

   存空间，就像`int`、`float`、`char`这些关键字本身不占用内存一样；结构体变量才包含实实在在的数据，才需要内存来存储。下面

   的写法是错误的，不可能去取一个结构体名的地址，也不能将它赋值给其他变量：

   ```c
   struct stu *pstu = &stu;
   struct stu *pstu = stu;
   ```

5. 访问结构体成员

   1. 格式：`(*pointer).memberName`  或  `pointer->memberName`

   2. 注意

      1. 第一种写法中，`.`的优先级高于`*`，`(*pointer)`两边的括号不能少。如果去掉括号写作`*pointer.memberName`，那么就等效于`*(pointer.memberName)`，这样意义就完全不对了。
      2. 第二种写法中，`->`是一个新的运算符，习惯称它为“箭头”，有了它，可以通过结构体指针直接取得结构体成员；这也是`->`在C语言中的唯一用途。

   3. 示例

      1. 结构体指针的使用

         ```c
         #include <stdio.h>
         
         int main()
         {
             struct
             {
                 char *name;  //姓名
                 int num;  //学号
                 int age;  //年龄
                 char group;  //所在小组
                 float score;  //成绩
             } stu1 = { "Tom", 12, 18, 'A', 136.5 }, *pstu = &stu1;
         
             //读取结构体成员的值
             printf("%s的学号是%d，年龄是%d，在%c组，今年的成绩是%.1f！\n", (*pstu).name, (*pstu).num, (*pstu).age, (*pstu).group, (*pstu).score);
             
             printf("%s的学号是%d，年龄是%d，在%c组，今年的成绩是%.1f！\n", pstu->name, pstu->num, pstu->age, pstu->group, pstu->score);
         
             return 0;
         }
         ```

         ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\结构体指针01.png)

      2. 结构体数组指针的使用

         ```c
         #include <stdio.h>
         
         struct stu
         {
             char *name;  //姓名
             int num;  //学号
             int age;  //年龄
             char group;  //所在小组
             float score;  //成绩
         }stus[] = 
         {
             {"Zhou ping", 5, 18, 'C', 145.0},
             {"Zhang ping", 4, 19, 'A', 130.5},
             {"Liu fang", 1, 18, 'A', 148.5},
             {"Cheng ling", 2, 17, 'F', 139.0},
             {"Wang ming", 3, 17, 'B', 144.5}
         }, *ps;
         
         int main()
         {
             //求数组长度
             int len = sizeof(stus) / sizeof(struct stu);
             printf("Name\t\tNum\tAge\tGroup\tScore\t\n");
             for(ps=stus; ps<stus+len; ps++)
             {
                 printf("%s\t%d\t%d\t%c\t%.1f\n", ps->name, ps->num, ps->age, ps->group, ps->score);
             }
         
             return 0;
         }
         ```

         ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\结构体指针02.png)

6. 结构体指针作为函数参数

   ​	结构体变量名代表的是整个集合本身，作为函数参数时传递的整个集合，也就是所有成员，而不是像数组一样被编译器转换成一个指针。如果结构体成员较多，尤其是成员为数组时，传送的时间和空间开销会很大，影响程序的运行效率。所以最好的办法就是使用结构体指针，这时由实参传向形参的只是一个地址，非常快速。

   ```c
   //计算全班学生的总成绩、平均成绩和以及 140 分以下的人数。
   #include <stdio.h>
   
   struct stu
   {
       char *name;  //姓名
       int num;  //学号
       int age;  //年龄
       char group;  //所在小组
       float score;  //成绩
   }stus[] = 
   {
       {"Li ping", 5, 18, 'C', 145.0},
       {"Zhang ping", 4, 19, 'A', 130.5},
       {"He fang", 1, 18, 'A', 148.5},
       {"Cheng ling", 2, 17, 'F', 139.0},
       {"Wang ming", 3, 17, 'B', 144.5}
   };
   
   void average(struct stu *ps, int len);
   
   int main()
   {
       int len = sizeof(stus) / sizeof(struct stu);
       average(stus, len);
       
       return 0;
   }
   
   void average(struct stu *ps, int len)
   {
       int i, num_140 = 0;
       float average, sum = 0;
       for(i=0; i<len; i++){
           sum += (ps + i) -> score;
           if((ps + i)->score < 140) num_140++;
       }
       printf("sum=%.2f\naverage=%.2f\nnum_140=%d\n", sum, sum/5, num_140);
   }
   ```

   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\结构体指针03.png)

## 结构体内存分析

1. 结构体变量占用的内存空间永远是所有成员中占用内存最大成员的倍数(对齐问题)

   1. 内存对齐：大多数实际的计算机系统对基本类型数据在内存中存放的位置有限制,它们会要求这些数据的起始地址的值是某个数`k`的倍数，这就是所谓的内存对齐。
   2. 对齐模数：这个`k`则被称为该数据类型的对齐模数(alignment modulus)。
   3. 这种强制的要求一来简化了处理器与内存之间传输系统的设计，二来可以提升读取数据的速度。比如这么一种处理器,它每次读写内存的时候都从某个8倍数的地址开始,一次读出或写入8个字节的数据，假如软件能保证`double`类型的数据都从8倍数地址开始，那么读或写一个`double`类型数据就只需要一次内存操作。否则，我们就可能需要两次内存操作才能完成这个动作，因为数据或许恰好横跨在两个符合对齐要求的8字节内存块上。

2. 结构体变量占用存储空间大小

   1. 示例1

      ```c
      struct Person
      {
      	int age; // 4
      	char ch; // 1
      	double score; // 8
      };
      
      struct Person p;
      
      printf("sizeof = %i\n", sizeof(p)); // 16
      ```

   2. 解释

      1. 占用内存最大属性是`score`, 占8个字节, 所以第一次会分配8个字节；
      2. 将第一次分配的8个字节分配给`age`4个,分配给`ch`1个, 还剩下3个字节；
      3. 当需要分配给`score`时, 发现只剩下3个字节, 所以会再次开辟8个字节存储空间；
      4. 一共开辟了两次8个字节空间, 所以最终`p`占用16个字节。

   3. 示例2

      ```c
      struct Person
      {
      	int age; // 4
      	double score; // 8
      	char ch; // 1
      };
      
      struct Person p;
      
      printf("sizeof = %i\n", sizeof(p)); // 24
      ```

   4. 解释

      1. 占用内存最大属性是`score`, 占8个字节, 所以第一次会分配8个字节；
      2. 将第一次分配的8个字节分配给`age`4个,还剩下4个字节；
      3. 当需要分配给`score`时, 发现只剩下4个字节, 所以会再次开辟8个字节存储空间；
      4. 将新分配的8个字节分配给`score`, 还剩下0个字节；（不能使用上次分配剩下的4个字节，因为不够用，如果使用会造成数据横跨在两块储存空间上）
      5. 当需要分配给`ch`时, 发现上一次分配的已经没有了, 所以会再次开辟8个字节存储空间；
      6. 一共开辟了3次8个字节空间, 所以最终`p`占用24个字节。

## 结构体嵌套

1. 结构体嵌套：结构体成员也可以是一个结构体，即构成嵌套结构。

2. 示例

   ```c
   struct Date
   {
   	int month;
   	int day;
   	int year;
   }
   
   struct stu
   {
   	int num;
   	char *name;
   	char sex;
   	struct Date birthday;
   	float score;
   }
   ```

3. 解释

   1. 在stu中嵌套存储Date结构体内容

      ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\结构体嵌套.jpg)

   2. 注意

      结构体不可以嵌套自己变量,可以嵌套指向自己这种类型的指针

      ```c
      struct Student
      {
      	int age;
      	struct Student stu;
      };
      ```

4. 嵌套结构体成员的访问

   如果某个成员也是结构体变量，可以连续使用成员运算符"."访问最低一级成员

   ```c
   struct Date
   {
   	int year;
   	int month;
   	int day;
   };
   
   struct Student
   {
   	char *name;
   	struct Date birthday;
   };
   
   struct Student stu;
   
   stu.birthday.year = 1986;
   stu.birthday.month = 9;
   stu.birthday.day = 10;
   ```

## 结构体和函数

1. 结构体虽然是构造类型, 但是结构体之间赋值是值拷贝, 而不是地址传递

   ```c
   struct Person
   {
   	char *name;
   	int age;
   };
   
   struct Person p1 = {"lnj", 35};
   struct Person p2;
   p2 = p1;
   p2.name = "zs"; // 修改p2不会影响p1
   printf("p1.name = %s\n", p1.name); // lnj
   printf("p2.name = %s\n", p2.name); // zs
   ```

2. 结构体变量作为函数形参时也是值传递, 在函数内修改形参, 不会影响外界实参

   ```c
   #include <stdio.h>
   
   struct Person
   {
   	char *name;
   	int age;
   };
   
   void test(struct Person per);
   
   int main()
   {
   	struct Person p1 = {"lnj", 35};
   	printf("p1.name = %s\n", p1.name); // lnj
       test(p1);
   	printf("p1.name = %s\n", p1.name); // lnj
       
   	return 0;
   }
   
   void test(struct Person per)
   {
   	per.name = "zs";
   }
   ```

# 位域（位段）

1. 位域（位段）：有些数据在存储时并不需要占用一个完整的字节，只需要占用一个或几个二进制位即可。例如开关只有通电和断电两种状态，用 0 和 1 表示足以，也就是用一个二进位。正是基于这种考虑，C语言又提供了一种叫做位域的数据结构。

2. 示例

   在结构体定义时，我们可以指定某个成员变量所占用的二进制位数（Bit），这就是位域。

   ```c
   struct bs
   {
       unsigned m;
       unsigned n: 4;
       unsigned char ch: 6;
   };
   ```

   `:`后面的数字用来限定成员变量占用的位数。成员 m 没有限制，根据数据类型即可推算出它占用 4 个字节（Byte）的内存。成员 n、ch 被`:`后面的数字限制，不能再根据数据类型计算长度，它们分别占用 4、6 位（Bit）的内存。

   n、ch 的取值范围非常有限，数据稍微大些就会发生溢出，请看下面的例子：

   ```c
   #include <stdio.h>
   
   int main()
   {
       struct bs
       {
           unsigned m;
           unsigned n: 4;
           unsigned char ch: 6;
       } a = { 0xad, 0xE, '$'};
       //第一次输出
       printf("%#x, %#x, %c\n", a.m, a.n, a.ch);
       //更改值后再次输出
       a.m = 0xb8901c;
       a.n = 0x2d;
       a.ch = 'z';
       printf("%#x, %#x, %c\n", a.m, a.n, a.ch);
   
       return 0;
   }
   ```

   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\位域01.png)

   ​	对于 n 和 ch，第一次输出的数据是完整的，第二次输出的数据是残缺的。

   ​	第一次输出时，n、ch 的值分别是`0xE`、`0x24`（'$' 对应的 ASCII 码为`0x24`），换算成二进制是`1110`、`10 0100`，都没有超出限定的位数，能够正常输出。

   ​	第二次输出时，n、ch 的值变为`0x2d`、`0x7a`（'z' 对应的 ASCII 码为`0x7a`），换算成二进制分别是`10 1101`、`111 1010`，都超出了限定的位数。超出部分被直接截去，剩下`1101`、`11 1010`，换算成十六进制为`0xd`、`0x3a`（`0x3a`对应的字符是 :）。

   ​	**C语言标准规定，位域的宽度不能超过它所依附的数据类型的长度。通俗地讲，成员变量都是有类型的，这个类型限制了成员变量的最大长度，`:`后面的数字不能超过这个长度。**

   ​	例如上面的`bs`，`n`的类型是`unsigned int`，长度为 4 个字节，共计 32 位，那么 n 后面的数字就不能超过 32；`ch`的类型是 `unsigned char`，长度为 1 个字节，共计 8 位，那么 ch 后面的数字就不能超过 8。

   ​	我们可以这样认为，位域技术就是在成员变量所占用的内存中选出一部分位宽来存储数据。

   ​	**C语言标准还规定，只有有限的几种数据类型可以用于位域。在 ANSI C 中，这几种数据类型是`int`、`signed int`和 `unsigned int`（`int `默认就是`signed int`）；到了 C99，_Bool 也被支持了。**

   ​	但编译器在具体实现时都进行了扩展，额外支持了`char`、`signed char`、`unsigned char`以及`enum`类型，所以上面的代码虽然不符合C语言标准，但它依然能够被编译器支持。

3. 位于的存储

   1. C语言标准并没有规定位域的具体存储方式，不同的编译器有不同的实现，但它们都尽量压缩存储空间。

   2. 位域的具体存储规则

      1. 当相邻成员的类型相同时，如果它们的位宽之和小于类型的 sizeof 大小，那么后面的成员紧邻前一个成员存储，直到不能容纳为止；如果它们的位宽之和大于类型的 sizeof 大小，那么后面的成员将从新的存储单元开始，其偏移量为类型大小的整数倍。

         ```c
         #include <stdio.h>
         
         int main()
         {
             struct bs
             {
                 unsigned m: 6;
                 unsigned n: 12;
                 unsigned p: 4;
             };
             printf("%d\n", sizeof(struct bs));
         
             return 0;
         }
         ```

         ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\位域02.png)

         ​	m、n、p 的类型都是`unsigned int`，`sizeof` 的结果为 4 个字节（Byte），也即 32 个位（Bit）。m、n、p 的位宽之和为 `6+12+4 = 22`，小于 32，所以它们会挨着存储，中间没有缝隙。

         ​	`sizeof(struct bs)`的大小之所以为 4，而不是 3，是因为要将内存对齐到 4 个字节，以便提高存取效率。

         ​	如果将成员 m 的位宽改为 22，那么输出结果将会是 8，因为`22+12 = 34`，大于 32，n 会从新的位置开始存储，相对 m 的偏移量是 `sizeof(unsigned int)`，也即 4 个字节。

         ​	如果再将成员 p 的位宽也改为 22，那么输出结果将会是 12，三个成员都不会挨着存储。

      2. 当相邻成员的类型不同时，不同的编译器有不同的实现方案，GCC会压缩存储，而 VC/VS 不会。

         ```c
         #include <stdio.h>
         
         int main()
         {
             struct bs
             {
                 unsigned m: 12;
                 unsigned char ch: 4;
                 unsigned p: 4;
             };
             printf("%d\n", sizeof(struct bs));
         
             return 0;
         }
         ```

         ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\位域03.png)

         ​	在之前，在 GCC 下的运行结果为 4，三个成员挨着存储；在 VC/VS 下的运行结果为 12，三个成员按照各自的类型存储（与不指定位宽时的存储方式相同）。但是现在GCC也不在压缩存储了。

         ​	m 、ch、p 的长度分别是 4、1、4 个字节，共计占用 9 个字节内存，之所以在 VC/VS 下的输出结果是 12，还是因为要将内存对齐（ch 单独占用 4 个字节），以便提高存取效率。

      3. 如果成员之间穿插着非位域成员，那么不会进行压缩。

         ```c
         struct bs
         {
             unsigned m: 12;
             unsigned ch;
             unsigned p: 4;
         };
         ```

         在各个编译器下 sizeof 的结果都是 12。

          	**通过上面的分析，我们发现位域成员往往不占用完整的字节，有时候也不处于字节的开头位置，因此使用`&`获取位域成员的地址是没有意义的，C语言也禁止这样做。地址是字节（Byte）的编号，而不是位（Bit）的编号。**

4. 无名位域

   位域成员可以没有名称，只给出数据类型和位宽。

   ```c
   struct bs
   {
       int m: 12;
       int  : 20;  //该位域成员不能使用
       int n: 4;
   };
   ```

   无名位域一般用来作填充或者调整成员位置。因为没有名称，无名位域不能使用。

   上面的例子中，如果没有位宽为 20 的无名成员，m、n 将会挨着存储，`sizeof(struct bs)` 的结果为 4；有了这 20 位作为填充，m、n 将分开存储，`sizeof(struct bs) `的结果为 8。

# 共用体

1. 共用体与结构体

   1. 结构体的各个成员会占用不同的内存，互相之间没有影响；而共用体的所有成员占用同一段内存，修改一个成员会影响其余所有成员。
   2. 结构体占用的内存大于等于所有成员占用的内存的总和（成员之间可能会存在缝隙），共用体占用的内存等于最长的成员占用的内存。共用体使用了内存覆盖技术，同一时刻只能保存一个成员的值，如果对新的成员赋值，就会把原来成员的值覆盖掉。

2. 格式

   1. 定义共用体类型

      ```c
      union 共用体名.
      {
      	数据类型 属性名称;
      	数据类型 属性名称;
      	... ....
      };
      ```

   2. 定义共用体类型变量

      ```c
      union 共用体名 共用体变量名称;
      ```

3. 特点：

4. 由于所有属性共享同一块内存空间, 所以只要其中一个属性发生了改变, 其它的属性都会受到影响。

5. 示例

   ```c
   union Test
   {
   	int age;
   	char ch;
   };
   
   union Test t;
   
   printf("sizeof(p) = %i\n", sizeof(t));
   t.age = 33;
   printf("t.age = %i\n", t.age); // 33
   t.ch = 'a';
   printf("t.ch = %c\n", t.ch); // a
   printf("t.age = %i\n", t.age); // 97
   ```

6. 共用体变量占用存储空间大小

   共用体`data`中，成员`f`占用的内存最多，为 8 个字节，所以`data`类型的变量（也就是 a、b、c）也占用 8 个字节的内存，请看下面的演示：

   ```c
   #include <stdio.h>
   
   union data
   {
       int n;
       char ch;
       short m;
   };
   
   int main()
   {
       union data a;
       printf("%d, %d\n", sizeof(a), sizeof(union data) );
       a.n = 0x40;
       printf("%X, %c, %hX\n", a.n, a.ch, a.m);
       a.ch = '9';
       printf("%X, %c, %hX\n", a.n, a.ch, a.m);
       a.m = 0x2059;
       printf("%X, %c, %hX\n", a.n, a.ch, a.m);
       a.n = 0x3E25AD54;
       printf("%X, %c, %hX\n", a.n, a.ch, a.m);
      
       return 0;
   }
   ```

   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\共用体变量的内存占用01.png)

   ​	这段代码不但验证了共用体的长度，还说明共用体成员之间会相互影响，修改一个成员的值会影响其他成员。

   ​	要想理解上面的输出结果，弄清成员之间究竟是如何相互影响的，就得了解各个成员在内存中的分布。以上面的`data`为例，各个成员在内存中的分布如下：

   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\共用体变量的内存占用02.jpg)

   ​	成员 n、ch、m 在内存中“对齐”到一头，对 ch 赋值修改的是前一个字节，对 m 赋值修改的是前两个字节，对 n 赋值修改的是全部字节。也就是说，ch、m 会影响到 n 的一部分数据，而 n 会影响到 ch、m 的全部数据。

   ​	上图是在绝大多数 PC 机上的内存分布情况，如果是 51 单片机，情况就会有所不同：

   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\共用体变量的内存占用03.jpg)

7. 应用场景

   1. 通信中的数据包会用到共用体，因为不知道对方会发送什么样的数据包过来，用共用体的话就简单了，定义几种格式的包，收到包之后就可以根据包的格式取出数据。

   2. 节约内存。如果有2个很长的数据结构，但不会同时使用，比如一个表示老师，一个表示学生，要统计老师和学生的情况，用结构体就比较浪费内存，这时就可以考虑用共用体来设计。

   3. 某些应用需要大量的临时变量，这些变量类型不同，而且会随时更换。而你的堆栈空间有限，不能同时分配那么多临时变量。这时可以使用共用体让这些变量共享同一个内存空间，这些临时变量不用长期保存，用完即丢，和寄存器差不多，不用维护。

   4. 共用体在一般的编程中应用较少，在单片机中应用较多。对于 PC 机，经常使用到的一个实例是： 现有一张关于学生信息和教师信息的表格。学生信息包括姓名、编号、性别、职业、分数，教师的信息包括姓名、编号、性别、职业、教学科目。

      请看下面的表格：

      ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\共用体变量的应用01.png)

      ​	f 和 m 分别表示女性和男性，s 表示学生，t 表示教师。可以看出，学生和教师所包含的数据是不同的。现在要求把这些信息放在同一个表格中，并设计程序输入人员信息然后输出。

      ​	如果把每个人的信息都看作一个结构体变量的话，那么教师和学生的前 4 个成员变量是一样的，第 5 个成员变量可能是 `score`或者`course`。当第 4 个成员变量的值是 s 的时候，第 5 个成员变量就是`score`；当第 4 个成员变量的值是 t 的时候，第 5 个成员变量就是`course`。

      ```c
      #include <stdio.h>
      #include <stdlib.h>
      
      #define TOTAL 4  //人员总数
      
      struct
      {
          char name[20];
          int num;
          char sex;
          char profession;
          union
          {
              float score;
              char course[20];
          } sc;
      } bodys[TOTAL];
      
      int main()
      {
          int i;
          //输入人员信息
          for(i=0; i<TOTAL; i++)
          {
              printf("Input info: ");
              scanf("%s %d %c %c", bodys[i].name, &(bodys[i].num), &(bodys[i].sex), &(bodys[i].profession));
              if(bodys[i].profession == 's')
              {  //如果是学生
                  scanf("%f", &bodys[i].sc.score);
              }
              else
              {  //如果是老师
                  scanf("%s", bodys[i].sc.course);
              }
              fflush(stdin);
          }
      
          //输出人员信息
          printf("\nName\t\tNum\tSex\tProfession\tScore / Course\n");
          for(i=0; i<TOTAL; i++)
          {
              if(bodys[i].profession == 's')
              {  //如果是学生
                  printf("%s\t%d\t%c\t%c\t\t%f\n", bodys[i].name, bodys[i].num, bodys[i].sex, bodys[i].profession, bodys[i].sc.score);
              }
              else
              {  //如果是老师
                  printf("%s\t%d\t%c\t%c\t\t%s\n", bodys[i].name, bodys[i].num, bodys[i].sex, bodys[i].profession, bodys[i].sc.course);
              }
          }
          
          return 0;
      }
      ```

      ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\共用体变量的应用02.png)

# 枚举

1. 引入

   ​	在实际编程中，有些数据的取值往往是有限的，只能是非常少量的整数，并且最好为每个值都取一个名字，以方便在后续代码中使用，比如一个星期只有七天，一年只有十二个月，一个班每周有六门课程等。

   ​	C语言提供了一种**枚举（Enum）类型**，能够列出所有可能的取值，并给它们取一个名字。

2. 格式

   ```c
   enum typeName{ valueName1, valueName2, valueName3, ...... };
   ```

   `enum`是一个新的关键字，专门用来定义枚举类型，这也是它在C语言中的唯一用途；`typeName`是枚举类型的名字；`valueName1, valueName2, valueName3, ......`是每个值对应的名字的列表。注意最后的`;`不能少。

3. 示例

   ```c
   enum week{ Mon, Tues, Wed, Thurs, Fri, Sat, Sun };
   ```

   ​	可以看到，我们仅仅给出了名字，却没有给出名字对应的值，这是因为枚举值默认从 0 开始，往后逐个加 1（递增）；也就是说，week 中的 Mon、Tues ...... Sun 对应的值分别为 0、1 ...... 6。

   ```c
   enum week{ Mon = 1, Tues = 2, Wed = 3, Thurs = 4, Fri = 5, Sat = 6, Sun = 7 };
   ```

   ​	这样，我们就给每个名字都指定了值。

   ```c
   enum week{ Mon = 1, Tues, Wed, Thurs, Fri, Sat, Sun };
   ```

   ​	这样系更简单，这样枚举值就从 1 开始递增，跟上面的写法是等效的。

4. 枚举变量

   枚举是一种类型，通过它可以定义枚举变量：

   ```c
   enum week a, b, c;
   ```

   也可以在定义枚举类型的同时定义变量：

   ```c
   enum week{ Mon = 1, Tues, Wed, Thurs, Fri, Sat, Sun } a, b, c;
   ```

   有了枚举变量，就可以把列表中的值赋给它：

   ```c
   enum week{ Mon = 1, Tues, Wed, Thurs, Fri, Sat, Sun };
   enum week a = Mon, b = Wed, c = Sat;
   ```

   或者：

   ```c
   enum week{ Mon = 1, Tues, Wed, Thurs, Fri, Sat, Sun } a = Mon, b = Wed, c = Sat;
   ```

5. 练习

   判断用户输入的是星期几。

   ```c
   #include <stdio.h>
   #include <string.h>
   
   int main()
   {
       enum week{ Mon = 1, Tues, Wed, Thurs, Fri, Sat, Sun } day;
       scanf("%d", &day);
       switch(day)
       {
           case Mon: puts("Monday"); break;
           case Tues: puts("Tuesday"); break;
           case Wed: puts("Wednesday"); break;
           case Thurs: puts("Thursday"); break;
           case Fri: puts("Friday"); break;
           case Sat: puts("Saturday"); break;
           case Sun: puts("Sunday"); break;
           default: puts("Error!");
       }
       
       return 0;
   }
   ```

   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\枚举示例.png)

6. 注意

   1.  枚举列表中的`Mon`、`Tues`、`Wed`这些标识符的作用范围是全局的（严格来说是`main()`函数内部），不能再定义与它们名字相同的变量。

   2. `Mon`、`Tues`、`Wed`等都是常量，不能对它们赋值，只能将它们的值赋给其他的变量。

   3. `case`关键字后面必须是一个整数，或者是结果为整数的表达式，但不能包含任何变量，正是由于`Mon`、`Tues`、`Wed`这些名字最终会被替换成一个整数，所以它们才能放在`case`后面。

      枚举类型变量需要存放的是一个整数，猜测它的长度和`int`应该相同，下面来验证一下：

      ```c
      #include <stdio.h>
      
      int main()
      {
          enum week{ Mon = 1, Tues, Wed, Thurs, Fri, Sat, Sun } day = Mon;
          printf("%d, %d, %d, %d, %d\n", sizeof(enum week), sizeof(day), sizeof(Mon), sizeof(Wed), sizeof(int) );
          
          return 0;
      }
      ```

      ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\枚举变量大小.png)

# 预处理命令

1. 预处理命令：这种以`#`号开头的命令称为预处理命令。例如使用库函数之前，应该用`#include`引入对应的头文件。

2. C语言源文件编译执行的过程

   1. 编译（Compile）会将源文件（`.c`文件）转换为目标文件。对于 VC/VS，目标文件后缀为`.obj`；对于GCC，目标文件后缀为`.o`。
   2. 链接（Link）是针对多个文件的，它会将编译生成的多个目标文件以及系统中的库、组件等合并成一个可执行程序。

3. 预处理

   ​	在实际开发中，有时候在编译之前还需要对源文件进行简单的处理。例如，我们希望自己的程序在 Windows 和 Linux 下都能够

   运行，那么就要在 Windows 下使用 VS 编译一遍，然后在 Linux 下使用 GCC 编译一遍。但是现在有个问题，程序中要实现的某个功

   能在 VS 和 GCC 下使用的函数不同（假设 VS 下使用 a()，GCC 下使用 b()），VS 下的函数在 GCC 下不能编译通过，GCC 下的函数在

    VS 下也不能编译通过，怎么办呢？

   ​	这就需要在编译之前先对源文件进行处理：如果检测到是 VS，就保留 a() 删除 b()；如果检测到是 GCC，就保留 b() 删除 a()。

   ​	这些在编译之前对源文件进行简单加工的过程，就称为**预处理**（即预先处理、提前处理）。

   ​	预处理主要是处理以`#`开头的命令，例如`#include <stdio.h>`等。预处理命令要放在所有函数之外，而且一般都放在源文件的

   前面。

   ​	预处理是C语言的一个重要功能，由**预处理程序**完成。当对一个源文件进行编译时，系统将自动调用预处理程序对源程序中的预

   处理部分作处理，处理完毕自动进入对源程序的编译。

   ​	编译器会将预处理的结果保存到和源文件同名的`.i`文件中，例如 main.c 的预处理结果在 main.i 中。和`.c`一样，`.i`也是文本文

   件，可以用编辑器打开直接查看内容。

   ​	C语言提供了多种预处理功能，如宏定义、文件包含、条件编译等，合理地使用它们会使编写的程序便于阅读、修改、移植和调

   试，也有利于模块化程序设计。

4. 实例

   假如现在要开发一个C语言程序，让它暂停 5 秒以后再输出内容，并且要求跨平台，在 Windows 和 Linux 下都能运行，怎么办呢？

   这个程序的难点在于，不同平台下的暂停函数和头文件都不一样：

   1. Windows 平台下的暂停函数的原型是`void Sleep(DWORD dwMilliseconds)`（注意 S 是大写的），参数的单位是“毫秒”，位于 `<windows.h> `头文件。
   2. Linux 平台下暂停函数的原型是`unsigned int sleep (unsigned int seconds)`，参数的单位是“秒”，位于`<unistd.h>`头文件。

   不同的平台下必须调用不同的函数，并引入不同的头文件，否则就会导致编译错误，因为 Windows 平台下没有`sleep()`函数，也没

   有`<unistd.h>`头文件，反之亦然。这就要求我们在编译之前，也就是预处理阶段来解决这个问题。请看下面的代码：

   ```c
   #include <stdio.h>
   
   //不同的平台下引入不同的头文件
   #if _WIN32  //识别windows平台
   #include <windows.h>
   #elif __linux__  //识别linux平台
   #include <unistd.h>
   #endif
   
   int main()
   {
       //不同的平台下调用不同的函数
       #if _WIN32  //识别windows平台
       Sleep(5000);
       #elif __linux__  //识别linux平台
       sleep(5);
       #endif
   
       puts("http://c.biancheng.net/");
   
       return 0;
   }
   ```

   `#if`、`#elif`、`#endif`就是预处理命令，它们都是在编译之前由预处理程序来执行的。这里我们不讨论细节，只从整体上来理解。

   对于 Windows 平台，预处理以后的代码变成：

   ```c
   #include <stdio.h>
   #include <windows.h>
   
   int main()
   {
       Sleep(5000);
       puts("http://c.biancheng.net/");
   
       return 0;
   }
   ```

   对于 Linux 平台，预处理以后的代码变成：

   ```c
   #include <stdio.h>
   #include <unistd.h>
   
   int main()
   {
       sleep(5);
       puts("http://c.biancheng.net/");
   
       return 0;
   }
   ```

   在不同的平台下，编译之前（预处理之后）的源代码都是不一样的。这就是预处理阶段的工作，它把代码当成普通文本，根据设定的

   条件进行一些简单的文本替换，将替换以后的结果再交给编译器处理。

## #include用法详解

1. `#include`：文件包含命令，用来引入对应的头文件（`.h`文件）。其也是C语言预处理命令的一种。

2. 处理过程

   `#include`的处理过程很简单，就是将头文件的内容插入到该命令所在的位置，从而把头文件和当前源文件连接成一个源文件，这与复制粘贴的效果相同。

3. 用法

   ```c
   #include <stdHeader.h>
   #include "myHeader.h"
   ```

   使用尖括号`< >`和双引号`" "`的区别在于头文件的搜索路径不同：

   1. 使用尖括号`< >`，编译器会到系统路径下查找头文件；
   2. 而使用双引号`" "`，编译器首先在当前目录下查找头文件，如果没有找到，再到系统路径下查找。

   也就是说，使用双引号比使用尖括号多了一个查找路径，它的功能更为强大。

   系统目录下的标准头文件用两种方法都可以找得到，而我们自己编写的头文件，一般存放于当前项目的路径下，所以不能使用尖括号，只能使用双引号。

4. 注意

   1. 一个`#include`命令只能包含一个头文件，多个头文件需要多个`#include`命令。
   2. 同一个头文件可以被多次引入，多次引入的效果和一次引入的效果相同，因为头文件在代码层面有防止重复引入的机制。
   3. 文件包含允许嵌套，也就是说在一个被包含的文件中又可以包含另一个文件。

5. 使用`#include`命令引入自定义头文件

   本例中需要创建三个文件，分别是 main.c、my.c 和 my.h，如下图所示：

   ![](D:\Programmering Learning\Markdown文档\C语言教程\动画\使用#include引入自定义头文件01.gif)

   ​												    Visual Studio

   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\使用#include引入自定义头文件02.png)
   
   ​											Visual Studio Code + Xmake
   
   my.c：
   
   ```c
   //计算从m加到n的和
   int sum(int m, int n)
   {
       int i, sum = 0;
       for (i = m; i <= n; i++)
       {
           sum += i;
       }
       
       return sum;
   }
   ```
   
   my.h：
   
   ```c
   //声明函数
   int sum(int m, int n);
   ```
   
   main.c：
   
   ```c
   #include <stdio.h>
   #include "my.h"
   
   int main()
   {
       printf("%d\n", sum(1, 100));
       
       return 0;
   }
   ```

   我们在`my.c`中定义了`sum()`函数，在`my.h`中声明了`sum()`函数，这可能与很多初学者的认知发生了冲突：函数不是在头文件中定

   义的吗？为什么头文件中只有声明？
   
   **「在头文件中定义定义函数和全局变量」这种认知是原则性的错误！不管是标准头文件，还是自定义头文件，都只能包含变量和函数的声明，不能包含定义，否则在多次引入时会引起重复定义错误。**
   
   此外，可能还有疑问，`main.c`只是引入了`my.h`，没有引入`my.c`，程序在编译时应该找不到函数定义呀，然而当我们亲自去运行程序的时候，却发现运行结果是正确的，这是怎么回事呢？
   
   原因在此处不做详述，关于这个问题的原因需要深入学习编译和链接的原理，感兴趣的可以自行在网上查找资料。

# 宏

1. 宏定义命令：`#define`叫做宏定义命令，它也是C语言预处理命令的一种。

2. 宏定义：用一个标识符来表示一个字符串，如果在后面的代码中出现了该标识符，那么就全部替换成指定的字符串。

3. 格式：`#define  宏名  字符串`

   `#`表示这是一条预处理命令，所有的预处理命令都以 # 开头。

   `宏名`是标识符的一种，命名规则和变量相同。

   `字符串`可以是数字、表达式、if 语句、函数等。

   这里所说的字符串是一般意义上的字符序列，不要和C语言中的字符串等同，它不需要双引号。

4. 示例

   ```c
   #include <stdio.h>
   
   #define N 100
   
   int main()
   {
       int sum = 20 + N;
       printf("%d\n", sum);//120
       
       return 0;
   }
   ```

   ​	注意第 6 行代码`int sum = 20 + N`，`N`被`100`代替了。

   ​	`#define N 100`就是宏定义，`N`为宏名，`100`是宏的内容（宏所表示的字符串）。在预处理阶段，对程序中所有出现的“宏名”，

   预处理器都会用宏定义中的字符串去代换，这称为“宏替换”或“宏展开”。

   ​	宏定义是由源程序中的宏定义命令`#define`完成的，宏替换是由预处理程序完成的。

   ```c
   //程序中反复使用的表达式就可以使用宏定义
   #define M (n*n+3*n)
   ```

   ​	它的作用是指定标识符`M`来表示`(y*y+3*y)`这个表达式。在编写代码时，所有出现 `(y*y+3*y) `的地方都可以用`M`来表示，而对源程序编译时，将先由预处理程序进行宏代替，即用 `(y*y+3*y)`去替换所有的宏名`M`，然后再进行编译。

   ```c
   #include <stdio.h>
   
   #define M (n*n+3*n)
   
   int main()
   {
       int sum, n;
       printf("Input a number: ");
       scanf("%d", &n);
       sum = 3*M+4*M+5*M;
       printf("sum=%d\n", sum);
       
       return 0;
   }
   ```

   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\宏01.png)

   ​	程序的开头首先定义了一个宏 M，它表示 `(n*n+3*n) `这个表达式。在 9 行代码中使用了宏`M`，预处理程序将它展开为下面的语句：

   ```c
   sum=3*(n*n+3*n)+4*(n*n+3*n)+5*(n*n+3*n);
   ```

   ​	需要注意的是，在宏定义中表达式`(n*n+3*n)`两边的括号不能少，否则在宏展开以后可能会产生歧义。下面是一个反面的例子：

   ```c
   #difine M n*n+3*n
   ```

   ​	在宏展开后将得到下述语句：

   ```c
   s=3*n*n+3*n+4*n*n+3*n+5*n*n+3*n;
   ```

   ​	这相当于：

   ```c
   3n²+3n+4n²+3n+5n²+3n
   ```

   ​	这显然是不正确的。所以进行宏定义时要注意，应该保证在宏替换之后不发生歧义。

5. 注意

   1. 宏名一般用大写字母，以便与变量名区别开来，但用小写也没有语法错误。

   2. 宏定义不是说明或语句，在行末不必加分号，如加上分号则连分号也一起替换。

   3. 对程序中用双引号扩起来的字符串内的字符，不进行宏的替换操作。

      ```c
      #include <stdio.h>
      
      #define R 10
      
      int main()
      {
          //在前面定义了一个叫 R 的宏，但是在这里“Radio”中的 R 不会被替换成10
          char *s = "Radio";
          
          return 0;
      }
      ```

   4. 在编译预处理用字符串替换宏名时，不作语法检查，只是简单的字符串替换。只有在编译的时候才对已经展开宏名的源程序进行语法检查。因为宏定义是用宏名来表示一个字符串，在宏展开时又以该字符串取代宏名，这只是一种简单粗暴的替换。

      ```c
      #include <stdio.h>
      
      #include I 100
      
      int main()
      {
          int i[3] = I;
          
          return 0;
      }
      ```

   5. 宏定义必须写在函数之外，宏名的有效范围是从定义位置到文件结束。如果需要终止宏定义的作用域，可以用`#undef`命令。

      ```c
      #include <stdio.h>
      
      #define PI 3.14
      
      int main()
      {
          printf("%f",PI);
          
          return 0;
      }
      
      #undef PI
      
      void test()
      {
          printf("%f",PI);//此处不能继续使用
      }
      ```

   6. 定义一个宏时可以引用已经定义的宏名。

      ```c
      #define R 3.0
      #define PI 3.14
      #define L 2*PI*R
      #define S PI*R*R
      ```

   7. 可用宏定义表示数据类型,使书写方便。

      ```c
      #include <stdio.h>
      
      #define String char*
      
      int main()
      {
          String str = "This is a string!";
          
          return 0;
      }
      ```

6. 带参数的宏定义

   1. C语言允许宏带有参数。在**宏定义**中的参数称为**"形式参数"**,在宏调用中的参数称为**"实际参数"**。对带参数的宏,在调用中,不仅要宏展开,而且要用实参去代换形参。

   2. 格式

      1. 带参宏定义的一般形式：` #define 宏名(形参表) 字符串`
      2. 带参宏调用的一般形式：`宏名(实参列表);`

   3. 示例

      ```c
      #include <stdio.h>
      
      //定义一个带有2个参数的宏average
      #define average(a,b) (a + b)/2
      
      int main()
      {
          //会被替换成：int a = (10 + 4)/2;
          int a = average(10,4);
          printf("average = %d",a);//average = 7
          
          return 0;
      }
      ```

      ```c
      #include <stdio.h>
      
      #define MAX(a,b) (a>b) ? a : b
      
      int main()
      {
          int x , y, max;
          printf("input two numbers: ");
          scanf("%d %d", &x, &y);
          max = MAX(x, y);
          printf("max=%d\n", max);
          
          return 0;
      }
      ```

      ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\带参数宏定义01.png)

   4. 注意

      1. 带参宏定义中，形参之间可以出现空格，但是宏名和形参列表之间不能有空格出现

         ```c
         #define MAX  (a,b)  (a>b)?a:b
         ```

         这将被认为是无参宏定义，宏名 MAX 代表字符串`(a,b) (a>b)?a:b`。宏展开时，宏调用语句：

         ```c
         max = MAX(x,y);
         ```

         将变为：

         ```c
         max = (a,b)(a>b)?a:b(x,y);
         ```

         这显然是错误的。

      2. 在带参宏定义中，不会为形式参数分配内存，因此不必指明数据类型。而在宏调用中，实参包含了具体的数据，要用它们去替换形参，因此实参必须要指明数据类型。

         这一点和函数是不同的：在函数中，形参和实参是两个不同的变量，都有自己的作用域，调用时要把实参的值传递给形参；而在带参数的宏中，只是符号的替换，不存在值传递的问题。

         ```c
         //输入 n，输出 (n+1)^2 的值。
         #include <stdio.h>
         
         #define SQ(y) (y)*(y)
         
         int main()
         {
             int a, sq;
             printf("input a number: ");
             scanf("%d", &a);
             sq = SQ(a+1);
             printf("sq=%d\n", sq);
             
             return 0;
         }
         ```

         ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\带参数宏定义02.png)

         第 3 行为宏定义，形参为 y。第 10 行宏调用中实参为`a+1`，是一个表达式，在宏展开时，用 `a+1`代换`y`，再用`(y)*(y)`代换`SQ`，得到如下语句：

         ```c
         sq=(a+1)*(a+1);
         ```

         这与函数的调用是不同的，函数调用时要把实参表达式的值求出来再传递给形参，而宏展开中对实参表达式不作计算，直接按照原样替换。

      3. 在宏定义中，字符串内的形参通常要用括号括起来以避免出错。例如上面的宏定义中`(y)*(y)`表达式的`y`都用括号括起来，因此结果是正确的。

         如果去掉括号，把程序改为以下形式：

         ```c
         #include <stdio.h>
         
         #define SQ(y) y*y
         
         int main()
         {
             int a, sq;
             printf("input a number: ");
             scanf("%d", &a);
             sq = SQ(a+1);
             printf("sq=%d\n", sq);
             
             return 0;
         }
         ```

         ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\带参数宏定义03.png)
         
         同样输入 9，但结果却是不一样的。问题在哪里呢？这是由于宏展开只是简单的符号替换的过程，没有任何其它的处理。宏替换后将得到以下语句：
         
         ```c
         sq=a+1*a+1;
         ```
         
         由于 a 为 9，故 sq 的值为 19。这显然与题意相违，因此参数两边的括号是不能少的。即使在参数两边加括号还是不够的，请看下面程序：
         
         ```c
         #include <stdio.h>
         
         #define SQ(y) (y)*(y)
         
         int main()
         {
             int a,sq;
             printf("input a number: ");
             scanf("%d", &a);
             sq = 200 / SQ(a+1);
             printf("sq=%d\n", sq);
             
             return 0;
         }
         ```
         
         与前面的代码相比，只是把宏调用语句改为：
         
         ```c
         sq = 200/SQ(a+1);
         ```
         
         运行程序后，如果仍然输入 9，那么我们希望的结果为 2。但实际情况并非如此：
         
         ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\带参数宏定义04.png)
         
         为什么会得这样的结果呢？分析宏调用语句，在宏展开之后变为：
         
         ```c
         sq=200/(a+1)*(a+1);
         ```
         
         a 为 9 时，由于`/`和`*`运算符优先级和结合性相同，所以先计算`200/(9+1)`，结果为 20，再计算`20*(9+1)`，最后得到 200。
         
         为了得到正确答案，应该在宏定义中的整个字符串外加括号：
         
         ```c
         #include <stdio.h>
         
         #define SQ(y) ((y)*(y))
         
         int main()
         {
             int a,sq;
             printf("input a number: ");
             scanf("%d", &a);
             sq = 200 / SQ(a+1);
             printf("sq=%d\n", sq);
             
             return 0;
         }
         ```
         
         **由此可见，对于带参宏定义不仅要在参数两侧加括号，还应该在整个字符串外加括号。**

7. 带参数宏定义与函数的区别

   1. 区别

      ​	宏展开仅仅是字符串的替换，不会对表达式进行计算；宏在编译之前就被处理掉了，它没有机会参与编译，也不会占用内存。而函数是一段可以重复使用的代码，会被编译，会给它分配内存，每次调用函数，就是执行这块内存中的代码。

   2. 示例

      1. 用函数计算平方值。

         ```c
         #include <stdio.h>
         
         int SQ(int y)
         {
           return ((y)*(y));
         }
         
         int main()
         {
             int i=1;
             while(i<=5)
             {
                 printf("%d^2 = %d\n", (i-1), SQ(i++));
             }
             
             return 0;
         }
         ```

         ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\带参数宏定义与函数的区别01.png)

      2. 用宏计算平方值。

         ```c
         #include <stdio.h>
         
         #define SQ(y) ((y)*(y))
         
         int main()
         {
             int i=1;
             while(i<=5)
             {
                 printf("%d^2 = %d\n", i, SQ(i++));
             }
             
             return 0;
         }
         ```

         在Visual Studio Code的运行结果如下下（其它编译器的运行结果可能不同，这个`++`运算的顺序有关）

         ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\带参数宏定义与函数的区别02.png)

      3. 解释

         在示例 1 中，先把实参`i`传递给形参`y`，然后再自增 1，这样每循环一次`i`的值增加 1，所以最终要循环 5  次。

         在示例 2 中，宏调用只是简单的字符串替换，`SQ(i++)`会被替换为`((i++)*(i++))`，这样每循环一次`i`的值增加 2，所以最终只循环 3  次。

         由此可见，宏和函数只是在形式上相似，本质上是完全不同的。

         带参数的宏也可以用来定义多个语句，在宏调用时，把这些语句又替换到源程序中，请看下面的例子：

         ```c
         #include <stdio.h>
         
         #define SSSV(s1, s2, s3, v) s1 = length * width; s2 = length * height; s3 = width * height; v = width * length * height;
         
         int main()
         {
             int length = 3, width = 4, height = 5, sa, sb, sc, vv;
             SSSV(sa, sb, sc, vv);
             printf("sa=%d, sb=%d, sc=%d, vv=%d\n", sa, sb, sc, vv);
             
             return 0;
         }
         ```

         ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\带参数宏定义与函数的区别03.png)

# 条件编译

1. 引入

   假如现在要开发一个C语言程序，让它输出红色的文字，并且要求跨平台，在 Windows 和 Linux 下都能运行，怎么办呢？

   这个程序的难点在于，不同平台下控制文字颜色的代码不一样，我们必须要能够识别出不同的平台。

   Windows 有专有的宏`_WIN32`，Linux 有专有的宏`__linux__`，以现有的知识，我们很容易就想到了`if else`，请看下面的代码：

   ```c
   #include <stdio.h>
   
   int main()
   {
       if(_WIN32)
       {
           system("color 0c");
           printf("Hello,World!\n");
       }
       else if(__linux__)
       {
           printf("\033[22;31mHello,World!\n\033[22;30m");
       }
       else
       {
           printf("I'm fine\n");
       }
   
       return 0;
   }
   ```

   但这段代码是错误的，在 Windows 下提示 __linux__ 是未定义的标识符，在 Linux 下提示 _Win32 是未定义的标识符。对上面的代码进行改进：

   ```c
   #include <stdio.h>
   
   int main()
   {
       #if _WIN32
           system("color 0c");
           printf("Hello,World!\n");
       #elif __linux__
           printf("\033[22;31mHello,World\n\033[22;30m");
       #else
           printf("I'm fine\n");
       #endif
   
       return 0;
   }
   ```

   ​	`#if`、`#elif`、`#else`和`#endif`都是预处理命令，整段代码的意思是：如果宏 _WIN32 的值为真，就保留第 6、7 行代码，删除第 9、11 行代码；如果宏 __linux__ 的值为真，就保留第 9 行代码；如果所有的宏都为假，就保留第 11 行代码。

   ​	这些操作都是在预处理阶段完成的，多余的代码以及所有的宏都不会参与编译，不仅保证了代码的正确性，还减小了编译后文件的体积。

   ​	**这种能够根据不同情况编译不同代码、产生不同目标文件的机制，称为条件编译。**条件编译是预处理程序的功能，不是编译器的功能。

2. `#if`的用法

   1. 格式

      ```c
      #if 整型常量表达式1
          程序段1
      #elif 整型常量表达式2
          程序段2
      #elif 整型常量表达式3
          程序段3
      #else
          程序段4
      #endif
      ```

   2. 解释

      ​	它的意思是：如常“表达式1”的值为真（非0），就对“程序段1”进行编译，否则就计算“表达式2”，结果为真的话就对“程序段2”进行编译，为假的话就继续往下匹配，直到遇到值为真的表达式，或者遇到`#else`。这一点和`if else`非常类似。

   3. 注意

      ​	`#if`命令要求判断条件为“整型常量表达式”，也就是说，表达式中不能包含变量，而且结果必须是整数；而`if`后面的表达式没有限制，只要符合语法就行。这是`#if`和`if`的一个重要区别。

      `#elif`和`#else`也可以省略，如下所示：

      ```c
      #include <stdio.h>
      
      int main()
      {
          #if _WIN32
              printf("This is Windows!\n");
          #else
              printf("Unknown platform!\n");
          #endif
         
          #if __linux__
              printf("This is Linux!\n");
          #endif
      
          return 0;
      }
      ```

3. `#ifdef`的用法

   1. 格式

      ```c
      #ifdef  宏名
          程序段1
      #else
          程序段2
      #endif
      ```

      也可以省略 #else：

      ```c
      #ifdef  宏名
          程序段
      #endif
      ```

   2. 解释

      它的意思是，如果当前的宏已被定义过，则对“程序段1”进行编译，否则对“程序段2”进行编译。

   3. 注意

      VS/VC 有两种编译模式，Debug 和 Release。在学习过程中，我们通常使用 Debug 模式，这样便于程序的调试；而最终发布的程序，要使用 Release 模式，这样编译器会进行很多优化，提高程序运行效率，删除冗余信息。

      为了能够清楚地看到当前程序的编译模式，我们不妨在程序中增加提示，请看下面的代码：

      ```c
      #include <stdio.h>
      #include <stdlib.h>
      int main(){
          #ifdef _DEBUG
              printf("正在使用 Debug 模式编译程序...\n");
          #else
              printf("正在使用 Release 模式编译程序...\n");
          #endif
      
          system("pause");
          return 0;
      }
      ```

      当以 Debug 模式编译程序时，宏 _DEBUG 会被定义，预处器会保留第 5 行代码，删除第 7 行代码。反之会删除第 5 行，保留第 7 行。

4. `#ifndef`的用法

   1. 格式

      ```c
      #ifndef 宏名
          程序段1 
      #else 
          程序段2 
      #endif
      ```

   2. 解释

      它的意思是，如果当前的宏未被定义，则对“程序段1”进行编译，否则对“程序段2”进行编译，这与 #ifdef 的功能正好相反。

5. `#if`、`#ifdef`、`#ifndef`的区别

   `#if`后面跟的是“整型常量表达式”，而`#ifdef`和`#ifndef`后面跟的只能是一个宏名，不能是其他的。

   例如，下面的形式只能用于`#if`：

   ```c
   #include <stdio.h>
   
   #define NUM 10
   
   int main()
   {
       #if NUM == 10 || NUM == 20
           printf("NUM: %d\n", NUM);
       #else
           printf("NUM Error\n");
       #endif
       
       return 0;
   }
   ```

   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\条件编译01.png)

   再如，两个宏都存在时编译代码A，否则编译代码B：

   ```c
   #include <stdio.h>
   
   #define NUM1 10
   #define NUM2 20
   
   int main()
   {
       #if (defined NUM1 && defined NUM2)
           //代码A
           printf("NUM1: %d, NUM2: %d\n", NUM1, NUM2);
       #else
           //代码B
           printf("Error\n");
       #endif
       
       return 0;
   }
   ```

   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\条件编译02.png)

   \#ifdef 可以认为是 #if defined 的缩写。

# typedef关键字

1. C语言不仅提供了丰富的数据类型，而且还允许由用户自己定义类型说明符，也就是说允许由用户为数据类型取“别名”。

2. 格式：` typedef 原类型名 新类型名;`

3. 使用

   1. 基本数据类型

      ```c
      typedef int INTEGER
      INTEGER a; // 等价于 int a;
      ```

      也可以在别名的基础上再起一个别名

      ```c
      typedef int Integer
      
      typedef Integer MyInteger
      ```

   2. 数组类型

      ```c
      typedef char NAME[20]; // 表示NAME是字符数组类型,数组长度为20。然后可用NAME 说明变量,
      NAME a; // 等价于 char a[20];
      ```

   3. 结构体类型

      ```c
      struct Person
      {
      	int age;
      	char *name;
      };
      
      typedef struct Person PersonType;
      ```

      ```c
      typedef struct Person
      {
      	int age;
      	char *name;
      } PersonType;
      ```

      ```c
      typedef struct
      {
      	int age;
      	char *name;
      } PersonType;
      ```

   4. 枚举

      ```c
      enum Sex
      {
      	SexMan,
      	SexWoman,
      	SexOther
      };
      
      typedef enum Sex SexType;
      ```

      ```c
      typedef enum Sex
      {
      	SexMan,
      	SexWoman,
      	SexOther
      } SexType;
      ```

      ```c
      typedef enum
      {
      	SexMan,
      	SexWoman,
      	SexOther
      } SexType;
      ```

   5. 指针

      1. typedef与指向结构体的指针

         ```c
         // 定义一个结构体并起别名
         typedef struct
         {
         	float x;
         	float y;
         } Point;
         
         // 起别名
         typedef Point *PP;
         ```

      2. typedef与指向函数的指针

         ```c
         // 定义一个sum函数，计算a跟b的和
         int sum(int a, int b)
         {
         	int c = a + b;
         	printf("%d + %d = %d", a, b, c);
             
         	return c;
         }
         
         typedef int (*MySum)(int, int);
         // 定义一个指向sum函数的指针变量p
         MySum p = sum;
         
         ```

## 宏与typedef关键字的区别

1. 宏定义只是简单的字符串替换，由预处理器来处理；而`typedef`是在编译阶段由编译器处理的，它并不是简单的字符串替换，而给原有的数据类型起一个新的名字，将它作为一种新的数据类型。

   ```c
   #define PIN1 int *
   typedef int *PIN2;  //也可以写作typedef int (*PIN2);
   ```

   从形式上看这两者相似， 但在实际使用中却不相同。

   下面用 PIN1，PIN2 说明变量时就可以看出它们的区别：

   ```c
   PIN1 a, b;
   ```

   在宏代换后变成：

   ```c
   int * a, b;
   ```

   表示 a 是指向整型的指针变量，而 b 是整型变量。然而：

   ```c
   PIN2 a,b;
   ```

   表示 a、b 都是指向整型的指针变量。因为 PIN2 是一个新的、完整的数据类型。由这个例子可见，**宏定义虽然也可表示数据类型， 但毕竟只是简单的字符串替换。在使用时要格外小心，以避出错。**

2. 可以使用其他类型说明符对宏类型名进行扩展，但对 typedef 所定义的类型名却不能这样做。如下所示：

   ```c
   #define INTERGE int
   unsigned INTERGE n;  //没问题
   
   typedef int INTERGE;
   unsigned INTERGE n;  //错误，不能在 INTERGE 前面添加 unsigned
   ```

3. 在连续定义几个变量的时候，typedef 能够保证定义的所有变量均为同一类型，而 #define 则无法保证。例如：

   ```c
   #define PTR_INT int *
   PTR_INT p1, p2;
   ```

   经过宏替换以后，第二行变为：

   ```c
   int *p1, p2;
   ```

   这使得 p1、p2 成为不同的类型：p1 是指向 int 类型的指针，p2 是 int 类型。

   相反，在下面的代码中：

   ```c
   typedef int * PTR_INT
   PTR_INT p1, p2;
   ```

   p1、p2 类型相同，它们都是指向 int 类型的指针。

4. 示例

   ```c
   typedef char *String;
   int main()
   {
   	String str = "This is a string!";
   	
       return 0;
   }
   
   #define String char *
   int main()
   {
   String str = "This is a string!";
   return 0;
   }
   ```

   ```c
   #include <stdio.h>
   
   typedef char *String1; // 给char *起了个别名String1
   #define String2 char * // 定义了宏String2
   int main()
   {
   	/*
   	只有str1、str2、str3才是指向char类型的指针变量
   	由于String1就是char *，所以上面的两行代码等于:
   	char *str1;
   	char *str2;
   	*/
   	String1 str1, str2;
   	/*
   	宏定义只是简单替换, 所以相当于
   	char *str3, str4;
   	*号只对最近的一个有效, 所以相当于
   	char *str3;
   	char str4;
   	*/
   	String2 str3, str4;
   	
       return 0;
   }
   ```

# const关键字

1. `const`：类型修饰符，使用`const`的变量的值不可改变。我们经常将`const`变量称为常量（constant）。

2. 示例

   ```c
   const int MaxNum = 100;  //班级的最大人数
   ```

   这样`MaxNum`的值就不能被修改了，任何对`MaxNum`赋值的行为都将引发错误：

   ```c
   MaxNum = 90;  //错误，试图向 const 变量写入数据
   ```

3. 格式：`const type name = value;`

   `const`和`type`都是用来修饰变量的，它们的位置可以互换，也就是将`type`放在`const`前面：

   ```c
   type const name = value;
   ```

   但我们通常采用第一种方式，不采用第二种方式。另外建议将常量名的首字母大写，以提醒程序员这是个常量。

4. 注意

   由于常量一旦被创建后其值就不能再改变，所以常量必须在定义的同时赋值（初始化），后面的任何赋值行为都将引发错误。一如既往，初始化常量可以使用任意形式的表达式，如下所示：

   ```c
   #include <stdio.h>
   
   int getNum()
   {
       return 100;
   }
   
   int main()
   {
       int n = 90;
       const int MaxNum1 = getNum();  //运行时初始化
       const int MaxNum2 = n;  //运行时初始化
       const int MaxNum3 = 80;  //编译时初始化
       printf("%d, %d, %d\n", MaxNum1, MaxNum2, MaxNum3);
   
       return 0;
   }
   ```

   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\const01.png)

5. `const`和指针

   `const`也可以和指针变量一起使用，这样可以限制指针变量本身，也可以限制指针指向的数据。`const`和指针一起使用会有几种不同的顺序，如下所示：

   ```c
   const int *p1;
   int const *p2;
   int * const p3;
   ```

   在最后一种情况下，指针是只读的，也就是`p3`本身的值不能被修改；在前面两种情况下，指针所指向的数据是只读的，也就是`p1`、`p2`本身的值可以修改（指向不同的数据），但它们指向的数据不能被修改。

   当然，指针本身和它指向的数据都有可能是只读的，下面的两种写法能够做到这一点：

   ```c
   const int * const p4;
   int const * const p5;
   ```

   `const`和指针结合的写法多少有点让初学者摸不着头脑，大家可以这样来记忆：**`const`离变量名近就是用来修饰指针变量的，离变量名远就是用来修饰指针指向的数据，如果近的和远的都有，那么就同时修饰指针变量以及它指向的数据。**

6. `const`和函数形参

   在C语言中，单独定义`const`变量没有明显的优势，完全可以使用`#define`命令代替。`const`通常用在函数形参中，如果形参是一个指针，为了防止在函数内部修改指针指向的数据，就可以用`const`来限制。

   在C语言标准库中，有很多函数的形参都被`const`限制了，下面是部分函数的原型：

   ```c
   size_t strlen ( const char * str );
   int strcmp ( const char * str1, const char * str2 );
   char * strcat ( char * destination, const char * source );
   char * strcpy ( char * destination, const char * source );
   int system (const char* command);
   int puts ( const char * str );
   int printf ( const char * format, ... );
   ```

   我们自己在定义函数时也可以使用`const`对形参加以限制，例如查找字符串中某个字符出现的次数：

   ```c
   #include <stdio.h>
   #include <string.h>
   
   size_t strnchr(const char *str, char ch)
   {
       int i, n = 0, len = strlen(str);
   
       for(i=0; i<len; i++)
       {
           if(str[i] == ch)
           {
               n++;
           }
       }
      
       return n;
   }
   
   int main()
   {
       char *str = "Hello,World!\\t";
       char ch = 't';
       int n = strnchr(str, ch);
       //strchr() 用于查找字符串中的一个字符，并返回该字符在字符串中第一次出现的位置。
       printf("%d\n", n);
       
       return 0;
   }
   ```

   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\const02.png)

   根据`strnchr()`的功能可以推断，函数内部要对字符串`str`进行遍历，不应该有修改的动作，用`const`加以限制，不但可以防止由于程序员误操作引起的字符串修改，还可以给用户一个提示，函数不会修改你提供的字符串，请你放心。

7. `const`和`const`类型转化

   ​	当一个指针变量`str1`被`const`限制时，并且类似`const char *str1`这种形式，说明指针指向的数据不能被修改；如果将`str1`赋值给另外一个未被`const`修饰的指针变量`str2`，就有可能发生危险。因为通过`str1`不能修改数据，而赋值后通过`str2`能够修改数据了，意义发生了转变，所以编译器不提倡这种行为，会给出错误或警告。

   ​	也就是说，`const char *`和`char *`是不同的类型，不能将`const char *`类型的数据赋值给`char *`类型的变量。但反过来是可以的，编译器允许将`char *`类型的数据赋值给`const char *`类型的变量。

   ​	这种限制很容易理解，`char *`指向的数据有读取和写入权限，而`const char *`指向的数据只有读取权限，降低数据的权限不会带来任何问题，但提升数据的权限就有可能发生危险。

   ​	C语言标准库中很多函数的参数都被`const`限制了，但我们在以前的编码过程中并没有注意这个问题，经常将非`const`类型的数据传递给`const`类型的形参，这样做从未引发任何副作用，原因就是上面讲到的，将非`const`类型转换为`const`类型是允许的。

   下面是一个将 const 类型赋值给非 const 类型的例子：

   ```c
   #include <stdio.h>
   
   void func(char *str){ }
   
   int main()
   {
       const char *str1 = "c.biancheng.net";
       char *str2 = str1;
       func(str1);
       
       return 0;
   }
   ```

   第8、9行代码分别通过赋值、传参（传参的本质也是赋值）将`const`类型的数据交给了非`const`类型的变量，编译器不会容忍这种行为，会给出警告，甚至直接报错。

# 内存管理

1. 变量

   1. 全局变量（外部变量）：出现在代码块`{ }`之外的变量就是全局变量。
   2. 局部变量（自动变量）：一般情况下，代码块`{ }`内部定义的变量就是自动变量，也可使用`auto`显示定义。
   3. 静态变量：是指内存位置在程序执行期间一直不改变的变量，用关键字`static`修饰。代码块内部的静态变量只能被这个代码块内部访问，代码块外部的静态变量只能被定义这个变量的文件访问。

2. 内存四区

   ​	计算机中的内存是分区来管理的，程序和程序之间的内存是独立的，不能互相访问，比如QQ和浏览器分别所占的内存区域是不能相互访问的。而每个程序的内存也是分区管理的，一个应用程序所占的内存可以分为很多个区域，我们需要了解的主要有四个区域，通常叫内存四区，分别为栈区、堆区、静态区、代码区。

   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\内存四区01.jpg)

## 栈内存（stack）

1. 栈区：栈（stack）是一种先进后出的内存结构，所有的自动变量、函数形参都存储在栈中，这个动作由编译器自动完成，我们写程序时不需要考虑。栈区在程序运行期间是可以随时修改的。当一个自动变量超出其作用域时，自动从栈中弹出。

2. 栈区特点

   1. 每个线程都有自己专属的栈；

   2. 栈的最大尺寸固定，超出则引起栈溢出；局部变量过多，过大 或 递归层数太多等就会导致栈溢出；

      ```c
      int ages[10240*10240]; // 程序会崩溃, 栈溢出
      ```

   3. 变量离开作用域后栈上的内存会自动释放。

3. 示例

   ```c
   #include <stdio.h>
   
   int main()
   {
   	// 存储在栈中, 内存地址从大到小
       //也就是说先定义的变量在下面，后定义的变量在上面，所以栈是一种先进后出的结构
   	int a = 10;
   	int b = 20;
   	printf("&a = %p\n", &a);
   	printf("&b = %p\n", &b);
       
   	return 0;
   }
   ```

   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\栈区01.png)
   
   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\栈区02.jpg)
   
   **注：此处只是简单对栈内存进行介绍，具体内容需到学习数据结构时才会进行详尽的介绍。**

## 堆内存（heap）

1. 堆区：堆（heap）和栈一样，也是一种在程序运行过程中可以随时修改的内存区域，但没有栈那样先进后出的顺序。更重要的是堆是一个大容器，它的容量要远远大于栈，这可以解决上面实验三造成的内存溢出困难。一般比较复杂的数据类型都是放在堆中。但是在C语言中，**堆内存空间的申请和释放需要手动通过代码来完成**。

2. 示例

   ```c
   int *p = (int *)malloc(10240 * 1024); // 不一定会崩溃
   ```

   ```c
   #include <stdio.h>
   #include <stdlib.h>
   
   int main()
   {
   	// 存储在栈中, 内存地址从小到大
   	int *p1 = malloc(4);
   	*p1 = 10;
   	int *p2 = malloc(4);
   	*p2 = 20;
   	printf("p1 = %p\n", p1);
   	printf("p2 = %p\n", p2);
       
   	return 0;
   }
   ```

   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\堆区.png)

## malloc函数

1. `malloc`函数

   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\malloc函数01.png)

2. 示例

   ```c
   #include <stdio.h>
   #include <stdlib.h>
   #include <string.h>
   
   int main()
   {
   	/*
   	* malloc
   	* 第一个参数: 需要申请多少个字节空间
   	* 返回值类型: void *
   	*/
   	int *p = (int *)malloc(sizeof(int));
   	printf("p = %i\n", *p); // 保存垃圾数据
   	/*
   	* 第一个参数: 需要初始化的内存地址
   	* 第二个初始: 需要初始化的值
   	* 第三个参数: 需要初始化对少个字节
   	*/
   	memset(p, 0, sizeof(int)); // 对申请的内存空间进行初始化
   	printf("p = %i\n", *p); // 初始化为0
       
   	return 0;
   }
   ```

3. `meset`函数

   1. 每种类型的变量都有各自的初始化方法，`memset()`函数可以说是初始化内存的“万能函数”，通常为新申请的内存进行初始化工作。它是直接操作内存空间，`mem`即“内存”（memory）的意思。

   2. 函数原型：`void *memset(void *s, int c, unsigned long n);`

   3. 函数功能：将指针变量 s 所指向的前 n 字节的内存单元用一个“整数” c 替换，注意 c 是 int 型。s 是`void*`型的指针变量，所以它可以为任何类型的数据进行初始化。

   4. 所在头文件：`string.h`

   5. 注意

      1. `memset()`的作用是在一段内存块中填充某个给定的值。因为它只能填充一个值，所以该函数的初始化为原始初始化，无法将变量初始化为程序中需要的数据。用`memset`初始化完后，后面程序中再向该内存空间中存放需要的数据。

      2. `memset`一般使用“0”初始化内存单元，而且通常是给数组或结构体进行初始化。一般的变量如`char`、`int`、`float`、`double`等类型的变量直接初始化即可，没有必要用`memset`。如果用`memset`的话反而显得麻烦。

      3. 数组也可以直接进行初始化，但`memset`是对较大的数组或结构体进行清零初始化的最快方法，因为它是直接对内存进行操作的。

      4. 字符串数组不是最好用'\0'进行初始化吗？那么可以用`memset`给字符串数组进行初始化吗？也就是说参数 c 可以赋值为'\0'吗？

         ​	可以的。虽然参数 c 要求是一个整数，但是整型和字符型是互通的。但是赋值为 '\0' 和`0`是等价的，因为字符 '\0' 在内存中就是 0。所以在`memset`中初始化为 0 也具有结束标志符 '\0' 的作用，所以通常我们就写“0”。

         ​	`memset`函数的第三个参数 n 的值一般用`sizeof()`获取，这样比较专业。注意，如果是对指针变量所指向的内存单元进行清零初始化，那么一定要先对这个指针变量进行初始化，即一定要先让它指向某个有效的地址。而且用`memset`给指针变量如p所指向的内存单元进行初始化时，n 千万别写成`sizeof(p)`，这是新手经常会犯的错误。因为 p 是指针变量，不管 p 指向什么类型的变量，`sizeof(p)`的值都是 4。

         **C语言中的指针和数组名不完全等价，不能将它们混为一谈。**

   6. 示例

      ```c
      # include <stdio.h>
      # include <string.h>
      
      int main(void)
      {
          int i;  //循环变量
          char str[10];
          char *p = str;
          memset(str, 0, sizeof(str));  //只能写sizeof(str), 不能写sizeof(p)
          for (i=0; i<10; ++i)
          {
              printf("%d\x20", str[i]);
          }
          printf("\n");
          
          return 0;
      }
      ```

      根据`memset`函数的不同，输出结果也不同，分为以下几种情况：
      ```c
      memset(p, 0, sizeof(p)); //地址的大小都是4字节
      0 0 0 0 -52 -52 -52 -52 -52 -52
      
      memset(p, 0, sizeof(*p)); //*p表示的是一个字符变量, 只有一字节
      0 -52 -52 -52 -52 -52 -52 -52 -52 -52
      
      memset(p, 0, sizeof(str));
      0 0 0 0 0 0 0 0 0 0
      
      memset(str, 0, sizeof(str));
      0 0 0 0 0 0 0 0 0 0
      
      memset(p, 0, 10); //直接写10也行, 但不专业
      0 0 0 0 0 0 0 0 0 0
      ```

## free函数

1. 注意

   通过`malloc`申请的存储空间一定要释放, 所以`malloc`和`free`函数总是成对出现

2. `free`函数

   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\free函数01.png)

3. 示例

   ```c
   #include <stdio.h>
   #include <stdlib.h>
   #include <string.h>
   
   int main()
   {
   	// 1.申请4个字节存储空间
   	int *p = (int *)malloc(sizeof(int));
   	// 2.初始化4个字节存储空间为0
   	memset(p, 0, sizeof(int));
   	// 3.释放申请的存储空间
   	free(p);
       
   	return 0;
   }
   ```

## calloc函数

1. `calloc`函数

   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\calloc函数01.png)

2. 示例

   ```c
   #include <stdio.h>
   #include <stdlib.h>
   #include <string.h>
   
   int main()
   {
   	/*
   		// 1.申请3块4个字节存储空间
   		int *p = (int *)malloc(sizeof(int) * 3);
   		// 2.使用申请好的3块存储空间
   		p[0] = 1;
   		p[1] = 3;
   		p[2] = 5;
   		printf("p[0] = %i\n", p[0]);
   		printf("p[1] = %i\n", p[1]);
   		printf("p[2] = %i\n", p[2]);
   		// 3.释放空间
   		free(p);
   	*/
   
       // 1.申请3块4个字节存储空间
   	int *p = calloc(3, sizeof(int));
   	// 2.使用申请好的3块存储空间
   	p[0] = 1;
   	p[1] = 3;
   	p[2] = 5;
   	printf("p[0] = %i\n", p[0]);
   	printf("p[1] = %i\n", p[1]);
   	printf("p[2] = %i\n", p[2]);
       // 3.释放空间
   	free(p);
       
   	return 0;
   }
   
   ```

## realloc函数

1. `realloc`函数

   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\realloc函数01.png)

2. 注意

   * 若参数`ptr`==`NULL`，则该函数等同于`malloc`
   * 返回的指针，可能与`ptr`的值相同，也有可能不同。若相同，则说明在原空间后面申请，否则，则可能后续空间不足，重新申请的新的连续空间，原数据拷贝到新空间， 原有空间自动释放。

3. 示例

   ```c
   #include <stdio.h>
   #include <stdlib.h>
   #include <string.h>
   
   int main()
   {
   	// 1.申请4个字节存储空间
   	int *p = NULL;
   	p = realloc(p, sizeof(int)); // 此时等同于malloc
   	// 2.使用申请好的空间
   	*p = 666;
   	printf("*p = %i\n", *p);
   	// 3.释放空间
   	free(p);
   
       return 0;
   }
   ```

   ```c
   #include <stdio.h>
   #include <stdlib.h>
   #include <string.h>
   
   int main()
   {
       // 1.申请4个字节存储空间
   	int *p = malloc(sizeof(int));
   	printf("p = %p\n", p);
   	// 如果能在传入存储空间地址后面扩容, 返回传入存储空间地址
   	// 如果不能在传入存储空间地址后面扩容, 返回一个新的存储空间地址
   	p = realloc(p, sizeof(int) * 2);
   	printf("p = %p\n", p);
   	// 2.使用申请好的空间
   	*p = 666;
   	printf("*p = %i\n", *p);
   	// 3.释放空间
   	free(p);
   
       return 0;
   }
   ```

# 链表

1. 链表：是一种线性数据结构，其中的每个元素都是一个节点对象，各个节点通过“引用”相连接。引用记录了下一个节点的内存地址，通过它可以从当前节点访问到下一个节点。

2. 链表的设计使得各个节点可以分散存储在内存各处，它们的内存地址无须连续。

3. 链表定义与存储方式

   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\链表01.jpg)

   链表的组成单位是「节点 node」对象。每个节点都包含两项数据：节点的“值”和指向下一节点的“引用”。

   * 链表的首个节点被称为“头节点”，最后一个节点被称为“尾节点”。
   * 尾节点指向的是“空”，它在 Java、C++ 和 Python 中分别被记为 null、nullptr 和 None 。
   * 在 C、C++、Go 和 Rust 等支持指针的语言中，上述“引用”应被替换为“指针”。

## 静态链表

1. 图示

   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\静态链表01.jpg)

2. 示例

   ```c
   #include <stdio.h>
   
   // 1.定义链表节点
   typedef struct node
   {
       //定义节点，存储节点数据
       int data;
       //指向下一节点的指针
       struct node *next;
   }Node;
   
   int main()
   {
       // 2.创建链表节点
       Node a;
       Node b;
       Node c;
       // 3.初始化节点数据
       a.data = 1;
       b.data = 3;
       c.data = 5;
       // 4.链接节点
       a.next = &b;
       b.next = &c;
       c.next = NULL;
       // 5.创建链表头
       Node *head = &a;
       // 6.使用链表
       while(head != NULL)
       {
           int currentData = head->data;
           printf("currentData = %i\n", currentData); 
           head = head->next;
       }
   
       return 0;
   }
   ```

   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\静态变量02.png)

3. 解释

   ​	上面先创建了一个名为`node`的结构体，然后使用`typedef`对结构体类型进行重命名，也就是说`struct node`等价于`Node`。然后结构体`node`里面包含了两个成员，分别为`data`和结构体指针变量`next`。

   - data：用于存放节点数据
   - next：指向下一节点的指针

   ​	然后我们对各节点进行链接。

   * `a.next = &b`：表示节点`a`接下来的节点是`b`
   * `b.next = &c`：表示节点`b`接下来的节点是`c`
   * `c.next = NULL`：表示节点`c`接下来是NULL（空）

   ​	然后我们创建并初始化了节点变量。接下来，我们就要创建链表头，也就是链表的起始点，我们创建了一个结构体指针`head`，这个指针指向第一个节点（当然也可以是其他节点，一般链表头从第一个节点开始）`a`。

   ​	链表的遍历输出就是使用while循环，在循环中，第一次循环，链表头是第一个节点，然后输出当前链表头，然后将链表头指向下一节点，进入下依次循环，当前链表头变为第二个节点，循环往复，直到链表头指向的节点的数据为NULL是，循环结束。

## 动态链表

1. 空链表

   1. 图示

      头指针带了一个空链表节点, 空链表节点中的`next`指向`NULL`

      ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\空链表01.jpg)

   2. 示例

      ```c
      #include <stdio.h>
      #include <stdlib.h>
      
      // 1.定义链表节点
      typedef struct node
      {
      	int data;
      	struct node *next;
      }Node;
      
      int main()
      {
      	Node *head = createList();
          
      	return 0;
      }
      
      // 创建空链表
      Node *createList()
      {
      	// 1.创建一个节点
      	Node *node = (Node *)malloc(sizeof(Node));
      	if(node == NULL)
          {
      		exit(-1);
      	}
      	// 2.设置下一个节点为NULL
      	node->next = NULL;
      	// 3.返回创建好的节点
          
      	return node;
      }
      ```

2. 非空链表

   头指针带了一个非空节点, 最后一个节点中的`next`指向`NULL`

   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\非空链表01.jpg)

3. 动态链表头插法

   1. 步骤

      1. 让新节点的下一个节点等于头结点的下一个节点
      2. 让头节点的下一个节点等于新节点

   2. 示例

      ```c
      #include <stdio.h>
      #include <stdlib.h>
      
      // 1.定义链表节点
      typedef struct node
      {
      	int data;
      	struct node *next;
      }Node;
      
      Node *createList();
      void printNodeList(Node *node);
      
      int main()
      {
      	Node *head = createList();
      	printNodeList(head);
          
      	return 0;
      }
      
      /**
      * @brief createList 创建链表
      * @return 创建好的链表
      */
      Node *createList()
      {
      	// 1.创建头节点
      	Node *head = (Node *)malloc(sizeof(Node));
      	if(head == NULL)
          {
      		return NULL;
      	}
      	head->next = NULL;
      	// 2.接收用户输入数据
      	int num = -1;
      	printf("请输入节点数据\n");
          scanf("%i", &num);
      	// 3.通过循环创建其它节点
      	while(num != -1)
          {
      		// 3.1创建一个新的节点
      		Node *cur = (Node *)malloc(sizeof(Node));
      		cur->data = num;
      		// 3.2让新节点的下一个节点指向头节点的下一个节点
      		cur->next = head->next;
              // 3.3让头节点的下一个节点指向新节点
      		head->next = cur;
      		// 3.4再次接收用户输入数据
      		scanf("%i", &num);
      	}
          
      	// 3.返回创建好的节点
      	return head;
      }
      
      /**
      * @brief printNodeList 遍历链表
      * @param node 链表指针头
      */
      void printNodeList(Node *node)
      {
      	Node *head = node->next;
      	while(head != NULL)
          {
      		int currentData = head->data;
      		printf("currentData = %i\n", currentData);
      		head = head->next;
      	}
      }
      ```

      

4. 动态链表尾插法

## 链表优化

## 链表销毁

## 链表长度计算

## 链表查找

## 链表删除

# 计数排序

1. 计数排序：是一个非基于比较的排序算法，该算法于1954年由 Harold H. Seward 提出。它的优势在于在**对一定范围内的整数**排序时，快于任何比较排序算法。

2. 排序思路

   1. 找出待排序数组最大值，确定排序数组的索引值
   2. 定义一个索引最大值为待排序数组最大值的数组
   3. 遍历待排序数组，将待排序数组中每个数字出现的次数存储在排序数组中
   4. 整理排序数组中的数字，如果排序数组的值不为零，输出对应的下标值
   5. 最后将索引值输出即为排序结果

3. 解释

   ![](D:\Programmering Learning\Markdown文档\C语言教程\动画\countingSort.gif)

4. 示例

   ```c
   #include <stdio.h>
   
   void CountingSort(int length,int OriginalArray[length]);
   void PrintArray(int length,int OriginalArray[length]);
   
   int main()
   {
       //创建待排序数组
       int length;
       printf("请输入待排序数组长度：");
       scanf("%d",&length);
       int OriginalArray[length];
   
       //初始化待排序数组
       printf("请输入待排序数组元素：");
       for(int i = 0;i < length;i++)
       {
           scanf("%d",&OriginalArray[i]);
       }
   
       //调用排序函数对待排序数组进行排序
       CountingSort(length,OriginalArray);
   
       //打印结果
       PrintArray(length,OriginalArray);
   
       return 0;
   }
   
   //排序函数
   void CountingSort(int length,int OriginalArray[length])
   {
       //寻找待排序数组最大值
       int max = OriginalArray[0];
       for(int i =1;i < length;i++)
       {
           if(OriginalArray[i] > max)
           {
               max = OriginalArray[i];
           }
       }
   
       //创建排序数组
       int SortArray[max + 1];
   
       //初始化排序数组
       for(int i = 0;i <= max;i++)
       {
           SortArray[i] = 0;
       }
   
       //统计待排序数组每个数字出现的次数
       for(int i = 0;i < length;i++)
       {
           SortArray[OriginalArray[i]]++;
       }
   
       //整理排序数组
       int index = 0;
       int AuxiliaryArray[length];
       for(int i = 0;i <= max;i++)
       {
           while(SortArray[i] > 0)
           {
               AuxiliaryArray[index] = i;
               index++;
               SortArray[i]--;
           }
       }
   
       //将排序结果返回待排序数组
       for(int i = 0;i < length;i++)
       {
           OriginalArray[i] = AuxiliaryArray[i];
       }
   }
   
   //打印结果
   void PrintArray(int length,int OriginalArray[length])
   {
       for(int i = 0;i < length;i++)
       {
           printf("%d ",OriginalArray[i]);
       }
   }
   ```

   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\计数排序01.png)

5. 练习

   输入90到100以内的5个数，优化计数排序，避免资源浪费

   ```c
   #include <stdio.h>
   
   void CountingSort(int length,int OriginalArray[length]);
   void PrintSort(int length,int OriginalSort[length]);
   
   int main()
   {
       //定义待排序数组
       int length;
       printf("请输入待排序数组长度:");
       scanf("%d",&length);
       int OriginalArray[length];
   
       //初始化待排序数组
       printf("请输入待排序数组元素：");
       for(int i = 0;i < length;i++)
       {
           scanf("%d",&OriginalArray[i]);
       }
   
       //调用函数
       CountingSort(length,OriginalArray);
   
       //打印结果
       PrintSort(length,OriginalArray);
   
       return 0;
   }
   
   //排序算法
   void CountingSort(int length,int OriginalArray[length])
   {
       //寻找待排序数组最大最小值
       int max = OriginalArray[0];
       int min = OriginalArray[0];
       for(int i = 1;i < length;i++)
       {
           if(OriginalArray[i] > max)
           {
               max = OriginalArray[i];
           }
           if(OriginalArray[i] < min)
           {
               min = OriginalArray[i];
           }
       }
   
       //定义计数数组
       int size = max -  min + 1;
       //int maximum = max - min;
       int SortArray[size];
   
       //初始化计数数组
       for(int i = 0;i < size;i++)
       {
           SortArray[i] = 0;
       }
   
       //统计待排序数组每个元素出现次数
       for(int i = 0;i < length;i++)
       {
           SortArray[OriginalArray[i] - min]++;
       }
   
       //整理计数数组
       int index = 0;
       int AuxiliaryArray[length];
       for(int i = 0;i < size;i++)
       {
           while(SortArray[i] > 0)
           {
               AuxiliaryArray[index] = i + min;
               index++;
               SortArray[i]--;
           }
       }
   
       //将排序结果返回待排序数组
       for(int i = 0;i < length;i++)
       {
           OriginalArray[i] = AuxiliaryArray[i];
       }
   }
   
   //打印结果
   void PrintSort(int length,int OriginalSort[length])
   {
       for(int i = 0;i < length;i++)
       {
           printf("%d ",OriginalSort[i]);
       }
   }
   ```

# 选择排序

1. 原理：先寻找待排序数组中的最小值，放在第一位，然后寻找剩下的数字中的最小值，放在第二位，以此类推，直到排序完成。

2. 排序思路

   1. 利用第0个元素和后面的元素依次进行对比
   2. 判断第0个元素是否大于当前被比较元素, 一旦小于就交换位置
   3. 第0个元素和后续所有元素比较完成后, 第0个元素就是最小值
   4. 排除第0个元素, 用第1个元素重复1~3操作, 比较完成后第1个元素就是倒数第二小的值
   5. 以此类推, 直到当前元素没有可比较的元素, 排序完成

3. 解释

   ![](D:\Programmering Learning\Markdown文档\C语言教程\动画\selectionSort.gif)

4. 示例

   ```C
   #include <stdio.h>
   
   void SelectSort(int length,int OriginalArray[length]);
   void PrintArray(int length,int OriginalArray[length]);
   
   int main()
   {
       //定义待排序数组
       int length;
       printf("请输入待排序数组长度：");
       scanf("%d",&length);
       int OriginalArray[length];
   
       //初始化待排序数组
       printf("请输入待排序数组元素：");
       for(int i = 0;i < length;i++)
       {
           scanf("%d",&OriginalArray[i]);
       }
   
       //调用排序函数
       SelectSort(length,OriginalArray);
   
       //打印结果
       PrintArray(length,OriginalArray);
   
       return 0;
   }
   
   //排序函数
   void SelectSort(int length,int OriginalArray[length])
   {
       for(int i = 0;i < length;i++)
       {
           for(int j = i;j < length - 1;j++)
           //j < length - 1的原因：最后一位数不用做比较，如果继续拿着最后一位数与后面的术进行比较，一来是后面没有数字，二来是会造成数组越界
           {
               if(OriginalArray[i] > OriginalArray[j + 1])
               {
                   int temp = OriginalArray[j + 1];
                   OriginalArray[j + 1] = OriginalArray[i];
                   OriginalArray[i] = temp;
               }
           }
       }
   }
   
   //打印结果
   void PrintArray(int length,int OriginalArray[length])
   {
       for(int i = 0;i < length;i++)
       {
           printf("%d ",OriginalArray[i]);
       }
   }
   ```

   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\选择排序.png)

# 冒泡排序

1. 冒泡排序：是一种简单直观的排序算法。它重复地走访过要排序的数列，一次比较两个元素，如果他们的顺序错误就把他们交换过来。走访数列的工作是重复地进行直到没有再需要交换，也就是说该数列已经排序完成。这个算法的名字由来是因为越小的元素会经由交换慢慢"浮"到数列的顶端。

2. 冒泡排序

   1. 比较相邻的元素。如果第一个比第二个大，就交换他们两个。

   2. 对每一对相邻元素作同样的工作，从开始第一对到结尾的最后一对。这步做完后，最后的元素会是最大的数。

   3. 针对所有的元素重复以上的步骤，除了最后一个。

   4. 持续每次对越来越少的元素重复上面的步骤，直到没有任何一对数字需要比较。

3. 解释

   ![](D:\Programmering Learning\Markdown文档\C语言教程\动画\bubbleSort.gif)

4. 示例

   ```c
   #include <stdio.h>
   
   void BubbleSort(int length,int OriginalArray[length]);
   void PrintArray(int length,int OriginalArray[length]);
   
   int main()
   {
       //创建待排序数组
       int length;
       printf("请输入待排序数组长度：");
       scanf("%d",&length);
       int OriginalArray[length];
   
       //初始化待排序数组
       printf("请输入待排序数组元素：");
       for(int i = 0; i < length;i++)
       {
           scanf("%d",&OriginalArray[i]);
       }
   
       //调用排序函数
       BubbleSort(length,OriginalArray);
   
       //打印结果
       PrintArray(length,OriginalArray);
   
       return 0;
   }
   
   //排序函数
   void BubbleSort(int length,int OriginalArray[length])
   {
       for(int i = 0;i < length;i++)
       {
           for(int j = 0;j < length - 1 -i;j++)
           {
               if(OriginalArray[j] > OriginalArray[j + 1])
               {
                   int temp = OriginalArray[j];
                   OriginalArray[j] = OriginalArray[j + 1];
                   OriginalArray[j + 1] = temp;
               }
               
           }    
       }
   }
   
   //打印结果
   void PrintArray(int length,int OriginalArray[length])
   {
       for(int i = 0;i < length;i++)
       {
           printf("%d ",OriginalArray[i]);
       }
   }
   ```

5. 计数排序与冒泡排序的区别

   乍一看，两种排序算法的代码貌似都一样，但是从原理上我们也知道，两者不一样，区别就在于选择排序是找最小值，而冒泡排序是比较相邻两数字的大小。

   ![](D:\Programmering Learning\Markdown文档\C语言教程\图片\冒泡排序与选择排序的区别.png)

# 插入排序

1. 插入排序：是一种最简单直观的排序算法，它的工作原理是通过构建有序序列，对于未排序数据，在已排序序列中从后向前扫描，找到相应位置并插入。

2. 算法步骤

   1. 将第一待排序序列第一个元素看做一个有序序列，把第二个元素到最后一个元素当成是未排序序列。
   2. 从头到尾依次扫描未排序序列，将扫描到的每个元素插入有序序列的适当位置。（如果待插入的元素与有序序列中的某个元素相等，则将待插入元素插入到相等元素的后面。）

3. 解释

   ![](D:\Programmering Learning\Markdown文档\C语言教程\动画\insertionSort.gif)

4. 示例

   ```c
   #include <stdio.h>
   
   void InsertionSort(int length,int OriginalArray[length]);
   void PrintReasult(int length,int OriginalArray[length]);
   
   int main()
   {
       //创建待排序数组
       int length;
       printf("请输入待排序数组长度：");
       scanf("%d",&length);
       int OriginalArray[length];
   
       //初始化待排序数组
       printf("请输入待排序数组元素：");
       for(int i = 0;i < length;i++)
       {
           scanf("%d",&OriginalArray[i]);
       }
   
       //调用排序函数
       InsertionSort(length,OriginalArray);
   
       //打印结果
       PrintReasult(length,OriginalArray);
   
       return 0;
   }
   
   //排序函数
   void InsertionSort(int length,int OriginalArray[length])
   {
       int key;
       for(int i = 1;i < length;i++)
       {
           key = OriginalArray[i];
           int j = i - 1;
           while((j >= 0) && (OriginalArray[j] > key))
           {
               OriginalArray[j + 1] = OriginalArray[j];
               j--;
           }
           OriginalArray[j + 1] = key;
       }
   }
   
   //打印结果
   void PrintReasult(int length,int OriginalArray[length])
   {
       for(int i = 0;i < length;i++)
       {
           printf("%d ",OriginalArray[i]);
       }
   }
   ```

# 折半查找

1. 折半查找：又名二分查找，在某些情况下相比于顺序查找，使用折半查找算法的效率更高。但是该算法的使用的前提是静态查找表中的数据必须是有序的。
2. 

## 进制转换（查表法）

# 希尔排序

1. 希尔排序:也称递减增量排序算法，是插入排序的一种更高效的改进版本。但希尔排序是非稳定排序算法。

2. 希尔排序是基于插入排序的以下两点性质而提出改进方法的：

   1. 插入排序在对几乎已经排好序的数据操作时，效率高，即可以达到线性排序的效率；
   2. 但插入排序一般来说是低效的，因为插入排序每次只能将数据移动一位。

3. 基本思想

   先将整个待排序的记录序列分割成为若干子序列分别进行直接插入排序，待整个序列中的记录"基本有序"时，再对全体记录进行依次直接插入排序。

4. 算法步骤

   1. 选择一个增量序列 t1，t2，……，tk，其中 ti > tj, tk = 1；

   2. 按增量序列个数 k，对序列进行 k 趟排序；
   3. 每趟排序，根据对应的增量 ti，将待排序列分割成若干长度为 m 的子序列，分别对各子表进行直接插入排序。仅增量因子为 1 时，整个序列作为一个表来处理，表长度即为整个序列的长度。

5. 解释

   ![](D:\Programmering Learning\Markdown文档\C语言教程\动画\Sorting_shellsort_anim.gif)

6. 示例

   ```c
   #include <stdio.h>
   
   void ShellSort(int length,int OriginalArray[length]);
   void PrintReasult(int length,int OriginalArray[length]);
   
   int main()
   {
       //创建待排序数组
       int length;
       printf("请输入待排序数组的长度：");
       scanf("%d",&length);
       int OrigianlArray[length];
   
       //初始化待排序数组
       printf("请输入待排序数组元素：");
       for(int i = 0;i < length;i++)
       {
           scanf("%d",&OrigianlArray[i]);
       }
   
       //调用排序函数
       ShellSort(length,OrigianlArray);
   
       //打印结果
       PrintReasult(length,OrigianlArray);
   
       return 0;
   }
   
   //排序函数
   void ShellSort(int length,int OriginalArray[length])
   {
       int temp;
       for(int gap = length >> 1;gap > 0;gap >>= 1)
       {
           for(int i = gap;i < length;i++)
           {
               temp = OriginalArray[i];
               int j;
               for(j = i - gap;j >= 0 && OriginalArray[j] > temp;j -= gap)
               {
                   OriginalArray[j + gap] = OriginalArray[j];
               }
               OriginalArray[j + gap] = temp;
           }
       }
   }
   
   //打印结果
   void PrintReasult(int length,int OriginalArray[length])
   {
       for(int i = 0;i < length;i++)
       {
           printf("%d ",OriginalArray[i]);
       }
   }
   ```

# 文件

## 文件的打开与关闭

## 一次读写一个字符

## 一次读写一行字符

## 一次读写一块数据

## 读写结构体

## 其他文件操作函数

# C标准库
