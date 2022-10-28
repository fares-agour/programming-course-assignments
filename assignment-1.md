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
### Output

![image](https://user-images.githubusercontent.com/116801554/198266588-f880d8f7-7bbb-429a-8751-4fed37725781.png)

___________________________________________________________________________

## TASK B

Write a program that reads the raduis of circle and prints its perimeter and area.

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
         
            Console.Write(" raduis = ");
            double raduis = double.Parse(Console.ReadLine());
            Console.WriteLine($"the perimeter =  {raduis * 3.142 * 2}");
            Console.WriteLine($"and its area =  {raduis * 3.142 * raduis}");

        }
    }
}
 

```
 ### Output
 ![image](https://user-images.githubusercontent.com/116801554/198271198-30c26489-d6f0-486f-a81f-f1c8ccf07e25.png)
 ____________________________________________________________________________
 ## TASK C
 Write a program that reads information about the company and its manager and then prints it.


### code section
``` C#
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace assignments
{
    class company
    {
      public string[] det = new string[8];
       public void details()
       {
        Console.WriteLine($" \n\t\t\t Hello! \n\n \t welcome to {det[0]} the biggest technology company in the middle east\n\n" +
                $"  if you want to enrole in {det[0]} you can conatct us via : \n\n" +
                $"  Number : {det[2]}\n" +
                $"  Fax Number : {det[3]}\n" +
                $"  or visit our website : {det[4]}\n" +
                $"  And you can head to our headquarter in \" {det[1]} \"\n\n " +
                $"\t\t\t\t\t\t The Manger / prof.eng.mr {det[5]} {det[6]} \n" +
                $"\t\t\t\t\t\t {det[7]}");
        }

    }

    internal class Program
    {
        static void Main(string[] args)
        {

             string[] info = { " Company name : ", " Company address : ", " Company phone number : ",
             " Company fax number : ", " Company website : ", " manger first name : "
                    , " manger last name : "," manger phone number : " };

             company company = new company();

             for (int i =0; i< info.Length; i++)
             {
                print(info[i]);

                 company.det[i] = read();
             }
              company.details();
        }

        static string read()
        {
            return Console.ReadLine();
        }
        static void print(string a)
        {
             Console.Write(a);
        }

    }
}

 ```
 
 ### Output
 ![image](https://user-images.githubusercontent.com/116801554/198300952-4b899f63-89a7-4a3d-b879-f2766df4e20f.png)

 
 
