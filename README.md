# Edge AI Recyclable Item Classification

![Recycling Concept](https://example.com/recycling-image.jpg) *(Replace with actual image)*

## Project Overview
This project implements an Edge AI solution for classifying recyclable items using TensorFlow Lite. The system is designed to run efficiently on resource-constrained devices like Raspberry Pi, enabling real-time waste classification at the edge.

## Key Features
- Lightweight CNN model optimized for edge deployment
- TensorFlow Lite conversion with quantization
- Real-time classification capabilities
- Small model footprint (~65KB quantized)
- Validation accuracy of 85-90%

## Dataset
The model is trained on a modified version of the [TrashNet dataset](https://github.com/garythung/trashnet) containing images of:
- Cardboard
- Glass
- Metal
- Paper
- Plastic
- General trash

## Technical Specifications
| Component            | Specification                          |
|----------------------|----------------------------------------|
| Framework            | TensorFlow 2.x / TensorFlow Lite      |
| Model Architecture   | Lightweight CNN (3 Conv layers)        |
| Input Resolution     | 128x128 RGB                           |
| Quantization         | Full integer quantization              |
| Inference Time (RPi) | 50-100ms per image                    |

## Installation

### Prerequisites
- Python 3.7+
- TensorFlow 2.x
- TensorFlow Lite Runtime (for deployment)
- Raspberry Pi (optional for edge deployment)

### Setup
```bash
# Clone repository
git clone https://github.com/yourusername/edge-ai-recycling.git
cd edge-ai-recycling

# Install dependencies
pip install -r requirements.txt

# Download dataset (automatically done in the notebook)# edgeAI.prototype
