# INFERÊNCIA DE TIPO

Podemos usar a palavra reservada `var` para declarar uma variável.

Assim o Java vai definir o tipo confrome o valor atribuido.

Nesse caso é obrigatório declarar e atribuir um valor a variável na mesma linha.

E claro, só pode alterar o valor por outro do memso tipo.

```java
package fundamentos;

public class InferenciaDeTipo {

    public static void main(String[] args) {

        var fruta = "uva";
        var idade = 32;
    }
}
```
