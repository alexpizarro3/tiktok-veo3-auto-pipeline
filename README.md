# TikTok Veo3 Auto Pipeline

Automated pipeline for scraping, generating, and posting TikTok content using Veo3.

📺 **TikTok + Veo3 Auto Pipeline**

Este proyecto crea un flujo 100% automatizado con **GitHub Actions** para:

- Leer métricas de TikTok (ejemplo: `data/metrics.csv`).
- Analizar resultados y generar prompts inteligentes.
- Crear thumbnails (usando **Gemini Imagen**).
- Generar videos (usando **Gemini/Veo3**).
- (Opcional) Publicar en TikTok con caption + hashtags.

👉 Todo corre en la nube con GitHub Actions, sin depender de tener tu PC encendida.

---

## 🚀 Requisitos previos

- Cuenta en **GitHub** con tu repo clonado en VSCode.
- Cuenta de **TikTok Developer**:
  - Registra tu app en [TikTok for Developers](https://developers.tiktokglobalplatform.com/).
  - Obtén tu **Client Key** y **Client Secret**.
  - Configura un redirect URL válido (ej: tu GitHub Pages `terms.html`).
- Cuenta educativa en **Gemini/Veo3**:
  - Consigue tu **GEMINI_API_KEY** desde [Google AI Studio](https://aistudio.google.com/).
  - Con plan educativo tienes 3 videos gratuitos al día.
- Configura **Secrets en GitHub** (Repo → Settings → Secrets and variables → Actions):
  - `GEMINI_API_KEY` → tu clave de Gemini.
  - `TIKTOK_CLIENT_KEY` → de tu app TikTok.
  - `TIKTOK_CLIENT_SECRET` → de tu app TikTok.
  - `TIKTOK_ACCESS_TOKEN` y `TIKTOK_OPEN_ID` (cuando termines el login flow).

---

## 📂 Estructura del Proyecto

