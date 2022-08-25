<head>
    <script src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
    <script type="text/x-mathjax-config">
        MathJax.Hub.Config({
            tex2jax: {
            skipTags: ['script', 'noscript', 'style', 'textarea', 'pre'],
            inlineMath: [['$','$']]
            }
        });
    </script>
</head>

[←返回主页](https://blog.jnw031.ga)

## <center>大 $O$ 时间复杂度表示法</center>

---

### $O(1)$

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

### $O(n)$

> 一次阶。时间和规模 $n$ 成一阶线性关系。

```cpp
int n;
cin>>n;
while(n--)
{
    cout<<n;
}
```

### $O(n^3)$

> 三阶线性关系。( $n$ 阶以此类推。)

```cpp
int total=0;
int n;
cin>>n;
for(int i=0;i!=n;i++)
{
    for(int j=0;j!=i;j++)
    {
        for(int k=0;j!=j;k++)
        {
            total++;
        }
    }
}
```

[原](https://blog.csdn.net/stary_yan/article/details/51383480)

## 后缀表达式法

括号法。

