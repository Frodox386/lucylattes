# LATTES_SCRAPER

## Motivação


## O que faz

Organiza os dados dos currículos da plataforma *Lattes* em arquivos de
texto organizados que proporcionam rapidez para a geração de
informação. 

## Desenvolvimento

- [X] Salva em pastas específicas arquivos `.csv` individuais para cada
pesquisador:
    - os projetos de pesquisa e extensão;
    - cursos de curta duração
    - orientações (tcc, ic, mestrado)
    - publicações em periódico com qualis, revista
- [X] Capturar os projetos de pesquisa, e extensão, com seus respectivos
participantes, classificação do tipo de projeto (pesquisa ou extensão)
organizando os dados em um `DataFrame`; 
- [X] Capturar produção técnica de cada pesquisador
- [X] Capturar as atividades de orientação;
- [X] Ler o `.xml` direto do `.zip`;
- [X] Realizar um looping para caturar uma série de currículos.
- [X] Capturar produção em periódicos;
- [X] Associar produção em periódico com capes qualis;
- [ ] Capturar as atividades dos projetos de extensão;
- [ ] Gerar um `.json` file para cada currículo;

## Histórico

- 20190214: foi criado um arquivo `config.txt` com objetivos de:
    - especificar o arquivo `.csv` que será utilizado no qualis.

- 20190213: função para capturar os periódicos com qualis foi concluída,
os arquivos `.xlm` foram movidos para a pasta `xlm_zip`.

- 20190212: os arquivos `.xlm` são lidos diretamente do arquivo
`.zip`. Foi criado um arquivo **lista** no formato `.csv`, neste arquivo
deve conter o **id** *Lattes* de cada pesquisador e seus respectivo nome.

- 20190126: do arquivo xlm do lattes é possível extrair o nome do
projeto, tipo do projeto, ano de início, e integrantes, etc

## Arquivos

- `parserlattes.py`: contém as funções que extraem as informações
necessárias e geram os `.csv`
- `readidlist.py`: faz a leitura da lista que contém o **id** dos pesquisadores 
- `scriptLattes.py`: funciona como o executável
- `config.txt`: cpnfigurações para funcionamento do script

## Autor

- Rafael Tieppo
- rafaeltieppo@yahoo.com.br
- https://rafatieppo.github.io/



