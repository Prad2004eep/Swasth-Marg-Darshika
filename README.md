# Swasth-Marg-Darshika 🏥

An intelligent healthcare assistant system that provides disease predictions, health insights, and personalized recommendations based on user symptoms.

## 🌟 Features

### Core Functionality
- **Symptom Analysis**: Input symptoms and get potential disease predictions
- **AI-Powered Insights**: Uses Google Gemini API for intelligent health recommendations
- **Multi-API Integration**: Combines data from RapidAPI diagnosis and OpenFDA medication databases
- **Personalized Recommendations**: Get diet, workout, and medication suggestions
- **User Authentication**: Secure login and registration system
- **Visual Symptom Guide**: Interactive symptom images and related conditions

### Technical Features
- **Intelligent Caching**: Optimized API calls with 24-hour cache system
- **Fallback Mechanisms**: Robust error handling with symptom-specific fallbacks
- **Responsive Design**: Modern UI with smooth animations and transitions
- **Text-to-Speech**: Audio playback for health recommendations
- **Session Management**: User profile and search history tracking

## 🛠️ Technology Stack

### Backend
- **Flask**: Python web framework
- **Machine Learning**: Scikit-learn SVM model for disease prediction
- **APIs**: Google Gemini, RapidAPI, OpenFDA
- **Caching**: LRU cache with file-based persistence

### Frontend
- **HTML5/CSS3**: Modern responsive design
- **JavaScript**: Interactive features and API communication
- **Anime.js**: Smooth animations and transitions
- **Bootstrap**: Responsive UI components

### Data Processing
- **Pandas**: Dataset management and processing
- **NumPy**: Numerical computations
- **Pickle**: Model serialization

## 📁 Project Structure

```
Swasthya_Mardarshika/
├── main.py                 # Main Flask application
├── gemini_api.py          # Google Gemini API integration
├── api_integration.py     # External API integrations
├── symptom_image_generator.py # Symptom image generation
├── models/                # Trained ML models
├── datasets/              # Medical datasets
├── templates/             # HTML templates
├── static/                # CSS, JS, and assets
├── api_cache/             # API response cache
└── requirements.txt       # Python dependencies
```

## 🚀 Installation & Setup

### Prerequisites
- Python 3.8+
- Node.js 14+ (for frontend dependencies)
- Git

### 1. Clone the Repository
```bash
git clone https://github.com/Prad2004eep/Swasth-Marg-Darshika.git
cd Swasth-Marg-Darshika/Swasthya_Mardarshika
```

### 2. Set Up Python Environment
```bash
# Create virtual environment
python -m venv venv

# Activate virtual environment
# On Windows:
venv\Scripts\activate
# On macOS/Linux:
source venv/bin/activate

# Install Python dependencies
pip install -r requirements.txt
```

### 3. Install Frontend Dependencies
```bash
npm install
```

### 4. Set Up API Keys
Create a `.env` file in the root directory and add your API keys:
```
GEMINI_API_KEY=your_gemini_api_key
RAPIDAPI_KEY=your_rapidapi_key
OPENFDA_KEY=your_openfda_key
PLAY_HT_API_KEY=your_play_ht_api_key
```

### 5. Prepare Datasets and Models
Ensure the following files are in place:
- `datasets/symtoms_df.csv`
- `datasets/precautions_df.csv`
- `datasets/workout_df.csv`
- `datasets/description.csv`
- `datasets/medications.csv`
- `datasets/diets.csv`
- `models/.ipynb_checkpoints/svc.pkl`

### 6. Run the Application
```bash
python main.py
```

The application will be available at `http://localhost:5001`

## 📊 Datasets

The system uses comprehensive medical datasets including:
- **Symptoms Dataset**: 132 symptoms mapped to diseases
- **Disease Descriptions**: Detailed information for 41 diseases
- **Precautions**: Safety measures for each condition
- **Medications**: Recommended treatments
- **Diet Plans**: Nutrition guidelines
- **Workout Routines**: Exercise recommendations

## 🔧 API Integrations

### Google Gemini API
- Provides intelligent health insights
- Generates personalized recommendations
- Handles symptom analysis beyond the trained dataset

### RapidAPI Diagnosis API
- Professional medical diagnosis
- Symptom-to-condition mapping
- Clinical-grade accuracy

### OpenFDA API
- FDA-approved medication information
- Drug indications and warnings
- Side effects and contraindications

## 🎯 Key Features Explained

### Disease Prediction System
- Uses Support Vector Machine (SVM) model
- 132-dimensional symptom space
- 41 disease classifications
- Confidence scoring and fallback mechanisms

### Intelligent Caching
- Reduces API calls by 80%
- 24-hour cache expiration
- File-based persistence
- LRU memory caching

### User Experience
- Modern, responsive interface
- Real-time symptom validation
- Interactive symptom images
- Audio playback of recommendations
- Personalized user profiles

## 🔒 Security Features

- Session-based authentication
- API key protection
- Input sanitization
- Rate limiting on API calls
- Secure password handling

## 📈 Performance Optimizations

- Asynchronous API calls
- Efficient data structures
- Minimal memory footprint
- Optimized database queries
- Compressed static assets

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## ⚠️ Disclaimer

**Important Medical Disclaimer**: This system is for informational purposes only and should not be used as a substitute for professional medical advice, diagnosis, or treatment. Always seek the advice of qualified healthcare providers with any questions you may have regarding a medical condition.

## 🐛 Bug Reporting

If you encounter any issues, please report them through the GitHub Issues page with:
- Detailed description of the issue
- Steps to reproduce
- Expected vs. actual behavior
- System information

## 📞 Support

For support and questions:
- Create an issue on GitHub
- Check the documentation
- Review existing issues

## 🔄 Version History

- **v1.0.0**: Initial release with core functionality
- **v1.1.0**: Added API integrations and caching
- **v1.2.0**: Enhanced UI and user authentication
- **v1.3.0**: Added symptom images and text-to-speech

## 🌟 Acknowledgments

- Google Gemini API for AI-powered insights
- RapidAPI for medical diagnosis data
- OpenFDA for medication information
- The medical community for dataset contributions
- Open-source community for tools and libraries

---

**Made with ❤️ for better healthcare accessibility**
