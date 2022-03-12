## Nivelamento

O objetivo desse artigo é ensinar o básico do VIM e Neovim.

Lembrando que caso você seja novato no mundo VIM, outros comandos já foram abordados no repositório [vim4noobs](https://github.com/luanmateuz/vim4noobs) de maneira aprofundada. Nesse artigo irei mostrar apenas o básico e importante.

**Obs:** apesar dos comandos valerem tanto pro VIM quanto pro Neovim, escreverei apenas VIM nesse artigo, a fim de não cansar o leitor.

Primeiramente, saiba que o VIM diferencia letras **MINÚSCULAS** de letras **MAIÚSCULAS** nos seus comandos. Então olhem e repliquem **exatamente da maneira que esse artigo apresenta**.

### Modos do VIM

O VIM trabalha com alguns modos, são eles: modo **NORMAL**, modo de **INSERÇÃO** e modo **VISUAL**.

O modo **NORMAL** é onde você pode utilizar os comandos do VIM, seja comandos de navegação ou comandos embutidos no próprio VIM (o modo normal é onde você passará a maior parte do tempo).

O modo de **INSERÇÃO** é o modo em que podemos entrar com digitação nos arquivos.

Já o modo **VISUAL** é onde poderemos selecionar cada caractér do arquivo.

Sempre que você abrir o VIM, ele entrará no modo **NORMAL**. Para entrar no modo de **INSERÇÃO**, aperte `i` (i **MINÚSCULO** em, lembre-se que o VIM diferencia o estados das letras). Para retornar ao modo **NORMAL**, aperte `ESC`. O modo **VISUAL** pode ser acessado apertando `v` (novamente, v **MINÚSCULO**), onde podemos selecionar o texto para deletar ou copiar (para selecionar os caractéres ou palavras que você deseja, basta usar as teclas de navegação que veremos no tópico a seguir).

### Movimentação

A movimentação entre as linhas e caractéres do VIM é feita através das teclas: `h j k l`, onde **h** movimenta para **ESQUERDA**, **j** movimenta para **BAIXO**, **k** movimenta para **CIMA** e **l** movimenta para **direita**.

O VIM nos permite usar combinações de comandos com números indicando a repetição do mesmo. Podemos entrar com `10j` para **DESCERMOS** 10 linhas, ou `4l` para **MOVIMENTARMOS** 4 caractéres para direita, sendo assim, qualquer número que você entrar sucedido do comando, fará ele repetir ***N vezes*** (vale pra qualquer comando).

Podemos também nos movimentar para a primeira e última linha do arquivo rapidamente. O comando `gg` nos leva para a primeira linha do arquivo. Já o comando `G` (isso mesmo, G **MAIÚSCULO**) nos leva para última linha do arquivo.

Além disso, podemos ir para o início e final da linha facilmente. O comando `0` (exatamente, apenas 0) nos leva para o início da linha. Já o comando `$` (nesse caso, SHIFT+4) nos leva para o final.

O VIM permite navegar entre o início das palavras com `w` e `b`. Como vimos, podemos usar da repetição com os números para fazer o comando repetir **N** vezes, então você pode usar `10w` para avançar 10 palavras (inclusive se a quantidade de palavras na linha que você estiver for menor que o número de repetições que você botou, o VIM irá avançar para as linhas sequentes).

Você pode movimentar através de linhas vazias utilizando `{` e `}` (ou SHIFT + [ e ]). É bastante útil quando você está navegando entre métodos de um arquivo que tem poucas linhas vazias.

### Copiar e colar

Nós podemos copiar as palavras e linhas no VIM de maneira fácil.

Para copiar um trecho de código, entre no modo **VISUAL** e use as teclas de navegações **h j k l** (lembre-se que o VIM otimiza o seu tempo programando ao ***MÁXIMO***, então **ABUSE** das repetições com as teclas de navegação, além das **w** e **j**). Com o trecho selecionado, simplesmente aperte `y` para **copiar**.

Agora com o texto no clipboard, aperte `p` para **colar**. O comando `p` também funciona com as repetições, então **10p** irá colar o trecho que está no clipboard **10 vezes**.

Você pode copiar uma linha inteira rapidamente usando `yy`.

### Scroll

Uma das melhores coisas do VIM é não precisar usar o mouse para nada (só se você quiser), então em um editor de texto comum, nós temos que tirar a mão do teclado e levar até o mouse para descer ou subir no arquivo. Com o VIM podemos usar `CTRL + y` para scrollar para **CIMA** e `CTRL + e` para scrollar para **BAIXO**.

<p align="right">
    <a href="../01-introducao/sobre-o-neovim.md">Próximo artigo - Instalação -></a>
</p>
