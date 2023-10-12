# DESCRIPCION cuantas 
Realice un programa que permita ingresar 5 calificaciones en un areglo y obtenga el promedio de las 5 calificaciones y cuente cuantas calificaciones son pares y e inpares 
# SOLUCION DEL PROGRAMA
#include <iostream>
using namespace std;

int main() {
    const int numCalificaciones = 5;
    int calificaciones[numCalificaciones];
    int suma = 0;
    int calificacionesPares = 0;
    int calificacionesImpares = 0;

    for (int i = 0; i < numCalificaciones; i++) {
        cout << "Ingrese la calificación " << i + 1 << ": ";
        cin >> calificaciones[i];
        suma += calificaciones[i];

        if (calificaciones[i] % 2 == 0) {
            calificacionesPares++;
        } else {
            calificacionesImpares++;
        }
    }

    // Cálculo del promedio
    int promedio = suma / numCalificaciones;

    cout << "Promedio de calificaciones: " << promedio << endl;
    cout << "Calificaciones pares: " << calificacionesPares << endl;
    cout << "Calificaciones impares: " << calificacionesImpares << endl;

    return 0;
}
