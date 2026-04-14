# Ejercicios-de-IF-ELSE
1,2,3,4,5

//1) "El control de peso de la Razor Crest"

using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApplication2
{
    class Program
    {

        static void Main(string[] args)
        {
            // 1. El Control de Peso de la Razor Crest
            //peso maximo = 5000kg
            //

            Console.WriteLine("Cuantos Kilogramos pesa su carga? ");
            int peso;
            peso = Convert.ToInt32(Console.ReadLine());

            if (peso <= 5000)
            {
                Console.WriteLine("Despegue autorizado. Buen viaje, Mando");
            }

            int diferencia;
            diferencia = peso - 5000;

            if (peso > 5000)
            {
                Console.WriteLine("Alerta: Exceso de peso. Debes descargar " + diferencia + " kg para despegar");
            }

        }
    }
}

