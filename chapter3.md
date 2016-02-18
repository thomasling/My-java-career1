# 类型提升与强制转换

### 3.1 数值类型提升和转换

```java
class VarDemo2
{
    public static void main (String[] args)
    {
        int x=3;
        x=x+3; //一啊不能情况下，运算两端只有是同一种数据类型才可以运算
    
        byte b=5;
        x=x+b; //四个八位和一个八位运算，占用内存较小的就会有一个类型提升
    
        byte b=3;
        b=b+4;//会出现丢失精度的结果，因为4是int型，占4个字节因此运算结果也是占四个字节的；
    
        b=(byte)(b+4);//做强制类型转换，这里的转换就是只去最后一个字节的数值，因此如果最前面是1，结果是负数
    
    
    
    System.out.println();
    }
}
```


### 3.2 字符类型运算
* [编码表](http://www.dreamdu.com/xhtml/ascii/)

```java
class VarDemo2
{
    public static void main(String[] agrs)
    {
        System.out.println('a'+1); //根据编码表,a字符对应的是96所以计算结果是97
        
        byte b=4; //4是一个int类型，但是在这句里会检查4是否在byte的精度内，如果在这个精度内就会一个数据类型的转换
        //b=3+7; //运行正常
        byte b1=3;
        byte b2=7;
        b=b1+b2; //显示精度错误，因为b1,b2都是变量所以系统不能检查不确定是否在精度内，所以显示精度错误
        
        int x;
        int x1=100;
        int x2=333;
        x=x1+x2; //这个却不会报错，因为int是数据的默认类型，如果超出了范围，高位全都舍弃，所以可能会出现负数的情况。
        
    }
}

```