// enteros.cpp : Este archivo contiene la función "main". La ejecución del programa comienza y termina ahí.
//

#include <iostream>
#include <limits>
#include <iomanip>
#include <locale>
#include <string>
using namespace std;

int main() {
    // Manejo de punto decimal y separador de miles
    locale loc("");
    cout.imbue(loc);
    // 1. Entero (int)
    int numeroEntero = 42;
    cout << "Entero: " << numeroEntero << endl;
    cout << "Rango INT : " << numeric_limits<int>::min() << " a " << numeric_limits<int>::max() << endl;
    string texto0 = "Hola Mundo";
    cout << texto0 << endl;
    // Union de dos variables
    // tipo string 
    string tipoa = "Hello ";
    string tipob = "Wordl ";
    string saludo = tipoa + tipob;
    cout << saludo << endl;
    // Introducir un valor en una variable tipo e imprimirlo
    string nombre;
    cout << "Dame tu nombre : ";
    cin >> nombre;
    cout << "Hola " << nombre << endl;
    // introducir una linea 
    cin.ignore();
    string nombreCompleto;
    cout << " Dame tu nombre completo ";
    getline(cin, nombreCompleto);
    cout << "Tu nombre Completo " << nombreCompleto << endl;
    // acceso a un caracter especifico
    cout << nombre[4] << endl;



    return 0;
}
