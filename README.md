# CursoHTML-CSS

## Figma

## HTML

- Geralmente o nome da página principal, por convenção, é **index.html**
- O HTML é visto por *tags*, ou seja, tudo para ser representado deve ser assim:  
```html
<tag>
  (conteúdo)
</tag>
```
Algumas tags especiais não precisam da tag de fechamento, se não é estruturada 
como: `<começo>` **(meio)** `</fim>`, não precisa fechar.
  
- As *tags* podem possuir **atributos**, que vem logo em seguida do nome delas 
na tag de abertura, como por exemplo: `<a href="link">`.
  
- Na mesma pasta do **index.html**, criar uma pasta chamada **assets**.
Nela, ficarão todos os recursos a serem utilizados no site, como imagens
por exemplo.
  
  
### Tags

#### Estrutura básica das tags
  
```html
<!DOCTYPE html>

<html>
    <head>
        <title>Titulo da Aba</title>
        <meta charset="utf-8">
    </head>

    <body>
        <header>
            --Cabeçalho
        </header>
      
        -- Resto do site
    </body>
</html>
```
> Esta estrutura é a **CERTA** de HTML, a válida para ser usada.
> No **VSCode**, digitar `! + tab` gera isso automaticamente.

- `<!-- -->` --> Comentário;

- `<!DOCTYPE html>` --> Define a versão mais estável do *HTML*;

- `<head>` --> Tudo que é configuração, vem antes do *<body>*;
  
- `<title>` --> Título da aba.
  
- `<meta charset="utf-8">` --> Define o *locale* do website.   
  
- `<body>` --> *corpo* do HTML, aonde as inf gerais do site estão;
  
- `<header>` --> Indica tudo que está dentro da parte do cabeçalho.
  
- `<h1>`, `<h2>`, ..., `<h6>` --> Heading (cabeçalhos ou títulos);
> Um bom site não passa de *h3*;
  
- `<p>` --> Parágrafo;
  
- `<em>` --> Tag de **ênfase**
> Exemplo: mudar o idioma de uma palavra escrita em inglês no meio 
de um parágrafo todo em português: `<em lang="em"> FrontEnd </em>`
  
- `<nav>` --> Navegação;
> É usada para botões que te façam **nav**egar pelo site;
    
- `<a>` --> *Anchor*, ou tag que é usada para links que te levam a 
outros lugares, fica dentro da tag `<nav>` também;
> `<a href=" ">` Skills `</a>` transforma *Skills* em um botão que te
leva para algum lugar indicado pelas "" após *href*
  
- `<img>` --> Insere uma imagem;
> `<img src="PATH">``</img>` Puxa uma imagem do **PATH** inserido.

### Atributos

  Atributos são modificadores dos conteúdos das tags, são divididos em 
**locais** e **globais**.  
  
  Os globais podem ser usados em qualquer tag, como por exemplo o
atributo `lang="pt-BR`, que altera a linguagem do conteúdo da tag.  
  Já os locais só podem ser usados em tags específicas, como o
`href="link"` da tag *<a>*.


## CSS

- Cuida do **visual** do site.  
  
### Primeiro jeito:
  
- Seus comandos são escritos nos **atributos** das tags do HTML:

```html  
<header style="background-color: rgb(171, 106, 255);">
```
> Sempre será nesse estilo, `<tag atribut= propriedade CSS: valor>`

### Segundo jeito:
  
- Abrir uma tag `<style>` antes:

```html
<!-- Aqui eu disse que quero style só na tag a-->
<!-- propriedade: valor-->
<style>
    a {
      color: white;
    }
</style>
```
  
### Terceiro jeito (melhor):
  
- Criar um arquivo separado com o mesmo nome do *.html*, para os *css*
  
- Funciona como uma função, a definição dela está no arquivo, e para chamá-la,
necessário fazer:

```html
<link rel="stylesheet" href="PATH">
```
>index.html

```css
a {
  color: white;
}
```
>index.css

#### Cores

- Há três jeitos de representar as propriedades de cor no **CSS**
  
1. **Nome**
  
`color: white;`
  
2. **Decimal**
  
`color: rgb(0, 0, 0);`
  
3. **Hexadecimal**
  
`color: #000000`

### Reset.css

- O arquivo adicional *reset.css* serve para consertar alguns detalhes 
específicos de navegadores, como por exemplo o caso da margem:

<img src="imagens/SiteSemResetCss.png">
> Observe a margem aos lados, não queremos ela no site.
  
Para isso, criamos o *reset*, inserindo-o no arquivo da mesma maneira 
que inserimos o *index*:
  
`<link rel="stylesheet" href="css/reset.css">`
  
E dentro desse arquivo, colocamos as propriedades que queremos definir
para cada tag:
  
```css
body {

    margin: 0;
}
```
  
- Agora note como ficou o site:
  
<img src="imagens/SiteComResetCss.png">
> As margens sumiram.  
<br />
<br />
  
- Geralmente é copiado algum reset.css, pois alguns são muito gerais e já
tratam de qualquer bug que o site possa ter. O mais famoso é o do [Eric Mayer](https://meyerweb.com/eric/tools/css/reset/)



## Anotações gerais
  
- Em um site, é melhor atualizar a página com `Ctrl + R` do que com `F5`,  
pois esse mantém o *cache* da página anterior, podendo não atualizar para  
a versão mais recente.
  
- Para programar com HTML no **VSCode**, fica muito mais fácil utilizando
a extensão ja instalada *Emmet*, digitando menos código. 
