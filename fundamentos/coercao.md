# COERÇÃO

É o famoso `(CAST)`.

```java
package fundamentos;

public class Coercao {

    public static void main(String[] args) {

        // Explícito.
        double preco = 10.9999;
        int novoPreco = (int) preco;

        // Implícito.
        int quantidade = 7;
        double novaQuantidade = quantidade;
    }
}
```
