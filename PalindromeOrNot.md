```
using System;
class PalindromeOrNot
{
    static void Main(string[] args)
    {
        string sentence = Console.ReadLine();
        sentence = sentence.ToLower();
        bool isPalindrome = true;
        int l = 0;
        int r = sentence.Length - 1;
        while(l <= r)
        {
            if(sentence[l] == sentence[r])
            {
                l = l + 1;
                r = r - 1;
            }
            else
            {
                isPalindrome = false;
                break;
            }
        }
        
        if(isPalindrome == true)
        {
        Console.WriteLine("Palindrome");
        }
        else
        {
            Console.WriteLine("Not a Palindrome");
        }
        
        
    }
}
```
