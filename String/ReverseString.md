```
using System;
class ReverseString
{
    static void Main(String[] args)
    {
        string sentence = Console.ReadLine();
        string rev = "";
        for(int i = sentence.Length - 1 ; i >= 0 ; i--)
        {
            rev = rev + sentence[i];
        }
        Console.WriteLine(rev);
    }
}
```
