# proje1
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using static yeniproje3.metodlarım;

namespace yeniproje3
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Birinci sayıyı giriniz");
            string sayı1 = Console.ReadLine();
            Console.WriteLine("İkinci sayıyı giriniz");
            string sayı2 = Console.ReadLine();
            int sonuc = 0;
            string hatalistesi = "";

            hatalistesi += sayıMı(sayı1);
            hatalistesi += sayıMı(sayı2);
            if (hatalistesi == "")
            {
                sonuc = Convert.ToInt32(sayı1) + Convert.ToInt32(sayı2);
                Console.WriteLine(sonuc.ToString());
            }
            else
            {
                Console.WriteLine(hatalistesi);
            }
            Console.ReadLine();
        }
    }
}
