# Carga-Dados-para-Data-Warehouse-com-SSIS

## Objetivo:
O projeto "Carga Dados para Data Warehouse com o SSIS" é uma solução de Business Intelligence que visa centralizar os dados de várias fontes em um único local (Data Warehouse) utilizando o SQL Server Integration Services (SSIS).

O objetivo é demonstrar a criação de um fluxo de ETL (Extração, Transformação e Carga) que extrai dados da fonte de banco de dados SQL Server, realiza transformações e carrega os dados em um Staging Area e, posteriormente, no Data Warehouse.


## Passos do Projeto:

#### Passo 1: Definição e Planejamento

- Definir os Requisitos:
Compreender as necessidades da empresa e dos usuários, como quais dados precisam ser carregados, com que frequência e quais transformações são necessárias.

- Análise de Fonte de Dados: 
Avaliar a fonte de dados (no caso, um banco de dados SQL Server) e entender sua estrutura, tabelas, relacionamentos e tipos de dados.

- Especificação do Data Warehouse:
  Definir a estrutura do Data Warehouse, incluindo as tabelas dimensionais e fatos, bem como as regras de negócios para agregações e métricas.
  
- Planejamento de Transformações:
Identificar as transformações necessárias para limpar, enriquecer e formatar os dados para atender aos requisitos do Data Warehouse.

#### Passo 2: Configuração das Fontes de Dados
- Definição da Conexão de Origem: Criar uma conexão OLE DB para o banco de dados de origem (SQL Server) no projeto SSIS.

- Criação do Pacote de Extração: Criar um pacote SSIS que utilize a conexão de origem para extrair os dados necessários das tabelas de fonte.


#### Passo 3: Transformação dos Dados


#### Passo 4: Carga no Staging Area

- Definição da Conexão de Staging: Criar uma nova conexão OLE DB para a área de Staging no projeto SSIS.

- Criação do Pacote de Staging: Criar um novo pacote SSIS que utilize a conexão de Staging para carregar os dados transformados na área de Staging.

#### Passo 5: Carga no Data Warehouse

- Definição da Conexão do Data Warehouse: Criar uma conexão OLE DB para o Data Warehouse no projeto SSIS.

- Criação do Pacote de Carga: Criar um novo pacote SSIS que utilize a conexão do Data Warehouse para carregar os dados da Staging Area nas tabelas dimensionais e de fatos.

#### Passo 6: Agendamento e Execução

- Agendamento de Execução: Configurar um agendamento para executar automaticamente os pacotes SSIS de acordo com a frequência necessária.

- Monitoramento e Logging: Implementar mecanismos de monitoramento e logging para acompanhar a execução dos pacotes e identificar possíveis problemas.

#### Passo 8: Testes e Validação

- Teste de Unidade: Testar cada etapa do processo de ETL individualmente para garantir que as transformações e carregamentos estejam funcionando conforme o esperado.

- Teste de Integração: Executar o fluxo completo do ETL, desde a extração até a carga no Data Warehouse, para verificar a integridade dos dados e a conformidade com as regras de negócios.


![ssis](https://github.com/DeboraSouza277/Carga-Dados-para-Data-Warehouse-com-SSIS/blob/main/SSIS_Package.PNG)








