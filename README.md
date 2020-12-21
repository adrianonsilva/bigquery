# BigQuery

- [1. Descrição](#link1)
- [2. Utilização](#link2)
- [3. Visualização](#link3)
- [4. Links](#link4)

<a id="link1"></a>
## 1. Descrição

BigQuery é um data warehouse na nuvem que permite análise de forma escalonável usando consultas SQL sobre
grandes datasets.

Na forma de Platafoma como Serviço (PaaS), toda a infra estrutura é gerenciada pelo Google, retirando do cliente a preocupação com o gerenciado de servidores, backup, atualizações.

<a id="link2"></a>
## 2. Utilização

Clientes novos ganham US$ 300 em créditos para gastar no Google Cloud nos primeiros 90 dias. Todos os clientes recebem 10 GB de armazenamento e até 1 TB de consultas/mês, completamente grátis. Após esse período serão aplicadas as cobranças decorrentes da utilização.

Para os testes que serão realizados, será utilizado o BigQuery Sandbox que permite a avaliação free, mas com algumas limitações.

- 10 GB de armazenamento ativo
- 1 TB de dados de consulta processados por mês.
- Todos os datasets têm o prazo de validade de 60 dias

![Screenshot](/images/b01.jpg)

- Na seção Recursos do painel de navegação, expanda o projeto e criar um conjunto de dados.

![Screenshot](/images/b02.jpg)

- Informe um nome para o dataset, note que como é um projeto sandbox a validade é de 60 dias.

![Screenshot](/images/b03.jpg)

- No lado direito da janela, no painel de detalhes, clique em criar tabela. O processo de carregamento de dados é igual ao de criação de uma tabela vazia.

![Screenshot](/images/b04.jpg)

![Screenshot](/images/b05.jpg)

- Em criar tabele, selecione Fazer Upload

- Selecione o tipo de arquivo

![Screenshot](/images/b06.jpg)

![Screenshot](/images/b07.jpg)

- Clique no botão Criar Tabela

- Ne Editor de consultas, podemos escrever as consultas sql

Onde o formato é RECURSO.DATASET.TABELA 

ex: SELECT  FROM `bigquery-296404.pagamento.tb_pag` LIMIT 1000

![Screenshot](/images/b08.jpg)

<a id="link3"></a>
## 3. Visualização

Podemos usar várias ferramentas para visualição:

- Looker
- Data Studio
- Google Sheets
- Ferramentas BI

![Screenshot](/images/v01.jpg)

- Vamos executadar uma consulta para analizarnos os valores de pagametos por periodo (ano-mês)

![Screenshot](/images/b09.jpg)

- Clicando em EXPLORAR DADOS, podemos usar o Data Studio para visialização

![Screenshot](/images/b10.jpg)

![Screenshot](/images/b11.jpg)

![Screenshot](/images/b12.jpg)

![Screenshot](/images/b13.jpg)

- Vamos trocar a métrica de Record Count pelo total

![Screenshot](/images/b14.jpg)

![Screenshot](/images/b15.jpg)

- Vamos classificar pelo periodo

![Screenshot](/images/b16.jpg)

- Vamos trocar filtrar o ano de 2019

![Screenshot](/images/b17.jpg)

![Screenshot](/images/b18.jpg)

- Na aba estilo, podemos melhorar o layout do gráfico, para esse exemplo vamos incluir os nomes no eixo e os valores

![Screenshot](/images/b19.jpg)

![Screenshot](/images/b20.jpg)

Esse foi um exemplo de uma consulta e visualização simples usando o BigQuery e Data Studio, análises mais complexas e em grandes volumes de dados podem ser realizados usando a plataforma.

<a id="link4"></a>
## 4. Links

BigQuery</br>
https://cloud.google.com/bigquery

BigQuery Console</br>
https://console.cloud.google.com/

BigQuerySpotlight</br>
https://www.youtube.com/watch?v=d3MDxC_iuaw&list=PLIivdWyY5sqLAbIdmcMwsxWg-w8Px34MS

Data Studio</br>
https://support.google.com/datastudio/answer/6283323?hl=en