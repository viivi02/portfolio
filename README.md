# Portfolio Vinicius Lemes

Este primeiro projeto foca em ser um portfolio inicial, que sera aprimorado de acordo com minha evolução como desenvolvedor Web.

## 🚀 Começando

Essas instruções permitirão que você obtenha uma cópia do projeto em operação na sua máquina local para fins de desenvolvimento e teste.

Consulte o site a seguir **https://portfolioviniciuslmes.netlify.app** para ver o mesmo.

### 📋 Pré-requisitos

De que coisas você precisa para instalar o software e como instalá-lo?

```
Um navegador como chrome ou explorer e internet
```

### 🔧 Explicando codigo utilizado

Aqui será dada uma explicação em relação aos códigos utilizados na parte de HTML quanto na de CSS.

HTML:

```
Foi gerado um template padrão de HTML informando que o arquivo era em HTML na primeira linha com o "<!DOCTYPE html>"
e aberto as tags <html></html>, logo em seguida vem a <head> que seria o cabeçalho, parte onde não exibe informações
no corpo do site.
<title>--> Utilizado para informar o título do site na barra de navegação
no trecho --> <link rel="icon" type="imagem/png" href="https://png.pngtree.com/png-vector/20191026/ourlarge/
pngtree-cat-face-glyph-icon-vector-png-image_1874311.jpg" /> fiz uma citação a uma imagem na web que irá funcionar
como icone na barra de navegação (é a imagem de gatinho logo atras do título do site)
<link rel='stylesheet' type='text/css' media='screen' href='style.css'> --> Esta linha serve para fazer referencia
ao arquivo Css referente a esta página utilizando o href para citar o mesmo.
href --> serve para citar um link ou arquivo externo
<body></body> --> entre estas tags irá ficar o corpo do site onde toda informação irá aparecer
<ul></ul>--> para criar uma lista não ordenada
<li></li>--> onde sera listado as informações dentro do <ul> toda esta parte foi utilizada para a estruturação da
barra de navegação.
seguindo pelo código foi utilizadas diversas tags de <div></div> que funcionam como blocos dentro da estrutura do HTML
dentro das tags <div>,<ul> e <li> foram utilizadas classes para indentificá-los no css posteriormente classe esta que se
cita como no exemplo a seguir <tag class="">.
<h1></h1>--> tag utilizada para gerar um título por padrão
<h2></h2>-->mesma funcionalidade do h1 porem seu tamanho por padrão é menor ao h1
<p></p>--> tag simples para inserção de texto dentro do html
outras parter que podem ser vistas no codigo seria o uso de id que funciona semelhante a classe <tag id=""> na qual
define um id que pode ser citado ou utilizado posteriormente e até mesmo o style dentro da tag para estilizar a mesma no
próprio html <tag style="">
```

CSS:

