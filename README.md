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
        public string name;
        public string addr;
        public long PhoneNum;
        public long FaxNum;
        public string website;
        public string MangName;
        public string MangSurame;
        public long MangPhone;

        public void details()
        {
            Console.WriteLine($" \n\t\t\t Hello! \n\n \t welcome to {name} the biggest technology company in the middle east\n\n" +
                $"  if you want to enrole in {name} you can conatct us via : \n\n" +
                $"  Number : {PhoneNum}\n" +
                $"  Fax Number : {FaxNum}\n" +
                $"  or visit our website : {website}\n" +
                $"  And you can head to our headquarter in \" {addr} \"\n\n " +
                $"\t\t\t\t\t\t The Manger / prof.eng.mr {MangName} {MangSurame} \n" +
                $"\t\t\t\t\t\t {MangPhone}");


           
        }
       
    }

    internal class Program
    {

       
      


        static void Main(string[] args)
        {
           
            company Company1 = new company();
            Console.Write($" Company name : ");  Company1.name = read();
            Console.Write($" Company address : "); Company1.addr = read();
            Console.Write($" Company phone number : ");  Company1.PhoneNum = long.Parse (read());
            Console.Write($" Company fax number : ");  Company1.FaxNum = long.Parse(read());
            Console.Write($" Company website : "); Company1.website = read();
            Console.Write($" manger first name : "); Company1.MangName = read();
            Console.Write($" manger last name : "); Company1.MangSurame = read();
            Console.Write($" manger phone number : "); Company1.MangPhone = long.Parse(read()) ;
            Company1.details();


      
        }
        static string read()
        {
            return Console.ReadLine();
        }
      
    }
}

 ```
 
 ### Output
 ![image](https://user-images.githubusercontent.com/116801554/198300952-4b899f63-89a7-4a3d-b879-f2766df4e20f.png)

 
 
