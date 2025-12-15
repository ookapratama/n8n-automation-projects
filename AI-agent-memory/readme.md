# 🧠 Simple AI Agent & Advanced Prompt Engineering

## 📌 Tujuan Proyek

Proyek ini bertujuan untuk mendemonstrasikan kemampuan saya dalam mengintegrasikan *Large Language Models* (LLM) ke dalam *workflow* otomatis menggunakan n8n, dengan fokus utama pada dua aspek kritis: **Manajemen Memori Percakapan** dan **Desain *System Message* Tingkat Lanjut (Prompt Engineering)**.

### **Workflow yang Dipamerkan:**

1.  **`workflow-Simple-AI-Agent-with-Memory.json`**: Menunjukkan kemampuan agen AI untuk mempertahankan konteks percakapan lintas pesan.
2.  **`workflow-Prompt-Engineering-with-User-Message-and-System-Message.json`**: Menunjukkan cara menginstruksikan LLM (Agen) untuk menjalankan tugas yang sangat spesifik dan terstruktur.

---

## 🛠️ Detail Implementasi & Skill yang Didemonstrasikan

### **1. Workflow: Simple AI Agent with Memory**

* **Fungsi:** Membangun *chatbot* sederhana yang dapat mengingat konteks pesan sebelumnya dalam satu sesi percakapan.
* **Skill Inti:**
    * **State Management:** Menggunakan node **Simple Memory (Buffer Window)** untuk menyimpan riwayat percakapan.
    * **Agent Orchestration:** Menghubungkan node **AI Agent** dengan *Language Model* (Gemini) dan *Memory* agar agen dapat merujuk pada pesan masa lalu.
    * **System Message Dasar:** Mengatur *System Message* dasar ("You are a helpful assistant who remember past conversations...") untuk menentukan persona agen.

### **2. Workflow: Advanced Prompt Engineering (Keyword Extractor)**

* **Fungsi:** Mengubah LLM menjadi Agen *Keyword Extraction* yang sangat spesifik untuk domain Machine Learning (ML).
* **Skill Inti:**
    * **Structured Prompting:** Merancang *System Message* yang detail dan terstruktur dengan bagian **Overview, Context, Instructions, Exclusion, Phrase Recognition, Format, Examples, dan SOP**.
    * **Output Consistency:** Memaksa model untuk memberikan *output* dalam format yang sangat spesifik (daftar terpisah koma tanpa teks pembuka).
    * **Input Handling:** Menerima input teks deskriptif dari *Form Trigger*, memprosesnya melalui node **Set**, dan menggunakannya sebagai *User Message* ("Extract keywords from this paragraph...").
    * **Task Reliability:** Mendemonstrasikan bagaimana *Prompt Engineering* yang tepat menghasilkan *output* yang bersih dan relevan untuk pemrosesan data hilir (misalnya, *tagging* atau *indexing*).

---

## 📈 Dampak dan Nilai Jual

Proyek ini menunjukkan pemahaman saya yang kuat dalam:

* **Arsitektur Agen AI:** Mampu menyusun agen yang terdiri dari LLM, Memori, dan logika.
* **Keandalan LLM:** Mampu merekayasa *prompt* untuk mengurangi *hallucination* dan meningkatkan keandalan *output* untuk tugas *backend* otomatis.
* **Integrasi Multi-Model:** Meskipun tidak semua terhubung, *workflow* pertama menunjukkan eksplorasi dan potensi integrasi dengan berbagai penyedia LLM (Gemini, DeepSeek, OpenAI).

---


## 🖼️ Visualisasi Alur Kerja

#### Simple AI Agent
![Visualisasi Flow AI Agent with Memory](https://github.com/ookapratama/n8n-automation-projects/blob/main/AI-agent-memory/screenshot/simple-ai-agent.png)

![Visualisasi Flow AI Agent with Memory](https://github.com/ookapratama/n8n-automation-projects/blob/main/AI-agent-memory/screenshot/result/simple-ai-agent.png)

#### Prompt Engineering
![Visualisasi Prompt Engineering with User message and System Message](https://github.com/ookapratama/n8n-automation-projects/blob/main/AI-agent-memory/screenshot/prompt-engineering.png)
![Visualisasi Prompt Engineering with User message and System Message](https://github.com/ookapratama/n8n-automation-projects/blob/main/AI-agent-memory/screenshot/result/prompt-engineering.png)


---
### ⚠️ Keterangan Kredensial

*Semua file `workflow.json` ini hanya berisi ID referensi dan telah di-*scrub*. Kredensial LLM harus dikonfigurasi pada *instance* n8n pribadi Anda.*

<!-- ---

## 📸 Panduan Screenshot yang Perlu Disertakan

Anda **pasti perlu** menyertakan *screenshot*. Dalam proyek otomatisasi visual seperti n8n, *screenshot* adalah cara terbaik untuk menunjukkan kompleksitas logika Anda.

Sertakan tiga tangkapan layar utama di folder Anda, dengan nama yang disarankan:

| Nama File Gambar | Apa yang Harus Di-*Screenshot* | 
| :--- | :--- | 
| **`workflow-visual-memory.png`** | Seluruh alur kerja `workflow-Simple-AI-Agent-with-Memory.json` (Trigger -> AI Agent -> Memory -> LM). | Menunjukkan bagaimana Anda menghubungkan node Memori ke Agen, membuktikan *skill* State Management. |
| **`workflow-visual-extractor.png`** | Seluruh alur kerja `workflow-Prompt-Engineering-with-User-Message-and-System-Message.json` (Form Trigger -> Set -> AI Agent -> Set). | Menunjukkan *pipeline* data dari *input* ke *output* dan bagaimana Anda mengemas fungsi agen. |
| **`system-message-detail.png`** | Buka node **AI Agent** pada *workflow* kedua, dan ambil tangkapan layar yang menunjukkan **semua detail *System Message*** (Overview, Context, Instructions, Examples, SOP). | **Ini sangat penting.** Ini adalah bukti kuat dari *skill Prompt Engineering* tingkat lanjut Anda, yang membedakan Anda dari pengguna LLM biasa. | -->