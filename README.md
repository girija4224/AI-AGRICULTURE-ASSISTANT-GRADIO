# AI-Powered Agriculture Assistant

## 🌿 Overview

This project leverages **Google Gemini** and **gTTS** (Google Text-to-Speech) APIs to create an intelligent agriculture assistant capable of detecting plant diseases from leaf images, providing farmer-friendly solutions, and answering general agriculture queries through a conversational chatbot. The assistant can also generate audio responses in multiple languages including English, Hindi, and Telugu.

## 🚀 Features

* **Leaf Disease Detection**: Upload an image of a plant leaf to detect diseases and get practical solutions.
* **Location-based Advice**: Provide a location (city or coordinates) to receive climate-specific agricultural advice.
* **Conversational Chatbot**: Ask any agriculture-related questions and receive expert answers in a structured format with audio support.
* **Text-to-Speech**: Receive answers as speech in multiple languages (English, Hindi, Telugu).

## 🔧 Requirements

* Python 3.x
* Google Cloud API keys (Gemini, OpenWeatherMap)
* Install required dependencies using `pip`

### Dependencies:

* `gradio`: For the user interface.
* `google`: For integrating with Google Gemini API.
* `gTTS`: Google Text-to-Speech for converting advice into audio.
* `requests`: For weather data fetching.

You can install all dependencies using the following command:

```bash
pip install -r requirements.txt
```

## 🧑‍💻 How to Set Up

1. **Clone the repository**:

   ```bash
   git clone https://github.com/your-username/agri-ai-assistant.git
   cd agri-ai-assistant
   ```

2. **Install required dependencies**:

   ```bash
   pip install -r requirements.txt
   ```

3. **Get API Keys**:

   * **Google Gemini API Key**: [Get it here](https://cloud.google.com/genai).
   * **OpenWeatherMap API Key**: [Get it here](https://openweathermap.org/api).

4. **Set your API keys**: Update the API keys in the code where indicated:

   ```python
   client = genai.Client(api_key="YOUR_GOOGLE_GENAI_API_KEY")
   OPENWEATHER_API_KEY = "YOUR_OPENWEATHERMAP_API_KEY"
   ```

5. **Launch the app**:

   ```bash
   python app.py
   ```

   The app will launch and open a web interface in your browser.

## 🌍 How It Works

* **Leaf Disease Detection**: The model uses an image of the leaf to detect the disease and provides advice on how to manage it, considering factors like location and farmer feedback (optional voice input).

* **Conversational Chatbot**: A natural language processing (NLP) model responds to any agriculture-related questions. You can ask the assistant in any of the supported languages (English, Hindi, Telugu), and receive a structured answer.

* **Voice Input/Output**: Voice inputs are processed using `gTTS` to provide spoken answers in the selected language.

## 📱 User Interface

The user interface is built using **Gradio**, allowing easy interaction. There are two main tabs:

1. **Leaf Disease Detection**: Upload a leaf image, optionally provide your location or voice input, and get solutions.
2. **Conversational Chatbot**: Ask any agriculture-related question and get detailed responses in a conversational format.

## 💬 Example Usage

1. **Leaf Disease Detection**: Upload a leaf image, select language, and optionally add location or voice input. The system will detect the disease and provide solutions.
2. **Conversational Chatbot**: Type any agriculture-related question, and get expert responses.

## 🌱 Example Outputs

### 🌿 Leaf Disease Detection:

* **Input**: Image of a leaf showing a yellowing pattern.
* **Output**: "The leaf shows signs of **Leaf Spot Disease**. Here are some solutions:"

  * **Practical Solutions**:

    * Organic: Neem oil application.
    * Chemical: Copper fungicide.
  * **Prevention Tips**:

    * Regular pruning of affected areas.
  * **Fertilizer/Pesticides**:

    * Recommended: Fungicides like Mancozeb, cost: ₹300 for 250g.
  * **Online Store Links**:

    * [Amazon](https://www.amazon.in)
    * [Flipkart](https://www.flipkart.com)
    * [BigHaat](https://www.bighaat.com)

### 💬 Conversational Chatbot:

* **Input**: "How to prevent pests in tomatoes?"
* **Output**: "For pest control in tomatoes, use **organic insecticides** like neem oil or chemical options like **Pyrethrin-based insecticides**."

## 🤖 Contributing

Feel free to fork the repository and make changes! Pull requests are welcome. Ensure to add tests and update the documentation if you introduce new features.

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---


