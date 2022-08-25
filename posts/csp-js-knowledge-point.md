[←返回主页](https://blog.jnw031.ga)

## <center>大 O 时间复杂度表示法</center>

### O(1)

> 常数阶。

```cpp
int x=91;
int y=100;
while(y>0)
{
    if(x>100)
    {
       x=x-10;
       y--;
    }
    else
    {
        x++;
    }
}
```

因为整个程序和 $n$ 没有关系，所以被称为常数阶，$O(1)$。

### O(n)