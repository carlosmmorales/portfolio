El programa que deber�s desarrollar simular� el funcionamiento de un cajero autom�tico. Como punto de partida
te damos la clase Principal con la implementaci�n de un men� que servir� como interfaz de usuario (en la p�gina
siguiente).
Como puedes comprobar en el men�, el programa permitir� retirar dinero, ingresar dinero, consultar saldo o
consultar movimientos.
Debes desarrollar la l�gica de la aplicaci�n utilizando las siguientes clases e interfaces:
� ICuenta
Interfaz qu� definir� el comportamiento (m�todos) de una clase Cuenta.
� Cuenta
Representa una cuenta bancaria que debe contener el nombre del cliente, n�mero de cuenta, movimientos y
saldo actual.
� Movimiento
Representa un movimiento en una cuenta (fecha_hora, concepto, etc.). Cada objeto Cuenta contendr� como
componente una colecci�n de movimientos.
T� decidir�s los m�todos que deber�s implementar en las clases para conseguir el comportamiento deseado.

----------------------------------------------------------------------------------------------------------------------
RECURSOS PREVIOS


import java.util.Scanner;
public class Principal {
static Scanner lector;
public static void main(String[] args) {
lector = new Scanner(System.in);
String opc = "";
do {
System.out.println("Cuenta de ...");
System.out.println("-------------------------");
System.out.println(" R - Retirar");
System.out.println(" I - Ingresar");
System.out.println(" S - Consultar Saldo");
System.out.println(" M - Consultar movimientos");
System.out.println(" F - Fin del programa");
System.out.println("-------------------------");
System.out.println("�Qu� operaci�n deseas realizar? ");
opc = lector.nextLine();
} while (!opc.toUpperCase().equals("F"));
lector.close();
}
}

----------------------------------------------------------------------------------------------------------------------
Tiempo 3h