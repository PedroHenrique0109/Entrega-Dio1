# Entrega-Dio1


📘 Miniguia de Machine Learning com NotebookLM

Autor: Pedro Henrique Alves dos Santos
Curso: Análise e Desenvolvimento de Sistemas
Projeto: Desafio DIO — Caderno Temático com Inteligência Artificial

🎯 Contexto e objetivos

Este projeto foi desenvolvido com o objetivo de organizar um caderno temático de estudos sobre Machine Learning, utilizando o NotebookLM como apoio para consulta, revisão e organização do conhecimento.

O tema foi escolhido por ter relação direta com minha formação em Análise e Desenvolvimento de Sistemas e com conteúdos importantes da área de Inteligência Artificial.

Os principais objetivos de estudo foram:

compreender a diferença entre aprendizado supervisionado e não supervisionado;

revisar conceitos de classificação;

entender algoritmos como Regressão Logística e Random Forest;

compreender métricas como Accuracy, Precision, Recall, F1 Score e AUC;

revisar validação cruzada e pré-processamento de dados;

criar um material curto que possa ser reutilizado em revisões futuras.

🔎 Curadoria de fontes

Foram selecionadas fontes abertas e confiáveis para servir de base ao estudo:

Google — Machine Learning Crash Course
https://developers.google.com/machine-learning/crash-course

Scikit-learn — User Guide
https://scikit-learn.org/stable/user_guide.html

Orange Data Mining — Test & Score
https://orangedatamining.com/widget-catalog/evaluate/testandscore/

Orange Data Mining — Preprocess
https://orangedatamining.com/widget-catalog/transform/preprocess/

As fontes cobrem fundamentos de Machine Learning, pré-processamento, classificação, validação cruzada e avaliação de modelos.

💬 Engenharia de prompts

Durante a organização do estudo, foram elaborados prompts com objetivos diferentes: explicar conceitos, comparar algoritmos, revisar métricas e gerar perguntas para estudo.

Prompt 1

Explique a diferença entre aprendizado supervisionado e não supervisionado de forma simples e dê um exemplo de cada.

Resposta consolidada:
No aprendizado supervisionado, o modelo utiliza dados que já possuem uma resposta conhecida e aprende a relacionar as entradas com essa resposta. Um exemplo é prever se um cliente irá cancelar um serviço. Já no aprendizado não supervisionado, os dados não possuem rótulos definidos e o objetivo é encontrar padrões ou agrupamentos, como separar clientes por comportamento de consumo.

Prompt 2

Compare Regressão Logística e Random Forest em um problema de classificação. Explique as principais diferenças de forma simples.

Resposta consolidada:
A Regressão Logística é um modelo de classificação que calcula probabilidades e costuma ser mais simples de interpretar. O Random Forest combina várias árvores de decisão e consegue representar relações mais complexas entre as variáveis. A escolha entre os dois depende dos dados e deve ser feita com base na avaliação das métricas do modelo.

Prompt 3

Explique Accuracy, Precision, Recall, F1 Score e AUC como se eu fosse um estudante iniciante.

Resposta consolidada:

Accuracy: porcentagem total de previsões corretas.

Precision: entre os casos previstos como positivos, quantos realmente eram positivos.

Recall: entre todos os casos positivos reais, quantos foram identificados.

F1 Score: combina Precision e Recall em uma única métrica.

AUC: representa a capacidade do modelo de diferenciar as classes.

Prompt 4

Por que a validação cruzada é importante na avaliação de um modelo de Machine Learning?

Resposta consolidada:
A validação cruzada divide os dados em diferentes partes e alterna os conjuntos usados para treinamento e teste. Isso ajuda a avaliar se o modelo consegue generalizar para dados que não foram utilizados diretamente no treinamento e reduz o risco de tirar conclusões com base em uma única divisão dos dados.

Prompt 5

Crie cinco perguntas rápidas para revisar classificação e avaliação de modelos de Machine Learning.

Perguntas geradas para revisão:

Qual é a diferença entre classificação e regressão?

O que significa uma variável-alvo em aprendizado supervisionado?

Qual é a diferença entre Precision e Recall?

Por que a validação cruzada pode ser melhor do que uma única divisão treino/teste?

O que a AUC indica sobre um classificador?

🩹 Cicatrizes e troubleshooting

Durante a construção dos prompts, foi possível perceber que perguntas muito amplas produzem respostas igualmente amplas.

Tentativa pouco eficiente

Explique Machine Learning.

Esse tipo de pergunta é genérico e pode misturar muitos assuntos em uma única resposta.

Prompt melhorado

Explique aprendizado supervisionado, classificação e validação cruzada separadamente, usando um exemplo simples em cada conceito.

Ao informar claramente o conteúdo, a forma da resposta e o nível de dificuldade esperado, a explicação fica mais organizada e útil para estudo.

