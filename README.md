# 🧠 EchoMind AI

### *An AI-Powered Emotional Intelligence Companion*

<p align="center">

**🥇 1st Prize Winner — TECH AI Fest 🏆**

*College AI Innovation Competition*

<br>

<img src="https://img.shields.io/badge/🏆-1st%20Prize%20Winner-gold?style=for-the-badge" />
<img src="https://img.shields.io/badge/AI-Emotional%20Intelligence-blueviolet?style=for-the-badge" />
<img src="https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge&logo=python&logoColor=white" />
<img src="https://img.shields.io/badge/Gradio-UI-orange?style=for-the-badge" />

</p>

---

## 🏆 Award-Winning Project

> ### 🥇 **1st Prize — TECH AI Fest**
>
> EchoMind AI was awarded **First Prize** at the **TECH AI Fest** for developing an AI-powered emotional intelligence companion that combines conversational AI, emotion analysis, overthinking detection, voice interaction, emotional memory, journaling, and crisis-awareness capabilities into a unified platform.

---

## 🌌 What is EchoMind AI?

**EchoMind AI** is an experimental **AI Emotional Intelligence Companion Platform** designed to understand not only *what a user says*, but also the **emotional context behind their message**.

Instead of functioning as a conventional chatbot, EchoMind analyzes conversations through multiple AI layers:

```text
                ┌──────────────────────────┐
                │       USER INPUT         │
                │   Text / 🎤 Voice        │
                └────────────┬─────────────┘
                             │
                             ▼
              ┌─────────────────────────────┐
              │      🧠 EMOTION ENGINE       │
              │  Emotion Classification      │
              └─────────────┬───────────────┘
                            │
                            ▼
              ┌─────────────────────────────┐
              │      🌀 OVERTHINKING         │
              │     Pattern Detection       │
              └─────────────┬───────────────┘
                            │
                            ▼
              ┌─────────────────────────────┐
              │      🧩 MEMORY ENGINE        │
              │ Previous Emotional Context  │
              └─────────────┬───────────────┘
                            │
                            ▼
              ┌─────────────────────────────┐
              │       🚨 RISK ENGINE         │
              │ Crisis / Stress Awareness   │
              └─────────────┬───────────────┘
                            │
                            ▼
              ┌─────────────────────────────┐
              │       🦙 LLAMA 3 LLM         │
              │  Personalized AI Response   │
              └─────────────┬───────────────┘
                            │
                 ┌──────────┴──────────┐
                 ▼                     ▼
          🔊 Voice Response      📝 Journal
                                   │
                                   ▼
                           📊 Emotion Dashboard
```

---

# ✨ Why EchoMind?

Most conversational AI systems focus primarily on generating an answer.

EchoMind takes a different approach:

> **Understand → Analyze → Remember → Respond**

A single message can pass through multiple intelligence layers before the final response is generated.

### EchoMind can analyze:

* 😊 Emotional state
* 🧠 Emotional context
* 🌀 Overthinking patterns
* 😟 Anxiety-like thought loops
* 🔥 Stress severity
* 🚨 Crisis indicators
* 🧩 Previous emotional context
* 📈 Conversation activity
* 🎤 Voice-based input
* 🔊 Voice-based responses

---

# 🚀 Key Features

## 🧠 1. Emotion Intelligence

EchoMind uses a transformer-based emotion classification model:

```text
j-hartmann/emotion-english-distilroberta-base
```

The user's message is analyzed to identify the dominant emotional state before the LLM generates its response.

### Example

```text
User:
"I've been working all day and I feel completely exhausted."

             ↓

Emotion Engine

             ↓

Detected Emotion:
Sadness / Exhaustion / Stress

             ↓

Llama 3

             ↓

Emotionally-aware response
```

---

## 🌀 2. Overthinking Detection

EchoMind uses:

```text
SamLowe/roberta-base-go_emotions
```

to identify emotional patterns associated with:

