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

![image](https://github.com/user-attachments/assets/19e28cb4-4105-4df1-9585-3a8d2fe4be06)
![image](https://github.com/user-attachments/assets/363b7f5f-be3b-4dd2-ad6d-1069c1dae4fe)



### 2. Injury Analysis 🩹
- **Image-based Analysis**: Upload and analyze injury photos
- **Emergency Response**: Get immediate action steps and recommendations
- **Required Items**: Suggests specific medical supplies needed
- **Product Recommendations**: Shows images of recommended medical products
- **Medical Guidance**: Provides conditions for seeking immediate medical help
![image](https://github.com/user-attachments/assets/86f0219c-f39c-449b-bacf-3a577342ee47)

### 3. Appointment Booking System 📅
- **Real-time Booking**: Schedule appointments with different specialists
- **Email Notifications**: Automated confirmation emails to patients and doctors
- **Calendar Integration**: In the emails there is a link will be provided by which they can mark their appointment in their Google Calender
- **Appointment Tracking**: View and manage upcoming appointments
- **Multiple Specialists**: Choose from various medical specialists
![image](https://github.com/user-attachments/assets/0b59df4c-646c-4346-8077-540ecb5bcdac)

## Technical Stack 💻

- **Frontend**: Streamlit
- **AI/ML**: 
  - Google's Gemini AI for image analysis
  - Random Forest classifier
  - TF-IDF vectorization for text processing
- **APIs**:
  - Gemini Flash 1.5
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
    ![image](https://github.com/user-attachments/assets/10e0e668-da6f-4dab-814b-704abc0740b8)

3. For bulk analysis:
   - Upload a CSV file containing medical cases
   - Click "Analyze All Cases" to process
![image](https://github.com/user-attachments/assets/b0e9860e-6d9d-437a-803d-b8d7e1f2a95a)

### Injury Analysis
1. Upload an injury photo
2. Click "Analyze Injury"
3. Review the analysis results, including:
   - Injury type classification
   - Immediate action steps
   - Required medical supplies
   - Conditions requiring medical attention
![image](https://github.com/user-attachments/assets/88133d33-db76-4d63-b571-c965b2886bc8)

### Appointment Booking
1. Fill in patient details
2. Select preferred doctor and appointment time
3. Enter symptoms/reason for visit
4. Submit to receive email confirmation and calendar invite
![image](https://github.com/user-attachments/assets/a03f9329-247f-47a9-a203-45a4f694c154)



## Contributing 🤝

Feel free to fork the repository and submit pull requests. For major changes, please open an issue first to discuss the proposed changes.

## Authors ✍️

- Lead Developer: Gandham Mani Saketh


## License 📄

This project is licensed under the MIT License - see the LICENSE file for details.