Outra dificuldade percebida é que algumas métricas podem parecer semelhantes no começo. Por isso, prompts de comparação foram mais úteis do que pedir apenas a definição isolada de cada termo.

Aprendizado: bons prompts normalmente possuem contexto, objetivo e formato esperado.

📚 Miniguia de estudo

1. O que é Machine Learning?

Machine Learning é uma área da Inteligência Artificial que utiliza dados para identificar padrões e produzir previsões ou decisões sem depender apenas de regras fixas programadas manualmente.

2. Aprendizado supervisionado

No aprendizado supervisionado, o conjunto de treinamento possui exemplos com respostas conhecidas.

Exemplo:

Dados do cliente → modelo → Cancela / Não cancela

Esse tipo de aprendizado é muito utilizado em problemas de classificação e regressão.

3. Aprendizado não supervisionado

No aprendizado não supervisionado não existe uma variável-alvo conhecida. O algoritmo procura estruturas nos próprios dados.

Um exemplo é usar técnicas de agrupamento para encontrar grupos de clientes com comportamentos semelhantes.

4. Classificação

Classificação é utilizada quando o resultado esperado pertence a uma categoria.

Exemplos:

fraude ou não fraude;

spam ou não spam;

cliente cancela ou não cancela;

imagem pertence à classe A ou B.

5. Regressão Logística

Apesar do nome, a Regressão Logística é muito utilizada em classificação. Ela estima a probabilidade de um exemplo pertencer a determinada classe.

Por ser relativamente simples, também permite interpretar melhor a influência das variáveis em muitos cenários.

6. Random Forest

Random Forest é um algoritmo que utiliza diversas árvores de decisão.

Cada árvore produz uma previsão e o conjunto dessas árvores é usado para determinar o resultado final. O método consegue representar relações mais complexas entre as características dos dados.

7. Pré-processamento

Antes de treinar um modelo, pode ser necessário preparar os dados.

Algumas etapas comuns são:

tratamento de valores ausentes;

remoção ou análise de outliers;

normalização;

transformação de variáveis categóricas;

seleção de características.

Um bom pré-processamento pode melhorar a qualidade da análise e evitar problemas durante o treinamento.

8. Validação cruzada

Na validação cruzada, os dados são divididos em várias partes.

Em uma validação com 10 partes, por exemplo, o modelo é treinado em nove partes e testado na parte restante. Esse processo é repetido até que todas as partes tenham sido utilizadas para teste.

Isso fornece uma avaliação mais confiável do desempenho do modelo.

9. Principais métricas

Métrica

Significado

Accuracy

Percentual total de previsões corretas

Precision

Qualidade das previsões classificadas como positivas

Recall

Capacidade de encontrar os casos positivos reais

F1 Score

Equilíbrio entre Precision e Recall

AUC

Capacidade do modelo de separar as classes

Uma única métrica nem sempre é suficiente. A escolha das métricas deve considerar o objetivo do problema.

🧠 Glossário

Termo

Definição

Dataset

Conjunto de dados utilizado em uma análise

Feature

Característica usada como entrada pelo modelo

Target

Variável que o modelo deve prever

Classificação

Previsão de uma categoria

Regressão

Previsão de um valor numérico

Treinamento

Processo em que o modelo aprende padrões dos dados

Teste

Etapa usada para avaliar as previsões do modelo

Outlier

Registro com comportamento muito diferente dos demais

Normalização

Transformação da escala das variáveis

Cross-validation

Técnica de validação que utiliza várias divisões dos dados

Accuracy

Proporção total de acertos

Precision

Precisão dos casos previstos como positivos

Recall

Proporção dos positivos reais encontrados

F1 Score

Combinação de Precision e Recall

AUC

Medida da capacidade de separação das classes

🔁 Prompts reutilizáveis

Explique [conceito] de forma simples e apresente um exemplo prático.

Compare [conceito A] e [conceito B] em uma tabela.

Crie 10 perguntas de múltipla escolha sobre os conteúdos das fontes.

Crie flashcards com os conceitos mais importantes das fontes.

Explique os erros mais comuns de iniciantes ao estudar [assunto].

Resuma as fontes em tópicos e destaque apenas o conteúdo essencial para uma prova.

Crie um exercício prático sobre [assunto] e depois forneça o gabarito comentado.

Faça uma revisão de [assunto] em três níveis: iniciante, intermediário e avançado.

✅ Conclusão

A organização deste caderno mostrou como ferramentas de Inteligência Artificial podem apoiar o aprendizado de forma ativa.

Além de reunir fontes confiáveis, o processo de criar, testar e melhorar prompts ajudou a transformar conteúdos amplos em explicações mais direcionadas.

O resultado final é um miniguia de Machine Learning que pode ser utilizado como material de revisão durante meus estudos em Análise e Desenvolvimento de Sistemas.

👨‍💻 Autor

Pedro Henrique Alves dos Santos
Estudante de Análise e Desenvolvimento de Sistemas
