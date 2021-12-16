# Ciagi

TO use this program , open console , add lenght of string ( Podaj długość ciągu) ,the C value in numbers and confirm it with ENTER , program will automaticly 
count it.


using System;

namespace ciag

{
    class Program
    {
        static void Main(string[] args)
        {           
            Console.WriteLine("Podaj długość ciągu.");
            int dlugosc = Convert.ToInt32(Console.ReadLine());
            Console.WriteLine("Podaj C: ");
            int c = Convert.ToInt32(Console.ReadLine());
            int[] ciag = new int[dlugosc];
            for (int i = 0; i < dlugosc; i++)
            {
                Console.WriteLine("Podaj wartość: ");
                ciag[i] = Convert.ToInt32(Console.ReadLine());
            }
            for (int n = 0; n < dlugosc - 1; n++)
            {
                if (ciag[n] + ciag[n + 1] == c)
                {
                    Console.WriteLine("a + b = c ");
                }
                else
                {
                    Console.WriteLine("a + b != c ");
                }
            }

        }
    }
}
