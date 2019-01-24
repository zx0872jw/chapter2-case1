# chapter2-case1
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using static System.Console;
namespace GreenvilleRevenue
{
    class Program
    {
        static void Main(string[] args)
        {
            string ThisYear;
            int This_Number1;
            string LastYear;
            int This_Number2;
            int fee;
            int total_revenue;
            Write("The amount of contestants in last years competition: ");
            LastYear = ReadLine();
            Write("The amount of contestants in this years competition: ");
            ThisYear = ReadLine();
            WriteLine("Last Years contestants: {0}", LastYear);
            WriteLine("This Years contestants: {0}", ThisYear);
            fee = 25;
            This_Number1 = Convert.ToInt16(ThisYear);
            This_Number2 = Convert.ToInt16(LastYear);
            total_revenue = fee * This_Number1;
            WriteLine("Total Revenue this year: {0}", total_revenue);
            if (This_Number1 > This_Number2)
                {
                WriteLine("This year has more contestants than last year.");
                }
            else
                {
                WriteLine("Last year had more contestants than this year.");
            }
        }
    }
}
