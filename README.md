# SPRIDER 

## SOBRE O PROJETO
Uma versao definitiva e altamente customizada do classico Paciencia Spider, construida para rodar de forma autonoma em um unico arquivo HTML. O codigo foi estruturado para entregar uma experiencia fluida, incorporando injecao de audio dinamico, mecanicas de combo e sistemas de assistencia criptografados.

## RECURSOS DO SISTEMA
- Motor de Audio Hibrido: Suporte nativo para injecao de links do YouTube. O script extrai o ID do video, burla as restricoes de autoplay atraves de interacao inicial e roda a faixa em segundo plano. Possui sistema de contingencia (fallback) com trilha Lofi padrao.
- Escalabilidade de Dificuldade: 6 configuracoes de "Nivel de Ameaca", alternando a complexidade do algoritmo de distribuicao entre 1, 2 e 4 naipes.
- Modulo de Defesa Integrado (SOS): Algoritmo de deteccao de ociosidade que libera uma rotina de socorro. O acesso a dicas de movimentacao (Highlight) e bloqueado por uma IA de Jogo da Velha (Minimax). Apenas derrotando-a o rastreio visual e liberado.
- Feedback Sensorial: Geracao de ondas sonoras complexas (Sine, Sawtooth, Square) diretamente via Web Audio API para eventos do jogo, dispensando arquivos de audio externos para efeitos.
- Persistencia de Sessao: Gravacao continua de estado via LocalStorage, permitindo a recuperacao de partidas nao finalizadas, pontuacoes maximas e preferencias de configuracao (Nome e URL).
- Renderizacao Dinamica: Sistema drag-and-drop fluido projetado tanto para mouse quanto para touch, com clonagem de elementos fantasma para visualizacao de arraste.

## INSTRUCOES DE EXECUCAO
1. Aloque o codigo-fonte em um arquivo local nomeado `sprider.html`.
2. Execute o arquivo em qualquer navegador com suporte a HTML5 e ES6.
3. Insira suas credenciais, defina os parametros de audio e dificuldade, e inicie a sessao.
4. OU ENTRE NO SITE OFICIAL

## ARQUITETURA E TECNOLOGIAS
- HTML5: Estruturacao do DOM e container Canvas para renderizacao de particulas.
- CSS3: Estilizacao baseada em Variaveis (Root), Flexbox/Grid para responsividade absoluta, e animacoes em Keyframes para eventos de sistema.
- JavaScript (Vanilla): Lógica de estado do jogo, manipulacao de eventos de ponteiro, integracao de iFrame (YouTube API) e IA Minimax.

## NOTAS DE SEGURANCA E LIMITACOES
O bloqueio padrao de Autoplay dos navegadores e contornado forçando a execucao dos modulos de audio (Web Audio API e YouTube Iframe) apenas apos o evento de "click" na tela de login.

---
Desenvolvido por mka.
