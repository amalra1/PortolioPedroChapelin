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
  
  
### --> Tags

#### Estrutura básica das tags
  
```html
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
```

- `<!-- -->` --> Comentário;

- `<head>` --> Tudo que é configuração, vem antes do *<body>*;
  
- `<title>` --> Título da aba.
  
- `<meta charset="utf-8">` --> Define o *locale* do website.   
  
- `<body>` --> *corpo* do HTML, aonde as inf gerais do site estão;
  
- `<header>` --> Indica tudo que está dentro da parte do cabeçalho.
  
- `<h1>`, `<h2>`, ..., `<h6>` --> Heading (cabeçalhos ou títulos);
> Um bom site não passa de *h3*;
  
- `<p>` --> Parágrafo;
  
- `<nav>` --> Navegação;
> É usada para botões que te façam **nav**egar pelo site;
    
- `<a>` --> *Anchor*, ou tag que é usada para links que te levam a 
outros lugares, fica dentro da tag `<nav>` também;
> `<a href=" ">` Skills `</a>` transforma *Skills* em um botão que te
leva para algum lugar indicado pelas "" após *href*
  
- `<img>` --> Insere uma imagem;
> `<img src="PATH">``</img>` Puxa uma imagem do **PATH** inserido.


## Anotações gerais
  
- Em um site, é melhor atualizar a página com `Ctrl + R` do que com `F5`,  
pois esse mantém o *cache* da página anterior, podendo não atualizar para  
a versão mais recente.
