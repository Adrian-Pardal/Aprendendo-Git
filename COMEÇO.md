<h1> Começo do Git </h1>

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

<h3>Tabela Editores de Codigos</h3>

| Editor Codigo                                      | comando Git                                                                                 |
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
