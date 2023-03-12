# CONTINUAR

Interrompe a iteração atual e pula para o próximo valor do iterável.

```java
package controle;

public class ContinuarQuebrar {

    public static void main(String[] args) {

        for(int i = 1; i <= 10; i++) {

            if(i % 2 != 0) {
                continue;
            }

            System.out.printf("O número %d é PAR.\n", i);
        }
    }
}
```
