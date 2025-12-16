```
using System;
using System.Collections.Generic;
class CharacterFrequency
{
    static void Main(string[] args)
    {
        string s = Console.ReadLine();
        Dictionary<char, int> freq = new Dictionary<char, int>();
        for(int i = 0 ; i < s.Length ; i++)
        {
            char ch = s[i];
            if(!freq.ContainsKey(ch))
            {
                freq.Add(ch, 1);
            }
            else
            {
                freq[ch] = freq[ch] + 1;
            }
        }
        
        //Printing using foreach loop
        foreach(var item in freq)
        {
            Console.WriteLine(item.Key + ":" + item.Value);
        }
    }
}
```
