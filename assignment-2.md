# Assignment 2

## TASK A

Write a program that print the following pattern.
```
   *******
    *****
     ***
      *
  ```    
### Code section 
```C#
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
            Console.Write("enter your width \"odd\" : ");
            int x = int.Parse(Console.ReadLine());
            Console.WriteLine();
         for (int i =1; i <= x ; i+=2)
            {
                for (int j = 0; j < (i-1)/2; j++)
                    Console.Write(" ");

                for (int j = 0; j <=x-i; j++)
                    Console.Write("*");
                Console.WriteLine();
                       
            }
        }

    }
}
```

### Output
![image](https://user-images.githubusercontent.com/116801554/198554269-f12645b8-be4d-4918-af25-e193b5ccfc4a.png)
