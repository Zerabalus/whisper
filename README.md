# 🎤 Transcripción de video de YouTube con Whisper (GPU) - Google Colab

<div align="center">
  
| <img src="https://i.pinimg.com/736x/58/03/ba/5803ba1d80ef1a52e660124eb9f471f9.jpg"> | **Acelerado por GPU** ☄️<br>Transcribe videos de YouTube usando OpenAI Whisper |
|-----------------------------------------------------------------------------|--------------------------------------------------------------------------------|

</div>

## 👩🏻‍💻 Cómo Empezar
1. **Abre el Notebook**:  
   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1FxsjSRuwrMh5aFsNQWfzgwFE-gqHaD04?usp=sharing)
2. **Conecta GPU**:  
   `Runtime > Change runtime type > T4 GPU`
3. **Ejecuta todas las celdas** (`Ctrl+F9`)

## 📌 Pasos (Colab)
```python
# 1. Instalación (ejecutar estas celdas primero)
!pip install openai-whisper
!pip insatll yt-dlp

# 2. Pegar URL de YouTube
youtube_url = "https://youtu.be/ejemplo"  # ← Cambiar aquí

# 3. Transcribir (automáticamente usa GPU)
model = whisper.load_model("medium")  # cambiar entre base, medium, small etc.
