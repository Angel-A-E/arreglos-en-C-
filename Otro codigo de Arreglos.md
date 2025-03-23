using System;

class Program
{
    static void Main()
    {
            //Declarar arreglos
        string[,] NombreDeEmpleados = new string[3,5];
        string[,] NombreDeDepartamento = new string[3,5];

        NombreDeEmpleados[0,0] = "Juan Carlos Reyes";
        NombreDeEmpleados[0,1] = "Angel Gabriel";
        NombreDeEmpleados[0,2] = "Braley Cedeño";
        NombreDeEmpleados[0,3] = "Wali Jimenez";
        NombreDeEmpleados[0,4] = "Juan Perez";

        NombreDeDepartamento[0,0] = "Contabilidad";
        NombreDeDepartamento[0,1] = "Ventas";
        NombreDeDepartamento[0,2] = "Recursos Humanos";
        NombreDeDepartamento[0,3] = "Almacen";
        NombreDeDepartamento[0,4] = "Calidad";

            //combinar
        string[,] Combinacion = new string[1,5];

            //unir
        for(int i = 0; i < 5; i++)
        {
        Combinacion[0,i] = NombreDeEmpleados[0,i] + " - " + NombreDeDepartamento[0,i];   
        }

            //Consola
        Console.WriteLine("Lista de empleados con puesto de Trabajo o Departamento");
        for(int i = 0; i < 5; i++)
        {
            Console.WriteLine(Combinacion[0,i]);
        }
    }
}
