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
```


### 3.2 字符类型运算

```java
class VarDemo2
{
    public static void main(String[] agrs)
    {
        System.out.println();
    }
}

```