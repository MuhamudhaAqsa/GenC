```
using System;
class Fibonacci
{
    static void Main(string[] args)
    {
        int n = int.Parse(Console.ReadLine());
        int ans = fibo(n);
        Console.WriteLine(ans);
    }
    
    static int fibo(int n)
    {
        if(n == 0 || n == 1)
        {
            return n;
        }
        return fibo(n - 2) + fibo(n - 1); 
    }
}
```
