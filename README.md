using System;

namespace Homework
{
    internal class Program
    {
        static void Main(string[] args)
        {
            Digits(1489);


        }


        static void Digits(int n)
        {
            var divisor = 1;
            while (n/ divisor>=10)
            {
                divisor *= 10;
            }
            while (divisor>0)
            {
                int digit = n / divisor;
                Console.WriteLine(digit);
                n %= divisor;
                divisor /= 10;
            }
            

        }
