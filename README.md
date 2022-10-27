# Assignment 1

## TASK A

Write a program that reads from console three number of type int and print their sum.

### Code section

``` C#
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace assignments
{
    internal class Program
    {
        static void Main(string[] args)
        {
            int a = int.Parse(Console.ReadLine());
            int b = int.Parse(Console.ReadLine());
            int c = int.Parse(Console.ReadLine());
            Console.WriteLine($"the sum of 3 numbers = {a + b + c}");
        }
    }
}


```
## Output

![image](https://user-images.githubusercontent.com/116801554/198266588-f880d8f7-7bbb-429a-8751-4fed37725781.png)


