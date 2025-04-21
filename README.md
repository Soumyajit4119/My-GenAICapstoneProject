# A GenAI-Powered Mental Health Assistant 🤖

Welcome to **Daily Journal Analyzer**, a Generative AI-powered mental wellness assistant that helps you reflect, track, and grow through intelligent journal analysis. Designed as part of my capstone project for the Gen AI Intensive Course, this tool blends emotional awareness with cutting-edge GenAI to make journaling a more insightful and helpful experience.

<br>

## 🚀 Project Overview

In today’s fast-paced world, journaling has emerged as a simple yet powerful tool to reflect on our thoughts, manage stress, and monitor emotional well-being. However, it’s often difficult for individuals to objectively interpret their own writing or derive actionable insights from it.

This notebook introduces a lightweight **Generative AI-powered Daily Journal Analyzer**, built using **Google’s Gemini API**. With just a short paragraph of text describing how your day went, the assistant provides a structured emotional analysis including:
- Mood classification
- Emotional tone and confidence
- Key thought patterns
- Mental health suggestions

Unlike traditional machine learning solutions, this project does **not require any dataset, training, or labeling**. Instead, it leverages **few-shot prompting**, **structured output (JSON mode)**, and the **Gemini LLM** to extract meaningful insights from unstructured text in real time.

> 💡 **Note:** This project is intended for educational use and self-reflection. It is **not a substitute for professional mental health support.**

<br>

## 📂 Project Structure

```
📁 Daily-Journal-Analyzer/
│
├── my-genai-capstone-project.ipynb        # The main Jupyter notebook
├── requirements.txt                       # Required Python packages with versions
├── sample_entries.txt                     # Sample journal entries for testing
├── sample_output.json                     # Example output from the model
├── assets/
│   └── banner.png                         # Optional: Banner image for README or LinkedIn
```

<br>

## 🧪 Features
Specifically, this Ai powered assistant will:

- Accept **natural language journal entries** as input  
- Use **few-shot prompting** to guide Gemini’s understanding of emotions  
- Return a **structured JSON response** containing:
  - Overall **mood classification** (e.g., positive, negative, neutral)
  - Detected **emotional tone** (e.g., stressed, content, anxious)
  - Detected **confidence score** and **stress level** (e.g., high, low)
  - Brief analysis of the user's **self awareness**
  - **Important words** related to mood or triggers
  - **Key thought patterns** extracted from the entry
  - **Actionable suggestions** to improve mental well-being in the analysis

The tool demonstrates how **Generative AI** can be used as a supportive mental wellness assistant, even with zero external data and minimal coding effort — making it accessible and practical for real-world use.

<br>

## 🧠 **GenAI Capabilities Used**

This project demonstrates the practical use of multiple Generative AI capabilities, integrated seamlessly using Google’s Gemini API:

| ✅ Capability                     | 💡 How It’s Used                                                                                                       |
|-----------------------------------|------------------------------------------------------------------------------------------------------------------------|
| **Structured Output (JSON Mode)** | The AI returns a consistent, machine-readable JSON response with fields like mood, tone, suggestions, etc.             |
| **Few-shot Prompting**            | Carefully crafted prompt includes example journal entries and expected JSON-format responses.                          |
| **Function Calling (Simulated)**  | The model acts like a callable function: input journal → output structured insights, without defining custom functions.|
| **Long Context Window**           | Gemini can process long journal entries while preserving coherence in the analysis.                                    |

⚠️ Note: While **Embeddings**, **Vector Search**, or **RAG** are not used in this project, the architecture can be extended to include them in future iterations (e.g., tracking mood trends over time).

<br>

## 📌 How to Use

1. **Clone the repository**  
   ```bash
   git clone https://github.com/your-username/daily-journal-analyzer.git
   cd daily-journal-analyzer
   ```

2. **Install dependencies**  
   ```bash
   pip install -r requirements.txt
   ```

3. **Add your Gemini API Key**  
   Store your API key securely using `kaggle_secrets` or environment variables.

4. **Open the notebook**  
   Run `my-genai-capstone-project.ipynb` on [Kaggle Kernels](https://www.kaggle.com/code) or Jupyter.

5. **(Optional)** Uncomment the sample simulation cell to preload journal history and visualize mood trends.

<br>

## 📊 Example Output

```json
{
  "mood": "positive",
  "emotional_tone": "relieved and joyful",
  "stress_level": "low",
  "keywords": ["friends", "relaxed", "social outing"],
  "confidence": 0.92
}
```

<br>

## 🔮 Future Updates

- Personalized coping suggestions based on recurring patterns
- Voice-to-text journaling for accessibility
- Secure cloud storage for cross-device journaling
- Recommendations of mental health resources

<br>

## 📜 License

This project is for educational purposes. All AI analysis is intended to assist with self-reflection and is not professional mental health advice.
