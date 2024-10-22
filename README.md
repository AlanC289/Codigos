

#include <iostream>
using namespace std;
//Clases
class Alumno
{
public:
    int NoCuenta;
    string NombreCompleto;
    int materiasCursadas;
    int materiasCursando;
    int materiasPorCursar;

    //Constructor
public:
    Alumno()
    {
        this->NoCuenta = 0;
        this->NombreCompleto = "";
    }
    Alumno(int nc, string nombre)
    {
        this->NoCuenta = nc;
        this->NombreCompleto = nombre;
    }
//Getters
    int getNoCuenta()
    {
        return this->NoCuenta;
    }
    string getNombreComleto()
    {
        return this->NombreCompleto;
    }
    int getmateriasCursadas()
    {
        return this->materiasCursadas;
    }
    int getmateriasCursando()
    {
        return this->materiasCursando;
    }
    int getmateriasPorCursar()
    {
        return this->materiasPorCursar;
    }
//Setters
    void setNoCuenta(int nc)
    {
        this->NoCuenta = nc;
    }
    void setNombreCompleto(string nombre)
    {
        this->NombreCompleto = nombre;
    }
    void setmateriasCursadas(int materias)
    {
        this->materiasCursadas = materias;
    }
    void setmateriasCursando(int materiascursadas)
    {
        this->materiasCursando = materiascursadas;
    }
    void setmateriasPorCursar(int materiasPorCursar)
    {
        this->materiasPorCursar = materiasPorCursar;
    }
};
/*int main()
{
    Alumno alumno1();
    Alumno alumno2(1234, "Alan Cervantes");
    cout << alumno2.NoCuenta << endl;
    cout << alumno2.NombreCompleto << endl;
   
}*/
int main()
{
    Alumno alan;
    alan.setNombreCompleto("Alan Cervantes");
    alan.setNoCuenta(335010760);
    alan.setmateriasCursadas(20);
    alan.setmateriasCursando(4);
    alan.setmateriasPorCursar(50);
    cout << alan.getNombreComleto() << endl;
    cout << alan.getNoCuenta() << endl;
    cout << alan.getmateriasCursadas() << endl;
    cout << alan.getmateriasCursando() << endl;
    cout << alan.getmateriasPorCursar() << endl;

}

/*
Struct 
  atributos --> Públicos
  funciones --> Públicos
Class
  atributos --> Privadas
  funciones --> Públicas y Privadas

Constructor --> cosntruye objetos, se llama igual que la clase
Destructor --> destruye objetos

Getters --> imprime información
*/
