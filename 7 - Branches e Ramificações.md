<h1>Branch</h1>

<h3>O que é branch?</h3>

<p>A forma de explicar branch que é um ponteiro que leva a um commit.</p>

<p>Quando criamos um repositorio no git e cada vez que faz um commmit vai gerar um hash que é um conjunto de e letras e pra cada hash vai tirar um snapshot "tira uma foto de tudo que foi alterado naquele momento."</p>

<p>Se começarmos um novo repositorio o primeiro branch que vamos ter vai se chamar "master".E cada vez que fizemos os commits a branch vai seguir os commits e vai ver a branch vai estar em cima do ultimo commit.</p>

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
