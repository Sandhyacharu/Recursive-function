# Recursive-function

## Aim: To write a C# program to reverse a number using recursive function.

## Algorithm:

## Program:
```python
using System;

namespace Recursive_Function
{
    class Program
    {
        public static int m, reverse = 0;
        public static int Recur(int number)
        {
            
            if (number > 0)
            {
                Program.m = number % 10;
                Program.reverse = Program.reverse * 10 + m;
                number = number / 10;
                return Recur(number);
            }
            return Program.reverse;

        }
        static void Main(string[] args)
        {
            int num;
            num = Convert.ToInt32(Console.ReadLine());
            Console.WriteLine(Recur(num));
        }
    }
}
```

## Output:
![Screenshot (3)](https://user-images.githubusercontent.com/75235167/170472116-4927ded1-a547-496a-9e2e-35b3ca08c68b.png)


## Result:
