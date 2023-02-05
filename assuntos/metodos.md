---
title: "Métodos"
author: Kézia Lima
date: 04/02/2023
institute: IFRN@IFRN
---

# Métodos

## O que são métodos e porquê utiliza-los?

Um método é uma coleção de instruções para executar uma determinada tarefa ou operação. Nós escrevemos um método uma vez e o usamos várias vezes, sem que haja a necessidade de ficar reescrevendo o mesmo código. Os métodos são usados para alcançar a reutilização do código, além de também fornecer a fácil modificação e legibilidade do código, apenas adicionando ou removendo um pedaço de código.

**O método é executado apenas quando o chamamos ou o invocamos.**

Exemplo do dia a dia: 

Todos os dias precisamos comer, dormir e fazer nossas necessidades.
Imagine que para cada uma dessas ações o cérebro envia um comando para nosso corpo. O que é mais fácil e rápido para o cerebro: o corpo já saber o que fazer ou o corpo ter que todo dia ser ensinado como deve fazer tal ação?

Vejamos isso em forma de codigo: 
```java
public class CorpoHumano{

	public static void main(String[] args) {
        //dia 1
	    comer(); //sempre que estiver com fome, só chamar o método comer() e nele já vai conter como comer

        //dia 2
        comer();
	}

	public static void comer(){
	    
	    String prato = "muita comida";
	    
	    if(prato == "muita comida"){
	        System.out.println("pegar colher\ncolocar colher na boca\ntirar colher da boca\npegar mais comida");
	    } else {
	        System.out.println("estou satisfeite");
	    }
	   
	}
}
```

ou 

```java
public class CorpoHumano{

	public static void main(String[] args) {

        //dia 1
	    String prato = "muita comida";
	    
	    if(prato == "muita comida"){
	        System.out.println("pegar colher\ncolocar colher na boca\ntirar colher da boca\npegar mais comida");
	    } else {
	        System.out.println("estou satisfeita");
	    }

	    //dia 2
	    if(prato == "muita comida"){
	        System.out.println("pegar colher\ncolocar colher na boca\ntirar colher da boca\npegar mais comida");
	    } else {
	        System.out.println("estou satisfeite");
	    }
    }
}
```

Com certeza você achou o primeiro código a melhor forma para o seu corpo fazer uma ação.


## Quando utilizá-los?

Vejamos que no segundo código estamos utilizando o mesmo comando várias vezes, este é o sinal para fazermos um método!

![](image.png)


## Declarando Métodos


A declaração de um metodo é bem simples.
Veja o exemplo abaixo de um método de soma: 

```java
public static int somar(int a, int b){
    return a + b;
}
```
*Exemplo 1 - Método de soma*

### Visibilidade

OBS: **Todos os métodos que estamos estudando iniciarão com:**

```java
public static
```

Essas duas palavrinhas vocês não precisam se preocupar agora, mas para não deixar vocês por fora...

**public:** Representa o tipo de visibilidade do método. Ele faz com que o método consiga ser acessado por qualquer classe.

**static:** Serve para referenciar que o método podem ser acessados diretamente da definição da classe, sem precisar instanciar nenhum objeto.

### Retorno 

```java
int somar(int a, int b){
    return a + b
}
```
**int:** Está repesenta que esse método, obrigatoriamente, deverá retornar um número inteiro.
Além de **int**, temos também:

* double
* String
* boolean
* float
* long
* entre outros. 

Além desses, ainda existe o **void** que não retorna a nada, ou seja, este metodo não necessitar por a palavra **return**.


### Nome do método

**somar:** Representa o nome do método.

Aqui vale ressaltar que os nomes dos métodos devem ser auto-explicativos, isto é, não faz sentido nomear de `comer` um método que te faz tomar banho.

```java
public static void comer() {
	System.out.println("Abrir choveiro");
	System.out.println("Tomar um banho bom");
}
```
Queeeee?!

### Parâmetros

Outra vantagem em utiliar métodos é que conseguimos gerar diferentes comportamentos de acordo com parâmetros informados. No *Exemplo 1* são definidos dois parâmetros:

- **int a**: o primeiro parâmetro informado deverá ser um inteiro e será identificado como `a`
- **int b**: o último parâmetro informado...

De forma geral, ainda temos as seguintes características de parâmetros:

- Os métodos podem possuir diversos parâmetros
- É permitido definir parâmetros com diferentes tipos

```java
public static void main(String[] args) {
	somar(6, 18);
	comer(); // método sem parâmetro
	removaTodosChars('o', "Calouro"); // diferentes tipos :)
}
```
*Exemplo 2 - Passar parâmetros para métodos*

____

Questões para treinar:

* [Soma Simples](https://www.beecrowd.com.br/judge/pt/problems/view/1003)

* [O Maior](https://www.beecrowd.com.br/judge/pt/problems/view/1013)

* [Formula de Bhaskara](https://www.beecrowd.com.br/judge/pt/problems/view/1036)

**Façam as questões usando métodos**