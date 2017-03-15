# triangulos
package test;

import java.util.Scanner;

public class Triangulo {

	private static double a;
	private static double b;
	private static double c;
	private static Scanner teclado;

	public static void main(String[] args) {
		teclado = new Scanner(System.in);
		a = teclado.nextDouble();
		b = teclado.nextDouble();
		c = teclado.nextDouble();

		if ((a > b + c) || (b > a + c) || (c > a + b) || (a < 1) || (b < 1) || (c < 1)) {
			System.out.println("Não é triangulo");
		} else if ((a == b) && (b == c)) {
			System.out.println("Equilatero");
		} else if ((a == b) || (b == c) || (c == a)) {
			System.out.println("Isoceles");
		} else {
			System.out.println("Scaleno");
		}
	}
}
