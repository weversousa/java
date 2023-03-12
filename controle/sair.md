# QUEBRAR

Ao atender a condição o laço (FOR ou WHILE) é interrompido.

Também pode ser usado na estrutura [CASO](caso.md).

```java
package controle;

public class ContinuarQuebrar {

    public static void main(String[] args) {

        for(int i = 1; i <= 10; i++) {

            if(i == 5) {
                System.out.printf("O número 5 foi encontrado.\n", i);
                break;
            }
        }
    }
}
```
