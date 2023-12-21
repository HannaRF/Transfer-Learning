# Transfer Learning e Fine-Tuning com VGG16

**Objetivo:**
Este repositório do GitHub contém um jupyter notebook sobre transfer learning e fine-tuning baseado em um notebook oficial do TensorFlow. O tutorial tem como objetivo demonstrar a classificação de imagens de gatos e cães usando transfer learning a partir de uma rede pré-treinada VGG16.

**Principais Conceitos:**
- **Transfer Learning:**
  - Utiliza um modelo pré-treinado, previamente treinado em um grande conjunto de dados para tarefas de classificação de imagens.
  - O modelo pré-treinado pode ser usado como está ou personalizado para uma tarefa específica.

- **Intuição por trás do Transfer Learning para Classificação de Imagens:**
  - Um modelo treinado em um conjunto de dados grande e diversificado serve como um modelo visual genérico.
  - Aproveita mapas de características aprendidos sem começar do zero, evitando a necessidade de treinar um modelo grande em um conjunto de dados maciço.

**Duas Abordagens de Customização:**
1. **Extração de Características:**
   - Usa representações aprendidas por uma rede anterior para extrair características significativas de novas amostras.
   - Adiciona um novo classificador (treinado do zero) sobre o modelo VGG16 pré-treinado, reaproveitando mapas de características aprendidos anteriormente.

2. **Fine-Tuning:**
   - Descongela algumas das camadas superiores de um modelo VGG16 congelado.
   - Treina em conjunto as camadas recém-adicionadas do classificador e as últimas camadas do modelo base.
   - Ajusta finamente as representações de características de ordem superior no modelo base para torná-las mais relevantes para a tarefa de classificação específica.

**Rede Utilizada:**
- VGG16

Explore o notebook para obter insights sobre a implementação de técnicas de transfer learning e fine-tuning, aproveitando os recursos poderosos da arquitetura VGG16.
