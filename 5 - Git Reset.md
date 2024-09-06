<h1>Git Reset</h1>

<p>Uma possibilidade boa do git e poder resetar os nossos erros digitei algo errdo ou não quero mais arquivo .Talvez você alterou o arquivo porem desistiu das alterações vamos usar o "git checkout + nome do arquivo" vai voltar para o arquivo para antes da edição se você digitar o git diff ira perceber que não vai aparecer nada. </p>

```
  git checkout ""
```

<p>Caso queira retorna sua alteração porem ja usou o git add  ira ver que o git diff não reconhece as alterações pois o arquivo ja esta pronto para commit para resetar e so usar "git reset head + nome do arquivo.</p>

```
  git reset HEAD 
```

<p>Agora se digitar o git diff novamento vai constar nossas alterações.Fazendo git checkout denova e dando um git status não vai mostrar nada para fazer.</p>

<h1>Tipos de Reset no Commit</h1>

<p>Vimos mudanças que era pra ser feitas antes de fazer o commit agora são reset pra quando ja foi feito o commit. Temos tres tipos de commit "soft" , "mixed" e "hard".</p>

<h3>Soft</h3>

<p>O soft vai pegar seu commit e as modeficações e vai so coltar o arquivo no estado staged pronto para fazer o commit.</p>

```
  git reset --soft
```

<h3>Mixed</h3>

<p>O mixed ele vai excluir o seu commit porem vai voltar o arquivo pro estado de modified pronto adicionado e fazer commit.</p>

```
  git reset --mixed
```


<h3>Hard</h3>

<p>O reset Hard vai simplismente ignorar o commit e tudo que foi alterado e vai excluir completamente tudo que foi feito no commit.</p>

```
  git reset --hard
```



<p> E importante não esquecer que quando for resetar vamos sempre pegar a hash do commit anterior que você fez pois vai retorna para aquele commit o git vai interpretar "A parti de qual quer mudar?".</p>

<img src="Imagens De Ilustração/explicando_como_usar_git reset.png">

<p> Para onde a seta vermelha ta apontando e seu commit mais recente . E para onde verde esta apontando e para o commit que quer retorna so copiar a rash dele e usar git reset.</p>
