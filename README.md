<img width="359" height="168" alt="Captura de tela 2026-06-02 185936" src="https://github.com/user-attachments/assets/0c23296e-26b9-40f2-a917-624ae1d15238" />
# ⚔️ Dungeon Crawler - Vila Jutaiteua

Um jogo RPG de exploração de masmorras (*Dungeon Crawler*) baseado em turnos, desenvolvido integralmente em linguagem C para a consola. Projeto prático final da disciplina de programação.

**👩‍💻 Desenvolvedora:** Francinetti De Paula Abreu Pessoa  
**🎓 Instituição:** CESUPA (Centro Universitário do Estado do Pará)  

---

## 📖 História do Jogo
Uma perigosa anomalia espalhou-se pelo subsolo da pacata **Vila Jutaiteua**, no município de Moju. Como a última esperança da região, o herói chega à vila armado com a sua coragem. A missão é clara: falar com o ancião da vila para obter uma arma, descer os 3 andares escuros e repletos de armadilhas da masmorra, superar os monstros corrompidos e derrotar o grande **Boss Final** para trazer a paz de volta à comunidade local.

---

## 🎮 Como Jogar:

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

## 📸 Imagens do Jogo
# ⚔️ Dungeon Crawler - Vila Jutaiteua

![Linguagem C](https://img.shields.io/badge/Linguagem-C-blue.svg)
![Ambiente](https://img.shields.io/badge/Ambiente-Console-black.svg)
![Status](https://img.shields.io/badge/Status-Conclu%C3%ADdo-success.svg)

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

## 📸 Imagens do Jogo

<img width="359" height="168" alt="Captura de tela 2026-06-02 185936" src="https://github.com/user-attachments/assets/4d71373c-27a9-455b-8232-3a741e4910d6" />


## 🤖 Declaração sobre o uso de IA Generativa

Para o desenvolvimento deste projeto, a Inteligência Artificial Generativa (Gemini) foi utilizada como ferramenta de suporte pedagógico e auxílio de otimização de código ("pair-programming"). O uso teve os seguintes objetivos:
1. **Estruturação do Motor do Jogo:** Auxílio na construção da máquina de estados (menus e andares) e na função base de renderização da matriz no ecrã sem causar "flickering" (piscar da consola usando a biblioteca `<windows.h>`).
2. **Resolução de Bugs (Debugging):** Suporte na identificação de falhas de lógica em matrizes (como formatação de espaços nulos nas extremidades dos mapas) e resolução de conflitos de compatibilidade com o padrão *C89* utilizado pelo compilador Falcon C++.
3. **Mecânicas Matemáticas:** Auxílio na construção da lógica matemática para projetar a "hitbox" (área de dano espelhada) do Arco e da Espada de acordo com o eixo X e Y direcional do jogador.

Todo o código gerado foi minuciosamente revisado, testado em tempo real e compreendido por mim. O level design das matrizes (mapas em labirinto) e a definição dos atributos específicos e limites do jogo foram guiados manualmente para atender aos requisitos académicos do projeto.

## 🤖 Declaração sobre o uso de IA Generativa

Para o desenvolvimento deste projeto, a Inteligência Artificial Generativa (Gemini) foi utilizada como ferramenta de suporte pedagógico e auxílio de otimização de código ("pair-programming"). O uso teve os seguintes objetivos:
1. **Estruturação do Motor do Jogo:** Auxílio na construção da máquina de estados (menus e andares) e na função base de renderização da matriz no ecrã sem causar "flickering" (piscar da consola usando a biblioteca `<windows.h>`).
2. **Resolução de Bugs (Debugging):** Suporte na identificação de falhas de lógica em matrizes (como formatação de espaços nulos nas extremidades dos mapas) e resolução de conflitos de compatibilidade com o padrão *C89* utilizado pelo compilador Falcon C++.
3. **Mecânicas Matemáticas:** Auxílio na construção da lógica matemática para projetar a "hitbox" (área de dano espelhada) do Arco e da Espada de acordo com o eixo X e Y direcional do jogador.

Todo o código gerado foi minuciosamente revisado, testado em tempo real e compreendido por mim. O level design das matrizes (mapas em labirinto) e a definição dos atributos específicos e limites do jogo foram guiados manualmente para atender aos requisitos académicos do projeto.