* Overthinking
* Anxiety-like loops
* Negative thinking
* Emotional exhaustion
* Obsessive thoughts
* Emotional spirals

The system extracts high-confidence emotional predictions and passes them to the LLM for contextual interpretation.

---

## 🧩 3. Emotional Memory

EchoMind isn't designed to treat every conversation as completely independent.

The project maintains an **emotional memory system** using JSON storage.

```text
Conversation
     │
     ▼
Emotional Analysis
     │
     ▼
Save Memory
     │
     ▼
emotional_memory.json
     │
     ▼
Retrieve Recent Memories
     │
     ▼
Personalized Response
```

The system keeps the **latest 20 memories** and uses the **most recent 5 memories** as conversational emotional context.

This enables responses that consider recurring emotional patterns across interactions.

---

## 🚨 4. Crisis Awareness

EchoMind includes a lightweight emergency-awareness layer.

The system checks the generated emotional analysis for indicators such as:

```text
Suicide Risk: High
Suicide Risk: Possible
Crisis Level: High
Stress Level: Critical
Stress Level: High
```

When high-risk indicators are detected, EchoMind activates an emergency-support message encouraging the user to:

* Contact a trusted person
* Avoid staying alone
* Seek appropriate emotional support

The prototype also references Indian support resources such as:

```text
Tele-MANAS: 14416
AASRA: +91 9820466726
```

---

## 🎤 5. Voice AI

EchoMind supports voice interaction.

### Voice Input

```text
🎤 Microphone
      ↓
SpeechRecognition
      ↓
Text
      ↓
AI Analysis
```

### Voice Output

```text
AI Response
     ↓
gTTS
     ↓
MP3
     ↓
🔊 Voice Playback
```

This allows users to interact with EchoMind through natural spoken conversations.

---

# 🦙 6. Local LLM with Llama 3

The conversational intelligence layer uses:

```text
Llama 3
```

through **Ollama**.

Architecture:

```text
EchoMind
   │
   ├── Emotion Model
   │
   ├── Overthinking Model
   │
   ├── Emotional Memory
   │
   └── Context
          │
          ▼
       Ollama
          │
          ▼
       Llama 3
          │
          ▼
   Personalized Response
```

The project therefore combines **specialized transformer models** with a **generative LLM** rather than relying on a single model.

---

# 💬 7. Personalized Emotional Response

The final LLM prompt combines:

```text
Current Message
       +
Emotion Analysis
       +
Overthinking Analysis
       +
Previous Emotional Memory
       +
Risk Awareness
       ↓
   Llama 3
       ↓
Personalized Response
```

The goal is to make responses feel:

> **Calm • Human • Conversational • Context-aware • Supportive**

---

# 📝 8. Emotional Journal

Every interaction can be stored in:

```text
emotional_journal.json
```

Each journal entry contains:

```json
{
  "timestamp": "...",
  "user_input": "...",
  "emotional_analysis": "...",
  "overthinking_analysis": "..."
}
```

EchoMind can also generate a downloadable:

```text
EchoMind_Journal_Report.txt
```

This creates a persistent record of previous conversations and emotional analyses.

---

# 📊 9. Emotion Activity Dashboard

EchoMind generates a visual dashboard using:

* Pandas
* Matplotlib

The current prototype visualizes conversation activity as an **emotional activity trend**.

```text
Conversations
     │
     ▼
Journal Data
     │
     ▼
Pandas DataFrame
     │
     ▼
Matplotlib
     │
     ▼
📊 emotion_dashboard.png
```

---

# 🎨 10. Modern Gradio Interface

The project includes a custom dark-themed interface built with **Gradio**.

### UI includes:

```text
┌─────────────────────────────────────────────┐
│              🧠 EchoMind AI                 │
│     AI Emotional Intelligence Companion     │
├─────────────────────────────────────────────┤
│                                             │
│  😊 Emotion Engine    🧩 Memory System      │
│  🛡 Safety System                            │
│                                             │
├─────────────────────────────────────────────┤
│                                             │
│              💬 AI CHAT                     │
│                                             │
├─────────────────────────────────────────────┤
│                                             │
│  🧘 Calm Mode                               │
│                                             │
│  Type your message...       🎤              │
│                                             │
│              🚀 SEND                        │
│                                             │
├─────────────────────────────────────────────┤
│ 🔊 Voice Response     📁 Journal             │
│                                             │
│              📊 Dashboard                   │
└─────────────────────────────────────────────┘
```

---

# 🧰 Tech Stack

## 🤖 Artificial Intelligence

| Technology              | Purpose                                        |
| ----------------------- | ---------------------------------------------- |
| **Llama 3**             | Conversational reasoning & response generation |
| **Transformers**        | Emotion and NLP pipelines                      |
| **DistilRoBERTa**       | Emotion classification                         |
| **RoBERTa GoEmotions**  | Emotional / overthinking pattern detection     |
| **LangChain Community** | LLM integration                                |
| **Ollama**              | Local LLM runtime                              |

---

## 🎙️ Voice AI

| Technology                | Purpose             |
| ------------------------- | ------------------- |
| SpeechRecognition         | Speech-to-text      |
| Google Speech Recognition | Voice transcription |
| gTTS                      | Text-to-speech      |
| PyDub                     | Audio processing    |

---

## 💻 Application

| Technology | Purpose                      |
| ---------- | ---------------------------- |
| Python     | Core development             |
| Gradio     | Interactive web UI           |
| JSON       | Journal & memory persistence |
| Pandas     | Data processing              |
| Matplotlib | Visualization                |

---

# 🏗️ System Architecture

```text
                         ┌─────────────────┐
                         │      USER       │
                         └────────┬────────┘
                                  │
                       ┌──────────┴──────────┐
                       │                     │
                    💬 Text              🎤 Voice
                       │                     │
                       │              SpeechRecognition
                       │                     │
                       └──────────┬──────────┘
                                  │
                                  ▼
                       ┌─────────────────────┐
                       │   Emotion Engine    │
                       │   DistilRoBERTa     │
                       └──────────┬──────────┘
                                  │
                                  ▼
                       ┌─────────────────────┐
                       │ Overthinking Engine │
                       │      RoBERTa        │
                       └──────────┬──────────┘
                                  │
                                  ▼
                       ┌─────────────────────┐
                       │   Memory Engine     │
                       │ emotional_memory    │
                       │       .json         │
                       └──────────┬──────────┘
                                  │
                                  ▼
                       ┌─────────────────────┐
                       │   Crisis Awareness  │
                       └──────────┬──────────┘
                                  │
                                  ▼
                       ┌─────────────────────┐
                       │      Ollama         │
                       │      Llama 3        │
                       └──────────┬──────────┘
                                  │
                         ┌────────┴────────┐
                         │                 │
                         ▼                 ▼
                   💬 AI Response     🔊 gTTS
                         │
              ┌──────────┴──────────┐
              ▼                     ▼
        📝 Emotional Journal   📊 Dashboard
```

---

# 🔄 End-to-End Workflow

```text
1. User enters text or voice
              ↓
2. Voice converted to text
              ↓
3. Emotion classification
              ↓
4. Overthinking/emotion pattern analysis
              ↓
5. Previous emotional memories retrieved
              ↓
6. Crisis-awareness check
              ↓
7. Context assembled
              ↓
8. Llama 3 generates response
              ↓
9. Conversation saved
              ↓
10. Emotional memory updated
              ↓
11. Voice response generated
              ↓
12. Journal report generated
              ↓
13. Dashboard generated
```

---

# 📁 Project Structure

```text
EchoMind-AI/
│
├── 📓 EchoMind_AI.ipynb
│
├── 📄 emotional_journal.json
│
├── 🧩 emotional_memory.json
│
├── 📝 EchoMind_Journal_Report.txt
│
├── 📊 emotion_dashboard.png
│
├── 🔊 response.mp3
│
└── README.md
```

