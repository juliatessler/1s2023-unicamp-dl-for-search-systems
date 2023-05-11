# Dense Passage Retrieval

This notebook has a [slide presentation](https://docs.google.com/presentation/d/1ZeByAI-s5bChkwCAi16j7DUuthuKbT_qpVRWROji1_0/edit?usp=sharing) as report.
I wasn't able to complete the assignment.

---

## Assignment

Fazer o finetuning de um buscador denso

Usar como treino o dataset "tiny" do MS MARCO
https://storage.googleapis.com/unicamp-dl/ia368dd_2023s1/msmarco/msmarco_triples.train.tiny.tsv

Avaliar o modelo no TREC-COVID, e comparar os resultados com o BM25 e doc2query

Comparar busca "exaustiva" (semelhança do vetor query com todos os vetores do corpus) com a busca aproximada (Approximate Nearest Neighbor - ANN)

Para a busca aproximada, usar os algoritmos existentes na biblioteca sentence-transformers (ex: hnswlib) OU implemente um você mesmo (Bonus!)

Dicas:
- Usar a média dos vetores da última camada (conhecido como mean pooling) do transformer para representar queries e passagens; Alternativamente, usar apenas o vetor do [CLS] da última cada.
- Tente inicialmente uma loss fácil de implementar, como a entropia-cruzada
- Começar o treino a partir do microsoft/MiniLM-L12-H384-uncased
- Avaliar o pipeline usando um modelo já bem treinado: sentence-transformers/all-mpnet-base-v2
- Comparar resultados usando semelhança de cosseno e produto escalar como funções de similaridade
- Para checar se seu codigo de avaliação está correto, comparar o seu desempenho com o do modelo já treinado no MS MARCO:   https://huggingface.co/sentence-transformers/all-MiniLM-L12-v2; O nDCG@10 no TREC-COVID deve ser ~0.47
- Usar a biblioteca do sentence-transformers para avaliar o modelo
