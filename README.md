# Práticas em Visão Computacional (IC009)

## Visão Geral
A Visão Computacional constitui um dos pilares da inteligência artificial contemporânea, sustentando aplicações nas áreas de reconhecimento de padrões, análise de cenas e interpretação automática de imagens. O desenvolvimento de algoritmos eficazes nessa área requer etapas eficientes de pré-processamento, conversão em representações discriminativas e modelos supervisionados capazes de explorar padrões estruturais e semânticos de dados visuais.

## Metodologia
As práticas desenvolvidas na disciplina **IC009 (Tópicos em Computação Visual I)**, documentadas neste repositório, seguem a metodologia estabelecida no *Manual de Práticas Laboratoriais em Visão Computacional* e estão organizadas em dois blocos principais de experimentos.

---

### 1. Processamento de Imagens e Extração de Características

Este primeiro bloco foca no tratamento inicial dos dados e na obtenção de descritores visuais.

* **Dataset:** O trabalho utiliza imagens do conjunto **Pascal VOC 2012**, composto por 20 classes.
* **Pré-processamento:**
    * Análise exploratória das imagens (experimento 2.1).
    * Aplicação de transformações fotométricas (RGB, HSV e LAB) (experimento 2.2).
    * Filtros espaciais: equalização de histograma, correção *gamma*, filtragem Gaussiana e operações de aguçamento (experimento 2.3).
    * Caracterização da distribuição da informação visual via histogramas (experimentos 2.2 e 2.3).

* **Extração de Características (Feature Extraction - experimento 2.4):**
    * Características de cor no espaço **HSV**.
    * Descritores de textura baseados em **Local Binary Patterns (LBP)**.
    * Descritores de forma baseados em gradientes, como o **Histogram of Oriented Gradients (HOG)**.

* **Redução de Dimensionalidade (experimento 2.4):**
    * Aplicação de **Principal Component Analysis (PCA)** para projetar os dados em subespaços de menor dimensão preservando a variância significativa. Esta etapa permite a inspeção visual da separabilidade entre classes.

---

### 2. Classificação e Detecção de Objetos

O segundo bloco concentra-se na aplicação de modelos de aprendizado de máquina para tarefas de visão.

* **Classificação Supervisionada:**
    * **Support Vector Machine (SVM) (experimento 3.1):** Utilizado devido à sua robustez em espaços de alta dimensionalidade.
    * **Multilayer Perceptron (MLP) (experimento 3.2):** Rede neural clássica aplicada para capturar relações não lineares em dados estruturados.

* **Detecção de Objetos (experimento 3.3):**
    * Experimentos com a família de detectores **YOLO**, reconhecida como uma das abordagens mais eficientes para detecção de objetos em tempo real.
