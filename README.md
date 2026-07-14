# Minutes of Meeting Generator

Automatically generate professional meeting minutes from audio recordings using AI.

This project uses OpenAI's **Whisper** model to transcribe meeting audio and **Meta Llama 3.2-3B Instruct** to transform the transcript into structured meeting minutes containing summaries, discussion points, takeaways, and action items.

---

## Features

- Transcribes meeting audio into text using Whisper
- Generates structured meeting minutes using Llama 3.2
- Produces:
  - Meeting summary
  - Attendees
  - Discussion points
  - Key takeaways
  - Action items with owners
- Outputs clean Markdown for easy sharing and documentation

---

## Tech Stack

- Python
- Hugging Face Transformers
- Whisper (`openai/whisper-medium.en`)
- Meta Llama 3.2-3B Instruct
- PyTorch
- BitsAndBytes (4-bit quantization)
- Google Colab

---

## 📂 Project Workflow

```
Meeting Audio (.mp3)
          │
          ▼
 Whisper Speech-to-Text
          │
          ▼
     Transcript
          │
          ▼
 Llama 3.2-3B Instruct
          │
          ▼
 Structured Meeting Minutes
```

## 📚 Models Used

| Task | Model |
|------|-------|
| Speech-to-Text | `openai/whisper-medium.en` |
| Meeting Minutes Generation | `meta-llama/Llama-3.2-3B-Instruct` |

---
