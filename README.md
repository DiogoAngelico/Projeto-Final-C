# Projeto-Final-C
Projetinho de mestre dos numeros feito por davi e diogo :D

# Planificação

## Contexto:

O nosso jogo vai ser uma réplica do jogo "Mastermind" no ternminal. 

Antes de tudo, o jogador terá uma opção de regras para caso não saiba das regras, ler as mesmas e entender como funciona o mastermind para conseguir jogar com melhor qualidade.

O utilizador terá de escrever um código de 4 digitos e cada digito tem de ser entre 1 e 6 sem o utilizador repetir 2 numeros iguais.

Depois do jogo ter acabado,aparecerá uma tela de vitória derrota ou desistência, dependendo das escolhas do utilizador ao longo do programa, todas as telas no final agradecendo ao utilizador de ter jogado o programa

# 1: Desafio

## o que o programa deve fazer:

O programa terá de seguir através destes passos:

1. mostra o menu do jogo que apresenta as opções Jogar e Regras

2.Se o utilizador escolher o menu regras:

-Aparece as regras

3. Senao aparece a tela do jogo, dentro da tela do jogo:

4. aparece uma pequena inteodução ao nome e uma opção para ele colocar o código

5. o utilizador terá de colocar a sua resposta

6. se o jogador acertar o código:

-Mostra uma tela de parabenização ao user por ter ganhado o jogo e agradece por ter jogado

7.Senão o programa terá de ver quais numeros estão certos, se estão certos nas suas posições correspondentes, e contabilizar os erros até o acerto ou o utilizador errar 10 vezes (Número maximo de erros).

## que dados precisa de guardar:

O programa precisa de guardar diversos dados para o funcionamento do mesmo. os dados que ele precisa guardar são a quantidade de tentativas que o utilizador tem para acertar o numero, guardar o numero secreto, quantas vezes a pessoa erra, as respostas do utilizador, e a posição onde os números estão.

## que entradas recebe:

O programa recebe como entradas a opção que o usuário escolheu no menu de entrada, e a resposta do utilizador certa ou errada do codigo secreto.   

## que saídas mostra:

O programa mostra 6 menus ao longo do código, o menu de entrada que mostra as duas opções de jogar e regras, e o menu de regras que mostra as regras do jogo, e o menu do jogo onde vai estar a mecânica do jogo e a jogabilidade do mesmo, o menu de vitoria, em que parabeniza o jogador por ter ganhado do jogo, o menu de derrota, que mostra o código secreto e agradece por ter jogado, e o menu de desistência, que fala uma mensagem diferente do menu de derrota, mas tambem mostra qual o codigo e agradece pelo mesmo ter jogado

## que funções fazem sentido:

Durante o nosso programa teremos diversas funcionalidades, logo para ser um trabalho mais facil de não so encontrar os erros mas tambem de organizar o código é de fazer diversas funções tambem. As funções que iremos usar são:

1. `Menu_Inicio`: Menu do inicio do jogo, que mostra o inicio do jogo e mostra as opçôes;
2. `Menu_Regras`: Mostra as regras e como funciona o jogo, tendo opção para voltar pro menu de inicio;
3. `Menu_Jogar`: Mostra o menu do jogo para que o jogo seja iniciado;
4. `Menu_Vitoria`: Mostra o menu que parabeniza o user de ter acertado o menu_secreto;
5. `Menu_Derrota`: Mostra o menu em que mostra o código secreto e agradece há pessoa por ter jogado;
6. `Menu_Desistiu`: Mostra o menu de quando o utilizador desiste, mostrando o codigo e agradecendo ao utilizador por ter jogado;
7. `Código_Secreto`: Cria o código secreto para ser usado na programação do jogo;
8. `Escolha_User`: Pergunta qual o código do utilizador e o guarda;

# 4: requisitos funcionais

1. O programa deve começar por um menu interativo, de fácil entendimento e
explicativo, com opções básicas de iniciar o jogo e ver as regras

2. O programa deve permitir inicialmente o jogador escolher entre duas
opções, jogar ou ver as regras, caso ele escolha regras irá poder ler as regras
e voltara ao menu do game, contendo as mesmas opções, ao escolher jogar,
ele poderá inserir os números dentro de 1 a 6, sem repetir ou colocar caractere
a mais, não podendo também escolher um número menor que 1 ou maior que
6

3. O programa validara as tentativas inseridas de forma correta, caso seja
errada colocara no contador de erros, caso esteja certo, agradecera o jogador
participar do game e terminara o programa.
4. O programa rejeitara a utilização dos números menor que zero 1 e maior
que 6, não irá contabilizar como erro também, assim como inserir letras será
rejeitado, inserir números repetidos, colocar mais do que 4 números.

5. O programa irá comparar o número secreto com o número inserido pelo
jogador, isso irá se repetir num total de 10 vezes caso o jogador erre as 10
vezes o programa irá dar como partida perdida.

6. O programa deve mostrar a quantidade de erros até a contagem de 10,
mostrar no final os números corretos independente do resultado do jogo

7. O programa deve guardar a quantidade de erros até a contagem de 10, o
número secreto e a ordem que se encontra o número, para que possa ajudar o
jogador a descobrir a ordem caso o número se encontre no local errado.

