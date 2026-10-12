import java.util.Scanner;
public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Escribe una frase o palabra en minúsculas: ");

        String texto = scanner.nextLine().toLowerCase();
        //toLowerCase(): Convierte el texto a minúsculas//

        int contador = 0;
        //contador = 0: Inicializa el contador//

        for (int i = 0; i < texto.length(); i++) {
            //for: Recorre cada carácter//

            char letra = texto.charAt(i);
            //charAt(i): Obtiene cada letra//

            switch (letra) {
                //switch: Compara la letra con las opciones//
                case 'a':
                case 'e':
                case 'i':
                case 'o':
                case 'u':
                    //case: identifica las vocales//

                    contador++;
                    //contador++: Aumenta el contador cuando encuentra una vocal//
                    break;
                    //break: Termina el caso actual//
            }
        }
        System.out.println("El total de elementos clave encontrados es: " + contador);
        scanner.close();
    }
}
//El programa recibe una frase y cuenta cuántas vocales contiene//