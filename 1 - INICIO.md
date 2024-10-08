<h1> Iniciando no Git </h1>

<h2>O Que é o Git</h2>

<p>O Git foi desenvolvido para ser um sistema de controle de versão distribuído que serve para monitorar e guardar o histórico de alterações feitas em arquivos durante o desenvolvimento de software. Tem como características , Controle de versão distribuído , Proteção de alterações , Rastreamento de alterações e Recuperação de versões anteriores.</p>

<p>
Proteção de alterações : O Git protege o código e o histórico de alterações contra alterações acidentais ou maliciosas. 
  
Rastreamento de alterações : O Git permite ver o histórico de alterações do projeto, incluindo todos os commits feitos, com suas respectivas mensagens e códigos identificadores.

Recuperação de versões anteriores : Como os desenvolvedores fazem alterações no projeto, qualquer versão anterior pode ser recuperada a qualquer momento.</p>


<img src="Imagens De Ilustração/Git Logo.jpeg" width="400px  " height="200px">



<h3> Configuração inicial do Git</h3>

<p>Vamos começar com o básico primeiro precisamos definir o seu nome , email e editor de código. Isso ira servir para que o git interprete e guarde essas informações e tenha um conexão fluida.</p>

<h3>Definir Nome</h3>
<p>Quando falamos em definir vamos usar o "config" do usuário que chamamos de "--global" para definir o nome vai entre aspas colocara seu nome.</p>

```
  git config --global user.name "armando"
```


<h3>Definir Email</h3>
<p>O mesmo se aplica para definir o email do usuario.</p>

```
  git config --global user.email "armandogenesio@gmail.com"
```


<h3>Definir Editor de Código</h3>
<p>A definir o editor de código você vai precisar escrever esse código mudando somente o final para a identificação do seu editor de código. Vou deixar a tebala de alguns editores de código.</p>

```
  git config --global core.editor "code --wait"
```

<h3>Tabela Editores de Códigos</h3>

| Editor Código                                      | comando Git                                                                                 |
| ---------------------------------------------------| --------------------------------------------------------------------------------------------|
| VS Code                                            | git config --global core.editor "code --wait"                                               |
| Atom                                               | git config --global core.editor "atom --wait"                                               |
| Emacs                                              | git config --global core.editor "emacs"                                                     |
| Nano                                               | git config --global core.editor "nano -w"                                                   |
| Vim                                                | git config --global core.editor "vim"                                                       |
| Sublime                                            | git config --global core.editor "subl -n -w"                                                |
| Sublime Text (Windows, instalação de 32 bits)      |git config --global core.editor "'c:/program files (x86)/sublime text 3/sublimetext.exe' -w" |
| Sublime Text (Windows, instalação de 64 bits)      |git config --global core.editor "'c:/program files/sublime text 3/sublimetext.exe' -w"       |
| Text Mate                                          | git config --global core.editor "mate -w"                                                   |


<h3> Acessa Suas Configurações </h3>
<p> precisamos verificar se definições que colocamos acima foi efetuado para isso usamos o "--list".</p>

```
  git config --list
```
>Obs : Levando em conta que você ja verificou se suas informações esta certa. Para sair da função "list" aperte a letra "Q" para encerrar o processo no git.

<p>Para entrar em um editor de texto externo que não seja no terminal do git . Ira entrar no git bash e dar o siguinte comando nome do editor que esta na tabela +o arquivo/pasta do projeto que quer mexer .</p>

```
  code --wait Readme.md
```

<p>Caso queira usar o vim para editar no proprio terminal do git para aprender entrar para editar usamos "i" e para sair pra salvar usamos butão "esc" e  para salvar sua alteração escreva ":wq" </p>

<p>Caso queiro limpar a tela pois esta muito poluida so usar CTRL + L .</p>
