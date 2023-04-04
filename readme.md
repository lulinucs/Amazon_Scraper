
# Descrição do código

Este código em Python tem como objetivo coletar informações de livros na Amazon brasileira a partir de uma lista de URLs de produtos. As informações coletadas incluem título, autor, ano de publicação, sinopse, editora, idioma, número de páginas, ISBN-10, ISBN-13, dimensões, capa e categoria do livro. Os dados coletados são armazenados em uma planilha Excel.

![enter image description here](https://images2.imgbox.com/c1/c5/LG2yo5OO_o.png)

O código utiliza a biblioteca `BeautifulSoup` para fazer o scraping do conteúdo HTML das páginas web e a biblioteca `requests` para enviar requisições HTTP para a Amazon. As informações coletadas são então processadas e armazenadas em uma planilha Excel usando a biblioteca `openpyxl`.

O código lê uma lista de URLs de produtos da Amazon de um arquivo chamado `urls.txt`. Em seguida, o código itera por cada URL, faz o scraping das informações do livro e armazena os dados na planilha Excel, além de baixar a imagem de capa do livro e nomear cada capa com seu respectivo ISBN.

O código lida com possíveis erros, como páginas indisponíveis ou dados faltantes, e tenta recuperar a informação solicitada com várias tentativas. Se o código não conseguir obter as informações após o número de tentativas especificado, ele passará para o próximo item na lista de URLs.

![enter image description here](https://images2.imgbox.com/72/8c/xqjsYCIi_o.png)



# Como usar

Antes de executar o código, crie um arquivo `urls.txt` contendo as URLs dos produtos da Amazon que você deseja coletar as informações. Crie também uma planilha em branco nomedada `cadastros.xlsx`, o nome da aba também deve ser `cadastros`.

Para executar o código, basta instalar as dependências e executar o arquivo Python:

`pip install -r requirements.txt`

`python amazon_scraper.py` 
