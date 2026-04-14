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


// 2) Clasificador de Aspirantes a la Academia Jedi 

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
            // 2. Clasificador de Aspirantes a la Academia Jedi

            Console.WriteLine("Ingrese la cantidad de midiclorianos ");
            int midiclorians;
            midiclorians = Convert.ToInt32(Console.ReadLine());

            if (midiclorians >= 15000)
            {
                Console.WriteLine("Potencial Maestro Jedi detectado. Avisar al Consejo");
            }

            if (midiclorians > 5000)
            {
                if (midiclorians < 15000)
                {
                    Console.WriteLine("Aceptable para entrenamiento Padawan");
                }
            }

            else if (midiclorians <= 5000)
            {
                Console.WriteLine("No posee sensibilidad a la Fuerza");
            }

        }
    }
}


// 3) Calculadora de Saltos al Hiperespacio

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
            // 3. Calculadora de Saltos al Hiperespacio

            // cada año luz consume 12 litros de combustible.

            Console.WriteLine("A cuantos Años Luz quiere viajar? ");
            int añosLuz;
            añosLuz = Convert.ToInt32(Console.ReadLine());

            Console.WriteLine("Cuantos Litros de cobustible nos quedan? ");
            int combustible;
            combustible = Convert.ToInt32(Console.ReadLine());


            int diferencia;
            diferencia = combustible / 12;

            if (diferencia >= añosLuz)
            {
                Console.WriteLine("Cálculos precisos. Saltando al hiperespacio");
            }


            int combustibleFaltante;
            combustibleFaltante = (añosLuz - diferencia) * 12;

            if (diferencia < añosLuz)
            {
                Console.WriteLine("Peligro: Combustible insuficiente.Faltan " + combustibleFaltante + " litros de combustible");
            }

        }
    }
}

