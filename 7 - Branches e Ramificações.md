<h1>Branch</h1>

<h3>O que é branch?</h3>

<p>A forma de explicar branch que é um ponteiro que leva a um commit.</p>

<img src="Imagens De Ilustração/Branch.jpg">

<p>Quando criamos um repositorio no git e cada vez que faz um commmit vai gerar um hash que é um conjunto de e letras e numeros com isso pra cada hash vai ser tirardo um snapshot "tira uma foto de tudo que foi alterado naquele momento."</p>

<p>Se começarmos um novo repositorio o primeiro branch que vamos ter vai se chamar "master".E cada vez que fizemos os commits a branch vai seguir os commits e vai ver a branch vai estar em cima do ultimo commit.</p>

<img src="Imagens De Ilustração/git_gitpush_branch_e_nome.png">

<h3>Vantagens</h3>

<p>Por que usar? Quais vantagens?</p>

<p>• Poder modificar sem alterar a branch principal (master) . </p>
<p>• Facilamente Desligavel . </p>
<p>• Multiplas pessoas trabalhando no mesmo projeto . </p>
<p>• Evita conflitos . </p>

<h3>Criando nova Branch</h3>

<p>Para criar um branch e simples digite ."git checkout -B + nome da branch"</p>

```
  git checkout -B testebranch
```

> OBS : O -B e para que o git interprete que e vai criar uma nova branch

<p>Se quiser ver se a branch foi criada digite "git branch" vai mostra todas as branches que tem nesse seu repositorio. A branch que estiver usando vai estar com um asteristico na frente . </p>

```
  git branch
```

<img src="Imagens De Ilustração/git_testando_branch.png">










<h3>Movendo e Deletando Branches</h3>

<p>Depois que criar os branches conseguimos navegar entre as branches. Para mover pra outro branch e so usar "git checkout main + nome do branch" .</p>

```
  git checkout main
```

<p>Ja se quisermos apagar um branch que não vou utilizar , vamos digitar "git branch -D + nome da branch" .</p>

```
  git branch -D
```

<p>Agora digitando denovo git branch vai ver que não tera mais essa branch. </p>







<h2>Unindo Branches</h2>

<p>Unir branches temos dois metodos importantes que são "Merge" e "Reabase" . Os metodos fazer a mesma coisa unindo porem de formar diferentes.</p>









<h3>Passo a Passo Merge</h3>

<p>O inicio nos temos um branch com trêS commits e temos 2 branches. O branch master e o JKLS3 se reparar os dois estão Apontando para o mesmo commit N3 . </p>

<img src="Imagens De Ilustração/Branch_passo_a_passo_1.jpg">

<p>Agora vamos criar um novo commit que vai ser N4. Se nos repararmos a branch master ainda esta apontando para o commit N3 e o JKLS3 aponta para o N4.</p>



<p>Como fizemos o commit JKLS3 pegando do commit N3 ainda esta linear os commits . </p>

<img src="Imagens De Ilustração/Branch_passo_a_passo_2.jpg">

<p>Agora se criarmos outro commit pegando da branch master (principal) . Como master estava no N3 se criar o novo branch ira direto para o N5  e se repararmos temos uma ramificação . </p>
<img src="Imagens De Ilustração/Branch_passo_a_passo_3.jpg">

<p>Porem se criarmos outro commit pegando do commit N4 vamos ter o N6 e N4 na branch separado fazendo parte da branch JKLS3. Enquanto o N5 ta pertecente ao master.</p>

<img src="Imagens De Ilustração/Branch_passo_a_passo_4.jpg">

<h3>Jutando os commits</h3>

<p>Unindo os branches pra juntar N4 e N6 e jogar no branch master(principal) e deixar linear a branch. Usando o merge vai acontecer dessa forma vamos pegar e criar um novo commit que é o N7 e ira juntar todas as modificações de N4 e N6 com o N5 e vai deixar novamente linear os commits.</p>

<img src="Imagens De Ilustração/Branch_passo_a_passo_5.jpg">

>OBS : Reparando nessa junção foi preciso criar um novo commit e criou tambem um ciclo muitos chamam esse ciclo de forma diamante . Chamado assim porque cria uma especie de triangulo se notar os vertices .

<p>Se usarmos o merge sempre vai criar um novo commit pegando o branch secundario e colocando no branch principal por isso o N7 e a junção de N4 , N5 e N6. </p>

<h3>Merge pro e contra</h3>

<h4>Pro</h4>

<p>• Operação não destrutiva.  </p>

<h4>Contra</h4>

<p>• Commit Extra : Esse commit não modificou nada so esta jutando os commits.  </p>
<p>• Historico Poluido : Se estiver com muitos branches dificulta a leitura da arvore de commits.  </p>

<h3>Pratica Merge</h3>

<p>Para usar o merge na pratica temos que usar o comando git merge + nome da branch que quer unir</p>

```
  git merge 
```

<img src="Imagens De Ilustração/pratica_mergerebase_fazendomerge.png">

<p>Quando fazer o merge  o diamente fica mais evidente.</p>

<img src="Imagens De Ilustração/pratica_mergerebase_1.png">



















<h2>Passo a Passo Rebase</h2>

<img src="Imagens De Ilustração/Rebase_passo_a_passo1.jpg">

<p>O rebase inves de adiciona outro commit ele ira pegar o branch "last" que tem seu commit A4 e vai mover para frente de onde ele estiver jogando que sera na frente do A5 que e a branch principal deixando linear . </p>

<img src="Imagens De Ilustração/Rebase_passo_a_passo2.jpg">

<p>Basicamente rebase pega tudo que esta no branch separado e coloco no inicio da fila assim quanto o branch primario e o secundario vai esta apontando para o mesmo commit . Inves de ter uma arvore fazendo um ciclo vai ficar sempre linear . </p>

<img src="Imagens De Ilustração/Rebase_passo_a_passo3.jpg">


<h3>Rebase pro e contra</h3>

<h4>Pro</h4>

<p>• Evita commits extra.  </p>
<p>• Historico linear.  </p>

<h4>Contra</h4>

<p>• Perde a ordem cronologica.  </p>

<p>Usando rebase nos acabamos mudando nosso historico então temos que tomar bastante cuidado porque se mudar o historioco e uma outra pessoa tambem esta trabalhando no mesmo branch o que pode acontecer e que não vai conseguir subir sua modificações por que o historico ta diferente.</p>

> OBS : Em geral use o rebase sempre que for da o pull das modificações.


<h3>Pratica Rebase</h3>

<p>Para usar o rebase tambem vai ser igual o merge so que no lugar o rebase  então seri git rebase + nome da branch que colocar na frente .</p>
