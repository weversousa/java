# OPERADORES

```java
package fundamentos;

public class Operadores {

    public static void main(String[] args) {

        // ARITMETICOS
        System.out.println(1 + 2);
        System.out.println(2 - 1);
        System.out.println(2 * 3);
        System.out.println(7 / 3);
        System.out.println(7 / (double) 3);
        System.out.println(7 / 3.0);
        System.out.println(7 % 3.0);
        System.out.println(Math.pow(2, 3));

        // LÓGICOS
        System.out.println(true && true);
        System.out.println(false || true);
        System.out.println(true ^ false); // XOR - OU EXCLUSIVO
        System.out.println(!false); // NOT
        System.out.println(!!true);

        // RELACIONAIS
        System.out.println(1 == 2);
        System.out.println(2 > 1);
        System.out.println(2 >= 1);
        System.out.println(1 < 2);
        System.out.println(1 <= 2);
        System.out.println(3 != 4);

        // ATRIBUIÇÃO
        int n = 1;
        n += 1;
        n -= 1;
        n *= 1;
        n /= 1;
        n %= 1;

        // INCREMENTO
        n++; // n = n + 1
        ++n; // n = n + 1

        // DECREMENTO
        n--; // n = n - 1;
        --n; // n = n - 1;

        int a = 1;
        int b = 2;

        /*
         * Primeiro, A vai receber 1 e com isso passará a valer 2.
         * Depois, já vai ser comparado A com B.
         * Por último, B vai receber mais 1 e com isso passará a valer 3.
         */
         System.out.println(++a == b--);
         System.out.println(a == b);

        // TERNÁRIO
        double idade = 18;
        String resultado = idade >= 18 ? "maior" : "menor";
    }
}
```
