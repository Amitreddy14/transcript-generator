# transcript-generator
This Python code is a Streamlit application that extracts transcripts from YouTube videos and generates detailed summaries using Google Gemini Pro. The key functionalities and components of the code are as follows:

Libraries and Modules:

streamlit for creating the web application interface.
dotenv for loading environment variables.
os for accessing environment variables.
google.generativeai for interacting with Google's generative AI models.
youtube_transcript_api for fetching YouTube video transcripts.
Environment Setup:

The dotenv module loads environment variables from a .env file.
The Google API key is retrieved using os.getenv and used to configure the google.generativeai module.
Prompt Definition:

A prompt string defines the task for the generative AI model, instructing it to summarize the transcript in points within 250 words.
Transcript Extraction:

The function extract_transcript_details(youtube_video_url) extracts the transcript from a YouTube video URL using the YouTubeTranscriptApi. It concatenates the transcript text into a single string.
Summary Generation:

The function generate_gemini_content(transcript_text, prompt) sends the transcript and prompt to the Google Gemini Pro model to generate a summary. The response text is returned as the summary.
Streamlit Application:

The app's title is set to "YouTube Transcript to Detailed Notes Converter".

A text input widget allows users to enter a YouTube video link.

When a valid YouTube link is provided, the video thumbnail is displayed.
A button labeled "Get Detailed Notes" triggers the extraction and summarization process.

The resulting summary is displayed as markdown under the heading "Detailed Notes".


##Required Packages

youtube_transcript_api: For fetching transcripts from YouTube videos.
streamlit: For building the web application interface.
google-generativeai: For interacting with Google's generative AI models.
python-dotenv: For loading environment variables from a .env file.
pathlib: For file path operations (although not explicitly used in the given code).



##Usage

Ensure the necessary packages are installed.
Set up a .env file with the required Google API key.
Run the Streamlit application using streamlit run <script_name>.py.
Enter a YouTube video link in the text input field and click "Get Detailed Notes" to generate the video summary.
This application provides a convenient way to convert YouTube video transcripts into concise, detailed notes using state-of-the-art generative AI.


OUTPUTS


![output 3](https://github.com/user-attachments/assets/6d405c3f-4c56-4143-b882-9c57a98d7244)

![output 2](https://github.com/user-attachments/assets/0098f56f-edb4-4ee2-a71f-e10519cc575a)

![output1](https://github.com/user-attachments/assets/9e2f70f7-8fb0-497d-a117-265b866815b2)

