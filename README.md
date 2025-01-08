# DeepLearning_RBF-Neural_Network

## Introdução

Este repositório contém um notebook que explora de forma detalhada o processo de **criação, treinamento, avaliação e visualização** de uma **Rede Neural de Base Radial (RBFN)** utilizando o conjunto de dados **make_moons**. **O notebook inclui todas as etapas, desde a geração dos dados até a avaliação do modelo,** com explicações claras e estruturadas após cada célula de código correspondente. Abaixo, você encontrará apenas uma visão geral das principais etapas, apresentada de maneira resumida:

## Imports

Os pacotes e bibliotecas necessários são importados, incluindo **sklearn** (com o **KMeans**), **matplotlib** para visualização, e outras bibliotecas essenciais para o pré-processamento e divisão dos dados.

## 1. Função Gaussiana (RBF)

A função de ativação RBF utiliza a função Gaussiana para calcular a ativação dos neurônios, determinando a influência de cada neurônio em relação aos dados de entrada.

## 2. Classe RBFNetwork

A classe **RBFNetwork** encapsula a lógica da rede de base radial. A função **fit** ajusta os centros dos neurônios utilizando **KMeans**, enquanto a função **predict** gera as previsões com base nos dados de entrada. O uso de **KMeans** permite a determinação eficiente dos centros.

## 3. Geração de Dados com make_moons (Ruído Controlado)

A função **make_moons** cria um conjunto de dados com separação não-linear, desafiando a classificação e simulando problemas do mundo real, com ruído controlado.

### `3.1 Divisão entre Treino e Teste (80% Treino, 20% Teste):`
A divisão dos dados em treino e teste organiza os conjuntos para treinamento e avaliação, utilizando **random_state** para garantir reprodutibilidade.

### `3.2 Escalonamento dos Dados (Normalização):`
A normalização com **StandardScaler** ajusta a escala dos dados, melhorando a performance do modelo e evitando problemas relacionados a diferentes escalas nas features.

## 4. Instanciar e Treinar a Rede RBF

A rede RBF é instanciada com 10 centros e sigma 1.0, e treinada nos dados de treino, ajustando os pesos para minimizar o erro nas previsões.

## 5. Predições

As predições são transformadas em classes binárias (0 ou 1), facilitando a avaliação do desempenho do modelo em tarefas de classificação.

## 6. Cálculo da Acurácia

A **acurácia** é calculada para medir o desempenho do modelo no conjunto de teste, fornecendo uma avaliação quantitativa da sua precisão.

## 7. Visualização

Gráficos são gerados para visualizar os dados de treino, teste e os centros RBF, ajudando na interpretação do comportamento da rede.

### `7.1 Plotar Dados de Treino e Centros RBF`
A visualização dos dados e centros RBF proporciona uma compreensão visual de como a rede está se comportando.

## Conclusão

Este repositório apresenta uma implementação detalhada de uma **rede neural de base radial (RBF)**, aplicada ao conjunto de dados **make_moons**. O foco principal do projeto foi a criação, treinamento e avaliação do modelo, abordando etapas como a geração de dados, divisão entre treino e teste, normalização, treinamento da rede e cálculo de acurácia. Além disso, gráficos de visualização foram gerados para proporcionar uma compreensão mais clara sobre o comportamento da rede e a distribuição dos dados e centros RBF.

***Para uma explicação mais detalhada e um entendimento completo sobre a implementação da rede RBF, consulte o código no notebook, onde cada etapa é explicada de forma clara e estruturada.***

## Autor

**Lucas Benício Gusmão da Silva**

Idealizador, criador e desenvolvedor deste projeto.

``Todos os Direitos Reservados``
