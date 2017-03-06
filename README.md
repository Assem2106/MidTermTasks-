# MidTermTasks-
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace IsPrime
{
    class Program
    {

        static void Main(string[] args)
        {
            String s;
            s = Console.ReadLine();
            string[] stringNumbers = s.Split();
            foreach (string ss in stringNumbers)
            {
                int a = int.Parse(ss);
                bool ok = true;
                for (int i = 2; i * i <= a; i++)
                {
                    if (a % i == 0) ok = false;

                }
                if (ok == true)
                    Console.WriteLine(a);
            }
            Console.ReadKey();
        }
    }
}
