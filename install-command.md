## Instalação dos drivers do SQLite (Windows)

* Faça o download dos drivers SQLite na página: https://www.sqlite.org/download.html;

* Selecione o sistema operacional e faça o download do arquivo Precompiled binaries for Windows - SQLite Tools;

* Crie uma pasta chamada sqlite3 na unidade C:\ do seu computador. O caminho final será: C:\sqlite3 ;

* Insira os arquivos SQLite descompactados na pasta C:\sqlite3 (você deverá extrair os arquivos para a pasta C:\sqlite3);

* Para permitir que a CLI do SQLite3 possa ser utilizada em diferentes locais, precisamos adicionar uma variável de ambiente ao Windows. Siga os passos:

1. Abra "Exibir configurações avançadas do Sistema" (Advanced System Properties). Painel de controle (Control Panel) > Sistema (System) > Configurações avançadas do Sistema (Advanced System Settings).

2. Selecione "Variáveis de Ambiente"

3. Em variáveis de sistema, selecione a variável PATH e clique em Editar..
Adicione C:\sqlite3 ao final e selecione a opção “Ok”

* Depois execute o cmd como administrador e rode o comando sqlite3.

## Configuração dos drivers SQLite

* Verifique a instalação com: sqlite3 --version ;

* Vamos utilizar a CLI (interface de linha de comando) do SQLite para acessar o arquivo e fazer consultas ao banco via terminal. Abra o terminal, navegue até a pasta onde o projeto foi baixado e instalado e insira o comando sqlite3 ./src/db/livraria.sqlite ;

* O terminal deverá exibir a seguinte mensagem (a data e hora do acesso serão as locais do momento em que você acessar): <br>
SQLite version 3.31.1 2020-01-27 19:55:54 <br>
Enter ".help" for usage hints. <br>
sqlite> 

* Digite os seguintes comandos no terminal do SQLite para verificar se a versão instalada tem suporte a FKs (foreign keys): <br>
PRAGMA foreign_keys;

* Deve retornar 1 se o suporte estiver habilitado e 0 se não estiver. Caso não esteja, insira o seguinte comando no terminal do SQLite para ativar: <br>
PRAGMA foreign_keys = ON;

* Você pode rodar novamente o comando PRAGMA foreign_keys; para verificar novamente se o suporte está habilitado. Agora deve retornar 1.

## Acesso ao banco de dados

* Você pode utilizar o CLI do SQLite para fazer consultas ao banco e conferir se os dados iniciais estão retornando;

* Utilize a CLI do SQLite para acessar o arquivo src/db/livraria.sqlite. Abra o terminal, navegue até a pasta do projeto e insira o comando: sqlite3 ./src/db/livraria.sqlite ;

* Digite o comando .tables para exibir no terminal as tabelas já criadas no banco: <br>
sqlite> .tables <br>
autores   editoras  livros 

* Digite SELECT * FROM autores; para exibir no terminal o conteúdo da tabela autores: <br>
sqlite> SELECT * FROM autores;
1|JRR Tolkien|sul-africano|2022-06-06 19:30:55 <br>
2|Ursula LeGuin|estadunidense|2022-06-06 19:30:55 <br>
3|Machado de Assis|brasileira|2022-06-06 19:30:55 <br>
sqlite> 

* Você pode testar os comandos SELECT * FROM livros; e SELECT * FROM editoras; para conferir os dados destas tabelas que já deixamos prontos para serem usados na API.

## NPM

* npm install

* npm run dev