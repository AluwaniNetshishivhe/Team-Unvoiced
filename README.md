SASL text translator
Team -Unvoiced
The project won 1st Place in Wecncode AI Hackathon SA 2025


this is a folder which contains project files by team Unvoiced

objectives of the project:
Build an AI translation tool that converts SASL signs into text or speech in real time.
Improve accessibility for Deaf and hard-of-hearing communities.
Support multilingual output for South Africa’s official languages.
Ensure high accuracy and speed in recognising diverse SASL variations.
Create a user-friendly interface for mobile and desktop devices.
Promote inclusion by keeping the tool affordable and widely accessible.
Raise SASL awareness through basic sign-learning features.


# 🖐️ ASL Letter Recognition with Gemini AI

An interactive web application that recognizes **South African Sign Language (SASL)** hand signs for the letters **A–E** using **Google Gemini 1.5 Flash** and a webcam or uploaded image. The application provides a simple interface for demonstrating how multimodal large language models can perform image-based classification.

## 📌 Features

* 📷 Capture images directly from your webcam or upload an image.
* 🤖 Recognize SASL letters **A, B, C, D, and E** using Google Gemini.
* ⚡ Fast predictions powered by Gemini 1.5 Flash.
* 🌐 Interactive web interface built with Gradio.
* 🧪 Includes example images for quick testing.

## 🛠️ Technologies Used

* Python
* Google Gemini 1.5 Flash API
* Google Generative AI SDK
* Gradio
* OpenCV
* NumPy
* Base64 Encoding

## ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/sasl-letter-recognition.git
cd sasl-letter-recognition
```

Install the required packages:

```bash
pip install google-generativeai
pip install gradio numpy opencv-python
```

or install from a requirements file:

```bash
pip install -r requirements.txt
```

## 🔑 Configure the Gemini API

Create a Google AI Studio API key.

Replace:

```python
api_key = "Put your Gemini API Key"
```

with your own API key:

```python
api_key = "YOUR_API_KEY"
```

For better security, it is recommended to store the key as an environment variable instead of hardcoding it.

## ▶️ Running the Application

Run the application:

```bash
python app.py
```

Gradio will start a local web server and display a URL such as:

```
http://127.0.0.1:7860
```

Open the URL in your browser.

## 🚀 How It Works

1. Capture or upload an image containing an SASL hand sign.
2. The image is converted into JPEG format and encoded as Base64.
3. The encoded image is sent to the Google Gemini 1.5 Flash model.
4. Gemini analyzes the image and predicts the SASL letter.
5. The application validates the response and displays one of:

* A
* B
* C
* D
* E
* Unknown

## 📸 Example

Input:

* Webcam image showing the SASL sign for **B**

Output:

```
B
```

## ⚠️ Current Limitations

* Supports only letters **A–E**.
* Performance depends on image quality and lighting conditions.
* Recognition accuracy is dependent on the Gemini model's visual understanding.
* This project is intended for learning and demonstration purposes.

## 🔮 Future Improvements

* Support the complete SASL alphabet (A–Z).
* Recognize numbers and common SASL words.
* Add confidence scores for predictions.
* Real-time video recognition.
* Fine-tune using a dedicated ASL dataset for higher accuracy.
* Deploy the application using Hugging Face Spaces or Streamlit Cloud.

## 👨‍💻 Author

Developed as a computer vision and generative AI project demonstrating multimodal image understanding with Google Gemini and Gradio.
