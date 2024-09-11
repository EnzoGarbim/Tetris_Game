# Tetris Game 🎮
### Este é um jogo de Tetris desenvolvido em C# usando WPF (Windows Presentation Foundation). O projeto implementa a lógica básica do jogo, incluindo movimentação das peças, rotação, detecção de colisões e preenchimento de linhas.

## 📋 Funcionalidades
### Movimentação das peças: O jogador pode mover as peças para a esquerda, direita e para baixo, além de girá-las em sentido horário e anti-horário.
### Gravidade: As peças caem automaticamente conforme o tempo passa.
### Detecção de colisão: O jogo detecta quando uma peça atinge o fundo da tela ou outras peças e se ajusta adequadamente.
### Remoção de linhas completas: Linhas completas são removidas, e os blocos acima delas são movidos para baixo.
### Game Over: O jogo termina quando as peças não podem mais ser colocadas no grid.
### Score (Pontuação): Sistema de pontuação baseado em linhas removidas.
### Guarda de peça (Hold): O jogador pode guardar uma peça para uso posterior (tecla C).
### Drop rápido (Fast Drop): O jogador pode fazer a peça cair instantaneamente até o fundo (tecla Espaço).
### Aumento de dificuldade: O jogo fica mais rápido conforme o jogador acumula pontos, aumentando o desafio.
## 🚀 Requisitos
### Para rodar este projeto, você precisará de:

### .NET Framework 8
### Visual Studio
## 🛠️ Estrutura do Projeto
### Arquivos Principais
#### GameState.cs: Contém a lógica principal do jogo, gerenciando a movimentação das peças, colisões e a criação de novas peças.
#### MainWindow.xaml: Define a interface gráfica do usuário, incluindo o canvas onde o jogo é desenhado.
#### MainWindow.xaml.cs: Contém a lógica de interação do usuário e o loop principal do jogo.
#### Block.cs: Representa as peças do jogo (os Tetrominos) e suas posições.
#### GameGrid.cs: Gerencia a grade onde as peças se movem e a detecção de colisões.
#### BlockQueue.cs: Gera novas peças aleatórias e mantém a fila de Tetrominos.
#### Position.cs: Armazena a posição das peças na grade.
#### Assets/: Contém as imagens utilizadas no jogo, como os blocos coloridos e o fundo.
## 🧩 Lógica de Jogo
#### GameState.cs: Esta classe controla o estado do jogo, como as peças atuais, a grade e se o jogo acabou ou não.
#### MainWindow.xaml.cs: O loop do jogo é gerenciado através de um async Task GameLoop(), onde as peças descem automaticamente após um determinado intervalo, com o intervalo diminuindo conforme a pontuação aumenta.
## 🎮 Input do Usuário
### O jogador pode usar as seguintes teclas para controlar o jogo:

#### ⬅️ Seta Esquerda: Move a peça para a esquerda.
#### ➡️ Seta Direita: Move a peça para a direita.
#### ⬇️ Seta Para Baixo: Acelera a descida da peça.
#### ⬆️ Seta Para Cima: Gira a peça no sentido horário.
#### Tecla Z: Gira a peça no sentido anti-horário.
#### Tecla C: Guarda a peça atual para uso posterior.
#### Tecla Espaço: Faz a peça descer instantaneamente até o fundo (drop rápido).

