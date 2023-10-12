# DESCRIPCION 
Realice un programa que permita ingresar numeros pero al ingresar la letra x finalize la insecion de numeros y muestre en pantalla realisado con do-while
# SOLUCION DEL PROBLEMA 
#include <iostream>
#include <stdlib.h>
#include <stdio.h>
int main (){
int contador=0;
char numero;
Do{
    cout<<"ingrse el"<<contador+1<<"o.numero";
    cin>>numero;
    contador +=1  
}
while(numero ! = 'x');
cout<<"programa finalizado";
}