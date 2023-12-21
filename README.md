# Transfer Learning e Fine-Tuning com VGG16

<p align="center">
  <img src="https://github.com/HannaRF/Transfer-Learning/assets/85463854/229a6434-f112-4902-b606-857894c64a1e" />
</p>


**Descrição:**
O projeto tem como objetivo implementar e avaliar o desempenho de um modelo VGG16 utilizado como "backbone" em três cenários distintos:

1. **Treinamento do Zero:**
   - Utiliza o VGG16 sem treinamento prévio.
   - Remove a última camada e adiciona um novo classificador.
   - Treina o modelo do zero e avalia seu desempenho.

2. **Usando uma Rede Pré-treinada como Extrator de Características:**
   - Utiliza o mesmo modelo do Experimento 1, mas com o VGG16 pré-treinado no ImageNet.
   - Congela todas as camadas do VGG16, treina e avalia o modelo.

3. **Ajuste Fino das Últimas Camadas:**
   - Utiliza um VGG16 pré-treinado.
   - Descongela os últimos blocos de convolução de acordo com opções específicas.
     - 3-a) Descongela os últimos blocos a partir de "block5_conv1", treina e avalia o modelo.
     - 3-b) Descongela os últimos blocos a partir de "block4_conv1", treina e avalia o modelo.
     - 3-c) Descongela todos os blocos de convolução, treina e avalia o modelo.

**Conjunto de Dados:**
Conjunto de dados Beans: imagens de feijões no campo, capturadas por smartphones, com 3 classes (2 de doenças e 1 saudável). As imagens são redimensionadas para 224x224.

- URL de Treinamento: ['https://storage.googleapis.com/ibeans/train.zip'](https://storage.googleapis.com/ibeans/train.zip)
- URL de Validação: ['https://storage.googleapis.com/ibeans/validation.zip'](https://storage.googleapis.com/ibeans/validation.zip)
- URL de Teste: ['https://storage.googleapis.com/ibeans/test.zip'](https://storage.googleapis.com/ibeans/test.zip)
