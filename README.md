# Ejercicio6
Realice un programa que mediante funciones las operaciones de suma, resta, multiplicación y división de números, la misma en f#

open System

let suma a b = a + b
let resta a b = a - b
let multiplicacion a b = a * b
let division a b = a / b

[<EntryPoint>]
let main argumentos =

    Console.WriteLine("****OPERACIONES****") 
    Console.WriteLine("Introduzca el primer numero")
    let num1 = Console.ReadLine()
    Console.WriteLine("Introduzca el segundo numero")
    let num2 = Console.ReadLine()
    let valor1 = Convert.ToInt32(num1)
    let valor2 = Convert.ToInt32(num2)
    let valor3 = suma valor1 valor2
    let valor4 = resta valor1 valor2
    let valor5 = multiplicacion valor1 valor2
    let valor6 = division valor1 valor2
    Console.WriteLine("La suma de sus dos numeros es:  "+valor3.ToString())
    Console.WriteLine("La resta de sus dos numeros es:  "+valor4.ToString())
    Console.WriteLine("La multiplicacion de sus dos numeros es:  "+valor5.ToString())
    Console.WriteLine("La division de sus dos numeros es:  "+valor6.ToString())
    let tecla = Console.ReadKey()
    0
