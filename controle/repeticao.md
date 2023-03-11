# ESTRUTURAS DE REPETIÇÃO

## ENQUANTO

```java
package controle;

public class SeSenao {

    public static void main(String[] args) {

        double contador = 1;

        while(contador < 5) {
            System.out.println(contador);

            contador++;
        }
        
        // INFINITO
        // while(true) {}
    }
}
```

## PARA

```java
package controle;

public class Para {

    public static void main(String[] args) {

        for(int j = 1; j <= 5; j++) {
            System.out.println(j);
        }

        // INFINITO
        // for(;;) {}
    }
}
```

## FAÇA ENQUANTO

```java
package controle;

import java.util.Scanner;

public class FacaEnquanto {

    public static void main(String[] args) {

        String opcao = "";
        Scanner entrada = new Scanner(System.in);

        do {
            System.out.println("Deseja sair [s/n]? ");
            opcao = entrada.nextLine();

        } while(opcao.trim().equalsIgnoreCase("n"));

        entrada.close();
    }
}
```
