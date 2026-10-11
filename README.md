# Hi, I'm Ayham 👋

**AI/ML Engineer · Document AI · Computer Vision · LLMs & Agents**

I build production AI systems end to end: VLM extraction, golden-set annotation, LoRA/QLoRA fine-tuning
and vLLM serving on an NVIDIA DGX Spark, per-field evaluation in W&B, all shipped behind tested,
containerised FastAPI services. I work in Arabic and English, from Aleppo, Syria.

### 🔧 What I've built

- **Document AI for Arabic work orders:** a spec-driven engine that turns image-only Arabic PDFs into typed JSON.
  One catalog of **123 fields across 31 document types** generates every prompt and schema, at **5–6 VLM calls
  per 5-page document**. A golden set of **183 reviewed documents** feeds Qwen3.5-VL (4B/9B) LoRA/QLoRA
  fine-tuning, with adapters served by vLLM. Runs as 8 Docker services with **1,130 tests** that need no GPU or API key.
- **Real-time PPE compliance monitoring:** YOLO26 pose finds each worker, then a fine-tuned YOLO26 PPE detector checks
  the crop. A tri-state machine (compliant / violation / indeterminate) confirms violations, and InsightFace re-ID names
  violators. Handles live RTSP and WebSocket streams with flat latency, and exports NMS-free ONNX.
- **Inspection-rule extraction from engineering standards:** multi-pass VLM extraction as Temporal workflows that turns
  standards into citation-backed yes/no rules, with every quote string-matched against its source page.
- **Multi-agent guest operations copilot:** 5 Google ADK agents inside a durable Temporal workflow, with human approval
  and a deterministic safety gate that can only make outcomes stricter.
- **Fully local Text-to-SQL RAG:** Arabic/English questions over Oracle 19c with a local Qwen, LlamaIndex and Qdrant.
  No data leaves the server.
- **SAM 3 auto-labeller:** a text prompt turns a folder of images into a ready YOLO dataset, as a PyQt6 desktop app
  or a Dockerised web app.

### 🧰 Stack

**LLMs & VLMs:** Qwen3.5-VL · Gemini · Unsloth (LoRA/QLoRA) · vLLM · Google ADK · LiteLLM · LlamaIndex · Qdrant  
**Computer vision:** YOLO26 · InsightFace · SAM 3 · OWLv2 · GeoCalib · OpenCV · ONNX  
**Backend & infra:** Python · FastAPI · Celery · Temporal · PostgreSQL · Redis · Docker · W&B · DGX Spark (GB10)

### 📫 Reach me

[LinkedIn](https://www.linkedin.com/in/ayham-ayan-02bba1203) · mayhamayan748@gmail.com · Open to remote AI/ML roles
