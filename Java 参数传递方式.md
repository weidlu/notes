# Java的值传递方式

## 简介
一般来说，值传递有两种方式。其实还有第三种，不过这一种已经很少使用了
* 按值传递(call by value)
* 按引用传递(call by reference)
* ~~按名字传递(call by name)~~

按值传递的就是接收的是调用者传过来的值
按引用传递接受的是传递过来的一个对象的引用，或者说，是传递了一个对象的地址。

那么我们是知道的，Java只有按值传递。

```java
  public static void tripleValue(double x){
        x = x * 3;
    }
    
    double percent = 10;
    tripleValue(percent);
```
以上代码是不会改变``perecent``的值的，原因如下图所示：
![tp](D:\Users\wdlu\Pictures)
