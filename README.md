# Desafio 01 - Dio e meutudo.

## Simulador de partidas do Mario Kart com Node.js
Conteúdo de Back-End.

### Objetivo:
Mario Kart é uma série de jogos de corrida desenvolvida e publicada pela Nintendo. Nosso desafio será criar uma lógica de um jogo de vídeo game para simular corridas de Mario Kart, levando em consideração as regras mecânicas abaixo:

| Personagem | Velocidade | Manobrabilidade | Poder |
| ---------- | ---------- | --------------- | ------ |
| Mario | 4 | 3 | 3 |
| Peach | 3 | 4 | 2 |
| Yoshi | 2 | 4 | 3 |
| Bowser | 5 | 2 | 5 |
| Luigi | 3 | 4 | 4 |
| Donkey Kong | 2 | 2 | 5 |

### Intuitos do projeto:
- testar a lógica de programação.
- rever conceitos de JavaScript.
- entender como funciona um pacote básico do Node.
- insights de melhoria de organização de código.

### Regras de negócio (como funciona o conteúdo do jogo):

*Sobre os Jogadores*
- O Computador deve receber dois personagens para disputar a corrida em um objeto cada.

*Sobre as Pistas*
- Os personagens irão correr em uma pista aleatória de 5 rodadas.
- A cada rodada, será sorteado um bloco de pista que pode ser uma reta, curva ou confronto.
    - Caso o bloco da pista seja uma RETA, o jogador deve jogar um dado de 6 lados e somar o atributo VELOCIDADE, quem vencer ganha um ponto.
    - Caso o bloco da pista seja uma CURVA, o jogador deve jogar um dado de 6 lados e somar o atributo MANOBRABILIDADE, quem vencer ganha um ponto.
    - Caso o bloco da pista seja um CONFRONTO, o jogador deve jogar um dado de 6 lados e somar o atributo PODER, quem perder, perde um ponto.
    - Nenhum jogador pode ter pontuação negativa (valores abaixo de 0).

*Condição de Vitória*
- Ao final, vence quem acumulou mais pontos.