#MVP Data Engineering
@author: Monique Dali

Course: Data Science & Analytics

University: PUC-Rio

##Database
The information was extracted from the public database of Brazilian's national oil regulator agency. This dataset contains montly information about crude oil and natural gas production per well located in Brazil. Only the accessible montly production of 2023 was downloaded. On the time of this work, July was the last month updated.

The dataset is available in: https://www.gov.br/anp/pt-br/centrais-de-conteudo/dados-abertos/producao-de-petroleo-e-gas-natural-por-poco

AWS was chosen as the cloud service to perform the ETL jobs.

image.png

Metadata is also available in: https://www.gov.br/anp/pt-br/centrais-de-conteudo/dados-abertos/arquivos/arquivos-producao-de-petroleo-e-gas-natural-por-poco/metadados-dados-producao-poco.pdf

image.png

##Data quality
There are many problems in this public dataset:

Variations in the name of the states, fields and basins difficulting aggregation and calculation;
Empty columns;
Wells without crude oil production.
Attention points:

Files with semicolon (;) separator;
Numbers in brazilian format: decimal separator is comma (,) and thousand separator is dot (.)
Proposal
With this database, data analysis process wants to answer a couple of general questions about crude oil commercial extraction during 2023 in Brazil.

##Goals:

Crude oil production analysis

What is the crude oil production of brazil accumulated in 2023?
What was the oil production per month?
What is the crude oil production accumulated per well location?
What are the top companies in oil production in 2023 with total number of wells and average oil production per well?
What is the most productive state?
What is the most productive field?
What is the most productive well?
Water is an undesirable subproduct of oil extraction. Water injection is widely used as secondary recovery method in wells. However, it is not good to produce water in high levels. Mature wells have oil production curve in decline.

What is the worst state in terms of crude oil extraction efficience?
In which state are located the worst fields in efficience?
What are the 10 most inneficient wells with oil production?
