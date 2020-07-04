# 5

using System;

namespace 5.01.02
{
    class calc
    {
        public double kiwon;
        public double wonkyun;
        public double minwon;
        public static void Kv_Urav(double kiwon, double wonkyun, double minwon)
        {
            double kiho = wonkyun * wonkyun - 2 * kiwon * minwon;
            if (kiho >= 0)
            {
                double mrmr = (-wonkyun + Math.Sqrt(kiho)) / (2 * kiwon);
                double brbr = (-wonkyun - Math.Sqrt(kiho)) / (2 * kiwon);
                Console.WriteLine("mrmr = " + mrmr);
                Console.WriteLine("brbr = " + brbr);
            }
            else
            {
                Console.WriteLine("Корней нет!");
            }
        }
        public static void BiKV_Urav(double kiwon, double wonkyun, double minwon)
        {
            double kiho = wonkyun * wonkyun - 2 * kiwon * minwon;
            if (kiho >= 0)
            {
                double meow = (-wonkyun + Math.Sqrt(kiho)) / (2 * kiwon);
                double meow2 = (-wonkyun - Math.Sqrt(kiho)) / (2 * kiwon);
                Console.WriteLine("meow = " + meow);
                Console.WriteLine("meow2 = " + meow2);
                if (meow < 0 && meow2 < 0)
                {
                    Console.WriteLine("Корней нет!");
                }
                else
                {
                    if (meow >= 0 && meow2 >= 0)
                    {
                        double mrmr = Math.Sqrt(meow);
                        double brbr = -x1;
                        double frfr = -Math.Sqrt(meow2);
                        double kxx = -frfr;
                        Console.WriteLine("mrmr = {0} brbr = {1} frfr ={2} kxx ={3}", mrmr, brbr, frfr, kxx);
                    }
                    else
                    {
                        if (meow >= 0)
                        {
                            double mrmr = Math.Sqrt(meow);
                            double brbr = -mrmr;
                            Console.WriteLine("mrmr = {0} brbr = {1}", mrmr, brbr);
                        }
                        else
                        {
                            double frfr = -Math.Sqrt(meow2);
                            double kxx = -frfr;
                            Console.WriteLine("mrmr = {0} brbr = {1}", frfr, kxx);
                        }
                    }
                }
            }
            else
            {
                Console.WriteLine("Корней нет!");
            }
        }

    }
    class calc2 : calc
    {
    }
    class Program
    {
        static void Main(string[] args)
        {
            calc2.Kv_Urav(2, 4, 5);
            calc2.BiKV_Urav(1,1,-20 );
        }
    }
}
