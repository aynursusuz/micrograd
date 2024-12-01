# Micrograd

This project is a neural network implementation inspired by Andrej Karpathy's ["Neural Networks: Zero to Hero"](https://www.youtube.com/watch?v=VMj-3S1tku0) video series. The main goal is to implement deep learning concepts from scratch in a clear and understandable way.

## Project Features

- Autograd engine for automatic differentiation
- Basic neural network components
- Visualization tools
- Computational graph creation
- Backpropagation implementation

## Quick Start

```bash
# Clone the repository
git clone https://github.com/yourusername/micrograd.git
cd micrograd

# Create virtual environment (Python 3.8+)
python -m venv venv
.\venv\Scripts\activate  # Windows
source venv/bin/activate # Linux/Mac

# Install dependencies
pip install -r requirements.txt
```

## Requirements

- Python 3.8+
- NumPy
- Matplotlib
- Graphviz (for visualization)
- Jupyter Notebook

## Usage Examples

### 1. Basic Mathematical Operations
```python
from engine import Value

# Create variables
a = Value(2.0)
b = Value(-3.0)
c = Value(10.0)

# Operations
d = a*b + c  # d = 2.0 * (-3.0) + 10.0 = 4.0
```

### 2. Automatic Differentiation
```python
# Backpropagation
d.backward()

# View gradients
print(f"d/da: {a.grad}")  # -3.0
print(f"d/db: {b.grad}")  # 2.0
print(f"d/dc: {c.grad}")  # 1.0
```

### 3. Computational Graph Visualization
```python
from utils import draw_dot

# Draw computational graph
draw_dot(d).render()
```

## Project Structure

```
micrograd/
├── notebooks/
│   └── 01_micrograd.ipynb  # Core examples and explanations
├── code/
│   ├── engine.py          # Autograd engine
│   └── utils.py           # Helper functions
└── requirements.txt
```

## Learning Resources

- [Neural Networks: Zero to Hero Video Series](https://www.youtube.com/watch?v=VMj-3S1tku0)
- [Automatic Differentiation Concepts](https://en.wikipedia.org/wiki/Automatic_differentiation)
- [Backpropagation Algorithm](https://en.wikipedia.org/wiki/Backpropagation)

## Contributing

We welcome your suggestions and pull requests to improve the project! You can contribute by adding new features, fixing bugs, or improving documentation.

## License

[MIT License](https://opensource.org/licenses/MIT) 2024

This project is open source and available under the MIT License.