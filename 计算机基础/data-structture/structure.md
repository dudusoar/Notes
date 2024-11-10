# 结构体

C语言中结构体的定义方法是：先在struct这个关键词后面接上结构体的名字（也被称作是结构体的标签）​，然后在名字后面接上用“{”和“}”括起来的程序块，并在程序块中列出若干个数据项。

一旦定义完结构体，就可以把结构体当作是一种数据类型，用它来定义变量。

被汇集到结构体中的每个数据项都被称作“结构体的成员”​。

```csharp
public struct Point
{
    public int X { get; set; }
    public int Y { get; set; }

    // 自定义的有参构造函数
    public Point(int x, int y)
    {
        X = x;
        Y = y;
    }

    // 方法示例
    public double DistanceFromOrigin()
    {
        return Math.Sqrt(X * X + Y * Y);
    }
}

```
