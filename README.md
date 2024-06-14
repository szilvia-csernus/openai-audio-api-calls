# OpenAI Audio API Calls

Simple API calls using OpenAI's Audio APIs: Whisper and the Text To Speach API.


> In the `audio-api-calls.ipynb` jupyter notebook, I demonstrate how to use the OpenAI Audio API models, Whisper and the Text To Speech APIs.


I included the following examples:



1. English speech to text function (whisper-1).

2. English speech to text with and without context (whisper-1).

3. Hungarian speech to Hungarian text (whisper-1).

4. Hungarian speech to English text translation (whisper-1).

5. English text to English audio (tts-1).

6. Hungarian text to Hungarian audio (tts-1).


---

---

## How to run this project?

0. Prerequisites:

   - Make sure Python3 is installed.
   - If you don't have an account with OpenAI, create one here: https://openai.com/
   - Create a project API key under Dashboard / API keys

1. Clone the project.

2. Create a virtual environment inside the project folder:

   `python -m venv venv`

3. Activate the virtual environment:

   Mac: `source venv/bin/activate`

   Windows: `venv\Scripts\activate`

4. Select interpreter in VSCode:

   (on Mac) Cmd + Shift + P  ---> Select Interpreter ---> Select the created venv environment

5. Install the python dependencies:

   `pip install -r requirements.txt`

   Note: `pyaudio` is required only for recording audio files programmatically, not essential to run the api calls. Nevertheless, on Macs, `pyaudio` requires `portaudio` to be installed globally. Best to install it with `brew`, i.e. `brew install portaudio`

6. Create an `.env` file in the root folder and add your project's API key:

   ```
   OPENAI_API_KEY=your-unique-opanai-project-key

   ```

7. Run the Jupyter Notebook:

   - `jupyter notebook` command will open the Notebook in the browser.
   - The `audio-api-calls.ipynb` file provides the examples.

## Credits

- This project was adopted from Colt Steele's Walkthrough project on Udemy: [Mastering OpenAI Python APIs](https://www.udemy.com/course/mastering-openai/?couponCode=24T3MT53024).

  Changes made: I updated the API calls as per the latest documentation.

- OpenAI: https://openai.com
