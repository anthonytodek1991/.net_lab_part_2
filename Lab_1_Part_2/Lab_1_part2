using System;
using System.Globalization;

namespace Lab_1_Part_2
{
    class Program
    {
        static void Main(string[] args)
        {
            string userInputOne = string.Empty;
            string userInputTwo = string.Empty;

            Console.WriteLine("Instructions to run program");

            Console.WriteLine("Please enter the first Date in this format MM/DD/YY Hour:minute AM/PM");
            userInputOne = Console.ReadLine();

            Console.WriteLine("Please enter the Second Date in this format MM/DD/YY Hour:minute AM/PM");
            userInputTwo = Console.ReadLine();

            CalculateDifferenceOfDateTimes(userInputOne, userInputTwo);

        }
     
        private static void CalculateDifferenceOfDateTimes(string userInputOne, string userInputTwo)
        {
            if (ValidateUserInput(userInputOne) && ValidateUserInput(userInputOne))
            {
                DateTime userDateOne = Convert.ToDateTime(userInputOne, CultureInfo.InvariantCulture);
                DateTime userDateTwo = Convert.ToDateTime(userInputTwo, CultureInfo.InvariantCulture);
                Console.WriteLine(userDateOne - userDateTwo);
            }
            else
            {
                Console.WriteLine("Error : You have enter an an invalid format for one of the inputs");
            }
        }

        private static bool ValidateUserInput(string dateTime)
        {
            DateTime tempDateTime;
            return DateTime.TryParse(dateTime, out tempDateTime);
        }
    }
}
