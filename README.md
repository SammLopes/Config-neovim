# Configurações do NeoVim  

## Pré-requisitos
Para instalar sem ter problemas tem que ter o python e pip e o node.js

## Instalação do python e pip

### Windows:
Link de instalação do python
https://www.python.org/downloads/

### Ubuntu / WSL:
A chace de ter o python instalado no Ubuntu ou WSL é muito grande. Caso o pip não esteja instalado siga os passos 
abaixo:

```
sudo apt update
sudo apt install python3-pip
```
Para instalar a versão mais recente do python , use esses comandos:
```
sudo apt install software-properties-common
sudo add-apt-repository ppa:deadsnakes/ppa
sudo apt install python3.9
```

O pip 3.9 pode ser instalado dessa forma
```
curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
sudo python3.9 get-pip.py
```
No exemplo que acima esta em uma versão antiga, coloquye em uma versõa mais recente como a 3.12.

### Biblioteca pynvim
Essa lib é necessário para utilizar o python no neovim. 
```
 pip install pynvim
```

## Instalação do Node.js

### Windows
No Windows podemos utilizar esse link abaixo para baixar a ultima versão do instalador:
https://nodejs.org/
E necessário colcoar os path do windows, pois o vim e o neovim precisam utilizar o Node.js
### Ubuntu/WSL
O recomendado é instalar a ultima versão do LTS do Node.js 
Existe um versionador de versões do Node.js como o nvm, para instalar acesse o repositório do nvm para instala-lo:

https://github.com/nvm-sh/nvm#installing-and-updating

Quando terminar de instalar reinicie o terminal, e execute o comando:

```
 nvm install --lts
```

## Instalação do vim 

### Windows 
Para instalar a versão estável do vim  recente click no link abaixo:
```
https://www.vim.org/download.php
```

 ### Pasta de instalação 
 Você pode instalar na c:/vim, basta descompactar a pasta para o diretório raiz e o seu binário vai ficar na c:/nvim/bin, 
 adicione essa pasta nas variáveis de ambiente de windows. 

 ### Linux/WSL
 
 ```
  sudo add-apt-repository ppa:jonathonf/vim
  sudo apt update
  sudo apt install vim
 ```


## Instalação do neovim 

### Windows 
Para instalar a versão estável do neovim recente click no link abaixo:
Baixar o arquivos nvim-win64.zip
```
https://github.com/neovim/neovim/releases/tag/stable
```

 ### Pasta de instalação 
 Você pode instalar na c:/nvim, basta descompactar a pasta para o diretório raiz e o seu binário vai ficar na c:/nvim/bin, 
 adicione essa pasta nas variáveis de ambiente de windows. 

 ### Linux/WSL
 Podemos inslatar nesse caso a versão unstable, use essas seguintes linhas para instalar:
 ```
 $ sudo add-apt-repository ppa:neovim-ppa/unstable
 $ sudo apt-get update
 $ sudo apt-get install neovim
 ```

## Criação dos arquivos de configuração
Tanto o vim e o neovim presisam de um arquivo de configuração, eles não são criados automaticamente, sendo necessários cria-los 
manualmente.

### Vim 
Para o vim temos que criar um arquivo chamado .vimrc na pasta HOME. 
No windows tem que estar na pasta do seu usuário c:/Users/seuUser/.vimrc.
No linux colocamos na home dessa forma ~/.vimrc.

### NeoVim 
Já o neovim temos que criar um arquivo chamado init.vim, a localização deles no windows e no linux varia bastante
No windows temos que colocar na pasta AppData/Local/nvim/init.vim dentro da pasta do seu usuário. Como o neovim não 
criar um pasta de configuração crie uma dentro desse caminho passado acima, crie uma pasta nvim e dentro dele um arquivo
chamado init.vim.

No linux colocamos em ~/.config/nvim/init.vim. Como dito antes é necessário criar um arquivo de configuração, logo crie uma 
pasta nvim na pasta ~/.config  e crie um arquivo chamado init.vim.
