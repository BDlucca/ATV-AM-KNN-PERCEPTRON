# AT1: Perceptron e KNN em Prática

Este repositório contém a resolução da **Atividade Avaliativa 1 (AT1)** da disciplina de **Aprendizagem de Máquina**. O objetivo principal é implementar, calibrar e aplicar algoritmos clássicos de Machine Learning utilizando exclusivamente **operações vetorizadas com a biblioteca NumPy**.

---

##  Sumário
- [Visão Geral dos Desafios](#-visão-geral-dos-desafios)
- [ Pré-requisitos e Tecnologias](#️-pré-requisitos-e-tecnologias)
- [ Como Executar](#-como-executar)

---

##  Visão Geral dos Desafios

### Desafio 1: Classificação Binária com Perceptron Treinável
- **Contexto:** Triagem preliminar de risco de fraude em transações financeiras.
- **Entradas ($X$):** Valor da Transação Normalizado ($x_1$) e Frequência de Operações Recentes ($x_2$).
- **Classes ($y$):** `0` (Transação Legítima) | `1` (Transação Suspeita/Fraude).
- **Abordagem:** Implementação do Perceptron de Rosenblatt com inicialização de pesos/viés em $1.0$ e ajuste iterativo por taxa de aprendizado ($\eta = 0.1$).

### Desafio 2: Predição de Risco de Churn com Classificador KNN
- **Contexto:** Antecipação de cancelamento de clientes corporativos (SaaS).
- **Entradas ($X$):** Dias de Inatividade ($x_1$) e Chamados Críticos em Aberto ($x_2$).
- **Classes ($y$):** `0` (Baixo Risco) | `1` (Alto Risco).
- **Abordagem:** Classificador $K$-Nearest Neighbors vetorizado, suportando as métricas de distância **Euclidiana** e **Manhattan** com apuração de classe por maioria de votos.

### Desafio 3: Recomendação de Servidores Cloud por Similaridade Espacial
- **Contexto:** Ferramenta de dimensionamento automático (*sizing*) de instâncias virtuais.
- **Entradas ($X$):** Espaço tridimensional contendo vCPUs ($x_1$), RAM em GB ($x_2$) e Armazenamento NVMe em GB ($x_3$).
- **Abordagem:** Cálculo de similaridade geométrica via distância Euclidiana em 3D para gerar um *ranking* das $K$ instâncias mais adequadas ao perfil demandado.

---

##  Pré-requisitos e Tecnologias

Apenas Python e NumPy são necessários para rodar todas as implementações:

* **Python** >= 3.8
* **NumPy** >= 1.20.0
* **Jupyter Notebook** / **Jupyter Lab** / **VS Code** (extensão Jupyter)

Para instalar as dependencias:
```bash
uv pip install numpy matplotlib jupyter ipykernel
