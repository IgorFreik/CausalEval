# CausalEval: Causal Inference Framework Evaluation Suite

CausalEval is a comprehensive evaluation framework designed to benchmark and compare different causal inference and machine learning frameworks. This tool provides a standardized way to assess the performance, reliability, and robustness of various causal inference methods across different scenarios.

## Features

- **Standardized Evaluation Metrics**: Compare frameworks using consistent metrics
- **Multiple Datasets**: Support for synthetic and real-world datasets
- **Framework Agnostic**: Works with various causal inference libraries
- **Reproducible Experiments**: Detailed logging and configuration management
- **Visualization Tools**: Generate comparative analysis plots and reports

## Supported Frameworks

- DoWhy
- CausalML
- EconML
- PyMC

## Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/CausalEval.git
cd CausalEval

# Install dependencies
pip install -r requirements.txt
```

## Quick Start

```python
from causaleval import Evaluator
from causaleval.datasets import SyntheticDataset

# Initialize evaluator
evaluator = Evaluator()

# Load dataset
dataset = SyntheticDataset()

# Run evaluation
results = evaluator.evaluate(
    dataset=dataset,
    frameworks=['dowhy', 'causalml'],
    metrics=['ate', 'cate', 'confidence_intervals']
)

# Generate report
evaluator.generate_report(results)
```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Citation

If you use CausalEval in your research, please cite:

```bibtex
@software{causaleval2024,
  author = {Igor Freik},
  title = {CausalEval: Causal Inference Framework Evaluation Suite},
  year = {2024},
  publisher = {GitHub},
  url = {https://github.com/IgorFreik/CausalEval}
}
```
