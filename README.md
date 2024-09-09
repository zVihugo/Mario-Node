# 🚗 Corrida de Personagens - Simulação em JavaScript

Este é um projeto simples de simulação de corrida entre dois personagens, Mario e Luigi, utilizando atributos como **Velocidade**, **Manobrabilidade** e **Poder**. O jogo é composto por várias rodadas, onde o resultado da corrida é determinado pelo lançamento de dados e testes de habilidade com base nos atributos dos personagens.

## 🎮 Personagens

### Player 1 - Mario
- **Nome**: Mario
- **Velocidade**: 4
- **Manobrabilidade**: 3
- **Poder**: 2
- **Pontos**: 0 (inicial)

### Player 2 - Luigi
- **Nome**: Luigi
- **Velocidade**: 3
- **Manobrabilidade**: 4
- **Poder**: 3
- **Pontos**: 0 (inicial)

## ⚙️ Funcionalidades

1. **Lançamento de Dados**: A função `rollDice()` retorna um valor aleatório entre 0 e 5, simulando um lançamento de dados.
   
2. **Blocos de Corrida**:
   - **Reta**: Testa a velocidade dos personagens.
   - **Curva**: Testa a manobrabilidade dos personagens.
   - **Confronto**: Os personagens se enfrentam com base no atributo de poder. O perdedor perde 1 ponto.

3. **Simulação de Rodadas**: Cada rodada é composta por um bloco de corrida (Reta, Curva ou Confronto), que é sorteado aleatoriamente. Os personagens lançam os dados e somam os resultados aos seus atributos para determinar o vencedor da rodada.

4. **Declaração do Vencedor**: Após cinco rodadas, o vencedor é determinado com base nos pontos acumulados.

## 🚀 Como Executar

Para executar o projeto, basta ter o [Node.js](https://nodejs.org/) instalado e seguir os passos abaixo:

1. Clone este repositório:
   ```bash
   git clone https://github.com/seu-usuario/nome-do-repositorio.git

2. Navegue até o diretório do repositório:
   ```bash
   cd nome-do-repositorio

3. Execute o script
   ```bash
   node nome-do-arquivo.js

### 🛠️ Estrutura do Código
  - player1 e player2: Objetos que representam os personagens da corrida.
  - rollDice(): Função que retorna o resultado do dado.
  - getRandomBlock(): Função que sorteia o bloco da corrida (Reta, Curva ou Confronto).
  - logRollResult(): Função que exibe os resultados das rolagens de dados.
  - playerRaceEngine(): Função que executa a lógica das rodadas da corrida.
  - declareWinner(): Função que declara o vencedor com base nos pontos acumulados.

### Exemplo de execução:
```bash
🏁 Iniciando corrida entre Mario e Luigi....

🎲 Rodada 1 🎲
Bloco: CURVA
Mario rolou um dado de Manobrabilidade 3 + 3 = 6
Luigi rolou um dado de Manobrabilidade 4 + 4 = 8
Luigi marcou um ponto!
-----------------------------

... (demais rodadas)

Resultado final:
Mario: 2 ponto(s)
Luigi: 3 ponto(s)

Luigi venceu a corrida! Parabéns! 🏆
