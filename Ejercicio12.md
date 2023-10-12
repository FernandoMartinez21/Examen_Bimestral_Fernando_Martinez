# DESCRIPCION
Realice un programa que me permitaingresar una palabra utilizando areglos X palabra 
# SOLUCION DEL PROBLEMA 
#include<iostream>
using name space std;
int main(){
char frases [50]
char arreglo_palabras[4][10]={"Se","puede","imaginar","programar"};
int tamano_arreglo=4;
bool encontrado=true;
cout<<"ingrese una frase";
cin.getline(Frases,50);
char*token=strtok(Frases,"50");
for(int i=0;i<tamano_arreglo; itt)
{
encontrado = false;
while(token!=NULL)
{
if(stremp(token,arreglo_palabras[i])==0)
{
encontrado=true;
breal;
}
tokenn=strtok(NULL;"");
}
if (encontrado)
{
    cout<<"La frase contiene la secuencia 'se puede imaginar se puede programar'"<<endl;
}
else
cout<<"La frase contiene la secuencia ' se puede inaginar se puede programar'"<<endl;
}
return 0;
}  