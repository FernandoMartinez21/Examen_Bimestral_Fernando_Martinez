# DESCRIPCION
Realice un programa que permita crear un arreglo bidimencional que permita almacenar numeros enteros,que entra un tamañano de 3x3 y que optenga la sumatoria de cada columna y pilar 
# SOLUCION DEL PROBLEMA 
#include <iostream>
#include <stdlib.h>
#include <stdio.h>
using namespace std;

int main() {
    const int filas = 3;
    const int columnas = 3;
    int matriz[filas][columnas];


    cout << "Ingrese los valores de la matriz 3x3:\n";
    for (int i = 0; i < filas; i++) {
        for (int j = 0; j < columnas; j++) {
            cout << "Ingrese el valor en la posición [" << i + 1 << "][" << j + 1 << "]: ";
            cin >> matriz[i][j];
        }
    }

 
    int sumaColumnas[columnas] = {0};
    for (int j = 0; j < columnas; j++) {
        for (int i = 0; i < filas; i++) {
            sumaColumnas[j] += matriz[i][j];
        }
    }


    int sumaFilas[filas] = {0};
    for (int i = 0; i < filas; i++) {
        for (int j = 0; j < columnas; j++) {
            sumaFilas[i] += matriz[i][j];
        }
    }


    cout << "Matriz ingresada:\n";
    for (int i = 0; i < filas; i++) {
        for (int j = 0; j < columnas; j++) {
            cout << matriz[i][j] << "\t";
        }
        cout << "\n";
    }

    cout << "Suma de cada columna:\n";
    for (int j = 0; j < columnas; j++) {
        cout << "Columna " << j + 1 << ": " << sumaColumnas[j] << "\n";
    }


    cout << "Suma de cada fila:\n";
    for (int i = 0; i < filas; i++) {
        cout << "Fila " << i + 1 << ": " << sumaFilas[i] << "\n";
    }

    return 0;
}