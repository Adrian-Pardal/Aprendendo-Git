<h1>Git Log</h1>

<p>Porventura queeria ver o historio de seus commits ou as versões do seu repositorio usamos git log . </p>

```
  git log
```
<p>O git log vai falar quem e o author do commit e data que foi   </p>

<img src="Imagens De Ilustração/git_log.png" >


<p>Temos a opção de ver mais detalhado podemos usar git log tambem .</p>

```
  git log --decorate
```

<img src="Imagens De Ilustração/git_log_decorate.png">

<p>Conseguimos filtrar o historico de commits procurando todos feitos pelo author . Exemplo : git log --author= "armando" . </p>

```
  git log --author= " "
```

<img src="Imagens De Ilustração/git_log_author.png">

<p>Podemos ainda ver mais informações pelo git shortlog vai mostra em ordem alfabetica o nome das pessoas que fizeram commits excelente para mostrar contribuinte
</p>

```
  git shortlog
```
<img src="Imagens De Ilustração/git_shortlog.png">

|Marcador          |Objeto                            |
|------------------|----------------------------------|
| Vermelho         | numero de commits do author      |
| Verde            |   nome do author dos commits     |
| Amarelo          | descrição do commit              |

<img src="Imagens De Ilustração/git_shorthlog_sn.png" width="580px"> 

<p>Temos tambme a opção de ver so o nome do author e a quantidade de commits.</p>

```
  git shortlog -sn
```

|Marcador          |Objeto                             |
|------------------|-----------------------------------|
| Vermelho         | numero de commits do author       |
| Verde            |   nome do author dos commits      |

<p>Um outro tipo de log e o "git log --graph" vai nos mostra de forma grafica os nossos commits e branches o que esta acontecendo ate o momento.</p>

<img src="Imagens De Ilustração/git_log_graph.png">

```
  git log --graph
```

>OBS : Cada asterisco mostra a sequencia do commits do ultimo ao primeiro.

<p>Cim a função log conseguimos ver o que aconteceu no commit usando o hash . Essa função git show + hash.</p>

```
  git show 
```

>OBS :  O hash e identificação do commit

<img src="Imagens De Ilustração/git_show.png">

|Cor               |Oque é?                            |
|------------------|-----------------------------------|
| Vermelho         | O que foi excluido.               |
| Verde            | O que foi adicionado.             |



<h1>Git Diff</h1>

<p>Caso queria ver a alterações antes de fazer o commit usando "git diff" vai lhe mostra a sua modificação antes de comitar use sempre antes de fazer commit.</p>

```
  git diff
```
<img src="Imagens De Ilustração/git_diff.png">

<p>Conseguimos so ver o nome do arquivo que modificado .</p>

```
  git diff --name-only
```

<img src="Imagens De Ilustração/git_diff_nameonly.png">

<p>Uma Dica! Se usarmos "git commit -am + "descrição" ja adiciona e faz commit ao memsmo tempo.</p>

>OBS : E como se fosse o git add mais o commit.

```
  git commit -am " "
```


