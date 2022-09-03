# Modulo 3 - Javascript Funcional

## Funções Puras
- Uma função em que seu valor de retorno é determinado por seus valores de entrada.
- Não Existe dependência externa.
- Os valores são passados como parâmetros.
- Não tem efeitos colaterais.

### Checklist para criar uma função pura
- [x] O nome da função deve ser claro e condizente com seu comportamento.
- [x] Os tipos de entrada devem ser validados. 
- [x] As funçãoes e varáveis impactadas devem ser declaradas dentro do seu proprio escopo.

#### Exemplo de Funções Puras
No Exemplo 1, a função retorna um valor de acordo com os seus argumentos de entrada, independente de quando e onde ela é chamada. Sempre que passarmos 2 e 3 sabemos que o resultado será 6. Nada mais afeta o resultado.

<img src="https://github.com/mendesrl/js-every/blob/module-3/javascript-funcional/modulo3/funcao-pura-exemplo-1.png" width="500"  />

Funções puras não devem alterar nenhuma variável fora de seu escopo, o Exemplo 2 mostra que a função não alterou os valores do objeto.

<img src="https://github.com/mendesrl/js-every/blob/module-3/javascript-funcional/modulo3/funcao-pura-exemplo-2.png" width="500"  />

Os métodos JS abaixo são normalmente associados a funções puras, veja o map no Exemplo-3.
- arr.map()
- arr.filter()
- arr.reduce()
- arr.each()
- arr.every()
- arr.concat()
- arr.slice()

<img src="https://github.com/mendesrl/js-every/blob/module-3/javascript-funcional/modulo3/funcao-pura-exemplo-3.png" width="500"  />

### Funções Impuras
- É quando uma função ao ser executada causa mudanças no estado da aplicação ela é chamada de função impura.
- Uma função impura altera ou tem seus valores alterados fora do seu **escopo léxico**.

#### O que é escopo léxico?
- É o escopo no qual as fuções foram definidas fisicamente.
- É a capacidade de um escopo de função acessar variáveis do escopo pai.
#### Destrinchando um exemplo de escopo léxico
- No código acima, o valor da variável `num1` é acessível por todos os escopos de função (`funcao()` e `funcaoInterna()`), pois está no escopo global. 
- Enquanto isso, a variável `num2` não é acessível fora da função `funcao()` devido a variável `num2` ser de escopo local. 
- Outra ponto é: a função `funcaoInterna()` pode acessar as variáveis `num2` e `num3`. Isso ocorre porque as funções internas são lexicalmente vinculadas pelas funções externas(função pai).
#### Exemplo de Funções Impuras
-
-
-

## Imutabilidade
#### Exemplo de Imutabilidade
-

## Recursividade
#### Exemplo de Recursividade
-

## High Order Functions
#### Exemplo de High Order Functions
-
-
-

## Currying
#### Exemplo de Currying
-
-
-

## O que é callback hell e como evitar?
