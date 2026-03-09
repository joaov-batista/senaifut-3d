# ⚽ SENAIFUT 3D - Multiplayer

SENAIFUT é um jogo de futebol 3D em primeira pessoa, com física de bola, sistema de stamina e multiplayer online via conexão P2P (Peer-to-Peer) direto no navegador. Tudo isso construído apenas com HTML, CSS e JavaScript puro (Vanilla), sem a necessidade de um servidor backend complexo!

## 🌟 Funcionalidades

* **Multiplayer P2P:** Jogue com seus amigos usando um código de sala de 6 dígitos. Sem lag de servidor centralizado, conexão direta!
* **Sistema de Lobby:** Sala de espera sincronizada com escolha de personagem e lista de jogadores em tempo real.
* **Física Realista:** A bola sofre ação da gravidade, quica, rola com atrito e colide com as paredes da quadra.
* **Mecânicas de Jogo:** Condução de bola, chute forte (M1), domínio no pé (M2), corrida com barra de fôlego (Shift) e mecânica de roubo de bola/bote (Espaço).
* **Personagens Customizados:** Escolha entre diferentes avatares texturizados.

## 🎮 Controles

| Tecla | Ação |
| :--- | :--- |
| **W, A, S, D** | Movimentar o personagem / Conduzir a bola (ao encostar) |
| **Mouse** | Girar a câmera (Visão FPS) |
| **Clique Esquerdo (M1)** | Chutar a bola (Chutão/Finalização) |
| **Clique Direito (M2)** | Dominar/Parar a bola no pé |
| **Espaço** | Dar o Bote (Puxa a bola do adversário quando estiver perto) |
| **SHIFT** | Correr (Consome a barra de Stamina) |

## 🛠️ Tecnologias Utilizadas

* **HTML5, CSS3 e JavaScript (Vanilla)**
* **[Three.js](https://threejs.org/):** Motor gráfico para renderizar o ambiente 3D, quadra, gols, jogadores e a física.
* **[PeerJS](https://peerjs.com/):** Biblioteca para WebRTC, responsável por conectar os jogadores ponto-a-ponto (P2P) para o modo multiplayer funcionar apenas com frontend.

## 🚀 Como Jogar (Multiplayer)

Como o jogo utiliza tecnologia P2P, um jogador precisa ser o **Host** (o "dono" da bola e do cálculo da física) e os outros serão os **Visitantes**.

1. **O Host** acessa o jogo, digita o nome, escolhe o personagem e clica em **Criar Sala**.
2. O Host copia o **Código da Sala (6 dígitos)** que aparecerá na tela e envia para os amigos.
3. **Os amigos** acessam o jogo, colocam o nome, inserem o código de 6 dígitos no campo inferior e clicam em **Entrar na Sala**.
4. Quando todos estiverem na lista do Lobby, o Host clica em **Começar Partida**.

## 📂 Estrutura de Arquivos Necessária

Para que o jogo funcione corretamente e não dê telas brancas nos personagens, certifique-se de que os seguintes arquivos estão na mesma pasta (raiz) do repositório:

```text
/
├── index.html
├── brisa.png
├── eduarda.png
├── gabriela.png
├── joão.png
├── leo.png
├── rafaela.png
└── taiana.png
