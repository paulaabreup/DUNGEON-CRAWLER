
# ⚔️ Dungeon Crawler - Vila Jutaiteua



Um jogo RPG de exploração de masmorras (*Dungeon Crawler*) baseado em turnos, desenvolvido integralmente em linguagem C para a consola. Projeto prático final da disciplina de programação.

**👩‍💻 Desenvolvedora:** Francinetti De Paula Abreu Pessoa  
**🎓 Instituição:** CESUPA (Centro Universitário do Estado do Pará)  

---

## 📖 História do Jogo
Uma perigosa anomalia espalhou-se pelo subsolo da pacata **Vila Jutaiteua**, no município de Moju. Como a última esperança da região, o herói chega à vila armado com a sua coragem. A missão é clara: falar com o ancião da vila para obter uma arma, descer os 3 andares escuros e repletos de armadilhas da masmorra, superar os monstros corrompidos e derrotar o grande **Boss Final** para trazer a paz de volta à comunidade local.

---

## 🎮 Como Jogar

O jogo é inteiramente jogado através do teclado e é baseado num **sistema de turnos**. O tempo só avança no jogo quando o jogador realiza uma ação. 

### Objetivo
Sobreviver aos três andares da masmorra. O jogador deve encontrar chaves para abrir portas bloqueadas, destruir caixas que barram o caminho, desviar-se de espinhos mortais e encontrar a escada (`L`) para o próximo nível, culminando na batalha final contra o Boss (`Z`).

### Controlos
* `W` : Move a personagem para Cima.
* `A` : Move a personagem para a Esquerda.
* `S` : Move a personagem para Baixo.
* `D` : Move a personagem para a Direita.
* `i` : **Interagir** (apanhar chaves, abrir portas fechadas, falar com o NPC ou carregar em botões). *É necessário estar virado de frente para o objeto!*
* `o` : **Atacar** (utiliza a arma que foi escolhida na Vila).

---

## 🗡️ Arsenal (Armas)
No início do jogo, na Vila, o jogador deve interagir com o NPC (`N`) para escolher o seu equipamento. A arma escolhida não pode ser trocada e define a estratégia de combate:

| Escolha | Arma | Área de Dano |
| :---: | :--- | :--- |
| **1** | **Espada** | Ataca uma área de 3x2 blocos diretamente à frente do jogador. |
| **2** | **Arco e Flecha** | Ataca em linha reta, atingindo 4 blocos consecutivos à frente. |
| **3** | **Cajado** | Magia em área: ataca simultaneamente todas as 8 células ao redor do jogador (3x3). |

---

## 🗺️ Significado dos Símbolos (Legenda)

A representação visual do mapa utiliza os seguintes caracteres ASCII:

| Símbolo | Significado e Mecânica |
| :---: | :--- |
| `^` `<` `v` `>` | O **Jogador** (aponta para a direção para onde está a olhar). |
| `*` | **Parede**: Bloqueia a passagem. |
| `#` | **Espinho**: Armadilha letal. Pisar retira 1 vida e reinicia o andar. |
| `k` | **Caixa**: Bloqueia o caminho, mas pode ser destruída com o botão de Atacar (`o`). |
| `@` | **Chave**: Necessária para abrir portas fechadas. Apanha-se com a tecla `i`. |
| `D` | **Porta Fechada**: Impede a passagem. Abre-se possuindo uma chave e utilizando `i`. |
| `=` | **Porta Aberta**: Caminho livre para passar. |
| `O` | **Botão**: Ativa mecanismos secretos no mapa (ex: remover espinhos) com a tecla `i`. |
| `L` | **Escada**: Conduz o jogador para o próximo andar. |
| `X` | **Monstro (Aleatório)**: Move-se 1 unidade por turno de forma aleatória. |
| `Y` | **Monstro (Perseguidor)**: Persegue a posição do jogador em linhas retas. |
| `Z` | **Boss Final**: Inimigo formidável do 3º andar. Corta caminho na diagonal para caçar o jogador de forma agressiva. |
| `N` | **NPC da Vila**: Distribui a arma inicial. |