```
Seletores utilizados:
*{
  margin:0px;
  padding:0px;
}
(neste primeiro defini um seletor universal para toda a estrutura que não haveria espaçamento nas margens e no padding facilitando alocação das
coisas)
li (organizar as listas da <ul>)
body (altera tudo que se encontra no corpo do site)
p (altera as formatações das tags <p>)
li:last-child (serve para atribuir propriedades ao "ultimo filho")
Classes:
navbar(esta classe foi utilizada para ajustar o a lista não ordenada <ul>)
active(classe criada para dar efeito de cor de fundo quando se esta em uma pagina, o bloco da navbar referente ira ficar com a cor
de fundo mais clara)
inicial(referente ao conteúdo principal do site nesta classe se encontra o div que armazena o background animado)
descricao(se encontra dentro da div de classe "inicial" a mesma possui uma prévia descrição de texto que será exibida)
texto(classe criada para organizar os textos presentes na classe "descricao")
imginicial(div criado com esta classe na qual teve seu backfround alterado para uma imagem da web, utilizando o comando
background-image: url('');)
mais(esta classe se refere ao div que fica em baixo do inicial, o mesmo visa "abrigar" informações abaixo da principal)
divmais(como diz o nome é um div que se encontra dentro do div de classe "mais")
lista(outra classe que se refere a uma lista não ordenada)
skill(se refere a classe dada as linhas da lista não organizada <li>)
rodape(div classe"rodape" funciona como o footer do site sendo referenciado na parte final do site)
stars(esta classe foi criada como pequenos divs, sua função é se tornar um background animado, agora vou explicar as alterações
dentro desta classe foi definido sua altura e largura com os comandos "width: px;" e "height: px;", para gerar um efeito de
arredondamento utilizei "border-radius: 50%;", utilizando um truque podemos gerar varias sombras do mesmo elemento, com o
"box-shadow:"criei diversas sombras deste elemento em diversos locais da tela com a cor branca, para gerar a animação utilizei o
codigo "animation  : anim-stars 20s linear infinite;" definindo sua duração e que irá repetir infinitamente)
stars::after(para evitar de criar mais uma div foi utilizado um pseudo-elemento que chama ::after, utilizando a propriedade content
 deixei ele sem conteúdo com o valor "", foi repetida todas as propriedades da div classe="stars" apenas deixando de lado a
"animation" pelo fato dela puxar da mesma)
com o mesmo intuito foram criada outra div seguindo o mesmo esquema da classes "stars" esta div possui a classe stars2 seu objetivo
é ser estrelas menores de fundo, suas propriedades seguem as mesmas da classe "stars" sua unica diferença é o tamanho
@keyframes(utilizando a base de animações utilizando o "from {transform: translatey(px);}" levamos o conteudo para o valor que
definirmos "to {transform : translatey(px);}" assim consegui fazer a animação ter o efeito de estar subindo pela tela)

Durante o css sera comum ver seletores de agrupamento como por exemplo:
.texto h1,p{}
.texto h1
li a{}
.about h1,h2{}
.about p{}

Explicando propriedades utilizadas no código:
position --> define a como será a posição aplicada como por exemplo na navbar sua posição
se mantera fixa, ex: "position: fixed;"
background-color--> altera a cor de fundo do objeto
z-index--> serve para indicar o posicionamento do objeto na tela se um objeto esta com valor 0 e outro com 1, o objeto de maior
valor ira sobrepor o de menor valor
border--> altera as características da borda do objeto
opacity--> como o nome diz serve para alterar os niveis de opacidade ou melhor dizendo
transparência do objeto
color--> altera a cor do elemento
font-size--> altera o tamanho da fonte
-family--> define a fonte do texto
text-align-->informa o tipo de alinhamento que o texto terá
-shadow-->aplica sombra ao texto com a cor que definir
box-shadow--> funciona de forma semelhante ao text-shadow porem a sombra é aplicada no
objeto
border-radius--> altera os valores das bordas do objeto assim podendo "arredonda-las" como por exemplo nas estrelas
"border-radius: 50%;" na qual o div foi arredondado
display-->ele indica como o objeto vai estar na pagina podendo estar lado a lado, posicionar em uma linha nova ou no caso a
forma que mais utilizei no codigo de forma responsiva com o valor flex;
flex-direction-->modifica a direção dos objetos como usado em ambos pode ser em row que
seria linha ou column de coluna
align-items--> serve para alinhar os itens dentro do seletor na qual a propriedade
referencia
justify-content-->Ajusta os objetos a partir da direção que foi definida na flex-direction(row ou column)
background-size--> define o tamanho do fundo no seletor aplicado
background-repeat--> informa se irá haver repetição do fundo opção que deixei como no-repet; para que não repetisse
background-image--> define uma imagem de plano de fundo no seletor aplicado
margin--> para ajustar as margens do seletor na qual se aplicou esta propriedade
overflow--> serve pra definir o que acontece quando ultrapassa o tamanho da div

Valores aplicados em algumas propriedades especificas:

none; --> para remover uma propriedade ou valor indesejado da mesma como exemplo "border-right: none;" para remover
a borda do lado direito
hidden; --> utilizei na navbar para cortar o que passar do tamanho da div
existem diversos outros valores pare serem citados porém os mesmos se tratam de posições que um objeto ou elemento pode
ter na pagina.
```


## ⚙️ Sobre o Portfolio

O mesmo foi construido totalmente do 0, sem uso de qualquer ferramenta de auxilio, agradeço a compreenção aos erros que poderão ser
encontrados pelo código e ficarei feliz caso informe sobre os mesmos. 

### 🔩 Linguagens utilizadas

```
O mesmo foi projetado utilizando HTML/CSS, futuramente será inclementado funções com Javascript para melhorias
```

### ⌨️ Para informar


```
Este portfolio esta em fase de desenvolvimento e o mesmo não corresponde a sua versão final
```

## 🛠️ Construído com


* Git/GitHub - Utilizado para o versionamento do código 
* Visualstudio code - Ambiente de programação
* Netlify - Usada para hospedar o site na internet


## 📌 Versão

Utilizei Github para controle de versão. Para as versões disponíveis, observe as [tags neste repositório](https://github.com/viivi02/portfolio.git). 

## ✒️ Autores

* **Vinicius Lemes** - *Trabalho Inicial* - [Vinicius Lemes](https://github.com/viivi02)
* **Vinicius Lemes** - *Documentação* - [Vinicius Lemes](https://github.com/viivi02)


## 📄 Licença

Este projeto está sob a licença de (Vinicius Lemes Ribeiro) - veja o arquivo(https://github.com/viivi02/portfolio.git) para detalhes.

## 🎁 Expressões de gratidão

* Conte a outras pessoas sobre este projeto 📢;
* Compartilhe dicas para upgrade do projeto 😎;
* Um agradecimento publicamente 🫂;
* etc.


---
⌨️ com ❤️ por [Vinicius Lemes](https://github.com/viivi02) 😊
