# IF

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
