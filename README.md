# G1 PI - APOIO DECISorio-RIO-AOS-NEG-CIOS-

# 3. Definição das Tecnologias
Nesta etapa, foi realizada a escolha das ferramentas e tecnologias utilizadas para a execução do projeto de **ETL** e análise **OLAP**. As decisões foram guiadas pela natureza dos dados, a complexidade do tratamento necessário e a necessidade de integração com ferramentas analíticas.

As seguintes tecnologias foram definidas e empregadas:

## Planilha Excel
Utilizada como fonte inicial de dados, onde foram feitas as adequações manuais e a normalização preliminar.  
*Descrição da fonte, conforme sugestão acadêmica e tema do trabalho.*

## MySQL
Banco de dados relacional escolhido para armazenar os dados estruturados e preparados para análises futuras.  
Foi criada a base de dados chamada `projeto_integrador` e tabelas correspondentes à estrutura da planilha, incluindo:
- Coluna `id` como chave primária auto-incremental.
- Colunas com nomes padronizados, compatíveis com as regras do banco.
- Inserção de dados com tratamento de células em branco como `NULL` e datas no formato `yyyy-mm-dd`.

## PowerBI
Além dessas, outras tecnologias que normalmente são consideradas nesta etapa e podem complementar o projeto incluem:
Git e Markdown
- Inclusão do **Power BI** como ferramenta de análise visual.
- Para controle e rastreamento do progresso do projeto.

# 4. Detalhamento Técnico
Esta etapa tem como objetivo documentar tecnicamente todas as ações e decisões tomadas durante o desenvolvimento do projeto, facilitando a manutenção, auditoria e entendimento por outros membros da equipe ou stakeholders.

## Normalização e tratamento dos dados de entrada
- Padronização dos nomes das colunas para corresponderem às tabelas no MySQL.
- Inserção da coluna `id` na planilha e no banco, garantindo integridade relacional.
- Tratamento de células em branco, substituindo por `NULL` para compatibilidade com bancos de dados.
- Formatação uniforme de datas no padrão `YYYY-MM-DD`.

## Estrutura da base de dados `projeto_integrador`
- Tabelas criadas com base na estrutura da planilha, mantendo os tipos de dados adequados (ex: `VARCHAR` para textos, `DATE` para datas).
- Definição de `id` como chave primária com auto-incremento no MySQL.
- Utilização de comandos SQL como `CREATE TABLE` e `INSERT INTO` com os dados tratados.

## Caminhos possíveis para a próxima etapa
- **Execução de consultas OLAP**: criação de visões (`views`), uso de cláusulas `GROUP BY`, `ROLLUP`, `CUBE` e `JOIN` para análises multidimensionais.
- **Criação de dashboards**: conexão do banco MySQL com ferramentas como Power BI ou Tableau para apresentação visual dos dados.
- **Automatização do processo de ETL**: script em Python ou ferramentas de ETL para automatizar a importação e transformação contínua dos dados.
