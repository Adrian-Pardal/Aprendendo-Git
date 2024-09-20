<h1> 〚 Git .gitignore 〛 </h1>

<h3> Criando .gitignore </h3>

<p>Basicamente o gitignore e um arquivo dentro do nosso diretorio  no repositorio e dentro do arquivo vamos escrever os padrões pra determinada informação e vai ser utilizado . </p>

<img src="Imagens De Ilustração/gitignore_como_adicionar.png">

<p>Primeiramente crie um arquivo .gitignore pode usar qual quer editor de codigo. Dentro do git ignore e consigo alem de escrever uma arquivo expecifico mas tambem sua extensões para marca o arquivo temos que digitar um asteristico na frente + o que não queremos . EX : *.json </p>

<p>O .gitignore serve para não trackear(coletar) os arquivos unutil. No gitignore podemos ignorar arquivos especificos digitando o nome do arquivo. </p>

<img src="Imagens De Ilustração/gitignore_como_adicionar_arquivo_especifico.png">

<p>Colocando o no arquivo do .gitignore .</p>

<img src="Imagens De Ilustração/gitignore_como_adicionar_arquivo_gol.mx.png">

<p>Se der o git status vai ver que o arquivo gol ira sumir .</p>

<img src="Imagens De Ilustração/gitignore_como_adicionar_arquivo_removido.png">











<h1> 〚 Git Stash 〛</h1>

<h3>O que faz? </h3>

<p>E responsavel por guarda modificações que ainda não foram commitadas todas e esses arquivos vai ficar em uma pasta. E vai ficar guardo e depois quando quiser consigo acessar e chamar quando necessario .</p>

<p>Digamos que ocorreu um imprevisto e temos que para outro projeto ou branch . Porem ainda não quero fazer o commit pois eu ainda não terminei as modificações e so digitar git stash .</p>

```
  git stash
```
<p>Para voltar com seu arquivo vamos digitar .</p>

```
  git stash apply
```

<p>Mostar a lista com todos os stash .</p>

```
  git stash list
```

<p>Ja para excluir todos stash da lista .</p>

```
  git stash clear
```

<h1> 〚 Criar Atalhos dentro do Termianl do Git 〛</h1>

<p>Uma coisas do git e de todo unix você pode criar alias que são atalho dos comandos .</p>

<p>Criando eses atalhos e bem simples vamos digitar. Git config --global + alias.s depois do alias. tem que colocar o atalho + a função desse atalho que ira fazer.</p>

```
  git config --global alias.s status
```







<h1> 〚 Versionando com Tags 〛 </h1>

<p>Vamos as tags quando nos estivermos trabalhando com grandes bibliotecas ou projetos grande para definir as versões que vamos usar. Quando fazemos um commit ele guarda estados e as vezes queremos delimitar um bloco determinadoe para fazer isso nos podemos utilizar as tags .</p>

```
  git tag -a 1.0.0 -m "Readme"
```
> OBS : -a e para quando quer fazer uma anotação e depois colocarmos -m e escrevemos a anotação .

<h3>Subir a tag para repositorio Remoto </h3>

```
  git push origin master --tags
```
> OBS : --tags e para subir a tag pro repositorio (github) .

<p>Visualizar as tags geradas so usar "git tag" .</p>

```
  git tag
```












<h1> 〚 Git Revert 〛 </h1>

<p>Fiz commit porem a não gostei do commit ou não queria ter colocado a alteração e ficou no lugar errado . O que vou fazer?</p>

<p>Vamos no git log buscar o commit que fiz errado e pegar o hash(identificador) do commit que quero reverter vamos fazer um git revert + o hash do commit .</p>

<h4>Pra que eu uso o revert ?</h4>

<p>Soponhamos que eu trabalho numa empresa grande e quando eu subo o commit porem quebrou a produção mas se eu desse o git reset eu vou perde todas as alterações que fiz. Mas eu quero trabalhar nisso depois saber qual foi o problema no meu codigo fonte quando tiver tempo.</p>

<p>Então dando um git revert e vai reverte colocando o codigo anterior desse commit. Com isso eu consigo revisar o meu commit e resolver e assim novamente subir commit.</p>




<h1> 〚 Apagando tags e branches em Repositorios Remotos 〛 </h1>

<h4>Como apagar as tags e branches nos nossos repositorios remoto com o github </h4>

<p>Se formos apagar a tag ou branch no local na sua maquina local vamos usar o "git tag -d" ou "git branch -d" porem no github como faz?</p>

<p>Para apagar os tags no repositorio remoto basta "git push origin : + tag (nome) que quero apgar" .</p>

<p>E o mesmo serve para a branch "git push origin : + branch(nome)</p>

```
  git push origin : 1.0.0
```



