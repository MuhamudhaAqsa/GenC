```
using System;
class CountVowels
{
    static void Main(string[] args)
    {
        string sentence = Console.ReadLine();
        int count = 0;
        for(int i = 0 ; i < sentence.Length ; i++)
        {
            if(sentence[i] == 'a' || sentence[i] == 'e' || sentence[i] == 'i' || sentence[i] == 'o' || sentence[i] == 'u' || sentence[i] == 'A' || sentence[i] == 'E' || 
            sentence[i] == 'I' || sentence[i] == 'O' || sentence[i] == 'U')
            {
               count = count + 1; 
            }
        }
        Console.WriteLine(count);
    }
}
```
