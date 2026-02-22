# c-
#include <iostream>
using namespace std;

void evaluarparimpar(int num) {
    if (num % 2 == 0) {
        cout << "El numero es PAR" << endl;
    }
    else {
        cout << "El numero es IMPAR" << endl;
    }
 }

int main() {

    int num;

    do {
        cout << "ingrasa un numero entero/ 0 termina el programa" << endl;
        cin >> num;
        if (cin.fail()) {
            cout << "ERROR, numero no valido" << endl;
            cin.clear();
            cin.ignore(1000, '\n');
        }
        else {
            if (num != 0) {
                evaluarparimpar(num);
            }
        }
    } while (num != 0);
    cout << "\n Programa finalizado" << endl;
 return 0;
}
