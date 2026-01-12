using System;

namespace MyProject 
{
    public class task3
    {
        static void Main(string[] args)
        {
            int[] numbers = { 3, 7, 12, 19, 21, 25, 30 };

            Console.Write("Enter a number to search for: ");
            int targetNumber = Convert.ToInt32(Console.ReadLine());

            bool found = false;

            for (int i = 0; i < numbers.Length; i++)
            {
                if (numbers[i] == targetNumber)
                {
                    Console.WriteLine($"Number found at position {i}!");
                    found = true;
                    break;
                }
            }

            if (!found)
            {
                Console.WriteLine("Number not found in the list.");
            }
        }
    }
}

