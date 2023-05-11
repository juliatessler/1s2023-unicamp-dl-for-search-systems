# Training a Language Model

This notebook has a [slide presentation](https://docs.google.com/presentation/d/1STiXvi7W1FjsSQhfh5S-f8Y23s76snPnUQxCgz96z44/edit?usp=sharing) as report.

---

## Assignment

Treinar um modelo de linguagem em dados em portugues

- Avaliar o modelo usando a perplexidade, que é simplesmente a exponencial de todas as losses do dataset de validação
- Iremos treinar o modelo para prever o próximo token dado os anteriores (também conhecido como Causal Language Modeling). Não confundir com o Masked Language Modeling (MLM), que consiste em prever tokens mascarados em uma dada sequência (ex: BERT's MLM)

Dicas:
- Usar como ponto de partida o modelo OPT-125M, que já foi treinado em 300B de tokens (maioria em Inglês)
- Usar este dataset reduzido do mc4 portugues, com ~300M de tokens: gs://unicamp-dl/ia025a_2022s1/aula9/sample-1gb.txt


