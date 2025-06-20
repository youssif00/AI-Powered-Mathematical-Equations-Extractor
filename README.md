# AI-Powered Mathematical Equations Extractor

An AI project that automatically extracts mathematical equations from PDF documents using Facebook's OPT (Open Pre-trained Transformer) model.

## Overview

This project leverages Facebook's OPT model and the Hugging Face transformers library to identify and extract mathematical equations from PDF documents. The system utilizes advanced natural language processing techniques to accurately recognize and parse mathematical content.

## Features

- Automatic equation extraction from PDF documents
- Support for various mathematical notations
- Integration with Facebook's OPT model
- High accuracy in equation recognition
- PDF document processing
- Equation validation and formatting

## Technologies Used

- Facebook's OPT Model
- Hugging Face Transformers
- PyTorch & TorchVision
- PDFMiner & PDFPlumber
- Python

## Requirements

```bash
# PDF Processing
pdfplumber
pypdf
pdfminer.six

# Machine Learning
transformers
torch
torchvision

# Utilities
markdown
pathlib
```

## Installation

1. Clone the repository:
```bash
git clone https://github.com/youssif00/AI-Powered-Mathematical-Equations-Extractor.git
cd AI-Powered-Mathematical-Equations-Extractor
```

2. Install the required packages:
```bash
pip install pdfplumber
pip install pypdf
pip install markdown
pip install pdfminer.six
pip install transformers
pip install torch torchvision
```

## Usage

1. Open the Jupyter notebook provided in the repository
2. Import the required libraries:
```python
import pypdf
import re
from transformers import AutoTokenizer, AutoModelForCausalLM
import json
from pathlib import Path
import markdown
import pdfplumber
import os
import torch 
import torchvision
from datetime import datetime
from IPython.display import FileLink, display
from pdfminer.high_level import extract_text
```

3. Run the cells sequentially to:
   - Load PDF documents
   - Process documents using the OPT model
   - Extract mathematical equations
   - Format and validate results

## Model Details

The project utilizes:
- Facebook's OPT model for text understanding and equation recognition
- Hugging Face transformers for model implementation
- PyTorch and TorchVision for deep learning operations
- PDFMiner and PDFPlumber for PDF processing

## Input Support

The system currently supports:
- PDF documents
- Digital textbooks
- Scientific papers
- Academic documents

## Output Format

Extracted equations are provided in:
- LaTeX format
- Plain text
- Structured JSON format for further processing

## How It Works

1. PDF Document Processing
   - Document loading using PDFPlumber and PDFMiner
   - Text extraction and preprocessing
   - Content parsing

2. Equation Detection
   - OPT model-based text analysis
   - Mathematical content identification

3. Equation Extraction
   - Pattern recognition using regex
   - Context understanding
   - Mathematical symbol parsing

4. Post-processing
   - Equation validation
   - Format standardization
   - JSON output generation

## License

MIT License

## Contributors

- [youssif00](https://github.com/youssif00)

## Acknowledgments

- Facebook AI Research for the OPT model
- Hugging Face team
- PyTorch community
- PDFMiner and PDFPlumber developers
