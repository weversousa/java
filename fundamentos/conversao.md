# CONVERSÃO

```java
package fundamentos;

public class Conversao {

    public static void main(String[] args) {

        int numeroPrimitivo = 10;


        // Exemplo 1: Número -> String
        Integer numeroObjeto = numeroPrimitivo;
        String numeroString = numeroObjeto.toString();

        // Exemplo 2: Número -> String
        numeroString = Integer.toString(numeroPrimitivo);

        // Exemplo 3: Número -> String.
        numeroString = numeroPrimitivo + "";


        // String -> Número
        numeroPrimitivo = Integer.parseInt("5");
    }
}
```
