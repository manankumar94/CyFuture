
# 🎤 **Speech-to-Text Transcription Application**

This is a Python-based **Speech-to-Text Transcription Application** that converts audio files into text using the **Google Speech Recognition API**. It supports multiple audio formats, including **WAV, MP3, M4A, OGG, and FLAC**, and saves the transcription to an output file.

---

## 🚀 **How to Run**

### 1️⃣ **Install Dependencies**

Ensure you have the required libraries installed by running the following commands:
```bash
pip install SpeechRecognition
pip install pydub
pip install ffmpeg  # Required for audio format conversion
```
✅ **Note:** You also need to have `ffmpeg` installed on your system. Install it using:
- **Linux:** `sudo apt install ffmpeg`
- **Mac:** `brew install ffmpeg`
- **Windows:** [Download FFmpeg](https://ffmpeg.org/download.html) and add it to your system PATH.

---

### 2️⃣ **Run the Application**

Execute the script:
```bash
python speech_to_text.py
```

### 3️⃣ **Input Prompts**
You will be asked for:
- **Input Path:** The path to the audio file you want to transcribe.  
- **Output Path:** The path where the transcription will be saved.  
- **Language Code:** The language code (e.g., `en-US` for English, `fr-FR` for French).

---

## 🔧 **File Structure**
```
/speech_to_text/
 ├── speech_to_text.py         # Main Python script
 ├── README.md                  # Documentation file
 ├── example.mp3                # Sample audio file (optional)
 ├── transcription.txt          # Output transcription file
```

---

## ⚙️ **Features**
✅ **Multi-format Support:** Works with WAV, MP3, M4A, OGG, and FLAC files.  
✅ **Automatic Conversion:** Converts non-WAV formats to WAV for transcription.  
✅ **Google Speech Recognition:** Uses Google’s API for accurate transcription.  
✅ **Customizable Language:** Supports different languages via language codes.  
✅ **Output to File:** Saves the transcription to a specified output file.  

---

## 🛠️ **Usage Example**

### 🎯 **Input:**
```
Input Path: /path/to/audio.mp3  
Output Path: /path/to/transcription.txt  
Language Code: en-US  
```

### 📝 **Transcription Output:**
```
Hello, this is a sample transcription of the audio file.
```
The output is saved to `transcription.txt`.

---

## 💡 **Customization**
- To change the speech recognition service, modify:
```python
text = r.recognize_google(audio_data, language=language)
```
➡️ Replace `recognize_google()` with:
- `recognize_sphinx()` → Offline recognition  
- `recognize_bing()` → Microsoft Bing API  
- `recognize_wit()` → Wit.ai  

---

