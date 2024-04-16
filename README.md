# Data-warehouse

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
