# transfer-learning-caes_e_gatos

## Descrição
Aplicação de Transfer Learning e Fine-Tuning usando o modelo pré-treinado VGG16 sobre o dataset Cats vs Dogs (gatos vs cachorros) com TensorFlow/Keras no Google Colab. Suporta troca para duas classes customizadas organizadas em pastas.

## Estrutura
- `notebook.ipynb`: notebook Colab principal com todo o pipeline (feature extraction + fine-tuning).  
- `requirements.txt`: dependências (para execução local).  
- `models/`: modelos treinados salvos.  
- `utils/helpers.py`: funções auxiliares (opcional).  
- `data/custom/`: local para conter suas próprias imagens (duas classes), com subpastas `train` e `val`.

## Dataset padrão
Usamos `cats_vs_dogs` via `tensorflow_datasets`, com divisão 80/10/10 (treino/validação/teste). Não é necessário versionar imagens grandes.

## Como rodar (no Colab)
1. Abra o notebook: `notebook.ipynb` no Google Colab.  
2. Execute as células em ordem:  
   - Carregamento do dataset.  
   - Pré-processamento.  
   - Transfer Learning (feature extraction).  
   - Fine-tuning parcial.  
   - Avaliação e inferência.  
3. Salve o modelo treinado em `models/`.

## Como customizar com suas próprias classes
Organize suas imagens assim:

data/custom/train/classeA/
data/custom/train/classeB/
data/custom/val/classeA/
data/custom/val/classeB/



