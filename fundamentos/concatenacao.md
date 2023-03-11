# CONCATENAÇÃO

```java
package fundamentos;

public class EntradaDadosTeclado {

    public static void main(String[] args) {

        String nome = "Weverton";
        String sobrenome = "Teixeira";
        int idade = 32;
        double salario = 4200.00;

        // Exemplo 1.
        String funcionario = nome + " " + sobrenome + " " + idade + " " + salario;

        // Exemplo 2.
        funcionario = String.format("%s %s %d %.2f", nome, sobrenome, 32, 3500.00);
    }
}
