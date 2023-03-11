# TIPOS DE DADOS

## PRIMITIVOS

### NÚMEROS INTEIROS

| TIPO  | BITS | FAIXA                 | PADRÃO |
| :-:   | :-:  | :-:                   | :-:    |
| byte  | 8    | -128 a 127            | 0      |
| short | 16   | -32.768 a 32.767      | 0      |
| int   | 32   | -2³¹ a 2³¹ – 1        | 0      |
| long  | 64   | -2 ** 63 a 2 ** 63 -1 | 0L     |

###  NÚMEROS DE PONTO FLUTUANTE

| TIPO   | BITS | FAIXA                                                         | PADRÃO |
| :-:    | :-:  | :-:                                                           | :-:    |
| float  | 32   | IEEE 754 ±1,40129846432481707e-45 a 3,40282346638528860e+38   | 0.0F   |
| double | 64   | IEEE 754 ±4,94065645841246544e-324 a 1,79769313486231570e+308 | 0.0    |

### UNICODE

| TIPO  | BITS | FAIXA               | PADRÃO   |
| :-:   | :-:  | :-:                 | :-:      |
| char  | 16   | ‘\u0000’ a ‘\uffff’ | ‘\u0000’ |

### BOOLEAN

| TIPO    | BITS | FAIXA         | PADRÃO |
| :-:     | :-:  | :-:           | :-:    |
| boolean | 1    | true ou false | false  |

## STRING

* Um ou uma sequência de caracteres entre aspas duplas.
* Cria um objeto e por isso tem métodos e comportamentos através da **notação ponto**.

```java
package fundamentos;

public class TiposDeDados {

    public static void main(String[] args) {

        int quantidade = 128;
        double preco = 1.99;
        char sexo = 'M';
        String nome = "Weverton";
        boolean casado = false;
        
        // Por padrão o java infere double, para forçar o float inserir o F.
        float troco  = 1.99F;
        
        // Por padrão o java infere int.
        byte total = 100B;
        byte itens = 30000S;
    }
}
```

## VERSÃO OBJETO DOS PRIMITIVOS

* Byte
* Short
* Integer
* Long
* Character
* Boolean

Por ser um objeto, faz com que os tipos primitivos tenham a notação ponto.

Auxiliam por exemplo na conversão de um Primitivo para String, entre outras coisas.
