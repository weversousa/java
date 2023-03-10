# JAVA

## CONCEITOS BÁSICOS

Para desenvolver em JAVA é preciso ter instalado em seu computador o \
`JDK - Java Development Kit`.

Os códigos em JAVA são escritos em arquivos `.java` dentro da pasta `src/`, e \
ao serem compilados são criados arquivos `.class` com os mesmos nomes dentro \
da pasta `bin/`, o resultado do `.class` é conhecido como `ByteCode`.

Esses arquivos `.class` podem ser lidos por qualquer dispositivo que tenha \
instalado nele o `JRE - Java Runtime Enviroment`, pois ele possui a \
`JMV - Java Virtual Machine` que é responsável em traduzir o `ByteCode` para a \
`JRE` da máquina.

Cada dispositivo (Linux, Windows, Mac, Android, ...) tem um tipo de `JRE`, \
porém todos eles entendem o `ByteCode` devido a `JVM`.

**_"Escreva uma vez e rode em qualquer lugar._"**

As IDEs compilam automaticamente quando executamos nosso código `.java`.

```bash
# Compilar de forma manual via terminal.
javac FileName.java
```

```bash
# Executar de forma manual via terminal.
java FileName.class
```

---

## COMENTÁRIOS

```java
package fundamentos;

public class Comentario {

    /**
     * javadoc
     *
     * @author Weverton Teixeira <...@email.com>
     * @since JDK1.0
     */

    public static void main(String[] args) {

        // Comentário de uma linha.

        /*
         * Comentário
         * de múltiplas
         * linhas.
         */
    }
}
```

## VARIÁVEL

`tipo nome = valor;`

`tipo nome;` \
`nome = valor;`

## CONSTANTE

`final tipo nome = valor;`

## TIPOS DE DADOS

### PRIMITIVOS / VERSÃO OBJETO

```java
package fundamentos;

public class TiposDados {

    public static void main(String[] args) {

        double preco = 1.99;
        final double PI = 3.14153;
        boolean aprovado = true;
        char simbolo = '#';
    }
}
```

**Números inteiros**:
* byte / Byte
* short / Short
* int (padrão) - Integer
* long / Long

**Números reais**:
* float - Float
* double (padrão) / Double

**Lógico**:
* boolean / Boolean

**1 caractere**:
* char / Character

### STRING

```java
package fundamentos;

public class Textos {

    public static void main(String[] args) {

        String nome = "Weverton";
        String sobrenome = "Teixeira";
    }
}
```

### INFERÊNCIA DE TIPO

```java
package fundamentos;

public class Textos {

    public static void main(String[] args) {

        // Nesses casos é obrigatório declarar e atribuir um valor a variável na mesma linha.
        var fruta = "uva";
        var idade = 32;
    }
}
```

### CAST

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

### CONVERSÃO

```java
package fundamentos;

public class Conversao {

    public static void main(String[] args) {

        // Número -> String 
        int numeroPrimitivo = 10;

        Integer numeroObjeto = numeroPrimitivo;
        String numeroString = numeroObjeto.toString();

        numeroString = Integer.toString(numeroPrimitivo);

        numeroString = numeroPrimitivo + "";


        // String -> Número
        numeroPrimitivo = Integer.parseInt("5");
    }
}
```

## CONCATENAÇÃO

```java
package fundamentos;

public class EntradaDadosTeclado {

    public static void main(String[] args) {

        String nome = "Weverton";
        String sobrenome = "Teixeira";
        int idade = 32;
        double salario = 4200.00;
        
        String funcionario = nome + " " + sobrenome + " " + idade + " " + salario;
        nomeCompleto = String.format("%s %s %d %.2f", nome, sobrenome, 32, 3500.00);
    }
}
```

## ENTRADA DE DADOS PELO TECLADO

```java
package fundamentos;

import java.util.Scanner;

import javax.swing.JOptionPane;

public class EntradaDadosTeclado {

    public static void main(String[] args) {

        Scanner entrada = new Scanner(System.in);
            System.out.println("Digite a sua idade: ");
            int idade = entrada.nextInt();

            System.out.println("Digite o seu nome: ");
            String nome = entrada.nextLine();

            System.out.printf("%s %d", nome, idade);
        entrada.close();

        String cor = JOptionPane.showInputDialog("Digite a sua cor: ");
        System.out.println(cor);
    }
}
```

## OPERADORES

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

        // == para String (equals)
        System.out.println("uva".equalsIgnoreCase(" uva ".trim()));

        // ATRIBUIÇÃO
        int n = 1;
        n += 1;
        n -= 1;
        n *= 1;
        n /= 1;
        n %= 1;

        // n = n + 1;
        n++;
        ++n;

        // n = n - 1;
        n--;
        --n;

        int a = 1;
        int b = 2;

        System.out.println(++a == b--);
        /*
         * Primeiro, A vai receber 1 e com isso passará a valer 2.
         * Depois, já vai ser comparado A com B.
         * Por último, B vai receber mais 1 e com isso passará a valer 3.
         */

        System.out.println(a == b);
        // Então aqui sim será false.

        // TERNÁRIO
        double idade = 18;
        String resultado = idade >= 18 ? "maior" : "menor";
    }
}
```
