# digit-recognition-CNN
Custom model trained on EMNIST

it has two models one trained on MNIST and other on EMINST it is not very advanced but it has been hypertuned and back propogates with kernal 3x3 and stride and padding of 1 each and max pooled with 2 convolutional layers and fully connected layers 

## 📁 Contents

- `Copy of Untitled8.ipynb`: Training + Inference code
- `model.pth`: Trained model (state_dict)
- `full_model.pth`: Full model including architecture
- `train_model.py` *(optional)*: Script-based training (if included)

## 🚀 How to Run

### Option 1: Run the notebook

1. Open the notebook `Copy of Untitled8.ipynb`
2. Follow the cells to train and test your model

### Option 2: Load the Trained Model

```python
import torch
from model import Net  # or whatever class name used

model = Net()
model.load_state_dict(torch.load('model.pth'))
model.eval()
