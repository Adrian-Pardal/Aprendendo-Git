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

