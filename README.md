# 🌱 Enviroken

**AI-Powered Waste Management for Environmental Justice in Kenya**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![React Native](https://img.shields.io/badge/React%20Native-0.72-61dafb.svg)](https://reactnative.dev/)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.13-orange.svg)](https://tensorflow.org/)

## 🎯 Mission

Transforming waste management in Kenya by incentivizing proper recycling through blockchain rewards while ensuring dignified employment for waste management communities.

## 🚀 Key Features

- **AI-Powered Classification**: VGG-16 transfer learning model for instant waste categorization
- **Blockchain Rewards**: EnviroKoin (EKO) cryptocurrency incentives
- **Community Employment**: Dignified jobs for former landfill workers
- **Partner Network**: Integration with major Kenyan retailers and recyclers
- **Real-time Impact**: Track environmental and social impact metrics

## 🛠 Technology Stack

### Mobile App
- **React Native** - Cross-platform mobile development
- **TensorFlow Lite** - On-device AI inference
- **Camera API** - Waste scanning functionality
- **Web3 Integration** - Blockchain wallet connectivity

### Backend
- **Python/Django** - REST API development
- **PostgreSQL** - Primary database
- **Redis** - Caching and session management
- **Celery** - Background task processing

### Machine Learning
- **TensorFlow 2.13** - Model training and deployment
- **VGG-16 Architecture** - Transfer learning base model
- **OpenCV** - Image preprocessing
- **Docker** - Model serving containers

### Blockchain
- **Polygon Network** - Low-cost transactions
- **Solidity** - Smart contract development
- **Web3.py** - Blockchain integration
- **MetaMask** - Wallet connectivity

## 🏗 Project Structure

```
enviroken/
├── 📱 frontend/
│   ├── mobile-app/          # React Native mobile application
│   ├── web-dashboard/       # Interactive installation prototype
│   └── admin-panel/         # Management dashboard
├── ⚙️ backend/
│   ├── api/                 # Django REST API
│   ├── blockchain/          # Smart contracts & Web3 integration
│   └── ml-model/           # VGG-16 model training & serving
├── 📚 docs/
│   ├── proposals/          # UNEP proposal & project documentation
│   ├── technical/          # API docs, architecture diagrams
│   └── user-guide/         # Installation & usage guides
├── 📊 data/
│   ├── training-data/      # ML model training datasets
│   └── sample-data/        # Test data for development
└── 🚀 deployment/
    ├── docker/             # Container configurations
    └── scripts/            # Deployment automation
```

## 🚀 Quick Start

### Prerequisites
- Node.js 18+
- Python 3.8+
- Docker & Docker Compose
- Git

### Installation

1. **Clone the repository**:
```bash
git clone https://github.com/YOUR_USERNAME/enviroken.git
cd enviroken
```

2. **Set up backend**:
```bash
cd backend
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

3. **Set up mobile app**:
```bash
cd frontend/mobile-app
npm install
# For iOS
cd ios && pod install && cd ..
npx react-native run-ios
# For Android
npx react-native run-android
```

4. **Set up ML model**:
```bash
cd backend/ml-model
python train_vgg16.py  # Train the model
python deploy_model.py  # Deploy for serving
```

## 🤖 ML Model Details

### VGG-16 Transfer Learning
- **Input**: 224x224 RGB images
- **Classes**: 5 waste categories (Plastic, Electronics, Glass, Paper, Metal)
- **Accuracy**: 94.2% on test dataset
- **Model Size**: Optimized to 15MB for mobile deployment
- **Inference Time**: <0.8 seconds on mobile devices

### Model Architecture
```python
# Key modifications to VGG-16
- Frozen base layers (VGG-16 ImageNet weights)
- Custom classifier head for 5 waste classes
- Dropout layers for regularization
- Data augmentation for improved generalization
```

## 🏦 Blockchain Integration

### EnviroKoin (EKO) Token
- **Network**: Polygon (MATIC)
- **Type**: ERC-20 utility token
- **Use Cases**: Recycling rewards, marketplace purchases
- **Distribution**: Algorithmic based on waste impact

### Smart Contracts
```solidity
// Core contracts
├── EnviroToken.sol          # ERC-20 token implementation
├── RewardDistributor.sol    # Automated reward logic
├── MarketplaceIntegration.sol # Retailer partnerships
└── CommunityFund.sol        # Employment fund management
```

## 📈 Impact Metrics

### Environmental Goals
- 🗑️ **10,000 tons** waste diverted annually
- 📉 **15% reduction** in landfill volume
- 🌊 **25% increase** in recycling rates
- 🌍 **5,000 tons CO2** equivalent reduced

### Social Goals
- 👥 **500 jobs** created for waste management communities
- 💰 **35% income increase** for participating workers
- 🏥 **50% reduction** in health issues (pilot communities)
- 📱 **10,000+ users** onboarded to digital payments

## 🤝 Contributing

We welcome contributions from developers, environmental scientists, and community advocates!

### How to Contribute
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### Development Guidelines
- Follow PEP 8 for Python code
- Use ESLint for JavaScript/TypeScript
- Write tests for new features
- Update documentation for API changes

## 📋 Roadmap

### Phase 1: Pilot (Q1-Q2 2024)
- [x] VGG-16 model development
- [x] Mobile app prototype
- [ ] Smart contract deployment
- [ ] Nairobi pilot launch

### Phase 2: Scale-Up (Q3-Q4 2024)
- [ ] Expand to 4 major Kenyan cities
- [ ] Partner integrations (HP, Coca-Cola Kenya)
- [ ] Community employment program
- [ ] UNEP partnership formalization

### Phase 3: National Rollout (2025)
- [ ] Nationwide deployment
- [ ] Regional recycling hubs
- [ ] International expansion framework
- [ ] Policy advocacy and implementation

## 🏆 Recognition & Partnerships

### Target Partnerships
- 🇺🇳 **UNEP** - Primary funding and policy support
- 🏢 **HP Kenya** - E-waste recycling partnership
- 🥤 **Coca-Cola Kenya** - Plastic bottle recycling
- 🛒 **Major Retailers** - Marketplace integration (Naivas, Carrefour, Tuskys)

### Alignment with UN SDGs
- **SDG 8**: Decent Work and Economic Growth
- **SDG 11**: Sustainable Cities and Communities
- **SDG 12**: Responsible Consumption and Production
- **SDG 13**: Climate Action
- **SDG 14**: Life Below Water

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 📞 Contact

**Project Lead**: Manasseh Kinyua  
**Email**: kinyuamanasseh10@gmail.com  
**Location**: Nairobi, Kenya

## 🙏 Acknowledgments

- Waste management communities in Dandora, Nakuru, and Mombasa
- Environmental justice advocates in Kenya
- Open source ML and blockchain communities
- UNEP and environmental policy researchers

---

*Built with ❤️ for environmental justice in Kenya*
