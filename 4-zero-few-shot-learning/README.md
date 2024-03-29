# Zero and Few-Shot Learning

This notebook has a [slide presentation](https://docs.google.com/presentation/d/1BXswNlocqnW7_SfQ4sIvJlNQHrMUfQbJaNweJrPrT-w/edit?usp=sharing) as report.

---

## Assignment

O aluno irá escolher uma tarefa para resolver de maneira zero ou few-shot. Sugestões:

- Classificação de textos (ex: análise de sentimos (IMDB))

- Predizer se uma passagem/parágrafo é relevante para uma pergunta/query

- Se uma resposta predita por um sistema de QA ou sumarizador é semanticamente igual à resposta ground-truth


É importante ter uma função de avaliação da qualidade das respostas do modelo few-shot. Por exemplo, acurácia.


É possível criar um pequeno dataset de teste manualmente (ex: com 10 à 100 exemplos)


- Usar a API do LLAMA fornecida por nós (licença exclusiva para pesquisa). Colab demo da API do LLAMA (obrigado, Thales Rogério)

- Opcionalmente, usar a API do code-davinci-002, que é de graça e trás resultados muito bons.

CUIDADO: NÃO USAR O TEXT-DAVINCI-002/003, que é pago

- Opcionalmente, usar a API do ChatGPT (gpt-3.5-turbo) que é barata: ~1 centavo de real por 1000 tokens (uma página)

- Opcionalmente, usar o Alpaca: https://alpaca-ai.ngrok.io/


Dicas:

- Teste com zero-shot E few-shot.
- No few-shot, faça testes com e sem instruções no cabeçalho (explicação da tarefa, ex: "Traduza de Ingles para Portugues"). Pode ser que sem a instrução o modelo até funcione melhor.
- Siga sempre um padrão ao criar os exemplos few-shot. Aqui tem uma pagina com dicas para prompt engineering: https://help.openai.com/en/articles/6654000-best-practices-for-prompt-engineering-with-openai-api
