# Makemore Project

This is a character-level language model inspired by Andrej Karpathy's "makemore" series. The model learns to generate new words similar to the given example words.

## About the Project

This project includes:
- Character-based language model implementation
- Neural network implementation using PyTorch
- Bigram model for word generation
- Training process visualization

## Installation

1. Install required packages:
```bash
pip install torch numpy matplotlib jupyter
```

2. Clone the project:
```bash
git clone https://github.com/aynursusuz/micrograd.git
cd micrograd
```

## Usage

1. Start Jupyter Notebook:
```bash
jupyter notebook
```

2. Open `makemore.ipynb`
3. Run the cells in order

## Dataset

The project is trained using names in the `names.txt` file. This file contains one name per line.

## Model Details

- Input: Character sequences
- Output: Probability distribution of the next character
- Training: Gradient descent using cross-entropy loss
- Activation: Tanh and Softmax functions

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

## Contributing

1. Fork this repository
2. Create a new branch (`git checkout -b new-feature`)
3. Commit your changes (`git commit -am 'Added new feature'`)
4. Push to the branch (`git push origin new-feature`)
5. Create a Pull Request
