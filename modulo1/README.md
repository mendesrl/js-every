# Modulo 1

## Event Loop

- Estudando para concluir o primeiro módulo do curso JS.every(), encontrei este video no youtube [Mas que diabos é o loop de eventos? | Philip Roberts | JSConf EU](https://www.youtube.com/watch?v=8aGhZQkoFbQ&t=31s), onde o palestrante Philip, demostra a partir de uma ferramenta chamada [Loupe](http://latentflip.com/loupe/) como a call stack,event loop e callback queue interagem entre si.

## Anotações/ilustrações durante o estudo
###  Memory Heap/Heap de Memória
é onde o javascript armazena e escreve informações de forma não ordenada,podemos assimilar com um armário.


![](https://github.com/mendesrl/js-every/blob/module-1/javascript-everyone/memory_heap.jpg)

### Call Stack/Pilha de Chamadas
Ajuda a nos situar no código, para que as instruções sejam executadas em ordem, onde o ultimo item inserido é o primeiro a sair,podemos assimilar com um bloco de notas.


![](https://github.com/mendesrl/js-every/blob/module-1/javascript-everyone/call_stack.jpg)

### Callback Queue/Fila de Retorno de Chamada
Quando uma função assincrona é invocada,ela é adicionada a uma lista de espera e aguarda a execução,podemos assimilar como uma fila de espera.


![](https://github.com/mendesrl/js-every/blob/module-1/javascript-everyone/callback_queue.jpeg)

### Event Loop/Loop de Eventos
É ele o responsável por olhar para a pilha e fila e fazer o gerenciamento. Aqui utilizei a ferramenta Loupe pára ilustrar toda a interação do evento.

![](https://github.com/mendesrl/js-every/blob/module-1/javascript-everyone/event_loop.gif)

## Conclusão
O javascript não faz varias coisas ao mesmo tempo, ele executa uma coisa por vez, porém o NAVEGADOR disponibiliza outros recursos que auxiliam no gerenciamento.
