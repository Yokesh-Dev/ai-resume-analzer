# 🧠 AI Resume Analyzer

An intelligent **AI-powered resume analysis web app** built with **React, Tailwind CSS, and Vite**.  
This app allows users to **upload their resume in PDF format** and receive an **instant, AI-driven evaluation** — scoring content quality, formatting, keyword usage, and ATS (Applicant Tracking System) compatibility.  

---

## 🚀 Features

- 📄 **PDF Upload Support** — upload and extract text from your resume.
- 🤖 **AI-Powered Resume Analysis** — evaluates your resume using GPT-based reasoning.
- 🧩 **Comprehensive Feedback** — includes overall score, strengths, improvements, and pro tips.
- ⚙️ **ATS Compatibility Checker** — ensures your resume passes automated HR filters.
- 🎯 **Actionable Recommendations** — provides action items and relevant keywords to improve your resume.
- 💅 **Modern UI/UX** — built with TailwindCSS for a clean, responsive design.

---

## 🛠️ Tech Stack

| Category | Technologies |
|-----------|---------------|
| Frontend | React 19, Vite |
| Styling | Tailwind CSS |
| AI Integration | [Puter.ai](https://puter.com) API (for chat and analysis) |
| PDF Parsing | pdfjs-dist |
| Linting | ESLint |

---

## 🧩 Project Structure

```

ai_resume_starter_code/
├── index.html
├── src/
│   ├── App.jsx
│   ├── constants.js
│   ├── main.jsx
│   └── styles.css
├── package.json
└── tailwind.config.js

````

---

## ⚡ Getting Started

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/yourusername/ai-resume-analyzer.git
cd ai-resume-analyzer
````

### 2️⃣ Install Dependencies

```bash
npm install
```

### 3️⃣ Run the Development Server

```bash
npm run dev
```

Then open your browser and navigate to **[http://localhost:5173](http://localhost:5173)** (or the port shown in your terminal).

---

## 📚 Usage

1. Click **“Choose PDF File”** to upload your resume.
2. The app extracts text using **pdfjs-dist**.
3. The resume is analyzed through **Puter.ai’s GPT model**.
4. You’ll see a detailed breakdown including:

   * Overall score
   * Strengths and improvements
   * Action items & professional tips
   * ATS optimization checklist
   * Recommended keywords

---

## 🧠 How It Works

* The core prompt logic is defined in **`constants.js`** (`ANALYZE_RESUME_PROMPT`).
* Once a PDF is uploaded, text is extracted, and the AI model is queried.
* The JSON response is parsed and rendered into user-friendly dashboards.

---

## 🎨 Styling

All UI components are styled with **Tailwind CSS**, including:

* Gradient backgrounds
* Status color coding (excellent / good / needs improvement)
* Responsive cards and progress bars
* Interactive hover and transition effects

---

## 🧾 Example Output

```json
{
  "overallScore": "8/10",
  "strengths": ["Strong formatting", "Relevant skills section", "Quantified achievements"],
  "improvements": ["Add more industry keywords", "Simplify layout for ATS", "Expand education details"],
  "keywords": ["React", "JavaScript", "Node.js"],
  "summary": "A well-structured and concise resume with strong technical focus.",
  "performanceMetrics": {
    "formatting": 9,
    "contentQuality": 8,
    "keywordUsage": 7,
    "atsCompatibility": 8,
    "quantifiableAchievements": 8
  }
}
```

---

## 🧑‍💻 Developer Notes

* Uses **Puter.ai’s `window.puter.ai.chat`** for GPT-powered responses.
* The default model is `gpt-5-nano`, but this can be replaced with other models.
* PDF extraction is handled asynchronously via `pdfjs-dist`.

---

## 📦 Build for Production

```bash
npm run build
```

This generates a production-optimized build in the `dist/` directory.

---

## 🪪 License

This project is open source under the **MIT License**.
Feel free to use, modify, and distribute it.

---

## 💬 Acknowledgments

Special thanks to:

* **Puter.ai** for their AI API integration
* **TailwindCSS** for the beautiful and efficient design system
* **pdfjs-dist** for robust PDF parsing

That would make it even more professional for a public GitHub repository.
```
