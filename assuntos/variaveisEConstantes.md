# Variáveis e Constantes

Quando estamos desenvolvendo algumas aplicações, é importante armazenarmos algumas informações que poderão ser usadas durante todo o nosso código. Para isso, usamos as **variáveis** e também as **constantes**. 

## O que é uma variável?

Uma variável é como uma caixinha, na qual, como o próprio nome já sugere, eu posso sempre estar mudando o conteúdo de dentro dela.

As variáveis sempre possuem um tipo específico de dado, e os objetos que variam dentro dela precisam ter o mesmo tipo.

Imagine uma caixinha de anel. Nessa caixinha, eu só posso guardar anéis. No momento que eu quiser, posso mudar o anel que está dentro da minha caixinha para um outro novo. É exatamente assim que funciona uma variável.

As variáveis podem receber diferentes tipos de dados. Segue a lista:

### Principais tipos de dados: 
- `int`
- `double`
- `String`
- `float`

### Como declarar uma variável?

Para declarar, é bem simples: basta colocar o tipo e o nome que você quer para a variável (coloquem nomes sugestivos em suas variáveis; fica mais fácil de entender o que você está guardando dentro dela).

Exemplo:

```java
public class Exemplo {
    public static void main(String[] args) {
        int numero1 = 1;
        int numero2;
        String palavra = "oi";
    }
}
```
## E o que é uma constante?

Uma constante tem a mesma finalidade que as variáveis, possui os mesmos tipos, mas o seu diferencial é que o seu conteúdo nunca mudará.
Como declarar uma constante?

As constantes sempre possuem um valor fixo. Um exemplo disso é o número PI, que sempre é representado pelo valor 3,14.

#### Exemplo:

```java

public class Exemplo {
    public static final int MINHA_CONSTANTE = 10;

    public static void main(String[] args) {
        System.out.println("O valor da constante é: " + MINHA_CONSTANTE);
    }
}
```

Note que o nome da minha constante é totalmente maiúsculo, separado por "_" e pertence ao escopo global.

## Importante

- Variáveis sempre precisam ter o nome iniciado com letra minúscula, sem caracteres especiais ou acentos!
- Em Java, utilizamos o formato camelCase. A segunda palavra deixamos com a inicial maiúscula.
Exemplo: ```String formatoNomeVariavel = "camelCase";```