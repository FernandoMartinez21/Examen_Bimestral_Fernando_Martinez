# DECRIPCION
Realice un programa que permita la suma de numeros pares y impares entre 1 y n,ciclo while
# SOLUCION DEL PROBLEMA 
#include <iostream>

using namespace std;

int main() {
    int n;
    int suma_pares = 0;
    int suma_impares = 0;
    int numero = 1;

    cout << "Ingrese un número entero positivo: ";
    cin >> n;

    while (numero <= n) {
        if (numero % 2 == 0) {
            suma_pares += numero;
        } else {
            suma_impares += numero;
        }
        numero++;
    }

    cout << "La suma de los números pares entre 1 y " << n << " es: " << suma_pares << endl;
    cout << "La suma de los números impares entre 1 y " << n << " es: " << suma_impares << endl;

    return 0;
}
