# Curso Node.js: testes unitários e de integração (Alura e Programa Desenvolve da Boticário)

> Status do projeto: em desenvolvimento

Conteúdo do curso:

* O porquê de testamos aplicações e sistemas, isto é, para aumentar a confiabilidade e qualidade do código;

* Alguns dos tipos de testes que podemos implementar, como: os estáticos, unitários, de integração e E2E. Sendo:
1. Testes estáticos - voltados para analisar o código sem necessariamente executá-lo, verificando se algumas boas práticas e formatação padronizada foram adotadas na implementação;
2. Testes unitários- são utilizados para verificar o comportamento das menores unidades de código da aplicação;
3. Testes de integração - são as fases do teste de software em que módulos são combinados e testados como um conjunto;
4. Teste E2E (End-to-End) - é um método de teste utilizado para testar um fluxo da aplicação desde o começo até o fim;

* O que é ter uma cultura de testes e alguns de seus benefícios, como a padronização e estabelecimento de processos para o nosso projeto;

* Como utilizar o ESLint para fazer testes estáticos em JS estabelecendo um padrão de escrita para o código, verificando se há divergências entre o código escrito e o padrão adotado e também analisando a estrutura do projeto em busca de problemas como módulos inexistentes, falta de clareza nas declarações etc;

* A implementar os primeiros testes de unidade utilizando um código implementado do zero;

* Utilizar métodos nativos de asserções para fins de comparação de igualdade;

* Instalar e executar o Jest com a flag --experimental;

* Criar arquivos de testes com o Jest e analisar erros;

* Usar a função describe um método do Jest usado para conjunto de testes relacionados. O describe possui a sintaxe de dois argumentos:
1. Uma string para descrever;
2. Uma função callback para executar o teste.

* Gerar relatório com o coverage, uma ferramenta integrada do jest para cobertura de testes, que possibilita identificar caminhos não testados no código;

* Usar Matchers para diferentes formas de testes, comparando igualdade, inclusão, erros e propriedades de valores;

* Alinhar o uso do matcher com asserções e estrutura de dados para utilizar em arrays, partes de objetos e conjuntos;

* Identificar as situações de "falso positivo", por meio da análise do percentual de cobertura com a flag --coverage;

* Reconhecer que nem sempre quando obtivermos 100% de cobertura de acordo com um relatório estaremos realmente testando todo o código;

* Conhecemos algumas formas que falso-positivos podem existir nos nossos testes.