8. O programa deve terminar quando o jogo chegar à conclusão, caso o
jogador perca suas 10 tentativas, ele irá terminar o programa deixando uma
mensagem agradecendo a participação do jogador e dizendo que eles
perderam, ele se passa caso o jogador ganhe, irá aparecer uma mensagem
agradecendo a participação do jogador.

9. O programa deve informar quais dígitos estão ou não no número secreto e
dar a dica de no caso o número esteja em posição errada, mas ainda existir no
meio do número secreto deve informar que o número está em um local errado,
caso o jogador inserir algo que vá contra as regras, o jogo avisara que isso
quebra as regras.

10. O programa deve conter textos simples e auto explicativos, para a
facilitação do entendimento e conclusão pratica do jogo, de forma a entreter o
jogador

# 5: Pensar nas entradas e saídas

## 5.1: Entradas

1. O jogador não precisara introduzir o nome, será sempre chamado de
jogador
2. O jogador poderá escolher duas opções do menu, a opção de jogar e a de
ver as regras, sendo selecionada entre opção 1 jogar, 2 regras
3. Será mostrado um campo onde dirá para ele introduzir o valor que desejar
dentro das regras postas no jogo
4. Valores dentro de 1 a 6, não podendo repetir os números, nem colocar mais
do que 4 números.
5. Os valores que devem ser recusados são, números maiores que 6 e
menores que 1, números repetidos, letras, repetir a mesma ordem.

## 5.2: Saida
1. No início do jogo será dado as boas-vindas e apresentaremos o menu do
jogo
2. Será comparado o valor com o número secreto e será mostrado o valor real
caso esteja correto a tentativa do utilizador, caso não esteja correto ele dirá
quais números estão presente na ordem secreta e quais não estão
3. Usando array diremos por posições qual é a posição certa e qual valor está
atribuído a aquela posição dentro da array
4. Iremos percorrer o valor por toda a array para ver se o valor está presente e
comparamos o valor da posição com a qual está no array
5. A parabenização do jogador por acerta os números presentes no jogo, e
agradeceremos pela participação, Ex: Parabéns, você descobriu os números
secretos, agradecemos a sua participação.
6. Informaremos que a quantidade de tentativas foram todas gastas e o
jogador não conseguiu adivinhar o número agradecendo da mesma forma. Ex:
Infelizmente você não conseguiu acertar a ordem secreta, mas ainda
agradecemos muito pela sua participação.
7. Em caso de desistência avisaremos a ele que o jogo será finalizado, e
daremos break no jogo, Ex: Como estás querendo desistir do jogo, estamos a
informa que o jogo irá ser fechado, até a próxima e espero que tenha
aproveitado o jogo.

# 6: Escolher estruturas de dados

## 6.1: Dados do código secreto

### O código secreto tem quantos valores?

O código secreto terá 4 digitos, esses digitos sendo numeros não repetiso de 1 a 6, escondido para o utilizador adivinhar. 

Ex de um codigo: 6234

### Todos os valores são do mesmo tipo?

Sim, todos os valores do código serão de tipo inteiro(`int`)

### Faz sentido guardar o código secreto num array?

Sim, já que nós iremos usar posições para dar dicas ao utilizador sobre onde está o numero certo e se ele acertou o numero sequer array seria o melhor jeito de fazer isso e deixar a parte da programação mais fácil de fazer.

## 6.2: Dados de uma tentativa

### Uma tentativa tem os mesmos 4 valores do código secreto?

Uma tentativa não é obrigada a ter o mesmos 4 valores nas mesmas posições, como o utilizador está a adivinhar o código, se a unica opção válida fosse o código não faria sentido o utilizador tentar adivinhar o código, já que ele sempre ganharia o jogo

### Além dos valores introduzidos, faz sentido guardar o resultado dessa tentativa?

Não faria sentido guardar os valores introduzidos, pois o nosso codigo so precisa de ver se o numero secreto está errado ou não, e contabilizar a quantidade de tentativas que sobram para o mesmo, assim sem precisar desse passo amais de guardar os resultados das tentativas. 

### Que campos poderiam existir numa struct que representa uma tentativa?

Alguns dos possiveis campos que poderiam representar uma tentativa seriam o da tentativa (int tentativa),

## 6.3: Dados do jogo

### O programa precisa de guardar várias tentativas?

Caso seja preciso de fazer um histórico de tentativas, é util guardar as mesmas para depois colocá-las em uma struct feita para guardar essas tentativas em um array para ir buscar futuramente caso precise.

### Como podes guardar um histórico de tentativas?

Poderiamos fazer um histórico de tentativas a guardar elas em uma struct feita para guardar as tentativas, para conseguirmos ir buscar o histórico de uma forma mais organizada e em arrays.

### Que informação indica se o jogo ainda está a decorrer, terminou com vitória ou terminou com derrota?

Depois de entrar em concenso achamos que a melhor forma seria como no trabalho antigo em python, ou seja, colocar o menu em um while true, e quando o jogo acaba-se ou seja aparecesse um desses 3 menus for ativado, o while ficar a off, sobre saber se ele terminou com vitoria ou não, pediriamos ao user o seu código, cada numero dele, e veriamos se os 4 numeros que ele escreveu estão com o mesmo numero e ordem do array do numero secreto, se estiver tudo correto, o menu de vitoria aparecerá para ele, caso ele não tenha acertado todo o código e as posições dos numeros no numero de tentativas o jogo mostra o menu de derrota.
