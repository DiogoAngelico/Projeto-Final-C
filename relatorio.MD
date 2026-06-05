
Para o desenvolvimento do nosso jogo, criamos 8 funções principais, cada uma sendo responsável por uma parte importante para a funcionalidade. Sendo elas as funções de desistir do jogo, exibição de regras, menu inicial, geração de números aleatórios, menu do jogo, um menu pra vitórias e derrotas, contabilização de tentativas.

A primeira função executada é a do menu inicial, que está dentro de um ciclo while(1), utilizado para simular uma repetição infinita. A função mostra inicialmente uma mensagem de boas-vindas ao jogador, exibe o título do jogo e mostra duas opções: iniciar o jogo ou consultar as regras.

A escolha é concretizada utilizando números no terminal, sendo mostradas da seguinte forma;
1 – Jogar
2 - Regras
Selecionando a opção “Regras”, é apresentado o menu de regras, contendo instruções do jogo. As regras são as seguintes:
1 – Não é permitido introduzir letras ou caracteres diferentes de números;
2 – Não são aceitos números negativos nem com valores decimais;
3-Não é permitido introduzir mais de quatro números;
4-O jogador tem no máximo dez tentativas para descobrir o código secreto.

Após a leitura das regras, o utilizador pode regressar ao menu inicial e escolher iniciar o jogo.
Ao selecionar a opção de “Jogar”, o programa direciona o jogador para o menu principal do jogo. A partir deste momento, passa a estar sempre disponível a opção de desistência. Para abandonar a partida, o jogador deve introduzir a letra “D” ou  “d” no terminal e em seguida, confirma sua saída introduzindo, também no terminal, “S” ou “s”.
Caso a decisão do jogador seja de permanecer a jogar, é apresentado um cantador de tentativas, controlado por uma função específica responsável por 
resistar cada tentativa realizada. Este contador é utilizado até que o jogador descubra o número ou atinja o limite de tentativas.
A geração do código secreto é realizado através da função código_secreto, responsável por criar números aleatórios entre 1 e 6. Os valores gerados são guardados em uma array, que representa o código que o jogador deverá descobrir ao longo da partida.
