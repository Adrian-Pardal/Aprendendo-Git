
<h1>Ciclo dos Arquivos no Git</h1>

<p>O git e separado em 4 estados</p>

<img src="Imagens De Ilustração/clico_vida_git.jpg" width="950px">

<h2>Primeiro Estado UNTRACKED ou Não Rastreado</h2>

<p>O untracked e o momento que o arquivo acabou de ser adicionado no repositorio porem ainda não esta rastreado pelo git ou seja o git não reconhece alguma versão que tenha esse arquivo.</p>

<h2>Segundo Estado UNMODIFIED ou Não Modificado</h2>

<p>Apos que for adicionado o arquivo muda o seu estado para unmodified com isso o arquivo existe no git porem ele não sofreu nenhuma alteração ate o momento.</p>

<h2>Terceiro Estado MODIFIED ou Modificado</h2>

<p>Quando você modificar o arquivo , ira mudar para o estado de modified mostrando que o arquivo foi modificado que lhe permite ir para o ultimo estado.</p>

<h2>Quarto Estado STAGED ou preparado </h2>

<p >Quando o arquivo ja estiver indexado vai estar no ultimo estado que eo staged.Deste modo fazendo o commit vai ser criado uma versão com todos os arquivos , e irão voltar para o estado de Unmodified ou seja "nada modificado desda ultima versão criada" . </p>


<h1>Vendo Na Prática</h1>

<h2>Git Status</h2>

<p>O primeiro comando que e importante aprender no git eo "git status". O git status ele serve para reportar como esta seu repositorio.</p>

```
    git status
```

<h3>Criando um novo arquivo vamos ver o estado no git  . Exemplo : Estadogit.md </h3>

<p font-size="50px">Se escrever git status novamento vai mecionar o estado do arquivo como não adicionamos ainda o arquivo estara em untracked. Com isso o arquivo foi criado porem o git não reconhece.</p>

<img src="Imagens De Ilustração/untracked.png" width="800px">

<h2>Adicionando o Arquivo</h2>

<p>Sobre adicionar o arquivo temos que usar "git add" mais o nome do arquivo . Exemplo : git add Estadogit.md .</p>

```
    git add " "
```

<p>Com isso vamos perceber que seu aquivos esta como comimited esse eo estado unmodified do git que esta marcado em amarelo. </p>

<img src="Imagens De Ilustração/commit.png" width="500px">

<p>Porem se alterarmos as informações do arquivo o git ira mostra que foi modificado mostrando marcado em azul.</p> 

<img src="Imagens De Ilustração/modified.png" width="700px">

<p>Se vermos melhor o arquivo foi modificado porem não podemos fazer o commit pois não esta no modo staged marcado em verde para isso precisamos usar de novo o "git add Estadogit.md"</p>

<img src="Imagens De Ilustração/not staged.png" width="700px">

<p>Agora vamos conseguir fazer o commit.</p>

<img src="Imagens De Ilustração/committed.png" width="500px">

<h2>Commit</h2>

<h3>O que é o Commit</h3>

<p>O commit e quando avisamos pro git , pegue todos esses arquivos do meu repositorio e crie uma versão.</p>

<h3>Comando do Commit</h3>

<p>Para fazer o commit vamos digitar "git commit -m " uma descrição" .</p>

```
    git commit -m " "
```
>OBS: O que seria o "-m" e para você deixar uma descrição sobre o que foi modificado ou o que você de fato fez , qual quer informação pertinente e bom colocar comentario.

<img src="Imagens De Ilustração/falando_sobre_o_commit.png" width="500px" >

<p>O que esta marcado em vermelho chamamos de "hash" ou numero de identificação e esse numero nunca vai ser igual. </p>
<p> Marcado em azul e o seu comentario do commmit .</p>
<p> Em verde o git mostra que foi so um arquivos modificado e quanto insertions foram editadas.</p>

<h3>Nothing to commit ou Nada para ser feito</h3>
<p>Se der um git status novamento  o git vai mostrar "nada para ser feito" , pois a mudança que fizemos ja foram lançadas e salvas.</p>

>OBS: E como se o git resetase tudo pois todos os arquivos esta sem modificação  , voltando para o estado unmodified .

<img src="Imagens De Ilustração/nada_pra_ser_modificado.png" width="500px">





















