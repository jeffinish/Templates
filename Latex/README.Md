<div align="center">

# Template para texto em LaTeX
</div>

## O que é LaTeX?
* De maneira resumida, o LaTeX é uma linguagem de programação utilizada para digitar documentos e é utilizada, em especial, no meio acadêmico ou para digitalização de documentos com formas matemáticas

## Porquê ter um modelo?
Ao utilizar o LaTeX por um tempo, você nota que certos pacotes adicionais são sempre úteis de ter nos seus documentos. Para citar alguns:

  * O "enumitem" permite um controle melhor sobre listas enumeradas de itens;
  * O "tkzeuclide" permite criação de diagramas e figuras geometricas;
  * Entre diversos outros.

Assim, imagine, a cada documento criado, ter que lembrar qual você sempre utiliza, qual foi necessário para aquele documento específico e etc. É ai que entra a utilidade de ter um arquivo base com todos os pacotes e customizações que você sempre utiliza.

### Outras vantagens de ter um modelo
Se você, assim como eu, gosta de deixar seus documentos com a sua cara, ter um modelo pode ajudar muito também. Você pode criar um template onde você altera a numeração dos Teoremas de acordo com a sua vontade, o estilo que eles aparecem, a cor dos enunciados, tudo isso apenas uma vez.

Além disso, permite uma padronização na organização do arquivo, como por exemplo, manter todas as figuras em uma determinada pasta, assim como todos os subarquivos.

## O que esse modelo têm de especial?
#### Ajustes básicos
* O ajuste das margens do documento utilizando o pacote `geometry`;
* Inclusão de alguns pacotes básicos para digitação de arquivos em português com atenção especial para o comandos`\usepackage[brazilian]{babel}` que traduz os comando originais do LaTeX, como o ambiente *Theorem* para *Teorema*.
* O comando `\graphicspath{{images/}{../images/}}` define a pasta na qual o LaTex vai procurar as imagens, neste caso, é a pasta *images* continda na mesma pasta do arquivo base.

#### Ajustes adicionais
* O pacote `\usepackage[light,math]{kurier}` altera a fonte para *Kurier*.
* Utilização do pacote `\usepackage{csquotes}` para inclusão de aspas simples e duplas que abrem e fecham;
* `\usepackage{enumitem}` para maior flexibilidade ao utilizar ambientes enumerados;
* O tão importante `\usepackage{faktor}` para digitar quocientes de maneira diferente de frações;
* Inclusão do `\usepackage{tkz-euclide}` para construção de diagramas e figuras geométricas diretamente no LaTeX;
#### Personalizações
* <span style=" color:#ff3366"> Define a cor que eu utilizo sempre que possível com o seu código em RGB.</span> `\definecolor{ros}{RGB}{255,51,102}`
* Define novos comandos para digitar de maneira prática os algumas letras que sao utilizadas com frequência, como a representação do conjunt dos inteiros, reais e etc com `\newcommand{\mb}[2]{\mathbb{#1}^{#2}}` e de letras caligráficas com `\newcommand{\mca}[1]{\mathcal{#1}}`;
* Define de maneira simples algo que sempre me incomodou, que é uma maneira de digitar d*x* ao invés de *dx* dentro de integrais. Para isso, basta definir `\newcommand{\der}{\text{d}}` ara ter o *d* como texto dentro do ambiente matemático.
* Muda a cor do quadradinho que aparece no final de demonstrações para rosa, com o comando `\renewcommand{\qedsymbol}{\textcolor{ros}{\openbox}}`
* Customiza a aparencia dos ambientes de demonstração e relacionados e define alguns novos também.
* Inclui também o pacote `\usepackage{subfiles}` para utilização de subarquivos. Isto é, permite a divisão de um documento em LaTeX em vários outros subarquivos para facilitar a organização. Estes arquivos estão todos localizados na pasta *sections*.


## Motivação

Minha principal motivação em criar estes arquivos, este repositório e esta descrição foi compartilhar, de maneira mais clara possível o que eu aprendi em todo esse tempo digitando e sendo um entusiasta do LaTeX.

Minha motivação secundária foi aprender um pouco mais sobre como utilizar Markdown, organização aqui no GitHub para qu eeu possa utilizar em outros projetos.
