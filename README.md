# Data Sentinel :Azure's PII Looker
Data Sentinel: Azure's PII Looker is a Streamlit application for extracting, detecting, and masking sensitive data from employee ID cards. Powered by Tesseract OCR and Azure Cognitive Services, it identifies PII like names, emails, and phone numbers, anonymizes them, and displays results in an interactive table with image previews.

## Features

1. **Extract Text from Images**:
   - Utilizes Tesseract OCR to extract text from uploaded employee ID card images.
   
2. **PII Detection**:
   - Detects sensitive information such as:
     - Names
     - Phone Numbers
     - Email Addresses
   - Powered by Azure Cognitive Services.

3. **Mask Sensitive Information**:
   - Phone numbers: Shows only the first 3 digits and masks the rest.
   - Email addresses: Displays the first 2 characters of the username, masking the rest.

4. **Department Detection**:
   - Automatically identifies the department (e.g., Sales, Marketing) using regex-based keyword matching.

5. **Interactive UI**:
   - Upload multiple employee ID card images simultaneously.
   - Display masked data in a dynamic table.
   - Preview images with clickable links for quick access.

6. **Batch Processing**:
   - Upload and process multiple images simultaneously.   

## Installation

### Prerequisites
- Python 3.8 or higher
- Azure Cognitive Services subscription for Text Analytics API
- Tesseract OCR installed on your system ([Installation Guide](https://github.com/tesseract-ocr/tesseract))

### Steps
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/data-sentinel.git
   cd data-sentinel
   
2. **Install Dependencies**:
pip install -r requirements.txt


3. **Set Environment Variables**: Replace your_azure_api_key and your_azure_endpoint with your Azure credentials:
 
Here's the README.md tailored for GitHub:

markdown
Copy code
# Data Sentinel: Azure's PII Looker 👁️‍🗨️

**Data Sentinel** is a Streamlit-based application for securely processing employee ID card images. Using **Tesseract OCR** for text extraction and **Azure Cognitive Services** for PII detection, it identifies and anonymizes sensitive data like names, phone numbers, and email addresses.

---

## 🌟 Features
- **Text Extraction**: Extracts text from uploaded employee ID card images.
- **PII Detection**: Identifies sensitive information such as names, phone numbers, and emails.
- **PII Masking**: Protects privacy by masking phone numbers and email addresses.
- **Department Identification**: Detects employee departments (e.g., Sales, Marketing) using keyword matching.
- **Interactive UI**: Displays extracted and masked data in a table with clickable image previews.
- **Batch Processing**: Upload and process multiple images simultaneously.

---

## 🛠️ Installation

### Prerequisites
- Python 3.8 or higher
- Tesseract OCR installed ([Installation Guide](https://github.com/tesseract-ocr/tesseract))
- Azure Cognitive Services subscription for Text Analytics

### Steps
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/data-sentinel.git
   cd data-sentinel
   
2. **Install Dependencies**:

bash
Copy code
pip install -r requirements.txt

3. **Set Environment Variables**: Replace your_azure_api_key and your_azure_endpoint with your Azure credentials:

bash
Copy code
export LANGUAGE_KEY="your_azure_api_key"
export LANGUAGE_ENDPOINT="your_azure_endpoint"

4. **Run the Application**:
streamlit run app.py


## Example Output
After processing employee ID card images, the app displays a table of masked data:

Serial Number	Name	Department	Mobile Number	Email ID	Image
1	John Doe	Marketing	123*******	jo*********@***	[Preview Link]

You can preview images by clicking the links or selecting from the dropdown.

## 🚀Deployment
This app can be deployed on Streamlit Cloud, Azure App Services, or in a Docker container for scalability and flexibility.
 
## 🤝Contributions:
Contributions are welcome! Feel free to fork this repo, create feature requests, or submit pull requests for improvements. Let’s make secure data processing easy and accessible for everyone.

##  📜License:
This project is licensed under the MIT License.

Start protecting your data today with Data Sentinel! 🚀
