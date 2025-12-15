```
using System;
class SecondLargest
{
    static void Main(string[] args)
    {
        int size = int.Parse(Console.ReadLine());
        int[] arr = new int[size];
        
        for(int i = 0 ; i < arr.Length ; i++)
        {
            arr[i] = int.Parse(Console.ReadLine());
        }
        
        int largest = arr[0];
        int secondLargest = arr[0];
        for(int i = 1 ; i < arr.Length ; i++)
        {
            if(arr[i] > largest)
            {
                secondLargest = largest;
                largest = arr[i];
            }
            else if(arr[i] > secondLargest && arr[i] < largest)
            {
                secondLargest = arr[i];
            }
        }
        
        Console.WriteLine(secondLargest);
    }
}
```
