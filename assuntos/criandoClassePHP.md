# Como Criar uma classe em PHP

Antes de começar fazendo os metodos e criando atributos eu preciso sempre definir que aquilo é realmente um classe, então é necessario sempre colocar antes de qualquer coisa:

**passo 1**
```PHP
    class NomeDaClasse{

    }
```
 **Atenção!!**

 **lembre-se sempre que nome de classe se iniciam sempre com letra Maiuscula!**

Em seguida, defina quais atributos você utilizará em sua classe. Lembre-se que sua classe é algo generico, então esse atributo precisa servir para todos os casos. No exemplo abaixo, os atributos nome e idade foram utilizados pelo fato de que todas as pessoas possuem um nome e uma idade. 

 **passo 2**
 ```PHP
    class Pessoa {
        private $nome; 
        private $idade;
    }
```

os atributos são informações importantes, por isso, não podemos deixar que outras pessoas tenham acesso tão facilmente a ela, então, antes do nome de cada atributo, adicionamos o tipo de visibilidade PRIVATE. Porém, de alguma forma precisamos manipular os valores, para isso utilizamos os getters e setters:

**passo 3**

 ```PHP
 public function Pessoa(){

    private $nome; 
    private $idade;

    public function getNome() { //lembrar sempre que o get vai me dar algo então, ele sempre terá o return.
        return $this->nome;
    }
    public function setNome($nome) { //lembrar sempre que o set vai adicionar alguma coisa, então sempre vai ter um paramentro.
        $this->nome = $nome; //Atenção ao $ antes do $ e a falta dele no nome da variável
    }

    public function getIdade() {
        return $this->idade;
    }
    public function setNome($idade) {
        $this->idade = $idade;
    }
 }
```
para cada atributo é necessário fazer um get e um set.


como utilizar e manipular os valores dos atributos de um objeto
```PHP
<?
    $obj1 = new $Pessoa; //criando um objeto do tipo pessoa
    $obj1->setNome = Francielen; //Adiciona um nome a variável

    echo $obj1->getNome();  //imprime o conteudo da variável nome;
?>
```





