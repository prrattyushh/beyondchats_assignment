# 🧠 Reddit Persona Generator

Generate detailed, structured user personas from any public Reddit profile using Large Language Models (LLMs).  
Inspired by the Lucas Mellor UX-style format, this tool transforms Reddit comments and posts into well-cited, personality-rich personas — ideal for product designers, researchers, marketers, and content strategists.

---

## 🚀 Features

- 🔍 Scrapes public Reddit posts and comments using `praw`
- 🤖 Generates high-quality user personas using LLMs via [OpenRouter](https://openrouter.ai)
- 💬 Supports quote-based citations for each trait
- 📈 Persona includes:
  - Identity (Name, Age, Occupation, Location, Archetype)
  - Personality sliders with visual bars
  - Motivations, behaviors, frustrations, goals
  - A hero quote
  - Topics discussed
  - Summary
- 💾 Saves persona as a Markdown file (`<username>_persona.md`)
- ✅ Resilient: handles API timeouts, retry logic, and prompt cutoffs

---

## 🧩 Persona Format

Example sections:

### 👤 Identity
- Name: Rohan Verma
- Age Range: 22–28
- Occupation: QA Engineer
- Archetype: The Meme Philosopher

### 🧭 Personality Sliders
```
Introvert ↔ Extrovert: ▓▓▓░░░ (40%)
"Mostly comments and avoids long threads."
```

### 🎯 Motivations
- Learning ▓▓▓▓▓▓░░ (80%) — “How do I automate using Appium?”
- Recognition ▓▓▓▓░░░ (60%) — “My cake day!”

### 🌀 Behaviours
- Shares memes and watches — “Damn the blue dial looks clean!”
- Casual replies — “Mai b mast, tu bata?”

### 😤 Frustrations
- “Procrastination ki hadd h yr!”
- “CSGO not launching after update!”

---

## 🛠️ How to Use

### 1. Install dependencies

```bash
pip install praw requests
```

### 2. Set your OpenRouter API Key

Open the script or notebook and replace:

```python
OPENROUTER_API_KEY = "sk-or-v1-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
```

### 3. Run the script or notebook

- For script:
```bash
python reddit_persona_generator.py
```

- For notebook:
```bash
jupyter notebook Reddit_Persona_Generator.ipynb
```

### 4. Enter a Reddit username

You'll be prompted:

```
Enter Reddit username: loudtype
```

---

## 📁 Output

- Output is saved as a markdown file:
  ```
  loudtype_persona.md
  ```

You can convert this `.md` file to:
- PDF (via VSCode export or Pandoc)
- HTML (for styled output)
- Notion (copy-paste)
- Slide decks or design docs

---

## 💡 Use Cases

- 🧪 UX Research and Empathy Mapping
- 📢 Content & Marketing Persona Building
- 🎮 Game/Story Character Design
- 📊 Product Segmentation Analysis
- 🔍 Subculture Understanding

---

## 🧱 Built With

- [PRAW](https://praw.readthedocs.io/) - Reddit API client
- [OpenRouter](https://openrouter.ai) - Unified API for open LLMs
- Mistral / LLAMA3-70B - AI model for persona generation

---

## 📜 License

MIT License. Use it, remix it, and improve it — attribution appreciated.

---

## ✨ Acknowledgements

- Lucas Mellor’s persona layout for inspiration  
- Redditors whose voices helped shape better personas  
- OpenRouter and Meta LLaMA/Mistral for LLM power  
```

---
