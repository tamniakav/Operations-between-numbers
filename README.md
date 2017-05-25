using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Operations_between_numbers
{
    class Program
    {
        static void Main(string[] args)
        {
            double n1 = double.Parse(Console.ReadLine());
            double n2 = double.Parse(Console.ReadLine());
            string operation = Console.ReadLine();

            if (operation == "+")
            {
                double result = n1 + n2;
                double result1 = result % 2;

                if (result1 == 0)
                {
                    Console.WriteLine("{0} {1} {2} = {3} - even", n1, operation, n2, result);
                }
                else if (result1 == 1)
                {
                    Console.WriteLine("{0} {1} {2} = {3} - odd", n1, operation, n2, result);
                }
            }
            else if (operation == "-")
            {
                double result = n1 - n2;
                double result1 = result % 2;

                if (result1 == 0)
                {
                    Console.WriteLine("{0} {1} {2} = {3} - even", n1, operation, n2, result);
                }
                else if (result1 == 1)
                {
                    Console.WriteLine("{0} {1} {2} = {3} - odd", n1, operation, n2, result);
                }
            }
            else if (operation == "*")
            {
                double result = n1 * n2;
                double result1 = result % 2;

                if (result1 == 0)
                {
                    Console.WriteLine("{0} {1} {2} = {3} - even", n1, operation, n2, result);
                }
                else if (result1 == 1)
                {
                    Console.WriteLine("{0} {1} {2} = {3} - odd", n1, operation, n2, result);
                }
            }
            else if (operation == "/")
            {
                if (n2 == 0)
                {
                    Console.WriteLine("Cannot divide {0} by zero", n1);
                }
                else
                {
                    double result = n1 / n2;
                    Console.WriteLine("{0} {1} {2} = {3:f2}", n1, operation, n2, result);
                }
            }
            else if (operation == "%")
            {
                if (n2 == 0)
                {
                    Console.WriteLine("Cannot divide {0} by zero", n1);
                }
                else
                {
                    double result = n1 % n2;
                    Console.WriteLine("{0} {1} {2} = {3}", n1, operation, n2, result);
                }
            }
        }
    }
}
