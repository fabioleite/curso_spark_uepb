# Resilient Distributed Dataset 
"Conjunto de dados distribuídos resilientes" em português, também chamado pela sigla RDD;
o DataFrame e o Dataset.

A **abstração principal** que o Spark fornece é justamente o RDD, 
que consiste em uma coleção de elementos particionados nos nós do cluster que podem ser 
operados em paralelo. O RDD é a API do Spark de nível mais baixo e há várias formas de criá-lo.
Está disponível nas linguagens Java, Python e Scala, então conseguimos utilizá-lo com o PySpark. Embora seja a estrutura original de dados do Spark,
não entraremos em mais detalhes sobre esta API porque nosso foco é o DataFrame.

O **DataFrame** é um conceito similar ao dataframe do Pandas e da linguagem R, estando disponível nas linguagens Java, 
Python, R e Scala.

O **Dataset**, por sua vez, é uma interface mais recente que fornece os benefícios do RDD
em conjunto com os do DataFrame. Em suma, trata-se de uma combinação das duas interfaces
anteriores e está disponível apenas nas linguagens Java e Scala