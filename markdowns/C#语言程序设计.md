# C#语言程序设计

![CSharp](./pictures/CSharp.png)

## 一、C#基础语法

### 1.Hello,World！

```c#
using System;//System是一个命名空间，using关键字用于引入命名空间

namespace HelloWorld//命名空间，用于对代码进行分类
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Hello World!");
            // Console.WriteLine("Hello World! 自动换行");
            // Console.Write("Hello World! 不自动换行");
        }
    }
}
//单行注释
/*
  多行注释
*/
```
> 程序的基本要点总结
* 注释快捷键
  * 注释所选行：Ctrl+k Ctrl+c
  * 对所选行解除注释：Ctrl+k Ctrl+u
  * 多行注释不可嵌套
* 一般一行放一条语句，也可以多条语句放在同一行，但是无论如何，在每条语句末尾都必须加上英文分号
* Main()方法是程序执行的入口
  * 不可改名
  * 必须是static void修饰的
> C#的编译过程
* C#源代码被编译成**符合CLI规范的中间语言（IL）**
* IL代码和资源被存储在**程序集**（通常为.dll，包含一个介绍程序集的类型、版本和区域性的清单）中
* 程序集在程序运行的时候才会被加载到CLR中进行**JIT实时编译**，将JIL代码转换成本机的机器指令
* 其中CLR（公共语言运行时）是Microsoft对CLI（公共语言基础结构）国际标准的实现，CLI是创建执行和开发环境的基础，语言和库可以在其中无缝地协同工作

### 2.类型系统

#### （1）值类型

> 简单类型
* 有符号整型：sbyte、short、int、long
* 无符号整型：byte、ushort、uint、ulong
* Unicode字符：char
* IEEE二进制浮点：float、double
* 高精度十进制浮点数：decimal
* 布尔类型：bool（只能为 **true** 或 **false**）
> 枚举类型
* 格式：enum E {...}
> 结构类型
* 格式：struct S {...}
> 元组值类型
* 格式：(T1,T2,...)

#### （2）引用类型

### 3.变量与常量

#### （1）变量的声明和赋值

```c#
//变量的声明
int age;
double length;

//变量的赋值
age = 21;
length = 18.4;

//输出变量的值
Console.WriteLine(age);
Console.WriteLine(length);
```
> 变量的命名规则
* 由a-z、A-Z、数字和下划线组成
* 不能以数字开头
* C#严格区分大小写
> 注意事项
* 变量必须先声明再使用，局部变量又要求先初始化再使用
* 变量的命名应当尽量保证 “见名知义”
* 某个类型的变量只能存储对应类型的数据
* 赋值号左边**只能是变量、属性或索引器**，不可以是表达式
* 同一个变量，多次赋值，**只会保留最后一次赋值的数据**，之前的都会被覆盖掉

#### （2）常量的使用

|运算转义序列| 含义          |
|-----------|--------------|
|   \\\     | \\字符        |
|   \\'     | '字符         |
|   \\n     | 换行符        |
|   \\r     | 回车，但不换行 |
|   \\t     | 水平制表符     |
|   \\v     | 垂直制表符     |
|   \\a     | Alert或Bell，操作系统会有提示音|




## 二、C#面向对象
## 三、C#高级编程