---
## 🗺️ Legenda do Mapa

| Símbolo | Cor | Entidade | Comportamento / Regra |
| :---: | :--- | :--- | :--- |
| `^` `<` `v` `>` | 🟩 Verde | **Jogador** | O protagonista. Começa com 3 vidas. |
| `*` | ⬛ Cinza Escuro | **Parede** | Obstáculo intransponível. |
| `#` | 🟥 Vermelho Escuro | **Espinho** | *Insta-kill*. Causa perda de vida e reinicia o nível atual. |
| `k` | 🟫 Castanho | **Caixa** | Obstrui o caminho, mas possui vida própria (HP). É destruída ao receber a ação de Ataque (<kbd>O</kbd>). |
| `@` | 🟨 Amarelo | **Chave** | Item colecionável. Incrementa a variável de chaves na mochila do jogador (`i`). |
| `D` | 🟦 Ciano | **Porta Fechada** | Tranca o progresso. Requer uma Chave (`@`) e a ação de Interagir (`i`) para se transformar em uma passagem livre. |
| `=` | 🟦 Ciano | **Porta Aberta** | Célula liberada para movimentação. |
| `O` | 🔵 Azul | **Botão** | Mecanismo de puzzle. Destrói armadilhas específicas no mapa (ex: Espinhos ocultos). |
| `L` | 🟪 Magenta | **Escada** | Gatilho de transição de fase. Carrega a próxima matriz (`carregar_fase()`). |
| `X` | 🔴 Vermelho Claro| **Minion (Aleatório)** | Move-se 1 bloco por turno de forma procedural (baseado na função `rand()`). |
| `Y` | 🔴 Vermelho Claro| **Minion (Perseguidor)**| Avalia o Delta X/Y do jogador e move-se linearmente para encurtar a distância. |
| `Z` | 🔴 Vermelho Claro| **Boss Final** | O ápice do 3º andar. Emprega atalhos em diagonal para interceptar agressivamente o jogador. |

---

## 📸 Imagens do Jogo

<img width="359" height="168" alt="Captura de tela 2026-06-02 185936" src="https://github.com/user-attachments/assets/4d71373c-27a9-455b-8232-3a741e4910d6" />



<img width="506" height="311" alt="Captura de tela 2026-06-02 185947" src="https://github.com/user-attachments/assets/92a63600-220e-40c8-b0b9-5adf60edadf9" />


<img width="508" height="304" alt="Captura de tela 2026-06-02 190029" src="https://github.com/user-attachments/assets/539000f4-0a6f-4c77-bcec-a5f260fe9cae" />



<img width="548" height="666" alt="Captura de tela 2026-06-02 190125" src="https://github.com/user-attachments/assets/5b5a5193-d76c-4c7f-8eca-955ad5fa8585" />



<img width="474" height="171" alt="Captura de tela 2026-06-02 185959" src="https://github.com/user-attachments/assets/129accdb-d7f3-485f-9da7-868ced09fc84" />




## 🤖 Declaração sobre o uso de IA Generativa

Para o desenvolvimento deste projeto, a Inteligência Artificial Generativa (Gemini) foi utilizada como ferramenta de suporte pedagógico e auxílio de otimização de código ("pair-programming"). O uso teve os seguintes objetivos:
1. **Resolução de Bugs (Debugging):** Suporte na identificação de falhas de lógica em matrizes (como formatação de espaços nulos nas extremidades dos mapas) e resolução de conflitos de compatibilidade com o padrão *C89* utilizado pelo compilador Falcon C++.
2. **Mecânicas Matemáticas:** Auxílio na construção da lógica matemática para projetar a "hitbox" (área de dano espelhada) do Arco e da Espada de acordo com o eixo X e Y direcional do jogador.
3. *Cores no jogo:** Deixar o jogo mais ilustrativo.

Todo o código gerado foi minuciosamente revisado, testado em tempo real e compreendido por mim. O level design das matrizes (mapas em labirinto) e a definição dos atributos específicos e limites do jogo foram guiados manualmente para atender aos requisitos académicos do projeto.
