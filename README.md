# DateAndTime

## BirthdayOfWeek
``` 
class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Good Morning");
            Console.WriteLine("What is your month of birth?");
            int month = Int32.Parse(Console.ReadLine());
            Console.WriteLine("What is your day of birth?");
            int day = Int32.Parse(Console.ReadLine());
            Console.WriteLine("What is your year of birth?");
            int year = Int32.Parse(Console.ReadLine());


            GetTheWeekDay(year, month, day);

        }
        public static void GetTheWeekDay(int year, int month, int date)
        {
            DateTime birthdate = new DateTime(year, month, date);
            var dayOfTheWeek = birthdate.DayOfWeek;
            Console.WriteLine($"You were born in {dayOfTheWeek}");
        }
    }
    
    ```
