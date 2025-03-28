# 🗣️🌐 Real-Time Language Translator - Speak & Translate! 🗣️🌐

## ✨ Description

Unleash the power of seamless communication with our **Real-Time Language Translator!** This cutting-edge application uses Python and the Streamlit framework to provide an unparalleled translation experience. Speak naturally into your microphone, and watch as your words are instantly translated into your chosen language, complete with synthesized voice output. Break down language barriers and connect with the world like never before! This application uses `SpeechRecognition`, `googletrans`, `gTTS`, `pygame` and `streamlit` library which ensures that the translation experience is seamless.

## 🚀 Features

*   **Instantaneous Translation:** Real-time translation of spoken input from your source language to the target language. No more waiting – just speak and translate!
*   **🎤 Advanced Speech Recognition:** Leverages the SpeechRecognition library for accurate and responsive voice-to-text conversion.
*   **🗣️ Natural-Sounding Voice Output:** Utilizes the gTTS library to convert translated text into clear and natural-sounding spoken audio. Hear your translations come to life!
*   **🌍 Extensive Language Support:** Choose from a vast selection of source and target languages via intuitive dropdown menus.
*   **✨ Intuitive Streamlit Interface:** User-friendly design built with Streamlit, featuring easy-to-use start/stop controls, real-time progress updates, and clear display of source and translated text.
*   **🛡️ Robust Error Handling:** Gracefully handles errors during speech recognition or translation, ensuring a smooth and reliable user experience.

## 🛠️ Dependencies

Before you start, ensure you have the following dependencies installed:

*   streamlit
*   speech\_recognition
*   googletrans
*   gTTS
*   pygame

Install them using pip:

## ⚙️ Setup and Usage

1.  **Clone the repository:**

    ```
    git clone <your-repo-url>
    cd <your-repo-directory>
    ```

2.  **Create a Virtual Environment (Highly Recommended):**

    Keeps your project dependencies isolated.

    ```
    python -m venv venv
    ```

3.  **Activate the Virtual Environment:**

    *   **On Windows:**

        ```
        venv\Scripts\activate
        ```

    *   **On macOS and Linux:**

        ```
        source venv/bin/activate
        ```

4.  **Install Dependencies (if not already done):**

    ```
    pip install -r requirements.txt # if you have requirements.txt file
    pip install streamlit speech_recognition googletrans gTTS pygame # if not
    ```

5.  **Run the application:**

    ```
    streamlit run main.py
    ```

    Replace `main.py` with the correct filename if necessary.

6.  **Using the Translator**

    *   Select your Source Language using the Select Source Language dropdown.
    *   Next, select the Target Language using the Select Target Language dropdown.
    *   To start the translation press the Start Translation button.
    *   To stop the translation press the Stop Translation button.


## 🗂️ Code Structure

*   `main.py`:  The heart of the application, containing the Streamlit UI, language selection logic, speech recognition, translation functions, and text-to-speech synthesis.
*   `get_language_code(language_name)`: Converts user-friendly language names into language codes compatible with the translation API.
*   `translator_function(spoken_text, from_language, to_language)`: Performs the core translation task, leveraging the Google Translate API.
*   `text_to_voice(text_data, to_language)`: Converts translated text into audible speech using gTTS and plays it through Pygame.
*   `main_process(output_placeholder, source_caption_box, target_caption_box, progress_bar, from_language, to_language)`: Manages the real-time translation loop, capturing audio, translating, and providing voice output.

## 🤝 Contributing

Contributions are welcome!  Feel free to submit pull requests with improvements, bug fixes, or new features.