> The notebook currently contains the complete implementation, including model loading, AI analysis, memory, journaling, voice processing, dashboard generation, and Gradio UI.

---

# ⚙️ Installation

## 1️⃣ Clone the Repository

```bash
git clone https://github.com/yourusername/EchoMind-AI.git

cd EchoMind-AI
```

---

## 2️⃣ Install Python Dependencies

```bash
pip install transformers
pip install gradio
pip install langchain
pip install langchain-community
pip install sentence-transformers
pip install SpeechRecognition
pip install gtts
pip install pydub
pip install accelerate
pip install torch
pip install matplotlib
pip install pandas
```

---

## 3️⃣ Install Ollama

The notebook uses Ollama as the local LLM runtime.

```bash
curl -fsSL https://ollama.com/install.sh | sh
```

Start Ollama:

```bash
ollama serve
```

---

## 4️⃣ Download Llama 3

```bash
ollama pull llama3
```

Verify:

```bash
ollama list
```

You should see:

```text
llama3
```

---

# ▶️ Running the Project

Open:

```text
EchoMind_AI.ipynb
```

Run the notebook cells sequentially.

The notebook will:

```text
Load AI Models
      ↓
Start Ollama
      ↓
Load Llama 3
      ↓
Initialize Emotion Engine
      ↓
Initialize Memory
      ↓
Launch Gradio Interface
```

Once the Gradio interface starts, interact with EchoMind through the web UI.

---

# ☁️ Kaggle Notebook

The project was developed in a notebook-oriented environment and can be adapted for **Kaggle Notebook** execution.

Basic workflow:

```text
Kaggle Notebook
      │
      ├── Install dependencies
      ├── Start Ollama
      ├── Pull Llama 3
      ├── Load Transformer models
      ├── Initialize EchoMind
      └── Launch Gradio UI
```

> ⚠️ LLM execution through Ollama can be resource-intensive. Runtime availability and model performance will depend on the notebook environment's CPU/GPU/RAM configuration.

---

# 🧪 Example Interaction

### 👤 User

```text
I have been thinking about the same problem all night.
I can't stop replaying everything in my head.
```

### 🧠 EchoMind Analysis

```text
Emotion:
Anxiety / Sadness

Stress Level:
High

Crisis Level:
Low

Suicide Risk:
Low

Mental Clarity Score:
Low
```

### 🌀 Overthinking Analysis

```text
Overthinking Level:
High

Thought Pattern:
Repetitive negative thinking

Emotional Spiral:
Present

Short Human Insight:
The message suggests a recurring thought loop
and difficulty disengaging from the situation.
```

### 💬 EchoMind Response

The Llama 3 conversational layer uses these signals together with recent emotional memory to generate a personalized supportive response.

---

# 🔬 AI Pipeline

EchoMind follows a **multi-model AI architecture**:

```text
                   USER MESSAGE
                        │
                        ▼
             ┌─────────────────────┐
             │ Emotion Classifier  │
             │   DistilRoBERTa     │
             └──────────┬──────────┘
                        │
                        ▼
             ┌─────────────────────┐
             │ Pattern Classifier  │
             │      RoBERTa        │
             └──────────┬──────────┘
                        │
                        ▼
             ┌─────────────────────┐
             │ Emotional Memory    │
             │ Recent Context      │
             └──────────┬──────────┘
                        │
                        ▼
             ┌─────────────────────┐
             │ Crisis Awareness    │
             └──────────┬──────────┘
                        │
                        ▼
             ┌─────────────────────┐
             │      Llama 3        │
             │ Conversational LLM  │
             └──────────┬──────────┘
                        │
                        ▼
                PERSONALIZED AI
                    RESPONSE
```

---

# 💡 What Makes This Project Different?

### Conventional chatbot

```text
User
 ↓
LLM
 ↓
Response
```

### EchoMind

```text
User
 ↓
Emotion
 ↓
Overthinking
 ↓
Memory
 ↓
Risk Awareness
 ↓
LLM Reasoning
 ↓
Personalized Response
 ↓
Voice + Journal + Dashboard
```

