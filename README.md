# Medical Report Processor

A Streamlit-based web application that processes medical report images (e.g., prescriptions or consultation notes) using OCR to extract structured data and generate formatted PDF reports. The app intelligently displays either prescription details (patient info and medications) or comprehensive details (doctor, patient, contact info, date) based on the extracted data.

## Features
- Upload JPEG/PNG images of medical reports.
- Extracts data using Mistral OCR into a JSON format.
- Displays extracted data in a clean, organized UI with boxed sections.
- Generates a downloadable PDF report:
  - For prescriptions: Patient details and medication table.
  - For non-prescriptions: Doctor, patient, contact info, and date.
- Runs in Google Colab with ngrok for easy access.

## Screenshots

### Home Page
![Home Page](screenshots/ui_home.png)
*Upload an image to start processing.*

### Prescription Output
![Prescription Output](screenshots/prescription_output.png)
*Formatted display of a prescription with patient details and medications table.*

### Non-Prescription Output
![Non-Prescription Output](screenshots/non_prescription_output.png)
*Structured view of doctor, patient, contact info, and date for non-prescription reports.*

## Tech Stack
- **Python**: Core programming language.
- **Streamlit**: Web app framework for the UI.
- **Mistral AI**: OCR and JSON parsing via `mistralai` API.
- **ReportLab**: PDF generation.
- **Pyngrok**: Exposes the app via a public URL.
- **Google Colab**: Runtime environment.

## Setup Instructions
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/CodeRxWizard/Medical-Report-Processor.git
