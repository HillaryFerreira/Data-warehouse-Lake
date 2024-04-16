<h1>DATA WAREHOUSE</h1>
<p>Breve explicação do que foi criado no código:</p>
<ul>
  <li>Foram importadas as Bibliotecas 'panda' e 'numpy'</li>
  <li>Foi feita a definição das váriaveis 'num_produtos=600' e 'num_vendas=1000',ou seja, se refere a quantidade total de produtos e do número de vendas </li>
  <li>Um dicionário chamado produtos é criado, contendo informações fictícias sobre os produtos, como ID, nome e categoria.<br>
   Esses dados são usados para criar um DataFrame chamado df_produtos.</li>
  <li>Um dicionário chamado data_vendas é criado, contendo informações fictícias sobre as vendas, como data, ID do produto, quantidade vendida, valor unitário e valor total.<br>
Esses dados são usados para criar um DataFrame chamado df_vendas.</li>
  <li>Os DataFrames df_vendas e df_produtos são salvos em arquivos CSV chamados 'vendas.csv' e 'produtos.csv', respectivamente, sem incluir o índice.</li>
  <li>Os dados dos arquivos CSV recém-criados são lidos de volta para os DataFrames df_vendas e df_produtos.</li>
  <li>Os DataFrames df_vendas e df_produtos são mesclados com base no ID do produto usando um inner join, criando um novo DataFrame chamado df_merge.</li>
  <li>O DataFrame resultante da mescla é salvo em um arquivo CSV chamado 'data_warehouse.csv', sem incluir o índice.</li>
  <li>Os dados do arquivo CSV 'data_warehouse.csv' são lidos de volta para o DataFrame df_warehouse.</li>
  <li>O conteúdo do DataFrame df_warehouse é impresso na saída padrão, exibindo assim os dados finais armazenados no "data warehouse".</li>
</ul>
<h2>Resultados:</h2>
<ul>
  <li>O DataFrame df_warehouse é impresso na saída padrão, exibindo o conteúdo do "data warehouse" criado a partir da mesclagem dos dados de vendas e produtos.</li>
  <li>Os dados são organizados de forma tabular, onde cada linha representa uma venda realizada. As informações incluem a data da venda, o ID do produto vendido, a quantidade vendida, o valor unitário, o valor total da venda, o nome do produto e a categoria do produto.</li>
  <li>É possível observar que as informações dos produtos foram mescladas com as informações das vendas com base no ID do produto. Isso cria um conjunto de dados mais completo e útil para análise posterior, como a avaliação do desempenho de vendas por categoria de produtos, tendências de vendas ao longo do tempo, entre outras análises.</li>
</ul>
<h3>Imagem do reusltado gerado pelo código:</h3>
<a href="https://github.com/HillaryFerreira/Data-warehouse-Lake/assets/129438048/836ea5ca-2d20-4ce4-bc6b-321c129d58db">Resultado do código</a>

