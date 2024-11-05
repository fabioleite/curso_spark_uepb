# Curso de Introdução a análise de dados com Spark
## Visão geral de Spark(https://spark.apache.org/)

Apache Spark é uma plataforma de computação em *cluster* que fornece uma API para
*programação distribuída* para *processamento de dados* em *larga escala*,
semelhante ao modelo *MapReduce*, mas projetada para ser rápida para consultas interativas
e algoritmos iterativos.

O Spark permite que você distribua dados e tarefas em clusters com vários nós.
Imagine cada nó como um computador separado. A divisão dos dados torna mais fácil o trabalho com conjuntos de
dados muito grandes porque cada nó funciona processa apenas uma parte parte do volume total de dados.

### Processamento distribuído
O Spark permite que você distribua dados e tarefas em clusters com vários nós. Imagine cada nó como um computador separado. A divisão dos dados torna mais fácil o trabalho com conjuntos de dados muito grandes porque cada nó funciona processa apenas uma parte parte do volume total de dados.

![Spark paralell processing](/docs/spark_paralell.png)

#### Passos no processo de execuç!ao de Jobs em Paralelo
Suponha que você tenha escrito um programa em Python para calcular a média de uma coluna específica. 
O código Python é enviado para o SparkContext, que solicita ao gerenciador de cluster que execute o programa em 4 partições,
e o gerenciador de cluster solicita que os núcleos estejam prontos para processamento, pois o processamento será realizado
em um período de tempo específico. As partições serão executadas em paralelo.

As partições precisam de estruturas de dados para serem armazenadas na memória.
Algumas das estruturas de dados mais utilizadas são RDD, DataFrames, Datasets, etc.

As partições 1 e 3 serão executadas em paralelo.
Em seguida, as partições 2 e 4 serão executadas em paralelo.

Após a execução, a agregação é realizada nos nós de trabalho ou enviada de volta
ao nó driver para realizar a agregação de acordo com o código.

Observações:

- "SparkContext" é o contexto de aplicativo do Apache Spark.
- "Gerenciador de cluster" é o responsável por gerenciar os recursos do cluster.
- "Partições" são divisões do conjunto de dados para processamento paralelo.
- "RDD" (Resilient Distributed Datasets) é uma estrutura de dados distribuída e resiliente.
- "DataFrames" e "Datasets" são estruturas de dados do Apache Spark para processamento de dados estruturados.
- "Nó driver" é o nó que coordena a execução do aplicativo Spark.


### O Spark é amplamente utilizado em projetos analíticos nas seguintes frentes:

- *Preparação de dados*
- Modelos de machine learning
- Análise de dados em tempo real
