I cant change the Visibility because this is a fork

I planned on using an existing steamlit ui and add my code to it.
The streamlit doesnt work for now please use the colab notebook to run the code.
https://colab.research.google.com/drive/18iHI3xTL5yV7J8Ao3f7CA3iTd1Ga4BBG?usp=sharing

**Indic Be My Eyes***
Project Overview
- Indic Be My Eyes is an AI-powered visual assistance application designed specifically for users who speak Indic languages. This application leverages advanced AI models and APIs to provide real-time assistance by converting audio input into text, generating captions for images, and translating them into the user's preferred Indic language. The application aims to empower visually impaired individuals by providing them with a reliable tool to understand their surroundings through voice interactions.

Key Features
- Audio to Text Conversion: Utilizes the Sarvam Audio to Text Translate API to convert audio input from the user into text.
- Visual Captioning: Employs the Groq LLava 1.0 Vision Language Model (VLM) to generate descriptive captions for images.
- Translation: Uses the Sarvam Translate API to convert the generated captions from English to the desired Indic language.
- Text to Speech: Converts the translated text back into speech using the Sarvam Text to Speech API, allowing users to hear the information in their preferred language.

Technical Architecture Overview
The application consists of several key components:
Frontend: The user interface is currently under development using Streamlit, which will provide an interactive experience for users to upload images, input audio, and receive audio feedback in their chosen language.
Backend: Implemented in Python, the backend handles requests to various APIs and processes the data.


# Setup Instructions for Indic Be My Eyes Application

To set up the **Indic Be My Eyes** application for local development using Google Colab, follow these steps:

1. **Open the Google Colab Notebook**:
   - Click on the following link to access the Colab notebook: [Indic Be My Eyes Colab Notebook](https://colab.research.google.com/drive/18iHI3xTL5yV7J8Ao3f7CA3iTd1Ga4BBG?usp=sharing).

2. **Run All Code Blocks**:
   - In the Colab notebook, click on the "Runtime" menu at the top and select "Run all" to execute all the code blocks sequentially. This will set up the necessary libraries and initialize the APIs.

3. **Interactive Section**:
   - The final block of the notebook is interactive and allows you to upload audio and image files to process.

4. **Record Your Voice**:
   - Use an online speech recording software such as [Aspose Voice Recorder](https://products.aspose.app/audio/voice-recorder) to record your voice. Save the recording as a `.wav` file on your local machine.

5. **Upload Audio and Image Files**:
   - In the Colab notebook, locate the section for uploading files. Use the file upload feature to upload your recorded `.wav` file and the image you want to analyze.

6. **Run the Code to Get the Output**:
   - After uploading the audio and image files, run the final code block in the notebook. This will process the audio input and image, generating the output.

7. **View the Output**:
   - The output will include the translated text in the language of your choice. The final speech output will also be generated and saved as a `.wav` file.

8. **Example Files**:
   - Example audio and image files are uploaded in the repository. You can use these files for testing and demonstration purposes.


Future Work
The Indic Be My Eyes application has significant potential for enhancement and expansion. Below are some key areas for future work:

Single Model Training on Synthetic Data:
Objective: To enhance the accuracy and reliability of the application, we will implement a feedback loop that allows users to provide input on the generated outputs.
Features:
Re-Capture: Users can request the application to re-capture or re-describe an image if the initial caption is not satisfactory. This can help in refining the model's understanding of user preferences.
Part-Based Answering: Users can specify parts of the image or audio they want more information about, allowing for a more interactive experience. For example, if a user is interested in a specific object in an image, they can ask for a detailed description of that object.
Continuous Learning: The feedback collected can be used to retrain the model periodically, allowing it to adapt to user preferences and improve accuracy over time.

User Personalization:
Objective: To cater to individual user needs, we will explore personalization features that adjust the model's responses based on user profiles.
Approach: By collecting user preferences (e.g., preferred language, types of descriptions they find most useful), the application can tailor its outputs. This may involve adjusting the level of detail in captions or the style of audio feedback.

Objective: To streamline the application and reduce latency, we aim to train a single, unified model that can handle multiple tasks—audio transcription, image captioning, translation, and text-to-speech generation—using synthetic data.
Approach: By creating a synthetic dataset that simulates various scenarios (e.g., diverse audio inputs, images with different contexts, and translations in multiple Indic languages), we can train a single deep learning model. This would eliminate the need for multiple API calls, reducing response times and improving user experience.
Benefits: This approach will simplify the architecture, reduce dependency on external APIs, and potentially lead to better performance as the model can learn to optimize its responses based on the context of the input.
Integration of Feedback Loop:


