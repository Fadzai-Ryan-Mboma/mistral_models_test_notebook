# Mistral AI Models Test Notebook

A comprehensive Jupyter notebook for testing and comparing different Mistral AI models across text generation, reasoning, multimodal (vision), and embedding capabilities.

## 🚀 Overview

This notebook provides a systematic way to:
- **Test different Mistral AI models** across various categories (Text, Reasoning, Multimodal, Embeddings)
- **Compare performance and costs** between models
- **Get real-time pricing estimates** for API usage
- **Run practical examples** with ready-to-use code cells

## 📋 Features

### Model Categories Tested
- **Text Generation**: `mistral-large-latest`, `mistral-medium-latest`, `mistral-small-latest`, `mistral-tiny-2407`
- **Reasoning**: Complex mathematical and logical problem solving `mistral-large-latest`, `mistral-medium-latest`
- **Multimodal (Vision)**: Image understanding and analysis with `mistral-large-vision-2407`
- **Embeddings**: Semantic search and similarity analysis with `mistral-embed`

### Key Capabilities
- ✅ **Cost Analysis**: Real-time cost estimation per model and request
- ✅ **Performance Comparison**: Side-by-side model comparison
- ✅ **Pricing Snapshots**: Up-to-date pricing information (verify on official site)
- ✅ **Test Harness**: Utilities for easy model testing
- ✅ **Similarity Analysis**: Embedding-based semantic similarity
- ✅ **Vision Testing**: Image analysis capabilities

## 🛠️ Setup

### Prerequisites
- Python 3.8+
- Mistral AI API key
- Jupyter Notebook or JupyterLab

### Installation

1. **Clone the repository**:
   ```bash
   git clone <repository-url>
   cd mistral_models_test_notebook
   ```

2. **Create a virtual environment** (recommended):
   ```bash
   python -m venv .venv
   source .venv/bin/activate  # On Windows: .venv\Scripts\activate
   ```

3. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Set up your Mistral AI API key**:
   
   **Option A: Environment Variable**
   ```bash
   export MISTRAL_API_KEY="your_api_key_here"
   ```
   
   **Option B: .env File**
   ```bash
   echo "MISTRAL_API_KEY=your_api_key_here" > .env
   ```

5. **Start Jupyter**:
   ```bash
   jupyter notebook
   # or
   jupyter lab
   ```

6. **Open the notebook**: `mistral_models_test_v2.ipynb`

### Getting Your API Key
1. Visit [Mistral AI Platform](https://console.mistral.ai/)
2. Sign up or log in
3. Navigate to API Keys section
4. Generate a new API key

## 📊 Usage

### Quick Start
1. **Run the Setup cell** (Cell 3) to initialize the Mistral client
2. **Execute the Pricing snapshot** (Cell 5) to see current model pricing
3. **Run specific test sections** based on your needs:
   - **Text Models** (Cell 11): Basic text generation comparison
   - **Reasoning** (Cell 13): Complex problem-solving tests
   - **Vision** (Cell 15): Image analysis (requires sample image)
   - **Embeddings** (Cell 17): Semantic similarity testing

### Test Categories

#### 1. Text Generation Tests
Compare different models on the same prompt to evaluate:
- Response quality
- Token usage
- Cost efficiency

#### 2. Reasoning Tests
Test complex problem-solving with:
- Mathematical calculations
- Logical puzzles
- Multi-step reasoning

#### 3. Vision Tests
Analyze images with vision-capable models:
- Image description
- Object identification
- Compositional analysis

#### 4. Embedding Tests
Generate and compare text embeddings:
- Semantic similarity
- Vector comparisons
- Cosine similarity analysis

## 💰 Cost Estimation

The notebook includes built-in cost estimation functions that:
- Calculate input and output token costs
- Provide real-time pricing based on current rates
- Compare cost efficiency across models

> ⚠️ **Important**: Always verify current pricing at [mistral.ai/pricing](https://mistral.ai/pricing/) before production use.

## 📁 Project Structure

```
mistral_models_test_notebook/
├── README.md                          # This file
├── requirements.txt                   # Python dependencies
├── mistral_models_test_v2.ipynb      # Main notebook
├── .env.example                      # Example environment file
└── .gitignore                        # Git ignore rules
```

## 🔧 Dependencies

| Package | Version | Purpose |
|---------|---------|---------|
| `mistralai` | ≥1.0.2 | Official Mistral AI SDK |
| `pandas` | ≥1.5.3 | Data analysis and tables |
| `matplotlib` | ≥3.7.1 | Plotting and visualization |
| `python-dotenv` | ≥1.0.0 | Environment variable management |
| `numpy` | ≥1.24.3 | Numerical computations |
| `ipywidgets` | ≥8.0.6 | Interactive notebook widgets |

## 📈 Example Outputs

### Model Comparison
```
📝 Testing model: mistral-large-latest
--------------------------------------------------
Infrastructure as Code (IaC) in Kubernetes...

📊 Usage:
  Prompt tokens: 28
  Completion tokens: 95
  Total tokens: 123
  Estimated cost: $0.004560
```

### Similarity Analysis
```
📊 Similarity Matrix:
Text 1  Text 2  Text 3  Text 4  Text 5
  1.000   0.842   0.123   0.567   0.445
```

## 🚨 Important Notes

1. **API Costs**: This notebook makes real API calls which incur costs. Monitor your usage.
2. **Rate Limits**: Be aware of Mistral AI's rate limits for your plan.
3. **Pricing Updates**: Verify current pricing before production deployment.
4. **Data Privacy**: Be cautious with sensitive data in API requests.

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/new-feature`)
3. Make your changes
4. Commit your changes (`git commit -am 'Add new feature'`)
5. Push to the branch (`git push origin feature/new-feature`)
6. Create a Pull Request

## 📚 Resources

- [Mistral AI Documentation](https://docs.mistral.ai/)
- [Mistral AI API Reference](https://docs.mistral.ai/api/)
- [Mistral AI Pricing](https://mistral.ai/pricing/)
- [Python SDK Documentation](https://github.com/mistralai/client-python)

## ⚖️ License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🐛 Troubleshooting

### Common Issues

**Issue**: `MISTRAL_API_KEY environment variable not found`
**Solution**: Ensure your API key is properly set in environment variables or `.env` file.

**Issue**: `MistralAPIException: Unauthorized`
**Solution**: Verify your API key is valid and has sufficient credits.

**Issue**: Vision tests failing
**Solution**: Ensure you have a sample image file in the correct path or update the image path in the notebook.

**Issue**: Import errors
**Solution**: Make sure all dependencies are installed: `pip install -r requirements.txt`

## 📞 Support

For issues and questions:
1. Check the [Mistral AI Documentation](https://docs.mistral.ai/)
2. Review common troubleshooting steps above
3. Create an issue in this repository
4. Contact Mistral AI support for API-related issues

---

**Last Updated**: September 2025
**Compatible with**: Mistral AI SDK v1.0.2+