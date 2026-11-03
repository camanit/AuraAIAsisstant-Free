# Privacy Policy — Aura AI Assistant

**Effective Date:** November 3, 2026  
**Extension Name:** Aura AI Assistant — Web, Voice & Meeting Copilot

---

## 1. Overview (Ringkasan Privasi)
**Aura AI Assistant** ("we", "our", or "the Extension") is committed to protecting your privacy. The Extension is designed with a **Local-First & Zero-Tracking Architecture**:
- We **do not** collect, store, sell, or share your personal data, browsing history, or API keys on any external servers owned by us.
- All user preferences and API keys are stored strictly on your own device using Chrome's isolated local storage (`chrome.storage.local`).

---

## 2. Data We Process & How It Is Used

### A. Web Page Content & Selected Text
- **When it is accessed:** Only when you explicitly trigger an action inside the Aura AI Side Panel or Context Menu (e.g., clicking *Summarize*, *Translate*, *Smart Reply*, or *Live Analysis*).
- **How it is used:** The extracted text from the active tab is sent directly from your browser to your selected AI/Translation provider (Google Gemini API, OpenAI API, Groq API, or Google Translate endpoint) solely to generate the requested summary, translation, or reply.
- **No background harvesting:** The Extension never reads or transmits web page content in the background without your explicit interaction.

### B. API Keys & User Settings (`storage` Permission)
- Your AI Provider API Key, selected language, and theme preferences are saved locally in `chrome.storage.local`.
- Your API Key is only transmitted in the `Authorization` or query header directly to the official AI provider endpoint (`generativelanguage.googleapis.com`, `api.openai.com`, or `api.groq.com`).

### C. Voice Input (Speech-to-Text) & Audio Output (Text-to-Speech)
- Voice recognition and speech synthesis use your browser's native **Web Speech API** (`webkitSpeechRecognition` and `window.speechSynthesis`).
- Microphone listening is only activated when you explicitly click the **🎙️ Speak (Mic)** button and stops immediately when your command finishes or when you stop it.

---

## 3. Permissions Justification (Chrome Web Store Compliance)
- **`activeTab` & `tabs`:** To detect the active tab platform (e.g., GitHub, LinkedIn, Zoom Web, Google Meet, YouTube Live) and update the Side Panel context badge.
- **`scripting` & `<all_urls>`:** To extract readable article text, live captions, or insert user-selected smart replies into comment/chat boxes when explicitly clicked by the user.
- **`sidePanel`:** To display the persistent Aura AI Assistant copilot interface alongside your active tab.
- **`storage`:** To save your language, theme, and encrypted local API key settings.
- **`contextMenus`:** To provide right-click shortcuts (*Summarize / Translate / Smart Reply*) on highlighted text.

---

## 4. Third-Party Services
When you initiate an AI or translation action, the text snippet you selected is processed by the provider you configured:
- [Google Gemini Privacy Policy](https://policies.google.com/privacy)
- [OpenAI Privacy Policy](https://openai.com/policies/privacy-policy)
- [Groq Privacy Policy](https://groq.com/privacy-policy/)

---

## 5. Contact
If you have any questions about this Privacy Policy, please contact the developer via the official GitHub repository or Chrome Web Store support tab.

