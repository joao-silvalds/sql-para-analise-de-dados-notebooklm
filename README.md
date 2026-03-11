# Desafio DIO com NotebookLM  
# SQL para Análise de Dados

# Contexto

Este projeto foi desenvolvido como parte de um desafio prático da DIO com o objetivo de explorar o uso da Inteligência Artificial como ferramenta de aprendizagem.

Utilizando o NotebookLM, organizei fontes de estudo sobre SQL aplicado à análise de dados, realizei testes de engenharia de prompts e produzi um miniguia consolidado para revisão e aprendizado.

# Objetivos de Estudo

Os principais objetivos deste estudo foram:

- Compreender como SQL é utilizado na análise de dados
- Aprender os principais comandos SQL utilizados por analistas de dados
- Desenvolver prompts eficientes para extrair conhecimento do NotebookLM
- Criar um material de estudo estruturado para revisões futuras

# Curadoria de Fontes

As seguintes fontes abertas foram utilizadas no NotebookLM:

1. https://www.thoughtspot.com/sql-tutorial
2. https://pm3.com.br/blog/sql-para-analise-de-dados/
3. https://learnsql.com.br/blog/sql-para-analise-de-dados-o-que-devo-aprender/
4. https://clarify.com.br/blog/principais-comandos-sql-analise-dados/
5. https://www.dio.me/articles/analise-de-dados-usando-sql
6. https://www.youtube.com/watch?v=3YYi-c4E1aI - O que é sql?
7. https://www.youtube.com/playlist?list=PLvlkVRRKOYFRo651oD0JptVqfQGDvMi3j - Aprenda SQL
8. Livro: SQL para análise de dados - Cathy Tanimura

Essas fontes foram selecionadas por apresentarem conteúdos confiáveis e introdutórios sobre SQL aplicado à análise de dados.

# Engenharia de Prompts

Durante o uso do NotebookLM foram testadas diferentes estratégias de prompts para obter respostas mais completas.

## Prompt 1

Explique o que é SQL e qual sua importância para análise de dados.

### Resultado

O SQL (Structured Query Language) é a linguagem padrão e universal usada para se comunicar com bancos de dados relacionais
. Ela permite que analistas e engenheiros de dados realizem consultas para acessar, manipular, filtrar e extrair informações organizadas em tabelas
. Desenvolvida inicialmente pela IBM com base no modelo relacional de Edgar Codd, o SQL tornou-se um padrão essencial por permitir que o usuário descreva o que deseja obter enquanto o sistema gerencia a execução da tarefa, o que a caracteriza como uma linguagem declarativa
.
A importância do SQL para a análise de dados é fundamentada em diversos pilares:
Acesso e Ubiquidade: A grande maioria dos dados mundiais e corporativos já está armazenada em bancos de dados relacionais, tornando o SQL a ferramenta de fato para interagir com essas informações
.
Poder Computacional e Escalabilidade: O SQL é executado diretamente nos servidores de banco de dados, aproveitando todos os seus recursos para processar volumes massivos de dados (terabytes ou petabytes) com rapidez e eficiência, superando as limitações de memória de ferramentas como planilhas
.
Integração e Interoperabilidade: Como é um padrão de mercado, o SQL integra-se perfeitamente com quase todas as ferramentas modernas de BI e visualização (como Power BI, Tableau e Excel), além de complementar linguagens como Python e R
.
Tratamento e Preparação de Dados: Ele é essencial em todas as etapas do fluxo de análise, permitindo a limpeza, transformação e agregação de dados brutos para torná-los prontos para gerar insights, garantindo a integridade e consistência das informações
.
Tomada de Decisão: Ao permitir consultas precisas e rápidas, o SQL capacita os profissionais a responderem perguntas de negócios de forma estratégica, identificando tendências, padrões e anomalias que fundamentam decisões baseadas em dados
.
Em resumo, habilidades sólidas em SQL são indispensáveis para transformar dados brutos em ativos valiosos, permitindo uma exploração eficiente que gera impacto direto no desempenho das organizações


### Observação

A resposta foi clara e bem detalhada.

---

## Prompt 2

Quais são os principais comandos SQL utilizados por analistas de dados?

### Resultado

