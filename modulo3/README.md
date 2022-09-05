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

<img src="https://github.com/mendesrl/js-every/blob/module-3/javascript-funcional/modulo3/funcao-pura-exemplo-1.png" width="500"  />

- **Exemplo-1:** A função retorna um valor de acordo com os seus argumentos de entrada, independente de quando e onde ela é chamada. Sempre que passarmos 2 e 3 sabemos que o resultado será 6. Nada mais afeta o resultado.

<img src="https://github.com/mendesrl/js-every/blob/module-3/javascript-funcional/modulo3/funcao-pura-exemplo-2.png" width="500"  />

- **Exemplo-2:** Funções puras não devem alterar nenhuma variável fora de seu escopo, nesse exemplo a função não alterou os valores do objeto.

<img src="https://github.com/mendesrl/js-every/blob/module-3/javascript-funcional/modulo3/funcao-pura-exemplo-3.png" width="500"  />

- **Exemplo-3:** O map é um método JS associado a função pura, assim como os outros.
  - arr.filter()
  - arr.reduce()
  - arr.each()
  - arr.every()
  - arr.concat()
  - arr.slice()

### Funções Impuras
- É quando uma função ao ser executada causa mudanças no estado da aplicação ela é chamada de função impura.
- Uma função impura altera ou tem seus valores alterados fora do seu **escopo léxico**.

#### O que é escopo léxico?
- É o escopo no qual as fuções foram definidas fisicamente.
- É a capacidade de um escopo de função acessar variáveis do escopo pai.
#### Destrinchando um exemplo de escopo léxico

<img src="https://github.com/mendesrl/js-every/blob/module-3/javascript-funcional/modulo3/escopo-lexico-exemplo-1.png"  />


- No código acima, o valor da variável `num1` é acessível por todos os escopos de função (`funcao()` e `funcaoInterna()`), pois está no escopo global. 
- Enquanto isso, a variável `num2` não é acessível fora da função `funcao()` devido a variável `num2` ser de escopo local. 
- Outro ponto é: a função `funcaoInterna()` pode acessar as variáveis `num2` e `num3`. Isso ocorre porque as funções internas são lexicalmente vinculadas pelas funções externas (função pai).
- Após o entendimento de escopo léxico, voltamos as explicações sobre funções impuras.

#### Exemplo de Funções Impuras
<img src="https://github.com/mendesrl/js-every/blob/module-3/javascript-funcional/modulo3/funcao-impura-exemplo-1.png" width="500"  />

- **Exemplo-1:** `num1` dentro da função `soma()` impacta efeitos colaterais, vejamos:
  - Dependência: `soma()` depender de `num1` pode resultar em erro, caso `num1` por algum motivo ser undefined.
  - Modifica o código externo: a cada chamada de `soma()` o valor de  `num1` é atualizado, alterando o valor de uma variavel fora do seu escopo.

<img src="https://github.com/mendesrl/js-every/blob/module-3/javascript-funcional/modulo3/funcao-impura-exemplo-2.png" width="500"  />

- **Exemplo-2:** Aparentemente `modificandoObj` parece ser pura, mas como estamos modificando o objeto no local, a abordagem acima é considerada impura.


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
