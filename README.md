# Neuro Trace

An AI-Powered Cognitive Health Assessment Platform that combines clinical data analysis with handwriting analysis for early detection of cognitive decline.

## 🌟 Features

### Multi-Modal Analysis
- **Clinical Features Analysis**: Processes comprehensive patient data including demographics, medical history, and cognitive assessments
- **Handwriting Analysis**: AI-powered analysis of handwriting samples for cognitive decline markers
- **Ensemble Predictions**: Combined analysis using both clinical data and handwriting samples for enhanced accuracy

### User-Friendly Interface
- **Flexible Input Methods**:
  - Upload medical reports (PDF extraction supported)
  - Manual data entry with validated forms
  - Handwriting sample uploads
- **Multiple User Modes**:
  - Doctor mode for healthcare professionals
  - Patient mode for self-assessment
- **Real-time Processing**: Instant feedback and analysis results

### Professional Tools
- Automated report generation
- Comprehensive prediction results
- Progress tracking
- PDF text extraction support
- Multiple prediction modes (features-only, image-only, ensemble)

## 🚀 Getting Started

### Prerequisites
- Python 3.8+
- Node.js 14+
- npm or yarn

### Backend Setup

1. Navigate to the Deployment directory:
```bash
cd Deployment
```

2. Install Python dependencies:
```bash
pip install -r requirements.txt
```

Required Python packages:
- fastapi
- uvicorn
- tensorflow
- opencv-python
- pandas
- numpy
- scikit-learn
- joblib

3. Run system checks:
```bash
python system_check.py
```

4. Start the API server:
```bash
python main.py
```

The backend API will be available at `http://localhost:9000`

### Frontend Setup

1. Navigate to the Frontend directory:
```bash
cd Frontend
```

2. Install dependencies:
```bash
npm install
```

3. Start the development server:
```bash
npm start
```

The frontend will be available at `http://localhost:3000`

## 📁 Project Structure

```
Neuro_Trace/
├── Deployment/          # Backend Python API
│   ├── main.py         # Main API implementation
│   ├── system_check.py # System verification
│   └── requirements.txt
├── Frontend/           # React TypeScript frontend
│   ├── src/
│   │   ├── components/ # UI components
│   │   ├── pages/      # Page components
│   │   ├── services/   # API integration
│   │   └── utils/      # Helper functions
│   └── package.json
└── Models/            # AI model files
    ├── densenet_handwriting.h5
    ├── mlp_dementia_model.h5
    └── preprocessor.pkl
```

## � Download Models

Pre-trained model files are large and may be hosted separately. You can download the models used by this project from the Google Drive folder:

https://drive.google.com/drive/folders/1ReZ96bGOH-uenS8uMQVVs_UxtLQYTK7O?usp=sharing

Place the downloaded model files into the `Models/` directory before starting the backend.

## �🔧 API Endpoints

- `POST /predict/json`: Prediction using clinical features
- `POST /predict/file`: Prediction using handwriting image
- `POST /predict/form`: Prediction using form data
- `POST /predict/ensemble`: Combined prediction using both features and handwriting
- `GET /health`: API health check

## 💡 Usage

1. Choose user mode (doctor/patient)
2. Upload medical data or enter manually
3. Upload handwriting sample (optional)
4. Review and validate data
5. Get instant AI-powered assessment
6. Download detailed reports

## 🔐 Features by Mode

### Doctor Mode
- Full access to all clinical features
- Professional report generation
- Comprehensive patient data management

### Patient Mode
- Simplified data entry
- Basic report access
- Self-assessment tools

## 🏆 Competition Ready Features

- Modern UI with glassmorphism effects
- ConvNeXt model for improved accuracy
- Multi-method preprocessing
- Sample data for demonstrations
- Enhanced error handling
- Real-time prediction timing

## 🛠️ Troubleshooting

If you encounter issues:

1. Run system checks:
```bash
python system_check.py
```

2. Verify all models are present in the Models directory
3. Check if the API is running on port 9000
4. Ensure all dependencies are installed correctly
