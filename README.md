using System;
using System.IO;
namespace RainbowStudentData
{
    internal class Program
    {
        static void Main(string[] args)

        {
            string filePath = "C:\\Users\\Pavan\\OneDrive\\Desktop\\project directory 2\\rainbow schools\\rainbow schools\\data\\students data.txt";
            if (!File.Exists(filePath))
            {
                Console.WriteLine("File not found: " + filePath);
                return;
            }

            string[] lines = File.ReadAllLines(filePath);

            Console.WriteLine("Student Data:");

            foreach (string line in lines)
            {
                Console.WriteLine(line);
            }
            Console.ReadLine();
        }
    }
}
