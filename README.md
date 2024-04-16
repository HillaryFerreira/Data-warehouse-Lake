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
  <li>O DataFrame df_warehouse foi impresso na saída padrão, exibindo o conteúdo do "data warehouse" criado a partir da mesclagem dos dados de vendas e produtos.</li>
  <li>Os dados foram organizados de forma tabular, onde cada linha representa uma venda realizada. As informações incluem a data da venda, o ID do produto vendido, a quantidade vendida, o valor unitário, o valor total da venda, o nome do produto e a categoria do produto.</li>
  <li>É possível observar que as informações dos produtos foram mescladas com as informações das vendas com base no ID do produto. Isso cria um conjunto de dados mais completo e útil para análise posterior, como a avaliação do desempenho de vendas por categoria de produtos, tendências de vendas ao longo do tempo, entre outras análises.</li>
</ul>
<h3>Imagem do reusltado gerado pelo código:</h3>
<a href="https://github.com/HillaryFerreira/Data-warehouse-Lake/assets/129438048/836ea5ca-2d20-4ce4-bc6b-321c129d58db">Resultado do código-Imagem</a>

<h1>Data-Lake</h1>
<p>Explicação do que foi criado no código:</p>
<ul>
  <li>Verifica se o diretório 'data_lake' existe. Se não existir, ele cria esse diretório.</li>
  <li>Define o número de arquivos a serem criados (num_files) e o número de linhas por arquivo (num_rows_per_file).</li>
  <li>Inicia um loop para criar vários arquivos CSV, onde cada arquivo contém um DataFrame com dados aleatórios.<br>
  Para cada iteração do loop:
Gera dados aleatórios para três colunas (coluna1, coluna2 e coluna3) usando numpy.<br>
  Cria um DataFrame pandas a partir desses dados<br>
  Salva o DataFrame como um arquivo CSV no diretório 'data_lake', incrementando o nome do arquivo com o valor de 'i'.<br>
  Adiciona o nome do arquivo e o DataFrame à lista dfs.</li>
  <li>Após a criação dos arquivos, inicia outro loop para iterar sobre cada arquivo e DataFrame na lista dfs.</li>
  <li>Para cada arquivo e DataFrame:Imprime o nome do arquivo e imprime as primeiras linhas do DataFrame.</li>
  <li>Define uma string de conexão com um banco de dados SQLite chamado 'data_lake.db'.<br>
Cria uma engine de conexão com o banco de dados usando SQLAlchemy.</li>
  <li>Deveria de Ler os dados da tabela 'dados_1' do banco de dados para um DataFrame (essa parte está comentada no código pois estava dando erro).</li>
  <li>Imprime as primeiras linhas do DataFrame (essa parte também está comentada no código fornecido).</li>
</ul>
<p>Resumidamente, o código cria uma estrutura de "data lake" local, gerando múltiplos arquivos CSV com dados aleatórios e armazenando-os em um diretório específico. Ele também demonstra como ler esses dados de volta para DataFrames pandas e como conectar e interagir com o banco de dados SQLite.</p>

<h2>Resultados:</h2>
<ul>
  <li>A confirmação de que os dados do "data lake" foram gerados com sucesso.</li>
  <li>m seguida, para cada arquivo CSV criado, o código imprime o nome do arquivo e as primeiras linhas do DataFrame correspondente.</li>
  <li>Cada DataFrame contém três colunas: coluna1, coluna2 e coluna3, com dados gerados aleatoriamente para cada arquivo.</li>
  <li>Os valores das colunas coluna1 e coluna2 são números aleatórios, enquanto os valores da coluna3 são aleatoriamente escolhidos entre 'A', 'B' e 'C'.</li>
  <li>Os resultados mostram que os dados foram criados e salvos com sucesso em arquivos CSV no diretório 'data_lake', e cada arquivo contém um DataFrame com dados aleatórios gerados para as colunas especificadas. Isso confirma que o processo de criação do "data lake" e salvamento dos dados em arquivos CSV foi bem-sucedido.</li>
</ul>
<h3>Imagem dos Resultados obtidos:</h3>
<a href="https://github.com/HillaryFerreira/Data-warehouse-Lake/assets/129438048/67391e92-9b4f-40b2-8aa5-1dd5cb7106b2">Resultado- imagem</a><br>
<a href="https://github.com/HillaryFerreira/Data-warehouse-Lake/assets/129438048/e36fb175-a59c-4343-865e-ce614960bd40">Resultado- imagem</a><br>
<a href="https://github.com/HillaryFerreira/Data-warehouse-Lake/assets/129438048/945b2a74-dfd2-459c-88ca-d1ff33cb8029">Resultado- imagem</a><br>
<a href="https://github.com/HillaryFerreira/Data-warehouse-Lake/assets/129438048/92d3940c-cedf-4433-8cfa-05e151fcad1a">Resultado- imagem</a>





