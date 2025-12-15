# 📄 Automated Text Summarizer (Dual Trigger)

## 📌 Tujuan Proyek

Membangun *workflow* otomatis yang memanfaatkan *Large Language Model* (LLM) untuk meringkas teks panjang (seperti artikel atau dokumen) dan mengirimkan hasilnya melalui email.

Proyek ini menyoroti fleksibilitas eksekusi dengan menyediakan **dua mekanisme *trigger*** yang berbeda: *On Schedule* (untuk tugas berulang) dan *On Form Submission* (untuk tugas *ad-hoc*).

---

## 🛠️ Detail Implementasi & Skill yang Didemonstrasikan

| Komponen | Fungsionalitas |
| :--- | :--- |
| **Dual Trigger Mechanism** | 1. **Cron Node:** Untuk menjalankan ringkasan konten dari sumber tertentu pada waktu yang terjadwal. <br> 2. **Form Trigger:** Memungkinkan pengguna untuk menempelkan teks atau tautan dokumen yang ingin diringkas kapan saja. |
| **Core AI Task** | Menggunakan node **AI Agent** atau **Chat Model** (misalnya, Google Gemini atau OpenAI) dengan *prompt* spesifik untuk menghasilkan ringkasan yang ringkas dan akurat. |
| **Prompt Engineering** | Merancang *System Message* yang menginstruksikan LLM untuk meringkas dalam format yang diminta (*e.g.*, *bullet points*, fokus pada *key takeaway*). |
| **Backend Communication** | Node **Email (Gmail)** digunakan untuk mengirimkan hasil ringkasan ke alamat email penerima. |
<!-- | **Data Flow Logic** | Menggunakan node **IF** atau **Merge** untuk memastikan *workflow* dapat memproses *input* data yang datang dari salah satu dari dua *trigger* (Cron atau Form) secara mulus. | -->

### 🔑 Kredensial yang Dibutuhkan

* Kredensial **LLM/AI** (OpenAI, Gemini, atau lainnya).
* Kredensial **SMTP/Email Service** (untuk mengirim email).

> **Penting:** File `workflow.json` ini hanya berisi ID referensi. Kredensial harus dikonfigurasi di *instance* n8n pribadi Anda.

---

## 📈 Dampak dan Nilai Jual

Proyek ini menunjukkan pemahaman saya yang kuat dalam:

1.  **System Design Fleksibel:** Kemampuan untuk merancang *workflow* yang melayani kebutuhan *push* (terjadwal) dan *pull* (berdasarkan permintaan/form).
2.  **AI for Business Efficiency:** Mampu mengaplikasikan AI untuk memecahkan masalah umum kantor (*information overload*) dan menyalurkan hasilnya langsung melalui saluran komunikasi yang umum (Email).
3.  **End-to-End Automation:** Mendemonstrasikan seluruh rantai otomatisasi, dari *input trigger* hingga *final action* (notifikasi).

## 🖼️ Visualisasi Alur Kerja

**(Anda harus memasukkan gambar-gambar ini di folder ini)**

* ![Visualisasi Flow Summarizer](https://github.com/ookapratama/n8n-automation-projects/blob/main/automated-text-summarizer/screenshot/workflow.png)
* ![Screenshot Email Content](https://github.com/ookapratama/n8n-automation-projects/blob/main/automated-text-summarizer/screenshot/result.png)

---

<!-- ### 📸 Panduan Screenshot yang Perlu Disertakan

Pastikan Anda menyertakan dua gambar berikut di folder ini:

1.  **`workflow-visual-summarizer.png`**: Tangkapan layar seluruh *workflow*, pastikan terlihat jelas adanya **dua jalur *trigger*** (Cron dan Form) yang bertemu sebelum node AI dan Email.
2.  **`email-content-preview.png`**: Tangkapan layar dari pratinjau data pada node **Email** yang menunjukkan hasil ringkasan LLM telah disisipkan dengan rapi di badan email. -->