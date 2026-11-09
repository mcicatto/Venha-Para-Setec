# VENHA PARA SETEC

Jogo arcade em HTML, CSS e JavaScript puro — labirinto em pixel art.

## Recursos
- 10 fases diferentes com labirintos maiores.
- 4 professores com IA e estratégias individuais.
  - Blinky persegue diretamente.
  - Pinky mira 4 blocos à frente.
  - Clyde alterna entre perseguição e fuga para o canto.
  - Inky calcula um alvo vetorial usando jogador + Blinky.
- A decisão de movimento usa busca de caminho e permite sair de becos sem ficar travada.
- Cada fase tem quatro chaves espalhadas pelo mapa que liberam a saída.
- Os professores começam na região central do labirinto, longe do jogador.
- Pontuação, vidas, cronômetro e itens coletáveis.
- Logo do Colégio Estadual Barbosa Ferraz flutuando no fundo animado (menu e ambiente, parallax; visual apenas).
- Fundo animado em camadas (grade digital, partículas, elementos escolares, logo) com suporte a `prefers-reduced-motion`.

## Dificuldades
Escolha antes de começar:
- **Fácil**: 2 professores, lentos e de visão curta. Patrulham bastante e só perseguem quando você chega perto.
- **Médio**: 3 professores, alternando entre perseguição e patrulha.
- **Difícil**: os 4 professores caçam sem descanso (visão total e mais rápidos).

Os professores revezam entre **patrulhar** e **perseguir**, só enxergam o jogador dentro de um alcance, às vezes tomam decisões imperfeitas e ficam atordoados por alguns instantes depois de te pegar.

## Colisões
A detecção de contato com os professores roda **a cada ciclo de atualização**, independente do timer de movimento (`g.cool`) e do atordoamento. São detectados tanto a ocupação da mesma célula quanto o cruzamento de trajetórias no mesmo ciclo, respeitando a invulnerabilidade temporária do jogador.

## Como abrir
Abra a pasta inteira no VS Code e use o Live Server. O arquivo `index.html` está na raiz do projeto.

## Identidade
- Nome oficial: **VENHA PARA SETEC**
- Assinatura: Desenvolvido por MC
- Fontes locais em `fonts/` (Press Start 2P e IBM Plex Mono)
