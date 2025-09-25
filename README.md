11111111111111111111111111111
a
using System;
class AddNumbers
{
    static void Main(string[] args)
    {
        if (args.Length < 2)
        {
            Console.WriteLine("Please enter two values");
            return;
        }

        int num1 = int.Parse(args[0]);
        int num2 = int.Parse(args[1]);
        int sum = num1 + num2;
        Console.WriteLine("Sum: " + sum);
    }
}


222222222222222222222222
using System;
class Expressions
{
    public static void Main ( )
    {
        // Declaration and Initialization
        int a = 10, b = 5, c = 8, d = 2;
        float x = 6.4F, y = 3.0F;

        // Order of Evaluation
        int answer1 = a * b + c / d;
        int answer2 = a * (b + c) / d;

        // Modulo Operations
        int answer3 = a % c;
        float answer4 = x % y;

        // Logical Operations
        bool bool1 = a > b && c > d;
        bool bool2 = a < b && c > d;
        bool bool3 = a < b || c > d;
        bool bool4 = !(a - b == c);

        Console.WriteLine("Order of Evaluation");
        Console.WriteLine("a * b + c / d = " + answer1);
        Console.WriteLine("a * (b + c) / d = " + answer2);
        Console.WriteLine("Modulo Operations");
        Console.WriteLine("a % c = " + answer3);
        Console.WriteLine("x % y = " + answer4);
        Console.WriteLine("Logical Operations");
        Console.WriteLine("a > b && c > d = " + bool1);
        Console.WriteLine("a < b && c > d = " + bool2);
        Console.WriteLine("a < b || c > d = " + bool3);
        Console.WriteLine("!(a - b) == c = " + bool4);
    }
}

3333333333333333
using System;
class IfTest
{
    public static void Main ( )
    {
        int i, count, count1, count2;
        float[] weight = { 45.0F, 55.0F, 47.0F, 51.0F, 54.0F };
        float[] height = { 176.5F, 174.2F, 168.0F, 170.7F, 169.0F };
        count = 0;
        count1 = 0;
        count2 = 0;
        for (i = 0; i <= 4; i++)
        {
            if (weight[i] < 50.0 && height[i] > 170.0)
            {
                count1 = count1 + 1; // Executed when condition is true
            }
            count = count + 1; // Always executed
        }
        count2 = count - count1;
        Console.WriteLine("Number of persons with ...");
        Console.WriteLine("Weight<50 and height>170 ="+count1);
        Console.WriteLine("Others = "+count2);
    }
}

444444444444

using System;
class IfElseTest
{
    public static void Main ( )
    {
        int[] number = { 50, 65, 56, 71, 81 };
        int even = 0, odd = 0;

        for (int i = 0; i < number.Length; i++)
        {
            if ((number[i] % 2) == 0) // use of modulus operator
            {
                even += 1; // counting EVEN numbers
            }
            else
            {
                odd += 1; // counting ODD numbers
            }
        }

        Console.WriteLine("Even Numbers : " + even);
        Console.WriteLine("Odd Numbers : " + odd);
    }
}

5555555555
using System;
class IfElseNesting
{
    public static void Main ( )
    {
        int a = 325, b = 712, c = 478;
        Console.Write("Largest value is : ");
        if (a > b)
        {
            if (a > c)
            {
                Console.WriteLine(a);
            }
            else
            {
                Console.WriteLine(c);
            }
        }
        else
        {
            if (c > b)
            {
                Console.WriteLine(c);
            }
            else
            {
                Console.WriteLine(b);
            }
        }
    }
}


77777777777

class DoWhileTest
{
    public static void Main ( )
    {
        int row, column, y;
        row = 1;
        System.Console.WriteLine("Multiplication Table \n");
        do
        {
            column = 1;
            do
            {
                y = row * column;
                System.Console.Write(" " + y);
                column = column + 1;
            }
            while (column <= 3);
            System.Console.WriteLine("\n");
            row = row + 1;
        }
        while (row <= 3);
    }
}

88888888888

using System;
class ForTest
{
    public static void Main ( )
    {
        long p;
        int n;
        double q;
        Console.WriteLine("2 to power -n     n     2 to power n");
        p = 1L;
        for (n = 0; n < 10; ++n)
        {
            if (n == 0)
            {
                p = 1L;
            }
            else
            {
                p = p * 2;
                q = 1.0 / (double)p;
                Console.WriteLine("{0:F6}  {1:D}  {2:D}", q, n, p);
            }
        }
    }
}

99999999
using System;
class Nesting
{
    void Largest ( int m, int n )
    {
        int large = Max ( m, n ); //Nesting
        Console.WriteLine( large );
    }

    int Max (int a, int b)
    {
        int x = (a > b) ? a : b;
        return ( x );
    }
}

class NestTesting
{
    public static void Main ( )
    {
        Nesting next = new Nesting ();
        next.Largest ( 100, 200 ); //Method call
    }
}

10101010101010

using System;
class NumberSorting
{
    public static void Main ( )
    {
        int[] number = { 55, 40, 80, 65, 71 };
        int n = number.Length;
        Console.Write("Given list : ");
        for (int i = 0; i < n; i++)
        {
            Console.Write(" " + number[i]);
        }
        Console.WriteLine("\n");

        // Sorting begins
        for (int i = 0; i < n; i++)
        {
            for (int j = i + 1; j < n; j++)
            {
                if (number[i] < number[j])
                {
                    // Interchange values
                    int temp = number[j];
                    number[j] = number[i];
                    number[i] = temp;
                }
            }
        }
        Console.Write("Sorted list : ");
        for (int i = 0; i < n; i++)
        {
            Console.Write(" " + number[i]);
        }
        Console.WriteLine(" ");
    }
}


