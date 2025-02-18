# DeepSeek-R1-AI-Voice-Agent 

This project enables real-time speech-to-text transcription using AssemblyAI, generates AI responses with **DeepSeek R1 (7B model) via Ollama**, and converts text responses into speech using ElevenLabs. The entire process happens in real-time, allowing for seamless interaction.  

---

## Features  
- **Real-time speech-to-text** using AssemblyAI  
- **AI-powered responses** with DeepSeek R1 (7B model) via Ollama  
- **Instant text-to-speech** conversion with ElevenLabs  
- **Live audio streaming** for an interactive experience  

---

## 🛠️ Setup Instructions  

### Step 1: Sign Up & Install Dependencies  

#### ✅ Get API Keys  
- **AssemblyAI (for speech-to-text):** [Sign up for a free API key](https://www.assemblyai.com/?utm_source=youtube&utm_medium=referral&utm_campaign=yt_smit_28)  
- **ElevenLabs (for text-to-speech):** [Sign up for an account](https://elevenlabs.io/)  

#### ✅ Install Ollama  
DeepSeek R1 is accessed via Ollama. Install Ollama from:  
🔗 **[Download Ollama](https://ollama.com/)**  

#### ✅ Install PortAudio (Required for real-time transcription)  
- **Debian/Ubuntu:**  
  ```bash
  apt install portaudio19-dev
  ```

  MacOS:
  ```bash
  brew install portaudio
  ```
####✅ Install Python Libraries

Before running the script, install the required dependencies:

```bash
pip install "assemblyai[extras]"
pip install ollama
pip install elevenlabs
```
✅ (MacOS Only) Install MPV for Audio Streaming

```bash
brew install mpv
```
### Step 2: Download the DeepSeek R1 Model
Since this script uses DeepSeek R1 via Ollama, download the model locally by running:

```bash
ollama pull deepseek-r1:7b
```


### 🎯 Running the Script

Once all dependencies are installed and the model is downloaded, simply run:

```bash
python AIVoiceAgent.py
```