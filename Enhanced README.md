# 🦟 WhiteFly Detection System - AgriLens

[![CI/CD Pipeline](https://github.com/[username]/whitefly-detection/actions/workflows/ci-cd.yml/badge.svg)](https://github.com/[username]/whitefly-detection/actions)
[![Python 3.9+](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/downloads/)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)

AI-powered WhiteFly pest detection system for precision agriculture using computer vision and deep learning.

## 👥 Development Team
- **Levy** - DevOps Engineer & CI/CD Pipeline
- **Tusiime Emmanuel** 
- **Ssentongo Henry** 

**Course**: BSE 4105 - DevOps and Cloud Computing  
**Institution**: Makerere University, Uganda

## 🚀 Features
- 🤖 Real-time WhiteFly detection using deep learning
- 🔄 Automated CI/CD pipeline with GitHub Actions
- 🐳 Containerized deployment with Docker
- ☁️ Cloud hosting on Render
- 🔌 RESTful API for predictions
- 📊 Detection accuracy tracking

## 🛠️ Technology Stack
| Category | Technology |
|----------|-----------|
| **Backend** | Python, Flask/FastAPI |
| **ML Framework** | TensorFlow/PyTorch |
| **DevOps** | GitHub Actions, Docker |
| **Deployment** | Render, Vercel |
| **Testing** | pytest, pytest-cov |
| **Version Control** | Git, GitHub |

## 📋 Prerequisites
- Python 3.9 or higher
- Docker Desktop
- Git
- GitHub account

## 🏃 Quick Start

### Local Development
```bash
# 1. Clone the repository
git clone https://github.com/[username]/whitefly-detection.git
cd whitefly-detection

# 2. Create virtual environment
python -m venv venv

# Activate (Linux/Mac)
source venv/bin/activate

# Activate (Windows)
venv\Scripts\activate

# 3. Install dependencies
pip install -r requirements.txt

# 4. Run the application
python app.py

# 5. Access at http://localhost:5000
```

### Using Docker
```bash
# Build the image
docker build -t whitefly-detection:latest .

# Run the container
docker run -p 5000:5000 whitefly-detection:latest

# Access at http://localhost:5000
```

## 🔄 CI/CD Pipeline

Our GitHub Actions pipeline automatically:

1. **🧪 Test Stage**
   - Runs unit tests
   - Checks code coverage
   - Validates code quality

2. **🏗️ Build Stage**
   - Creates Docker images
   - Tests container functionality

3. **🚀 Deploy Stage**
   - Deploys to Render (production)
   - Updates live environment

**Pipeline Status**: View workflows in [Actions tab](https://github.com/[username]/whitefly-detection/actions)

## 📡 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | `/api/predict` | Upload image for detection |
| GET | `/api/health` | Health check endpoint |
| GET | `/api/docs` | API documentation |
| GET | `/api/stats` | Detection statistics |

### Example Request
```bash
curl -X POST http://localhost:5000/api/predict \
  -F "image=@whitefly_sample.jpg"
```

### Example Response
```json
{
  "prediction": "WhiteFly Detected",
  "confidence": 0.94,
  "timestamp": "2025-11-24T10:30:00Z",
  "bounding_boxes": [...]
}
```

## 🧪 Testing
```bash
# Run all tests
pytest

# Run with coverage report
pytest --cov=app --cov-report=html

# Run specific test
pytest tests/test_detection.py -v
```

## 📁 Project Structure
```
whitefly-detection/
├── .github/
│   └── workflows/
│       └── ci-cd.yml       # GitHub Actions pipeline
├── app/
│   ├── __init__.py
│   ├── detection.py        # Detection logic
│   ├── api.py              # API routes
│   └── models/             # ML models
├── tests/
│   ├── test_api.py
│   └── test_detection.py
├── Dockerfile
├── requirements.txt
├── README.md
└── CONTRIBUTING.md
```

## 🤝 Contributing
We welcome contributions! Please see [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

## 📝 License
This project is licensed under the MIT License - see [LICENSE](LICENSE) file.

## 📧 Contact & Support
- **GitHub Issues**: [Report bugs or request features](https://github.com/[username]/whitefly-detection/issues)
- **Email**: [team email]
- **Course**: BSE 4105 - Makerere University

## 🙏 Acknowledgments
- Makerere University - College of Computing & Information Sciences
- BSE 4105 DevOps and Cloud Computing Course
- AgriLens Project Team

---
**⭐ Star this repo if you find it helpful!**

*Developed with 💚 for sustainable agriculture in Uganda*
