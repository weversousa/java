# ESTRUTURAS DE CONDIÇÃO

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
    }
}
```

## SE

```java
package controle;

public class SeSenao {

    public static void main(String[] args) {

        double media = 8.1;
        String situacao;

        if(media >= 7.0) {
            situacao = "aprovado";
        } else if(media >= 6.0) {
            situacao = "em recuperação";
        } else {
            situacao = "reprovado";
        }
    }
}
```

## CASO

```java
package controle;

public class Caso {

    public static void main(String[] args) {

        int nota = 3;
        String conceito = "";

        switch(nota) {
            case 10:
                conceito = "excelente";
                break;
            case 9: case 8:
                conceito = "ótimo";
                break;
            case 7:
                conceito = "regular";
                break;
            case 6:
                conceito = "em recuperação";
                break;
            default:
            conceito = "péssimo";
        }
    }
}
```
