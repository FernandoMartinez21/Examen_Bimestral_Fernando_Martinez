# DESCRIPCION 
Dado realizado dueldo de n trabajadores de 15% a cada uno de ellos inferior a Q800.Imprima el sueldo incorporado si corresponde
# SOLUCION DEL PROBLEMA
#include <iostream>
using namespace std;


int calcularNuevoSueldo(int sueldo) {
    const double aumento = 0.15;
    int nuevoSueldo = sueldo + sueldo * aumento;
    return nuevoSueldo;
}

int main() {
    int n;
    cout << "Ingrese la cantidad de trabajadores: ";
    cin >> n;

    for (int i = 1; i <= n; i++) {
        int sueldo;
        cout << "Ingrese el sueldo del trabajador " << i << ": Q";
        cin >> sueldo;

        if (sueldo < 800) {
            int nuevoSueldo = calcularNuevoSueldo(sueldo);
            cout << "El sueldo modificado del trabajador " << i << " es: Q" << nuevoSueldo << endl;
        }
    }

    return 0;
}
