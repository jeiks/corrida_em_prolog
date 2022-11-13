# Corrida em Prolog

Trabalho Prático da Disciplina de Inteligência Artificial.

Este trabalho foi desenvolvido como trabalho prático da disciplina de Inteligência Artificial.

A parte em HTML/JS/CSS foi gerada à partir do código do *Radu Mariescu-Istodor*, disponível em seu [github](https://github.com/gniziemazity/Self-driving-car).

As modificações foram: a quantidade e posição dos carrinhos, o tamanho da pista, a colisão entre os carrinhos e a adequação do código com o [SWI-Prolog](https://www.swi-prolog.org/).

O objetivo passado aos alunos foi de implementar em Prolog o código necessário para que o carrinho controlado possa ganhar a corrida.

[![Corrida em Prolog](https://img.youtube.com/vi/O5NWlz6S4zM/0.jpg)](https://www.youtube.com/watch?v=O5NWlz6S4zM)

### Como executar o servidor

Primeiro, instale o [SWI-Prolog](https://www.swi-prolog.org/). Em distribuições baseadas na Debian (como Ubuntu), basta executar:
```sh
sudo apt install swi-prolog
```

Faça o download do código:
```sh
git clone https://github.com/jeiks/corrida_em_prolog
```

Então, modifique a linha 10 do arquivo ```main.js``` para ```const use_prolog = true;``` e execute o comando:

```sh
cd corrida_em_prolog
swipl -s servidor.pl
```

O servidor já iniciará automaticamente e exibirá a seguinte mensagem:
```sh
   --========================================--

   % Started server at http://localhost:8080/


   --========================================--
```

Agora então, é só abrir um navegador de Internet (testado no Brave - derivação do Chrome) e acessar o endereço acima (http://localhost:8080/).

Na implementação atual em Prolog, a única ação informada é para acelerar o carro, mas se você deixar a linha 10 do arquivo ```main.js``` igual a ```const use_prolog = false;```, você poderá controlar o carrinho com as setinhas do teclado.

Outras informações:
* Para controlar o carro usando as setas do teclado ou o Prolog, modifique o arquivo 'main.js', linha 10 (false ou true);
* A criação de mais carros e o tamanho da pista é também definido no 'main.js', linhas 16-29;
* O script em prolog só vai funcionar se todas as regras estiverem certas.

Have fun =)

