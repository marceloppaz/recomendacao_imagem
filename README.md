# Sistema de Recomendacao por Imagem

![TensorFlow](https://img.shields.io/badge/TensorFlow-2.0%2B-orange) ![Python](https://img.shields.io/badge/Python-3.7%2B-blue) ![Colab](https://img.shields.io/badge/Google-Colab-yellow)

## 📌 Descricao do Projeto

Este projeto implementa um sistema de recomendacao baseado em imagens, utilizando redes neurais convolucionais (CNNs). Ele permite encontrar imagens similares a uma imagem de consulta dentro de um dataset. O modelo utiliza redes pre-treinadas como ResNet50 e VGG16 para extracao de caracteristicas e comparacao de similaridade usando cosseno.

## 📁 Estrutura do Projeto

```
📂 Sistema_Recomendacao_Imagem/
│── 📜 notebook.ipynb       # Codigo principal do projeto (Colab)
│── 📜 requirements.txt      # Dependencias do projeto
│── 📂 dataset/              # Diretorio com imagens para treinamento
│── 📂 validation/           # Diretorio com imagens para validacao
│── 📂 results/              # Diretorio com resultados de recomendacao
```

## 🚀 Tecnologias Utilizadas

- Python 3.7+
- TensorFlow/Keras
- ResNet50 e VGG16 (Modelos Pre-Treinados)
- ImageDataGenerator (Pre-processamento de Imagens)
- Matplotlib (Visualizacao de Resultados)
- Sklearn (Metricas de Similaridade)
- Google Colab (Execucao do Projeto)

## 🔧 Instalacao e Uso

### 1️⃣ Clonar o Repositorio
```bash
git clone https://github.com/seu_usuario/sistema_recomendacao_imagem.git
cd sistema_recomendacao_imagem
```

### 2️⃣ Instalar Dependencias
```bash
pip install -r requirements.txt
```

### 3️⃣ Executar no Google Colab
Carregue o arquivo `notebook.ipynb` no Google Colab e execute as celulas.

### 4️⃣ Estrutura dos Dados
As imagens de treino e validacao devem ser organizadas da seguinte forma:
```
📂 dataset/
  ├── 📂 classe_1/
  │    ├── imagem1.jpg
  │    ├── imagem2.jpg
  │
  ├── 📂 classe_2/
  │    ├── imagem3.jpg
  │    ├── imagem4.jpg
```

## 🖼️ Exemplo de Uso

Para encontrar as imagens mais similares a uma imagem de consulta:
```python
query_image_path = "relogio.jpg"  # Caminho da imagem de consulta
similar_images = find_similar_images(query_image_path, model, features, image_paths, top_n=5)
plot_images(similar_images, query_image_path)
```

## 📊 Resultados

O sistema utiliza similaridade de cosseno para recomendar imagens visualmente similares.

---
💡 **Dica:** Se gostou deste projeto, nao se esqueca de dar uma estrela ⭐ no GitHub!
