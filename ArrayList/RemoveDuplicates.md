```
using System;
using System.Collections.Generic;
class RemoveDuplicates
{
    static void Main(string[] args)
    {
        int n = int.Parse(Console.ReadLine());
        int[] arr = new int[n];
        for(int i = 0 ; i < arr.Length ; i++)
        {
            arr[i] = int.Parse(Console.ReadLine());
        }
        List<int> list = new List<int>();
        
        for(int i = 0 ; i < arr.Length ; i++)
        {
            int num = arr[i];
            if(!list.Contains(num))
            {
               list.Add(num); 
            }
        }
        
        for(int i = 0 ; i < list.Count ; i++)
        {
            Console.Write(list[i] + " ");
        }
```
        
        
    }
}
