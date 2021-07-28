import java.util.Scanner;

public class TallerSemana1Ciclo2 {

    public static void main(String[] args) {
        calcularPuntos();
    }

    public static void calcularPuntos() {
        Scanner sc = new Scanner(System.in);
        int puntos, puntosPremio, numAciertos;
        numAciertos = sc.nextInt();
        puntos = (numAciertos * 2) + 4;
        puntosPremio = (numAciertos + puntos) / 5;
        System.out.println(numAciertos + " " + puntos + " " + puntosPremio);
        if (puntosPremio >= 50) {
            System.out.print("Cuatro");
        } else {
            if (puntosPremio >= 30) {
                System.out.print("Tres");
            } else {
                if (puntosPremio >= 20) {
                    System.out.print("Dos");
                } else {
                    System.out.print("Uno");
                }
            }
        }
    }

}