Os analistas de dados utilizam uma variedade de comandos SQL para extrair, filtrar e transformar informações, sendo a Data Query Language (DQL) a sublinguagem mais utilizada no dia a dia
.
Abaixo estão os principais comandos e cláusulas divididos por suas funções:
1. Comandos de Consulta e Recuperação (DQL)
Estes são os fundamentos para qualquer análise de dados:
SELECT: O comando mais essencial, usado para especificar quais colunas você deseja recuperar de uma tabela
.
FROM: Indica a origem dos dados, ou seja, de qual tabela ou conjunto de tabelas as informações serão extraídas
.
WHERE: Filtra os resultados com base em condições específicas, permitindo selecionar apenas as linhas que atendem a determinados critérios
.
DISTINCT: Utilizado para retornar apenas valores únicos em uma coluna, eliminando duplicatas dos resultados
.
LIMIT: Uma cláusula importante para evitar o travamento do banco de dados ao retornar apenas um número limitado de registros (útil para testes e criação de perfis)
.
2. Integração e Agregação de Dados
Para análises mais complexas, os analistas combinam e resumem informações:
JOIN: Combina dados de duas ou mais tabelas com base em relacionamentos comuns (ex: INNER JOIN, LEFT JOIN, RIGHT JOIN e FULL OUTER JOIN)
.
GROUP BY: Agrupa os resultados com base nos valores de uma ou mais colunas, permitindo a aplicação de funções de agregação
.
HAVING: Semelhante ao WHERE, mas usado especificamente para filtrar os resultados que já foram agrupados pelo GROUP BY
.
ORDER BY: Ordena os resultados da consulta em ordem crescente (ASC) ou decrescente (DESC)
.
3. Funções de Agregação
Frequentemente usadas com o GROUP BY para gerar estatísticas
:
COUNT: Calcula o número total de registros
.
SUM: Realiza a soma de valores numéricos
.
AVG: Calcula a média dos valores
.
MAX e MIN: Identificam os valores máximo e mínimo de um conjunto
.
4. Comandos de Manipulação e Definição (DML e DDL)
Embora menos frequentes na fase pura de análise, são cruciais na preparação de dados:
INSERT, UPDATE e DELETE: Usados para adicionar, modificar ou excluir registros em tabelas autogerenciadas ou sandboxes
.
CREATE, ALTER e DROP: Comandos de Definição de Dados (DDL) usados para criar novos objetos (como tabelas temporárias ou views), estruturar colunas ou excluir objetos inteiros
.
5. Recursos Avançados
Analistas experientes também utilizam:
Subqueries: Consultas aninhadas dentro de outras consultas para realizar cálculos complexos
.
CTEs (Common Table Expressions): Definidas pela palavra-chave WITH, criam conjuntos de resultados temporários que tornam o código mais organizado e legível
.
Window Functions (Funções de Janela): Realizam cálculos em um intervalo de linhas (como RANK, LEAD, LAG e NTILE) sem reduzir o número de linhas no resultado final
.

### Dificuldade encontrada

O modelo inicialmente listou apenas comandos básicos devido a limitação de fontes, porém após adicionar outras fontes e permitir que ele buscasse informaçções adicionais ele apresentou uma resposta detalhada. 

---

## Prompt 3 

Explique os diferentes tipos de JOIN em SQL e quando cada um deve ser utilizado.

### Resultado

