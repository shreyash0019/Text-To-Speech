# Text-To-Speech Converter

This project converts text from a file (`abc.txt`) into speech, saves it as an MP3 file, and plays the MP3 file on your device.

---

## **Prerequisites**

1. **Text File (`abc.txt`):** A text file containing the text you want to convert to speech.
2. **gTTS==2.1.1 module:** This is the Google Text-to-Speech library. Install it using the following command:
   ```bash
   pip install gTTS
   ```
3. **os module:** This module comes pre-installed with Python and does not require a separate installation.

---

## **Installation**

1. Ensure you have Python installed. If not, download and install it from [python.org](https://www.python.org/).
2. Install the `gTTS` module by running the following command in your terminal or command prompt:
   ```bash
   pip install gTTS
   ```

---

## **How it Works**

1. The script reads the text from the `abc.txt` file.
2. The Google Text-to-Speech (`gTTS`) module converts the text into speech.
3. The speech is saved as an MP3 file named `voice.mp3`.
4. The MP3 file is played using the system's default media player.

---

## **Usage Instructions**

1. Create a text file named `abc.txt` and enter the desired text.
2. Run the Python script to convert the text to speech and play it.

---

## **Sample Code**
```python
from gtts import gTTS
import os

# Step 1: Read text from the file
with open('abc.txt', 'r') as file:
    text = file.read()

# Step 2: Convert the text to speech
tts = gTTS(text=text, lang='en')

# Step 3: Save the speech as an MP3 file
tts.save('voice.mp3')

# Step 4: Play the MP3 file
os.system('start voice.mp3')
```

---

## **Contributing**

Feel free to fork this repository and make improvements. Pull requests are welcome!

---

## **License**

This project is licensed under the MIT License.

---

### **Additional Notes**

- The `gTTS` module supports multiple languages. You can change the `lang` parameter in the script to use different languages (e.g., `lang='fr'` for French).
- Ensure your device has a default media player configured to play MP3 files.
- If you encounter any issues with playing the MP3 file, try using other methods or packages like `playsound` for audio playback.

---

