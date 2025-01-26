# Telemedicine

This Project is Done during the Internship under the Infosys Springboard 


# MediScan - Medical Analysis Suite 🏥

MediScan is a comprehensive medical analysis web application built with Streamlit that offers medical text analysis, injury analysis, and appointment booking capabilities. The application leverages advanced AI models and APIs to provide accurate medical assessments and recommendations.

## Features 🌟

### 1. Medical Text Analysis 📝
- **Single Case Analysis**: Analyze individual medical cases with severity assessment
- **Bulk Case Analysis**: Process multiple cases via CSV upload
- **Severity Classification**: Automatic classification into High, Moderate, and Low severity
- **Confidence Scores**: Provides confidence levels for each assessment
- **Duration Context Analysis**: Identifies and flags concerning symptom durations
- **Interactive Visualizations**: Gauge charts and pie charts for analysis results

### 2. Injury Analysis 🩹
- **Image-based Analysis**: Upload and analyze injury photos
- **Emergency Response**: Get immediate action steps and recommendations
- **Required Items**: Suggests specific medical supplies needed
- **Product Recommendations**: Shows images of recommended medical products
- **Medical Guidance**: Provides conditions for seeking immediate medical help

### 3. Appointment Booking System 📅
- **Real-time Booking**: Schedule appointments with different specialists
- **Email Notifications**: Automated confirmation emails to patients and doctors
- **Calendar Integration**: Google Calendar integration for appointment management
- **Appointment Tracking**: View and manage upcoming appointments
- **Multiple Specialists**: Choose from various medical specialists

## Technical Stack 💻

- **Frontend**: Streamlit
- **AI/ML**: 
  - Google's Gemini AI for image analysis
  - Custom trained medical text classifier
  - TF-IDF vectorization for text processing
- **APIs**:
  - Google Calendar API
  - Google Custom Search API
  - Gmail SMTP for email notifications
- **Data Processing**:
  - Pandas for data manipulation
  - Plotly for interactive visualizations
  - Joblib for model serialization

## Setup Instructions 🚀

1. Clone the repository
```bash
git clone <repository-url>
```

2. Install required dependencies
```bash
pip install -r requirements.txt
```

3. Set up environment variables:
```bash
GEMINI_API_KEY=your_gemini_api_key
GOOGLE_SEARCH_API_KEY=your_google_search_api_key
GOOGLE_CX=your_google_cx_id
```

4. Configure email settings:
- Update the sender email and password in the `send_appointment_email` function
- Enable "Less secure app access" for the sender Gmail account

5. Run the application:
```bash
streamlit run app.py
```

## Usage Guide 📖

### Medical Text Analysis
1. Choose between single case or bulk analysis
2. For single case:
   - Enter medical notes or select from example cases
   - Click "Analyze Case" to get results
3. For bulk analysis:
   - Upload a CSV file containing medical cases
   - Click "Analyze All Cases" to process

### Injury Analysis
1. Upload an injury photo
2. Click "Analyze Injury"
3. Review the analysis results, including:
   - Injury type classification
   - Immediate action steps
   - Required medical supplies
   - Conditions requiring medical attention

### Appointment Booking
1. Fill in patient details
2. Select preferred doctor and appointment time
3. Enter symptoms/reason for visit
4. Submit to receive email confirmation and calendar invite

## Security and Privacy 🔒

- All medical data is processed locally
- No patient data is stored permanently
- Secure email communications
- OAuth2 authentication for calendar integration

## Contributing 🤝

Feel free to fork the repository and submit pull requests. For major changes, please open an issue first to discuss the proposed changes.

## Authors ✍️

- Lead Developer: Gandham Mani Saketh
- Group-1 Team Members

## License 📄

This project is licensed under the MIT License - see the LICENSE file for details.
