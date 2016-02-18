# 1.关键字及注释


###前言
Java中[环境变量的配置](http://www.cnblogs.com/linjiqin/archive/2013/11/02/3403095.html)以及对JDK的我就不做过多的赘述，直接进入主题.

###1.1 关键字和标识符

关键字：赋予了特殊含义的单词，比如class之类的特殊含义的单词。
标识符：在程序中定义的一些名称，比如类名，main也是，其只能有a-z,0-9,__, **$**，并且不可以用数字开头，不可以使用关键字，class _以及class **$**都是正确的。

+ 类名必须要大写，这是规范

###1.2 注释

```java
/**
@author
@thomas
*/
/*注释：注解说明解释程序的文字
作用是对程序进行说明
*/
class Demo  //这是我的第一个小程序
{
    public static void main (String[] args)
    {
        System.out.println("Hello World");
    }
}
```
注释：注解说明解释程序的文字,有以上三种注释方法。
作用:1.是对程序进行说明； 2.调试程序；
注意事项：单行注释里面可以有单行注释；多行注释里面也可以有单行注释；但是多行注释里面不能嵌套多行注释。

+ 在写程序之前先写下类似如下的开头程序

```java

/**
需求：写一个helloworld程序，将helloworld字样写在屏幕上
思路: 1.找个编译器
      2.用Java语言写个程序
      3.这个程序需要运行，并具备显示的功能
      
步骤：1.定义一个类，通过class完成
      2.让这个类运行，并具备显示的功能
      3。显示功能可以通过输出语句实现

代码：
    测试： javac java
*/
//1.用 class定义类
class Demo 
{
    //2.类中定义主方法
    public static void main(String[] args)
    {
        //3.主方法定义输出语句
        System.out.println("hello world");
    }
}
```
        
        
        
        
        
        
        
        