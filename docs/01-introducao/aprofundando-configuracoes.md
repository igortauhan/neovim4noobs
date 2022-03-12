## Aprofundando nas configurações

No artigo anterior nós citamos algumas configurações que eu considero importante. Nesse artigo irei citar algumas essências. Lembrando que você pode adicionar ou remover quaisquer configurações a vontade. Lembrando novamente que temos o repositório [vim4noobs](https://github.com/luanmateuz/vim4noobs) que aborda profundamente as configurações.

Apesar de não ter citado no artigo anterior, qualquer configuração pode ser aplicada enquanto o Neovim estiver aberto. Para isso, rode o comando `:set "nome_da_config"` e a configuração ficará ligada enquanto a sessão do Neovim estiver **ATIVA**. Lembrando que o Neovim irá carregar sempre o arquivo **init.vim** em toda inicialização, então se você já configurou no arquivo e tentar sobrescrever, o efeito só irá durar enquanto você estiver com o Neovim aberto.

Lista das configurações:

```
set nowrap
set shell="insira seu shell preferido aqui"
set lazyredraw
set termguicolors
set tabstop=4
set shiftwidth=4
set expandtab
set mouse=a
syntax on
```

Como mencionado no artigo de Ambiente de Configurações, nós podemos inspecionar cada configuração dessa com o comando `:h "nome_da_config"`. Porém irei explicar o porque utiliza-las.

A configuração `set nowrap` impede que os caractéres que chegarem no limite da largura da janela do Neovim venham para próxima linha de baixo. Isso é uma característica pessoal, mas eu não gosto. Caso você prefira, pode apagar essa linha.

Há maneiras de abrir um Shell embutido no Neovim (como o terminal no VSCode). Para especificar o Shell padrão à ser aberto, adicione `set shell=/path/to/shell` no seu arquivode configuração. Por exemplo: `set shell=/usr/bin/zsh` irá adicionar o ZSH como Shell padrão no Neovim.

`set lazyredraw` faz com que o Neovim não "redesenhe" a tela enquanto você esteja executando alguma ação. Isso é útil para problemas de performance.

`set termguicolors` liga o modo **true color** do terminal no Neovim.

As seguintes configurações faz com que o Neovim sempre insira 4 espaços em branco ao teclar `TAB`. Isso pode ser útil pois dependendo do arquivo (bem comum em arquivos de texto .txt), o client LSP do Neovim utilizará 8 espaços em branco.

```
set tabstop=4
set shiftwidth=4
set expandtab
```

`set mouse=a` adiciona suporte a mouse no Neovim. Com isso você pode selecionar e scrollar utilizando o mouse. Eu particulamente não uso muito, mas eu prefiro deixar ligado para alguma ocasião que seja necessária.

E por último, `syntax on` liga o modo de coloração da syntaxe do Neovim.

Essas são um conjunto de configurações que considero essênciais. Como mencionado, você pode ajustar do seu jeito (recomendo fortemente que pesquise sobre as configurações, pois são muitas que podem trazer a tona alguma coisa do seu gosto).
