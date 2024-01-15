# IMDb Scrapper

**Versão:** 1.0

**Autor:** Bard

**Data:** 2024-01-14

**Descrição:**

Este código é um scrapper do IMDb que extrai dados sobre filmes, incluindo título, ano, classificação e sinopse. Ele usa as bibliotecas Python `requests`, `BeautifulSoup`, `time`, `csv` e `concurrent.futures`.

**Como usar:**

Para usar o scrapper, siga estas etapas:

1. Instale as bibliotecas Python necessárias:

```
pip install requests
pip install BeautifulSoup4
pip install time
pip install csv
pip install concurrent.futures
```

2. Clone este repositório:

```
git clone https://github.com/bard/imdb-scrapper.git
```

3. Entre no diretório do repositório:

```
cd imdb-scrapper
```

4. Execute o código:

```
python imdb_scrapper.py
```

**O que o código faz:**

O código funciona da seguinte forma:

1. Ele acessa a página "IMDB Most Popular Movies".
2. Ele analisa o HTML da página e encontra os links para as páginas individuais dos filmes.
3. Ele usa multithreading para acessar as páginas individuais dos filmes.
4. Para cada página de filme, ele extrai os seguintes dados:

* Título
* Ano
* Classificação
* Sinopse

5. Ele escreve os dados extraídos em um arquivo CSV chamado `movies.csv`.

**Observações:**

* O código pode precisar de ajustes se a estrutura do site do IMDb mudar.
* Considere usar nomes de variáveis mais descritivos para melhor legibilidade.
* Explore o tratamento de erros para tornar o código mais robusto.

**Exemplo de saída:**


Título | Ano | Classificação | Sinopse
------- | -------- | -------- | --------
The Shawshank Redemption | 1994 | 9.3 | Andy Dufresne, um banqueiro acusado de matar sua esposa e seu amante, é condenado à prisão perpétua na Penitenciária Estadual de Shawshank, no Maine. Lá, ele faz amizade com Red, um contrabandista experiente, e começa a trabalhar na lavanderia da prisão. Com o tempo, Andy se torna um membro respeitado da comunidade carcerária e começa a planejar uma fuga.
The Godfather | 1972 | 9.2 | A história da família Corleone, uma das mais poderosas famílias mafiosas da cidade de Nova York. O patriarca Vito Corleone (Marlon Brando) é um homem respeitado e temido em toda a cidade. Seus filhos Michael (Al Pacino), Sonny (James Caan) e Fredo (John Cazale) estão envolvidos nos negócios da família, mas cada um deles tem suas próprias ambições e desejos.
The Dark Knight | 2008 | 9.0 | Bruce Wayne/Batman (Christian Bale) e James Gordon (Gary Oldman) formam uma parceria para combater o crime em Gotham City. Seu principal inimigo é o Coringa (Heath Ledger), um criminoso psicótico que quer destruir a cidade.
The Godfather: Part II | 1974 | 9.0 | Continuação do filme "O Poderoso Chefão". O filme conta a história da família Corleone desde a ascensão de Vito Corleone (Marlon Brando) até a queda de Michael Corleone (Al Pacino).
12 Angry Men | 1957 | 9.0 | Um jurado é designado para um caso de assassinato. Ele é o único que acredita na inocência do réu.
