### 1) Explique qual a função da Máquina Virtual Java (JVM).

1) A JVM tem como função interpretar o bytecode gerado pela compilação de um código Java e o tornar um código de máquina executável. Dessa forma, a JVM é uma máquina virtual que emula a aplicação Java, o que permite que essa aplicação seja executada em diferentes sistemas, dada a condição que esse sistema esteja equipado com sua JVM específica, garantindo a portabilidade e permitindo ao desenvolvedor criar aplicações Java multiplataforma eficientemente.

### 2) Qual a diferença entre JRE e JDK?

2. Apesar de ambos serem relacionados ao Java, o JRE ou Java Runtime enviorament como é autoexplicativo dado o nome, é o ambiente de execução da linguagem Java e serve para executar programas construidos nessa linguagem, e é geralmente utilizado pelos usuários comuns. Nele estão inclusos a JVM, as bibliotecas padrões da linguagem Java e os Class Loaders.
   
   Já, a JDK ou Java Development Kit contém não só a JRE como também um conjunto de outros componentes e utilitários que permitem a criação de programas com a linguagem Java, entre eles: javac - o compilador da linguagem Java, o interpretador Java e uma série de outros utilitiários.

### 3) Crie um programa Java que imprima o seguinte texto “Terminei a primeira aula com um programa Java"

```java
public class QuestaoTres {  

    public static void main(String[] args) {  
        
        System.out.println("Terminei a primeira aula com um programa Java!");

    }  
}
```

### 4) Compile o programa desenvolvido no exercício anterior. A seguir, apague o arquivo ".class" gerado e tente executar o programa. O que aconteceu?

```bash
$ Erro: Não foi possível localizar nem carregar a classe principal QuestaoQuatro
Causada por: java.lang.ClassNotFoundException: QuestaoQuatro
  
```

4. Nos deparamos com o erro acima por que a JVM não achou o bytecode para executar.

### 5) Mude o nome do método “main” para “start”, compile e execute. O que aconteceu?

```bash
$ Erro: o método main não foi encontrado na classe QuestaoCinco; defina o método main como:
   public static void main(String[] args)
ou uma classe de aplicativo JavaFX deve expandir javafx.application.Application
```

5. Ocorreu um erro na execução do programa, que acusou a falta de um método main, impossibilitando o começo da aplicação

### 6) Crie um programa Java para imprimir duas linhas de texto usando duas linhas de código “System.out”, onde aparecerá o seu nome na primeira linha e na segunda linha aparecerá o time para o qual você torce.

```java
public class QuestaoSeis{

    public static void main(String[] args){

        System.out.println("Meu nome é: João");
        System.out.println("Eu torço pro Corinthians");

    }
}
```

### 7) Experimente escrever todo o programa anterior em maiúsculo, compile e execute. O que aconteceu?

```java
PUBLIC CLASS QUESTAOSETE {

    PUBLIC STATIC VOID MAIN(STRING[] ARGS) {

        SYSTEM.OUT.PRINTLN("MEU NOME É: JOÃO");
        SYSTEM.OUT.PRINTLN("EU TORÇO PRO CORINTHIANS");

    }
}
```

```bash
QuestaoSete.java:1: error: class, interface, or enum expected
PUBLIC CLASS QUESTAOSETE {
^
QuestaoSete.java:6: error: class, interface, or enum expected
        SYSTEM.OUT.PRINTLN("EU TORÇO PRO CORINTHIANS");
        ^
QuestaoSete.java:8: error: class, interface, or enum expected
    }
    ^
3 errors

```

7. Não foi possível compilar, pois por uma diversidade de motivos, o código escrito não é um código Java válido.

### 8) Experimente salvar o arquivo com um nome diferente do nome da classe,compile e execute. O que aconteceu?

```bash
$ QuestaoOito.java:1: error: class main is public, should be declared in a file named main.java
public class main {
       ^
1 error

```

8. O erro aconteceu já que meu arquivo não tem o mesmo nome que a classe então ele falhou na compilação. E como o nome da classe é Main, ele indica que o arquivo deve ser chamar Main.java
