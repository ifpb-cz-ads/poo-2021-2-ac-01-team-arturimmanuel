### 3) Crie um programa Java que imprima o seguinte texto “Terminei a primeira aula com um programa Java"

### 1) Explique qual a função da Máquina Virtual Java (JVM).

1) A JVM tem como função interpretar o bytecode gerado pela compilação de um código Java e o tornar um código de máquina executável. Dessa forma, a JVM é uma máquina virtual que emula a aplicação Java, o que permite que essa aplicação seja executada em diferentes sistemas, dada a condição que esse sistema esteja equipado com sua JVM específica, garantindo a portabilidade e permitindo ao desenvolvedor criar aplicações Java multiplataforma eficientemente.

### 2) Qual a diferença entre JRE e JDK?

2. Apesar de ambos serem relacionados ao Java, o JRE ou Java Runtime enviorament como é autoexplicativo dado o nome, é o ambiente de execução da linguagem Java e serve para executar programas construidos nessa linguagem, e é geralmente utilizado pelos usuários comuns. Nele estão inclusos a JVM, as bibliotecas padrões da linguagem Java e os Class Loaders.
   
   Já, a JDK ou Java Development Kit contém não só a JRE como também um conjunto de outros componentes e utilitários que permitem a criação de programas com a linguagem Java, entre eles: javac - o compilador da linguagem Java, o interpretador Java e uma série de outros utilitiários.

### 3) Crie um programa Java que imprima o seguinte texto “Terminei a primeira aula com um programa Java"

```
public class Main {  
 public static void main(String[] args) {  
     System.out.println("Terminei a primeira aula com um programa Java!");  
 }  
}
```
