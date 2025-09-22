Atualiza README com informações do projeto
# 🎶 Chord Finder App

Aplicativo **Flutter + FastAPI** para **análise e extração automática de acordes musicais** a partir de arquivos de áudio.

---

## 🚀 Tecnologias usadas
- [Flutter](https://flutter.dev/) — app mobile (Android/iOS)
- [FastAPI](https://fastapi.tiangolo.com/) — API em Python para processamento de áudio
- [Librosa](https://librosa.org/doc/latest/index.html) — extração de cromas e features musicais
- [Essentia](https://essentia.upf.edu/) *(opcional, futuro)*

---

## 📱 Funcionalidades (MVP)
- Upload de arquivos MP3/WAV
- Retorno de sequência de acordes (C, G, Am, F…)
- Detecção simples de tom (key)
- Exportação futura em **ChordPro** e **PDF**

---

## 🛠 Como rodar localmente

### Back-end (FastAPI)
```bash
cd api
python -m venv .venv
source .venv/bin/activate   # Windows: .venv\Scripts\activate
pip install -r requirements.txt
uvicorn main:app --reload
cd chords_app
flutter pub get
flutter run
chord-finder-app/
 ├─ api/              # Back-end FastAPI
 │   ├─ main.py
 │   ├─ chordify.py
 │   └─ requirements.txt
 ├─ chords_app/       # App Flutter
 │   └─ lib/main.dart
 ├─ README.md
 ├─ LICENSE
 └─ .gitignore
## 📌 Roadmap
- [ ] Versão inicial com acordes maiores/menores
- [ ] Exportação em ChordPro
- [ ] Integração com Spotify/YouTube (legalidade em análise)
- [ ] Interface amigável para músicos iniciantes
## 👤 Autor
- Peu Pereira  
- 🔗 [LinkedIn](https://www.linkedin.com)  
- 🔗 [Instagram](https://www.instagram.com)
