---
name: "TrOCR multiline Docker API"
status: "shipped"
github: "https://github.com/Atyab124/Full-page-docker-TrOCR-Completebuild-v2"
---

# TrOCR multiline API on Docker

- What it is: a GPU-accelerated handwriting/multiline OCR API, containerized, with a Gradio demo UI
- Role: solo build
- Stack: Docker (GPU support, nvidia-container-toolkit), Flask API, TrOCR model, Gradio for the visual demo, Python 3.9
- Notable: serves live at `localhost:8080/hand_OCR` once running; an alternate API mode returns bounding-box coordinates alongside text, toggled by a one-line Dockerfile edit. `Completebuild_OG` (github.com/Atyab124/Completebuild_OG) is the original version this v2 superseded — same core, kept as history rather than deleted.
- Real numbers: 2 GitHub stars
