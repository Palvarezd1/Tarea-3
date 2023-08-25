# TAREA 1 - CALCULADORA DE LONGITUDES
## **Instrucciones**: *Escriba un algoritmo para conversión de unidades de longitud, el programa debe recibir un número que es representado en centímetros. Luego preguntar a qué unidad se quiere convertir, las opciones son: metros, yardas, varas, pulgadas y pies.*
>## **PSEUDOCODIGO**
###### **CODIGO**:
:computer:
```
Algoritmo Longitudes
	Definir num Como Real
	Definir eleccion Como Entero
	Escribir "Ingrese el numero en centimetros para saber su conversion"
	Leer num 
	Escribir "A que Longitud lo desea convertir: "
	Escribir "1- metros"
	Escribir "2- varas"
	Escribir "3- yardas"
	Escribir "4- pulgadas"
	Escribir "5- pies"
	Leer eleccion 
	Segun eleccion Hacer
		1:
			Escribir "El resultado es: " num / 100 " metros"
 		2:
			Escribir "El resultado es: " num / 83.5905 " varas"
		3:
			Escribir "El resultado es: " num / 91.44 " yardas"
		4:
			Escribir "El resultado es: " num / 2.54 " pulgadas" 
		5:
			Escribir "El resultado es: " num / 30.48 " pies"
		De Otro Modo:
			Escribir "El numero que ingreso no se encuentra en el rango de opciones"
	Fin Segun
FinAlgoritmo
```
> ## **C++**
###### **CODIGO**: 
:computer:
```c++
#include<iostream>
using namespace std;
int main() {
	int eleccion;
	float num;
	cout << "Ingrese el numero en centimetros para saber su conversion" << endl;
	cin >> num;
	cout << "A que Longitud lo desea convertir: " << endl;
	cout << "1- metros" << endl;
	cout << "2- varas" << endl;
	cout << "3- yardas" << endl;
	cout << "4- pulgadas" << endl;
	cout << "5- pies" << endl;
	cin >> eleccion;
	switch (eleccion) {
	case 1:
		cout << "El resultado es: " << num/100 << " metros" << endl;
		break;
	case 2:
		cout << "El resultado es: " << num/83.5905 << " varas" << endl;
		break;
	case 3:
		cout << "El resultado es: " << num/91.44 << " yardas" << endl;
		break;
	case 4:
		cout << "El resultado es: " << num/2.54 << " pulgadas" << endl;
		break;
	case 5:
		cout << "El resultado es: " << num/30.48 << " pies" << endl;
		break;
	default:
		cout << "El numero que ingreso no se encuentra en el rango de opciones" << endl;
	}
	return 0;
}

```
> ## **PYTHON** 
###### **CODIGO**: 
:computer:
```python
num = float(input('Ingrese la cantidad en centrimetos para su conversion '))
eleccion = int(input('Seleccion el numero de la opcion para saber su conversion; 1- Metros; 2- Varas; 3- Yardas; 4- Pulgadas; 5- Pies; '))
calculo = float
if eleccion == 1:
        print('El resultado en metros es : ',  str(num / 100)) 
else: 
    if eleccion == 2:
        print('El resultado en varas es: ', str(num / 83.5905))
    else: 
         if eleccion == 3:
              print('El resultado en yardas: ', str(num / 91.44))
         else:
              if eleccion == 4:
                   print('El resultado en pulgadas es: ', str(num / 2.54))
              else:
                   if eleccion == 5:
                        print('El resultado en pies es: ', str(num / 30.48))
                   else: 
                        input('El numero que ingreso no se encuentra en el rango de las opciones')
```