# ENTRADA DE DADOS PELO TECLADO

```java
package fundamentos;

import java.util.Scanner;

import javax.swing.JOptionPane;

public class EntradaDadosTeclado {

    public static void main(String[] args) {

        // Exemplo 1: Via Terminal.
        Scanner entrada = new Scanner(System.in);
            System.out.println("Digite a sua idade: ");
            int idade = entrada.nextInt();

            System.out.println("Digite o seu nome: ");
            String nome = entrada.nextLine();

            System.out.printf("%s %d", nome, idade);
        entrada.close();

        // Exemplo 2: Abre uma caixa de diálogo no sistema operacional.
        String cor = JOptionPane.showInputDialog("Digite a sua cor: ");
        System.out.println(cor);
    }
}
```
