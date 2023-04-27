# EjLibro01Borrar

#include <iostream>

using namespace std;

/// @brief 
/// @return 
int main () {
    int costo=0;
    int VidaUtil=0;
    int ValorRecuperacion=0;
    int Anio=0;
    int D=0;
    int Acumulado=0;

    cout<< "Ingrese el costo: ";
    cin >> costo;
    cout<< "Ingrese la Vida Util: ";
    cin >> VidaUtil;
    cout<< "Ingrese el valor de recuperacion: ";
    cin >> ValorRecuperacion;
    D=(costo-ValorRecuperacion)/VidaUtil;
    do {
     Acumulado= Acumulado + D;
     costo= costo-D;
     Anio=Anio+1;
     cout<< endl <<"Anio " << Anio << " Depreciacion " << D << " Depreciación acumulada  " <<Acumulado << " Valor anual "<<costo;
    } while (Anio<VidaUtil);
    
    }
    
    
