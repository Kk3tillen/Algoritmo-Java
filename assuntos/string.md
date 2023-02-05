---
title: "Métodos"
author: Kézia Lima
date: 04/02/2023
institute: IFRN@IFRN
---

# Métodos String

Os métodos String servem para a manipulação de Strings.
Quando pensarmos em uma **String** devemos pensar sempre em um array/vetor. Cada letra está em um posição.


![](../vetor.png)

Aqui vai o exemplo de alguns métodos:

## charAt()

O nosso primeiro método é bem simples e consiste em retornar apenas um caractere em determinada posição de nossa String.

exemplo de utilização:

```java
String text= "Algoritmo";
System.out.println(text.charAt(0));
```
teremos como output a letra **A**.

## split()

O método split cria um array/vetor de Strings com base no paramêtro passado, dividindo uma String em várias outras Strings.

```java
String text= "Algoritmo.é.muito.legal";
String[] textComSplit = text.split(".");

for(int i = 0; i < textComSplit.length; i++){
    System.out.println(textComSplit(i));
}
```
Isso imprimi-rá na tela a frase:

```
Algoritmo

é

muito

legal
```

Imagine como se cada palavra estivesse em um quadradinho, assim como na primeira imagem.

## length()

O método *length()* retorna o tamanho da String.

```java
String text= "Algoritmo";
int tamanhoDoText = text.length();

System.out.println("O tamanho do texto é: " + tamanhoDoText);
```
isso nos retornará: 
```
O tamanho do texto é: 8
```

## equals()

Comapara duas String

```java
String myStr1 = "oi";
String myStr2 = "oi";
String myStr3 = "outra string";
System.out.println(myStr1.equals(myStr2)); 
System.out.println(myStr1.equals(myStr3)); 
```
output
```
true
false
```

## replace

Substitui as letras de acordo com os parametros que foram passados.

```java
String myStr = "Hello";
System.out.println(myStr.replace('l', 'p'));
```
output
```
Heppo
```

`replace('l', 'p')`

* **l** é a letra que queremos mudar

* **p** letra que irá substituir **l**

## toLowerCase() e toUpperCase()
* toLowerCase() deixa todas a letras da frase/palavra minúscula. 
* toUpperCase() deixa todas a letras da frase/palavra maiúscula.
  
exemplo:

```java
String txt = "Hello World";
System.out.println(txt.toUpperCase());
System.out.println(txt.toLowerCase());
```

output
```
HELLO WORLD
hello world
```

[clique aqui para ver mais exemplos](https://docs.oracle.com/javase/7/docs/api/java/lang/String.html)