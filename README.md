# switch_statements



using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace cis_115_week4
{
    class Program
    {
        static void Main(string[] args)
        {
            double totPoints = 0;
            double maxPoints = 1000;
            double totPct;
            char Grade;
            string stuFirst = "";
            string stuLast = "";

            //Declare

            //output greeting
            Console.WriteLine("Welcome to your Grade Determinator");
            Console.WriteLine("______________________________");

            // prompt user for input
            Console.WriteLine("______________________________");
            Console.WriteLine("Enter Students First Name ");
            stuFirst = (Console.ReadLine());
            Console.WriteLine("______________________________");
            Console.WriteLine("Enter Students Last Name ");
            stuLast = (Console.ReadLine());
            Console.WriteLine("______________________________");
            Console.WriteLine("Enter Students Score in Class ");
            totPoints = Convert.ToInt32(Console.ReadLine());
            Console.WriteLine("______________________________");
            //Console.WriteLine("Enter Max Points in Class ");
            maxPoints = Convert.ToInt32(Console.ReadLine());


            // validate total points
            //  if (totPoints < 0 || totPoints > maxPoints)
            if (totPoints < 0 )
            {
                Console.WriteLine("Error incorrect value ");
                Console.ReadLine();
                return;

            }
           
            // calculate total percent
            totPct = totPoints / maxPoints;

            switch (totPct)
            {
                case 1:
                    (totPoints >= 100);
                    Console.WriteLine("I am 100 or above: {n}");
                    break;
            }
            /*
            switch (Grade)
            {
                case int when (n >= 100):
                     Console.WriteLine($"I am 100 or above: {n}");
                     break;

                case int n when (n < 100 && n >= 50):
    Console.WriteLine($"I am between 99 and 50: {n}");
                    break;

                case int n when (n < 50):
    Console.WriteLine($"I am less than 50: {n}");
                    break;
            }


            /* determine grade
            if (totPct >= .90)
                Grade = Convert.ToChar("A");

            else if
                     (totPct >= .8)
                Grade = Convert.ToChar("B");

            else if

                (totPct >= .7)
            {
                Grade = Convert.ToChar("C");
            }
            else if
                (totPct >= .6)
            {
                Grade = Convert.ToChar("D");
            }
            else
            {
                Grade = Convert.ToChar("F");
            }
            */

            // output Double totPoints,String stuFrist,String stuLast,Double totPct,Char grade
            Console.WriteLine("________________________");
            Console.WriteLine(" Students First Name : " + stuFirst);
            Console.WriteLine(" Students Last Name : " + stuLast);
            Console.WriteLine(" Total Percent : " + totPct);
            Console.WriteLine(" Students Grade : " + Grade);
            Console.WriteLine(" thanks for using this calculator");

            Console.ReadLine();


            // ending message


        }
    }
}