The project demonstrates how **multiple AI components can be orchestrated into one intelligent application** rather than simply connecting a chatbot to an interface.

---

# 🧠 Skills Demonstrated

This project demonstrates practical experience with:

* Python
* Natural Language Processing
* Transformer Models
* Emotion Classification
* LLM Integration
* Prompt Engineering
* Local LLM Deployment
* Ollama
* LangChain
* Speech-to-Text
* Text-to-Speech
* Conversational AI
* Memory Systems
* JSON Data Persistence
* Data Visualization
* Gradio
* AI Application Development
* Multi-model AI orchestration

---

# 🏆 Competition Highlight

## 🥇 TECH AI Fest — 1st Prize

EchoMind AI was presented as an AI innovation project at **TECH AI Fest** and received:

<div align="center">

# 🥇 FIRST PRIZE

### TECH AI FEST

**AI • Innovation • Emotional Intelligence**

</div>

The project stood out by bringing together:

```text
🤖 Generative AI
🧠 Emotion Intelligence
🌀 Overthinking Detection
🧩 Emotional Memory
🎤 Voice AI
🚨 Crisis Awareness
📊 Data Visualization
🎨 Interactive UI
```

into a single AI application.

---

# 🔮 Future Roadmap

EchoMind is designed as a foundation for a more advanced emotional-intelligence platform.

### 🚧 Planned Improvements

* [ ] Real-time emotion trend extraction
* [ ] More accurate stress scoring
* [ ] Advanced risk classification
* [ ] Multilingual emotional conversations
* [ ] Real-time voice conversation
* [ ] Speaker emotion recognition
* [ ] Long-term vector-based memory
* [ ] RAG-based personal context
* [ ] PostgreSQL / MongoDB persistence
* [ ] User authentication
* [ ] Cloud deployment
* [ ] Mobile application
* [ ] Advanced analytics dashboard
* [ ] Explainable emotion predictions
* [ ] Model evaluation framework
* [ ] MLOps monitoring
* [ ] Model versioning
* [ ] Privacy-focused data architecture

---

# 🔐 Privacy & Responsible AI

EchoMind is an **experimental AI emotional-wellness project**, not a medical or clinical diagnostic system.

The emotional analysis generated by the project should **not be treated as a professional medical diagnosis or substitute for qualified mental-health care**.

For a production implementation, additional safeguards would be required, including:

* Secure data storage
* Encryption
* Authentication
* Explicit consent
* Stronger crisis classification
* Human escalation workflows
* Privacy controls
* Model evaluation
* Bias and safety testing

---

# 📜 Disclaimer

> **EchoMind AI is an educational and experimental AI project intended to demonstrate conversational AI, emotion analysis, memory systems, voice interaction, and responsible AI concepts. It is not a medical device, therapist, or replacement for professional mental-health services.**

---

# 🌟 Project Vision

EchoMind is built around one simple idea:

> ### **AI shouldn't only understand our words. It should understand the emotional context behind them.**

The long-term vision is to build an AI companion capable of recognizing emotional patterns, remembering meaningful context, understanding voice and language, and responding in a more human-centered way.

```text
        LISTEN
           ↓
       UNDERSTAND
           ↓
        REMEMBER
           ↓
        ANALYZE
           ↓
        RESPOND
           ↓
        SUPPORT
```

### 🧠 EchoMind AI

**From conversation → to emotional intelligence.**

---

# 👨‍💻 Project

**EchoMind AI**
AI Emotional Intelligence Companion Platform

🏆 **1st Prize — TECH AI Fest**

Built with:

```text
Python • Transformers • Llama 3 • Ollama
LangChain • Gradio • SpeechRecognition
gTTS • Pandas • Matplotlib
```

---

<p align="center">

### ⭐ If you found EchoMind AI interesting, consider giving the repository a star!

<br>

**Made with 🧠 + 🤖 + ❤️**

</p>
