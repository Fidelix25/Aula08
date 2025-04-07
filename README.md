# Pipeline de Extração, Transformação e Carga.

🐍 Utilizando Python foram criadas funções para extrair, transformar e carregar dados.
Neste exemplo os dados estavam salvos em uma pasta no formato JSON, contudo poderiam ser
dados extraídos de uma API ou banco de dados, por exemplo.

#### Extract

1. A primeira função lê os arquivos dentro da pasta e faz a combinação(merge) dos arquivos e cria um dataframe com a estrutura Pandas

#### Transform

2. A segunda função lê o Dataframe gerado pela função anterior e adiciona uma coluna calculada. O cálculo se baseia nas colunas 'Quantidade' e 'Venda' para chegar ao Valor Total.

#### Load

3. A terceira função faz com que arquivos sejam gerados em formato csv, parquet ou ambos, a depender da escolhado do usuário da pipeline. Neste case, ao executar o código os arquivos são no respectivo formato são adicionados, novamente este exemplo poderia inserir os dados em um banco de dados

#### Orchestration

4. Por fim, uma última função foi criada para executar as outras função, criando uma espécie de orquestração para que o código seja executado na ordem correta, além de simplificar a vida do usuário final que fica responsável apenas por indicar a pasta em que os arquivos estão e formato que deseja visualizar os arquivos.

#### Bibliotecas Python

Foram utilizados neste projetos as bibliotecas <b>Pandas, OS e Glob</b>
