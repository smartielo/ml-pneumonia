# 🫁 Detecção de Pneumonia em Raios-X com Deep Learning

## 📌 Sobre o Projeto

Este projeto aplica técnicas avançadas de **Visão Computacional** e **Deep Learning** para classificar radiografias de tórax (Raios-X), identificando automaticamente a presença de Pneumonia.

> **Motivação Pessoal:** A escolha deste tema vai além da tecnologia. Por já ter tido pneumonia no passado, conheço de perto o impacto da doença. Acredito que a Inteligência Artificial tem um potencial gigantesco para auxiliar médicos em diagnósticos mais rápidos e precisos, priorizando filas de atendimento e salvando vidas.

---

## 🗂️ O Dataset

Os dados utilizados são provenientes do famoso dataset **[Chest X-Ray Images (Pneumonia)](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia)**, disponível publicamente no Kaggle.

| Atributo | Detalhe |
|----------|---------|
| **Classes** | `NORMAL` (Pulmões Saudáveis) e `PNEUMONIA` (Pulmões com infecção) |
| **Formato** | Imagens JPEG em tons de cinza, de tamanhos variados |

---

## 🧠 Abordagem Técnica e Pipeline de Dados

Para garantir que o modelo aprenda os verdadeiros padrões da doença (e não apenas memorize as imagens), o projeto foi estruturado com as seguintes etapas:

### 1. 🔧 Pré-processamento
Redimensionamento padronizado de todas as imagens para `224x224` pixels e normalização das escalas de cor (0 a 1).

### 2. 🔄 Data Augmentation
Implementação de técnicas para evitar o **Overfitting** (Decoreba). O pipeline aplica pequenas rotações, distorções e zooms aleatórios nas imagens de treino, forçando a rede neural a generalizar o aprendizado de forma robusta.

### 3. 🤖 Transfer Learning *(Em breve)*
Utilização da arquitetura `MobileNetV2` pré-treinada para extração avançada de características radiológicas.

---

## 🚀 Como Executar o Projeto

### Pré-requisitos

Certifique-se de ter o **Python** instalado. É recomendado o uso de um ambiente virtual (`venv` ou `conda`).

**1. Clone este repositório:**
```bash
git clone https://github.com/smartielo/ml-pneumonia.git
cd ml-pneumonia
```

**2. Instale as dependências:**
```bash
pip install -r requirements.txt
```

**3.** Baixe o dataset no Kaggle e extraia a pasta `chest_xray` na raiz do projeto.

**4.** Execute o notebook `main.ipynb` no Jupyter ou DataSpell.

---

## 📊 Resultados e Métricas

> ⚙️ **Em Andamento** — Esta seção será atualizada com a Matriz de Confusão, Acurácia e Recall assim que o treinamento do modelo for concluído.

---

Desenvolvido com ☕ e dedicação por **Gabriel**.
Conecte-se comigo no **[LinkedIn](https://www.linkedin.com/in/gabrielmartielo)**!
