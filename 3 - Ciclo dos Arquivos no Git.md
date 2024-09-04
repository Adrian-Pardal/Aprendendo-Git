
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

<p>Quando o arquivo ja estiver indexado vai estar no ultimo estado que eo staged.Deste modo fazendo o commit vai ser criado uma versão com todos os arquivos , e irão voltar para o estado de Unmodified ou seja "nada modificado desda ultima versão criada" . </p>


<h1>Vendo Na Prática</h1>

<h2>Git Status</h2>

<p>O primeiro comando que e importante aprender no git eo "git status". O git status ele serve para reportar como esta seu repositorio.</p>

```
    git status
```

<p>Criando um novo arquivo vamos ver o estado no git  . Exemplo : Estadogit.md </p>

<p>Se escrever git status novamento vai mecionar o estado do arquivo como não adicionamos ainda o arquivo estara em untracked. Com isso o arquivo foi criado porem o git não reconhece.</p>

<img src="">































