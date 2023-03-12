# JAVA

## FUNDAMENTOS

* [Comentários](./fundamentos/comentarios.md)
* [Variável e Constante](./fundamentos/variavel_e_constante.md)
* [Tipos de Dados](./fundamentos/tipos_de_dados.md)
* [Inferência de Tipo](./fundamentos/inferencia_de_tipo.md)
* [Coerção de Tipo - (CAST)](./fundamentos/coercao.md)
* [Conversão de Tipo](./fundamentos/conversao.md)
* [Concatenação de Dados](./fundamentos/concatenacao.md)
* [Operadores](./fundamentos/operadores.md)
* [Entrada de Dados via Teclado](./fundamentos/entrada_de_dados_pelo_teclado.md)

## ESTRUTURAS DE CONTROLE

* [Condição](./controle/condicao.md)
* [Repetição](./controle/repeticao.md)
* [Continuar](./controle/repeticao.md)
* [Quebrar](./controle/repeticao.md)

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
