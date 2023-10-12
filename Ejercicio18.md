# DESCRIPCION
Realice un programa que me permita ingresar n,numeros y que muestre en pantalla cuantos pares y impares,con ciclo while
# SOLUCION DEL PROBLEMA
#include <iostream>

using namespace std;

int main() {
    int n;
    int numero;
    int pares = 0;
    int impares = 0;

    cout << "Ingrese la cantidad de números a evaluar: ";
    cin >> n;

    int i = 1;
    while (i <= n) {
        cout << "Ingrese el número " << i << ": ";
        cin >> numero;

        if (numero % 2 == 0) {
            pares++;
        } else {
            impares++;
        }

        i++;
    }

    cout << "Cantidad de números pares: " << pares << endl;
    cout << "Cantidad de números impares: " << impares << endl;

    return 0;
}
