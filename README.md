# Text-To-Speech

This project converts text from a file (`abc.txt`) into speech, saves it as an MP3 file, and plays the MP3 file on your device.

## Prerequisites

- **abc.txt**: A text file containing the text you want to convert to speech.
- **gTTS==2.1.1** module: Install using `pip install gTTS`.
- **os** module: This module comes pre-installed with Python, no need to install separately.

## Installation

1. Ensure you have Python installed. If not, download and install it from [python.org](https://www.python.org/).
2. Install the `gTTS` module by running the following command:
   ```bash
   pip install gTTS
## How it works

   1.The script reads the text from the abc.txt file.
   
   2.The Google Text-to-Speech (gTTS) module converts the text into speech.
   
   3.The speech is saved as an MP3 file (voice.mp3).
   
   4.The MP3 file is played using the system's default media player.

## Contributing

Feel free to fork this repository and make improvements. Pull requests are welcome!

## License
This project is licensed under the MIT License.