O JOIN é um comando fundamental em SQL utilizado para combinar dados de duas ou mais tabelas com base em relacionamentos comuns entre elas
. Geralmente, essa combinação é feita através de uma condição de igualdade especificada na cláusula ON, embora também possam ser utilizadas desigualdades ou intervalos de valores
.
Abaixo estão os diferentes tipos de JOIN e quando utilizá-los:
1. INNER JOIN
Este comando retorna apenas os registros que possuem valores correspondentes em ambas as tabelas envolvidas na consulta
.
Quando utilizar: Use o INNER JOIN quando você deseja extrair apenas as informações que são comuns a ambos os conjuntos de dados, descartando linhas que não possuam um par correspondente na outra tabela
.
2. LEFT JOIN (ou LEFT OUTER JOIN)
Retorna todos os registros da primeira tabela (à esquerda) e apenas os registros da segunda tabela (à direita) que sejam coincidentes
. Caso não haja correspondência, o resultado trará valores nulos para as colunas da segunda tabela
.
Quando utilizar: É muito útil para identificar dados ausentes ou lacunas na segunda tabela, como encontrar clientes que nunca realizaram uma compra
. Na prática da análise de dados, o LEFT JOIN é muito mais utilizado do que o RIGHT JOIN
.
3. RIGHT JOIN (ou RIGHT OUTER JOIN)
Funciona de forma inversa ao anterior, retornando todos os registros da segunda tabela (à direita) e apenas os correspondentes da primeira tabela (à esquerda)
.
Quando utilizar: Deve ser usado quando o foco da análise é a integridade da segunda tabela em relação à primeira
. No entanto, analistas costumam preferir inverter a ordem das tabelas e usar um LEFT JOIN para facilitar a leitura lógica do código
.
4. FULL OUTER JOIN
Retorna todos os registros de ambas as tabelas, independentemente de haver ou não uma correspondência entre elas
. Onde não houver coincidência, o banco de dados preencherá as colunas com valores nulos
.
Quando utilizar: É útil quando você precisa de uma visão completa de dois conjuntos de dados e deseja manter todas as informações disponíveis de ambos, podendo ser uma alternativa ao uso de UNION em certos contextos
.
5. JOIN Cartesiana (ou CROSS JOIN)
Ocorre quando cada registro da primeira tabela é combinado com todos os registros da segunda tabela
.
Quando utilizar: Geralmente deve ser evitada, pois pode gerar volumes massivos de dados e travar o banco
. Contudo, é usada intencionalmente em casos específicos, como para preencher lacunas em séries temporais ou gerar todas as combinações possíveis de categorias para um relatório
.
Considerações Importantes para Analistas:
Aliases: É recomendável atribuir nomes curtos (aliases) às tabelas para tornar a consulta mais legível e evitar digitar nomes longos repetidamente
.
Cuidado com Duplicatas: Junções mal configuradas, como um relacionamento "muitos-para-muitos" oculto, podem gerar duplicidades acidentais que distorcem os resultados da análise
.
Desempenho: O desempenho do banco de dados pode ser afetado se a condição de JOIN contiver cálculos complexos em vez de igualdades simples entre campos indexados
.

### Observação

A resposta foi clara e bem detalhada, inclusive adicionando considerações relevantes.

---

# Miniguia de Estudo

## O que é SQL

## O que é SQL

SQL (Structured Query Language) é uma linguagem usada para gerenciar e consultar dados armazenados em bancos de dados relacionais.

Ela é amplamente utilizada em áreas como:

- Business Intelligence
- Análise de dados
- Engenharia de dados
- Ciência de dados

---

## Principais Comandos SQL para Análise de Dados

### SELECT

Usado para consultar dados de uma tabela.

SELECT nome, salario
FROM funcionarios;

### WHERE

Filtra registros com base em condições.

SELECT *
FROM vendas
WHERE valor > 1000;

### GROUP BY

Agrupa dados para realizar agregações.

SELECT categoria, SUM(valor)
FROM vendas
GROUP BY categoria;

### ORDER BY

Ordena os resultados da consulta.

SELECT *
FROM vendas
ORDER BY valor DESC;

### JOIN

Combina dados de múltiplas tabelas.

SELECT clientes.nome, pedidos.valor
FROM clientes
JOIN pedidos
ON clientes.id = pedidos.cliente_id;

# Glossário

SQL
Structured Query Language, linguagem usada para consultar bancos de dados.

Banco de Dados Relacional
Estrutura que organiza dados em tabelas relacionadas.

Query
Comando SQL utilizado para consultar ou manipular dados.

JOIN
Operação que combina dados de duas ou mais tabelas.

Agregação
Processo de resumir dados usando funções como SUM, AVG ou COUNT.

# Prompts Reutilizáveis

Alguns prompts úteis para revisar SQL:

- Explique os principais comandos SQL usados por analistas de dados.

- Crie exemplos práticos de consultas SQL para análise de dados.

- Explique a diferença entre JOIN, LEFT JOIN e INNER JOIN.

- Crie exercícios simples para praticar SQL.

# Conclusão

O uso do NotebookLM permitiu organizar fontes de estudo e testar diferentes abordagens de prompts para compreender conceitos de SQL aplicados à análise de dados.

Esse processo demonstrou como a Inteligência Artificial pode ser utilizada como ferramenta de apoio ao aprendizado técnico.
