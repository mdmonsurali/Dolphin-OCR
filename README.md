# 🐬 Dolphin OCR - Document Image Parser

A powerful and intuitive Streamlit app that leverages [ByteDance's Dolphin](https://github.com/bytedance/Dolphin) model to extract structured **Markdown**, **JSON**, and **DOCX** content from images and PDFs files.

---
## Demo OCR Video

[Watch Dolphin OCR Demo Video](Demo%20UI/Dolphin%20OCR.mp4)


---

## Demo UI Screenshot

![Demo UI Screenshot](Demo%20UI/Streamlit%20UI%20-1.jpg)



## ✨ Features

- ✅ Extract structured text from **images** and **PDFs** files  
- ✅ Outputs in **Markdown**, **JSON**, and downloadable **.docx** format  
- ✅ Preserves layout including **tables**, **formulas**, **titles**, **headers**, and **paragraphs**  etc
- ✅ Supports **multi-page PDFs** and **Single Image**  
- ✅ Built with **Streamlit** for an interactive and user-friendly UI  

---

## 🛠️ Setup Instructions

### 1. Create and Activate Conda Environment

```bash
conda create -n dolphin python=3.10
conda activate dolphin
```

### 2. Clone This Repository

```bash
git clone git@github.com:mdmonsurali/Dolphin-OCR.git
cd Dolphin-OCR
```

### 3. Install Python Dependencies

```bash
pip install -r requirements.txt
```

### 4. Clone ByteDance Dolphin Model Repository

```bash
git clone https://github.com/bytedance/Dolphin.git
cd Dolphin
pip install -r requirements.txt
```

### 5. Download Pretrained Dolphin Model Weights

```bash
mkdir hf_model
cd hf_model
huggingface-cli download ByteDance/Dolphin --local-dir ./hf_model
cd ..
```

> 💡 Make sure you're logged in to [Hugging Face CLI](https://huggingface.co/docs/huggingface_hub/quick-start#login).

---

## 🚀 Run the Streamlit App

```bash
streamlit run apps.py
```

Open your browser and go to: [http://localhost:8501](http://localhost:8501)

---

## 📂 Supported Input Types

- 🖼️ Image files: `PNG`, `JPG`, `JPEG`  
- 📄 PDF files (single or multi-page) 

---

## 📦 Output Formats

- 📝 **Markdown (.md)** – human-readable structured output  
- 🧾 **JSON (.json)** – structured output for programmatic use  
- 📄 **DOCX (.docx)** – editable Word documents (layout preserved)

---

## 💡 How It Works

1. Upload an image, PDF, or DOCX file in the sidebar  
2. Click **"Extract Text 📄"**  
3. Preview the document and download outputs in Markdown, JSON, or DOCX(Figure, image, table display as it's original format)

Behind the scenes, the app uses:
- [pdf2image](https://pypi.org/project/pdf2image/) to convert PDFs
- [LibreOffice](https://www.libreoffice.org/) to convert DOCX to PDF.(Future works)
- [ByteDance Dolphin](https://github.com/bytedance/Dolphin) for document understanding
- [Streamlit](https://streamlit.io/) for the UI

---

## 🔧 Dependencies

- Python 3.10  
- Streamlit  
- pdf2image  
- python-docx  
- Pillow   
- Hugging Face CLI  

---

## 🙌 Acknowledgements

- 📚 OCR & Layout Model: [ByteDance Dolphin](https://github.com/bytedance/Dolphin)  
- 🤗 Model Hub: [Hugging Face](https://huggingface.co/ByteDance/Dolphin)  
- UI Framework: [Streamlit](https://streamlit.io/)

---

## 📜 License

This project is licensed under the **MIT License**.  
See the [LICENSE](LICENSE) file for more information.

---

## 👨‍💻 Author & Credits

Made with ❤️ by **Md Monsur Ali**

  
## 👤 Author & Links

- 🔗 GitHub: [@mdmonsurali](https://github.com/mdmonsurali)
- 💼 LinkedIn (Author): <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/linkedin/linkedin-original.svg" width="16" style="vertical-align: middle;"> [Md Monsur Ali](https://www.linkedin.com/in/mdmonsurali/)
- 🌐 Website: [inventaai.com](https://inventaai.com/)
- 🏢 LinkedIn (Company): [InventaAI](https://www.linkedin.com/company/inventaai/)


---

## 🌍 Footer

---

Made with Bytedance 🐬 Dolphin Image Parser  
🔗 [GitHub Repo](https://github.com/bytedance/Dolphin) 
Author: Md Monsur Ali | [Website](https://inventaai.com/) | [LinkedIn](https://www.linkedin.com/company/inventaai/) | [GitHub](https://github.com/mdmonsurali) | © 2025
