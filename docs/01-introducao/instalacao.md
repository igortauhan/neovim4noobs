## Instalação

O Neovim está presente para a maioria dos Sistemas Operacionais, encontrado inclusive na maioria dos gerenciadores de pacotes de distribuições Linux.

**Obs:** Para melhor utilização do Neovim nos próximos módulos, recomendo a instalação acima da versão 6.0.

### Linux

Instalar o Neovim no Linux é bem prático, pois como vimos, ele se encontra presente na maioria dos gerenciadores de pacotes do Linux, além de possuir uma versão em App Image. Alguns exemplos de instalação nos gerenciadores de pacotes mais famosos:

**Obs:** Nem sempre a versão que está nos repositórios dos gerenciadores de pacote da distribuição Linux é o mais atual. Caso a versão instalada não seja a 6.0 ou superior, recomendo baixar direto das [Releases](https://github.com/neovim/neovim/releases) no Github ou [Compilar manualmente](https://github.com/neovim/neovim/wiki/Building-Neovim).

Ubuntu / Debian ou derivados: `sudo apt install neovim`

Manjaro / Arch Linux e derivados `sudo pacman -S neovim`

[Você pode encontrar o App Image do Neovim nas Releases no Github](https://github.com/neovim/neovim/releases)

### Windows

O Neovim encontra-se disponível para ser utilizado nativamente no Windows, em versão QT com janela gráfica ou tradicionalmente pelo terminal. Eu particularmente recomendo que você utilize a versão pelo terminal.

A instalação e utilização do Neovim pelo terminal é feita através do [chocolatey](https://chocolatey.org/). Com o chocolatey instalado no seu Windows, entre no PowerShell com privilégios de administrador e rode o comando: `choco install neovim -y`. Isso fará com que o Neovim seja instalado na sua última versão estável.

Já a instalação em janela gráfica no Windows é bem simples também. Entre nas versões de [Releases](https://github.com/neovim/neovim/releases) do Neovim no Github e baixe a versão com Windows.

### MacOS

A instalação do Neovim no MacOS é feita através do [Home Brew](https://brew.sh/).

Com o Home Brew instalado no seu SO, rode o seguinte comando: `brew install neovim`

`Para abrir o Neovim após a instalação, reinicie seu terminal e digite nvim.`

<div style="display: flex; justify-content: space-between;">
    <p align="left">
        <a href="./sobre-o-neovim.md"><- Voltar para - Sobre o Neovim</a>
    </p>
    <p align="right">
        <a href="./sobre-o-neovim.md">Próximo artigo - Ambiente de configuração -></a>
    </p>
</div>
