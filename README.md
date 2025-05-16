# PI-5. Apoio Decisorio aos Negocios
Grupo 1
- Fabiane Yoshie Otani da Silva
- Fernando Messias da Mata
- Jonatas de Lima Barros
- Jorge de Carvalho Cavalcanti
- Leandro Fragoso Blanco
- Lucas Barbosa Oliveira
- Wanderlucio de Almeida da Silva

# 3. Definição das Tecnologias
Nesta etapa, foi realizada a escolha das ferramentas e tecnologias utilizadas para a execução do projeto de **ETL** e análise **OLAP**. As decisões foram guiadas pela natureza dos dados, a complexidade do tratamento necessário e a necessidade de integração com ferramentas analíticas.

As seguintes tecnologias foram definidas e empregadas:

## Planilha Excel
Utilizada como fonte inicial de dados, onde foram feitas as adequações manuais e a normalização preliminar.  
* *Descrição da fonte, conforme sugestão acadêmica e tema do trabalho.*

## MySQL
Banco de dados relacional escolhido para armazenar os dados estruturados e preparados para análises futuras.  
Foi criada a base de dados chamada `projeto_integrador` e tabelas correspondentes à estrutura da planilha, incluindo:
- Coluna `id` como chave primária auto-incremental.
- Colunas com nomes padronizados, compatíveis com as regras do banco.
- Inserção de dados com tratamento de células em branco como `NULL` e datas no formato `yyyy-mm-dd`.

## PowerBI
Realizar consultas multidimensionais.
Criar dashboards analíticos.
Controlar e rastrear o progresso do projeto, facilitando a visualização de padrões e indicadores importantes.

## Navicat
Ferramenta gráfica utilizada para gerenciar o banco de dados MySQL de forma prática e visual. 

- Criação das tabelas e inserção de dados.
- Geração de dois gráficos com o objetivo de testar o gerenciamento de integração entre os dados do banco e a ferramenta.
Além dessas, outras tecnologias que normalmente são consideradas nesta etapa e podem complementar o projeto incluem:

## Git
Sistema de controle de versão distribuído, utilizado para registrar o histórico das alterações no projeto. Permite colaboração entre diferentes integrantes da equipe, criação de ramificações (branches) para testes ou novas funcionalidades, e recuperação de versões anteriores.

## Markdown
Linguagem de marcação leve utilizada para documentação técnica do projeto. Sua sintaxe simples permite escrever documentos estruturados como arquivos README, instruções de uso, manuais técnicos e relatórios, mantendo a legibilidade tanto em editores de texto quanto em visualizadores como o GitHub.

# 4. Detalhamento Técnico
Esta etapa tem como objetivo documentar tecnicamente todas as ações e decisões tomadas durante o desenvolvimento do projeto, facilitando a manutenção, auditoria e entendimento por outros membros da equipe ou stakeholders.

## Pré-processamento da planilha
- Normalização da estrutura.
- Padronização dos nomes das colunas para coincidirem com os nomes das tabelas no MySQL.
- Inclusão de coluna `id` como chave primária, com valores sequenciais na planilha e auto-incremento no MySQL.
- Substituição de células em branco por `NULL`.
- Padronização do formato de datas para `YYYY-MM-DD`.

## Normalização e tratamento dos dados de entrada
- Padronização dos nomes das colunas para corresponderem às tabelas no MySQL.
- Inserção da coluna `id` na planilha e no banco, garantindo integridade relacional.
- Tratamento de células em branco, substituindo por `NULL` para compatibilidade com bancos de dados.
- Formatação uniforme de datas no padrão `YYYY-MM-DD`.
- Navicat: utilizado para criação de tabelas, gestão do banco e construção de gráficos de teste para validar a integração com os dados do MySQL.

## Estrutura da base de dados `projeto_integrador`
- Tabelas criadas com base na estrutura da planilha, mantendo os tipos de dados adequados (ex: `VARCHAR` para textos, `DATE` para datas).
- Definição de `id` como chave primária com auto-incremento no MySQL.
- Utilização de comandos SQL como `CREATE TABLE` e `INSERT INTO` com os dados tratados.

## Ferramentas de versionamento e documentação
### Git: utilizado para versionar os scripts SQL, scripts de ETL (caso existam) e arquivos de documentação. As práticas comuns incluem:
Commits frequentes com mensagens descritivas.
Uso de branches para desenvolver novas funcionalidades ou melhorias de forma isolada.
Armazenamento remoto no GitHub ou GitLab para facilitar o trabalho colaborativo.

### Markdown: empregado para elaborar:
Documentação técnica com estrutura clara (README.md, docs/).
Registro das tecnologias utilizadas, instruções para execução local, e descrição das tabelas do banco.
Relatórios intermediários e finais, com formatação leve e visualmente organizada (títulos, listas, tabelas de exemplo, blocos de código SQL).

## Visualização
Power BI:
- Conectado ao banco MySQL para realizar consultas OLAP.
- Criação de dashboards interativos para análise e visualização dos dados.
- Acompanhamento do progresso do projeto por meio de indicadores visuais.
