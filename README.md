# Desafio: Criando um Jogo de Sudoku em Java

Projeto desenvolvido como parte do curso **"Coleções e Streams em Java"** da DIO.

O objetivo deste desafio é criar uma aplicação em Java que simule um jogo de Sudoku utilizando os conhecimentos de coleções (`List`, `Map`, `Set`) e `Stream API`.

---

## Como Executar o Projeto

A aplicação aceita como argumento uma sequência de posições iniciais do tabuleiro de Sudoku. Cada valor deve ser informado no seguinte formato:

```
linha,coluna;valor,fixo
```

* `linha` e `coluna`: coordenadas (de 0 a 8)
* `valor`: número entre 1 e 9
* `fixo`: `true` se o valor não pode ser alterado pelo jogador, ou `false` se for editável

### Exemplo de Argumento Completo:

```text
0,0;4,false 1,0;7,false 2,0;9,true 3,0;5,false 4,0;8,true 5,0;6,true 6,0;2,true 7,0;3,false 8,0;1,false
0,1;1,false 1,1;3,true 2,1;5,false 3,1;4,false 4,1;7,true 5,1;2,false 6,1;8,false 7,1;9,true 8,1;6,true
0,2;2,false 1,2;6,true 2,2;8,false 3,2;9,false 4,2;1,true 5,2;3,false 6,2;7,false 7,2;4,false 8,2;5,true
0,3;5,true 1,3;1,false 2,3;3,true 3,3;7,false 4,3;6,false 5,3;4,false 6,3;9,false 7,3;8,true 8,3;2,false
0,4;8,false 1,4;9,true 2,4;7,false 3,4;1,true 4,4;2,true 5,4;5,true 6,4;3,false 7,4;6,true 8,4;4,false
0,5;6,false 1,5;4,true 2,5;2,false 3,5;3,false 4,5;9,false 5,5;8,false 6,5;1,true 7,5;5,false 8,5;7,true
0,6;7,true 1,6;5,false 2,6;4,false 3,6;2,false 4,6;3,true 5,6;9,false 6,6;6,false 7,6;1,true 8,6;8,false
0,7;9,true 1,7;8,true 2,7;1,false 3,7;6,false 4,7;4,true 5,7;7,false 6,7;5,false 7,7;2,true 8,7;3,false
0,8;3,false 1,8;2,false 2,8;6,true 3,8;8,true 4,8;5,true 5,8;1,false 6,8;4,true 7,8;7,false 8,8;9,false
```

> 💡 **Dica:** Para facilitar a execução, copie a linha de argumentos e cole na hora de rodar o projeto.

---

## Funcionalidades

* Leitura de configuração inicial via argumentos
* Preenchimento interativo do tabuleiro
* Verificação de regras do Sudoku
* Diferenciação entre valores fixos e editáveis
* Uso de coleções Java (`Map`, `List`) para armazenar o estado do jogo
* Aplicação de `Streams` para filtragem, validação e exibição de dados
