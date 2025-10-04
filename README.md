# BlueRoots 🌱

[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://python.org)
[![Streamlit](https://img.shields.io/badge/Streamlit-1.28%2B-FF4B4B.svg)](https://streamlit.io)

An AI-powered satellite imagery analysis system for monitoring UAE mangrove ecosystem health. This project leverages machine learning and remote sensing to provide real-time insights into mangrove forest conditions, supporting conservation efforts and environmental monitoring.

## 🌟 Features

- **Satellite Imagery Analysis**: Process and analyze high-resolution satellite imagery of UAE mangrove areas
- **AI-Powered Health Assessment**: Machine learning models to evaluate mangrove health indicators
- **Interactive Dashboard**: Real-time visualization of mangrove health metrics and trends
- **Automated Monitoring**: Continuous tracking of environmental changes and alerts
- **Data Export**: Export analysis results for research and reporting purposes

## 🚀 Quick Start

### Prerequisites

- Python 3.8 or higher
- pip package manager
- Git

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/Blue-Roots/blue_roots.git
   cd blue_roots
   ```

2. **Create a virtual environment**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Set up environment variables**
   ```bash
   cp .env.example .env
   # Edit .env with your API keys and configuration
   ```

5. **Run the dashboard**
   ```bash
   streamlit run dashboard/app.py
   ```

## 📁 Project Structure

```
blue_roots/
├── 📊 dashboard/          # Streamlit web application
│   ├── app.py            # Main dashboard application
│   ├── components/       # UI components
│   └── utils/           # Dashboard utilities
├── 📁 data/              # Data storage and samples
│   ├── raw/             # Raw satellite imagery
│   ├── processed/       # Processed datasets
│   └── samples/         # Sample data for testing
├── 📚 docs/              # Documentation and reports
│   ├── api/             # API documentation
│   ├── reports/         # Analysis reports
│   └── presentations/   # Project presentations
├── 🤖 models/            # Machine learning models
│   ├── trained/         # Pre-trained model weights
│   ├── architectures/   # Model definitions
│   └── evaluation/      # Model evaluation scripts
├── 🛠️ scripts/           # Utility and processing scripts
│   ├── data_processing/ # Data preprocessing utilities
│   ├── model_training/  # Training scripts
│   └── deployment/      # Deployment utilities
├── 📋 requirements.txt   # Python dependencies
├── 📄 LICENSE           # Project license
└── 📖 README.md         # This file
```

## 🛠️ Usage

### Data Processing

```bash
# Process raw satellite imagery
python scripts/data_processing/preprocess_imagery.py --input data/raw --output data/processed

# Extract features for ML models
python scripts/data_processing/extract_features.py --data data/processed
```

### Model Training

```bash
# Train mangrove health classification model
python scripts/model_training/train_classifier.py --config configs/classifier_config.yaml

# Train change detection model
python scripts/model_training/train_change_detection.py --config configs/change_detection_config.yaml
```

### Dashboard

Access the interactive dashboard at `http://localhost:8501` after running:

```bash
streamlit run dashboard/app.py
```

## 🔧 Configuration

### Environment Variables

Create a `.env` file in the root directory with the following variables:

```env
# Satellite Data APIs
SENTINEL_API_KEY=your_sentinel_api_key
LANDSAT_API_KEY=your_landsat_api_key

# Database Configuration
DATABASE_URL=your_database_url

# Model Configuration
MODEL_PATH=models/trained/
BATCH_SIZE=32
LEARNING_RATE=0.001

# Dashboard Configuration
DASHBOARD_HOST=localhost
DASHBOARD_PORT=8501
```

## 📊 Data Sources

- **Sentinel-2**: High-resolution multispectral imagery
- **Landsat 8/9**: Long-term historical data
- **UAE Environmental Data**: Ground truth and validation data
- **Climate Data**: Temperature, precipitation, and tide information

## 🤖 Models

### Mangrove Health Classifier
- **Architecture**: ResNet-50 based CNN
- **Input**: Multispectral satellite imagery (RGB + NIR bands)
- **Output**: Health classification (Healthy, Stressed, Degraded)
- **Accuracy**: 92.5% on validation set

### Change Detection Model
- **Architecture**: U-Net with attention mechanism
- **Input**: Temporal image pairs
- **Output**: Pixel-wise change probability maps
- **Metrics**: IoU = 0.87, F1-Score = 0.89

## 🧪 Testing

Run the test suite:

```bash
# Run all tests
python -m pytest tests/

# Run specific test categories
python -m pytest tests/test_models.py
python -m pytest tests/test_data_processing.py
python -m pytest tests/test_dashboard.py
```

## 📈 Performance Metrics

| Model | Accuracy | Precision | Recall | F1-Score |
|-------|----------|-----------|--------|----------|
| Health Classifier | 92.5% | 91.8% | 92.1% | 91.9% |
| Change Detection | 89.3% | 88.7% | 90.2% | 89.4% |

## 🤝 Contributing

We welcome contributions! Please see our [Contributing Guidelines](CONTRIBUTING.md) for details.

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- UAE Ministry of Environment for providing ground truth data
- European Space Agency for Sentinel-2 imagery access
- NASA for Landsat imagery and climate data
- The open-source community for amazing tools and libraries

## 📞 Contact

- **Project Team**: [Blue-Roots Organization](https://github.com/Blue-Roots)
- **Issues**: [GitHub Issues](https://github.com/Blue-Roots/blue_roots/issues)
- **Discussions**: [GitHub Discussions](https://github.com/Blue-Roots/blue_roots/discussions)

## 🔗 Related Projects

- [Mangrove Monitoring Toolkit](https://github.com/Blue-Roots/mangrove-toolkit)
- [Satellite Data Pipeline](https://github.com/Blue-Roots/satellite-pipeline)
- [Environmental Analytics](https://github.com/Blue-Roots/env-analytics)

---

*Built with ❤️ for UAE mangrove conservation*
