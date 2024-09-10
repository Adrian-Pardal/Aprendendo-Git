<h1>Git Hub</h1>

<h2>SHH key</h2>
  
<p>Conectar o git com o git-hub precisamos da SSH pois e a chave para que o github entenda qual e sua conta e repositorio.</p>

Aqui o link para fazer a ação . [GitHub SSH](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent).

<p>Pra gerar o ssh temos que entrar no terminal Git BASH usando esse comando.</p>

```
  ssh-keygen -t ed25519 -C "your_email@example.com"
```

> OBS : Caso estiver usando um sistema legado que não suporta o algoritmo ed25519 use:
> ```
>   ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
> ```


<p>Sendo assim vai colocar o email e dar "ENTER" caso queira colocar uma senha fiquei a sua escolh porem se não quiser e o que ue aconselho so clicar ENTER .</p>

<p>Depois que executar o comando o local da chave pra ver se funcionou e cd ~/.ssh/ para entrar e "ls" para pesquisar.</p>

```
  cd ~/.ssh/
```

<p>Pra pegar sua chave com codigo/identificador . Vai achar usando o ls um arquivo id_"nome".pub voce ira copiar o nome desse arquivos .</p>

<p> Para pegar o codigo vai usar cat + nome do arquivo ai vai mostra o codigo da chave pra colocar no github .</p>

```
  cat
```

> OBS: Tambem podera usar comando "more" + nome do arquivo  ou Pelo seu editor do texto (nome do editor) + o arquivo

<h2>Vai no seu perfil do git hub vai en settings . </h2>

<img src="Imagens De Ilustração/git_ssh_setings.png">

<h2>Depois em SSH e GPG keys .</h2>

<img src="Imagens De Ilustração/git_setings_sshkey.png">

<h2>Vai clicar em new ssh . </h2>

<img src="Imagens De Ilustração/new_sshkey.png" width="700px">

<h2>Colocara o codigo da chave aqui dera um title para saber qual computador e essa key e vai em add ssh key .</h2>

<img src="Imagens De Ilustração/git_ssh_add.png" width="700px" >

<h1>Ligando Repositorio Local a um Remoto</h1>

<h3>Para ligar o repositorio localmente vai ter que ir no github no repositorio que criou porem o repositorio tem q vir sem o Readme.md na hora da criação.</h3>

<img src="Imagens De Ilustração/git_readme.png">

> OBS : Não e pra marca essa caixinha  .

<h3>Vai aparecer essa tela .</h3>

<img src="Imagens De Ilustração/git_config_push.png">

<p>Agora vamos no terminal do git bash e você ira pegar primeiro codigo para linkar o git com o github .</p>

<p>Para confirmar se o comando foi sucedido digite "git remote" . Aparecendo o nome do repositorio exemplo "origin" vai esta tudo certo .</p>

```
  git remote
```

<p>Se quiser mais informações digite "git remote -v" </p>

```
  git remote -v
```

<p>O segundo comando vai mudar arquivo de master para branch main pois o git hub reconhece main.</p>

```
  git branch -M main
```
<p>Vamos pegar o ultimo comando o git push o que ele faz? o git push vai pegar todos os arquivos que tem e envia para o github pro repositorio determinado . </p>

> OBS : Temos o "-u" porque ? e quando fizer esse comando não precisa digitar todo vez o comando todo e vai digitar somente "git push".


<h3>Como enviar sua mudanças pro repositorio remoto do github</h3>

<p>Se fizer uma modificação no meu arquivo como subo para o github?</p>

<p>Quando fizer a alteração ira ver que se for no git não tera nada pois o git push para isso temos que escrever "git push + nome da pasta default ex: origin + a nossa branch que e main" .</p>

```
  git push origin main
```

<h3>Clonando Repositorio Remoto</h3>

<p>Como estamos trabalhando com codigo open source é bastante comum querer trabalhar em algum outro repositorio famoso ou ate mesmo pegar aquele codigo para trabalhar na nossa maquina localmente . </p>

<p>A gente tem um comando chamado "git clone" que permite clonar todo um repositorio para uma maquina local "git clone + link do projeto + Escreve o nome do projeto.</p>
