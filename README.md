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
        static void Main()
        {
            string ThisYear;
            int NumContestants1;
            string LastYear;
            int NumContestants2;
            int fee;
            int total_revenue;
            Write("The amount of contestants in last years competition: ");
            LastYear = ReadLine();
            Write("The amount of contestants in this years competition: ");
            ThisYear = ReadLine();
            WriteLine("Last Years contestants: {0}", LastYear);
            WriteLine("This Years contestants: {0}", ThisYear);
            fee = 25;
            NumContestants1 = Convert.ToInt16(ThisYear);
            NumContestants2 = Convert.ToInt16(LastYear);
            total_revenue = fee * NumContestants1;
            WriteLine("Total Revenue this year: {0}", total_revenue);
            if (NumContestants1 > NumContestants2)
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
