using System;
using System.Collections.Generic;
using System.Linq;
using System.Runtime.CompilerServices;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    internal class Program
    {
        static void Main(string[] args)
        { 
            Random random = new Random();
            int[] rasgelesayilar = new int[10];
           
            Random r= new Random(); 
            int rastgelesayi = r.Next(1,10);
            for (int i = 0; i < rasgelesayilar.Length; i++)
            {
                rasgelesayilar[i] = r.Next(1,10);                 
            }
            int puan1 = 0;
            int puan2 = 0;
            for (int i = 0; i < rasgelesayilar.Length; i++)
            {
                Console.WriteLine("1.tahmininizi girin");
                int tahmin1=Convert.ToInt32(Console.ReadLine());
                if (tahmin1 == rastgelesayi)
               {           
                   puan1 += 10;                   
               }
                else
                {
                    if (rastgelesayi > tahmin1)
                    {
                        puan1 += 10 - (rasgelesayilar[i] -tahmin1);
                    }
                    else
                    {
                        puan1 += 10 - (tahmin1 - rastgelesayi);
                    }               
                }
                Console.Clear();
                //2.oyuncu 

                Console.WriteLine("2.oyuncunu tahminini girin");
                int tahmin2 = Convert.ToInt32(Console.ReadLine());
                if (tahmin2 == rasgelesayilar[i])
                {
                    puan2 += 10;
                }
                else
                {
                    if (rastgelesayi > tahmin2)
                    {
                        puan2 += 10 - (rasgelesayilar[i] - tahmin2);
                    }
                    else
                    {
                        puan2 += 10 - (tahmin2 - rasgelesayilar[i]);
                    }
                }
                Console.Clear();
                Console.WriteLine("1. OYUNCUNUNUN PUANI:" + puan1);
                Console.WriteLine("2. OYUNCUNUNUN PUANI:" + puan2);               
                Console.ReadKey();
             }
        }
        
     
    }
}
